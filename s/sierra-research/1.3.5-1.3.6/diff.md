# Comparing `tmp/sierra-research-1.3.5.tar.gz` & `tmp/sierra-research-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierra-research-1.3.5.tar", last modified: Thu Jun  8 03:06:36 2023, max compression
+gzip compressed data, was "sierra-research-1.3.6.tar", last modified: Mon Apr  1 09:27:59 2024, max compression
```

## Comparing `sierra-research-1.3.5.tar` & `sierra-research-1.3.6.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.coveragerc
--rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.dir-locals.el
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/publish/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/publish/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/sample-project-setup/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/sample-project-setup/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/sierra-setup/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/sierra-setup/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/slurm-setup/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/slurm-setup/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/argos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/exec-env-plugins.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/integration-all.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/ros1gazebo.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/ros1robot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/sierra-core.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/unit-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.projectile
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.pylintrc
--rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 03:03:32.000000 sierra-research-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-08 03:06:36.557962 sierra-research-1.3.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    14452 2023-06-08 03:03:32.000000 sierra-research-1.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    54227 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-cli.1
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-examples.7
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-exec-envs.7
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-glossary.7
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-platforms.7
--rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-usage.7
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra.7
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/_ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/_ext/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/_templates/autoapi/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/_templates/autoapi/module.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   175198 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/figures/architecture.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2632 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-exec-envs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-platforms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-usage.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      154 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/exec_env/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7330 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/exec_env/hpc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/exec_env/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/exec_env/robot.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8755 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/faq.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     7274 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/getting_started.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    10817 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/matrix.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/packages.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/philosophy.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/argos/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4659 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/argos/batch_criteria.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/argos/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/ros1gazebo/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1gazebo/batch_criteria.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1gazebo/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/ros1robot/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1robot/batch_criteria.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1robot/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/plugins/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/roadmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/storage/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8787 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/trial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/hpc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/hpc/cluster_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/hpc/local_setup.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/docs/src/tutorials/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/cmdline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/plugin/storage/
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/storage/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/storage/plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/docs/src/tutorials/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/cmdline.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2964 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/generators.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     6370 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/graphs_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/hooks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/docs/src/tutorials/project/main_config/
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/controllers.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/main.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/perf.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/models.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/new_bc.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/project.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/stage5_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/template_input_file.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/docs/src/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-argos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-ros1gazebo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-ros1robot.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      691 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4608 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/examples.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4439 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/pipeline.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     6039 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/rendering.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8617 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/run_time_tree.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/stage5.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/subprograms.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/variables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-08 03:03:32.000000 sierra-research-1.3.5/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    26821 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/argos-integration-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/core-integration-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     8637 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/ros1gazebo-integration-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4192 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/ros1robot-integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/slurm-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/slurm.conf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:06:36.557962 sierra-research-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-08 03:03:32.000000 sierra-research-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/sierra/
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58191 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/cmdline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/bindings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11458 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/definition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/generators/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/controller_generator_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15596 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/exp_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5574 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/exp_generators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8919 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/generator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/graphs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12218 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/heatmap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3685 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/scatterplot2D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9125 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/stacked_line_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8125 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/stacked_surface_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13573 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/summary_line_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/hpc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5186 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/hpc/cmdline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3330 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/models/graphs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/models/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/pipeline/
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7487 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage1/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage1/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage1/pipeline_stage1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage2/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage2/exp_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage2/pipeline_stage2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5094 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/imagizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4572 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/pipeline_stage3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12585 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/run_collator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18186 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/statistics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage4/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12042 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/graph_collator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9591 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/inter_exp_graph_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13814 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/intra_exp_graph_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6745 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/model_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18911 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/pipeline_stage4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9385 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/rendering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/yaml_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage5/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14183 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/inter_scenario_comparator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43936 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/intra_scenario_comparator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10600 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/pipeline_stage5.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12535 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/plugin_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8173 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/root_dirpath_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/ros1/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/ros1/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/variables/exp_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/startup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6030 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/stat_kernels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12471 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/variables/
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/base_variable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25747 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/batch_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/exp_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/population_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/variable_density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3843 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/vector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6618 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/adhoc/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/adhoc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4046 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/adhoc/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/local/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/local/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/local/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/pbs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3858 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/pbs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/slurm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4164 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/slurm/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/argos/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15855 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/argos/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/generators/platform_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6062 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/arena_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9031 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/cameras.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4618 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/constant_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/exp_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19636 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/physics_engines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_constant_density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4967 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_variable_density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9920 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8463 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/population_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6972 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/platform_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/population_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/robot/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/robot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/storage/csv/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/storage/csv/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/storage/csv/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra_research.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/arena_extent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/exp_def_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/test1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/vector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-08 03:03:32.000000 sierra-research-1.3.5/todo.org
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.130452 sierra-research-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.coveragerc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.dir-locals.el
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.074452 sierra-research-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.074452 sierra-research-1.3.6/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.086452 sierra-research-1.3.6/.github/actions/publish/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/actions/publish/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.086452 sierra-research-1.3.6/.github/actions/sample-project-setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/actions/sample-project-setup/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.086452 sierra-research-1.3.6/.github/actions/sierra-setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/actions/sierra-setup/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.086452 sierra-research-1.3.6/.github/actions/slurm-setup/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/actions/slurm-setup/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.086452 sierra-research-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/argos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/exec-env-plugins.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/integration-all.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/ros1gazebo.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/ros1robot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/sierra-core.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.github/workflows/unit-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.projectile
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.pylintrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-01 09:25:50.000000 sierra-research-1.3.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 09:25:50.000000 sierra-research-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16925 2024-04-01 09:27:59.130452 sierra-research-1.3.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14480 2024-04-01 09:25:50.000000 sierra-research-1.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.090452 sierra-research-1.3.6/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      604 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.074452 sierra-research-1.3.6/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.090452 sierra-research-1.3.6/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (127)    54484 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra-cli.1
+-rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra-examples.7
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra-exec-envs.7
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra-glossary.7
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra-platforms.7
+-rw-r--r--   0 runner    (1001) docker     (127)    24725 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra-usage.7
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-01 09:27:36.000000 sierra-research-1.3.6/docs/_build/man/sierra.7
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.090452 sierra-research-1.3.6/docs/_ext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/_ext/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.074452 sierra-research-1.3.6/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.090452 sierra-research-1.3.6/docs/_templates/autoapi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/_templates/autoapi/module.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11594 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.090452 sierra-research-1.3.6/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   175198 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/figures/architecture.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2632 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.094452 sierra-research-1.3.6/docs/man/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      897 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra-examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra-exec-envs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra-glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra-platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra-usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1493 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/man/sierra.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      156 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.094452 sierra-research-1.3.6/docs/src/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      156 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2990 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.094452 sierra-research-1.3.6/docs/src/exec_env/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7330 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/exec_env/hpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/exec_env/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1284 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/exec_env/robot.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8755 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/faq.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7274 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/getting_started.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10819 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/matrix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/packages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/philosophy.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.094452 sierra-research-1.3.6/docs/src/platform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.094452 sierra-research-1.3.6/docs/src/platform/argos/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4659 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/argos/batch_criteria.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/argos/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/platform/ros1gazebo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/ros1gazebo/batch_criteria.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/ros1gazebo/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/platform/ros1robot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/ros1robot/batch_criteria.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/platform/ros1robot/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/plugins/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/roadmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/storage/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8781 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/trial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/tutorials/hpc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2277 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/hpc/cluster_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/hpc/local_setup.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      948 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.078452 sierra-research-1.3.6/docs/src/tutorials/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/tutorials/plugin/exec_env/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1480 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/exec_env/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/exec_env/plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/tutorials/plugin/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/platform/cmdline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/platform/generators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/platform/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/platform/plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.098452 sierra-research-1.3.6/docs/src/tutorials/plugin/storage/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/storage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/plugin/storage/plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.102452 sierra-research-1.3.6/docs/src/tutorials/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/cmdline.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2964 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/generators.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6370 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/graphs_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/hooks.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.102452 sierra-research-1.3.6/docs/src/tutorials/project/main_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/main_config/controllers.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      496 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/main_config/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/main_config/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/main_config/perf.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/models.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5688 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/new_bc.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6362 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/stage5_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/tutorials/project/template_input_file.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.102452 sierra-research-1.3.6/docs/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/cli-argos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/cli-core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/cli-ros1gazebo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/cli-ros1robot.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      691 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4608 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/environment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/examples.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      699 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4439 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/pipeline.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6039 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/rendering.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8617 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/run_time_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/stage5.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      897 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/subprograms.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1795 2024-04-01 09:25:50.000000 sierra-research-1.3.6/docs/src/usage/variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-01 09:25:50.000000 sierra-research-1.3.6/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.106452 sierra-research-1.3.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26821 2024-04-01 09:25:50.000000 sierra-research-1.3.6/scripts/argos-integration-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4951 2024-04-01 09:25:50.000000 sierra-research-1.3.6/scripts/core-integration-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8637 2024-04-01 09:25:50.000000 sierra-research-1.3.6/scripts/ros1gazebo-integration-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4192 2024-04-01 09:25:50.000000 sierra-research-1.3.6/scripts/ros1robot-integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 09:25:50.000000 sierra-research-1.3.6/scripts/slurm-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-01 09:25:50.000000 sierra-research-1.3.6/scripts/slurm.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:27:59.130452 sierra-research-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-01 09:25:50.000000 sierra-research-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.106452 sierra-research-1.3.6/sierra/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.106452 sierra-research-1.3.6/sierra/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58191 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/cmdline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4562 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.110452 sierra-research-1.3.6/sierra/core/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/experiment/bindings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11458 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/experiment/definition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6950 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/experiment/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/experiment/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.110452 sierra-research-1.3.6/sierra/core/generators/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/generators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      873 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/generators/controller_generator_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15596 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/generators/exp_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5574 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/generators/exp_generators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8919 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/generators/generator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.110452 sierra-research-1.3.6/sierra/core/graphs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/graphs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12218 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/graphs/heatmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3685 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/graphs/scatterplot2D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9125 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/graphs/stacked_line_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8125 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/graphs/stacked_surface_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13573 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/graphs/summary_line_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.110452 sierra-research-1.3.6/sierra/core/hpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/hpc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5186 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/hpc/cmdline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      985 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.110452 sierra-research-1.3.6/sierra/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3330 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/models/graphs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6729 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/models/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.114452 sierra-research-1.3.6/sierra/core/pipeline/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7487 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.114452 sierra-research-1.3.6/sierra/core/pipeline/stage1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage1/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3304 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage1/pipeline_stage1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.114452 sierra-research-1.3.6/sierra/core/pipeline/stage2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10734 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage2/exp_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage2/pipeline_stage2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.114452 sierra-research-1.3.6/sierra/core/pipeline/stage3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5094 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage3/imagizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4572 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage3/pipeline_stage3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12585 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage3/run_collator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18186 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage3/statistics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.114452 sierra-research-1.3.6/sierra/core/pipeline/stage4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12042 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/graph_collator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9591 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/inter_exp_graph_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13814 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/intra_exp_graph_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6745 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/model_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18911 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/pipeline_stage4.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9385 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/rendering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3486 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage4/yaml_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/core/pipeline/stage5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage5/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14183 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage5/inter_scenario_comparator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43936 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage5/intra_scenario_comparator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10600 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/pipeline/stage5/pipeline_stage5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12535 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/plugin_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8173 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/root_dirpath_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/core/ros1/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/ros1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/ros1/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/ros1/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/ros1/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/core/ros1/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/ros1/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/ros1/variables/exp_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/startup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6030 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/stat_kernels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12464 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/core/variables/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1562 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/variables/base_variable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25747 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/variables/batch_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/variables/exp_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/variables/population_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3240 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/variables/variable_density.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3843 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/core/vector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6618 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/plugins/hpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/plugins/hpc/adhoc/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/adhoc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4046 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/adhoc/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/plugins/hpc/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/local/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2501 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/local/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.118452 sierra-research-1.3.6/sierra/plugins/hpc/pbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/pbs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3858 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/pbs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.122452 sierra-research-1.3.6/sierra/plugins/hpc/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/slurm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4164 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/hpc/slurm/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.122452 sierra-research-1.3.6/sierra/plugins/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.122452 sierra-research-1.3.6/sierra/plugins/platform/argos/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15855 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.122452 sierra-research-1.3.6/sierra/plugins/platform/argos/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15432 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/generators/platform_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.122452 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6062 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/arena_shape.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9031 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/cameras.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4618 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/constant_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/exp_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19636 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/physics_engines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6577 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/population_constant_density.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3539 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/population_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4967 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/population_variable_density.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/argos/variables/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.122452 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9920 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8463 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/variables/population_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6972 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/generators/platform_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14603 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5485 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/platform/ros1robot/variables/population_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/robot/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/robot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/robot/turtlebot3/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/robot/turtlebot3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7216 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/robot/turtlebot3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.126452 sierra-research-1.3.6/sierra/plugins/storage/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/storage/csv/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/plugins/storage/csv/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 09:25:50.000000 sierra-research-1.3.6/sierra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.130452 sierra-research-1.3.6/sierra_research.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16925 2024-04-01 09:27:59.000000 sierra-research-1.3.6/sierra_research.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-04-01 09:27:59.000000 sierra-research-1.3.6/sierra_research.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:27:59.000000 sierra-research-1.3.6/sierra_research.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 09:27:59.000000 sierra-research-1.3.6/sierra_research.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 09:27:59.000000 sierra-research-1.3.6/sierra_research.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 09:27:59.000000 sierra-research-1.3.6/sierra_research.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:27:59.130452 sierra-research-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-01 09:25:50.000000 sierra-research-1.3.6/tests/arena_extent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-01 09:25:50.000000 sierra-research-1.3.6/tests/exp_def_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-01 09:25:50.000000 sierra-research-1.3.6/tests/test1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-01 09:25:50.000000 sierra-research-1.3.6/tests/vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-01 09:25:50.000000 sierra-research-1.3.6/todo.org
```

### Comparing `sierra-research-1.3.5/.dir-locals.el` & `sierra-research-1.3.6/.dir-locals.el`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/actions/publish/action.yml` & `sierra-research-1.3.6/.github/actions/publish/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   steps:
     - uses: actions/checkout@v3
     - uses: ./.github/actions/sierra-setup
     - name: Build package
       shell: bash
       run: |
         python3 -m build
+        cd docs && make linkcheck
 
     - name: Set tag
       if: github.ref == 'refs/heads/devel'
       shell: bash
       run: echo "RELEASE_TAG=$(python3 setup.py --version).beta" >> $GITHUB_ENV
 
     - name: Github beta release
```

### Comparing `sierra-research-1.3.5/.github/actions/sample-project-setup/action.yml` & `sierra-research-1.3.6/.github/actions/sample-project-setup/action.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/actions/sierra-setup/action.yml` & `sierra-research-1.3.6/.github/actions/sierra-setup/action.yml`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,14 @@
 
     ############################################################################
     # SIERRA install
     ############################################################################
     - name: Install SIERRA
       shell: bash
       run: |
-        python -m pip install -r docs/requirements.txt
+        python3 -m pip install -r docs/requirements.txt
         cd docs && make man && cd ..
         python3 -m pip install .
         python3 -m pip install .[devel]
 
         which sierra-cli
         sierra-cli --version
```

### Comparing `sierra-research-1.3.5/.github/actions/slurm-setup/action.yml` & `sierra-research-1.3.6/.github/actions/slurm-setup/action.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/argos.yml` & `sierra-research-1.3.6/.github/workflows/argos.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/coverage.yml` & `sierra-research-1.3.6/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/exec-env-plugins.yml` & `sierra-research-1.3.6/.github/workflows/exec-env-plugins.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/integration-all.yml` & `sierra-research-1.3.6/.github/workflows/integration-all.yml`

 * *Files 26% similar despite different names*

```diff
@@ -10,53 +10,68 @@
     paths:
       - 'sierra/**'
 
   schedule:
     - cron: '0 0 1 * *'
 
 jobs:
-  argos-ci-ubuntu:
-    uses: ./.github/workflows/argos.yml
+  sierra-core-ci-ubuntu:
+    uses: ./.github/workflows/sierra-core.yml
     secrets: inherit
     with:
       os: ubuntu-20.04
 
-  argos-ci-osx:
-    uses: ./.github/workflows/argos.yml
+  sierra-core-ci-osx:
+    uses: ./.github/workflows/sierra-core.yml
     secrets: inherit
     with:
       os: macos-12
 
-  sierra-core-ci-ubuntu:
-    uses: ./.github/workflows/sierra-core.yml
+  argos-ci-ubuntu:
+    uses: ./.github/workflows/argos.yml
     secrets: inherit
+    needs:
+      - sierra-core-ci-ubuntu
+
     with:
       os: ubuntu-20.04
 
-  sierra-core-ci-osx:
-    uses: ./.github/workflows/sierra-core.yml
+  argos-ci-osx:
+    uses: ./.github/workflows/argos.yml
     secrets: inherit
+    needs:
+      - sierra-core-ci-osx
     with:
       os: macos-12
 
+
   ros1gazebo-ci-ubuntu:
     uses: ./.github/workflows/ros1gazebo.yml
     secrets: inherit
+    needs:
+      - sierra-core-ci-ubuntu
+
     with:
       os: ubuntu-20.04
 
   ros1robot-ci-ubuntu:
     uses: ./.github/workflows/ros1robot.yml
     secrets: inherit
+    needs:
+      - sierra-core-ci-ubuntu
+
     with:
       os: ubuntu-20.04
 
   exec-env-ci-ubuntu:
     uses: ./.github/workflows/exec-env-plugins.yml
     secrets: inherit
