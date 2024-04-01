# Comparing `tmp/aws_lambda_builders-1.8.1.tar.gz` & `tmp/aws_lambda_builders-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws_lambda_builders-1.8.1.tar", last modified: Thu Sep 30 00:15:05 2021, max compression
+gzip compressed data, was "dist/aws_lambda_builders-1.9.0.tar", last modified: Mon Oct 25 23:49:47 2021, max compression
```

## Comparing `aws_lambda_builders-1.8.1.tar` & `aws_lambda_builders-1.9.0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/
--rw-r--r--   0 root         (0) root         (0)      303 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)      293 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/
--rw-r--r--   0 root         (0) root         (0)     5213 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/utils.py
--rw-r--r--   0 root         (0) root         (0)     3147 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/registry.py
--rw-r--r--   0 root         (0) root         (0)     1006 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/path_resolver.py
--rw-r--r--   0 root         (0) root         (0)      106 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/architecture.py
--rw-r--r--   0 root         (0) root         (0)      592 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/binary_path.py
--rw-r--r--   0 root         (0) root         (0)     4891 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/builder.py
--rw-r--r--   0 root         (0) root         (0)    11495 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflow.py
--rw-r--r--   0 root         (0) root         (0)       86 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1932 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5265 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2735 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/
--rw-r--r--   0 root         (0) root         (0)     4456 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)     1182 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/utils.py
--rw-r--r--   0 root         (0) root         (0)     1402 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/workflow.py
--rw-r--r--   0 root         (0) root         (0)       94 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1877 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/actions.py
--rw-r--r--   0 root         (0) root         (0)     2138 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/bundler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/
--rw-r--r--   0 root         (0) root         (0)     3341 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)      598 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/maven_resolver.py
--rw-r--r--   0 root         (0) root         (0)     1439 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/utils.py
--rw-r--r--   0 root         (0) root         (0)     1532 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/maven.py
--rw-r--r--   0 root         (0) root         (0)     1719 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/workflow.py
--rw-r--r--   0 root         (0) root         (0)      105 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2793 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/actions.py
--rw-r--r--   0 root         (0) root         (0)     2861 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/maven_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/
--rw-r--r--   0 root         (0) root         (0)     1531 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)      579 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/utils.py
--rw-r--r--   0 root         (0) root         (0)     2179 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/builder.py
--rw-r--r--   0 root         (0) root         (0)     1263 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/workflow.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      681 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/actions.py
--rw-r--r--   0 root         (0) root         (0)     2396 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/
--rw-r--r--   0 root         (0) root         (0)     5133 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)      936 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/utils.py
--rw-r--r--   0 root         (0) root         (0)      817 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli_resolver.py
--rw-r--r--   0 root         (0) root         (0)     1565 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/workflow.py
--rw-r--r--   0 root         (0) root         (0)      210 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2129 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli.py
--rw-r--r--   0 root         (0) root         (0)     4904 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/
--rw-r--r--   0 root         (0) root         (0)     6786 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)     3254 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/utils.py
--rw-r--r--   0 root         (0) root         (0)     2851 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/workflow.py
--rw-r--r--   0 root         (0) root         (0)     5691 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/compat.py
--rw-r--r--   0 root         (0) root         (0)    33020 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/packager.py
--rw-r--r--   0 root         (0) root         (0)      109 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1923 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/actions.py
--rw-r--r--   0 root         (0) root         (0)     2069 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/validator.py
--rw-r--r--   0 root         (0) root         (0)      487 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/
--rw-r--r--   0 root         (0) root         (0)     7336 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/utils.py
--rw-r--r--   0 root         (0) root         (0)     2413 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/workflow.py
--rw-r--r--   0 root         (0) root         (0)      109 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6522 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/actions.py
--rw-r--r--   0 root         (0) root         (0)     2384 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/npm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/
--rw-r--r--   0 root         (0) root         (0)     8228 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)     1439 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/resources/
--rw-r--r--   0 root         (0) root         (0)     3073 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/resources/lambda-build-init.gradle
--rw-r--r--   0 root         (0) root         (0)      940 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/gradle_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2183 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/workflow.py
--rw-r--r--   0 root         (0) root         (0)      107 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2795 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/actions.py
--rw-r--r--   0 root         (0) root         (0)     1865 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/gradle.py
--rw-r--r--   0 root         (0) root         (0)     2858 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/gradle_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/
--rw-r--r--   0 root         (0) root         (0)     1719 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)     2509 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/subproc_exec.py
--rw-r--r--   0 root         (0) root         (0)      863 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/utils.py
--rw-r--r--   0 root         (0) root         (0)     1757 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/workflow.py
--rw-r--r--   0 root         (0) root         (0)      107 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1937 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/
--rw-r--r--   0 root         (0) root         (0)     3451 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/DESIGN.md
--rw-r--r--   0 root         (0) root         (0)     1046 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/utils.py
--rw-r--r--   0 root         (0) root         (0)     2226 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/workflow.py
--rw-r--r--   0 root         (0) root         (0)     2541 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/make.py
--rw-r--r--   0 root         (0) root         (0)      123 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/__init__.py
--rw-r--r--   0 root         (0) root         (0)      115 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3627 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/actions.py
--rw-r--r--   0 root         (0) root         (0)      500 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/validator.py
--rw-r--r--   0 root         (0) root         (0)     2243 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/aws_lambda_builders/validator.py
--rw-r--r--   0 root         (0) root         (0)     2372 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/requirements/
--rw-r--r--   0 root         (0) root         (0)      886 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)      171 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/requirements/python_pip.txt
--rw-r--r--   0 root         (0) root         (0)       49 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)     1198 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/
--rw-r--r--   0 root         (0) root         (0)       20 2021-09-30 00:15:04.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2372 2021-09-30 00:15:04.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       71 2021-09-30 00:15:04.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-30 00:15:04.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      570 2021-09-30 00:15:04.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     4390 2021-09-30 00:15:04.000000 aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2488 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/setup.py
--rw-r--r--   0 root         (0) root         (0)       79 2021-09-30 00:15:05.000000 aws_lambda_builders-1.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11392 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      102 2021-09-30 00:09:47.000000 aws_lambda_builders-1.8.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)       10 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      441 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/requirements/python_pip.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/
+-rw-r--r--   0 root         (0) root         (0)    12188 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflow.py
+-rw-r--r--   0 root         (0) root         (0)      106 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/architecture.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/utils.py
+-rw-r--r--   0 root         (0) root         (0)      592 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/binary_path.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/validator.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/actions.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/
+-rw-r--r--   0 root         (0) root         (0)     2324 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/workflow.py
+-rw-r--r--   0 root         (0) root         (0)      632 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/maven_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/maven.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/actions.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      105 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/maven_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/
+-rw-r--r--   0 root         (0) root         (0)     1757 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/subproc_exec.py
+-rw-r--r--   0 root         (0) root         (0)      863 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      107 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/
+-rw-r--r--   0 root         (0) root         (0)     2891 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/gradle_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/actions.py
+-rw-r--r--   0 root         (0) root         (0)      974 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/gradle_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     8228 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      107 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/resources/
+-rw-r--r--   0 root         (0) root         (0)     3073 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/resources/lambda-build-init.gradle
+-rw-r--r--   0 root         (0) root         (0)     1865 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/gradle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/
+-rw-r--r--   0 root         (0) root         (0)     3970 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6522 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/actions.py
+-rw-r--r--   0 root         (0) root         (0)     7336 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      109 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/npm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/
+-rw-r--r--   0 root         (0) root         (0)     1263 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/workflow.py
+-rw-r--r--   0 root         (0) root         (0)      579 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/validator.py
+-rw-r--r--   0 root         (0) root         (0)      681 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      102 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/
+-rw-r--r--   0 root         (0) root         (0)     1565 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/workflow.py
+-rw-r--r--   0 root         (0) root         (0)      936 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4904 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/actions.py
+-rw-r--r--   0 root         (0) root         (0)      817 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     5133 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      210 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/
+-rw-r--r--   0 root         (0) root         (0)     2138 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/bundler.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4456 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)       94 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java/
+-rw-r--r--   0 root         (0) root         (0)     1551 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java/actions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      487 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/
+-rw-r--r--   0 root         (0) root         (0)     3900 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/validator.py
+-rw-r--r--   0 root         (0) root         (0)      241 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/actions.py
+-rw-r--r--   0 root         (0) root         (0)     6786 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      109 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5691 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/compat.py
+-rw-r--r--   0 root         (0) root         (0)    33020 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/packager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/
+-rw-r--r--   0 root         (0) root         (0)     2226 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/utils.py
+-rw-r--r--   0 root         (0) root         (0)      500 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/validator.py
+-rw-r--r--   0 root         (0) root         (0)      115 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/actions.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/make.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/DESIGN.md
+-rw-r--r--   0 root         (0) root         (0)      123 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       86 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5484 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/path_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/aws_lambda_builders/builder.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     4426 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      318 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2368 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11392 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       79 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      303 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)      285 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      102 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2368 2021-10-25 23:49:47.000000 aws_lambda_builders-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1198 2021-10-25 23:44:42.000000 aws_lambda_builders-1.9.0/README.md
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
     :type ignore: function
     :param ignore:
         A function that returns a set of file names to ignore, given a list of available file names. Similar to the
         ``ignore`` property of ``shutils.copytree`` method
     """
 
+    if not os.path.exists(source):
+        LOG.warning("Skipping copy operation since source %s does not exist", source)
+        return
+
     if not os.path.exists(destination):
         os.makedirs(destination)
 
         try:
             # Let's try to copy the directory metadata from source to destination
             shutil.copystat(source, destination)
         except OSError as ex:
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/registry.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/registry.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/path_resolver.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/path_resolver.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/binary_path.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/binary_path.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/builder.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         scratch_dir,
         manifest_path,
         runtime=None,
         optimizations=None,
         options=None,
         executable_search_paths=None,
         mode=None,
+        download_dependencies=True,
+        dependencies_dir=None,
+        combine_dependencies=True,
         architecture=X86_64,
     ):
         """
         Actually build the code by running workflows
 
         :type source_dir: str
         :param source_dir:
@@ -104,14 +107,27 @@
         :param executable_search_paths:
             Additional list of paths to search for executables required by the workflow.
 
         :type mode: str
         :param mode:
             Optional, Mode the build should produce
 
+        :type download_dependencies: bool
+        :param download_dependencies:
+            Optional, Should download dependencies when building
+
+        :type dependencies_dir: str
+        :param dependencies_dir:
+            Optional, Path to folder the dependencies should be downloaded to
+
+        :type combine_dependencies: bool
+        :param combine_dependencies:
+            Optional, This flag will only be used if dependency_folder is specified. False will not copy dependencies
+            from dependency_folder into build folder
+
         :type architecture: str
         :param architecture:
             Type of architecture x86_64 and arm64 for Lambda Function
         """
 
         if not os.path.exists(scratch_dir):
             os.makedirs(scratch_dir)
@@ -122,14 +138,17 @@
             scratch_dir,
             manifest_path,
             runtime=runtime,
             optimizations=optimizations,
             options=options,
             executable_search_paths=executable_search_paths,
             mode=mode,
+            download_dependencies=download_dependencies,
+            dependencies_dir=dependencies_dir,
+            combine_dependencies=combine_dependencies,
             architecture=architecture,
         )
 
         return workflow.run()
 
     def _clear_workflows(self):
         DEFAULT_REGISTRY.clear()
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,14 +156,17 @@
         scratch_dir,
         manifest_path,
         runtime=None,
         executable_search_paths=None,
         optimizations=None,
         options=None,
         mode=BuildMode.RELEASE,
+        download_dependencies=True,
+        dependencies_dir=None,
+        combine_dependencies=True,
         architecture=X86_64,
     ):
         """
         Initialize the builder with given arguments. These arguments together form the "public API" that each
         build action must support at the minimum.
 
         Parameters