+    needs:
+      - sierra-core-ci-ubuntu
+
     with:
       os: ubuntu-20.04
 
   publish:
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `sierra-research-1.3.5/.github/workflows/ros1gazebo.yml` & `sierra-research-1.3.6/.github/workflows/ros1gazebo.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/ros1robot.yml` & `sierra-research-1.3.6/.github/workflows/ros1robot.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/sierra-core.yml` & `sierra-research-1.3.6/.github/workflows/sierra-core.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/static-analysis.yml` & `sierra-research-1.3.6/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.github/workflows/unit-tests.yml` & `sierra-research-1.3.6/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.gitignore` & `sierra-research-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.pylintrc` & `sierra-research-1.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/.readthedocs.yml` & `sierra-research-1.3.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/LICENSE` & `sierra-research-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/PKG-INFO` & `sierra-research-1.3.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,22 @@
-Metadata-Version: 2.1
-Name: sierra-research
-Version: 1.3.5
-Summary: Automation framework for the scientific method in AI research
-Home-page: https://github.com/jharwell/sierra
-Author: John Harwell
-Author-email: john.r.harwell@gmail.com
-License: MIT
-Keywords: research,automation,robotics,agent-based modeling,reproducibility,reusability
-Platform: linux
-Platform: osx
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: devel
-License-File: LICENSE
-
 ===========================================================================
 SIERRA (reSearch pIpEline for Reproducibility, Reusability, and Automation)
 ===========================================================================
 
 .. |pepy-downloads| image:: https://pepy.tech/badge/sierra-research
                     :target: https://pepy.tech/project/sierra-research
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/sierra-research.svg
                   :target: https://pypi.python.org/pypi/sierra-research/
 
 .. |supported-pythons| image:: https://img.shields.io/pypi/pyversions/sierra-research.svg
                        :target: https://pypi.python.org/pypi/sierra-research/
 
-.. |linux-supported| image:: https://svgshare.com/i/Zhy.svg
-.. |osx-supported| image:: https://svgshare.com/i/ZjP.svg
+.. |linux-supported| image:: https://img.shields.io/badge/os-Linux-crimson
+.. |osx-supported| image:: https://img.shields.io/badge/os-OSX-crimson
 
 .. |ci-integration-master| image:: https://github.com/jharwell/sierra/actions/workflows/integration-all.yml/badge.svg?branch=master
 .. |ci-analysis-master| image:: https://github.com/jharwell/sierra/actions/workflows/static-analysis.yml/badge.svg?branch=master
 .. |ci-coverage-master| image:: https://coveralls.io/repos/github/jharwell/sierra/badge.svg?branch=master
 
 .. |ci-integration-devel| image:: https://github.com/jharwell/sierra/actions/workflows/integration-all.yml/badge.svg?branch=devel
 .. |ci-analysis-devel| image:: https://github.com/jharwell/sierra/actions/workflows/static-analysis.yml/badge.svg?branch=devel
```

### Comparing `sierra-research-1.3.5/README.rst` & `sierra-research-1.3.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,87 @@
+Metadata-Version: 2.1
+Name: sierra-research
+Version: 1.3.6
+Summary: Automation framework for the scientific method in AI research
+Home-page: https://github.com/jharwell/sierra
+Author: John Harwell
+Author-email: john.r.harwell@gmail.com
+License: MIT
+Keywords: research,automation,robotics,agent-based modeling,reproducibility,reusability
+Platform: linux
+Platform: osx
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: pyyaml
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: sympy
+Requires-Dist: psutil
+Requires-Dist: distro
+Requires-Dist: netifaces
+Requires-Dist: haggis
+Requires-Dist: coloredlogs
+Requires-Dist: implements
+Requires-Dist: retry
+Provides-Extra: devel
+Requires-Dist: pylint==2.14.5; extra == "devel"
+Requires-Dist: pytype; extra == "devel"
+Requires-Dist: pydocstyle; extra == "devel"
+Requires-Dist: xenon; extra == "devel"
+Requires-Dist: flake8; extra == "devel"
+Requires-Dist: nox; extra == "devel"
+Requires-Dist: psutil; extra == "devel"
+Requires-Dist: pytest; extra == "devel"
+Requires-Dist: pytest-cov; extra == "devel"
+Requires-Dist: mypy; extra == "devel"
+Requires-Dist: xmldiff; extra == "devel"
+Requires-Dist: coverage; extra == "devel"
+Requires-Dist: coveralls; extra == "devel"
+Requires-Dist: mypy-runner; extra == "devel"
+Requires-Dist: build; extra == "devel"
+Requires-Dist: twine; extra == "devel"
+Requires-Dist: setuptools; extra == "devel"
+Requires-Dist: sphinx==5.0.2; extra == "devel"
+Requires-Dist: docutils==0.18.1; extra == "devel"
+Requires-Dist: sphinx-rtd-theme; extra == "devel"
+Requires-Dist: sphinx-argparse; extra == "devel"
+Requires-Dist: sphinx-tabs; extra == "devel"
+Requires-Dist: sphinxcontrib-napoleon; extra == "devel"
+Requires-Dist: psutil; extra == "devel"
+Requires-Dist: sphinx-last-updated-by-git; extra == "devel"
+Requires-Dist: autoapi; extra == "devel"
+Requires-Dist: graphviz; extra == "devel"
+
 ===========================================================================
 SIERRA (reSearch pIpEline for Reproducibility, Reusability, and Automation)
 ===========================================================================
 
 .. |pepy-downloads| image:: https://pepy.tech/badge/sierra-research
                     :target: https://pepy.tech/project/sierra-research
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/sierra-research.svg
                   :target: https://pypi.python.org/pypi/sierra-research/
 
 .. |supported-pythons| image:: https://img.shields.io/pypi/pyversions/sierra-research.svg
                        :target: https://pypi.python.org/pypi/sierra-research/
 
-.. |linux-supported| image:: https://svgshare.com/i/Zhy.svg
-.. |osx-supported| image:: https://svgshare.com/i/ZjP.svg
+.. |linux-supported| image:: https://img.shields.io/badge/os-Linux-crimson
+.. |osx-supported| image:: https://img.shields.io/badge/os-OSX-crimson
 
 .. |ci-integration-master| image:: https://github.com/jharwell/sierra/actions/workflows/integration-all.yml/badge.svg?branch=master
 .. |ci-analysis-master| image:: https://github.com/jharwell/sierra/actions/workflows/static-analysis.yml/badge.svg?branch=master
 .. |ci-coverage-master| image:: https://coveralls.io/repos/github/jharwell/sierra/badge.svg?branch=master
 
 .. |ci-integration-devel| image:: https://github.com/jharwell/sierra/actions/workflows/integration-all.yml/badge.svg?branch=devel
 .. |ci-analysis-devel| image:: https://github.com/jharwell/sierra/actions/workflows/static-analysis.yml/badge.svg?branch=devel
```

### Comparing `sierra-research-1.3.5/docs/Makefile` & `sierra-research-1.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra-cli.1` & `sierra-research-1.3.6/docs/_build/man/sierra-cli.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-CLI" "1" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra-cli \- The SIERRA Command Line Interface (CLI).
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,31 +23,34 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA-CLI" "1" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra-cli \- The SIERRA Command Line Interface (CLI).
 .sp
 Unless an option says otherwise, it is applicable to all batch criteria. That
 is, option batch criteria applicability is only documented for options which