@@ -174,37 +177,47 @@
             Path to a folder where the built artifacts should be placed
         scratch_dir : str
             Path to a directory that the workflow can use as scratch space. Workflows are expected to use this directory
             to write temporary files instead of ``/tmp`` or other OS-specific temp directories.
         manifest_path : str
             Path to the dependency manifest
         runtime : str, optional
-            name of the AWS Lambda runtime that you are building for. This is sent to the builder for
+            Optional, name of the AWS Lambda runtime that you are building for. This is sent to the builder for
             informational purposes, by default None
         executable_search_paths : list, optional
             Additional list of paths to search for executables required by the workflow, by default None
         optimizations : dict, optional
             dictionary of optimization flags to pass to the build action. **Not supported**, by default None
         options : dict, optional
             dictionary of options ot pass to build action. **Not supported**., by default None
         mode : str, optional
             Mode the build should produce, by default BuildMode.RELEASE
+        download_dependencies: bool, optional
+            Should download dependencies when building
+        dependencies_dir : str, optional
+            Path to folder the dependencies should be downloaded to
+        combine_dependencies: bool, optional
+            This flag will only be used if dependency_folder is specified. False will not copy dependencies
+            from dependency_folder into build folder
         architecture : str, optional
             Architecture type either arm64 or x86_64 for which the build will be based on in AWS lambda, by default X86_64
         """
 
         self.source_dir = source_dir
         self.artifacts_dir = artifacts_dir
         self.scratch_dir = scratch_dir
         self.manifest_path = manifest_path
         self.runtime = runtime
         self.optimizations = optimizations
         self.options = options
         self.executable_search_paths = executable_search_paths
         self.mode = mode
+        self.download_dependencies = download_dependencies
+        self.dependencies_dir = dependencies_dir
+        self.combine_dependencies = combine_dependencies
         self.architecture = architecture
 
         # Actions are registered by the subclasses as they seem fit
         self.actions = []
         self._binaries = {}
 
     def is_supported(self):
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/exceptions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/__main__.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,17 @@
             params["scratch_dir"],
             params["manifest_path"],
             executable_search_paths=params.get("executable_search_paths", None),
             runtime=params["runtime"],
             optimizations=params["optimizations"],
             options=params["options"],
             mode=params.get("mode", None),
+            download_dependencies=params.get("download_dependencies", True),
+            dependencies_dir=params.get("dependencies_dir", None),
+            combine_dependencies=params.get("combine_dependencies", True),
             architecture=params.get("architecture", X86_64),
         )
 
         # Return a success response
         response = _success_response(request_id, artifacts_dir)
 
     except (WorkflowNotFoundError, WorkflowUnknownError, WorkflowFailedError) as ex:
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/workflow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """
-Ruby Bundler Workflow
+Go Modules Workflow
 """
-
 from aws_lambda_builders.workflow import BaseWorkflow, Capability
-from aws_lambda_builders.actions import CopySourceAction
 
-from .actions import RubyBundlerInstallAction, RubyBundlerVendorAction
+from .actions import GoModulesBuildAction
+from .builder import GoModulesBuilder
+from .validator import GoRuntimeValidator
 from .utils import OSUtils
-from .bundler import SubprocessBundler
-
-
-class RubyBundlerWorkflow(BaseWorkflow):
 
-    """
-    A Lambda builder workflow that knows how to build
-    Ruby projects using Bundler.
-    """
 
-    NAME = "RubyBundlerBuilder"
+class GoModulesWorkflow(BaseWorkflow):
 
-    CAPABILITY = Capability(language="ruby", dependency_manager="bundler", application_framework=None)
+    NAME = "GoModulesBuilder"
 
-    EXCLUDED_FILES = (".aws-sam", ".git")
+    CAPABILITY = Capability(language="go", dependency_manager="modules", application_framework=None)
 
-    def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, osutils=None, **kwargs):
+    def __init__(
+        self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, osutils=None, mode=None, **kwargs
+    ):
 
-        super(RubyBundlerWorkflow, self).__init__(
+        super(GoModulesWorkflow, self).__init__(
             source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=runtime, **kwargs
         )
 
         if osutils is None:
             osutils = OSUtils()
 
-        subprocess_bundler = SubprocessBundler(osutils)
-        bundle_install = RubyBundlerInstallAction(artifacts_dir, subprocess_bundler=subprocess_bundler)
+        options = kwargs.get("options") or {}
+        handler = options.get("artifact_executable_name", None)
+
+        output_path = osutils.joinpath(artifacts_dir, handler)
+
+        builder = GoModulesBuilder(osutils, binaries=self.binaries, mode=mode, architecture=self.architecture)
+        self.actions = [GoModulesBuildAction(source_dir, output_path, builder)]
 
-        bundle_deployment = RubyBundlerVendorAction(artifacts_dir, subprocess_bundler=subprocess_bundler)
-        self.actions = [
-            CopySourceAction(source_dir, artifacts_dir, excludes=self.EXCLUDED_FILES),
-            bundle_install,
-            bundle_deployment,
-        ]
+    def get_validators(self):
+        return [GoRuntimeValidator(runtime=self.runtime, architecture=self.architecture)]
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/ruby_bundler/bundler.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/ruby_bundler/bundler.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/maven_resolver.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/maven_resolver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Maven executable resolution
 """
 
-from .utils import OSUtils
+from aws_lambda_builders.workflows.java.utils import OSUtils
 
 
 class MavenResolver(object):
     def __init__(self, executable_search_paths=None, os_utils=None):
         self.binary = "mvn"
         self.executables = [self.binary]
         self.executable_search_paths = executable_search_paths
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     def is_windows(self):
         return platform.system().lower() == "windows"
 
     def copy(self, src, dst):
         shutil.copy2(src, dst)
         return dst
 
+    def move(self, src, dst):
+        shutil.move(src, dst)
+
     def listdir(self, d):
         return os.listdir(d)
 
     def exists(self, p):
         return os.path.exists(p)
 
     def which(self, executable, executable_search_paths=None):
@@ -45,10 +48,13 @@
                 self.copytree(new_source, new_destination)
             else:
                 self.copy(new_source, new_destination)
 
     def makedirs(self, d):
         return os.makedirs(d)
 
+    def rmtree(self, d):
+        shutil.rmtree(d)
+
     @property
     def pipe(self):
         return subprocess.PIPE
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/maven.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/maven.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 """
-Java Maven Workflow
+.NET Core CLI Package Workflow
 """
 from aws_lambda_builders.workflow import BaseWorkflow, Capability
-from aws_lambda_builders.actions import CopySourceAction
 
-from .actions import JavaMavenBuildAction, JavaMavenCopyDependencyAction, JavaMavenCopyArtifactsAction
-from .maven import SubprocessMaven
-from .maven_resolver import MavenResolver
-from .maven_validator import MavenValidator
+from .actions import GlobalToolInstallAction, RunPackageAction
+from .dotnetcli import SubprocessDotnetCLI
+from .dotnetcli_resolver import DotnetCliResolver
 from .utils import OSUtils
 
 
-class JavaMavenWorkflow(BaseWorkflow):
+class DotnetCliPackageWorkflow(BaseWorkflow):
+
     """
-    A Lambda builder workflow that knows how to build Java projects using Maven.
+    A Lambda builder workflow that knows to build and package .NET Core Lambda functions
     """
 
-    NAME = "JavaMavenWorkflow"
-
-    CAPABILITY = Capability(language="java", dependency_manager="maven", application_framework=None)
+    NAME = "DotnetCliPackageBuilder"
 
-    EXCLUDED_FILES = (".aws-sam", ".git")
+    CAPABILITY = Capability(language="dotnet", dependency_manager="cli-package", application_framework=None)
 
-    def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, **kwargs):
-        super(JavaMavenWorkflow, self).__init__(source_dir, artifacts_dir, scratch_dir, manifest_path, **kwargs)
+    def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, mode=None, **kwargs):
 
-        self.os_utils = OSUtils()
-        # Assuming root_dir is the same as source_dir for now
-        root_dir = source_dir
-        subprocess_maven = SubprocessMaven(maven_binary=self.binaries["mvn"], os_utils=self.os_utils)
-
-        self.actions = [
-            CopySourceAction(root_dir, scratch_dir, excludes=self.EXCLUDED_FILES),
-            JavaMavenBuildAction(scratch_dir, subprocess_maven),
-            JavaMavenCopyDependencyAction(scratch_dir, subprocess_maven),
-            JavaMavenCopyArtifactsAction(scratch_dir, artifacts_dir, self.os_utils),
-        ]
+        super(DotnetCliPackageWorkflow, self).__init__(
+            source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=runtime, mode=mode, **kwargs
+        )
+
+        options = kwargs["options"] if "options" in kwargs else {}
+        subprocess_dotnetcli = SubprocessDotnetCLI(os_utils=OSUtils())
+        dotnetcli_install = GlobalToolInstallAction(subprocess_dotnet=subprocess_dotnetcli)
+
+        dotnetcli_deployment = RunPackageAction(
+            source_dir,
+            subprocess_dotnet=subprocess_dotnetcli,
+            artifacts_dir=artifacts_dir,
+            options=options,
+            mode=mode,
+            architecture=self.architecture,
+        )
+        self.actions = [dotnetcli_install, dotnetcli_deployment]
 
     def get_resolvers(self):