-apply to a subset of the available Batch Criteria\&.
+apply to a subset of the available \fI\%Batch Criteria\fP\&.
 .sp
 If an option is given more than once, the last such occurrence is used.
 .sp
 See also \fBsierra\-examples\fP\&.
 .sp
 
 .nf
 :seealso:\(galn\-sierra\-examples\(ga
 .fi
 
 .SH SIERRA CORE
 .sp
-These options are for all Platforms\&.
+These options are for all \fI\%Platforms\fP\&.
 .SS Bootstrap+Multi\-stage Options
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 usage: sphinx\-build [\-h] [\-\-project PROJECT] [\-\-version]
@@ -73,39 +73,39 @@
 .UNINDENT
 .UNINDENT
 .SS Bootstrap options
 .sp
 Bare\-bones options for bootstrapping SIERRA
 .INDENT 0.0
 .TP
-.B\-\-project
+.B \-\-project
 .INDENT 7.0
 .INDENT 3.5
-Specify which Project to load.
+Specify which \fI\%Project\fP to load.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,2,3,4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-version, \-v
+.B \-\-version, \-v
 .INDENT 7.0
 .INDENT 3.5
 Display SIERRA version information on stdout and
 then exit.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-log\-level
+.B \-\-log\-level
 Possible choices: ERROR, INFO, WARNING, DEBUG, TRACE
 .INDENT 7.0
 .INDENT 3.5
 The level of logging to use when running
 SIERRA.
 .UNINDENT
 .UNINDENT
@@ -113,100 +113,100 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,2,3,4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "INFO"
+Default: \(dqINFO\(dq
 .TP
-.B\-\-platform
+.B \-\-platform
 .INDENT 7.0
 .INDENT 3.5
-This argument defines the Platform you
+This argument defines the \fI\%Platform\fP you
 want to run experiments on.
 .sp
 The value of this argument determines the
 execution environment for experiments; different
 platforms (e.g., simulator, real robots) will
 have different configuration options.
 .sp
 Valid values can be any folder name inside a
-folder on the \fBSIERRA_PLUGIN_PATH\fP (with
+folder on the \fI\%SIERRA_PLUGIN_PATH\fP (with
 \fB/\fP replaced with \fB\&.\fP as you would expect for
 using path names to address python packages). The
 platforms which come with SIERRA are:
 .INDENT 0.0
 .IP \(bu 2
 \fBplatform.argos\fP \- This directs SIERRA to run
-experiments using the ARGoS
+experiments using the \fI\%ARGoS\fP
 simulator. Selecting this platform assumes your
 code has been developed and configured for
 ARGoS.
 .IP \(bu 2
 \fBplatform.ros1gazebo\fP \- This directs SIERRA to
-run experiments using the Gazebo
-simulator and ROS1\&. Selecting this
+run experiments using the \fI\%Gazebo\fP
+simulator and \fI\%ROS1\fP\&. Selecting this
 platform assumes your code has been developed
 and configured for Gazebo and ROS1.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
-Default: "platform.argos"
+Default: \(dqplatform.argos\(dq
 .TP
-.B\-\-skip\-pkg\-checks
+.B \-\-skip\-pkg\-checks
 .INDENT 7.0
 .INDENT 3.5
 Skip the usual startup package checks. Only do
 this if you are SURE you will never use the
 SIERRA functionality which requires packages you
 don\(aqt have installed/can\(aqt install.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-exec\-env
+.B \-\-exec\-env
 .INDENT 7.0
 .INDENT 3.5
 This argument defines \fIhow\fP experiments are going
 to be run, using the \fB\-\-platform\fP you have
 selected.
 .sp
 Valid values can be any folder name inside a
-folder on the \fBSIERRA_PLUGIN_PATH\fP (with
+folder on the \fI\%SIERRA_PLUGIN_PATH\fP (with
 \fB/\fP replaced with \fB\&.\fP as you would expect for
 using path names to address python packages). The
 execution environments which come with SIERRA
 are:
 .INDENT 0.0
 .IP \(bu 2
 \fBhpc.local\fP \- This directs SIERRA to run
 experiments on the local machine. See
-ln\-sierra\-hpc\-plugins\-local for a detailed
+\fI\%Local HPC Plugin\fP for a detailed
 description.
 .IP \(bu 2
 \fBhpc.pbs\fP \- The directs SIERRA to run
 experiments spread across multiple allocated
 nodes in an HPC computing environment managed
-by TORQUE\-PBS. See ln\-sierra\-hpc\-plugins\-pbs
+by TORQUE\-PBS. See \fI\%PBS HPC Plugin\fP
 for a detailed description.
 .IP \(bu 2
 \fBhpc.slurm\fP \- The directs SIERRA to run
 experiments spread across multiple allocated
 nodes in an HPC computing environment managed
 by SLURM. See
-ln\-sierra\-hpc\-plugins\-slurm for a
+\fI\%SLURM HPC Plugin\fP for a
 detailed description.
 .IP \(bu 2
 \fBhpc.adhoc\fP \- This will direct SIERRA to run
 experiments on an ad\-hoc network of
 computers. See
-ln\-sierra\-hpc\-plugins\-adhoc for a
+\fI\%Adhoc HPC Plugin\fP for a
 detailed description.
 .IP \(bu 2
 \fBrobot.turtlebot3\fP \- This will direct SIERRA
 to run experiments on real Turtlebots.
 .UNINDENT
 .sp
 Not all platforms support all execution
@@ -217,22 +217,22 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "hpc.local"
+Default: \(dqhpc.local\(dq
 .UNINDENT
 .SS Multi\-stage options
 .sp
 Options which are used in multiple pipeline stages
 .INDENT 0.0
 .TP
-.B\-\-template\-input\-file
+.B \-\-template\-input\-file
 .INDENT 7.0
 .INDENT 3.5
 The template \fB\&.xml\fP input file for the
 batch experiment. Beyond the requirements
 for the specific \fB\-\-platform\fP, the
 content of the file can be any valid XML,
 with the exception of the SIERRA
@@ -244,15 +244,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,2,3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-exp\-overwrite
+.B \-\-exp\-overwrite
 .INDENT 7.0
 .INDENT 3.5
 When SIERRA calculates the batch experiment
 root (or any child path in the batch
 experiment root) during stage {1, 2}, if
 the calculated path already exists it is
 treated as a fatal error and no
@@ -270,15 +270,15 @@
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-sierra\-root
+.B \-\-sierra\-root
 .INDENT 7.0
 .INDENT 3.5
 Root directory for all SIERRA generated and
 created files.
 .sp
 Subdirectories for controllers, scenarios,
 experiment/experimental run inputs/outputs
@@ -291,17 +291,17 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,2,3,4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "<home directory>/exp"
+Default: \(dq<home directory>/exp\(dq
 .TP
-.B\-\-batch\-criteria
+.B \-\-batch\-criteria
 .INDENT 7.0
 .INDENT 3.5
 Definition of criteria(s) to use to define
 the experiment.
 .sp
 Specified as a list of 0 or 1 space
 separated strings, each with the following
@@ -324,15 +324,15 @@
 .INDENT 3.5
 Used by stage {1,2,3,4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: []
 .TP
-.B\-\-pipeline
+.B \-\-pipeline
 .INDENT 7.0
 .INDENT 3.5
 Define which stages of the experimental
 pipeline to run:
 .INDENT 0.0
 .IP \(bu 2
 Stage1 \- Generate the experiment
@@ -361,15 +361,15 @@
 run. Not part of default pipeline.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 Default: [1, 2, 3, 4]
 .TP
-.B\-\-exp\-range
+.B \-\-exp\-range
 .INDENT 7.0
 .INDENT 3.5
 Set the experiment numbers from the batch to
 run, average, generate intra\-experiment
 graphs from, or generate inter\-experiment
 graphs from (0 based). Specified in the form
 \fBmin_exp_num:max_exp_num\fP (closed
@@ -391,42 +391,42 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {2,3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-platform\-vc
+.B \-\-platform\-vc
 .INDENT 7.0
 .INDENT 3.5
 For applicable \fB\-\-platforms\fP, enable
 visual capturing of run\-time data during
 stage 2. This data can be frames (i.e., .png
 files), or rendering videos, depending on
 the platform. If the captured data was
 frames, then SIERRA can render the captured
 frames into videos during stage 4. If the
 selected \fB\-\-platform\fP does not support
 visual capture, then this option has no
 effect. See
-ln\-sierra\-usage\-rendering\-platform
+\fI\%Platform Visual Capture\fP
 for full details.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-processing\-serial
+.B \-\-processing\-serial
 .INDENT 7.0
 .INDENT 3.5
 If TRUE, then results processing/graph
 generation will be performed serially,
 rather than using parallellism where
 possible.
 .UNINDENT
@@ -437,15 +437,15 @@
 .INDENT 3.5
 Used by stage {3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-n\-runs
+.B \-\-n\-runs
 .INDENT 7.0
 .INDENT 3.5
 The # of experimental runs that will be
 executed and their results processed to form
 the result of a single experiment within a
 batch.
 .sp
@@ -460,15 +460,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-skip\-collate
+.B \-\-skip\-collate
 .INDENT 7.0
 .INDENT 3.5
 Specify that no collation of data across
 experiments within a batch (stage 4) or
 across runs within an experiment (stage 3)
 should be performed. Useful if collation
 takes a long time and multiple types of
@@ -483,15 +483,15 @@
 .INDENT 3.5
 Used by stage {3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-plot\-log\-xscale
+.B \-\-plot\-log\-xscale
 .INDENT 7.0
 .INDENT 3.5
 Place the set of X values used to generate intra\- and
 inter\-experiment graphs into the logarithmic
 space. Mainly useful when the batch criteria involves
 large system sizes, so that the plots are more
 readable.
@@ -514,15 +514,15 @@
 .INDENT 3.5
 Used by stage {4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-plot\-enumerated\-xscale
+.B \-\-plot\-enumerated\-xscale
 .INDENT 7.0
 .INDENT 3.5
 Instead of using the values generated by a
 given batch criteria for the X values, use
 an enumerated list[0, ..., len(X value) \-
 1]. Mainly useful when the batch criteria
 involves large system sizes, so that the
@@ -546,15 +546,15 @@
 .INDENT 3.5
 Used by stage {4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-plot\-log\-yscale
+.B \-\-plot\-log\-yscale
 .INDENT 7.0
 .INDENT 3.5
 Place the set of Y values used to generate
 intra \- and inter\-experiment graphs into
 the logarithmic space. Mainly useful when
 the batch criteria involves large system
 sizes, so that the plots are more readable.
@@ -579,15 +579,15 @@
 .INDENT 3.5
 Used by stage {4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-plot\-regression\-lines
+.B \-\-plot\-regression\-lines
 .INDENT 7.0
 .INDENT 3.5
 For all 2D generated scatterplots, plot a
 linear regression line and the equation of
 the line to the legend.
 .UNINDENT
 .UNINDENT
@@ -606,30 +606,30 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-plot\-primary\-axis
+.B \-\-plot\-primary\-axis
 .INDENT 7.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 This option allows you to override the
 primary axis, which is normally is computed
 based on the batch criteria.
 .sp
 For example, in a bivariate batch criteria
 composed of
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-ln\-sierra\-platform\-argos\-bc\-population\-size
+\fI\%Population Size\fP
 on the X axis (rows)
 .IP \(bu 2
 Another batch criteria which does not
 affect system size (columns)
 .UNINDENT
 .sp
 Metrics will be calculated by \fIcomputing\fP
@@ -669,15 +669,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-plot\-large\-text
+.B \-\-plot\-large\-text
 .INDENT 7.0
 .INDENT 3.5
 This option specifies that the title, X/Y
 axis labels/tick labels should be larger
 than the SIERRA default. This is useful when
 generating graphs suitable for two column
 paper format where the default text size for
@@ -693,15 +693,15 @@
 .INDENT 3.5
 Used by stage {4,5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-plot\-transpose\-graphs
+.B \-\-plot\-transpose\-graphs
 .INDENT 7.0
 .INDENT 3.5
 Transpose the X, Y axes in generated
 graphs. Useful as a general way to tweak
 graphs for best use of space within a paper.
 .sp
 Changed in version 1.2.20: Renamed from \fB\-\-transpose\-graphs\fP to
@@ -750,21 +750,21 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage3: General options for eprocessing experiment results
 .INDENT 0.0
 .TP
-.B\-\-df\-skip\-verify
+.B \-\-df\-skip\-verify
 .INDENT 7.0
 .INDENT 3.5
 SIERRA generally assumes/relies on all
 dataframes with the same name having the same #
 of columns which are of equivalent length
-across Experimental Runs (different columns within a dataframe can
+across \fI\%Experimental Runs\fP (different columns within a dataframe can
 of course have different lengths). This is
 strictly verified during stage 3 by default.
 .sp
 If passed, then the verification step will be
 skipped during experimental results processing,
 and outputs will be averaged directly.
 .sp
@@ -782,20 +782,20 @@
 .INDENT 3.5
 Used by stage {3}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-storage\-medium
+.B \-\-storage\-medium
 Possible choices: storage.csv
 .INDENT 7.0
 .INDENT 3.5
 Specify the storage medium for
-Experimental Run outputs, so that
+\fI\%Experimental Run\fP outputs, so that
 SIERRA can select an appropriate plugin to read
 them. Any plugin under \fBplugins/storage\fP can
 be used, but the ones that come with SIERRA
 are:
 .INDENT 0.0
 .IP \(bu 2
 \fBstorage.csv\fP \- Experimental run outputs
@@ -812,17 +812,17 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {3}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "storage.csv"
+Default: \(dqstorage.csv\(dq
 .TP
-.B\-\-dist\-stats
+.B \-\-dist\-stats
 Possible choices: none, all, conf95, bw
 .INDENT 7.0
 .INDENT 3.5
 Specify what kinds of statistics, if any,
 should be calculated on the distribution of
 experimental data during stage 3 for inclusion
 on graphs during stage 4:
@@ -861,17 +861,17 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "none"
+Default: \(dqnone\(dq
 .TP
-.B\-\-processing\-mem\-limit
+.B \-\-processing\-mem\-limit
 .INDENT 7.0
 .INDENT 3.5
 Specify, as a percent in [0, 100], how much
 memory SIERRA should try to limit itself to
 using. This is useful on systems with limited
 memory, or on systems which are shared with
 other users without per\-user memory
@@ -884,15 +884,15 @@
 .INDENT 3.5
 Used by stage {3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: 90
 .TP
-.B\-\-df\-homogenize
+.B \-\-df\-homogenize
 .INDENT 7.0
 .INDENT 3.5
 SIERRA generally assumes/relies on all
 dataframes with the same name having the same #
 of columns which are of equivalent length
 across: term: \fIExperimental Runs < Experimental
 Run >\fP (different columns within a dataframe
@@ -930,15 +930,15 @@
 the number of datapoints captured per\-robot is
 slightly different, depending on when they
 started executing relative to when the
 experiment started.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "none"
+Default: \(dqnone\(dq
 .UNINDENT
 .SS Stage4: Deliverable Generation
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
@@ -949,15 +949,15 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage4: General options for generating graphs
 .INDENT 0.0
 .TP
-.B\-\-exp\-graphs
+.B \-\-exp\-graphs
 Possible choices: intra, inter, all, none
 .INDENT 7.0
 .INDENT 3.5
 Specify which types of graphs should be
 generated from experimental results:
 .INDENT 0.0
 .IP \(bu 2
@@ -989,17 +989,17 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "all"
+Default: \(dqall\(dq
 .TP
-.B\-\-project\-no\-LN
+.B \-\-project\-no\-LN
 .INDENT 7.0
 .INDENT 3.5
 Specify that the intra\-experiment and
 inter\-experiment linegraphs defined in project
 YAML configuration should not be
 generated. Useful if you are working on
 something which results in the generation of
@@ -1010,15 +1010,15 @@
 Model linegraphs are still generated, if
 applicable.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-project\-no\-HM
+.B \-\-project\-no\-HM
 .INDENT 7.0
 .INDENT 3.5
 Specify that the intra\-experiment heatmaps
 defined in project YAML configuration should
 not be generated. Useful if:
 .INDENT 0.0
 .IP \(bu 2
@@ -1042,30 +1042,30 @@
 .UNINDENT
 .sp
 Default: False
 .UNINDENT
 .SS Models
 .INDENT 0.0
 .TP
-.B\-\-models\-enable
+.B \-\-models\-enable
 .INDENT 7.0
 .INDENT 3.5
 Enable running of all models; otherwise, no models
 are run, even if they appear in the project config
 file. The logic behind having models disabled by
 default is that most users won\(aqt have them.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .UNINDENT
 .SS Stage4: Rendering (see also stage1 rendering options)
 .INDENT 0.0
 .TP
-.B\-\-render\-cmd\-opts
+.B \-\-render\-cmd\-opts
 .INDENT 7.0
 .INDENT 3.5
 Specify the: program: \fIffmpeg\fP options to appear
 between the specification of the input image
 files and the specification of the output
 file. The default is suitable for use with ARGoS
 frame grabbing set to a frames size of 1600x1200
@@ -1076,57 +1076,57 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "\-r 10 \-s:v 800x600 \-c:v libx264 \-crf 25 \-filter:v scale=\-2:956 \-pix_fmt yuv420p"
+Default: \(dq\-r 10 \-s:v 800x600 \-c:v libx264 \-crf 25 \-filter:v scale=\-2:956 \-pix_fmt yuv420p\(dq
 .TP
-.B\-\-project\-imagizing
+.B \-\-project\-imagizing
 .INDENT 7.0
 .INDENT 3.5
 Enable generation of image files from CSV files
 captured during stage 2 and averaged during stage
 3 for each experiment. See
-ln\-sierra\-usage\-rendering\-project for
+\fI\%Project Rendering\fP for
 details and restrictions.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {3,4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-project\-rendering
+.B \-\-project\-rendering
 .INDENT 7.0
 .INDENT 3.5
 Enable generation of videos from imagized CSV
 files created as a result of
 \fB\-\-project\-imagizing\fP\&. See
-ln\-sierra\-usage\-rendering\-project for
+\fI\%Project Rendering\fP for
 details.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {4}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-bc\-rendering
+.B \-\-bc\-rendering
 .INDENT 7.0
 .INDENT 3.5
 Enable generation of videos from generated
 graphs, such as heatmaps. Bivariate batch
 criteria only.
 .UNINDENT
 .UNINDENT
@@ -1156,15 +1156,15 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage5: General options for controller comparison
 .INDENT 0.0
 .TP
-.B\-\-controllers\-list
+.B \-\-controllers\-list
 .INDENT 7.0
 .INDENT 3.5
 Comma separated list of controllers to compare
 within \fB\-\-sierra\-root\fP\&.
 .sp
 The first controller in this list will be used
 for as the controller of primary interest if \fB\-\-comparison\-type\fP is passed.
@@ -1174,15 +1174,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-controllers\-legend
+.B \-\-controllers\-legend
 .INDENT 7.0
 .INDENT 3.5
 Comma separated list of names to use on the
 legend for the generated comparison graphs,
 specified in the same order as the
 \fB\-\-controllers\-list\fP\&.
 .UNINDENT
@@ -1191,15 +1191,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. If omitted: the raw controller names will be used.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-scenarios\-list
+.B \-\-scenarios\-list
 .INDENT 7.0
 .INDENT 3.5
 Comma separated list of scenarios to compare
 \fB\-\-controller\fP across within
 \fB\-\-sierra\-root\fP\&.
 .UNINDENT
 .UNINDENT
@@ -1207,15 +1207,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-scenarios\-legend
+.B \-\-scenarios\-legend
 .INDENT 7.0
 .INDENT 3.5
 Comma separated list of names to use on the
 legend for the generated inter\-scenario
 controller comparison graphs(if applicable),
 specified in the same order as the
 \fB\-\-scenarios\-list\fP\&.
@@ -1225,15 +1225,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. If omitted: the raw scenario names will be used.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-scenario\-comparison
+.B \-\-scenario\-comparison
 .INDENT 7.0
 .INDENT 3.5
 Perform a comparison of \fB\-\-controller\fP across
 \fB\-\-scenarios\-list\fP (univariate batch criteria
 only).
 .UNINDENT
 .UNINDENT
@@ -1244,15 +1244,15 @@
 Used by stage {5}; can be omitted otherwise. Either \fB\-\-scenario\-comparison\fP or \fB\-\-controller\-comparison\fP must be
 passed.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-controller\-comparison
+.B \-\-controller\-comparison
 .INDENT 7.0
 .INDENT 3.5
 Perform a comparison of \fB\-\-controllers\-list\fP
 across all scenarios at least one controller
 has been run on.
 .UNINDENT
 .UNINDENT
@@ -1262,15 +1262,15 @@
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. Either \fB\-\-scenario\-comparison\fP or \fB\-\-controller\-comparison\fP must be passed.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-comparison\-type
+.B \-\-comparison\-type
 Possible choices: LNraw, HMraw, HMdiff, HMscale, SUraw, SUscale, SUdiff
 .INDENT 7.0
 .INDENT 3.5
 Specify how controller comparisons should be
 performed.
 .sp
 If the batch criteria is univariate, the
@@ -1351,15 +1351,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-bc\-univar
+.B \-\-bc\-univar
 .INDENT 7.0
 .INDENT 3.5
 Specify that the batch criteria is
 univariate. This cannot be deduced from the
 command line \fB\-\-batch\-criteria\fP argument in
 all cases because we are comparing controllers
 \fIacross\fP scenarios, and each scenario
@@ -1376,15 +1376,15 @@
 .INDENT 3.5
 Used by stage {5}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-bc\-bivar
+.B \-\-bc\-bivar
 .INDENT 7.0
 .INDENT 3.5
 Specify that the batch criteria is
 bivariate. This cannot be deduced from the
 command line \fB\-\-batch\-criteria\fP argument in
 all cases because we are comparing controllers
 \fIacross\fP scenarios, and each
@@ -1424,38 +1424,38 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage1: Experiment generation
 .INDENT 0.0
 .TP
-.B\-\-exp\-setup
+.B \-\-exp\-setup
 .INDENT 7.0
 .INDENT 3.5
-Defines experiment run length, Ticks per second for the experiment
+Defines experiment run length, \fI\%Ticks\fP per second for the experiment
 (<experiment> tag), # of datapoints to
 capture/capture interval for each
-simulation. See ln\-sierra\-vars\-expsetup for
+simulation. See \fI\%Experiment Setup\fP for
 a full description.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "exp_setup.T5000.K5.N50"
+Default: \(dqexp_setup.T5000.K5.N50\(dq
 .UNINDENT
 .SS Stage1: Configuring ARGoS physics engines
 .INDENT 0.0
 .TP
-.B\-\-physics\-engine\-type2D
+.B \-\-physics\-engine\-type2D
 Possible choices: dynamics2d
 .INDENT 7.0
 .INDENT 3.5
 The type of 2D physics engine to use
 for managing spatial extents within the
 arena, choosing one of the types that
 ARGoS supports. The precise 2D areas
@@ -1468,17 +1468,17 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "dynamics2d"
+Default: \(dqdynamics2d\(dq
 .TP
-.B\-\-physics\-engine\-type3D
+.B \-\-physics\-engine\-type3D
 Possible choices: dynamics3d
 .INDENT 7.0
 .INDENT 3.5
 The type of 3D physics engine to use
 for managing 3D volumetric extents
 within the arena, choosing one of the
 types that ARGoS supports. The precise
@@ -1492,29 +1492,29 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "dynamics3d"
+Default: \(dqdynamics3d\(dq
 .TP
-.B\-\-physics\-n\-engines
+.B \-\-physics\-n\-engines
 Possible choices: 1, 2, 4, 6, 8, 12, 16, 24
 .INDENT 7.0
 .INDENT 3.5
 # of physics engines to use during
 simulation (yay ARGoS!). If N > 1, the
 engines will be tiled in a uniform grid
 within the arena (X and Y spacing may
 not be the same depending on dimensions
 and how many engines are chosen,
 however), extending upward in Z to the
 height specified by \fB\-\-scenario\fP
-(i.e., forming a set of "silos" rather
+(i.e., forming a set of \(dqsilos\(dq rather
 that equal volumetric extents).
 .sp
 If 2D and 3D physics engines are mixed,
 then half of the specified # of engines
 will be allocated among all arena
 extents cumulatively managed by each
 type of engine. For example, if 4
@@ -1564,19 +1564,19 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-physics\-iter\-per\-tick
+.B \-\-physics\-iter\-per\-tick
 .INDENT 7.0
 .INDENT 3.5
 The # of iterations all physics engines
-should perform per Tick each
+should perform per \fI\%Tick\fP each
 time the controller loops are run (the
 # of ticks per second for controller
 control loops is set via
 \fB\-\-exp\-setup\fP).
 .UNINDENT
 .UNINDENT
 .sp
@@ -1585,29 +1585,29 @@
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: 10
 .TP
-.B\-\-physics\-spatial\-hash2D
+.B \-\-physics\-spatial\-hash2D
 .INDENT 7.0
 .INDENT 3.5
 Specify that each 2D physics engine
 should use a spatial hash (only applies
 to \fBdynamics2d\fP engine type).
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .UNINDENT
 .SS Stage1: Rendering (see also stage4 rendering options)
 .INDENT 0.0
 .TP
-.B\-\-camera\-config
+.B \-\-camera\-config
 Possible choices: overhead, sw, sw+interp
 .INDENT 7.0
 .INDENT 3.5
 Select the camera configuration for
 simulation. Ignored unless
 \fB\-\-platform\-vc\fP is passed. Valid
 values are:
@@ -1634,20 +1634,20 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "overhead"
+Default: \(dqoverhead\(dq
 .UNINDENT
 .SS Stage1: Configuring robots
 .INDENT 0.0
 .TP
-.B\-\-with\-robot\-rab
+.B \-\-with\-robot\-rab
 .INDENT 7.0
 .INDENT 3.5
 If passed, do not remove the Range and
 Bearing (RAB) sensor, actuator, and
 medium XML definitions from
 \fB\-\-template\-input\-file\fP before
 generating experimental
@@ -1669,15 +1669,15 @@
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-with\-robot\-leds
+.B \-\-with\-robot\-leds
 .INDENT 7.0
 .INDENT 3.5
 If passed, do not remove the robot LED
 actuator XML definitions from the
 \fB\-\-template\-input\-file\fP before
 generating experimental
 inputs. Otherwise, the following XML
@@ -1698,15 +1698,15 @@
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-with\-robot\-battery
+.B \-\-with\-robot\-battery
 .INDENT 7.0
 .INDENT 3.5
 If passed, do not remove the robot
 battery sensor XML definitions from
 \fB\-\-template\-input\-file\fP before
 generating experimental
 inputs. Otherwise, the following XML
@@ -1725,15 +1725,15 @@
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-n\-robots
+.B \-\-n\-robots
 .INDENT 7.0
 .INDENT 3.5
 The # robots that should be used in the
 simulation. Can be used to override
 batch criteria, or to supplement
 experiments that do not set it so that
 manual modification of input file is
@@ -1761,15 +1761,15 @@
 .UNINDENT
 .UNINDENT
 .SS HPC options
 .sp
 For platforms which are simulators (and can therefore be run in HPC environments).
 .INDENT 0.0
 .TP
-.B\-\-exec\-jobs\-per\-node
+.B \-\-exec\-jobs\-per\-node
 .INDENT 7.0
 .INDENT 3.5
 Specify the maximum number of parallel jobs to run
 per allocated node. By default this is computed
 from the selected HPC environment for maximum
 throughput given the desired \fB\-\-n\-runs\fP and CPUs
 per allocated node. However, for some environments
@@ -1781,15 +1781,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-exec\-devnull
+.B \-\-exec\-devnull
 .INDENT 7.0
 .INDENT 3.5
 Redirect ALL output from simulations to
 /dev/null. Useful for platform where you can\(aqt
 disable all INFO messages at compile time, and
 don\(aqt want to have to grep through lots of
 redundant stdout files to see if there were any
@@ -1802,15 +1802,15 @@
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: True
 .TP
-.B\-\-exec\-no\-devnull
+.B \-\-exec\-no\-devnull
 .INDENT 7.0
 .INDENT 3.5
 Don\(aqt redirect ALL output from simulations to
 /dev/null. Useful for platform where you can\(aqt
 disable all INFO messages at compile time, and
 don\(aqt want to have to grep through lots of
 redundant stdout files to see if there were any
@@ -1823,15 +1823,15 @@
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: True
 .TP
-.B\-\-exec\-resume
+.B \-\-exec\-resume
 .INDENT 7.0
 .INDENT 3.5
 Resume a batch experiment that was
 killed/stopped/etc last time SIERRA was run.
 .UNINDENT
 .UNINDENT
 .sp
@@ -1840,26 +1840,26 @@
 .INDENT 3.5
 Used by stage {2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-exec\-strict
+.B \-\-exec\-strict
 .INDENT 7.0
 .INDENT 3.5
 If passed, then if any experimental commands fail
 during stage 2 SIERRA will exit, rather than try
 to keep going and execute the rest of the
 experiments.
 .sp
 Useful for:
 .INDENT 0.0
 .IP \(bu 2
-"Correctness by construction" experiments, where
+\(dqCorrectness by construction\(dq experiments, where
 you know if SIERRA doesn\(aqt crash and it makes it
 to the end of your batch experiment then none of
 the individual experiments crashed.
 .IP \(bu 2
 CI pipelines
 .UNINDENT
 .UNINDENT
@@ -1885,40 +1885,40 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage1: Experiment generation
 .INDENT 0.0
 .TP
-.B\-\-exp\-setup
+.B \-\-exp\-setup
 .INDENT 7.0
 .INDENT 3.5
 Defines experiment run length, ticks per
 second for the experiment, # of datapoints
 to capture/capture interval for each
-simulation. See ln\-sierra\-vars\-expsetup for
+simulation. See \fI\%Experiment Setup\fP for
 a full description.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "exp_setup.T1000.K5.N50"
+Default: \(dqexp_setup.T1000.K5.N50\(dq
 .TP
-.B\-\-robot
+.B \-\-robot
 .INDENT 7.0
 .INDENT 3.5
 The key name of the robot model, which must
 be present in the appropriate section of
-\fBmain.yaml\fP for the Project\&. See
+\fBmain.yaml\fP for the \fI\%Project\fP\&. See
 ln\-sierra\-tutorials\-project\-main\-config
 for details.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
@@ -1926,18 +1926,18 @@
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS Stage1: Experiment setup
 .INDENT 0.0
 .TP
-.B\-\-robot\-positions
+.B \-\-robot\-positions
 .INDENT 7.0
 .INDENT 3.5
-A list of space\-separated "X,Y,Z" tuples
+A list of space\-separated \(dqX,Y,Z\(dq tuples
 (no quotes) passed on the command line as
 valid starting positions for the robots
 within the world.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
@@ -1948,37 +1948,37 @@
 .UNINDENT
 .sp
 Default: []
 .UNINDENT
 .SS Stage1: Configuring Gazebo physics engines
 .INDENT 0.0
 .TP
-.B\-\-physics\-engine\-type
+.B \-\-physics\-engine\-type
 Possible choices: ode, bullet, dart, simbody
 .INDENT 7.0
 .INDENT 3.5
 The type of 3D physics engine to use
 for managing spatial extents within the
 arena, choosing one of the types that
-Gazebo supports. A single
+\fI\%Gazebo\fP supports. A single
 engine instance is used to manage all
 physics in the arena.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "ode"
+Default: \(dqode\(dq
 .TP
-.B\-\-physics\-iter\-per\-tick
+.B \-\-physics\-iter\-per\-tick
 .INDENT 7.0
 .INDENT 3.5
 The # of iterations all physics engines
 should perform per tick each time the
 controller loops are run (the # of
 ticks per second for controller control
 loops is set via \fB\-\-exp\-setup\fP).
@@ -1990,28 +1990,28 @@
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: 1000
 .TP
-.B\-\-physics\-n\-threads
+.B \-\-physics\-n\-threads
 .INDENT 7.0
 .INDENT 3.5
 Gazebo can group non\-interacting
-entities into computational "islands"
+entities into computational \(dqislands\(dq
 and do the physics updates for those
 islands in parallel each timestep
 (islands) are recomputed after each
 timestep). Gazebo can also parallelize
 the computation of velocity/position
 updates with the computation of
 resolving collisions (i.e., the
 timestep impulse results in one entity
-"inside" another). You can assign
+\(dqinside\(dq another). You can assign
 multiple threads to a pool for
 cumulative use for these two
 parallelization methods (threads will
 be allocated evenly between them). The
 point at which adding more threads will
 start to DECREASE performance depends
 on the complexity of your world, the
@@ -2040,22 +2040,22 @@
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: 0
 .TP
-.B\-\-physics\-ec\-threadpool
+.B \-\-physics\-ec\-threadpool
 .INDENT 7.0
 .INDENT 3.5
 Gazebo can parallelize the computation
 of velocity/position updates with the
 computation of resolving collisions
 (i.e., the timestep impulse results in
-one entity "inside" another). You can
+one entity \(dqinside\(dq another). You can
 assign multiple threads to a pool for
 cumulative use for this purpose. The
 point at which adding more threads will
 start to DECREASE performance depends
 on the complexity of your world, the
 number and type of robots in it, etc.,
 so don\(aqt just set this parameter to the
@@ -2098,15 +2098,15 @@
 .UNINDENT
 .UNINDENT
 .SS HPC options
 .sp
 For platforms which are simulators (and can therefore be run in HPC environments).
 .INDENT 0.0
 .TP
-.B\-\-exec\-jobs\-per\-node
+.B \-\-exec\-jobs\-per\-node
 .INDENT 7.0
 .INDENT 3.5
 Specify the maximum number of parallel jobs to run
 per allocated node. By default this is computed
 from the selected HPC environment for maximum
 throughput given the desired \fB\-\-n\-runs\fP and CPUs
 per allocated node. However, for some environments
@@ -2118,15 +2118,15 @@
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .TP
-.B\-\-exec\-devnull
+.B \-\-exec\-devnull
 .INDENT 7.0
 .INDENT 3.5
 Redirect ALL output from simulations to
 /dev/null. Useful for platform where you can\(aqt
 disable all INFO messages at compile time, and
 don\(aqt want to have to grep through lots of
 redundant stdout files to see if there were any
@@ -2139,15 +2139,15 @@
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: True
 .TP
-.B\-\-exec\-no\-devnull
+.B \-\-exec\-no\-devnull
 .INDENT 7.0
 .INDENT 3.5
 Don\(aqt redirect ALL output from simulations to
 /dev/null. Useful for platform where you can\(aqt
 disable all INFO messages at compile time, and
 don\(aqt want to have to grep through lots of
 redundant stdout files to see if there were any
@@ -2160,15 +2160,15 @@
 .INDENT 3.5
 Used by stage {1,2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: True
 .TP
-.B\-\-exec\-resume
+.B \-\-exec\-resume
 .INDENT 7.0
 .INDENT 3.5
 Resume a batch experiment that was
 killed/stopped/etc last time SIERRA was run.
 .UNINDENT
 .UNINDENT
 .sp
@@ -2177,26 +2177,26 @@
 .INDENT 3.5
 Used by stage {2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: False
 .TP
-.B\-\-exec\-strict
+.B \-\-exec\-strict
 .INDENT 7.0
 .INDENT 3.5
 If passed, then if any experimental commands fail
 during stage 2 SIERRA will exit, rather than try
 to keep going and execute the rest of the
 experiments.
 .sp
 Useful for:
 .INDENT 0.0
 .IP \(bu 2
-"Correctness by construction" experiments, where
+\(dqCorrectness by construction\(dq experiments, where
 you know if SIERRA doesn\(aqt crash and it makes it
 to the end of your batch experiment then none of
 the individual experiments crashed.
 .IP \(bu 2
 CI pipelines
 .UNINDENT
 .UNINDENT
@@ -2217,40 +2217,40 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage1: Experiment generation
 .INDENT 0.0
 .TP
-.B\-\-exp\-setup
+.B \-\-exp\-setup
 .INDENT 7.0
 .INDENT 3.5
 Defines experiment run length, ticks per
 second for the experiment, # of datapoints
 to capture/capture interval for each
-simulation. See ln\-sierra\-vars\-expsetup for
+simulation. See \fI\%Experiment Setup\fP for
 a full description.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
-Default: "exp_setup.T1000.K5.N50"
+Default: \(dqexp_setup.T1000.K5.N50\(dq
 .TP
-.B\-\-robot
+.B \-\-robot
 .INDENT 7.0
 .INDENT 3.5
 The key name of the robot model, which must
 be present in the appropriate section of
-\fBmain.yaml\fP for the Project\&. See
+\fBmain.yaml\fP for the \fI\%Project\fP\&. See
 ln\-sierra\-tutorials\-project\-main\-config
 for details.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
@@ -2258,22 +2258,22 @@
 Used by stage {1}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS Stage1: Experiment generation
 .INDENT 0.0
 .TP
-.B\-\-skip\-sync
+.B \-\-skip\-sync
 .INDENT 7.0
 .INDENT 3.5
 If passed, then the generated experiment will not
 be synced to robots. This is useful when:
 .INDENT 0.0
 .IP \(bu 2
-You are developing your Project and
+You are developing your \fI\%Project\fP and
 just want to check locally if the experiment
 is being generated properly.
 .IP \(bu 2
 You have a lot of robots and/or the network
 connection from the SIERRA host machine to
 the robots is slow, and copying the
 experiment multiple times as you tweak
@@ -2301,33 +2301,33 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Stage2: Experiment executionFor running real robot experiments
 .INDENT 0.0
 .TP
-.B\-\-exec\-inter\-run\-pause
+.B \-\-exec\-inter\-run\-pause
 .INDENT 7.0
 .INDENT 3.5
-How long to pause between Experimental
-Runs, giving you time to
+How long to pause between \fI\%Experimental
+Runs\fP, giving you time to
 reset the environment, move robots, etc.
 .UNINDENT
 .UNINDENT
 .sp
 \fBTIP:\fP
 .INDENT 7.0
 .INDENT 3.5
 Used by stage {2}; can be omitted otherwise. If omitted: N/A.
 .UNINDENT
 .UNINDENT
 .sp
 Default: 60
 .TP
-.B\-\-exec\-resume
+.B \-\-exec\-resume
 .INDENT 7.0
 .INDENT 3.5
 Resume a batch experiment that was
 killed/stopped/etc last time SIERRA was
 run.
 .UNINDENT
 .UNINDENT
```

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra-examples.7` & `sierra-research-1.3.6/docs/_build/man/sierra-examples.7`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-EXAMPLES" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra-examples \- Examples of SIERRA usage. These examples all assume that you have successfully set up SIERRA with a project of your choice.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,31 +23,34 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA-EXAMPLES" "7" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra-examples \- Examples of SIERRA usage. These examples all assume that you have successfully set up SIERRA with a project of your choice.
 .sp
 This page contains reference examples of SIERRA usage to help you craft your own
 SIERRA invocation.  These examples use the SIERRA project plugins from the
-SIERRA sample project repo: \fI\%https://github.com:jharwell/sierra\-sample\-project.git\fP\&. See
-ln\-sierra\-trial or ln\-sierra\-getting\-started for setting up the
+SIERRA sample project repo: \fI\%https://github.com/jharwell/sierra\-sample\-project\fP\&. See
+\fI\%Trying Out SIERRA\fP or \fI\%Getting Started With SIERRA\fP for setting up the
 sample project repository.
 .sp
 In all examples:
 .INDENT 0.0
 .IP \(bu 2
 \fB$HOME/git/mycode\fP contains the ARGoS C++ library
 .IP \(bu 2
 \fB$HOME/git/sierra\-sample\-project/projects\fP contains the SIERRA project
 plugin
 .IP \(bu 2
 \fB$HOME/git/sierra\-sample\-project/projects\fP is on
-\fBSIERRA_PLUGIN_PATH\fP\&.
+\fI\%SIERRA_PLUGIN_PATH\fP\&.
 .UNINDENT
 .sp
 If your setup is different, adjust paths in the commands below as needed.
 .sp
 \fBIMPORTANT:\fP
 .INDENT 0.0
 .INDENT 3.5
@@ -98,15 +98,15 @@
 for robots to forage for. In fact, whatever is passed to \fB\-\-scenario\fP is
 totally arbitrary from SIERRA\(aqs point of view.
 .sp
 Within each experiment, 3 copies of each simulation will be run (each with
 different random seeds), for a total of 21 ARGoS simulations. On a reasonable
 machine it should take about 10 minutes or so to run. After it finishes, you can
 go to \fB$HOME/exp\fP and find all the simulation outputs. For an explanation of
-SIERRA\(aqs runtime directory tree, see ln\-sierra\-usage\-runtime\-exp\-tree\&.
+SIERRA\(aqs runtime directory tree, see \fI\%SIERRA Runtime Directory Tree\fP\&.
 .SS HPC Example
 .sp
 In order to run on a SLURM managed cluster, you need to invoke SIERRA within a
 script submitted with \fBsbatch\fP, or via \fBsrun\fP with the correspond cmdline
 options set.
 .INDENT 0.0
 .INDENT 3.5
@@ -124,15 +124,15 @@
 #SBATCH \-J argos\-slurm\-example
 
 # setup environment
 export ARGOS_INSTALL_PREFIX=/$HOME/.local
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$ARGOS_INSTALL_PREFIX/lib/argos3
 export ARGOS_PLUGIN_PATH=$ARGOS_INSTALL_PREFIX/lib/argos3:$HOME/git/mycode
 export SIERRA_PLUGIN_PATH=$HOME/git/sierra\-projects
-export PARALLEL="\-\-env ARGOS_PLUGIN_PATH \-\-env LD_LIBRARY_PATH"
+export PARALLEL=\(dq\-\-env ARGOS_PLUGIN_PATH \-\-env LD_LIBRARY_PATH\(dq
 
 sierra\-cli \e
 \-\-sierra\-root=$HOME/exp \e
 \-\-template\-input\-file=exp/your\-experiment.argos \e
 \-\-n\-runs=96 \e
 \-\-platform=platform.argos\e
 \-\-project=argos_project \e
@@ -153,25 +153,25 @@
 parallel, 6 at a time on each allocated node.  Each simulation will be 10,000
 seconds long and use \fBLowBlockCount\fP scenario in a 10x10x2 arena, as in the
 previous example.
 .sp
 \fBIMPORTANT:\fP
 .INDENT 0.0
 .INDENT 3.5
-You need to export \fBPARALLEL\fP containing all necessary
+You need to export \fI\%PARALLEL\fP containing all necessary
 environment variables your code uses in addition to those needed
 by SIERRA before invoking it, otherwise some of them might not be
 transferred to the SLURM job and/or the new shell GNU parallel
 starts each simulation in.
 .UNINDENT
 .UNINDENT
 .sp
 Note that if you compile ARGoS for different architectures within the same HPC
 environment, you can use a combination of conditionally setting
-\fBARGOS_PLUGIN_PATH\fP with setting \fBSIERRA_ARCH\fP to some string to
+\fI\%ARGOS_PLUGIN_PATH\fP with setting \fI\%SIERRA_ARCH\fP to some string to
 tell SIERRA to use a given version of ARGoS, depending on where you request
 resources from. For example, you could set \fBSIERRA_ARCH=x86\fP or
 \fBSIERRA_ARCH=arm\fP to link to an \fBargos3\-x86\fP or \fBargos3\-arm\fP executable
 and libraries, respectively.
 .SS Rendering Example
 .sp
 This example shows how to use ARGoS image capturing ability to create nice
@@ -198,15 +198,15 @@
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 The runs 3 simulations in parallel with 1 physics engine each, and runs ARGoS
 under \fBXvfb\fP to get it to render headless images. During stage 4, these
 images are stitched together using \fBffmpeg\fP to create videos (see
-ln\-sierra\-usage\-runtime\-exp\-tree for where the videos will appear). No
+\fI\%SIERRA Runtime Directory Tree\fP for where the videos will appear). No
 graphs are generated during stage 4 in this example.
 .sp
 You may also be interested in the \fB\-\-camera\-config\fP option, which allows you
 to specify different static/dynamic camera arrangements (e.g., do a nice
 circular pan around the arena during simulation).
 .sp
 \fBNOTE:\fP
@@ -354,15 +354,15 @@
 This will run a batch of 4 experiments using a correlated random walk controller
 (CRW) on the turtlebot3. Population size will be varied from 1..8, by powers
 of 2. Within each experiment, 4 copies of each simulation will be run (each with
 different random seeds), for a total of 16 Gazebo simulations. Each experimental
 run will be will be 10 seconds of simulated time. On a reasonable machine it
 should take about 10 minutes or so to run. After it finishes, you can go to
 \fB$HOME/exp\fP and find all the simulation outputs. For an explanation of
-SIERRA\(aqs runtime directory tree, see ln\-sierra\-usage\-runtime\-exp\-tree\&.
+SIERRA\(aqs runtime directory tree, see \fI\%SIERRA Runtime Directory Tree\fP\&.
 .SS HPC Example
 .sp
 In order to run on a SLURM managed cluster, you need to invoke SIERRA within a
 script submitted with \fBsbatch\fP, or via \fBsrun\fP with the correspond cmdline
 options set.
 .INDENT 0.0
 .INDENT 3.5
@@ -403,15 +403,15 @@
 In this example, the user requests 10 nodes with 24 cores each. SIERRA will run
 each of the 96 runs in parallel, 24 at a time on each allocated node.  Each
 simulation will be 1,000 seconds long and use same scenario as before.
 .sp
 \fBIMPORTANT:\fP
 .INDENT 0.0
 .INDENT 3.5
-You need to export \fBPARALLEL\fP containing all necessary
+You need to export \fI\%PARALLEL\fP containing all necessary
 environment variables your code uses in addition to those needed
 by SIERRA before invoking it, otherwise some of them might not be
 transferred to the SLURM job and/or the new shell GNU parallel
 starts each simulation in.
 .UNINDENT
 .UNINDENT
 .SS Bivariate Batch Criteria Example
@@ -470,19 +470,19 @@
 This will run a batch of 4 experiments using a correlated random walk controller
 (CRW) on the turtlebot3. Population size will be varied from 1,2,3,4,5,6. Within
 each experiment, 4 experimental runs will be conducted with each swarm
 size. SIERRA will pause for 60 seconds between runs so you can reset the robot\(aqs
 positions and environment before continuing with the next
 run. \fBturtlebots3.txt\fP contains the IP addresses of all 6 robots in the swarm
 (SIERRA may use different combinations of these if the swarm size is < 6).  You
-could also omit \fB\-\-nodefile\fP and set \fBSIERRA_NODEFILE\fP instead.
+could also omit \fB\-\-nodefile\fP and set \fI\%SIERRA_NODEFILE\fP instead.
 .sp
 For these experiments, no master node is needed, so it is disabled. After all
 runs have completed and SIERRA finishes stages 3 and 4, you can go to
 \fB$HOME/exp\fP and find all the simulation outputs. For an explanation of
-SIERRA\(aqs runtime directory tree, see ln\-sierra\-usage\-runtime\-exp\-tree\&.
+SIERRA\(aqs runtime directory tree, see \fI\%SIERRA Runtime Directory Tree\fP\&.
 .SH AUTHOR
 John Harwell
 .SH COPYRIGHT
 2022, John Harwell
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra-exec-envs.7` & `sierra-research-1.3.6/docs/_build/man/sierra-exec-envs.7`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-EXEC-ENVS" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra-exec-envs \- The execution environments SIERRA supports.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,28 +23,31 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA-EXEC-ENVS" "7" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra-exec-envs \- The execution environments SIERRA supports.
 .SH HPC EXECUTION ENVIRONMENT PLUGINS
 .sp
 SIERRA is capable of adapting its runtime infrastructure to a number of
 different HPC environments so that experiments can be run efficiently on
 whatever computational resources a researcher has access to. Supported
 environments that come with SIERRA are listed on this page.
 .sp
 These plugins tested with the following platforms (they may work on other
 platforms out of the box too):
 .INDENT 0.0
 .IP \(bu 2
-ln\-sierra\-platform\-plugins\-argos
+\fI\%ARGoS Platform\fP
 .IP \(bu 2
-ln\-sierra\-platform\-plugins\-ros1gazebo
+\fI\%ROS1+Gazebo Platform\fP
 .UNINDENT
 .sp
 SIERRA makes the following assumptions about the HPC environments corresponding
 to the plugins listed on this page:
 .SH HPC ENVIRONMENT ASSUMPTIONS
 .TS
 center;
@@ -102,15 +102,15 @@
 If more simulations are requested than can be run in parallel, SIERRA will start
 additional simulations as currently running simulations finish.
 .sp
 No additional configuration/environment variables are needed with this HPC
 environment for use with SIERRA.
 .SS ARGoS Considerations
 .sp
-The # threads per experimental run is defined with
+The # threads per \fI\%experimental run\fP is defined with
 \fB\-\-physics\-n\-engines\fP, and that option is required for this HPC environment
 during stage 1.
 .SS PBS HPC Plugin
 .sp
 This HPC environment can be selected via \fB\-\-exec\-env=hpc.pbs\fP\&.
 .sp
 In this HPC environment, SIERRA will run experiments spread across multiple
@@ -173,22 +173,22 @@
 T{
 Environment variable
 T}	T{
 Use
 T}
 _
 T{
-\fBSIERRA_ARCH\fP
+\fI\%SIERRA_ARCH\fP
 T}	T{
 Used to enable architecture/OS specific builds of simulators for maximum
 speed at runtime on clusters.
 T}
 _
 T{
-\fBPARALLEL\fP
+\fI\%PARALLEL\fP
 T}	T{
 Used to transfer environment variables into the GNU parallel
 environment. This must be always done because PBS doesn\(aqt transfer
 variables automatically, and because GNU parallel starts another level of
 child shells.
 T}
 _
@@ -263,22 +263,22 @@
 T{
 Environment variable
 T}	T{
 Use
 T}
 _
 T{
-\fBSIERRA_ARCH\fP
+\fI\%SIERRA_ARCH\fP
 T}	T{
 Used to enable architecture/OS specific builds of simulators for maximum
 speed at runtime on clusters.
 T}
 _
 T{
-\fBPARALLEL\fP
+\fI\%PARALLEL\fP
 T}	T{
 Used to transfer environment variables into the GNU parallel
 environment. This must be done even though SLURM can transfer variables
 automatically, because GNU parallel starts another level of child
 shells.
 T}
 _
@@ -307,22 +307,22 @@
 T}	T{
 Command line override
 T}	T{
 Notes
 T}
 _
 T{
-\fBSIERRA_NODEFILE\fP
+\fI\%SIERRA_NODEFILE\fP
 T}	T{
 Contains hostnames/IP address of all compute nodes SIERRA can use. Same
 format as GNU parallel \fB\-\-sshloginfile\fP\&.
 T}	T{
 \fB\-\-nodefile\fP
 T}	T{
-\fBSIERRA_NODEFILE\fP must be defined or \fB\-\-nodefile\fP passed. If
+\fI\%SIERRA_NODEFILE\fP must be defined or \fB\-\-nodefile\fP passed. If
 neither is true, SIERRA will throw an error.
 T}
 _
 .TE
 .SH AUTHOR
 John Harwell
 .SH COPYRIGHT
```

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra-glossary.7` & `sierra-research-1.3.6/docs/_build/man/sierra-glossary.7`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-GLOSSARY" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra-glossary \- Glossary of SIERRA terminology.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA-GLOSSARY" "7" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra-glossary \- Glossary of SIERRA terminology.
 .SH GLOSSARY
 .sp
 SIERRA uses a number of common research\-related terms, perhaps in different ways
 than you are used to. They are defined here to help demystify \fIwhy\fP SIERRA
 works/is designed the way it is, and to help you find your way around.
 .INDENT 0.0
 .TP
@@ -41,15 +41,15 @@
 A state\-of\-the\-art multi\-physics engine robotics simulator which SIERRA
 supports as a \fI\%Platform\fP\&. The ARGoS website is at
 \fI\%https://www.argos\-sim.info/index.php\fP\&.
 .TP
 .B Gazebo
 A state\-of\-the\-art robotics simulator with many features including .urdf
 robot models, realistic 3D rendering, and more. The Gazebo website is at
-\fI\%http://gazebosim.org\fP\&.
+\fI\%https://gazebosim.org\fP\&.
 .TP
 .B ROS1
 You know it. You either love it or hate it, but you can\(aqt escape it. The
 ROS website is at \fI\%https://wiki.ros.org\fP\&.
 .TP
 .B ROS1+Gazebo
 A \fI\%Platform\fP supported by SIERRA to use \fI\%ROS1\fP with the
@@ -67,43 +67,43 @@
 argument passed on the cmdline to sets of XML changes as part of
 \fI\%Experiment\fP definition.
 .sp
 \fBIMPORTANT:\fP
 .INDENT 7.0
 .INDENT 3.5
 The parent directories of all SIERRA project plugins must
-be on \fBSIERRA_PLUGIN_PATH\fP, or SIERRA won\(aqt be able
+be on \fI\%SIERRA_PLUGIN_PATH\fP, or SIERRA won\(aqt be able
 to find them.
 .UNINDENT
 .UNINDENT
 .sp
 \fBIMPORTANT:\fP
 .INDENT 7.0
 .INDENT 3.5
 You can\(aqt share projects across \fI\%Platforms\fP, so if you want to be able to use your project
 on ROS and ARGoS (for example), you will need to create 2
 separate projects with shared python code imported into
 each as needed.
 .UNINDENT
 .UNINDENT
 .sp
-Specified via \fB\-\-project\fP on the cmdline. See ln\-sierra\-usage\-cli for
+Specified via \fB\-\-project\fP on the cmdline. See \fI\%Command Line Interface\fP for
 documentation.
 .TP
 .B Tick
 A timestep. In SIERRA, physics engines will perform some number of
 iterations per tick, and after that the controllers for all agents will be
 run.
 .TP
 .B Batch Criteria
 A \fIvariable\fP you wish to use with SIERRA to measure its effect on system
 behavior. A batch criteria can has a single axis (such as
-ln\-sierra\-platform\-argos\-bc\-population\-size), in which case it is
+\fI\%Population Size\fP), in which case it is
 called \fIunivariate\fP, or have two axes (such as
-ln\-sierra\-platform\-argos\-bc\-population\-size and another batch
+\fI\%Population Size\fP and another batch
 criteria such as one defining sensor and actuator noise to apply to the
 robots), in which case it is called \fIbivariate\fP\&.
 .sp
 Univariate batch criteria have one dimension, and so the graphs produced
 by them are (usually) linegraphs with a numerical representation of the
 range for the variable on the X axis, and some other quantity of interest
 on the Y.
@@ -142,15 +142,15 @@
 SIERRA itself does not define any batch criteria.
 .TP
 .B Batch Experiment
 A set of \fI\%Experiments\fP each defined by XML changes
 generated by the selected \fI\%Batch Criteria\fP to a template \fB\&.argos\fP
 file passed to SIERRA during stage 1 via \fB\-\-template\-input\-file\fP\&.
 .sp
-For example, for the ln\-sierra\-platform\-argos\-bc\-population\-size
+For example, for the \fI\%Population Size\fP
 batch criteria, each experiment is defined by a single XML change to the
 provided \fB\&.argos\fP file: the number of robots in the swarm. Depending on
 the specifics you set for the \fIrange\fP of sizes you are interested in,
 several experiments will be generated from the template \fB\&.argos\fP file,
 each differing from the template in the configured swarm size.
 .TP
 .B Experiment
@@ -208,15 +208,15 @@
 after. However, you can also capture transient behaviors by creating
 \fI\%Collated .csv\fP and \fI\%Summary .csv\fP files from captured
 \fI\%Experimental Run\fP outputs over short stretches of time\-\-SIERRA does
 not know the difference.
 .TP
 .B Inter\-Batch .csv
 A CSV file created by SIERRA during stage 5. An inter\-batch CSV
-is created by "collating" columns from a \fI\%Summary .csv\fP present in
+is created by \(dqcollating\(dq columns from a \fI\%Summary .csv\fP present in
 multiple \fI\%Batch Experiments\fP into a single
 CSV. Used during stage 5.
 .TP
 .B Imagizing
 The process of turning a text file of some kind (e.g., CSV, \fB\&.gml\fP)
 into an image.
 .TP
@@ -241,15 +241,15 @@
 robots allocate tasks, you might create a \fBLN_task_alloc\fP label, so that
 you can enable/disable all task allocation related graphs for one or more
 controllers easily when configuring your project.
 .TP
 .B Controller Category
 A semantic label attached to a set of controllers which are similar in
 some way. For example, if you have two controllers which use the same type
-of memory (say it\(aqs a "last N objects seen" memory), you could create a
+of memory (say it\(aqs a \(dqlast N objects seen\(dq memory), you could create a
 \fBLastN\fP category, and then define controllers within it, e.g.,
 \fBLastN.Ring\fP and \fBLastN.DecayRing\fP for two controllers which have a
 ringbuffer of remembered objects and a decaying ringbuffer of remembered
 objects (i.e., an object is forgotten after some period of time even if it
 is not forced out of the ringbuffer by seeing a new object). See
 configuring your project.
 .TP
@@ -257,15 +257,15 @@
 A python implementation of a theoretical model of some kind. Can use
 empirical data from simulations/real robot experiments, or not, as
 needed. Intended to generate predictions of \fIsomething\fP which can then be
 plotted against empirical results for comparison.
 .TP
 .B Plugin
 A python package/module living in a directory on
-\fBSIERRA_PLUGIN_PATH\fP which contains functionality to extend SIERRA
+\fI\%SIERRA_PLUGIN_PATH\fP which contains functionality to extend SIERRA
 without modifying its core (i.e., customization of different parts of the
 pipeline). Plugins come in several flavors, all of which are handled
 equivalently by SIERRA:
 .INDENT 7.0
 .IP \(bu 2
 Pipeline plugins \- Plugins which provide different ways of executing
 core parts of the SIERRA pipeline (e.g., how to run experiments).
```

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra-platforms.7` & `sierra-research-1.3.6/docs/_build/man/sierra-platforms.7`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-PLATFORMS" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra-platforms \- The platforms SIERRA supports, and platform-specific Batch Criteria.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,26 +23,29 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA-PLATFORMS" "7" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra-platforms \- The platforms SIERRA supports, and platform-specific Batch Criteria.
 .SH ARGOS PLATFORM
 .sp
 This platform can be selected via \fB\-\-platform=platform.argos\fP\&.
 .sp
 This is the default platform on which SIERRA will run experiments, and uses the
-ARGoS simulator. It cannot be used to run experiments on real robots.
+\fI\%ARGoS\fP simulator. It cannot be used to run experiments on real robots.
 .SS Batch Criteria
 .sp
-See Batch Criteria for a thorough explanation of batch criteria, but the
+See \fI\%Batch Criteria\fP for a thorough explanation of batch criteria, but the
 short version is that they are the core of SIERRA\-\-how to get it to DO stuff for
 you.  The following batch criteria are defined which can be used with any
-Project\&.
+\fI\%Project\fP\&.
 .INDENT 0.0
 .IP \(bu 2
 \fI\%Population Size\fP
 .IP \(bu 2
 \fI\%Constant Population Density\fP
 .IP \(bu 2
 \fI\%Variable Population Density\fP
@@ -158,46 +158,46 @@
 .SS Examples
 .INDENT 0.0
 .IP \(bu 2
 \fBpopulation_variable_density.1p0.4p0.C4\fP: Densities of 1.0,2.0,3.0,4.0.
 .UNINDENT
 .SS Environment Variables
 .sp
-This platform respects \fBSIERRA_ARCH\fP\&.
+This platform respects \fI\%SIERRA_ARCH\fP\&.
 .SS Random Seeding For Reproducibility
 .sp
 ARGoS provides its own random seed mechanism under \fB<experiment>\fP which SIERRA
-uses to seed each experiment. Project code should use this mechanism or
+uses to seed each experiment. \fI\%Project\fP code should use this mechanism or
 a similar random seed generator manager seeded by the same value so that
 experiments can be reproduced exactly. By default SIERRA does not overwrite its
 generated random seeds for each experiment once generated; you can override with
 \fB\-\-no\-preserve\-seeds\fP\&. See ln\-sierra\-tutorials\-project\-template\-input\-file and
-ln\-sierra\-req\-exp for details on the format of the provided seed.
+\fI\%Experimental Definition Requirements\fP for details on the format of the provided seed.
 .SH ROS1+GAZEBO PLATFORM
 .sp
 This platform can be selected via \fB\-\-platform=platform.ros1gazebo\fP\&.
 .sp
 This is the platform on which SIERRA will run experiments using the
-Gazebo simulator and ROS1\&. It cannot be used to run
+\fI\%Gazebo\fP simulator and \fI\%ROS1\fP\&. It cannot be used to run
 experiments on real robots. To use this platform, you must setup the
-SIERRA ROSBridge\&.
+\fI\%SIERRA ROSBridge\fP\&.
 .sp
 Worlds within ROS1+Gazebo are infinite from the perspective of physics engines,
 even though a finite area shows up in rendering. So, to place robots randomly in
-the arena at the start of simulation across Experimental Runs (if you want to do that) "dimensions" for a given world must
+the arena at the start of simulation across \fI\%Experimental Runs\fP (if you want to do that) \(dqdimensions\(dq for a given world must
 be specified as part of the \fB\-\-scenario\fP argument. If you don\(aqt specify
 dimensions as part of the \fB\-\-scenario\fP argument, then you need to supply a
 list of valid robot positions via \fB\-\-robot\-positions\fP which SIERRA will choose
 from randomly for each robot.
 .SS Batch Criteria
 .sp
-See Batch Criteria for a thorough explanation of batch criteria, but the
+See \fI\%Batch Criteria\fP for a thorough explanation of batch criteria, but the
 short version is that they are the core of SIERRA\-\-how to get it to DO stuff for
 you.  The following batch criteria are defined which can be used with any
-Project\&.
+\fI\%Project\fP\&.
 .INDENT 0.0
 .IP \(bu 2
 \fI\%System Population Size\fP
 .UNINDENT
 .SS System Population Size
 .sp
 Changing the system size to investigate behavior across scales within a static
@@ -232,48 +232,48 @@
 .IP \(bu 2
 \fBpopulation_size.Linear3.C3\fP: Static population sizes 1...3 (3)
 .IP \(bu 2
 \fBpopulation_size.Linear10.C2\fP: Static population sizes 5...10 (2)
 .UNINDENT
 .SS Environment Variables
 .sp
-This platform ignores \fBSIERRA_ARCH\fP\&.
+This platform ignores \fI\%SIERRA_ARCH\fP\&.
 .SS Random Seeding For Reproducibility
 .sp
 ROS1+Gazebo do not provide a random number generator manager, but SIERRA
-provides random seeds to each Experimental Run which Project
+provides random seeds to each \fI\%Experimental Run\fP which \fI\%Project\fP
 code should use to manage random number generation, if needed, to maximize
 reproducability. See ln\-sierra\-tutorials\-project\-template\-input\-file and
-ln\-sierra\-req\-exp for details on the format of the provided seed. By default
+\fI\%Experimental Definition Requirements\fP for details on the format of the provided seed. By default
 SIERRA does not overwrite its generated random seeds for each experiment once
 generated; you can override with \fB\-\-no\-preserve\-seeds\fP\&.
 .SH ROS1+ROBOT PLATFORM
 .sp
 This platform can be selected via \fB\-\-platform=platform.ros1robot\fP\&.
 .sp
-This is the platform on which SIERRA will run experiments using ROS1 on
+This is the platform on which SIERRA will run experiments using \fI\%ROS1\fP on
 a real robot of your choice. To use this platform, you must setup the
-SIERRA ROSBridge\&.  This is a generic
-platform meant to work with most real robots which ROS1 supports, and as
+\fI\%SIERRA ROSBridge\fP\&.  This is a generic
+platform meant to work with most real robots which \fI\%ROS1\fP supports, and as
 a starting point to derive more specific platform configuration for a given
 robot (if needed). For all execution environments using this platform (see
-ln\-sierra\-exec\-env\-robot for examples), SIERRA will run experiments
+\fI\%Real Robot Execution Environment Plugins\fP for examples), SIERRA will run experiments
 spread across multiple robots using GNU parallel.
 .sp
 SIERRA designates the host machine as the ROS master, and allows you to
 (optionally) specify configuration for running one or more nodes on it in the
 \fB\-\-template\-input\-file\fP to gather data from robots (see below). This is
 helpful in some situations (e.g., simple robots which can\(aqt manage network
 mounted filesystems).
 .SS Batch Criteria
 .sp
-See Batch Criteria for a thorough explanation of batch criteria, but the
+See \fI\%Batch Criteria\fP for a thorough explanation of batch criteria, but the
 short version is that they are the core of SIERRA\-\-how to get it to DO stuff for
 you. The following batch criteria are defined which can be used with any
-Project\&.
+\fI\%Project\fP\&.
 .INDENT 0.0
 .IP \(bu 2
 \fI\%System Population Size\fP
 .UNINDENT
 .SS System Population Size
 .sp
 Changing the system size to investigate behavior across scales within a static
@@ -307,52 +307,52 @@
 .IP \(bu 2
 \fBpopulation_size.Linear3.C3\fP: Static population sizes 1...3 (3)
 .IP \(bu 2
 \fBpopulation_size.Linear10.C2\fP: Static population sizes 5...10 (2)
 .UNINDENT
 .SS Environment Variables
 .sp
-This platform ignores \fBSIERRA_ARCH\fP\&.
+This platform ignores \fI\%SIERRA_ARCH\fP\&.
 .SS Random Seeding For Reproducibility
 .sp
 ROS do not provide a random number generator manager, but SIERRA provides random
-seeds to each Experimental Run which Project code should use to
+seeds to each \fI\%Experimental Run\fP which \fI\%Project\fP code should use to
 manage random number generation, if needed, to maximize reproducability. See
 ln\-sierra\-tutorials\-project\-template\-input\-file and
-ln\-sierra\-req\-exp for details on the format of the provided seed. By
+\fI\%Experimental Definition Requirements\fP for details on the format of the provided seed. By
 default SIERRA does not overwrite its generated random seeds for each experiment
 once generated; you can override with \fB\-\-no\-preserve\-seeds\fP\&.
 .SS Real Robot Considerations
 .sp
 SIERRA makes the following assumptions about the robots it is allocated each
 invocation:
 .INDENT 0.0
 .IP \(bu 2
-No robots will die/run out of battery during an Experimental Run\&.
+No robots will die/run out of battery during an \fI\%Experimental Run\fP\&.
 .IP \(bu 2
 Password\-less ssh is setup to each robot SIERRA is handed to use (can be as a
 different user than the one which is invoking SIERRA on the host machine).
 .IP \(bu 2
 The robots have static IP addresses, or are always allocated an IP from a
 known set so you can pass the set of IPs to SIERRA to use. This set of IP
 address/hostnames can be explicitly passed to SIERRA via cmdline (see
-ln\-sierra\-usage\-cli) or implicitly passed via
-\fBSIERRA_NODEFILE\fP\&.
+\fI\%Command Line Interface\fP) or implicitly passed via
+\fI\%SIERRA_NODEFILE\fP\&.
 .IP \(bu 2
 The ROS environment is setup either in the .bashrc for the robot login user,
 or the necessary bits are in a script which SIERRA sources on login to each
 robot (this is a configuration parameter\-\-see
 ln\-sierra\-tutorials\-project\-main\-config).
 .IP \(bu 2
-ROS does not provide a way to say "Run this experiment for X seconds", so
+ROS does not provide a way to say \(dqRun this experiment for X seconds\(dq, so
 SIERRA inserts its own timekeeper node into each robot which will exit after X
 seconds and take the roslaunch process with it on each robot and/or the master
 node.
 .UNINDENT
 .sp
-See also ln\-sierra\-req\-code\-ros1robot\&.
+See also \fI\%ROS1+Robot Platform\fP\&.
 .SH AUTHOR
 John Harwell
 .SH COPYRIGHT
 2022, John Harwell
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra-usage.7` & `sierra-research-1.3.6/docs/_build/man/sierra-usage.7`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-USAGE" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra-usage \- How to use SIERRA. This covers all non-command line interface aspects.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,45 +23,48 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA-USAGE" "7" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra-usage \- How to use SIERRA. This covers all non-command line interface aspects.
 .sp
-This covers everything which is (mostly) Platform independent and is not
+This covers everything which is (mostly) \fI\%Platform\fP independent and is not
 the command line interface.
 .SH SIERRA PIPELINE
 .sp
 When invoked SIERRA will run one or more stages of its execution path, as
 specified via \fB\-\-pipeline\fP on the cmdline. Only the first 4 pipeline stages
 will run by default. The pipeline stages are:
 .SS Stage 1: Experiment Generation
 .sp
 Experiments using the scientific method have an independent variable whose
 impact on results are measured through a series of trials. SIERRA allows you to
 express this as a research query on the command line, and then parses your query
 to make changes to a template input file to generate launch commands and
 experimental inputs to operationalize it. Switching from targeting platform A
 (e.g., ARGoS) to platform B (e.g., ROS1+Gazebo) is as easy as changing a single
-command line argument. SIERRA handles the "backend" aspects of defining
+command line argument. SIERRA handles the \(dqbackend\(dq aspects of defining
 experimental inputs allowing you to focus on their \fIcontent\fP, rather than the
 mechanics of how to turn the content into something that can be executed. See
 also:
 .INDENT 0.0
 .IP \(bu 2
-ln\-sierra\-support\-matrix
+\fI\%SIERRA Support Matrix\fP
 .IP \(bu 2
-ln\-sierra\-usage\-cli
+\fI\%Command Line Interface\fP
 .UNINDENT
 .sp
 Part of default pipeline.
 .SS Stage 2: Experiment Execution
 .sp
-SIERRA runs a previously generated Batch Experiment\&. Exactly which batch
+SIERRA runs a previously generated \fI\%Batch Experiment\fP\&. Exactly which batch
 experiment SIERRA runs is determined by:
 .INDENT 0.0
 .IP \(bu 2
 \fB\-\-controller\fP
 .IP \(bu 2
 \fB\-\-scenario\fP
 .IP \(bu 2
@@ -78,37 +78,37 @@
 SIERRA currently supports two types of execution environments: simulators and
 real robots, which are handled seamlessly. For simulators, SIERRA will run
 multiple experimental runs from each experiment in parallel if possible. Similar
 to stage 1, switching between execution environments is as easy as changing a
 single command line argument. See also:
 .INDENT 0.0
 .IP \(bu 2
-ln\-sierra\-exec\-env\-plugins
+\fI\%Execution Environment Plugins\fP
 .IP \(bu 2
-ln\-sierra\-platform\-plugins
+\fI\%Platform Plugins\fP
 .IP \(bu 2
-ln\-sierra\-support\-matrix
+\fI\%SIERRA Support Matrix\fP
 .UNINDENT
 .sp
 Part of default pipeline.
 .SS Stage 3: Experiment Post\-Processing
 .sp
 SIERRA supports a number of data formats which simulations/real robot
 experiments can output their data, e.g., the number of robots engaged in a given
 task over time for processing.  SIERRA post\-processes experimental results after
 running the batch experiment; some parts of this can be done in parallel. This
 includes one or more of:
 .INDENT 0.0
 .IP \(bu 2
 Computing statistics over/about experimental data for stage 4 for use in graph
-generation in stage 4. See ln\-sierra\-usage\-cli documentation for
+generation in stage 4. See \fI\%Command Line Interface\fP documentation for
 \fB\-\-dist\-stats\fP for details.
 .IP \(bu 2
 Creating images from project CSV files for rendering in stage 4. See
-ln\-sierra\-usage\-rendering\-project for details.
+\fI\%Project Rendering\fP for details.
 .UNINDENT
 .sp
 Part of default pipeline.
 .SS Stage 4: Deliverable Generation
 .sp
 SIERRA can generate many deliverables from the processed experimental results
 automatically (independent of the platform/execution environment!), thus greatly
@@ -124,75 +124,75 @@
 Videos built from captured experimental output .csv files.
 .UNINDENT
 .sp
 SIERRA also has a rich model framework allowing you to run arbitrary models,
 generate data, and plot it on the same figure as empirical results,
 automatically. See ln\-sierra\-tutorials\-project\-models for details.
 .sp
-For some examples, see the "Generating Deliverables" section of
-\fI\%2022 AAMAS Demo\fP <\fBhttps://www-users.cse.umn.edu/~harwe006/showcase/aamas-2022-demo\fP>\&. See ln\-sierra\-usage\-rendering for details about
+For some examples, see the \(dqGenerating Deliverables\(dq section of
+\fI\%2022 AAMAS Demo\fP <\fBhttps://www-users.cse.umn.edu/~harwe006/showcase/aamas-2022-demo\fP>\&. See \fI\%Rendering\fP for details about
 rendering capabilities.
 .sp
 Part of default pipeline.
 .SS Stage 5: Graph Generation for Controller/Scenario Comparison
 .sp
 SIERRA can perform additional graph generation \fIAFTER\fP graph generation for
 batch experiments has been run. This is extremely useful for generating graphs
 which can be dropped immediately into academic papers without modification. This
 can be used to compare:
 .INDENT 0.0
 .IP \(bu 2
 Different agent control algorithms which have all been run in the same
-\fB\-\-scenario\fP\&. See ln\-sierra\-usage\-stage5\-intra\-scenario for details.
+\fB\-\-scenario\fP\&. See \fI\%Intra\-Scenario Comparison\fP for details.
 .IP \(bu 2
 A single \fB\-\-controller\fP across multiple scenarios. See
-ln\-sierra\-usage\-stage5\-inter\-scenario for details.
+\fI\%Inter\-Scenario Comparison\fP for details.
 .UNINDENT
 .sp
 Not part of default pipeline.
 .SH PIPELINE STAGE 5
 .sp
-The main idea of this pipeline stage is to "collate" the results of one or more
-Summary .csv files present in different Batch Experiments into a Inter\-Batch .csv file, and then use that file to
-generate graphs. Any Summary .csv that is present in multiple
-Batch Experiments can be used during stage 5!  This
+The main idea of this pipeline stage is to \(dqcollate\(dq the results of one or more
+\fI\%Summary .csv\fP files present in different \fI\%Batch Experiments\fP into a \fI\%Inter\-Batch .csv\fP file, and then use that file to
+generate graphs. Any \fI\%Summary .csv\fP that is present in multiple
+\fI\%Batch Experiments\fP can be used during stage 5!  This
 gives this pipeline stage tremendous flexibility as a camera\-ready graph
 generation tool.
 .sp
 In general, stage 5 is always run separate from stages 1\-4 (i.e., a separate
 SIERRA invocation), because the options are quite different, but you don\(aqt
 \fIhave\fP to do this.
 .sp
 \fBIMPORTANT:\fP
 .INDENT 0.0
 .INDENT 3.5
 You \fIcannot\fP use this stage before successfully running stage 4
-for each of the Batch Experiments you
+for each of the \fI\%Batch Experiments\fP you
 want to include on the final graph.
 .UNINDENT
 .UNINDENT
 .sp
 \fBWARNING:\fP
 .INDENT 0.0
 .INDENT 3.5
 Because SIERRA never deletes stuff for you, running stage 5 is
 \fINOT\fP idempotent. Running the same stage 5 invocation comparing 3
 controllers in a single scenario (for example) could result in
 linegraphs containing 3,6,9,..., lines with duplicated data. In
 general, you want to delete the directories generated by stage 5
 between successive runs. See
-ln\-sierra\-usage\-runtime\-exp\-tree for details on what
+\fI\%SIERRA Runtime Directory Tree\fP for details on what
 directories are generated.
 .UNINDENT
 .UNINDENT
 .SS Intra\-Scenario Comparison
 .sp
 Intra\-scenario comparison compares the of experiments using one or more
 controllers on the same \fB\-\-scenario\fP\&. To use it, you need to pass the
-following options to SIERRA (see ln\-sierra\-usage\-cli for documentation):
+following options to SIERRA (see \fI\%Command Line Interface\fP for documentation):
 .INDENT 0.0
 .IP \(bu 2
 \fB\-\-scenario\-comparison\fP
 .IP \(bu 2
 \fB\-\-bc\-univar\fP or \fB\-\-bc\-bivar\fP
 .IP \(bu 2
 \fB\-\-dist\-stats\fP (to get statistics generated during stage 3 to show up on the
@@ -204,15 +204,15 @@
 .sp
 For YAML configuration, see
 ln\-sierra\-tutorials\-project\-stage5\-config\-intra\&.
 .SS Inter\-Scenario Comparison
 .sp
 Inter\-scenario comparison compares the same \fB\-\-controller\fP across multiple
 \fB\-\-scenarios\fP\&. To use it, you need to pass the following options to SIERRA
-when running stage 5 (see ln\-sierra\-usage\-cli for documentation):
+when running stage 5 (see \fI\%Command Line Interface\fP for documentation):
 .INDENT 0.0
 .IP \(bu 2
 \fB\-\-controller\-comparison\fP
 .IP \(bu 2
 \fB\-\-bc\-univar\fP or \fB\-\-bc\-bivar\fP
 .IP \(bu 2
 \fB\-\-dist\-stats\fP (to get statistics generated during stage 3 to show up on the
@@ -293,26 +293,26 @@
 for a previously used project on subsequent runs.
 .INDENT 2.0
 .IP \(bu 2
 \fBCATEGORY.my_controller\fP \- Each controller gets their own directory in the
 project root, which is \fBNOT\fP deleted on subsequent runs.
 .INDENT 2.0
 .IP \(bu 2
-\fBmytemplate\-SS.12x6\fP \- The directory for the Batch Experiment
+\fBmytemplate\-SS.12x6\fP \- The directory for the \fI\%Batch Experiment\fP
 is named from a combination of the template input file used
 (\fB\-\-template\-input\-file\fP) and the scenario (\fB\-\-scenario\fP).
 .INDENT 2.0
 .IP \(bu 2
-\fBexp\-inputs\fP \- Root directory for Experimental
+\fBexp\-inputs\fP \- Root directory for \fI\%Experimental\fP
 inputs; each experiment in the batch gets their own directory in here.
 .INDENT 2.0
 .IP \(bu 2
 \fBexp0\fP \- Within the input directory for each experiment in the
 batch (there are 4 such directories in this example), there will be
-an input file for each Experimental Run in the experiment,
+an input file for each \fI\%Experimental Run\fP in the experiment,
 as well as a \fBcommands.txt\fP used by GNU parallel to run them all
 in parallel. The leaf of the \fB\-\-template\-input\-file\fP, sans
 extension, has the experimental run # appended to it
 (e.g. \fBmy\-template_0.argos\fP is the input file for simulation 0).
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
@@ -397,36 +397,36 @@
 .IP \(bu 2
 \fBexp1\fP
 .IP \(bu 2
 \fBexp2\fP
 .IP \(bu 2
 \fB\&...\fP
 .IP \(bu 2
-\fBcollated\fP \- Contains Collated .csv files. During
+\fBcollated\fP \- Contains \fI\%Collated .csv\fP files. During
 stage4, SIERRA will draw specific columns from .csv files under
 \fBstatistics\fP according to configuration, and collate them under
 here for graph generation of \fIinter\fP\-experiment graphs.
 .IP \(bu 2
 \fBexec\fP \- Statistics about SIERRA runtime. Useful for capturing
 runtime of specific experiments to better plan/schedule time on
 HPC clusters.
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
 \fBimagize\fP \- Root directory for holding imagized files (averaged run
 outputs which have been converted to graphs) which can be patched
 together in stage 4 to generated videos. Each experiment will get its
 own directory under here, with unique sub\-directories for each
-different type of Experimental Run data captured for
-imagizing. See ln\-sierra\-usage\-rendering\-project for more details.
+different type of \fI\%Experimental Run\fP data captured for
+imagizing. See \fI\%Project Rendering\fP for more details.
 .IP \(bu 2
 \fBvideos\fP \- Root directory for holding rendered videos generated
 during stage 4 from either captured simulator frames for imagized
 project files. Each experiment will get its own directory under here,
-with See ln\-sierra\-usage\-rendering for more details.
+with See \fI\%Rendering\fP for more details.
 .IP \(bu 2
 \fBmodels\fP \- During stage4, the dataframes generated by all executed
 models are stored under this directory. Each experiment in the batch
 gets their own directory for \fIintra\fP\-experiment models.
 .IP \(bu 2
 \fBgraphs\fP \- During stage4, all generated graphs are output under this
 directory. Each experiment in the batch gets their own directory for
@@ -463,15 +463,15 @@
 .sp
 .nf
 .ft C
 \-\-pipeline 5\e
 \-\-scenario\-comparison\e
 \-\-batch\-criteria population_size.Log8\e
 \-\-scenarios\-list=RN.16x16x2,PL.16x16x2\e
-\-\-sierra\-root=$HOME/exp"
+\-\-sierra\-root=$HOME/exp\(dq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 This invocation will cause SIERRA to create the following directory structure as
 it runs:
@@ -497,15 +497,15 @@
 .sp
 .nf
 .ft C
 \-\-pipeline 5\e
 \-\-controller\-comparison\e
 \-\-batch\-criteria population_size.Log8\e
 \-\-controllers\-list d0.CRW,d0.DPO\e
-\-\-sierra\-root=$HOME/exp"
+\-\-sierra\-root=$HOME/exp\(dq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 This invocation will cause SIERRA to create the following directory structure as
 it runs:
@@ -527,43 +527,43 @@
 .SH SIERRA SUBPROGRAMS
 .sp
 These are the shell programs which SIERRA \fImay\fP use internally when running,
 depending on what you are doing.
 .INDENT 0.0
 .IP \(bu 2
 \fBparallel\fP \- GNU parallel. Used during stage 2 when running
-experiments (ARGoS, ROS1+Gazebo, ROS1+Robot platforms).
+experiments (\fI\%ARGoS\fP, \fI\%ROS1+Gazebo\fP, \fI\%ROS1+Robot\fP platforms).
 .IP \(bu 2
 \fBffmpeg\fP \- Used during stage 3 if imagizing is run. See
-ln\-sierra\-usage\-rendering\-platform\&.
+\fI\%Platform Visual Capture\fP\&.
 .IP \(bu 2
 \fBXvfb\fP \- Used during stage 1 when generating simulation inputs, and
-during stage 2 when running experiments for the ARGoS
-Platform\&. See also ln\-sierra\-usage\-rendering\-platform\&.
+during stage 2 when running experiments for the \fI\%ARGoS\fP
+\fI\%Platform\fP\&. See also \fI\%Platform Visual Capture\fP\&.
 .IP \(bu 2
 \fBparallel\-ssh\fP \- Used during stage 1 when generating experiments
-experiments (ROS1+Robot platform).
+experiments (\fI\%ROS1+Robot\fP platform).
 .IP \(bu 2
 \fBparallel\-rsync\fP \- Used during stage 1 when generating experiments
-experiments (ROS1+Robot platform).
+experiments (\fI\%ROS1+Robot\fP platform).
 .UNINDENT
 .SH ENVIRONMENT VARIABLES
 .INDENT 0.0
 .TP
 .B SIERRA_PLUGIN_PATH
-Used for locating plugins\&. The directory \fIcontaining\fP a
+Used for locating \fI\%plugins\fP\&. The directory \fIcontaining\fP a
 plugin directory outside the SIERRA source tree must be on
 \fBSIERRA_PLUGIN_PATH\fP\&. Paths are added to \fBPYTHONPATH\fP as needed to load
 plugins correctly. For example, if you have a different version of the
 \fB\-\-storage\-medium\fP plugin you\(aqd like to use, and you have but the directory
 containing the plugin in \fB$HOME/plugins\fP, then you need to add
 \fB$HOME/plugins\fP to your \fBSIERRA_PLUGIN_PATH\fP to so that SIERRA will find
 it. This variable is used in stages 1\-5.
 .sp
-Used for locating projects; all projects specifiable with
+Used for locating \fI\%projects\fP; all projects specifiable with
 \fB\-\-project\fP are directories found within the directories on this path. For
 example, if you have a project \fB$HOME/git/projects/myproject\fP, then
 \fB$HOME/git\fP must be on \fBSIERRA_PLUGIN_PATH\fP in order for you to be able
 to specify \fB\-\-project=myproject\fP\&. This variable is used in stages 1\-5.
 .sp
 You \fIcannot\fP just put the parent directory of your project on
 \fI\%PYTHONPATH\fP because SIERRA uses this path for other things
@@ -577,17 +577,17 @@
 .INDENT 0.0
 .TP
 .B ARGOS_PLUGIN_PATH
 Must be set to contain the library directory where you installed/built ARGoS,
 as well as the library directory for your project \fB\&.so\fP\&. Checked to be
 non\-empty before running stage 2 for all \fB\-\-exec\-env\fP plugins. SIERRA does
 \fInot\fP modify this variable, so it needs to be setup properly prior to
-invoking SIERRA (i.e., the directory containing the Project \fB\&.so\fP
+invoking SIERRA (i.e., the directory containing the \fI\%Project\fP \fB\&.so\fP
 file needs to be on it). SIERRA can\(aqt know, in general, where the location of
-the C++ code corresponding to the loaded Project is.
+the C++ code corresponding to the loaded \fI\%Project\fP is.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B SIERRA_ARCH
 Can be used to determine the names of executables launch in HPC environment,
 so that in environments with multiple queues/sub\-clusters with different
 architectures simulators can be compiled natively for each for maximum
@@ -613,24 +613,24 @@
 Used by SIERRA to configure experiments during stage 1,2; if it is not
 defined and \fB\-\-nodefile\fP is not passed SIERRA will throw an error.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B PARALLEL
 When running on some execution environments, such as \fBhpc.slurm,hpc.pbs\fP,
-any and all environment variables needed by your Project should be
+any and all environment variables needed by your \fI\%Project\fP should be
 exported via the \fBPARALLEL\fP environment variable before invoking SIERRA,
 because GNU parallel does not export the environment of the node it is
 launched from to slave nodes (or even on the local machine). Something like:
 .INDENT 7.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-export PARALLEL="\-\-workdir . \e
+export PARALLEL=\(dq\-\-workdir . \e
 \-\-env PATH \e
 \-\-env LD_LIBRARY_PATH \e
 \-\-env LOADEDMODULES \e
 \-\-env _LMFILES_ \e
 \-\-env MODULE_VERSION \e
 \-\-env MODULEPATH \e
 \-\-env MODULEVERSION_STACK
@@ -640,27 +640,27 @@
 \-\-env OMP_NESTED \e
 \-\-env OMP_NUM_THREADS \e
 \-\-env OMP_SCHEDULE \e
 \-\-env OMP_STACKSIZE \e
 \-\-env OMP_THREAD_LIMIT \e
 \-\-env OMP_WAIT_POLICY \e
 \-\-env SIERRA_ARCH \e
-\-\-env SIERRA_PLUGIN_PATH"
+\-\-env SIERRA_PLUGIN_PATH\(dq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 Don\(aqt forget to include \fI\%ARGOS_PLUGIN_PATH\fP,
-\fI\%ROS_PACKAGE_PATH\fP, etc., depending on your chosen Platform\&.
+\fI\%ROS_PACKAGE_PATH\fP, etc., depending on your chosen \fI\%Platform\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B PARALLEL_SHELL
-SIERRA sets up the Experiment execution environments by running one
+SIERRA sets up the \fI\%Experiment\fP execution environments by running one
 or more shell commands in a subprocess (treated as a \fBshell\fP, which means
 that \fBparallel\fP can\(aqt determine \fBSHELL\fP, and therefore defaults to
 \fB/bin/sh\fP, which is not what users expect. SIERRA explicitly sets
 \fBPARALLEL_SHELL\fP to the result of \fBshutil.which(\(aqbash\(aq)\fP in keeping with
 the Principle Of Least Surprise.
 .UNINDENT
 .INDENT 0.0
@@ -669,40 +669,40 @@
 The list of directories which defines where ROS will search for
 packages. SIERRA does \fInot\fP modify this variable, so it needs to be setup
 properly prior to invoking SIERRA (i.e., sourcing the proper \fBsetup.bash\fP
 script).
 .UNINDENT
 .SH CONFIGURABLE SIERRA VARIABLES
 .sp
-Non\-Batch Criteria variables which you can use to configure
+Non\-\fI\%Batch Criteria\fP variables which you can use to configure
 simulations. All batch criteria are variables, but not all variables are batch
 criteria.
 .INDENT 0.0
 .IP \(bu 2
 \fI\%Experiment Setup\fP
 .UNINDENT
 .SS Experiment Setup
 .sp
-Configure Experiment time: length, controller cadence (Tick
-duration/timestep), and how many datapoints to capture per Experimental
-Run\&.
+Configure \fI\%Experiment\fP time: length, controller cadence (\fI\%Tick\fP
+duration/timestep), and how many datapoints to capture per \fI\%Experimental
+Run\fP\&.
 .SS Cmdline Syntax
 .sp
 \fBT{duration}[.K{ticks_per_sec}][.N{n_datapoints}\fP
 .INDENT 0.0
 .IP \(bu 2
 \fBduration\fP \- Duration of timesteps in \fIseconds\fP (not timesteps).
 .IP \(bu 2
 \fBticks_per_sec\fP \- How many times each controller will be run per second.
 .IP \(bu 2
-\fBn_datapoints\fP \- # datapoints per Experimental Run to be captured;
+\fBn_datapoints\fP \- # datapoints per \fI\%Experimental Run\fP to be captured;
 the capture interval (if configurable) should be adjusted in
-Project\-derived class from the platform "Experiment setup class"
+\fI\%Project\fP\-derived class from the platform \(dqExperiment setup class\(dq
 (e.g., \fBsierra.plugins.platform.argos.variables.exp_setup.ExpSetup\fP for
-ARGoS).
+\fI\%ARGoS\fP).
 .UNINDENT
 .SS Examples
 .INDENT 0.0
 .IP \(bu 2
 \fBexp_setup.T1000\fP: Experimental run will be 1,000 seconds long and have
 1,000*5=5,000 timesteps, with default (50) # datapoints.
 .IP \(bu 2
```

### Comparing `sierra-research-1.3.5/docs/_build/man/sierra.7` & `sierra-research-1.3.6/docs/_build/man/sierra.7`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
-.SH NAME
-sierra \- reSearch pIpEline for Reproducability, Reusability, and Automation.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,17 +23,20 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "SIERRA" "7" "Apr 01, 2024" "1.3.6" "SIERRA"
+.SH NAME
+sierra \- reSearch pIpEline for Reproducability, Reusability, and Automation.
 .SH SYNOPSIS
 .sp
-This the "main menu" of the SIERRA reference manual, which captures most, but
+This the \(dqmain menu\(dq of the SIERRA reference manual, which captures most, but
 not all of its documentation. For the full experience, look at the online docs
 at \fI\%https://sierra.readthedocs.io/en/master\fP\&.
 .SH COMPONENTS
 .sp
 The following manpages are available:
 .INDENT 0.0
 .IP \(bu 2
@@ -61,15 +61,15 @@
 .sp
 Generally speaking, SIERRA is very conservative, and uses lots of assert()s to
 verify its internal state and the state of a given experiment at a given step of
 execution before proceeding to the next step. SIERRA should rarely crash with a
 cryptic interpreter error message/exception, but if it does, please report it so
 I can fix it and/or create a better error message.
 .sp
-Errors should be reported to \fI\%https://github.com:jharwell/sierra.git\fP\&.
+Errors should be reported to \fI\%https://github.com/jharwell/sierra\fP\&.
 .SH RETURN VALUE
 .sp
 SIERRA will always return 0, unless it crashes with an exception or a failed
 assert, in which case the return code will be non\-zero.
 .SH AUTHOR
 John Harwell
 .SH COPYRIGHT
```

### Comparing `sierra-research-1.3.5/docs/_ext/xref.py` & `sierra-research-1.3.6/docs/_ext/xref.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/_templates/autoapi/module.rst` & `sierra-research-1.3.6/docs/_templates/autoapi/module.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/conf.py` & `sierra-research-1.3.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,29 +145,29 @@
 autoapi_ignore = ['*flycheck*']
 xref_links = {
     "Harwell2021a-metrics": ("Improved Swarm Engineering: Aligning Intuition and Analysis",
                              "https://arxiv.org/pdf/2012.04144.pdf"),
     "Harwell2022b-ode": ("Characterizing The Limits of Linear Modeling of Non-Linear Swarm Behaviors",
                          "https://arxiv.org/abs/2110.12307"),
     "Harwell2020a-demystify": ("Demystifying Emergent Intelligence and Its Effect on Performance in Large Swarms",
-                               "http://ifaamas.org/Proceedings/aamas2020/pdfs/p474.pdf"),
+                               "https://ifaamas.org/Proceedings/aamas2020/pdfs/p474.pdf"),
     "Harwell2019a-metrics": ("Swarm Engineering Through Quantitative Measurement in a 10,000 Robot Swarm",
                              "https://www.ijcai.org/Proceedings/2019/0048.pdf"),
     "White2019-social": ("Socially Inspired Communication in Swarm Robotics",
                          "https://arxiv.org/abs/1906.01108"),
     "Chen2019-battery": ("Maximizing Energy Efficiency in Swarm Robotics",
                          "https://arxiv.org/abs/1906.01957"),
     "Hecker2015": ("Hecker2015",
                    "https://www.cs.unm.edu/~wjust/CS523/S2018/Readings/Hecker_Beyond_Pheromones_Swarm_Intelligence.pdf"),
     "Rosenfeld2006": ("Rosenfeld2006",
-                      "http://users.umiacs.umd.edu/~sarit/data/articles/rosenfeldetalbook06.pdf"),
-    "SIERRA_GITHUB": ("https://github.com:jharwell/sierra.git",
-                      "https://github.com:jharwell/sierra.git"),
-    "SIERRA_SAMPLE_PROJECT": ("https://github.com:jharwell/sierra-sample-project.git",
-                              "https://github.com:jharwell/sierra-sample-project.git"),
+                      "https://users.umiacs.umd.edu/~sarit/data/articles/rosenfeldetalbook06.pdf"),
+    "SIERRA_GITHUB": ("https://github.com/jharwell/sierra",
+                      "https://github.com/jharwell/sierra"),
+    "SIERRA_SAMPLE_PROJECT": ("https://github.com/jharwell/sierra-sample-project",
+                              "https://github.com/jharwell/sierra-sample-project"),
     "SIERRA_DOCS": ("https://sierra.readthedocs.io/en/master",
                     "https://sierra.readthedocs.io/en/master"),
     "FORDYCA": ("FORDYCA", "https://swarm-robotics-fordyca.readthedocs.io"),
     "PRISM": ("PRISM", "https://swarm-robotics-prism.readthedocs.io"),
     "2022-aamas-demo": ("2022 AAMAS Demo",
                         "https://www-users.cse.umn.edu/~harwe006/showcase/aamas-2022-demo")
 
@@ -306,15 +306,15 @@
     'python3': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
     'matplotlib': ('https://matplotlib.org', None),
     'sphinx': ('https://www.sphinx-doc.org/en/stable/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/dev', None),
     'implements': ('https://implements.readthedocs.io/en/latest/', None),
-    'libra': ('https://libra2.readthedocs.io/en/master', None)
+    'libra': ('https://jharwell.github.io/libra', None)
 }
 
 # This is the expected signature of the handler for this event, cf doc
 
 
 def autodoc_skip_member_handler(app, what, name, obj, skip, options):
     # Basic approach; you might want a regex instead
```

### Comparing `sierra-research-1.3.5/docs/figures/architecture.png` & `sierra-research-1.3.6/docs/figures/architecture.png`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/index.rst` & `sierra-research-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/man/sierra-cli.rst` & `sierra-research-1.3.6/docs/man/sierra-cli.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/man/sierra.rst` & `sierra-research-1.3.6/docs/man/sierra.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/contributing.rst` & `sierra-research-1.3.6/docs/src/contributing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 Mechanics
 =========
 
 Writing the code
 ----------------
 
 To contribute to the SIERRA core, in you should follow the general workflow and
-python development guide outlined in :ref:`ln-libra-python-dev-guide` and
-:ref:`ln-libra-dev-workflow`. For the static analysis step:
+python development guide outlined in :ref:`libra:dev/python-guide` and
+:ref:`libra:dev/workflow`. For the static analysis step:
 
 #. Install development packages for SIERRA (from the SIERRA repo root)::
 
      pip3 install .[devel]
 
 #. Run ``nox`` to check most things prior to commiting/pushing your changes. If
    there are errors *you* have introduced, fix them. Some checkers (such as
```

### Comparing `sierra-research-1.3.5/docs/src/description.rst` & `sierra-research-1.3.6/docs/src/description.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/exec_env/hpc.rst` & `sierra-research-1.3.6/docs/src/exec_env/hpc.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/exec_env/robot.rst` & `sierra-research-1.3.6/docs/src/exec_env/robot.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/faq.rst` & `sierra-research-1.3.6/docs/src/faq.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/getting_started.rst` & `sierra-research-1.3.6/docs/src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/glossary.rst` & `sierra-research-1.3.6/docs/src/glossary.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       `https://www.argos-sim.info/index.php <https://www.argos-sim.info/index.php>`_.
 
 
    Gazebo
 
       A state-of-the-art robotics simulator with many features including .urdf
       robot models, realistic 3D rendering, and more. The Gazebo website is at
-      `http://gazebosim.org <http://gazebosim.org>`_.
+      `https://gazebosim.org <https://gazebosim.org>`_.
 
    ROS1
 
       You know it. You either love it or hate it, but you can't escape it. The
       ROS website is at `https://wiki.ros.org <https://wiki.ros.org>`_.
```

### Comparing `sierra-research-1.3.5/docs/src/matrix.rst` & `sierra-research-1.3.6/docs/src/matrix.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
      - Description
 
    * - `ARGoS <https://www.argos-sim.info/index.php>`_
 
      - Simulator for fast simulation of large swarms. Requires ARGoS >=
        3.0.0-beta59.
 
-   * - `ROS1 <https://ros.org)+[Gazebo](https://www.gazebosim.org>`_
+   * - `ROS1 <https://ros.org>`_ + `Gazebo <https://github.com/gazebosim/gz-sim>`_
 
      - Using ROS1 with the Gazebo simulator. Requires Gazebo >= 11.9.0, ROS1
        Noetic or later.
 
    * - `ROS1+Robot <https://ros.org>`_
 
      - Using ROS1 with a real robot platform of your choice. ROS1 Noetic or
@@ -80,29 +80,28 @@
      - Description
 
    * - `ARGoS <https://www.argos-sim.info/index.php>`_
 
      - Simulator for fast simulation of large swarms. Requires ARGoS >=
        3.0.0-beta59.
 
-   * - `ROS1 <https://ros.org)+[Gazebo](https://www.gazebosim.org>`_
+   * - `ROS1 <https://ros.org>`_ + `Gazebo <https://github.com/gazebosim/gz-sim>`_
 
      - Using ROS1 with the Gazebo simulator. Requires Gazebo >= 11.9.0, ROS1
        Kinetic or later.
 
    * - `ROS1+Robot <https://ros.org>`_
 
      - Using ROS1 with a real robot platform of your choice. ROS1 Kinetic or
        later is required.
 
 SIERRA also supports multiple output formats for experimental outputs. If the
-format for your experimental outputs is not listed, see the `docs
-<https://sierra.readthedocs.io/en/master/src/tutorials.html>`_
-for how to add it via a plugin. SIERRA currently only supports XML experimental
-inputs.
+format for your experimental outputs is not listed, see the
+:ref:`ln-sierra-tutorials` for how to add it via a plugin. SIERRA currently only
+supports XML experimental inputs.
 
 .. list-table::
    :header-rows: 1
    :widths: 50,50
 
    * - Experimental Output Format
```

### Comparing `sierra-research-1.3.5/docs/src/packages.rst` & `sierra-research-1.3.6/docs/src/packages.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 SIERRA ROSBridge
 ================
 
 SIERRA provides a :term:`ROS1` package containing functionality it uses to
 manage simulations and provide run-time support to :term:`projects<Project>`
 using a :term:`Platform` built on ROS. To use SIERRA with a ROS platform, you
 need to setup the SIERRA ROSbridge package here (details in README):
-`<https://github.com/jharwell/sierra_rosbridge.git>`_.
+`<https://github.com/jharwell/sierra_rosbridge>`_.
 
 This package provides the following nodes:
 
 - ``sierra_timekeeper`` - Tracks time on an :term:`Experimental Run`, and
   terminates once the amount of time specified in ``--exp-setup`` has
   elapsed. Necessary because ROS does not provide a way to say "Run for this
   long and then terminate". An XML tag including this node is inserted by SIERRA
```

### Comparing `sierra-research-1.3.5/docs/src/philosophy.rst` & `sierra-research-1.3.6/docs/src/philosophy.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/platform/argos/batch_criteria.rst` & `sierra-research-1.3.6/docs/src/platform/argos/batch_criteria.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/platform/argos/index.rst` & `sierra-research-1.3.6/docs/src/platform/argos/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/platform/ros1gazebo/batch_criteria.rst` & `sierra-research-1.3.6/docs/src/platform/ros1gazebo/batch_criteria.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/platform/ros1gazebo/index.rst` & `sierra-research-1.3.6/docs/src/platform/ros1gazebo/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/platform/ros1robot/batch_criteria.rst` & `sierra-research-1.3.6/docs/src/platform/ros1robot/batch_criteria.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/platform/ros1robot/index.rst` & `sierra-research-1.3.6/docs/src/platform/ros1robot/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/requirements.rst` & `sierra-research-1.3.6/docs/src/requirements.rst`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         for specifics.
 
 #. ROS does not currently provide a way to shut down after a given # of
    iterations/timesteps, so SIERRA provides a ROS package with a node tracking
    the elapsed time in seconds, and which exits (and takes down the roslaunch
    when it does) after the specified experiment time has elapsed. This node is
    inserted into all ``.launch`` files. All ROS projects must depend on this
-   `ROS bridge <https://github.com/jharwell/sierra_rosbridge.git>`_
+   `ROS bridge <https://github.com/jharwell/sierra_rosbridge>`_
    package so the necessary nodes can be found by ROS at runtime.
 
 
 Additional Platform Requirements
 ================================
 
 :term:`ROS1+Robot` Platform
```

### Comparing `sierra-research-1.3.5/docs/src/roadmap.rst` & `sierra-research-1.3.6/docs/src/roadmap.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/storage/index.rst` & `sierra-research-1.3.6/docs/src/storage/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/trial.rst` & `sierra-research-1.3.6/docs/src/trial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             - ``ros-<distro>-turtlebot3-description``
             - ``ros-<distro>-turtlebot3-msgs``
             - ``ros-<distro>-turtlebot3-gazebo``
             - ``ros-<distro>-turtlebot3-bringup``
 
             Where ``<distro>`` is replaced by your ROS distro.
 
-         #.  Install the `SIERRA ROSBridge <https:github.com/jharwell/sierra_rosbridge.git>`_::
+         #.  Install the `SIERRA ROSBridge <https://github.com/jharwell/sierra_rosbridge>`_::
 
                pip3 install catkin_tools
                git clone https://github.com/jharwell/sierra_rosbridge.git
                cd sierra_rosbridge
                catkin init
                catkin config --extend /opt/ros/<distro>
 
@@ -130,15 +130,15 @@
          compiled!). This is used instead of the ``FindARGoS()`` cmake
          functionality to support having multiple versions of ARGoS installed in
          multiple directories.
 
       .. group-tab:: ROS1+Gazebo
 
          Based on one of the turtlebot3 `intro tutorials
-         <https://github.com:ROBOTIS-GIT/turtlebot3_simulations.git>`_::
+         <https://github.com/ROBOTIS-GIT/turtlebot3_simulations>`_::
 
            git clone https://github.com/jharwell/sierra-sample-project.git
            cd sierra-sample-project/ros1gazebo
            git checkout devel
            catkin init
            catkin config --extend=$HOME/.local/ros/noetic
            catkin build
```

### Comparing `sierra-research-1.3.5/docs/src/tutorials/hpc/cluster_setup.rst` & `sierra-research-1.3.6/docs/src/tutorials/hpc/cluster_setup.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/index.rst` & `sierra-research-1.3.6/docs/src/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/index.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/exec_env/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/plugin.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/exec_env/plugin.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/cmdline.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/platform/cmdline.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/generators.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/platform/generators.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/index.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/platform/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/plugin.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/platform/plugin.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/storage/index.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/storage/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/plugin/storage/plugin.rst` & `sierra-research-1.3.6/docs/src/tutorials/plugin/storage/plugin.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/cmdline.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/cmdline.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/generators.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/generators.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/graphs_config.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/graphs_config.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/hooks.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/hooks.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/main_config/controllers.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/main_config/controllers.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/main_config/main.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/main_config/main.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/main_config/perf.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/main_config/perf.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/models.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/models.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/new_bc.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/new_bc.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/project.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/project.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/stage5_config.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/stage5_config.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/tutorials/project/template_input_file.rst` & `sierra-research-1.3.6/docs/src/tutorials/project/template_input_file.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/cli-core.rst` & `sierra-research-1.3.6/docs/src/usage/cli-core.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/cli.rst` & `sierra-research-1.3.6/docs/src/usage/cli.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/environment.rst` & `sierra-research-1.3.6/docs/src/usage/environment.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/examples.rst` & `sierra-research-1.3.6/docs/src/usage/examples.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/index.rst` & `sierra-research-1.3.6/docs/src/usage/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/pipeline.rst` & `sierra-research-1.3.6/docs/src/usage/pipeline.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/rendering.rst` & `sierra-research-1.3.6/docs/src/usage/rendering.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/run_time_tree.rst` & `sierra-research-1.3.6/docs/src/usage/run_time_tree.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/stage5.rst` & `sierra-research-1.3.6/docs/src/usage/stage5.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/subprograms.rst` & `sierra-research-1.3.6/docs/src/usage/subprograms.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/docs/src/usage/variables.rst` & `sierra-research-1.3.6/docs/src/usage/variables.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/noxfile.py` & `sierra-research-1.3.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/scripts/argos-integration-tests.sh` & `sierra-research-1.3.6/scripts/argos-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/scripts/core-integration-tests.sh` & `sierra-research-1.3.6/scripts/core-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/scripts/ros1gazebo-integration-tests.sh` & `sierra-research-1.3.6/scripts/ros1gazebo-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/scripts/ros1robot-integration-tests.sh` & `sierra-research-1.3.6/scripts/ros1robot-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/scripts/slurm-test.sh` & `sierra-research-1.3.6/scripts/slurm-test.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/scripts/slurm.conf` & `sierra-research-1.3.6/scripts/slurm.conf`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/setup.py` & `sierra-research-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,21 @@
 
             # Deployment packages
             'build',
             'twine',
             'setuptools',
 
             # Sphinx packages
-            "sphinx==4.4.0",
-            "docutils==0.16",
+            "sphinx==5.0.2",
+            "docutils==0.18.1",
             "sphinx-rtd-theme",
             "sphinx-argparse",
             "sphinx-tabs",
             "sphinxcontrib-napoleon",
+            "psutil",
             "sphinx-last-updated-by-git",
             "autoapi",
             "graphviz"
         ]
     },
     python_requires=">=3.8",
     entry_points={
```

### Comparing `sierra-research-1.3.5/sierra/core/cmdline.py` & `sierra-research-1.3.6/sierra/core/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/config.py` & `sierra-research-1.3.6/sierra/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     # Set MPL backend (headless for non-interactive use). Must be BEFORE
     # importing pyplot reduce import loading time.
     mpl.use('agg')
 
     import matplotlib.pyplot as plt
 
     # Set MPL style
-    plt.style.use('seaborn-colorblind')
+    plt.style.use('seaborn-v0_8-colorblind')
 
 
 # Actually initialize matplotlib
 mpl_init()
 
 ################################################################################
 # General Configuration
```

### Comparing `sierra-research-1.3.5/sierra/core/experiment/bindings.py` & `sierra-research-1.3.6/sierra/core/experiment/bindings.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/experiment/definition.py` & `sierra-research-1.3.6/sierra/core/experiment/definition.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/experiment/spec.py` & `sierra-research-1.3.6/sierra/core/experiment/spec.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/experiment/xml.py` & `sierra-research-1.3.6/sierra/core/experiment/xml.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/generators/controller_generator_parser.py` & `sierra-research-1.3.6/sierra/core/generators/controller_generator_parser.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/generators/exp_creator.py` & `sierra-research-1.3.6/sierra/core/generators/exp_creator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/generators/exp_generators.py` & `sierra-research-1.3.6/sierra/core/generators/exp_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/generators/generator_factory.py` & `sierra-research-1.3.6/sierra/core/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/graphs/heatmap.py` & `sierra-research-1.3.6/sierra/core/graphs/heatmap.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/graphs/scatterplot2D.py` & `sierra-research-1.3.6/sierra/core/graphs/scatterplot2D.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/graphs/stacked_line_graph.py` & `sierra-research-1.3.6/sierra/core/graphs/stacked_line_graph.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/graphs/stacked_surface_graph.py` & `sierra-research-1.3.6/sierra/core/graphs/stacked_surface_graph.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/graphs/summary_line_graph.py` & `sierra-research-1.3.6/sierra/core/graphs/summary_line_graph.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/hpc/cmdline.py` & `sierra-research-1.3.6/sierra/core/hpc/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/logging.py` & `sierra-research-1.3.6/sierra/core/logging.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/models/graphs.py` & `sierra-research-1.3.6/sierra/core/models/graphs.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/models/interface.py` & `sierra-research-1.3.6/sierra/core/models/interface.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/pipeline.py` & `sierra-research-1.3.6/sierra/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage1/pipeline_stage1.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage1/pipeline_stage1.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage2/exp_runner.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage2/exp_runner.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage2/pipeline_stage2.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage2/pipeline_stage2.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage3/imagizer.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage3/imagizer.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage3/pipeline_stage3.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage3/pipeline_stage3.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage3/run_collator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage3/run_collator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage3/statistics_calculator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage3/statistics_calculator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/graph_collator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/graph_collator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/inter_exp_graph_generator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/inter_exp_graph_generator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/intra_exp_graph_generator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/intra_exp_graph_generator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/model_runner.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/model_runner.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/pipeline_stage4.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/pipeline_stage4.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/rendering.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/rendering.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage4/yaml_config_loader.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage4/yaml_config_loader.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage5/inter_scenario_comparator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage5/inter_scenario_comparator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage5/intra_scenario_comparator.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage5/intra_scenario_comparator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/pipeline/stage5/pipeline_stage5.py` & `sierra-research-1.3.6/sierra/core/pipeline/stage5/pipeline_stage5.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/platform.py` & `sierra-research-1.3.6/sierra/core/platform.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/plugin.py` & `sierra-research-1.3.6/sierra/core/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/plugin_manager.py` & `sierra-research-1.3.6/sierra/core/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/root_dirpath_generator.py` & `sierra-research-1.3.6/sierra/core/root_dirpath_generator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/ros1/callbacks.py` & `sierra-research-1.3.6/sierra/core/ros1/callbacks.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/ros1/cmdline.py` & `sierra-research-1.3.6/sierra/core/ros1/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/ros1/generators.py` & `sierra-research-1.3.6/sierra/core/ros1/generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/ros1/variables/exp_setup.py` & `sierra-research-1.3.6/sierra/core/ros1/variables/exp_setup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/startup.py` & `sierra-research-1.3.6/sierra/core/startup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/stat_kernels.py` & `sierra-research-1.3.6/sierra/core/stat_kernels.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/storage.py` & `sierra-research-1.3.6/sierra/core/storage.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/types.py` & `sierra-research-1.3.6/sierra/core/types.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/utils.py` & `sierra-research-1.3.6/sierra/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
     elif policy == 'zero':
         return df.fillna(value=0)
     else:
         raise RuntimeError(f"Bad fill policy {policy}")
 
 
 @retry(OSError, tries=10, delay=0.100, backoff=1.1)  # type:ignore
-def pickle_dump(obj: object, f: tp.IO) -> None:
+def pickle_dump(obj: object, f) -> None:
     pickle.dump(obj, f)
 
 
 def gen_scenario_spec(cmdopts: types.Cmdopts, **kwargs) -> tp.Dict[str, tp.Any]:
     # scenario is passed in kwargs during stage 5 (can't be passed via
     # --scenario in general )
     scenario = kwargs.get('scenario', cmdopts['scenario'])
```

### Comparing `sierra-research-1.3.5/sierra/core/variables/base_variable.py` & `sierra-research-1.3.6/sierra/core/variables/base_variable.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/variables/batch_criteria.py` & `sierra-research-1.3.6/sierra/core/variables/batch_criteria.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/variables/exp_setup.py` & `sierra-research-1.3.6/sierra/core/variables/exp_setup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/variables/population_size.py` & `sierra-research-1.3.6/sierra/core/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/variables/variable_density.py` & `sierra-research-1.3.6/sierra/core/variables/variable_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/core/vector.py` & `sierra-research-1.3.6/sierra/core/vector.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/main.py` & `sierra-research-1.3.6/sierra/main.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/hpc/adhoc/plugin.py` & `sierra-research-1.3.6/sierra/plugins/hpc/adhoc/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/hpc/local/plugin.py` & `sierra-research-1.3.6/sierra/plugins/hpc/local/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/hpc/pbs/plugin.py` & `sierra-research-1.3.6/sierra/plugins/hpc/pbs/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/hpc/slurm/plugin.py` & `sierra-research-1.3.6/sierra/plugins/hpc/slurm/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/cmdline.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/generators/platform_generators.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/generators/platform_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/plugin.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/arena_shape.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/arena_shape.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/cameras.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/cameras.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/constant_density.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/constant_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/exp_setup.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/exp_setup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/physics_engines.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/physics_engines.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_constant_density.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/population_constant_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_size.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_variable_density.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/population_variable_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/rendering.py` & `sierra-research-1.3.6/sierra/plugins/platform/argos/variables/rendering.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/cmdline.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/plugin.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/population_size.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1gazebo/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/cmdline.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1robot/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/platform_generators.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1robot/generators/platform_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/plugin.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1robot/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/population_size.py` & `sierra-research-1.3.6/sierra/plugins/platform/ros1robot/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/plugin.py` & `sierra-research-1.3.6/sierra/plugins/robot/turtlebot3/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra/plugins/storage/csv/plugin.py` & `sierra-research-1.3.6/sierra/plugins/storage/csv/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/sierra_research.egg-info/PKG-INFO` & `sierra-research-1.3.6/sierra_research.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierra-research
-Version: 1.3.5
+Version: 1.3.6
 Summary: Automation framework for the scientific method in AI research
 Home-page: https://github.com/jharwell/sierra
 Author: John Harwell
 Author-email: john.r.harwell@gmail.com
 License: MIT
 Keywords: research,automation,robotics,agent-based modeling,reproducibility,reusability
 Platform: linux
@@ -17,32 +17,71 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: devel
 License-File: LICENSE
+Requires-Dist: pyyaml
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: sympy
+Requires-Dist: psutil
+Requires-Dist: distro
+Requires-Dist: netifaces
+Requires-Dist: haggis
+Requires-Dist: coloredlogs
+Requires-Dist: implements
+Requires-Dist: retry
+Provides-Extra: devel
+Requires-Dist: pylint==2.14.5; extra == "devel"
+Requires-Dist: pytype; extra == "devel"
+Requires-Dist: pydocstyle; extra == "devel"
+Requires-Dist: xenon; extra == "devel"
+Requires-Dist: flake8; extra == "devel"
+Requires-Dist: nox; extra == "devel"
+Requires-Dist: psutil; extra == "devel"
+Requires-Dist: pytest; extra == "devel"
+Requires-Dist: pytest-cov; extra == "devel"
+Requires-Dist: mypy; extra == "devel"
+Requires-Dist: xmldiff; extra == "devel"
+Requires-Dist: coverage; extra == "devel"
+Requires-Dist: coveralls; extra == "devel"
+Requires-Dist: mypy-runner; extra == "devel"
+Requires-Dist: build; extra == "devel"
+Requires-Dist: twine; extra == "devel"
+Requires-Dist: setuptools; extra == "devel"
+Requires-Dist: sphinx==5.0.2; extra == "devel"
+Requires-Dist: docutils==0.18.1; extra == "devel"
+Requires-Dist: sphinx-rtd-theme; extra == "devel"
+Requires-Dist: sphinx-argparse; extra == "devel"
+Requires-Dist: sphinx-tabs; extra == "devel"
+Requires-Dist: sphinxcontrib-napoleon; extra == "devel"
+Requires-Dist: psutil; extra == "devel"
+Requires-Dist: sphinx-last-updated-by-git; extra == "devel"
+Requires-Dist: autoapi; extra == "devel"
+Requires-Dist: graphviz; extra == "devel"
 
 ===========================================================================
 SIERRA (reSearch pIpEline for Reproducibility, Reusability, and Automation)
 ===========================================================================
 
 .. |pepy-downloads| image:: https://pepy.tech/badge/sierra-research
                     :target: https://pepy.tech/project/sierra-research
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/sierra-research.svg
                   :target: https://pypi.python.org/pypi/sierra-research/
 
 .. |supported-pythons| image:: https://img.shields.io/pypi/pyversions/sierra-research.svg
                        :target: https://pypi.python.org/pypi/sierra-research/
 
-.. |linux-supported| image:: https://svgshare.com/i/Zhy.svg
-.. |osx-supported| image:: https://svgshare.com/i/ZjP.svg
+.. |linux-supported| image:: https://img.shields.io/badge/os-Linux-crimson
+.. |osx-supported| image:: https://img.shields.io/badge/os-OSX-crimson
 
 .. |ci-integration-master| image:: https://github.com/jharwell/sierra/actions/workflows/integration-all.yml/badge.svg?branch=master
 .. |ci-analysis-master| image:: https://github.com/jharwell/sierra/actions/workflows/static-analysis.yml/badge.svg?branch=master
 .. |ci-coverage-master| image:: https://coveralls.io/repos/github/jharwell/sierra/badge.svg?branch=master
 
 .. |ci-integration-devel| image:: https://github.com/jharwell/sierra/actions/workflows/integration-all.yml/badge.svg?branch=devel
 .. |ci-analysis-devel| image:: https://github.com/jharwell/sierra/actions/workflows/static-analysis.yml/badge.svg?branch=devel
```

### Comparing `sierra-research-1.3.5/sierra_research.egg-info/SOURCES.txt` & `sierra-research-1.3.6/sierra_research.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/tests/arena_extent_test.py` & `sierra-research-1.3.6/tests/arena_extent_test.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/tests/exp_def_test.py` & `sierra-research-1.3.6/tests/exp_def_test.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/tests/test1.xml` & `sierra-research-1.3.6/tests/test1.xml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/tests/vector_test.py` & `sierra-research-1.3.6/tests/vector_test.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.5/todo.org` & `sierra-research-1.3.6/todo.org`

 * *Files identical despite different names*