-        return [MavenResolver(executable_search_paths=self.executable_search_paths)]
-
-    def get_validators(self):
-        return [MavenValidator(self.runtime, self.architecture, self.os_utils)]
+        return [DotnetCliResolver(executable_search_paths=self.executable_search_paths)]
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_maven/maven_validator.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_maven/maven_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Maven Binary Validation
 """
 
 import logging
 import re
 
+from aws_lambda_builders.workflows.java.utils import OSUtils
 from aws_lambda_builders.validator import RuntimeValidator
 
-from .utils import OSUtils
-
 LOG = logging.getLogger(__name__)
 
 
 class MavenValidator(RuntimeValidator):
     VERSION_STRING_WARNING = (
         "%s failed to return a version string using the '-v' option. The workflow is unable to "
         "check that the version of the JVM used is compatible with AWS Lambda."
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/builder.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/builder.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_modules/validator.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_modules/validator.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli_resolver.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli_resolver.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/workflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 """
-.NET Core CLI Package Workflow
+Go Dep Workflow
 """
-from aws_lambda_builders.workflow import BaseWorkflow, Capability
 
-from .actions import GlobalToolInstallAction, RunPackageAction
-from .dotnetcli import SubprocessDotnetCLI
-from .dotnetcli_resolver import DotnetCliResolver
+import logging
+import os
+
+from aws_lambda_builders.actions import CopySourceAction
+from aws_lambda_builders.workflow import BaseWorkflow, Capability
+from .actions import DepEnsureAction, GoBuildAction
 from .utils import OSUtils
+from .subproc_exec import SubprocessExec
 
+LOG = logging.getLogger(__name__)
 
-class DotnetCliPackageWorkflow(BaseWorkflow):
 
+class GoDepWorkflow(BaseWorkflow):
     """
-    A Lambda builder workflow that knows to build and package .NET Core Lambda functions
+    A Lambda builder workflow that knows how to build
+    Go projects using `dep`
     """
 
-    NAME = "DotnetCliPackageBuilder"
+    NAME = "GoDepBuilder"
 
-    CAPABILITY = Capability(language="dotnet", dependency_manager="cli-package", application_framework=None)
+    CAPABILITY = Capability(language="go", dependency_manager="dep", application_framework=None)
 
-    def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, mode=None, **kwargs):
+    EXCLUDED_FILES = (".aws-sam", ".git")
 
-        super(DotnetCliPackageWorkflow, self).__init__(
-            source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=runtime, mode=mode, **kwargs
+    def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, osutils=None, **kwargs):
+
+        super(GoDepWorkflow, self).__init__(
+            source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=runtime, **kwargs
         )
 
         options = kwargs["options"] if "options" in kwargs else {}
-        subprocess_dotnetcli = SubprocessDotnetCLI(os_utils=OSUtils())
-        dotnetcli_install = GlobalToolInstallAction(subprocess_dotnet=subprocess_dotnetcli)
+        handler = options.get("artifact_executable_name", None)
 
-        dotnetcli_deployment = RunPackageAction(
-            source_dir,
-            subprocess_dotnet=subprocess_dotnetcli,
-            artifacts_dir=artifacts_dir,
-            options=options,
-            mode=mode,
-            architecture=self.architecture,
-        )
-        self.actions = [dotnetcli_install, dotnetcli_deployment]
+        if osutils is None:
+            osutils = OSUtils()
 
-    def get_resolvers(self):
-        return [DotnetCliResolver(executable_search_paths=self.executable_search_paths)]
+        # project base name, where the Gopkg.toml and vendor dir are.
+        base_dir = osutils.abspath(osutils.dirname(manifest_path))
+        output_path = osutils.joinpath(osutils.abspath(artifacts_dir), handler)
+
+        subprocess_dep = SubprocessExec(osutils, "dep")
+        subprocess_go = SubprocessExec(osutils, "go")
+
+        self.actions = [
+            DepEnsureAction(base_dir, subprocess_dep),
+            GoBuildAction(
+                base_dir,
+                osutils.abspath(source_dir),
+                output_path,
+                subprocess_go,
+                self.architecture,
+                env=osutils.environ,
+            ),
+        ]
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/dotnetcli.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/dotnet_clipackage/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/dotnet_clipackage/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/compat.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/compat.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/packager.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/packager.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 class PythonPipBuildAction(BaseAction):
 
     NAME = "ResolveDependencies"
     DESCRIPTION = "Installing dependencies from PIP"
     PURPOSE = Purpose.RESOLVE_DEPENDENCIES
     LANGUAGE = "python"
 
-    def __init__(self, artifacts_dir, scratch_dir, manifest_path, runtime, binaries, architecture=X86_64):
+    def __init__(
+        self, artifacts_dir, scratch_dir, manifest_path, runtime, dependencies_dir, binaries, architecture=X86_64
+    ):
         self.artifacts_dir = artifacts_dir
         self.manifest_path = manifest_path
         self.scratch_dir = scratch_dir
         self.runtime = runtime
+        self.dependencies_dir = dependencies_dir
         self.binaries = binaries
         self.architecture = architecture
 
     def execute(self):
         os_utils = OSUtils()
         python_path = self.binaries[self.LANGUAGE].binary_path
         try:
@@ -36,14 +39,19 @@
             osutils=os_utils, pip_runner=pip_runner, runtime=self.runtime, architecture=self.architecture
         )
 
         package_builder = PythonPipDependencyBuilder(
             osutils=os_utils, runtime=self.runtime, dependency_builder=dependency_builder
         )
         try:
+            target_artifact_dir = self.artifacts_dir
+            # if dependencies folder is provided, download the dependencies into dependencies folder
+            if self.dependencies_dir:
+                target_artifact_dir = self.dependencies_dir
+
             package_builder.build_dependencies(
-                artifacts_dir_path=self.artifacts_dir,
+                artifacts_dir_path=target_artifact_dir,
                 scratch_dir_path=self.scratch_dir,
                 requirements_path=self.manifest_path,
             )
         except PackagerError as ex:
             raise ActionFailedError(str(ex))
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/python_pip/validator.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/python_pip/validator.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/actions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 """
-NodeJS NPM Workflow
+Actions for Go dependency resolution with dep
 """
-import logging
-
-from aws_lambda_builders.path_resolver import PathResolver
-from aws_lambda_builders.workflow import BaseWorkflow, Capability
-from aws_lambda_builders.actions import CopySourceAction
-
-from .actions import NodejsNpmPackAction, NodejsNpmInstallAction, NodejsNpmrcCopyAction, NodejsNpmrcCleanUpAction
-from .utils import OSUtils
-from .npm import SubprocessNpm
 
-LOG = logging.getLogger(__name__)
+import logging
+import os
 
+from aws_lambda_builders.actions import BaseAction, Purpose, ActionFailedError
+from aws_lambda_builders.architecture import X86_64, ARM64
+from aws_lambda_builders.utils import get_goarch
 
-class NodejsNpmWorkflow(BaseWorkflow):
 
-    """
-    A Lambda builder workflow that knows how to pack
-    NodeJS projects using NPM.
-    """
+from .subproc_exec import ExecutionError
 
-    NAME = "NodejsNpmBuilder"
 
-    CAPABILITY = Capability(language="nodejs", dependency_manager="npm", application_framework=None)
+LOG = logging.getLogger(__name__)
 
-    EXCLUDED_FILES = (".aws-sam", ".git")
 
-    def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, osutils=None, **kwargs):
+class DepEnsureAction(BaseAction):
 
-        super(NodejsNpmWorkflow, self).__init__(
-            source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=runtime, **kwargs
-        )
+    """
+    A Lambda Builder Action which runs dep to install dependencies from Gopkg.toml
+    """
 
-        if osutils is None:
-            osutils = OSUtils()
+    NAME = "DepEnsure"
+    DESCRIPTION = "Ensures all dependencies are installed for a project"
+    PURPOSE = Purpose.RESOLVE_DEPENDENCIES
 
-        subprocess_npm = SubprocessNpm(osutils)
+    def __init__(self, base_dir, subprocess_dep):
+        super(DepEnsureAction, self).__init__()
 
-        tar_dest_dir = osutils.joinpath(scratch_dir, "unpacked")
-        tar_package_dir = osutils.joinpath(tar_dest_dir, "package")
+        self.base_dir = base_dir
+        self.subprocess_dep = subprocess_dep
 
-        if osutils.file_exists(manifest_path):
-            npm_pack = NodejsNpmPackAction(
-                tar_dest_dir, scratch_dir, manifest_path, osutils=osutils, subprocess_npm=subprocess_npm
-            )
+    def execute(self):
+        try:
+            self.subprocess_dep.run(["ensure"], cwd=self.base_dir)
+        except ExecutionError as ex:
+            raise ActionFailedError(str(ex))
 
-            npm_install = NodejsNpmInstallAction(artifacts_dir, subprocess_npm=subprocess_npm)
 
-            npm_copy_npmrc = NodejsNpmrcCopyAction(tar_package_dir, source_dir, osutils=osutils)
+class GoBuildAction(BaseAction):
 
-            self.actions = [
-                npm_pack,
-                npm_copy_npmrc,
-                CopySourceAction(tar_package_dir, artifacts_dir, excludes=self.EXCLUDED_FILES),
-                npm_install,
-                NodejsNpmrcCleanUpAction(artifacts_dir, osutils=osutils),
-            ]
-        else:
-            LOG.warning("package.json file not found. Continuing the build without dependencies.")
-            self.actions = [CopySourceAction(source_dir, artifacts_dir, excludes=self.EXCLUDED_FILES)]
+    """
+    A Lambda Builder Action which runs `go build` to create a binary
+    """
 
-    def get_resolvers(self):
-        """
-        specialized path resolver that just returns the list of executable for the runtime on the path.
-        """
-        return [PathResolver(runtime=self.runtime, binary="npm")]
+    NAME = "GoBuild"
+    DESCRIPTION = "Builds final binary"
+    PURPOSE = Purpose.COMPILE_SOURCE
+
+    def __init__(self, base_dir, source_path, output_path, subprocess_go, architecture=X86_64, env=None):
+        super(GoBuildAction, self).__init__()
+
+        self.base_dir = base_dir
+        self.source_path = source_path
+        self.output_path = output_path
+
+        self.subprocess_go = subprocess_go
+        self.goarch = get_goarch(architecture)
+        self.env = env if not env is None else {}
+
+    def execute(self):
+        env = self.env
+        env.update({"GOOS": "linux", "GOARCH": self.goarch})
+
+        try:
+            self.subprocess_go.run(["build", "-o", self.output_path, self.source_path], cwd=self.source_path, env=env)
+        except ExecutionError as ex:
+            raise ActionFailedError(str(ex))
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/nodejs_npm/npm.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/nodejs_npm/npm.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/resources/lambda-build-init.gradle` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/resources/lambda-build-init.gradle`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/gradle_resolver.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/gradle_resolver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Gradle executable resolution
 """
 
-from .utils import OSUtils
+from aws_lambda_builders.workflows.java.utils import OSUtils
 
 
 class GradleResolver(object):
     def __init__(self, executable_search_paths=None, os_utils=None):
         self.binary = "gradle"
         self.executables = [self.binary]
         self.executable_search_paths = executable_search_paths
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/workflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Java Gradle Workflow
 """
 import hashlib
 import os
+from aws_lambda_builders.actions import CleanUpAction
 from aws_lambda_builders.workflow import BaseWorkflow, Capability
+from aws_lambda_builders.workflows.java.actions import JavaCopyDependenciesAction, JavaMoveDependenciesAction
+from aws_lambda_builders.workflows.java.utils import OSUtils
 
 from .actions import JavaGradleBuildAction, JavaGradleCopyArtifactsAction
 from .gradle import SubprocessGradle
-from .utils import OSUtils
 from .gradle_resolver import GradleResolver
 from .gradle_validator import GradleValidator
 
 
 class JavaGradleWorkflow(BaseWorkflow):
     """
     A Lambda builder workflow that knows how to build Java projects using Gradle.
@@ -32,14 +34,23 @@
         subprocess_gradle = SubprocessGradle(gradle_binary=self.binaries["gradle"], os_utils=self.os_utils)
 
         self.actions = [
             JavaGradleBuildAction(source_dir, manifest_path, subprocess_gradle, scratch_dir, self.os_utils),
             JavaGradleCopyArtifactsAction(source_dir, artifacts_dir, self.build_output_dir, self.os_utils),
         ]
 
+        if self.dependencies_dir:
+            # clean up the dependencies first
+            self.actions.append(CleanUpAction(self.dependencies_dir))
+
+            if self.combine_dependencies:
+                self.actions.append(JavaCopyDependenciesAction(artifacts_dir, self.dependencies_dir, self.os_utils))
+            else:
+                self.actions.append(JavaMoveDependenciesAction(artifacts_dir, self.dependencies_dir, self.os_utils))
+
     def get_resolvers(self):
         return [GradleResolver(executable_search_paths=self.executable_search_paths)]
 
     def get_validators(self):
         return [GradleValidator(self.runtime, self.architecture, self.os_utils)]
 
     @property
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/gradle.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/gradle.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/java_gradle/gradle_validator.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/java_gradle/gradle_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Gradle Binary Validation
 """
 
 import logging
 import re
 
+from aws_lambda_builders.workflows.java.utils import OSUtils
 from aws_lambda_builders.validator import RuntimeValidator
 
-from .utils import OSUtils
-
 
 LOG = logging.getLogger(__name__)
 
 
 class GradleValidator(RuntimeValidator):
     VERSION_STRING_WARNING = (
         "%s failed to return a version string using the '-v' option. The workflow is unable to "
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/subproc_exec.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/subproc_exec.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/go_dep/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/go_dep/workflow.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/workflow.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 """
-Go Dep Workflow
+ProvidedMakeWorkflow
 """
-
-import logging
-import os
-
-from aws_lambda_builders.actions import CopySourceAction
+from aws_lambda_builders.workflows.custom_make.validator import CustomMakeRuntimeValidator
 from aws_lambda_builders.workflow import BaseWorkflow, Capability
-from .actions import DepEnsureAction, GoBuildAction
+from aws_lambda_builders.actions import CopySourceAction
+from aws_lambda_builders.path_resolver import PathResolver
+from .actions import CustomMakeAction
 from .utils import OSUtils
-from .subproc_exec import SubprocessExec
+from .make import SubProcessMake
+from ...exceptions import WorkflowFailedError
 
-LOG = logging.getLogger(__name__)
 
+class CustomMakeWorkflow(BaseWorkflow):
 
-class GoDepWorkflow(BaseWorkflow):
     """
-    A Lambda builder workflow that knows how to build
-    Go projects using `dep`
+    A Lambda builder workflow for provided runtimes based on make.
     """
 
-    NAME = "GoDepBuilder"
+    NAME = "CustomMakeBuilder"
 
-    CAPABILITY = Capability(language="go", dependency_manager="dep", application_framework=None)
+    CAPABILITY = Capability(language="provided", dependency_manager=None, application_framework=None)
 
     EXCLUDED_FILES = (".aws-sam", ".git")
 
     def __init__(self, source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=None, osutils=None, **kwargs):
 
-        super(GoDepWorkflow, self).__init__(
+        super(CustomMakeWorkflow, self).__init__(
             source_dir, artifacts_dir, scratch_dir, manifest_path, runtime=runtime, **kwargs
         )
 
-        options = kwargs["options"] if "options" in kwargs else {}
-        handler = options.get("artifact_executable_name", None)
+        self.os_utils = OSUtils()
+
+        # Find the logical id of the function to be built.
+        options = kwargs.get("options") or {}
+        build_logical_id = options.get("build_logical_id", None)
+
+        if not build_logical_id:
+            raise WorkflowFailedError(
+                workflow_name=self.NAME,
+                action_name=None,
+                reason="Build target {} is not found!".format(build_logical_id),
+            )
+
+        subprocess_make = SubProcessMake(make_exe=self.binaries["make"].binary_path, osutils=self.os_utils)
+
+        make_action = CustomMakeAction(
+            artifacts_dir,
+            scratch_dir,
+            manifest_path,
+            osutils=self.os_utils,
+            subprocess_make=subprocess_make,
+            build_logical_id=build_logical_id,
+        )
+
+        self.actions = [CopySourceAction(source_dir, scratch_dir, excludes=self.EXCLUDED_FILES), make_action]
 
-        if osutils is None:
-            osutils = OSUtils()
+    def get_resolvers(self):
+        return [PathResolver(runtime="provided", binary="make", executable_search_paths=self.executable_search_paths)]
 
-        # project base name, where the Gopkg.toml and vendor dir are.
-        base_dir = osutils.abspath(osutils.dirname(manifest_path))
-        output_path = osutils.joinpath(osutils.abspath(artifacts_dir), handler)
-
-        subprocess_dep = SubprocessExec(osutils, "dep")
-        subprocess_go = SubprocessExec(osutils, "go")
-
-        self.actions = [
-            DepEnsureAction(base_dir, subprocess_dep),
-            GoBuildAction(
-                base_dir,
-                osutils.abspath(source_dir),
-                output_path,
-                subprocess_go,
-                self.architecture,
-                env=osutils.environ,
-            ),
-        ]
+    def get_validators(self):
+        return [CustomMakeRuntimeValidator(runtime=self.runtime, architecture=self.architecture)]
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/DESIGN.md` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/DESIGN.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/utils.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/make.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/make.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/workflows/custom_make/actions.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/workflows/custom_make/actions.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders/validator.py` & `aws_lambda_builders-1.9.0/aws_lambda_builders/validator.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/PKG-INFO` & `aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aws_lambda_builders
-Version: 1.8.1
+Name: aws-lambda-builders
+Version: 1.9.0
 Summary: Python library to compile, build & package AWS Lambda functions for several runtimes & frameworks.
 Home-page: https://github.com/awslabs/aws-lambda-builders
 Author: Amazon Web Services
 Author-email: aws-sam-developers@amazon.com
 License: Apache License 2.0
 Keywords: AWS Lambda Functions Building
 Platform: UNKNOWN
@@ -12,21 +12,22 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.6
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 ## Lambda Builders
 
 [![Build status](https://ci.appveyor.com/api/projects/status/mrehrn5im0305lje/branch/develop?svg=true)](https://ci.appveyor.com/project/AWSSAMCLI/aws-lambda-builders/branch/develop)
```

### Comparing `aws_lambda_builders-1.8.1/README.md` & `aws_lambda_builders-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/PKG-INFO` & `aws_lambda_builders-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aws-lambda-builders
-Version: 1.8.1
+Name: aws_lambda_builders
+Version: 1.9.0
 Summary: Python library to compile, build & package AWS Lambda functions for several runtimes & frameworks.
 Home-page: https://github.com/awslabs/aws-lambda-builders
 Author: Amazon Web Services
 Author-email: aws-sam-developers@amazon.com
 License: Apache License 2.0
 Keywords: AWS Lambda Functions Building
 Platform: UNKNOWN
@@ -12,21 +12,22 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.6
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 ## Lambda Builders
 
 [![Build status](https://ci.appveyor.com/api/projects/status/mrehrn5im0305lje/branch/develop?svg=true)](https://ci.appveyor.com/project/AWSSAMCLI/aws-lambda-builders/branch/develop)
```

### Comparing `aws_lambda_builders-1.8.1/aws_lambda_builders.egg-info/SOURCES.txt` & `aws_lambda_builders-1.9.0/aws_lambda_builders.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,30 +48,31 @@
 aws_lambda_builders/workflows/go_modules/DESIGN.md
 aws_lambda_builders/workflows/go_modules/__init__.py
 aws_lambda_builders/workflows/go_modules/actions.py
 aws_lambda_builders/workflows/go_modules/builder.py
 aws_lambda_builders/workflows/go_modules/utils.py
 aws_lambda_builders/workflows/go_modules/validator.py
 aws_lambda_builders/workflows/go_modules/workflow.py
+aws_lambda_builders/workflows/java/__init__.py
+aws_lambda_builders/workflows/java/actions.py
+aws_lambda_builders/workflows/java/utils.py
 aws_lambda_builders/workflows/java_gradle/DESIGN.md
 aws_lambda_builders/workflows/java_gradle/__init__.py
 aws_lambda_builders/workflows/java_gradle/actions.py
 aws_lambda_builders/workflows/java_gradle/gradle.py
 aws_lambda_builders/workflows/java_gradle/gradle_resolver.py
 aws_lambda_builders/workflows/java_gradle/gradle_validator.py
-aws_lambda_builders/workflows/java_gradle/utils.py
 aws_lambda_builders/workflows/java_gradle/workflow.py
 aws_lambda_builders/workflows/java_gradle/resources/lambda-build-init.gradle
 aws_lambda_builders/workflows/java_maven/DESIGN.md
 aws_lambda_builders/workflows/java_maven/__init__.py
 aws_lambda_builders/workflows/java_maven/actions.py
 aws_lambda_builders/workflows/java_maven/maven.py
 aws_lambda_builders/workflows/java_maven/maven_resolver.py
 aws_lambda_builders/workflows/java_maven/maven_validator.py
-aws_lambda_builders/workflows/java_maven/utils.py
 aws_lambda_builders/workflows/java_maven/workflow.py
 aws_lambda_builders/workflows/nodejs_npm/DESIGN.md
 aws_lambda_builders/workflows/nodejs_npm/__init__.py
 aws_lambda_builders/workflows/nodejs_npm/actions.py
 aws_lambda_builders/workflows/nodejs_npm/npm.py
 aws_lambda_builders/workflows/nodejs_npm/utils.py
 aws_lambda_builders/workflows/nodejs_npm/workflow.py
```

### Comparing `aws_lambda_builders-1.8.1/setup.py` & `aws_lambda_builders-1.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,30 +39,31 @@
     long_description=read("README.md"),
     author="Amazon Web Services",
     author_email="aws-sam-developers@amazon.com",
     url="https://github.com/awslabs/aws-lambda-builders",
     license="Apache License 2.0",
     packages=find_packages(exclude=["tests.*", "tests"]),
     keywords="AWS Lambda Functions Building",
-    # Support Python 2.7 and 3.6 or greater
-    python_requires=(">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*"),
+    # Support 3.6 or greater
+    python_requires=(">=3.6"),
     entry_points={"console_scripts": ["{}=aws_lambda_builders.__main__:main".format(cmd_name)]},
     install_requires=read_requirements("base.txt") + read_requirements("python_pip.txt"),
     extras_require={"dev": read_requirements("dev.txt")},
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Internet",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Utilities",
     ],
 )
```

### Comparing `aws_lambda_builders-1.8.1/LICENSE` & `aws_lambda_builders-1.9.0/LICENSE`

 * *Files identical despite different names*

