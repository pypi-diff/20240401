# Comparing `tmp/fedrq-0.9.0.tar.gz` & `tmp/fedrq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedrq-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedrq-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedrq-0.9.0.tar` & `fedrq-1.0.0.tar`

### file list

```diff
@@ -1,131 +1,167 @@
--rw-r--r--   0        0        0      749 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/epel9.yml
--rw-r--r--   0        0        0     2348 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/main.yml
--rw-r--r--   0        0        0     1187 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/mockbuild-37.yml
--rw-r--r--   0        0        0      791 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      264 2023-06-26 23:03:24.118349 fedrq-0.9.0/.copr/Makefile
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
--rw-r--r--   0        0        0      268 2023-06-26 23:03:24.119349 fedrq-0.9.0/.gitignore
--rw-r--r--   0        0        0     2553 2023-06-26 23:03:24.119349 fedrq-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    17337 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2427 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     1211 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0    14474 2023-06-29 17:37:52.842689 fedrq-0.9.0/NEWS.md
--rw-r--r--   0        0        0       89 2023-06-26 23:03:24.120349 fedrq-0.9.0/NEWS.md.license
--rw-r--r--   0        0        0    12644 2023-06-29 17:31:29.461913 fedrq-0.9.0/README.md
--rwxr-xr-x   0        0        0      687 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/add_frag.py
--rwxr-xr-x   0        0        0      906 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/api_examples/a_noarch_bash.py
--rwxr-xr-x   0        0        0     2502 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/api_examples/ftbfs_retirements.py
--rw-r--r--   0        0        0      548 2023-06-28 23:32:16.904799 fedrq-0.9.0/contrib/container/Containerfile
--rw-r--r--   0        0        0      573 2023-06-29 17:14:01.127260 fedrq-0.9.0/contrib/container/Containerfile.rhel
--rw-r--r--   0        0        0      759 2023-06-28 23:32:16.904799 fedrq-0.9.0/contrib/container/build.yml
--rw-r--r--   0        0        0      446 2023-06-29 17:17:07.001666 fedrq-0.9.0/contrib/container/rhel.toml
--rw-r--r--   0        0        0      630 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/deploy-docsite/main.yaml
--rw-r--r--   0        0        0      183 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
--rw-r--r--   0        0        0      885 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
--rw-r--r--   0        0        0      163 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
--rw-r--r--   0        0        0      415 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
--rw-r--r--   0        0        0      156 2023-06-26 23:03:24.123349 fedrq-0.9.0/contrib/deploy-docsite/vars.yaml
--rwxr-xr-x   0        0        0      914 2023-06-26 23:03:24.123349 fedrq-0.9.0/contrib/fedoraify.py
--rw-r--r--   0        0        0     5728 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/Summary.md
--rw-r--r--   0        0        0      147 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/backends/base.md
--rw-r--r--   0        0        0      343 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/backends/dnf.md
--rw-r--r--   0        0        0      532 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/backends/libdnf5.md
--rw-r--r--   0        0        0      133 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/config.md
--rw-r--r--   0        0        0      145 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/API/release_repo.md
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/News.md -> ../NEWS.md
--rw-r--r--   0        0        0     3322 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/dnf-repoquery-diff.md
--rw-r--r--   0        0        0    16598 2023-06-29 16:24:22.948766 fedrq-0.9.0/doc/fedrq.1.scd
--rw-r--r--   0        0        0       98 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/fedrq.1.scd.license
--rw-r--r--   0        0        0     4958 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/fedrq.5.scd
--rw-r--r--   0        0        0       98 2023-06-26 23:03:24.125349 fedrq-0.9.0/doc/fedrq.5.scd.license
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.125349 fedrq-0.9.0/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      193 2023-06-26 23:03:24.125349 fedrq-0.9.0/fedrq.rpmlintrc
--rw-r--r--   0        0        0     3641 2023-06-29 17:37:52.482691 fedrq-0.9.0/fedrq.spec
--rw-r--r--   0        0        0     2169 2023-06-26 23:03:24.125349 fedrq-0.9.0/mkdocs.yml
--rw-r--r--   0        0        0     6722 2023-06-29 03:33:21.071453 fedrq-0.9.0/noxfile.py
--rw-r--r--   0        0        0     3496 2023-06-29 16:24:22.847766 fedrq-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      532 2023-06-26 23:03:24.126349 fedrq-0.9.0/ruff.toml
--rw-r--r--   0        0        0      371 2023-06-29 17:37:47.357707 fedrq-0.9.0/src/fedrq/__init__.py
--rw-r--r--   0        0        0      219 2023-06-26 23:03:24.126349 fedrq-0.9.0/src/fedrq/__main__.py
--rw-r--r--   0        0        0     2822 2023-06-28 23:32:16.252803 fedrq-0.9.0/src/fedrq/_archive.py
--rw-r--r--   0        0        0     1713 2023-06-26 23:03:24.126349 fedrq-0.9.0/src/fedrq/_compat.py
--rw-r--r--   0        0        0      173 2023-06-26 23:03:24.126349 fedrq-0.9.0/src/fedrq/_config.py
--rw-r--r--   0        0        0     1268 2023-06-28 23:32:16.468802 fedrq-0.9.0/src/fedrq/_utils.py
--rw-r--r--   0        0        0     2526 2023-06-26 23:03:24.127349 fedrq-0.9.0/src/fedrq/backends/__init__.py
--rw-r--r--   0        0        0    14850 2023-06-29 16:24:22.745766 fedrq-0.9.0/src/fedrq/backends/base.py
--rw-r--r--   0        0        0      630 2023-06-26 23:03:24.127349 fedrq-0.9.0/src/fedrq/backends/dnf/__init__.py
--rw-r--r--   0        0        0     7039 2023-06-29 02:38:33.991820 fedrq-0.9.0/src/fedrq/backends/dnf/backend.py
--rw-r--r--   0        0        0      741 2023-06-26 23:03:24.128349 fedrq-0.9.0/src/fedrq/backends/libdnf5/__init__.py
--rw-r--r--   0        0        0    29790 2023-06-29 16:40:18.859715 fedrq-0.9.0/src/fedrq/backends/libdnf5/backend.py
--rw-r--r--   0        0        0     2313 2023-06-28 23:32:16.795800 fedrq-0.9.0/src/fedrq/cli/__init__.py
--rw-r--r--   0        0        0    17914 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/base.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.129349 fedrq-0.9.0/src/fedrq/cli/commands/__init__.py
--rw-r--r--   0        0        0     5672 2023-06-28 23:32:16.795800 fedrq-0.9.0/src/fedrq/cli/commands/download.py
--rw-r--r--   0        0        0     1926 2023-06-28 23:32:16.577801 fedrq-0.9.0/src/fedrq/cli/commands/pkgs.py
--rw-r--r--   0        0        0     1425 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/commands/repolist.py
--rw-r--r--   0        0        0     2394 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/commands/subpkgs.py
--rw-r--r--   0        0        0    10020 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/commands/whatrequires.py
--rw-r--r--   0        0        0    13218 2023-06-28 02:09:36.446265 fedrq-0.9.0/src/fedrq/cli/formatters.py
--rw-r--r--   0        0        0    16472 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/config.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/__init__.py
--rw-r--r--   0        0        0     9322 2023-06-28 02:09:36.446265 fedrq-0.9.0/src/fedrq/data/releases.toml
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/repos/__init__.py
--rw-r--r--   0        0        0     2053 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/repos/almalinux.repo
--rw-r--r--   0        0        0      639 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/repos/amazonlinux.repo
--rw-r--r--   0        0        0     1386 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream-compose.repo
--rw-r--r--   0        0        0     1850 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream.repo
--rw-r--r--   0        0        0     1494 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream8-compose.repo
--rw-r--r--   0        0        0     1599 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream8.repo
--rw-r--r--   0        0        0     1342 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos7.repo
--rw-r--r--   0        0        0     1809 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/eln.repo
--rw-r--r--   0        0        0     2158 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/epel.repo
--rw-r--r--   0        0        0    14146 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/fedora-eln.repo
--rw-r--r--   0        0        0     2402 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/data/repos/fedora-rawhide.repo
--rw-r--r--   0        0        0     1480 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/data/repos/fedora-updates-testing.repo
--rw-r--r--   0        0        0     1422 2023-06-29 16:45:13.311775 fedrq-0.9.0/src/fedrq/data/repos/fedora-updates.repo
--rw-r--r--   0        0        0     1375 2023-06-29 16:45:05.106801 fedrq-0.9.0/src/fedrq/data/repos/fedora.repo
--rw-r--r--   0        0        0     1374 2023-06-28 02:09:36.446265 fedrq-0.9.0/src/fedrq/data/repos/oraclelinux-8.repo
--rw-r--r--   0        0        0     1374 2023-06-29 16:45:34.108708 fedrq-0.9.0/src/fedrq/data/repos/oraclelinux-9.repo
--rw-r--r--   0        0        0      425 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/data/repos/rawhide-buildroot.repo
--rw-r--r--   0        0        0     6475 2023-06-28 02:09:36.447265 fedrq-0.9.0/src/fedrq/data/repos/rocky.repo
--rw-r--r--   0        0        0     3505 2023-06-28 02:09:36.447265 fedrq-0.9.0/src/fedrq/data/repos/ubi.repo
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/py.typed
--rw-r--r--   0        0        0     9225 2023-06-29 16:24:22.948766 fedrq-0.9.0/src/fedrq/release_repo.py
--rw-r--r--   0        0        0      994 2023-06-26 23:03:24.134349 fedrq-0.9.0/src/fedrq/repoquery.py
--rw-r--r--   0        0        0      154 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     2948 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1775 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0      416 2023-06-28 23:32:16.795800 fedrq-0.9.0/tests/integration/test_download.py
--rw-r--r--   0        0        0      771 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/test_pkgs.py
--rw-r--r--   0        0        0     1292 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/test_subpkgs.py
--rw-r--r--   0        0        0     1761 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/integration/test_whatrequires.py
--rw-r--r--   0        0        0     1370 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/integration/test_whatrequires_src.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0      332 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/test_data/_template.spec
--rwxr-xr-x   0        0        0     1449 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/test_data/build.sh
--rw-r--r--   0        0        0     1130 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
--rw-r--r--   0        0        0     1060 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/test_data/repos/repo1/specs/packagea.spec
--rw-r--r--   0        0        0     1156 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/test_data/repos/repo1/specs/packageb.spec
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     1178 2023-06-29 01:21:42.132684 fedrq-0.9.0/tests/unit/test_archive.py
--rw-r--r--   0        0        0     2128 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/unit/test_checkconfig.py
--rw-r--r--   0        0        0     7163 2023-06-26 23:03:24.137349 fedrq-0.9.0/tests/unit/test_command.py
--rw-r--r--   0        0        0     1351 2023-06-28 23:32:16.795800 fedrq-0.9.0/tests/unit/test_download.py
--rw-r--r--   0        0        0     9077 2023-06-28 02:09:36.447265 fedrq-0.9.0/tests/unit/test_formatters.py
--rw-r--r--   0        0        0     3361 2023-06-26 23:03:24.137349 fedrq-0.9.0/tests/unit/test_pkgs.py
--rw-r--r--   0        0        0     1681 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_release.py
--rw-r--r--   0        0        0      562 2023-06-29 16:24:22.948766 fedrq-0.9.0/tests/unit/test_release_repo.py
--rw-r--r--   0        0        0      449 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_repo.py
--rw-r--r--   0        0        0      640 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_repolist.py
--rw-r--r--   0        0        0     1325 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_repoquery.py
--rw-r--r--   0        0        0     2712 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_subbpkgs.py
--rw-r--r--   0        0        0      428 2023-06-28 23:32:16.468802 fedrq-0.9.0/tests/unit/test_util.py
--rw-r--r--   0        0        0     4088 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_whatrequires.py
--rw-r--r--   0        0        0      689 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_whatrequires_src.py
--rw-r--r--   0        0        0    14835 1970-01-01 00:00:00.000000 fedrq-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      532 2023-09-23 07:50:00.855336 fedrq-1.0.0/.builds/epel9.yml
+-rw-r--r--   0        0        0     2105 2023-09-23 07:50:00.856336 fedrq-1.0.0/.builds/main.yml
+-rw-r--r--   0        0        0      809 2023-09-23 07:50:00.856336 fedrq-1.0.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      473 2023-12-10 19:23:08.443940 fedrq-1.0.0/.builds/test.yml
+-rw-r--r--   0        0        0      384 2024-03-02 00:23:56.673824 fedrq-1.0.0/.copr/Makefile
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
+lrwxr-xr-x   0        0        0        0 2024-02-27 23:08:32.868655 fedrq-1.0.0/.dockerignore -> .gitignore
+-rw-r--r--   0        0        0      287 2024-04-01 17:06:49.284414 fedrq-1.0.0/.gitignore
+-rw-r--r--   0        0        0      155 2023-09-23 07:50:00.857336 fedrq-1.0.0/.reuse/dep5
+-rw-r--r--   0        0        0     2553 2023-06-26 23:03:24.119349 fedrq-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      673 2024-02-28 18:14:09.530518 fedrq-1.0.0/Containerfile
+-rw-r--r--   0        0        0      817 2024-02-28 18:14:09.531518 fedrq-1.0.0/Containerfile.rhel
+-rw-r--r--   0        0        0     1564 2024-02-28 18:14:09.532518 fedrq-1.0.0/Containerfile.rhel8
+-rw-r--r--   0        0        0    17337 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2427 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     1211 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0    19096 2024-04-01 17:09:57.580057 fedrq-1.0.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-06-26 23:03:24.120349 fedrq-1.0.0/NEWS.md.license
+-rw-r--r--   0        0        0    13182 2024-02-09 05:24:13.924912 fedrq-1.0.0/README.md
+-rwxr-xr-x   0        0        0      687 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/add_frag.py
+-rwxr-xr-x   0        0        0      906 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/api_examples/a_noarch_bash.py
+-rwxr-xr-x   0        0        0     2502 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/api_examples/ftbfs_retirements.py
+-rw-r--r--   0        0        0      103 2023-09-23 07:50:00.861336 fedrq-1.0.0/contrib/container/000-container.toml
+-rw-r--r--   0        0        0      641 2024-02-28 18:14:09.532518 fedrq-1.0.0/contrib/container/Containerfile
+-rw-r--r--   0        0        0      722 2024-02-28 18:14:09.533518 fedrq-1.0.0/contrib/container/Containerfile.rhel
+-rw-r--r--   0        0        0      759 2023-10-15 18:51:34.227066 fedrq-1.0.0/contrib/container/build.yml
+-rwxr-xr-x   0        0        0      296 2023-09-23 07:50:00.863336 fedrq-1.0.0/contrib/container/entrypoint.sh
+-rw-r--r--   0        0        0      544 2023-09-23 07:50:00.863336 fedrq-1.0.0/contrib/container/rhel.toml
+-rw-r--r--   0        0        0      544 2024-02-28 18:14:09.533518 fedrq-1.0.0/contrib/container/rhel8.toml
+-rw-r--r--   0        0        0      630 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/deploy-docsite/main.yaml
+-rw-r--r--   0        0        0      183 2023-06-26 23:03:24.122349 fedrq-1.0.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
+-rw-r--r--   0        0        0      885 2023-06-26 23:03:24.122349 fedrq-1.0.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
+-rw-r--r--   0        0        0      284 2023-09-18 05:35:56.213359 fedrq-1.0.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
+-rw-r--r--   0        0        0      415 2023-06-26 23:03:24.122349 fedrq-1.0.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
+-rw-r--r--   0        0        0      156 2023-06-26 23:03:24.123349 fedrq-1.0.0/contrib/deploy-docsite/vars.yaml
+-rwxr-xr-x   0        0        0      914 2023-06-26 23:03:24.123349 fedrq-1.0.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     6047 2024-03-18 02:08:06.660954 fedrq-1.0.0/doc/API/Summary.md
+-rw-r--r--   0        0        0      204 2023-12-08 02:08:39.952633 fedrq-1.0.0/doc/API/_archive.md
+-rw-r--r--   0        0        0      147 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/backends/base.md
+-rw-r--r--   0        0        0      343 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/backends/dnf.md
+-rw-r--r--   0        0        0      532 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/backends/libdnf5.md
+-rw-r--r--   0        0        0      133 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/config.md
+-rw-r--r--   0        0        0      214 2023-12-08 02:07:21.668887 fedrq-1.0.0/doc/API/release_repo.md
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.124349 fedrq-1.0.0/doc/News.md -> ../NEWS.md
+-rw-r--r--   0        0        0     4254 2024-02-09 05:26:11.065414 fedrq-1.0.0/doc/dnf-repoquery-diff.md
+-rw-r--r--   0        0        0    21314 2024-04-01 16:51:28.499461 fedrq-1.0.0/doc/fedrq.1.scd
+-rw-r--r--   0        0        0       98 2023-06-26 23:03:24.124349 fedrq-1.0.0/doc/fedrq.1.scd.license
+-rw-r--r--   0        0        0     5024 2024-02-08 21:05:40.487851 fedrq-1.0.0/doc/fedrq.5.scd
+-rw-r--r--   0        0        0       98 2023-06-26 23:03:24.125349 fedrq-1.0.0/doc/fedrq.5.scd.license
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.125349 fedrq-1.0.0/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      583 2024-02-08 21:00:35.705899 fedrq-1.0.0/doc/mkdocs_mangen.py
+-rw-r--r--   0        0        0      193 2023-06-26 23:03:24.125349 fedrq-1.0.0/fedrq.rpmlintrc
+-rw-r--r--   0        0        0     4292 2024-04-01 17:09:56.826058 fedrq-1.0.0/fedrq.spec
+-rw-r--r--   0        0        0     2300 2024-02-08 20:47:24.834435 fedrq-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0     8384 2024-04-01 17:08:37.764166 fedrq-1.0.0/noxfile.py
+-rw-r--r--   0        0        0     4001 2024-02-09 05:28:42.366800 fedrq-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4849 2024-04-01 16:53:31.810130 fedrq-1.0.0/requirements/all.txt
+-rw-r--r--   0        0        0     1118 2024-03-25 01:38:31.567468 fedrq-1.0.0/requirements/codeqa.txt
+-rw-r--r--   0        0        0     3820 2024-04-01 16:53:31.811130 fedrq-1.0.0/requirements/doc.txt
+-rw-r--r--   0        0        0     1019 2024-03-18 01:55:52.346007 fedrq-1.0.0/requirements/formatters.txt
+-rw-r--r--   0        0        0       13 2023-09-23 07:50:00.868336 fedrq-1.0.0/requirements/pydanticv1.in
+-rw-r--r--   0        0        0     1030 2024-03-25 01:38:31.569468 fedrq-1.0.0/requirements/pydanticv1_test.txt
+-rw-r--r--   0        0        0     1516 2023-09-23 07:50:00.868336 fedrq-1.0.0/requirements/refresh.yml
+-rw-r--r--   0        0        0      703 2024-03-18 01:55:52.346007 fedrq-1.0.0/requirements/requirements.txt
+-rw-r--r--   0        0        0        7 2023-09-23 07:50:00.869336 fedrq-1.0.0/requirements/srpm.in
+-rw-r--r--   0        0        0      448 2024-04-01 16:53:31.811130 fedrq-1.0.0/requirements/srpm.txt
+-rw-r--r--   0        0        0     1044 2024-03-25 01:38:31.570468 fedrq-1.0.0/requirements/test.txt
+-rw-r--r--   0        0        0     1056 2024-03-18 01:55:52.346007 fedrq-1.0.0/requirements/typing.txt
+-rw-r--r--   0        0        0     1162 2024-03-18 02:02:24.166704 fedrq-1.0.0/ruff.toml
+-rw-r--r--   0        0        0      753 2024-04-01 17:09:50.809067 fedrq-1.0.0/src/fedrq/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-26 23:03:24.126349 fedrq-1.0.0/src/fedrq/__main__.py
+-rw-r--r--   0        0        0     2822 2024-01-07 21:00:32.692014 fedrq-1.0.0/src/fedrq/_archive.py
+-rw-r--r--   0        0        0     1713 2023-09-11 04:00:33.008787 fedrq-1.0.0/src/fedrq/_compat.py
+-rw-r--r--   0        0        0      173 2023-06-26 23:03:24.126349 fedrq-1.0.0/src/fedrq/_config.py
+-rw-r--r--   0        0        0     1370 2023-12-23 06:34:35.309654 fedrq-1.0.0/src/fedrq/_utils.py
+-rw-r--r--   0        0        0     2645 2023-12-18 18:23:31.398146 fedrq-1.0.0/src/fedrq/backends/__init__.py
+-rw-r--r--   0        0        0    17124 2024-01-30 01:19:25.798526 fedrq-1.0.0/src/fedrq/backends/base/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-26 23:03:24.127349 fedrq-1.0.0/src/fedrq/backends/dnf/__init__.py
+-rw-r--r--   0        0        0     8305 2024-02-13 03:17:16.970902 fedrq-1.0.0/src/fedrq/backends/dnf/backend/__init__.py
+-rw-r--r--   0        0        0      629 2023-09-23 07:50:00.872336 fedrq-1.0.0/src/fedrq/backends/libdnf5/__init__.py
+-rw-r--r--   0        0        0    27966 2024-01-08 18:50:00.087299 fedrq-1.0.0/src/fedrq/backends/libdnf5/backend/__init__.py
+-rw-r--r--   0        0        0     2667 2024-02-07 02:23:15.413353 fedrq-1.0.0/src/fedrq/cli/__init__.py
+-rw-r--r--   0        0        0    17869 2024-02-28 18:14:09.546517 fedrq-1.0.0/src/fedrq/cli/base.py
+-rw-r--r--   0        0        0      758 2023-11-06 03:39:21.572134 fedrq-1.0.0/src/fedrq/cli/commands/COMMAND.py.in
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.129349 fedrq-1.0.0/src/fedrq/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1228 2023-11-06 23:45:40.679278 fedrq-1.0.0/src/fedrq/cli/commands/cache.py
+-rw-r--r--   0        0        0     2427 2024-02-11 23:38:01.083470 fedrq-1.0.0/src/fedrq/cli/commands/changelogs.py
+-rw-r--r--   0        0        0     6390 2024-01-07 21:00:32.693014 fedrq-1.0.0/src/fedrq/cli/commands/download.py
+-rw-r--r--   0        0        0     1926 2024-02-07 02:26:01.958945 fedrq-1.0.0/src/fedrq/cli/commands/formatters.py
+-rw-r--r--   0        0        0     1729 2023-11-06 04:24:41.488764 fedrq-1.0.0/src/fedrq/cli/commands/pkgs.py
+-rw-r--r--   0        0        0     1425 2023-09-23 07:50:00.875336 fedrq-1.0.0/src/fedrq/cli/commands/repolist.py
+-rw-r--r--   0        0        0     2394 2023-09-23 07:50:00.876336 fedrq-1.0.0/src/fedrq/cli/commands/subpkgs.py
+-rw-r--r--   0        0        0    10927 2024-03-02 04:35:52.918510 fedrq-1.0.0/src/fedrq/cli/commands/whatrequires.py
+-rw-r--r--   0        0        0    18643 2024-03-18 01:57:56.367426 fedrq-1.0.0/src/fedrq/cli/formatters.py
+-rw-r--r--   0        0        0    16327 2024-01-08 17:19:25.034112 fedrq-1.0.0/src/fedrq/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/__init__.py
+-rw-r--r--   0        0        0     9590 2023-12-20 20:41:15.739589 fedrq-1.0.0/src/fedrq/data/releases.toml
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/repos/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/repos/almalinux.repo
+-rw-r--r--   0        0        0      639 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/repos/amazonlinux.repo
+-rw-r--r--   0        0        0     1386 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream-compose.repo
+-rw-r--r--   0        0        0     1850 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream.repo
+-rw-r--r--   0        0        0     1494 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream8-compose.repo
+-rw-r--r--   0        0        0     1599 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream8.repo
+-rw-r--r--   0        0        0     1342 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos7.repo
+-rw-r--r--   0        0        0      389 2023-12-20 20:39:55.482913 fedrq-1.0.0/src/fedrq/data/repos/eln-buildroot.repo
+-rw-r--r--   0        0        0     1809 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/eln.repo
+-rw-r--r--   0        0        0     2158 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/epel.repo
+-rw-r--r--   0        0        0    14146 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/fedora-eln.repo
+-rw-r--r--   0        0        0     2402 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/data/repos/fedora-rawhide.repo
+-rw-r--r--   0        0        0     1480 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/data/repos/fedora-updates-testing.repo
+-rw-r--r--   0        0        0     1422 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/fedora-updates.repo
+-rw-r--r--   0        0        0     1375 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/fedora.repo
+-rw-r--r--   0        0        0     1374 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-8.repo
+-rw-r--r--   0        0        0     1374 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-9.repo
+-rw-r--r--   0        0        0      425 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/data/repos/rawhide-buildroot.repo
+-rw-r--r--   0        0        0     6475 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/rocky.repo
+-rw-r--r--   0        0        0     3505 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/ubi.repo
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/py.typed
+-rw-r--r--   0        0        0     9259 2024-01-30 01:19:25.593526 fedrq-1.0.0/src/fedrq/release_repo.py
+-rw-r--r--   0        0        0     1828 2024-01-08 18:49:59.600302 fedrq-1.0.0/src/fedrq/repoquery.py
+-rw-r--r--   0        0        0      154 2023-06-26 23:03:24.134349 fedrq-1.0.0/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2988 2023-09-23 07:50:00.879336 fedrq-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-1.0.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1748 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_backends.py
+-rw-r--r--   0        0        0      405 2023-11-06 23:48:33.545619 fedrq-1.0.0/tests/integration/test_cache.py
+-rw-r--r--   0        0        0      553 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_download.py
+-rw-r--r--   0        0        0      988 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_pkgs.py
+-rw-r--r--   0        0        0     1483 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_subpkgs.py
+-rw-r--r--   0        0        0     1964 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_whatrequires.py
+-rw-r--r--   0        0        0     1447 2023-09-23 07:50:00.881336 fedrq-1.0.0/tests/integration/test_whatrequires_src.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.135349 fedrq-1.0.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      408 2024-02-07 03:25:08.056407 fedrq-1.0.0/tests/test_data/_template.spec
+-rwxr-xr-x   0        0        0     1484 2024-02-28 18:14:09.546517 fedrq-1.0.0/tests/test_data/build.sh
+-rw-r--r--   0        0        0     1212 2023-09-23 07:50:00.881336 fedrq-1.0.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
+-rw-r--r--   0        0        0     1196 2024-01-08 18:49:59.717301 fedrq-1.0.0/tests/test_data/repos/repo1/specs/packagea.spec
+-rw-r--r--   0        0        0     1232 2023-09-23 07:50:00.881336 fedrq-1.0.0/tests/test_data/repos/repo1/specs/packageb.spec
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.136349 fedrq-1.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1193 2023-10-24 21:56:15.297461 fedrq-1.0.0/tests/unit/test_archive.py
+-rw-r--r--   0        0        0      722 2023-09-23 07:50:00.882336 fedrq-1.0.0/tests/unit/test_backend_base.py
+-rw-r--r--   0        0        0      757 2023-12-18 18:23:31.399147 fedrq-1.0.0/tests/unit/test_backends.py
+-rw-r--r--   0        0        0     2066 2023-12-15 04:34:12.105772 fedrq-1.0.0/tests/unit/test_base_maker.py
+-rw-r--r--   0        0        0      386 2023-11-06 23:46:04.528187 fedrq-1.0.0/tests/unit/test_cache.py
+-rw-r--r--   0        0        0     2113 2023-09-23 07:50:00.882336 fedrq-1.0.0/tests/unit/test_changelog.py
+-rw-r--r--   0        0        0     2128 2023-06-26 23:03:24.136349 fedrq-1.0.0/tests/unit/test_checkconfig.py
+-rw-r--r--   0        0        0     8696 2023-09-23 07:50:00.882336 fedrq-1.0.0/tests/unit/test_command.py
+-rw-r--r--   0        0        0      610 2023-12-15 04:25:23.386435 fedrq-1.0.0/tests/unit/test_dnf.py
+-rw-r--r--   0        0        0     1351 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_download.py
+-rw-r--r--   0        0        0    13062 2024-03-01 01:14:29.816477 fedrq-1.0.0/tests/unit/test_formatters.py
+-rw-r--r--   0        0        0     2407 2024-03-01 01:24:17.512465 fedrq-1.0.0/tests/unit/test_formatters_command.py
+-rw-r--r--   0        0        0      860 2024-01-08 18:50:00.087299 fedrq-1.0.0/tests/unit/test_libdnf5.py
+-rw-r--r--   0        0        0     3361 2023-06-26 23:03:24.137349 fedrq-1.0.0/tests/unit/test_pkgs.py
+-rw-r--r--   0        0        0     1681 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_release.py
+-rw-r--r--   0        0        0      562 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_release_repo.py
+-rw-r--r--   0        0        0      449 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_repo.py
+-rw-r--r--   0        0        0      640 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_repolist.py
+-rw-r--r--   0        0        0     3905 2023-12-15 04:34:12.105772 fedrq-1.0.0/tests/unit/test_repoquery.py
+-rw-r--r--   0        0        0     2712 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_subbpkgs.py
+-rw-r--r--   0        0        0      428 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_util.py
+-rw-r--r--   0        0        0     4292 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_whatrequires.py
+-rw-r--r--   0        0        0      689 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_whatrequires_src.py
+-rw-r--r--   0        0        0    15604 1970-01-01 00:00:00.000000 fedrq-1.0.0/PKG-INFO
```

### Comparing `fedrq-0.9.0/.builds/main.yml` & `fedrq-1.0.0/.builds/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 ---
 image: fedora/rawhide
 packages:
-  - createrepo_c
   - hut
   - pandoc
-  - python3-libdnf5
-  - rpm-build
+  - python3-devel
+  - python3.11-devel
+  - nox
   - rsync
   - scd2html
   - tar
 secrets:
-  # Production Copr
-  # - 759db354-8651-427c-b00a-0755164c8cae
   # Dev Copr
   - 9683b939-5f2b-4a0a-966e-acd99b5944a0
   # fedrq.gtmx.me
   - 1ec4d132-f9e9-4e00-9ba6-eb5528e6945e
-environment:
-  nox: ./venv/bin/nox
 oauth: pages.sr.ht/PAGES:RW
 sources:
   - https://git.sr.ht/~gotmax23/fedrq
 tasks:
   - copr-webhook: |
       cd fedrq/
       if ! [ -x "${HOME}/.copr-dev-hook" ]
@@ -34,21 +30,20 @@
       fi
       if [ "$(git rev-parse HEAD)" != "$(git rev-parse origin/main)" ]
       then
         echo "Not submitting copr-build. Branch is not main."
         exit
       fi
       ~/.copr-dev-hook
-  - setup-venv: |
+  - lint: |
       cd fedrq
-      python3 -m venv venv
-      ./venv/bin/pip install nox
+      nox -e lint
   - submit-docs: |
       cd fedrq
-      $nox -e mkdocs -- build
+      VIRTUALENV_PYTHON=3.11 nox -e mkdocs -- build
       if [ "$(git rev-parse HEAD)" = "$(git rev-parse origin/main)" ]; then
         echo "Submitting docs for main branch"
         ssh-keyscan fedrq.gtmx.me | tee -a ~/.ssh/known_hosts
         rsync -Pr site/. deploy@fedrq.gtmx.me:/var/www/fedrq
       fi
   - submit-man: |
       cd fedrq/doc
@@ -73,13 +68,7 @@
       else
         echo "Not submitting manpage build. Branch is not main or _dev."
         exit
       fi
 
       tar czvf fedrq.tar.gz *.html
       hut pages publish fedrq.tar.gz -d gotmax23.srht.site -s "${site}"
-  - lint: |
-      cd fedrq
-      $nox -e lint
-  - pytest: |
-      cd fedrq
-      $nox -e testa -- -v --durations=7
```

### Comparing `fedrq-0.9.0/.builds/mockbuild.yml` & `fedrq-1.0.0/.builds/mockbuild.yml`

 * *Files 19% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 ---
 image: fedora/rawhide
 packages:
   - mock
   - mock-core-configs
+  - python3.11
   - rpmlint
   - rpm-build
 sources:
   - https://git.sr.ht/~gotmax23/fedrq
 environment:
   CHROOT: fedora-rawhide
   nox: ./venv/bin/nox
 artifacts:
   - fedrq/results_fedrq.tar.gz
 tasks:
   - setup-add-mock-group: |
       sudo usermod -aG mock $USER
   - setup-venv: |
       cd fedrq
-      python3 -m venv venv
+      python3.11 -m venv venv
       ./venv/bin/pip install nox
   - mockbuild-rawhide: |
       cd fedrq
       $nox -e mockbuild -- --resultdir results_fedrq -r "${CHROOT}-$(rpm -E %_arch)"
       tar cvf results_fedrq.tar.gz results_fedrq
   - rpmlint: |
       cd fedrq/
```

### Comparing `fedrq-0.9.0/CONTRIBUTING.md` & `fedrq-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/LICENSES/GPL-2.0-or-later.txt` & `fedrq-1.0.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/LICENSES/MIT.txt` & `fedrq-1.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/LICENSES/PSF-2.0.txt` & `fedrq-1.0.0/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/LICENSES/Unlicense.txt` & `fedrq-1.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/NEWS.md` & `fedrq-1.0.0/NEWS.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,203 @@
 NEWS
 =====
 
+## 1.0.0 - 2024-04-01 <a id='1.0.0'></a>
+
+First stable release
+
+### Added
+
+- Containerfiles: add experimental UBI 8–based Containerfile
+- cli formatters: add `source+requiresmatch` and `source+rm` formatters
+
+### Changed
+
+- Containerfiles: license under `GPL-2.0-or-later`
+- doc fedrq.1: use formatting consistent with `man-pages(7)`
+
+### Fixed
+
+- doc: remove broken reference
+
+### Removed
+
+- cli formatters: remove long-deprecated `_DefaultFormatters` class (INTERNAL API)
+
+## 0.15.0 - 2024-02-13 <a id='0.15.0'></a>
+
+### Added
+
+- backends dnf: add `load_filelists()` implementation. This makes sure that
+  systems with `dnf >= 4.19.0` can, for example, use `-L always` to load
+  filelists.
+
+### Changed
+
+- doc: revamp and cleanup
+
+### Fixed
+
+- changelogs: fix off-by-one error with `--entry-limit` flag
+
+## 0.14.0 - 2024-02-07 <a id='0.14.0'></a>
+
+### Added
+
+- api: add `fedrq.cli.formatters.Formatters.formatters_it()` method
+- cli: add `formatters` subcommand to list formatters
+- formatters: add `-F multiline`
+- formatters: add `-F requiresmatch` and related formatters
+- releases: add `--branch=eln` / `--repo=buildroot` repo definition
+
+### Changed
+
+- api: clean up INTERNAL `fedrq.cli.formatters` API
+
+### Deprecated
+
+- api: deprecate standalone `fedrq.repoquery` module
+
+### Removed
+
+- all: drop support for libdnf5 version less than 5.0.12
+
+## 0.13.0 - 2023-12-18 <a id='0.13.0'></a>
+
+!!! warning
+    The next release will drop support for `libdnf5<5.0.12`
+
+### Added
+
+CLI:
+
+- cli `download` / `download-spec`: mark commands as stable and document
+- cli: add new `make-cache` subcommand
+
+---
+
+API:
+
+- backends `Repoquery.resolve_pkg_specs`: add `nevra_forms` argument
+- backends `Repoquery.resolve_pkg_specs`: allow more granular `resolve` control
+- backends: add `allow_multiple_backends_per_process` argument to `get_backend()`
+- backends: make `base` a package instead of a single module
+
+---
+
+contrib:
+
+- Caddyfile: update for 404.html template
+
+---
+
+doc:
+
+- API Summary: add dnf and libdnf5 intersphinx links
+- dnf-repoquery-diff: fix inter-doc links
+- release_repo: add unstable API warning admonition
+- add _archive.md API doc
+
+### Changed
+
+- all: use `metaclass=abc.ABCMeta` instead of inheriting `abc.ABC`
+- backends: make `libdnf5.backends.${NAME}.backend` packages instead of single modules
+- cli: correct license of changelogs and download.
+  They are now `GPL-2.0-or-later` as opposed to `MIT`.
+- doc: switch to google docstring style
+
+### Fixed
+
+- fedrq.repoquery: fix type checking
+- backends dnf: fix `BaseMaker.set_var()` error typo
+- cli whatrequires: fix typo (`Exception: Unrecognized key name: recommend`).
+
+## 0.12.0 - 2023-09-11 <a id='0.12.0'></a>
+
+### Added
+
+- whatrequires: add experimental `--extra-exact` argument
+- add support for pydantic v2
+
+## 0.11.0 - 2023-08-31 <a id='0.11.0'></a>
+
+### Added
+
+API:
+
+- backends: add `repo` @property to PackageCompat
+- BaseMaker: add `load_changelogs()`; improve `load_filelists()`
+- BaseMaker: add `conf` property
+- backends: add API for accessing Package changelogs
+
+CLI:
+
+- handle repo ssl client certificates in `download` subcommand
+- add `changelog` subcommand
+
+Container images:
+
+- add `@epel` release group to the `rhel9` release configuration in the `ubi9`
+  container
+
+General:
+
+- Declare support for Python 3.12
+
+### Deprecated
+
+API:
+
+- libdnf5 BaseMaker: deprecate config property
+
+### Fixed
+
+- fix `importlib.abc` `DeprecationWarning`.
+- improve CLI error handling by erroring out before loading metadata if other
+  non-fatal errors have occurred.
+- fix help message in `download` subcommand
+
+### Removed
+
+API:
+
+- config: remove pydantic validators from public API. These never should have
+  been exposed in the first place.
+
+## 0.10.0 - 2023-07-12 <a id='0.10.0'></a>
+
+### Added
+
+- add unconditional dependency on python3-rpm
+- container - refresh redhat.repo on entrypoint
+- add `smartcache=always` config option
+- add `--smartcache-always` CLI flag
+- add more documentation for the container builds
+
+### Changed
+
+- container - install config file to set `smartcache=always`
+- `fedrq.backends.libdnf5.backend.Package` - use libdnf5's getters for
+  `debug_name` and `source_debug_name` instead of our copies from dnf4.
+  There is still a fallback to the dnf4 versions for libdnf5 < 5.0.12.
+- fedrq.spec - favor python3-libdnf5 if dnf5 is installed
+
+### Deprecated
+
+- deprecate support for libdnf5 < 5.0.12 in the libdnf5 backend
+
+### Fixed
+
+- container - make sure cache persistence volume is actually used
+
+### Removed
+
+- remove deprecated `config.get_rq()` function
+- drop support for libdnf5 < 5.0.10 in the libdnf5 backend
+
 ## 0.9.0 - 2023-06-29 <a id='0.9.0'></a>
 
 ### Added
 
 - add remote_location formatter
 - document CentOS 7 release configuration
 - add UBI release configuration
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fedrq-0.9.0/README.md` & `fedrq-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 A tool for querying the Fedora and EPEL repositories
 
 fedrq makes it easy to query any branch of Fedora or EPEL. It uses the dnf
 Python bindings and does not shell out to `dnf repoquery`. It allows querying
 for reverse dependencies, packages that contain a certain Provide or file,
 subpackages of an SRPM, and package metadata.
 
-The tool doesn't seek to replace every feature of dnf repoquery. It provides a
+The tool doesn't seek to replace every feature of `dnf repoquery`. It provides a
 more user friendly interface than `dnf repoquery` for certain common tasks.
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/fedrq/commits/main.svg)](https://builds.sr.ht/~gotmax23/fedrq/commits/main?)
 
 [![copr build status][badge-copr]][link-copr] (stable)
 
 [![copr build status][badge-copr-dev]][link-copr-dev] (dev)
@@ -30,18 +30,18 @@
 [![fedrq on lists.sr.ht][badge-list]][link-list]
 
 [![fedrq on todo.sr.ht][badge-todo]][link-todo]
 
 
 ## Installation
 
-fedrq has a copr repository at [gotmax23/fedrq][link-copr] that contains
+fedrq has a Copr repository at [gotmax23/fedrq][link-copr] that contains
 released versions.
 Development snapshots are available at [gotmax23/fedrq-dev][link-copr-dev].
-The RPM specfile is in the repository root.
+The RPM specfile is located in the repository root.
 
 fedrq is also [published to PyPI](https://pypi.org/project/fedrq/) so you can
 `pip install fedrq`.
 
 When installing the package with pip, some additional system packages
 are needed.
 
@@ -49,14 +49,17 @@
 
 - python3-dnf (dnf is currently the default Fedora package manager, so this
   should already be installed)
 
 The following additional system packages are required for the libdnf5 backend:
 
 - python3-libdnf5
+
+The following additional system packages are always required:
+
 - python3-rpm
 
 fedrq defaults to the dnf backend, but fedrq falls back to the libdnf5 backend
 if the former's dependencies aren't installed.
 Users can explicitly choose a backend with the
 `--backend` [CLI option](https://fedrq.gtmx.me/fedrq1/#shared-options)
 or globally in the [fedrq config file](https://fedrq.gtmx.me/fedrq5).
@@ -67,76 +70,88 @@
 
 `fedrq check-config --dump` requires `tomli-w`.
 The RPM package weakly depends on `python3-tomli-w`.
 
 ## Container images
 
 fedrq now provides container images.
-- `quay.io/gotmax23/fedrq:latest` is built with
+
+- [`quay.io/gotmax23/fedrq:latest`][Containerfile] is built with
   `registry.fedoraproject.org/fedora:latest`.
-- `quay.io/gotmax23/fedrq:ubi9` is built with the ubi9 image.
+- [`quay.io/gotmax23/fedrq:ubi9`][Containerfile.rhel] is built with the ubi9
+  image.
   It includes a builtin `rhel9` repository configuration that can be used to
   query the actual RHEL repositories when run on a system registered with
   subscription-manager.
 
 Both of these images use the latest fedrq RPM packages from the
 [gotmax23/fedrq][link-copr] Copr repository.
 
+``` console
+$ podman run --rm -v ~/.cache/fedrq:/fedrq-cache/fedrq:z quay.io/gotmax23/fedrq \
+    pkgs fedrq -Fnevrr
+fedrq-0.9.0-1.fc39.noarch rawhide
+fedrq-0.9.0-1.fc39.src rawhide-source
+```
+
+[Containerfile]: https://git.sr.ht/~gotmax23/fedrq/tree/main/item/contrib/container/Containerfile
+[Containerfile.rhel]: https://git.sr.ht/~gotmax23/fedrq/tree/main/item/contrib/container/Containerfile.rhel
+
 ## Versioning
 
 This project is in beta and its versioning scheme follows semver.
 
 See [NEWS.md](https://git.sr.ht/~gotmax23/fedrq/tree/main/NEWS.md).
 
 ## Python API
 
 The `fedrq.config` module and the `fedrq.backend` package are public API.
-Everything under `fedrq.cli` is internal. fedrq is a primarily a CLI tool and
-its API abstracts the specific dnf/libdnf5 functionality that it uses. The
-API's main purpose is repoquerying, but you can use the fedrq functionality
+Everything under `fedrq.cli` is internal. fedrq is primarily a CLI tool and
+its API only abstracts the specific dnf/libdnf5 functionality that the CLI uses. The
+API's main purpose is "repoquerying", but you can use the fedrq functionality
 you'd like and then access the underlying dnf Base object to preform other
 tasks if needed.
 
 See the [API Summary] on the docsite for more information. See [api-examples]
 for some example code. As always, direct any feedback, questions, or issues to
 the mailing list (see [Contributing](#contributing)).
 
 [API Summary]: https://fedrq.gtmx.me/API/Summary/
 
 
-## Documentaion
+## Documentation
 
-See our new [docsite][link-docsite] for rendered manpages, changelogs, and
+See fedrq's [documentation site][link-docsite] for rendered manpages, changelogs, and
 Python API documentation.
 
 
 ## Contributing
 
 Development, issue reporting, and project discussion happen on [the mailing
 list][link-list] ([~gotmax23/fedrq@lists.sr.ht][mailto]).
 
 See [CONTRIBUTING.md].
 
 
 ## Credits
 Thank you to the dnf maintainers. This tool is inspired by `dnf repoquery` and
-uses the `dnf` python bindings.
+uses the dnf python bindings.
 
 
 ## License
 
 This project follows the REUSE specification. In general:
 
 - Code is licensed under GPL-2.0-or-later. This is the same license as dnf.
 - Configuration and repo files in fedrq/data/ are `UNLICENSE`ed
 - fedrq.spec is licensed under MIT to match Fedora
 - The embedded repo defs in src/fedrq/data/repos from fedora-repos.rpm are MIT
   licensed.
   These are only used when the needed repo defs are not available in the system
-  config (i.e. for querying the Fedora repos from a non Fedora system).
+  config (i.e., for querying the Fedora repos from a non Fedora system).
 - `enum.StrEnum` is copied from Cpython 3.11 for older Python versions. It's
   ~30 lines of PSF-2.0 licensed code.
 
 ```
 SPDX-License-Identifier: GPL-2.0-or-later AND Unlicense AND MIT AND PSF-2.0
 ```
```

### Comparing `fedrq-0.9.0/contrib/add_frag.py` & `fedrq-1.0.0/contrib/add_frag.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/contrib/api_examples/a_noarch_bash.py` & `fedrq-1.0.0/contrib/api_examples/a_noarch_bash.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/contrib/api_examples/ftbfs_retirements.py` & `fedrq-1.0.0/contrib/api_examples/ftbfs_retirements.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/contrib/container/Containerfile` & `fedrq-1.0.0/contrib/container/Containerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 ARG IMAGE=registry.fedoraproject.org/fedora:latest
 
 FROM ${IMAGE}
 
 RUN set -euo pipefail ;\
     dnf-3 install --disablerepo=\*-modular --disablerepo=fedora-cisco-openh264 -y \
         dnf-plugins-core ;\
     dnf-3 copr enable -y gotmax23/fedrq ;\
     dnf-3 install --disablerepo=\*-modular --disablerepo=fedora-cisco-openh264 -y \
         fedrq ;\
     dnf-3 clean all ;
 
-ENV XDG_CACHE_DIR=/fedrq-cache
+COPY 000-container.toml /etc/fedrq/000-container.toml
+
+RUN fedrq check-config
+
+ENV XDG_CACHE_HOME=/fedrq-cache
 ENTRYPOINT ["/usr/bin/fedrq"]
 CMD ["--help"]
 VOLUME /fedrq-cache
```

### Comparing `fedrq-0.9.0/contrib/container/Containerfile.rhel` & `fedrq-1.0.0/contrib/container/Containerfile.rhel`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 ARG IMAGE=registry.access.redhat.com/ubi9
 
 FROM ${IMAGE}
 
 RUN set -euo pipefail ;\
     dnf-3 install -y \
         dnf-plugins-core \
         https://dl.fedoraproject.org/pub/epel/epel-release-latest-$(rpm -E %rhel).noarch.rpm ;\
     dnf-3 copr enable -y gotmax23/fedrq ;\
     dnf-3 install -y \
         fedrq ;\
     dnf-3 clean all ;
 
+COPY 000-container.toml /etc/fedrq/000-container.toml
 COPY rhel.toml /etc/fedrq/rhel.toml
 
 RUN fedrq check-config
 
-ENV XDG_CACHE_DIR=/fedrq-cache
-ENTRYPOINT ["/usr/bin/fedrq"]
+COPY entrypoint.sh /usr/local/bin/entrypoint.sh
+
+ENV XDG_CACHE_HOME=/fedrq-cache
+ENTRYPOINT ["/usr/local/bin/entrypoint.sh", "/usr/bin/fedrq"]
 CMD ["--help"]
 VOLUME /fedrq-cache
```

### Comparing `fedrq-0.9.0/contrib/container/build.yml` & `fedrq-1.0.0/contrib/container/build.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/contrib/deploy-docsite/main.yaml` & `fedrq-1.0.0/contrib/deploy-docsite/main.yaml`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/contrib/deploy-docsite/roles/configure/tasks/main.yml` & `fedrq-1.0.0/contrib/deploy-docsite/roles/configure/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/contrib/fedoraify.py` & `fedrq-1.0.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/doc/API/Summary.md` & `fedrq-1.0.0/doc/API/Summary.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,91 +2,97 @@
 SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
 SPDX-License-Identifier: GPL-2.0-or-later
 -->
 
 # fedrq's Python API
 
 The `fedrq.config` module and the `fedrq.backend` package are public API.
-Everything under `fedrq.cli` is internal. fedrq is a primarily a CLI tool and
-its API abstracts the specific dnf/libdnf5 functionality that it uses. Its main
-purpose is repoquerying, but you can use the fedrq functionality you want and
-then access the underlying dnf Base object to preform other tasks if needed.
+Everything under `fedrq.cli` is internal. fedrq is primarily a CLI tool and
+its API only abstracts the specific dnf/libdnf5 functionality that the CLI uses. The
+API's main purpose is "repoquerying", but you can use the fedrq functionality
+you'd like and then access the underlying dnf Base object to preform other
+tasks if needed.
 
 Take a look at the docstrings for more information.
 
 Note that fedrq is still in beta and its API may be subject to breaking
 changes.
 
 ## fedrq.backends
 
-This is the heart of fedrq's API. There is a dnf backend (`fedrq.backends.dnf`)
-and a libdnf5 backend (`fedrq.backends.libdnf5`). This package provides an
-interface to configure a Base session, load repositories, preform queries, and
-related functionality. The main primitives are:
+`fedrq.backends` is the heart of fedrq's API.
+There is a dnf backend (`fedrq.backends.dnf`)
+and a libdnf5 backend (`fedrq.backends.libdnf5`).
+This package provides an interface to configure a Base session, load
+repositories, preform queries, and related functionality.
+The main primitives are:
 
 ### BaseMaker
 
 **Base class**: [`fedrq.backends.base.BaseMakerBase`][fedrq.backends.base.BaseMakerBase]
 
 **dnf backend:** [`fedrq.backends.dnf.backend.BaseMaker`][fedrq.backends.dnf.backend.BaseMaker]
 
 **libdnf5 backend:** [`fedrq.backends.libdnf5.backend.BaseMaker`][fedrq.backends.libdnf5.backend.BaseMaker]
 
-`BaseMaker` allows configuring a dnf Base session and loading repositories.
+`BaseMaker` allows configuring a dnf `Base` session and loading repositories.
 
 ### Repoquery
 
 **Base class**: [`fedrq.backends.base.RepoqueryBase`][fedrq.backends.base.RepoqueryBase]
 
 **dnf backend:** [`fedrq.backends.dnf.backend.Repoquery`][fedrq.backends.dnf.backend.Repoquery]
 
 **libdnf5 backend:** [`fedrq.backends.libdnf5.backend.Repoquery`][fedrq.backends.libdnf5.backend.Repoquery]
 
-`Repoquery` takes an initialized Base object (see `BaseMaker`) and allows
-preforming a large range of queries. Most of its methods return
+`Repoquery` accepts an initialized Base object (see `BaseMaker`) and allows
+performing a large range of queries. Most of its methods return
 `PackageQueryCompat` or `PackageCompat` objects.
 
 
 ### PackageQueryCompat
 
 **Protocol:** [`fedrq.backends.base.PackageQueryCompat`][fedrq.backends.base.PackageQueryCompat]
 
-**dnf backend:** [`fedrq.backends.dnf.backend.PackageQuery`][fedrq.backends.dnf.backend.PackageQuery] -> `hawkey.Query`
+**dnf backend:** [`fedrq.backends.dnf.backend.PackageQuery`][fedrq.backends.dnf.backend.PackageQuery] -> [`hawkey.Query`][dnf.query.Query]
 
-**libdnf5 backend:** [`fedrq.backends.libdnf5.backend.Package`](fedrq.backends.libdnf5.backend.Package)
-(`libdnf5.package.Package` subclass)
+**libdnf5 backend:** [`fedrq.backends.libdnf5.backend.PackageQuery`][fedrq.backends.libdnf5.backend.PackageQuery]
+([`libdnf5.rpm.PackageQuery`][libdnf5.rpm.PackageQuery] subclass)
 
-PackageQueryCompat is a set like object of PackageCompat objects. It contains
-methods to filter its Packages based on certain criteria. Typically, you'd
-access these through the Repoquery class.
+`PackageQueryCompat` is a set-like object of `PackageCompat` objects. It contains
+methods to filter its Packages based on certain criteria. Typically, you would
+access the filtering methods through the `Repoquery` class's wrappers.
 
-- `fedrq.backends.libdnf5.backend.PackageQuery` - subclass of
+- `fedrq.backends.libdnf5.backend.PackageQuery` --- subclass of
   `libdnf5.rpm.PackageQuery`. adds back missing `query` and `querym` methods.
 
 
 ### PackageCompat
 
 
 **Protocol:** [`fedrq.backends.base.PackageCompat`][fedrq.backends.base.PackageCompat]
 
-**dnf backend:** [`fedrq.backends.dnf.backend.Package`][fedrq.backends.dnf.backend.Package] -> `dnf.package.Package`
+**dnf backend:** [`fedrq.backends.dnf.backend.Package`][fedrq.backends.dnf.backend.Package] -> [`dnf.package.Package`][dnf.package.Package]
 
 **libdnf5 backend:** [`fedrq.backends.libdnf5.backend.Package`][fedrq.backends.libdnf5.backend.Package]
-(`libdnf5.package.Package` subclass)
+([`libdnf5.rpm.Package`][libdnf5.rpm.Package] subclass)
 
-- `fedrq.backends.libdnf5.backend.Package` - subclass of `libdnf5.rpm.Package`
-  that implements missing functionality and compatability with
-  `dnf.package.Package`. includes properties to access Package attributes.
+- [`fedrq.backends.libdnf5.backend.Package`][fedrq.backends.libdnf5.backend.Package] ---
+  subclass of [`libdnf5.rpm.Package`][libdnf5.rpm.Package]
+  that implements missing functionality and compatibility with
+  [`dnf.package.Package`][dnf.package.Package].
+  The subclass includes properties to access Package attributes.
   These properties were removed from libdnf5 in favor of `get_foo()` methods.
   It also includes rich comparison support (`__lt__`, `__gt__`, etc.) and
   implements roughly the same sort order as the dnf backend and adds a
-  `__hash__()` method so it can e.g. be used in a set or as a dictionary key.
+  `__hash__()` method so it can e.g., be used in a set or as a dictionary key.
 
-    Importing `fedrq.backends.libdnf5.backend` registers the `Package` subclass
-    so PackageQuery contains our subclass.
+    Importing
+    [`fedrq.backends.libdnf5.backend`][fedrq.backends.libdnf5.backend]
+    registers the `Package` subclass so PackageQuery contains our subclass.
 
 ## [`fedrq.config`][fedrq.config]
 
 Most of the code here should not be called directly. Use `get_config()` to load
 the configuration from the filesystem. Create an `RQConfig` object manually if
 you must.
```

### Comparing `fedrq-0.9.0/doc/API/backends/libdnf5.md` & `fedrq-1.0.0/doc/API/backends/libdnf5.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/doc/dnf-repoquery-diff.md` & `fedrq-1.0.0/doc/dnf-repoquery-diff.md`

 * *Files 23% similar despite different names*

```diff
@@ -8,201 +8,259 @@
 00000070: 7320 6265 7477 6565 6e20 6665 6472 7120  s between fedrq 
 00000080: 616e 6420 646e 6620 7265 706f 7175 6572  and dnf repoquer
 00000090: 790a 0a57 6869 6c65 2066 6564 7271 2061  y..While fedrq a
 000000a0: 6e64 2060 646e 6620 7265 706f 7175 6572  nd `dnf repoquer
 000000b0: 7960 2068 6176 6520 7369 6d69 6c61 7220  y` have similar 
 000000c0: 6675 6e63 7469 6f6e 616c 6974 792c 0a74  functionality,.t
 000000d0: 6865 6972 2072 6573 7065 6374 6976 6520  heir respective 
-000000e0: 696e 7465 7266 6163 6573 2068 6176 6520  interfaces have 
-000000f0: 736f 6d65 206b 6579 2064 6966 6665 7265  some key differe
-00000100: 6e63 6573 2e0a 5468 6520 6175 7468 6f72  nces..The author
-00000110: 2062 656c 6965 7665 7320 7468 6573 6520   believes these 
-00000120: 6469 6666 6572 656e 6365 7320 6d61 6b65  differences make
-00000130: 2066 6564 7271 206d 6f72 6520 706f 7765   fedrq more powe
-00000140: 7266 756c 2061 6e64 206d 6f72 6520 7573  rful and more us
-00000150: 6572 0a66 7269 656e 646c 792c 2062 7574  er.friendly, but
-00000160: 2065 7870 6572 6965 6e63 6564 2060 646e   experienced `dn
-00000170: 6620 7265 706f 7175 6572 7960 2075 7365  f repoquery` use
-00000180: 7273 2073 686f 756c 6420 6b65 6570 2074  rs should keep t
-00000190: 6865 6d20 696e 206d 696e 642e 0a0a 2323  hem in mind...##
-000001a0: 2044 6566 6175 6c74 2072 6570 6f73 6974   Default reposit
-000001b0: 6f72 6965 730a 0a42 7920 6465 6661 756c  ories..By defaul
-000001c0: 742c 2060 646e 6620 7265 706f 7175 6572  t, `dnf repoquer
-000001d0: 7960 2072 6561 6473 2074 6865 2073 7973  y` reads the sys
-000001e0: 7465 6d20 636f 6e66 6967 7572 6174 696f  tem configuratio
-000001f0: 6e20 616e 6420 7175 6572 6965 7320 7468  n and queries th
-00000200: 650a 7265 706f 7369 746f 7269 6573 2077  e.repositories w
-00000210: 6974 6820 6065 6e61 626c 6564 3d31 6020  ith `enabled=1` 
-00000220: 616e 6420 6e6f 7468 696e 6720 6d6f 7265  and nothing more
-00000230: 2e0a 6665 6472 712c 206f 6e20 7468 6520  ..fedrq, on the 
-00000240: 6f74 6865 7220 6861 6e64 2c20 6265 6861  other hand, beha
-00000250: 7665 7320 6d6f 7265 206c 696b 6520 6066  ves more like `f
-00000260: 6564 706b 6760 2e0a 5175 6572 6965 7320  edpkg`..Queries 
-00000270: 6465 6661 756c 7420 746f 2060 7261 7768  default to `rawh
-00000280: 6964 6560 2061 6e64 2065 6e61 626c 6520  ide` and enable 
-00000290: 7468 6520 6072 6177 6869 6465 6020 616e  the `rawhide` an
-000002a0: 6420 6072 6177 6869 6465 2d73 6f75 7263  d `rawhide-sourc
-000002b0: 6560 0a72 6570 6f73 6974 6f72 6965 732e  e`.repositories.
-000002c0: 0a54 6869 7320 6361 6e20 6265 2063 6861  .This can be cha
-000002d0: 6e67 6564 2075 7369 6e67 2074 6865 2060  nged using the `
-000002e0: 2d62 6020 2f20 602d 2d62 7261 6e63 6860  -b` / `--branch`
-000002f0: 2066 6c61 6773 206f 6e20 7468 6520 434c   flags on the CL
-00000300: 4920 6f72 2070 6572 6d61 6e65 6e74 6c79  I or permanently
-00000310: 0a77 6974 6820 7468 6520 6064 6566 6175  .with the `defau
-00000320: 6c74 5f62 7261 6e63 6860 206f 7074 696f  lt_branch` optio
-00000330: 6e20 696e 2074 6865 2063 6f6e 6669 6775  n in the configu
-00000340: 7261 7469 6f6e 2e0a 5365 6520 7468 6520  ration..See the 
-00000350: 5b42 5549 4c54 494e 2052 454c 4541 5345  [BUILTIN RELEASE
-00000360: 535d 282e 2e2f 6665 6472 7131 2f23 6275  S](../fedrq1/#bu
-00000370: 696c 7469 6e2d 7265 6c65 6173 6573 2920  iltin-releases) 
-00000380: 7365 6374 696f 6e20 6f66 2060 6d61 6e20  section of `man 
-00000390: 6665 6472 7160 0a66 6f72 2076 616c 6964  fedrq`.for valid
-000003a0: 2060 2d2d 6272 616e 6368 6020 6f70 7469   `--branch` opti
-000003b0: 6f6e 732e 0a55 7365 7273 2063 616e 206f  ons..Users can o
-000003c0: 6620 636f 7572 7365 2063 6f6e 6669 6775  f course configu
-000003d0: 7265 2074 6865 6972 206f 776e 2063 7573  re their own cus
-000003e0: 746f 6d20 7265 6c65 6173 6520 7072 6f66  tom release prof
-000003f0: 696c 6573 2e0a 596f 7520 6361 6e20 7573  iles..You can us
-00000400: 6520 7468 6520 7073 6575 646f 2060 2d62  e the pseudo `-b
-00000410: 206c 6f63 616c 6020 7265 6c65 6173 6520   local` release 
-00000420: 7768 6963 6820 7573 6573 2074 6865 2064  which uses the d
-00000430: 6566 6175 6c74 2072 6570 6f73 6974 6f72  efault repositor
-00000440: 6965 730a 7769 7468 2060 656e 6162 6c65  ies.with `enable
-00000450: 643d 3160 2069 6e20 2f65 7463 2f79 756d  d=1` in /etc/yum
-00000460: 2e72 6570 6f73 2e64 2061 6e64 2074 6865  .repos.d and the
-00000470: 2073 7973 7465 6d27 7320 7265 6c65 6173   system's releas
-00000480: 6576 6572 2e0a 0a23 2320 536f 7572 6365  ever...## Source
-00000490: 2072 6570 6f73 6974 6f72 6965 730a 0a66   repositories..f
-000004a0: 6564 7271 2065 6e61 626c 6573 2073 6f75  edrq enables sou
-000004b0: 7263 6520 7265 706f 7369 746f 7269 6573  rce repositories
-000004c0: 2062 7920 6465 6661 756c 7420 696e 2069   by default in i
-000004d0: 7473 2062 7569 6c74 696e 2072 656c 6561  ts builtin relea
-000004e0: 7365 2063 6f6e 6669 6773 2e0a 5768 696c  se configs..Whil
-000004f0: 6520 7573 6572 7320 6172 6520 6672 6565  e users are free
-00000500: 2074 6f20 696e 636c 7564 6520 7768 6963   to include whic
-00000510: 6865 7665 7220 7265 706f 7369 746f 7269  hever repositori
-00000520: 6573 2074 6865 7920 7769 7368 2069 6e20  es they wish in 
-00000530: 7468 6569 7220 6c6f 6361 6c0a 636f 6e66  their local.conf
-00000540: 6967 7572 6174 696f 6e73 2c0a 636f 6d6d  igurations,.comm
-00000550: 616e 6473 2073 7563 6820 6173 2060 6665  ands such as `fe
-00000560: 6472 7120 7375 6270 6b67 7360 2061 6e64  drq subpkgs` and
-00000570: 2060 6665 6472 7120 7768 6174 7265 7175   `fedrq whatrequ
-00000580: 6972 6573 2d73 7263 6020 7769 6c6c 206e  ires-src` will n
-00000590: 6f74 2077 6f72 6b0a 7072 6f70 6572 6c79  ot work.properly
-000005a0: 2077 6974 686f 7574 2073 6f75 7263 6520   without source 
-000005b0: 7265 706f 7369 746f 7269 6573 2065 6e61  repositories ena
-000005c0: 626c 6564 2e0a 0a23 2320 5265 6c65 6173  bled...## Releas
-000005d0: 6520 636f 6e66 6967 7572 6174 696f 6e73  e configurations
-000005e0: 0a0a 5265 6c65 6173 6520 636f 6e66 6967  ..Release config
-000005f0: 7572 6174 696f 6e73 2063 6f6e 7461 696e  urations contain
-00000600: 2074 6872 6565 206d 6169 6e20 7061 7274   three main part
-00000610: 733a 0a0a 2d20 6076 6572 7369 6f6e 6020  s:..- `version` 
-00000620: 2d20 7468 6973 2069 7320 6120 7265 6765  - this is a rege
-00000630: 7820 6f66 206d 6174 6368 696e 6720 6272  x of matching br
-00000640: 616e 6368 6573 2e20 466f 7220 6578 616d  anches. For exam
-00000650: 706c 652c 2074 6865 2072 6570 6f73 6974  ple, the reposit
-00000660: 6f72 790a 2020 6465 6669 6e69 7469 6f6e  ory.  definition
-00000670: 2066 6f72 2074 6865 2046 6564 6f72 6120   for the Fedora 
-00000680: 6272 616e 6368 6573 2063 6f6e 6669 6775  branches configu
-00000690: 7261 7469 6f6e 2069 7320 605e 6628 5c64  ration is `^f(\d
-000006a0: 7b32 7d29 2460 2e20 5468 6572 6566 6f72  {2})$`. Therefor
-000006b0: 652c 0a20 2060 2d2d 6272 616e 6368 2066  e,.  `--branch f
-000006c0: 3337 6020 616e 6420 602d 2d62 7261 6e63  37` and `--branc
-000006d0: 6820 6633 3660 2077 696c 6c20 6d61 7463  h f36` will matc
-000006e0: 6820 7468 6973 2063 6f6e 6669 6775 7261  h this configura
-000006f0: 7469 6f6e 2061 6e64 2074 6865 0a20 2060  tion and the.  `
-00000700: 2472 656c 6561 7365 7665 7260 2077 696c  $releasever` wil
-00000710: 6c0a 2020 6265 2073 6574 2074 6f20 6033  l.  be set to `3
-00000720: 3760 2061 6e64 2060 3336 602c 2072 6573  7` and `36`, res
-00000730: 7065 6374 6976 656c 792e 0a2d 2060 6465  pectively..- `de
-00000740: 6673 6020 2d20 7468 6973 2069 7320 6120  fs` - this is a 
-00000750: 6d61 7070 696e 6720 6f66 2070 726f 6669  mapping of profi
-00000760: 6c65 206e 616d 6573 2074 6f20 6120 6c69  le names to a li
-00000770: 7374 206f 6620 7265 706f 7369 746f 7279  st of repository
-00000780: 2049 4473 2e20 4561 6368 0a20 2072 656c   IDs. Each.  rel
-00000790: 6561 7365 2068 6173 2061 2060 6261 7365  ease has a `base
-000007a0: 6020 7072 6f66 696c 6520 7768 6963 6820  ` profile which 
-000007b0: 6973 2074 6865 2064 6566 6175 6c74 2070  is the default p
-000007c0: 726f 6669 6c65 2066 6f72 2074 6861 7420  rofile for that 
-000007d0: 7265 6c65 6173 652e 0a20 204f 7468 6572  release..  Other
-000007e0: 7320 6361 6e20 6265 2073 656c 6563 7465  s can be selecte
-000007f0: 6420 7769 7468 2060 2d72 6020 2f20 602d  d with `-r` / `-
-00000800: 2d72 6570 6f60 2e0a 0a66 6564 7271 2063  -repo`...fedrq c
-00000810: 616e 2072 6561 6420 636f 6e66 6967 7572  an read configur
-00000820: 6174 696f 6e20 6672 6f6d 202e 7265 706f  ation from .repo
-00000830: 2066 696c 6573 206c 6f63 6174 6564 206f   files located o
-00000840: 7574 7369 6465 206f 660a 602f 6574 632f  utside of.`/etc/
-00000850: 7975 6d2e 7265 706f 732e 642f 6020 6966  yum.repos.d/` if
-00000860: 2074 6865 7927 7265 2073 7065 6369 6669   they're specifi
-00000870: 6564 2069 6e20 7468 6520 7265 6c65 6173  ed in the releas
-00000880: 6527 7320 6064 6566 7061 7468 7360 2e0a  e's `defpaths`..
-00000890: 0a54 6865 2063 6f6e 6669 6775 7261 7469  .The configurati
-000008a0: 6f6e 2073 796e 7461 7820 6973 2064 6573  on syntax is des
-000008b0: 6372 6962 6564 206d 6f72 6520 696e 205b  cribed more in [
-000008c0: 606d 616e 2035 2066 6564 7271 605d 282e  `man 5 fedrq`](.
-000008d0: 2e2f 6665 6472 7135 292e 0a0a 2323 202d  ./fedrq5)...## -
-000008e0: 2d6c 6174 6573 740a 0a60 6665 6472 7160  -latest..`fedrq`
-000008f0: 2061 7070 6c69 6573 2060 2d2d 6c61 7465   applies `--late
-00000900: 7374 3d31 6020 6279 2064 6566 6175 6c74  st=1` by default
-00000910: 2e20 5468 6973 206d 6561 6e73 2074 6861  . This means tha
-00000920: 7420 6f6e 6c79 206f 6e65 2070 6163 6b61  t only one packa
-00000930: 6765 0a76 6572 7369 6f6e 2077 696c 6c20  ge.version will 
-00000940: 6265 2073 686f 776e 2066 6f72 2065 6163  be shown for eac
-00000950: 6820 6172 6368 6974 6563 7475 7265 2e20  h architecture. 
-00000960: 6064 6e66 2072 6570 6f71 7565 7279 602c  `dnf repoquery`,
-00000970: 206f 6e20 7468 6520 6f74 6865 720a 6861   on the other.ha
-00000980: 6e64 2c20 7368 6f77 7320 6576 6572 7974  nd, shows everyt
-00000990: 6869 6e67 2e20 596f 7520 6361 6e20 7061  hing. You can pa
-000009a0: 7373 2060 2d2d 6c61 7465 7374 3d61 6c6c  ss `--latest=all
-000009b0: 6020 746f 2066 6564 7271 2074 6f20 6368  ` to fedrq to ch
-000009c0: 616e 6765 2074 6869 730a 6265 6861 7669  ange this.behavi
-000009d0: 6f72 2e0a 0a23 2320 2d2d 7265 706f 2061  or...## --repo a
-000009e0: 6e64 202d 2d65 6e61 626c 6572 6570 6f0a  nd --enablerepo.
-000009f0: 0a66 6564 7271 2061 6c73 6f20 7375 7070  .fedrq also supp
-00000a00: 6f72 7473 2074 6865 7365 206f 7074 696f  orts these optio
-00000a10: 6e73 2c20 6275 7420 7468 6579 2068 6176  ns, but they hav
-00000a20: 6520 6164 6469 7469 6f6e 616c 2066 756e  e additional fun
-00000a30: 6374 696f 6e61 6c69 7479 2e0a 496e 2061  ctionality..In a
-00000a40: 6464 6974 696f 6e20 6072 6570 6f69 6460  ddition `repoid`
-00000a50: 732c 2074 6865 7365 206f 7074 696f 6e73  s, these options
-00000a60: 2061 6363 6570 7420 7265 6c65 6173 652d   accept release-
-00000a70: 7370 6563 6966 6963 2067 726f 7570 206e  specific group n
-00000a80: 616d 6573 2028 7468 6573 650a 6172 6520  ames (these.are 
-00000a90: 636f 6e66 6967 7572 6564 2069 6e20 6120  configured in a 
-00000aa0: 7265 6c65 6173 6527 7320 6064 6566 7360  release's `defs`
-00000ab0: 2061 7320 6578 706c 6169 6e65 6420 6162   as explained ab
-00000ac0: 6f76 6529 2c20 616e 6420 6765 6e65 7269  ove), and generi
-00000ad0: 6320 7265 706f 0a63 6c61 7373 6573 2e0a  c repo.classes..
-00000ae0: 0a46 6f72 2065 7861 6d70 6c65 2c20 796f  .For example, yo
-00000af0: 7520 6361 6e20 7061 7373 2060 2d62 2066  u can pass `-b f
-00000b00: 3337 202d 7220 4063 6f70 723a 676f 746d  37 -r @copr:gotm
-00000b10: 6178 3233 2f66 6564 7271 6020 746f 2071  ax23/fedrq` to q
-00000b20: 7565 7279 202a 6f6e 6c79 2a20 7468 650a  uery *only* the.
-00000b30: 6066 6564 6f72 612d 3337 6020 6368 726f  `fedora-37` chro
-00000b40: 6f74 2773 2072 6570 6f73 6974 6f72 6965  ot's repositorie
-00000b50: 732e 2059 6f75 2063 616e 2070 6173 7320  s. You can pass 
-00000b60: 602d 6220 6633 3720 2d2d 656e 6162 6c65  `-b f37 --enable
-00000b70: 7265 706f 0a40 636f 7072 3a67 6f74 6d61  repo.@copr:gotma
-00000b80: 7832 332f 6665 6472 7160 2069 6620 796f  x23/fedrq` if yo
-00000b90: 7520 7761 6e74 2074 6f20 656e 6162 6c65  u want to enable
-00000ba0: 2074 6861 7420 636f 7072 2773 2072 6570   that copr's rep
-00000bb0: 6f73 6974 6f72 7920 6f6e 2074 6f70 206f  ository on top o
-00000bc0: 660a 7468 6520 6261 7365 2072 6570 6f73  f.the base repos
-00000bd0: 6974 6f72 6965 732e 0a0a 5365 6520 7468  itories...See th
-00000be0: 6520 5b52 4550 4f20 434c 4153 5345 535d  e [REPO CLASSES]
-00000bf0: 282e 2e2f 6665 6472 7131 2f23 7265 706f  (../fedrq1/#repo
-00000c00: 2d63 6c61 7373 6573 2920 7365 6374 696f  -classes) sectio
-00000c10: 6e20 6f66 2060 6d61 6e20 6665 6472 7160  n of `man fedrq`
-00000c20: 2066 6f72 206d 6f72 650a 696e 666f 726d   for more.inform
-00000c30: 6174 696f 6e2e 0a0a 2323 2053 7562 636f  ation...## Subco
-00000c40: 6d6d 616e 6473 0a0a 6665 6472 7127 7320  mmands..fedrq's 
-00000c50: 434c 4920 696e 7465 7266 6163 6520 6973  CLI interface is
-00000c60: 2073 706c 6974 2069 6e74 6f20 7375 6263   split into subc
-00000c70: 6f6d 6d61 6e64 7320 756e 6c69 6b65 2060  ommands unlike `
-00000c80: 646e 6620 7265 706f 7175 6572 7960 2077  dnf repoquery` w
-00000c90: 6869 6368 0a72 656c 6965 7320 6f6e 2066  hich.relies on f
-00000ca0: 6c61 6773 2e0a 0a53 6565 205b 606d 616e  lags...See [`man
-00000cb0: 2066 6564 7271 605d 282e 2e2f 6665 6472   fedrq`](../fedr
-00000cc0: 7131 2920 666f 7220 616e 2069 6e20 6465  q1) for an in de
-00000cd0: 7074 6820 6f72 6965 6e74 6174 696f 6e20  pth orientation 
-00000ce0: 6f66 2066 6564 7271 2773 2043 4c49 0a69  of fedrq's CLI.i
-00000cf0: 6e74 6572 6661 6365 2e0a                 nterface..
+000000e0: 696e 7465 7266 6163 6573 2070 6f73 7365  interfaces posse
+000000f0: 7373 2073 6f6d 6520 6b65 7920 6469 6666  ss some key diff
+00000100: 6572 656e 6365 732e 0a54 6865 2061 7574  erences..The aut
+00000110: 686f 7220 6265 6c69 6576 6573 2074 6865  hor believes the
+00000120: 7365 2064 6966 6665 7265 6e63 6573 206d  se differences m
+00000130: 616b 6520 6665 6472 7120 6d6f 7265 2070  ake fedrq more p
+00000140: 6f77 6572 6675 6c20 616e 6420 7573 6572  owerful and user
+00000150: 0a66 7269 656e 646c 792c 2062 7574 2065  .friendly, but e
+00000160: 7870 6572 6965 6e63 6564 2060 646e 6620  xperienced `dnf 
+00000170: 7265 706f 7175 6572 7960 2075 7365 7273  repoquery` users
+00000180: 2073 686f 756c 6420 6b65 6570 2074 6865   should keep the
+00000190: 6d20 696e 206d 696e 642e 0a0a 2323 2044  m in mind...## D
+000001a0: 6566 6175 6c74 2072 6570 6f73 6974 6f72  efault repositor
+000001b0: 6965 730a 0a42 7920 6465 6661 756c 742c  ies..By default,
+000001c0: 2060 646e 6620 7265 706f 7175 6572 7960   `dnf repoquery`
+000001d0: 2072 6561 6473 2074 6865 2073 7973 7465   reads the syste
+000001e0: 6d20 636f 6e66 6967 7572 6174 696f 6e20  m configuration 
+000001f0: 616e 6420 7175 6572 6965 7320 7468 650a  and queries the.
+00000200: 7265 706f 7369 746f 7269 6573 2077 6974  repositories wit
+00000210: 6820 6065 6e61 626c 6564 3d31 6020 696e  h `enabled=1` in
+00000220: 2074 6865 6972 2063 6f6e 6669 6775 7261   their configura
+00000230: 7469 6f6e 7320 2d2d 2d20 616e 6420 6e6f  tions --- and no
+00000240: 7468 696e 6720 6d6f 7265 2e0a 6665 6472  thing more..fedr
+00000250: 712c 206f 6e20 7468 6520 6f74 6865 7220  q, on the other 
+00000260: 6861 6e64 2c20 6265 6861 7665 7320 6d6f  hand, behaves mo
+00000270: 7265 206c 696b 6520 6066 6564 706b 6760  re like `fedpkg`
+00000280: 2e0a 5175 6572 6965 7320 6465 6661 756c  ..Queries defaul
+00000290: 7420 746f 2060 7261 7768 6964 6560 2061  t to `rawhide` a
+000002a0: 6e64 2065 6e61 626c 6520 7468 6520 6072  nd enable the `r
+000002b0: 6177 6869 6465 6020 616e 6420 6072 6177  awhide` and `raw
+000002c0: 6869 6465 2d73 6f75 7263 6560 0a72 6570  hide-source`.rep
+000002d0: 6f73 6974 6f72 6965 732e 0a54 6869 7320  ositories..This 
+000002e0: 6361 6e20 6265 2063 6861 6e67 6564 2075  can be changed u
+000002f0: 7369 6e67 2074 6865 2060 2d62 6020 2f20  sing the `-b` / 
+00000300: 602d 2d62 7261 6e63 6860 2066 6c61 6773  `--branch` flags
+00000310: 206f 6e20 7468 6520 434c 4920 6f72 2070   on the CLI or p
+00000320: 6572 6d61 6e65 6e74 6c79 0a63 6861 6e67  ermanently.chang
+00000330: 6564 2077 6974 6820 7468 6520 6064 6566  ed with the `def
+00000340: 6175 6c74 5f62 7261 6e63 6860 206f 7074  ault_branch` opt
+00000350: 696f 6e20 696e 2074 6865 2063 6f6e 6669  ion in the confi
+00000360: 6775 7261 7469 6f6e 2e0a 5365 6520 7468  guration..See th
+00000370: 6520 5b42 5549 4c54 494e 2052 454c 4541  e [BUILTIN RELEA
+00000380: 5345 535d 2866 6564 7271 312e 6d64 2f23  SES](fedrq1.md/#
+00000390: 6275 696c 7469 6e2d 7265 6c65 6173 6573  builtin-releases
+000003a0: 2920 7365 6374 696f 6e20 6f66 2060 6d61  ) section of `ma
+000003b0: 6e20 6665 6472 7160 0a66 6f72 2076 616c  n fedrq`.for val
+000003c0: 6964 2060 2d2d 6272 616e 6368 6020 6f70  id `--branch` op
+000003d0: 7469 6f6e 732e 0a55 7365 7273 2063 616e  tions..Users can
+000003e0: 206f 6620 636f 7572 7365 2063 6f6e 6669   of course confi
+000003f0: 6775 7265 2074 6865 6972 206f 776e 2063  gure their own c
+00000400: 7573 746f 6d20 7265 6c65 6173 6520 7072  ustom release pr
+00000410: 6f66 696c 6573 2e0a 5573 6520 7468 6520  ofiles..Use the 
+00000420: 7073 6575 646f 2060 2d62 206c 6f63 616c  pseudo `-b local
+00000430: 6020 7265 6c65 6173 6520 7768 6963 6820  ` release which 
+00000440: 696e 636c 7564 6573 2074 6865 2064 6566  includes the def
+00000450: 6175 6c74 2072 6570 6f73 6974 6f72 6965  ault repositorie
+00000460: 730a 7769 7468 2060 656e 6162 6c65 643d  s.with `enabled=
+00000470: 3160 2069 6e20 2f65 7463 2f79 756d 2e72  1` in /etc/yum.r
+00000480: 6570 6f73 2e64 2061 6e64 2074 6865 2073  epos.d and the s
+00000490: 7973 7465 6d27 7320 7265 6c65 6173 6576  ystem's releasev
+000004a0: 6572 2e0a 0a23 2320 536f 7572 6365 2072  er...## Source r
+000004b0: 6570 6f73 6974 6f72 6965 730a 0a66 6564  epositories..fed
+000004c0: 7271 2065 6e61 626c 6573 2073 6f75 7263  rq enables sourc
+000004d0: 6520 7265 706f 7369 746f 7269 6573 2062  e repositories b
+000004e0: 7920 6465 6661 756c 7420 696e 2069 7473  y default in its
+000004f0: 2062 7569 6c74 696e 2072 656c 6561 7365   builtin release
+00000500: 2063 6f6e 6669 6773 2e0a 5768 696c 6520   configs..While 
+00000510: 7573 6572 7320 6172 6520 6672 6565 2074  users are free t
+00000520: 6f20 696e 636c 7564 6520 7768 6963 6865  o include whiche
+00000530: 7665 7220 7265 706f 7369 746f 7269 6573  ver repositories
+00000540: 2074 6865 7920 7769 7368 2069 6e20 7468   they wish in th
+00000550: 6569 7220 6c6f 6361 6c0a 636f 6e66 6967  eir local.config
+00000560: 7572 6174 696f 6e73 2c0a 636f 6d6d 616e  urations,.comman
+00000570: 6473 2073 7563 6820 6173 2060 6665 6472  ds such as `fedr
+00000580: 7120 7375 6270 6b67 7360 2061 6e64 2060  q subpkgs` and `
+00000590: 6665 6472 7120 7768 6174 7265 7175 6972  fedrq whatrequir
+000005a0: 6573 2d73 7263 6020 7769 6c6c 206e 6f74  es-src` will not
+000005b0: 2077 6f72 6b0a 7072 6f70 6572 6c79 2077   work.properly w
+000005c0: 6974 686f 7574 2073 6f75 7263 6520 7265  ithout source re
+000005d0: 706f 7369 746f 7269 6573 2065 6e61 626c  positories enabl
+000005e0: 6564 2e0a 0a23 2320 5265 6c65 6173 6520  ed...## Release 
+000005f0: 636f 6e66 6967 7572 6174 696f 6e73 0a0a  configurations..
+00000600: 5265 6c65 6173 6520 636f 6e66 6967 7572  Release configur
+00000610: 6174 696f 6e73 2063 6f6e 7461 696e 2074  ations contain t
+00000620: 6872 6565 206d 6169 6e20 7061 7274 733a  hree main parts:
+00000630: 0a0a 2d20 6076 6572 7369 6f6e 6020 2d2d  ..- `version` --
+00000640: 2d20 7468 6973 2069 7320 6120 7265 6765  - this is a rege
+00000650: 7820 6f66 206d 6174 6368 696e 6720 6272  x of matching br
+00000660: 616e 6368 6573 2e20 466f 7220 6578 616d  anches. For exam
+00000670: 706c 652c 2074 6865 2072 6570 6f73 6974  ple, the reposit
+00000680: 6f72 790a 2020 6465 6669 6e69 7469 6f6e  ory.  definition
+00000690: 2066 6f72 2074 6865 2046 6564 6f72 6120   for the Fedora 
+000006a0: 6272 616e 6368 6573 2063 6f6e 6669 6775  branches configu
+000006b0: 7261 7469 6f6e 2069 7320 605e 6628 5c64  ration is `^f(\d
+000006c0: 7b32 7d29 2460 2e20 5468 6572 6566 6f72  {2})$`. Therefor
+000006d0: 652c 0a20 2060 2d2d 6272 616e 6368 2066  e,.  `--branch f
+000006e0: 3337 6020 616e 6420 602d 2d62 7261 6e63  37` and `--branc
+000006f0: 6820 6633 3660 2077 696c 6c20 6d61 7463  h f36` will matc
+00000700: 6820 7468 6973 2063 6f6e 6669 6775 7261  h this configura
+00000710: 7469 6f6e 2061 6e64 2074 6865 0a20 2060  tion and the.  `
+00000720: 2472 656c 6561 7365 7665 7260 2077 696c  $releasever` wil
+00000730: 6c0a 2020 6265 2073 6574 2074 6f20 6033  l.  be set to `3
+00000740: 3760 2061 6e64 2060 3336 602c 2072 6573  7` and `36`, res
+00000750: 7065 6374 6976 656c 792e 0a2d 2060 6465  pectively..- `de
+00000760: 6673 6020 2d2d 2d20 7468 6973 2069 7320  fs` --- this is 
+00000770: 6120 6d61 7070 696e 6720 6f66 2070 726f  a mapping of pro
+00000780: 6669 6c65 206e 616d 6573 2074 6f20 6120  file names to a 
+00000790: 6c69 7374 206f 6620 7265 706f 7369 746f  list of reposito
+000007a0: 7279 2049 4473 2e20 4561 6368 0a20 2072  ry IDs. Each.  r
+000007b0: 656c 6561 7365 2068 6173 2061 2060 6261  elease has a `ba
+000007c0: 7365 6020 7072 6f66 696c 6520 7768 6963  se` profile whic
+000007d0: 6820 6973 2074 6865 2064 6566 6175 6c74  h is the default
+000007e0: 2070 726f 6669 6c65 2066 6f72 2074 6861   profile for tha
+000007f0: 7420 7265 6c65 6173 652e 0a20 204f 7468  t release..  Oth
+00000800: 6572 7320 6361 6e20 6265 2073 656c 6563  ers can be selec
+00000810: 7465 6420 7769 7468 2060 2d72 6020 2f20  ted with `-r` / 
+00000820: 602d 2d72 6570 6f60 2e0a 0a66 6564 7271  `--repo`...fedrq
+00000830: 2063 616e 2072 6561 6420 636f 6e66 6967   can read config
+00000840: 7572 6174 696f 6e20 6672 6f6d 202e 7265  uration from .re
+00000850: 706f 2066 696c 6573 206c 6f63 6174 6564  po files located
+00000860: 206f 7574 7369 6465 206f 660a 602f 6574   outside of.`/et
+00000870: 632f 7975 6d2e 7265 706f 732e 642f 6020  c/yum.repos.d/` 
+00000880: 6966 2074 6865 7927 7265 2073 7065 6369  if they're speci
+00000890: 6669 6564 2069 6e20 7468 6520 7265 6c65  fied in the rele
+000008a0: 6173 6527 7320 6064 6566 7061 7468 7360  ase's `defpaths`
+000008b0: 2e0a 0a54 6865 2063 6f6e 6669 6775 7261  ...The configura
+000008c0: 7469 6f6e 2073 796e 7461 7820 6973 2064  tion syntax is d
+000008d0: 6573 6372 6962 6564 206d 6f72 6520 696e  escribed more in
+000008e0: 205b 606d 616e 2035 2066 6564 7271 605d   [`man 5 fedrq`]
+000008f0: 2866 6564 7271 352e 6d64 292e 0a0a 2323  (fedrq5.md)...##
+00000900: 2060 2d2d 6c61 7465 7374 600a 0a60 6665   `--latest`..`fe
+00000910: 6472 7160 2061 7070 6c69 6573 2060 2d2d  drq` applies `--
+00000920: 6c61 7465 7374 3d31 6020 6279 2064 6566  latest=1` by def
+00000930: 6175 6c74 2e20 5468 6973 206d 6561 6e73  ault. This means
+00000940: 2074 6861 7420 6f6e 6c79 206f 6e65 2070   that only one p
+00000950: 6163 6b61 6765 0a76 6572 7369 6f6e 2077  ackage.version w
+00000960: 696c 6c20 6265 2073 686f 776e 2066 6f72  ill be shown for
+00000970: 2065 6163 6820 6172 6368 6974 6563 7475   each architectu
+00000980: 7265 2e20 6064 6e66 2072 6570 6f71 7565  re. `dnf repoque
+00000990: 7279 602c 206f 6e20 7468 6520 6f74 6865  ry`, on the othe
+000009a0: 720a 6861 6e64 2c20 7368 6f77 7320 6576  r.hand, shows ev
+000009b0: 6572 7974 6869 6e67 2e20 596f 7520 6361  erything. You ca
+000009c0: 6e20 7061 7373 2060 2d2d 6c61 7465 7374  n pass `--latest
+000009d0: 3d61 6c6c 6020 746f 2066 6564 7271 2074  =all` to fedrq t
+000009e0: 6f20 6368 616e 6765 2074 6869 730a 6265  o change this.be
+000009f0: 6861 7669 6f72 2e0a 0a23 2320 602d 2d72  havior...## `--r
+00000a00: 6570 6f60 2061 6e64 2060 2d2d 656e 6162  epo` and `--enab
+00000a10: 6c65 7265 706f 600a 0a66 6564 7271 2061  lerepo`..fedrq a
+00000a20: 6c73 6f20 7375 7070 6f72 7473 2060 2d2d  lso supports `--
+00000a30: 7265 706f 6020 616e 6420 602d 2d65 6e61  repo` and `--ena
+00000a40: 626c 6572 6570 6f60 2c20 6275 7420 7468  blerepo`, but th
+00000a50: 6579 2068 6176 6520 6164 6469 7469 6f6e  ey have addition
+00000a60: 616c 2066 756e 6374 696f 6e61 6c69 7479  al functionality
+00000a70: 2e0a 496e 2061 6464 6974 696f 6e20 6072  ..In addition `r
+00000a80: 6570 6f69 6460 732c 2074 6865 7365 206f  epoid`s, these o
+00000a90: 7074 696f 6e73 2061 6363 6570 7420 7265  ptions accept re
+00000aa0: 6c65 6173 652d 7370 6563 6966 6963 2067  lease-specific g
+00000ab0: 726f 7570 206e 616d 6573 2028 7468 6573  roup names (thes
+00000ac0: 650a 6172 6520 636f 6e66 6967 7572 6564  e.are configured
+00000ad0: 2069 6e20 6120 7265 6c65 6173 6527 7320   in a release's 
+00000ae0: 6064 6566 7360 2061 7320 6578 706c 6169  `defs` as explai
+00000af0: 6e65 6420 6162 6f76 6529 2c20 616e 6420  ned above), and 
+00000b00: 6765 6e65 7269 6320 7265 706f 0a63 6c61  generic repo.cla
+00000b10: 7373 6573 2e0a 0a46 6f72 2065 7861 6d70  sses...For examp
+00000b20: 6c65 2c20 796f 7520 6361 6e20 7061 7373  le, you can pass
+00000b30: 2060 2d62 2066 3337 202d 7220 4063 6f70   `-b f37 -r @cop
+00000b40: 723a 676f 746d 6178 3233 2f66 6564 7271  r:gotmax23/fedrq
+00000b50: 6020 746f 2071 7565 7279 202a 6f6e 6c79  ` to query *only
+00000b60: 2a20 7468 650a 676f 746d 6178 3233 2f66  * the.gotmax23/f
+00000b70: 6564 7271 2060 6665 646f 7261 2d33 3760  edrq `fedora-37`
+00000b80: 2043 6f70 7220 6368 726f 6f74 2773 2072   Copr chroot's r
+00000b90: 6570 6f73 6974 6f72 6965 732e 0a59 6f75  epositories..You
+00000ba0: 2063 616e 2070 6173 7320 602d 6220 6633   can pass `-b f3
+00000bb0: 3720 2d2d 656e 6162 6c65 7265 706f 2040  7 --enablerepo @
+00000bc0: 636f 7072 3a67 6f74 6d61 7832 332f 6665  copr:gotmax23/fe
+00000bd0: 6472 7160 2069 6620 796f 7520 7761 6e74  drq` if you want
+00000be0: 2074 6f20 656e 6162 6c65 0a74 6861 7420   to enable.that 
+00000bf0: 436f 7072 2773 2072 6570 6f73 6974 6f72  Copr's repositor
+00000c00: 7920 6f6e 2074 6f70 206f 6620 7468 6520  y on top of the 
+00000c10: 6261 7365 2072 6570 6f73 6974 6f72 6965  base repositorie
+00000c20: 732e 0a0a 5365 6520 7468 6520 5b52 4550  s...See the [REP
+00000c30: 4f20 434c 4153 5345 535d 2866 6564 7271  O CLASSES](fedrq
+00000c40: 312e 6d64 2f23 7265 706f 2d63 6c61 7373  1.md/#repo-class
+00000c50: 6573 2920 7365 6374 696f 6e20 6f66 2060  es) section of `
+00000c60: 6d61 6e20 6665 6472 7160 2066 6f72 206d  man fedrq` for m
+00000c70: 6f72 650a 696e 666f 726d 6174 696f 6e2e  ore.information.
+00000c80: 0a0a 2323 2053 7562 636f 6d6d 616e 6473  ..## Subcommands
+00000c90: 0a0a 6665 6472 7127 7320 434c 4920 696e  ..fedrq's CLI in
+00000ca0: 7465 7266 6163 6520 6973 2073 706c 6974  terface is split
+00000cb0: 2069 6e74 6f20 7375 6263 6f6d 6d61 6e64   into subcommand
+00000cc0: 7320 756e 6c69 6b65 2060 646e 6620 7265  s unlike `dnf re
+00000cd0: 706f 7175 6572 7960 2077 6869 6368 0a72  poquery` which.r
+00000ce0: 656c 6965 7320 6f6e 2066 6c61 6773 2e0a  elies on flags..
+00000cf0: 0a53 6565 205b 606d 616e 2066 6564 7271  .See [`man fedrq
+00000d00: 605d 2866 6564 7271 312e 6d64 2920 666f  `](fedrq1.md) fo
+00000d10: 7220 616e 2069 6e20 6465 7074 6820 6f72  r an in depth or
+00000d20: 6965 6e74 6174 696f 6e20 6f66 2066 6564  ientation of fed
+00000d30: 7271 2773 2043 4c49 0a69 6e74 6572 6661  rq's CLI.interfa
+00000d40: 6365 2e0a 0a23 2320 602d 2d72 6571 7569  ce...## `--requi
+00000d50: 7265 7360 2c20 602d 2d70 726f 7669 6465  res`, `--provide
+00000d60: 7360 2c20 616e 6420 6f74 6865 7220 7061  s`, and other pa
+00000d70: 636b 6167 6520 6174 7472 6962 7574 6573  ckage attributes
+00000d80: 0a0a 6064 6e66 2072 6570 6f71 7565 7279  ..`dnf repoquery
+00000d90: 6020 6861 7320 666c 6167 7320 7375 6368  ` has flags such
+00000da0: 2061 7320 602d 2d72 6571 7569 7265 7360   as `--requires`
+00000db0: 2061 6e64 2060 2d2d 7072 6f76 6964 6573   and `--provides
+00000dc0: 6020 746f 2064 6574 6572 6d69 6e65 0a63  ` to determine.c
+00000dd0: 6572 7461 696e 2070 6163 6b61 6765 2061  ertain package a
+00000de0: 7474 7269 6275 7465 732e 0a60 6665 6472  ttributes..`fedr
+00000df0: 7160 2073 7570 706f 7274 7320 7468 6573  q` supports thes
+00000e00: 6520 6f70 6572 6174 696f 6e73 2076 6961  e operations via
+00000e10: 2074 6865 2060 706b 6773 6020 7375 6263   the `pkgs` subc
+00000e20: 6f6d 6d61 6e64 2061 6e64 0a74 6865 2060  ommand and.the `
+00000e30: 2d46 6020 2f20 602d 2d66 6f72 6d61 7474  -F` / `--formatt
+00000e40: 6572 6020 666c 6167 2e0a 5365 6520 7468  er` flag..See th
+00000e50: 6520 7461 626c 6520 6265 6c6f 7720 666f  e table below fo
+00000e60: 7220 736f 6d65 2065 7861 6d70 6c65 732e  r some examples.
+00000e70: 0a0a 3c74 6162 6c65 3e0a 2020 2020 3c74  ..<table>.    <t
+00000e80: 623e 0a20 2020 2020 2020 203c 7472 3e0a  b>.        <tr>.
+00000e90: 2020 2020 2020 2020 2020 2020 3c74 643e              <td>
+00000ea0: 646e 6620 7265 706f 7175 6572 7920 2d2d  dnf repoquery --
+00000eb0: 7265 7175 6972 6573 2050 4143 4b41 4745  requires PACKAGE
+00000ec0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00000ed0: 2020 3c74 643e 6665 6472 7120 706b 6773    <td>fedrq pkgs
+00000ee0: 202d 4620 7265 7175 6972 6573 2050 4143   -F requires PAC
+00000ef0: 4b41 4745 3c2f 7464 3e0a 2020 2020 2020  KAGE</td>.      
+00000f00: 2020 3c2f 7472 3e0a 2020 2020 2020 2020    </tr>.        
+00000f10: 3c74 723e 0a20 2020 2020 2020 2020 2020  <tr>.           
+00000f20: 203c 7464 3e64 6e66 2072 6570 6f71 7565   <td>dnf repoque
+00000f30: 7279 202d 2d70 726f 7669 6465 7320 5041  ry --provides PA
+00000f40: 434b 4147 453c 2f74 643e 0a20 2020 2020  CKAGE</td>.     
+00000f50: 2020 2020 2020 203c 7464 3e66 6564 7271         <td>fedrq
+00000f60: 2070 6b67 7320 2d46 2070 726f 7669 6465   pkgs -F provide
+00000f70: 7320 5041 434b 4147 453c 2f74 643e 0a20  s PACKAGE</td>. 
+00000f80: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
+00000f90: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
+00000fa0: 2020 2020 2020 3c74 643e 646e 6620 7265        <td>dnf re
+00000fb0: 706f 7175 6572 7920 2d2d 7166 2022 257b  poquery --qf "%{
+00000fc0: 6e61 6d65 7d5c 6e22 2050 4143 4b41 4745  name}\n" PACKAGE
+00000fd0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00000fe0: 2020 3c74 643e 6665 6472 7120 706b 6773    <td>fedrq pkgs
+00000ff0: 202d 4620 6e61 6d65 2050 4143 4b41 4745   -F name PACKAGE
+00001000: 3c2f 7464 3e0a 2020 2020 2020 2020 3c2f  </td>.        </
+00001010: 7472 3e0a 2020 2020 3c2f 7462 3e0a 3c2f  tr>.    </tb>.</
+00001020: 7461 626c 653e 0a0a 5365 6520 7468 6520  table>..See the 
+00001030: 5b46 4f52 4d41 5454 4552 535d 2866 6564  [FORMATTERS](fed
+00001040: 7271 312e 6d64 2f23 666f 726d 6174 7465  rq1.md/#formatte
+00001050: 7273 5f31 2920 7365 6374 696f 6e20 6f66  rs_1) section of
+00001060: 2060 6d61 6e20 6665 6472 7160 2066 6f72   `man fedrq` for
+00001070: 206d 6f72 650a 696e 666f 726d 6174 696f   more.informatio
+00001080: 6e20 6162 6f75 7420 6176 6169 6c61 626c  n about availabl
+00001090: 6520 666f 726d 6174 7465 7273 2e0a       e formatters..
```

### Comparing `fedrq-0.9.0/doc/fedrq.1.scd` & `fedrq-1.0.0/doc/fedrq.1.scd`

 * *Files 21% similar despite different names*

```diff
@@ -2,102 +2,112 @@
 
 # NAME
 
 fedrq - Simplified repository querying
 
 # SYNOPSIS
 
-*\[fedrq \| python -m fedrq]* *[query type]* [options...] *[package...]*
+*<fedrq \| python -m fedrq>* *QUERY TYPE* [_OPTIONS_] [_PACKAGE_...]
 
-*\[fedrq \| python -m fedrq]* *[query type]* [options...] *\[-i \| --stdin ]*
+*<fedrq \| python -m fedrq>* *QUERY TYPE* [_OPTIONS_] _<-i|--stdin>_
 
-*\[fedrq \| python -m fedrq]* *check-config* [--dump] [--debug]
+*<fedrq \| python -m fedrq>* *check-config* [_--dump_] [_--debug_]
+
+*<fedrq | python -m fedrq>* *formatters* [_FORMATTERS OPTIONS_...]
 
 # DESCRIPTION
 
 fedrq is a tool to simplify querying the Fedora and EPEL repositories.
 
 # SUBCOMMANDS
 
 [[ check-config
 :[ Verify fedrq configuration. Only has *--debug* and *--dump* to dump the
    config. *--dump* requires *tomli-w*.
 |  pkgs
 :  Find the packages that match a list of package specs. Allows
-   *--whatprovides* like functionality with *--resolve-packages*.
+   *--whatprovides*-like functionality with the *--resolve-packages* flag.
 |  subpkgs
 :  Find the subpackages provided by a list of SRPMs.
-   Doesn't have *--src*, because subpkgs aren't SRPMs.
+   Doesn't support a *--src* flag, because subpkgs aren't SRPMs.
 |  whatenhances
-:  Find the packages that Enhance *[package...]*
+:  Find the packages that Enhance [_PACKAGE_...]
 |  whatrecommends
-:  Find the packages that Recommend *[package...]*
+:  Find the packages that Recommend [_PACKAGE_...]
 |  whatrequires
-:  Find the packages that Require *[package...]*
+:  Find the packages that Require [_PACKAGE_...]
 |  wr
-:  Alias for _whatrequires_
+:  Alias for *whatrequires*
 |  whatrequires-src
-:  Find the packages Require the subpackages of *[package...]*.
-   *[package...]* must be source package(s).
+:  Find the packages Require the subpackages of [_PACKAGE_...].
+   [_PACKAGE_...] must be source package(s).
 |  wrsrc
-:  Alias for _whatrequires-src_
+:  Alias for *whatrequires-src*
 |  whatsuggests
-:  Find the packages that Suggest *[package...]*
+:  Find the packages that Suggest [_PACKAGE_...]
 |  whatsupplements
-:  Find the packages that Supplement *[package...]*
+:  Find the packages that Supplement [_PACKAGE_...]
+|  make-cache
+:  Load the repodata for the current branch/repo config
+|  download
+:  Download an RPM from the repos. No GPG checking is performed.
+|  download-spec
+:  Download an (S)RPM and extract its specfile. No GPG checking is performed.
 
 # OPTIONS
 
 ## GLOBAL OPTIONS
 
 *-h*, *--help*
 	Show help message and quit.
 	Can be used after a command to get more information it.
 
 ## SHARED OPTIONS
 
 These options have the same meaning across multiple subcommands.
 
 *-i*, *--stdin*
-	Read package names from stdin. Cannot be used when passing postional
-	*[packages...]*.
-*-b*, *--branch* <branch name> (default: _rawhide_)
+	Read package names from stdin. Cannot be used when passing positional
+	\[_PACKAGE_...].
+*-b* _BRANCH NAME_, *--branch* _BRANCH NAME_ (default: *rawhide*)
 	Distribution release. This matches distgit branch names by convention.
 	See BUILTIN RELEASES for the releases available out of the box. Extra
 	configurations may be specified by the user. The chosen release impacts
-	what the releasever will be set to and which repositories will be
+	what the value of *$releasever* and which repositories will be
 	enabled by default.
-*-r*, *--repo* <repo class> (default: _@base_)
-	Enable <repo class> and disable all others for this operation. <repo
-	class> can be a standard repoid that's configured in /etc/yum.repos.d in
-	a ReleaseConfig's *defpaths* (see fedrq(5)). In addition, release
-	specifc repo groups and generic release class macros (e.g. *@copr*) are
-	accepted. When *--repo* isn't specified, the repositories in a Release's
+*-r* _REPO CLASS_, *--repo* _REPO CLASS_ (default: *@base*)
+	Enable _REPO CLASS_ and disable all others for this operation.
+	_REPO CLASS_ can be a standard repoid that's configured in
+	/etc/yum.repos.d or a custom one specified in a ReleaseConfig's
+	*defpaths* (see fedrq(5)).
+	In addition, release-specific repo groups and generic release class
+	macros (e.g., *@copr*) are accepted.
+	When *--repo* isn't specified, the repositories in a Release's
 	*@base* repo group are selected. See REPO CLASSES for more information.
-*-e*, *--enablerepo* <repo class>
+*-e* _REPO CLASS_, *--enablerepo* _REPO CLASS_
 	Enable certain repositories for this operation. All repositories in the
-	system configuration and any fedrq repo classes are accepted. Can be
-	specified multiple times. Accepts comma separated values. See REPO
-	CLASSES.
-*-l*, *--latest* <integer|"all"> (default: _1_)
+	system configuration and any fedrq repo classes are accepted. The option can be
+	specified multiple times. Accepts comma separated values.
+	See REPO CLASSES.
+*-l* _<integer|"all">_, *--latest* _<integer|"all">_ (default: _1_)
 	How many package versions to show for a given _name.arch_.
 	By default, only the latest is included.
 
 	*NOTE*: *dnf repoquery* includes _all_ by default.
-*-F*, *--formatter* <str> (default: _plain_)
+*-F*, *--formatter* _<str>_ (default: _plain_)
 	How the output should be formatted.
 	This is similar to *dnf repoquery --qf* but more limited.
 	All Package attributes from *dnf repoquery --querytags* are supported.
 	Some custom formatters are also available. See FORMATTERS for a list.
 *--debug*
 	Enable debug logging. Useful for development or bug reporting.
 *-P*, *--resolve-packages*
 	Resolve the correct Package when given a virtual Provide or file path.
 	For instance, /usr/bin/yt-dlp would resolve to yt-dlp.
-*-A*, *--arch* <str>
+*-A* _<str>_, *--arch* _<str>_
 	Only include packages that match this arch.
 	This does not apply \--forcearch.
 
 	*NOTE*: Unlike other tools, the -source repositories are always
 	enabled. You need to filter out src packages if you don't want them in
 	the output.
 *-s*, *--src*
@@ -109,111 +119,184 @@
 	for source packages that depend on a virtual Provide of the input
 	packages, because arch filtering is applied when resolving the input
 	packages' virtual Provides and files.
 *-S*, *--notsrc*
 	Equivalent to *--arch=notsrc*. This is a pseudo arch that does not exist
 	in rpm. It includes noarch and the system architecture. It does NOT
 	include multilib.
-*--forcearch* <str>
+*--forcearch* _ARCHITECTURE_
 	Query a foreign architecture's repositories
-*-B*, *--backend* <dnf|libdnf5>
+*-B* _<dnf|libdnf5>_, *--backend* _<dnf|libdnf5>_
 	Which package manager backend to use.
 	By default, fedrq uses dnf and falls back to libdnf5. Set *-B* /
 	*--backend* to make an explicit choice.
 	If you explicitly choose a backend whose dependencies are not met on
 	your system, fedrq will not fallback to another one.
-*-L*, *--filelists* <always|auto|never> (default: _auto_)
+*-L*  _<always|auto|never>_, *--filelists* _<always|auto|never>_ (default: _auto_)
 	Whether to load filelists. By default, filelists are only loaded when
 	using the files formatter (i.e. *-F files* or *-F json:files*). This
-	only applies when using the libdnf5 backend, which doesn't load
-	filelists by default to save memory and bandwidth. dnf4 always loads
-	filelists.
+	only applies when using the libdnf5 backend or newer versions of dnf4,
+	which do not load filelists by default to save memory and bandwidth.
+	*dnf < 4.19.0* always loads filelists.
 
 ## whatrequires, whatrecommends, whatsuggests
 
 *-X*, *--exclude-subpackages*
 	Filter out reverse dependencies that are built from the same source
 	package as _any_ of the input packages. See the whatrequires EXAMPLES.
 
 
 ## subpkgs
 
-*-M*, *--match* <pattern> (can be repeated to match against multiple patterns)
+*-M* _PATTERN_, *--match* _PATTERN_ (can be repeated to match against multiple patterns)
 	Only show subpackages whose name matches this string. Glob
 	patterns are permitted. When specified multiple times, _any_
 	match is included.
 
+## download and download-spec
+
+*-o* _PATH_, *--destdir* _PATH_
+	Directory in which to download/extract files.
+	Defaults to the current directory.
+
+## formatters
+
+The *formatters* subcommand lists available formatters.
+By default, all available formatters are shown,
+but they can be filtered by passing one or more of the following options.
+
+*--attrs*, *--only-attrs*
+	Only list package attributes
+*--formatters*, *--only-formatters*
+	Only list regular formatters
+*--special-formatters*, *--only-special-formatters*
+	Only list special formatters
+	(i.e., formatters that accept their own arguments)
+
 # FORMATTERS
 
-Package attributes (nonexhaustive; see *dnf repoquery --querytags*):
-- *-F name*: Show package names ++
-(example line: *yt-dlp*)
-- *-F arch*: Show package arches only ++
-(example line : *noarch*)
-- *-F repoid*: Show package's repo. ++
-(example line: *updates-testing*)
-
-Custom formatters:
-- *-F na*: Show package _name_._arch_ ++
-(example line: *yt-dlp.noarch*)
-- *-F nv*: Show package _name_-_version_ ++
-(example line: *yt-dlp-2022.11.11*)
-- *-F nev*: Show package _name_-_epoch_:_version_ ++
-(example line: *bind-32:9.18.8*)
-- *-F source*: Package queries can include source and binary
-  RPMs. The *source* formatter combines and deduplicates all of
-  the source names.
-  For example, if *python3-setuptools.noarch* is in the result,
-  it'll become *python-setuptools*.
-  If *python-setuptools.src* is also in the result, it'll become
-  *python-setuptools*, but *python-setuptools* won't be
-  duplicated in the output.
-- *-F breakdown*: Only supported by *fedrq --whatrequires*.
-  Shows a breakdown of runtime and buildtime dependencies.
-- *-F json:[comma seperated list of Package attrs]*:
-  Return an array of objects containing the specified Package attributes. The
-  JSON output is formatted with _indent=2_. The output can be piped to jq.
-- *-F line:[comma seperated list of Package attrs]*:
-  Return the specified package attributes on a single line.
-- *-F plainwithrepo*: Show default format and repoid separated by space: ++
-  (example line: *yt-dlp-2023.01.06-2.fc38.noarch rawhide*)
-- *-F nevrr*: alias to plainwithrepo formatter.
+## Package attributes
+
+This list is non-exhaustive. See *fedrq formatters --attrs*.
+
+*-F* name
+	Show package names ++
+	(example line: *yt-dlp*)
+*-F* arch
+	Show package arches only ++
+	(example line : *noarch*)
+*-F* repoid
+	Show package's repo. ++
+	(example line: *updates-testing*)
+
+## Regular formatters
+
+*-F* na
+	Show package _name_._arch_ ++
+	(example line: *yt-dlp.noarch*)
+*-F* nv
+	Show package _name_-_version_ ++
+	(example line: *yt-dlp-2022.11.11*)
+*-F* nev
+	Show package _name_-_epoch_:_version_ ++
+	(example line: *bind-32:9.18.8*)
+*-F* source
+	Package queries can include source and binary
+	RPMs. The *source* formatter combines and deduplicates all of
+	the source names.
+	For example, if *python3-setuptools.noarch* is in the result,
+	it'll become *python-setuptools*.
+	If *python-setuptools.src* is also in the result, it'll become
+	*python-setuptools*, but *python-setuptools* won't be
+	duplicated in the output.
+*-F* breakdown
+	Only supported by *fedrq --whatrequires*.
+	Shows a breakdown of runtime and buildtime dependencies.
+
+## Special formatters
+
+"Special formatters" accept arguments.
+
+*-F* json:_[comma separated list of Package attrs]_
+	Return an array of objects containing the specified Package attributes.
+	The JSON output is formatted with _indent=2_.
+	The output can be piped to jq.
+*-F* line:_[comma separated list of Package attrs]_
+	Return the specified package attributes on a single line.++
+	*NOTE*: The attributes provided must fit on one line. Attributes such as
+	_files_ or _requires_ that contain a list of items are not supported by
+	the *line* formatter.
+	See *-F* multiline for that usecase.
+*-F* multiline:_[single line attribute]_,_[multiline attribute]_
+	Display two package attributes together.++
+	(example call: -F multiline:name,files)++
+	(example line: _yt-dlp : /usr/bin/yt-dlp_)
+*-F* plainwithrepo
+	Show default format and repoid separated by space: ++
+	(example line: *yt-dlp-2023.01.06-2.fc38.noarch rawhide*)
+*-F* nevrr
+	Alias to plainwithrepo formatter.
+*-F* requiresmatch:_[comma- or semicolon-separated list of packages]_
+	List the Requires of *[package ...]* that resolve to the list of
+	packages provided to requiresmatch.
+	For example, *python3dist(ansible-core)* resolves to
+	requiresmatch:_ansible-core_.
+*-F* rm:_[comma- or semicolon-separated list of packages]_
+	Alias for *-F* requiresmatch
+*-F* na-requiresmatch:_[comma- or semicolon-separated list of packages]_
+	Combine the *-F* na and *-F* requiresmatch on a single line.
+	See the whatrequires EXAMPLES for usage.
+*-F* narm:_[comma- or semicolon-separated list of packages]_
+	Shortcut for *-F* na-requiresmatch
+*-F* source+requiresmatch:_[comma- or semicolon-separated list of packages]_
+	Combine the *-F* source and *-F* requiresmatch on a single line.
+*-F* source+rm:_[comma- or semicolon-separated list of packages]_
+	Shortcut for *-F* na-requiresmatch
+
+There are also _requiresmatch-src_ / _rmsrc_ and _na-requiresmatch_ / _narmsrc_
+formatters that work similarly to their non-src conterparts, expect they take a
+list of source packages.
+The list of source packages is converted into a list of binary packages
+(like the *subpkgs* subcommand) and then processed in the same way.
+If, say, a source package named *foo* has *foo*, *foo-devel*, and *foo-static*
+subpackages, *-F* _rmsrc:foo_ is equivalent to *-F* _rm:foo,foo-devel,foo-static_
 
 # REPO CLASSES
 
 The following generic repo class macros are available for all releases:
 
-*@file:[url or local path]*
+*@file:*_[url or local path]_
 	Load a .repo file from a local path or a url. Repositories with
 	*enabled=0* won't be loaded unless they are enabled explicitly with
 	*--enablerepo*.
-*@baseurl:[url]*
-	Load a repository from *url*. gpgcheck will be disabled.
-*@baseurl:[url],[gpgkey]*
-	Load a repository from *url* and set its gpgkey to *gpgkey*
-*@copr:[user/name]* or *@copr:[@group/name]*
+*@baseurl:*_[url]_
+	Load a repository from _[url]_. *gpgcheck* will be disabled.
+*@baseurl:*_[url]_,_[gpgkey]_
+	Load a repository from *url* and set its *gpgkey* to _[gpgkey]_
+*@copr:*_[user/name]_ or *@copr:*_[@group/name]_
 	Load a Copr repository. The Copr instance defaults to
 	*https://copr.fedoraproject.org* but may be configured in fedrq's
 	configuration. *copr_chroot_fmt* must be specifced in the selected
 	branch's release configuration for this repo class to work. This is
 	configured for the builtin releases.
-*@copr:[user/name@copr_baseurl]* or *@copr:[@group/name@copr_baseurl]*
+*@copr:*_[user/name@copr_baseurl]_ or *@copr:*_[@group/name@copr_baseurl]_
 	The *@copr* repo class also accepts a custom Copr instance.
 	Append *@* and a url.
 *@source-repos*
 	Enable the corresponding -source repos of the currently enabled
 	repositories
 *@base* or *base* or other group
-	The default repoistories for a release specified in a ReleaseConfig's
-	*defs.base*. Any other repo group specified in a release's is accepted,
-	with or without the *@*. See SPECIAL REPOS for which repo groups are
-	available for each release.
-*@repo:[key]* or *key* (fallback)
+	The default repositories for a release specified in a ReleaseConfig's
+	*defs.base*.
+	Any other repo group specified in a release's configuration is accepted,
+	with or without the *@*.
+	See SPECIAL REPOS for which repo groups are available for each release.
+*@repo:*_[key]_ or _key_ (fallback)
 	Accepts any repoid available in the system configuration or a .repo file
-	specific in the current ReleaseConfig's *defpaths*. If *key* is the name
+	specified in the current ReleaseConfig's *defpaths*. If *key* is the name
 	of a release's repo group (see above), that will be enabled instead.
 
 The following generic repo class macros are available for Fedora releases:
 
 *@koji:[key]*
 	Load the repositories for a koji.fedoraproject.org tag. ++
 	Example: *@koji:f39-build-side-XXXX*
@@ -292,15 +375,15 @@
 :  
 |  Amazon Linux
 :  amazon2023
 :  *@base*
 : 
 |  Fedora ELN
 :  eln
-:  *@base*, *no-crb*
+:  *@base*, *@no-crb*, *@buildroot*
 : 
 |  Default local system repositories
 :  local
 :  N/A
 :  This uses the default repositories with *enabled=1* in /etc/yum.repos.d and
    and the system's releasever.
 |  Default local system repositories with a different releasever
@@ -332,21 +415,24 @@
 	they don't have corresponding source repos. This causes problems for
 	fedrq, so those definitions are not available.
 
 # FILES
 
 ## CONFIGURATION
 
-*PYTHON_SITELIB/fedrq/data/\*.toml* Builtin configuration files. These should not be
-modified directly but may be overridden or used as examples.
-
-*/etc/fedrq/\*.toml* System wide configuration files. Has precedence over
-builtin configuration files.
+*PYTHON_SITELIB/fedrq/data/\*.toml* 
+	Builtin configuration files.
+	These should not be modified directly but may be overridden or used as examples.
+
+*/etc/fedrq/\*.toml*
+	System wide configuration files.
+	Has precedence over builtin configuration files.
 
-*~/.config/fedrq/\*.toml* User configuration files. Highest precedence
+*~/.config/fedrq/\*.toml*
+	User configuration files. Highest precedence.
 
 See fedrq(5) for configuration file syntax.
 
 # EXAMPLES
 
 ## pkgs
 
@@ -441,41 +527,92 @@
 ```
 $ fedrq pkgs -F nevrr -b f36 -r @copr:gotmax23/fedrq-dev fedrq
 fedrq-0.4.1^25.20230318.76d7910-1.fc36.noarch copr:copr.fedorainfracloud.org:gotmax23:fedrq-dev
 fedrq-0.4.1^25.20230318.76d7910-1.fc36.src copr:copr.fedorainfracloud.org:gotmax23:fedrq-dev
 ```
 
 
+In a single query, print the Requires of more than one package:
+```
+$ fedrq pkgs -F requires ansible-core.src yt-dlp.noarch
+make
+python3-devel
+python3dist(packaging)
+[...]
+/usr/bin/python3
+python3.12dist(requests)
+python3.12dist(urllib3)
+[...]
+```
+
+In a single query, print the Requires of more than one package, qualified by
+package name:
+```
+$ fedrq pkgs -F multiline:name,requires ansible-core.src yt-dlp.noarch
+ansible-core : make
+ansible-core : python3-devel
+ansible-core : python3dist(packaging)
+[...]
+yt-dlp : /usr/bin/python3
+yt-dlp : python3.12dist(requests)
+yt-dlp : python3.12dist(urllib3)
+[...]
+```
+
+
 ## whatrequires
 
 Find the packages that require another package, at buildtime or runtime:
 ```
 $ fedrq whatrequires yt-dlp
-audiotube-22.11-1.fc38.src
-audiotube-22.11-1.fc38.x86_64
-celluloid-0.24-4.fc38.x86_64
-gpodder-3.11.0-1.fc37.noarch
-media-downloader-2.7.0-2.fc38.x86_64
-persepolis-3.2.0-11.fc37.noarch
-video-downloader-0.10.12-1.fc38.noarch
-yt-dlp-bash-completion-2022.11.11-1.fc38.noarch
-yt-dlp-fish-completion-2022.11.11-1.fc38.noarch
-yt-dlp-zsh-completion-2022.11.11-1.fc38.noarch
+audiotube-24.01.95-1.fc40.src
+audiotube-24.01.95-1.fc40.x86_64
+celluloid-0.26-1.fc40.x86_64
+gpodder-3.11.4-4.fc40.noarch
+lollypop-1.4.37-7.fc40.noarch
+media-downloader-4.2.0-4.fc40.x86_64
+persepolis-3.2.0-16.fc40.noarch
+video-downloader-0.12.10-3.fc40.noarch
+yt-dlp-bash-completion-2023.12.30-2.fc40.noarch
+yt-dlp-fish-completion-2023.12.30-2.fc40.noarch
+yt-dlp-zsh-completion-2023.12.30-2.fc40.noarch
 ```
 
 Find a package's reverse dependencies, excluding subpackages:
 ```
 $ fedrq whatrequires -X yt-dlp
-audiotube-22.11-1.fc38.src
-audiotube-22.11-1.fc38.x86_64
-celluloid-0.24-4.fc38.x86_64
-gpodder-3.11.0-1.fc37.noarch
-media-downloader-2.7.0-2.fc38.x86_64
-persepolis-3.2.0-11.fc37.noarch
-video-downloader-0.10.12-1.fc38.noarch
+audiotube-24.01.95-1.fc40.src
+audiotube-24.01.95-1.fc40.x86_64
+celluloid-0.26-1.fc40.x86_64
+gpodder-3.11.4-4.fc40.noarch
+lollypop-1.4.37-7.fc40.noarch
+media-downloader-4.2.0-4.fc40.x86_64
+persepolis-3.2.0-16.fc40.noarch
+video-downloader-0.12.10-3.fc40.noarch
+```
+
+Find the packages that require another package, at buildtime or runtime and show
+which package spec it depends on.
+```
+$ fedrq whatrequires -F multiline:plain,rm:ansible-core: ansible-core
+ansible-9.2.0-1.fc40.noarch : (python3.12dist(ansible-core) >= 2.16.3 with python3.12dist(ansible-core) < 2.17)
+ansible-9.2.0-1.fc40.src : (python3dist(ansible-core) >= 2.16.3 with python3dist(ansible-core) < 2.17)
+ansible-bender-0.10.1-5.fc40.noarch : (ansible-core or ansible)
+ansible-collection-ansible-netcommon-6.0.0-3.fc40.noarch : (ansible-core or (ansible < 2.10.0 with ansible >= 2.9.10))
+[...]
+```
+
+Shortcut for the above:
+```
+$ fedrq whatrequires -F narm:ansible-core ansible-core
+ansible.noarch : (python3.12dist(ansible-core) >= 2.16.3 with python3.12dist(ansible-core) < 2.17)
+ansible.src : (python3dist(ansible-core) >= 2.16.3 with python3dist(ansible-core) < 2.17)
+ansible-bender.noarch : (ansible-core or ansible)
+ansible-collection-ansible-netcommon.noarch : (ansible-core or (ansible < 2.10.0 with ansible >= 2.9.10))
+[...]
 ```
 
 ## subpkgs
 
 Find an epel9 SRPM's subpackages
 ```
 $ fedrq subpkgs -b epel9 -F na epel-release
@@ -503,15 +640,14 @@
 Find the packages the need to be rebuilt when libindi's .so name is bumped:
 ```
 $ fedrq whatrequires-src -X -F source libindi
 indi-3rdparty-drivers
 indi-3rdparty-libraries
 kstars
 phd2
-stellarium
 ```
 
 
 # AUTHOR
 
 fedrq is maintained by Maxwell G <maxwell@gtmx.me>.
 See https://fedrq.gtmx.me/ for more information about fedrq.
```

### Comparing `fedrq-0.9.0/doc/fedrq.5.scd` & `fedrq-1.0.0/doc/fedrq.5.scd`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,39 @@
 # SYNTAX
 
 fedrq uses the TOML syntax for its configuration files.
 
 
 # DIRECTORIES
 
-*PYTHON_SITELIB/fedrq/data/\*.toml* Builtin configuration files. These should not be
-modified directly but may be overridden or used as examples.
-
-*/etc/fedrq/\*.toml* System wide configuration files. Has precedence over
-builtin configuration files.
-
-*~/.config/fedrq/\*.toml* User configuration files. Highest precedence
-
-Top level options and releases in the *[releases]* table can be redefined
-by creating a configuration file with higher precedence.
+*PYTHON_SITELIB/fedrq/data/\*.toml*
+	Builtin configuration files.
+	These should not be modified directly but may be overridden or used as examples.
+
+*/etc/fedrq/\*.toml*
+	System wide configuration files.
+	Has precedence over builtin configuration files.
+
+*~/.config/fedrq/\*.toml* 
+	User configuration files. Highest precedence.
+	Top level options and releases in the *[releases]* table can be redefined
+	by creating a configuration file with higher precedence.
 
 # OPTIONS
 
 *default_branch* <str> (default: _rawhide_)
 	What branch to query by default when *-b*/*--branch* is not specified.
-*smartcache* <bool> (default: _true_)
+*smartcache* <bool|Literal["always"]> (default: _true_)
 	Different releases have different _releasever_\s.
 	Switching the releasever (i.e. passing a different value to *--branch*)
 	clears the dnf cache.
 	When *smartcache* is _true_\, fedrq sets *base.conf.cachedir* to
 	_$XDG_CACHE_DIR/fedrq/BRANCH_ when changing the releasever.
-	The system cache is used if the requested branch's releasever is the
-	same as the system's releasever.
+	Unless *smartcache* is set to _always_, the system cache is used if the
+	requested branch's releasever is the same as the system's releasever.
 *releases* <dict[str, ReleaseConfig]>
 	Keys are a friendly name for the distribution.
 	RELEASE specifies the format for the values.
 *filelists* <always|never|auto> (default: _auto_)
 	See *--filelists* in fedrq(1)
 *backend* <dnf|libdnf5>
 	See *--backend* in fedrq(1)
```

### Comparing `fedrq-0.9.0/fedrq.spec` & `fedrq-1.0.0/fedrq.spec`

 * *Files 20% similar despite different names*

```diff
@@ -3,45 +3,43 @@
 # Copyright (C) 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 %bcond libdnf5 %[0%{?fedora} >= 38]
 
 Name:           fedrq
-Version:        0.9.0
+Version:        1.0.0
 Release:        1%{?dist}
 Summary:        A tool to query the Fedora and EPEL repositories
 
 # - code is GPL-2.0-or-later
 # - the data and config files in fedrq/data are UNLICENSEed
 # - Embeded repo defs are MIT.
 # - PSF-2.0 code copied from Cpython 3.11 for older Python versions
 License:        GPL-2.0-or-later AND Unlicense AND MIT AND PSF-2.0
 URL:            https://fedrq.gtmx.me
 %global furl    https://git.sr.ht/~gotmax23/fedrq
 Source0:        %{furl}/refs/download/v%{version}/fedrq-%{version}.tar.gz
 
 BuildArch:      noarch
 
-BuildRequires:  tomcli+tomlkit
 BuildRequires:  python3-devel
 # Test deps
 BuildRequires:  createrepo_c
 BuildRequires:  distribution-gpg-keys
 BuildRequires:  python3-argcomplete
 BuildRequires:  python3-dnf
 %if %{with libdnf5}
 BuildRequires:  python3-libdnf5
-BuildRequires:  python3-rpm
 %endif
 # Manpage
 BuildRequires:  scdoc
 
-Requires:       (python3-dnf or (python3-libdnf5 and python3-rpm))
-Suggests:       python3-dnf
+Requires:       (python3-dnf or python3-libdnf5)
+Suggests:       (python3-libdnf5 if dnf5)
 Requires:       distribution-gpg-keys
 Recommends:     fedora-repos-rawhide
 Recommends:     python3-argcomplete
 
 # fedrq config --dump
 Recommends:     python3-tomli-w
 
@@ -49,17 +47,14 @@
 %description
 fedrq is a tool to query the Fedora and EPEL repositories.
 
 
 %prep
 %autosetup -p1
 
-# See the comments in pyproject.toml
-tomcli-set pyproject.toml del tool.flit.external-data
-tomcli-set pyproject.toml list build-system.requires "flit_core >=3.2,<4"
 
 %generate_buildrequires
 %pyproject_buildrequires -x test
 
 
 %build
 %py3_shebang_fix contrib/api_examples/*.py
@@ -77,32 +72,65 @@
 install -Dpm 0644 fedrq.1 -t %{buildroot}%{_mandir}/man1/
 install -Dpm 0644 fedrq.5 -t %{buildroot}%{_mandir}/man5/
 install -Dpm 0644 fedrq.bash %{buildroot}%{bash_completions_dir}/fedrq
 install -Dpm 0644 fedrq.fish %{buildroot}%{fish_completions_dir}/fedrq.fish
 
 
 %check
+bash -x ./tests/test_data/build.sh
+
 FEDRQ_BACKEND=dnf %pytest -v -m "not no_rpm_mock"
+
 %if %{with libdnf5}
-FEDRQ_BACKEND=libdnf5 %pytest -v -m "not no_rpm_mock"
+# Some tests are failing only in mock and only with Python 3.12
+#   RuntimeError: Failed to download metadata
+%if v"0%{?python3_version}" >= v"3.12"
+%global skips %{shrink:
+    not test_smartcache_not_used
+    and not test_smartcache_config
+    and not test_baseurl_repog
+}
+%endif
+FEDRQ_BACKEND=libdnf5 %pytest -v -m "not no_rpm_mock" %{?skips:-k '%{skips}'}
 %endif
 
 
 %files -f %{pyproject_files}
 # Licenses are included in the wheel
-%license LICENSES/*.txt
+%license %{_licensedir}/fedrq/
 %doc README.md CONTRIBUTING.md NEWS.md contrib/api_examples
 %{_bindir}/fedrq*
 %{bash_completions_dir}/fedrq
 %{fish_completions_dir}/fedrq.fish
 %{_mandir}/man1/fedrq.1*
 %{_mandir}/man5/fedrq.5*
 
 
 %changelog
+* Mon Apr 01 2024 Maxwell G <maxwell@gtmx.me> - 1.0.0-1
+- Release 1.0.0.
+
+* Tue Feb 13 2024 Maxwell G <maxwell@gtmx.me> - 0.15.0-1
+- Release 0.15.0.
+
+* Wed Feb 07 2024 Maxwell G <maxwell@gtmx.me> - 0.14.0-1
+- Release 0.14.0.
+
+* Mon Dec 18 2023 Maxwell G <maxwell@gtmx.me> - 0.13.0-1
+- Release 0.13.0.
+
+* Mon Sep 11 2023 Maxwell G <maxwell@gtmx.me> - 0.12.0-1
+- Release 0.12.0.
+
+* Thu Aug 31 2023 Maxwell G <maxwell@gtmx.me> - 0.11.0-1
+- Release 0.11.0.
+
+* Wed Jul 12 2023 Maxwell G <maxwell@gtmx.me> - 0.10.0-1
+- Release 0.10.0.
+
 * Thu Jun 29 2023 Maxwell G <maxwell@gtmx.me> - 0.9.0-1
 - Release 0.9.0.
 
 * Wed Jun 21 2023 Maxwell G <maxwell@gtmx.me> - 0.8.0-1
 - Release 0.8.0.
 
 * Wed May 31 2023 Maxwell G <maxwell@gtmx.me> - 0.7.1-1
```

### Comparing `fedrq-0.9.0/mkdocs.yml` & `fedrq-1.0.0/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -28,44 +28,51 @@
       scheme: slate
       primary: pink
       accent: pink
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
 markdown_extensions:
+  - admonition
+  - smarty
   - toc:
       permalink: true
   - tables
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.magiclink
   - pymdownx.superfences
 plugins:
   - mkdocstrings:
       default_handler: python
       handlers:
         python:
           options:
-            docstring_style: sphinx
+            docstring_style: google
             show_if_no_docstring: true
             merge_init_into_class: true
             filters: ["!^__?", "!LOG", "!logger"]
             show_signature_annotations: true
             separate_signature: true
           paths:
             - src/
           import:
             - https://docs.python.org/3/objects.inv
             - https://dnf.readthedocs.io/en/latest/objects.inv
             - https://dnf5.readthedocs.io/en/latest/objects.inv
+  - gen-files:
+      scripts:
+        - doc/mkdocs_mangen.py
   - exclude:
       glob:
         - "*.tar.gz"
         - "fedrq.1*"
         - "fedrq.5*"
+        - "*.py"
+        - "requirements.*"
 watch:
   - "README.md"
   - "NEWS.md"
   - "src/fedrq"
 nav:
   - Home: index.md
   - News.md
```

### Comparing `fedrq-0.9.0/noxfile.py` & `fedrq-1.0.0/noxfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,137 @@
 # SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later OR MIT
 
 from __future__ import annotations
 
 import os
+from collections.abc import Sequence
 from glob import iglob
 from pathlib import Path
 from shutil import copy2
 
 import nox
 
 IN_CI = "JOB_ID" in os.environ or "CI" in os.environ
 ALLOW_EDITABLE = os.environ.get("ALLOW_EDITABLE", str(not IN_CI)).lower() in (
     "1",
     "true",
 )
+PINNED = os.environ.get("PINNED", "true").lower() in (
+    "1",
+    "true",
+)
 
 PROJECT = "fedrq"
 SPECFILE = "fedrq.spec"
 LINT_SESSIONS = ("formatters", "codeqa", "typing")
 LINT_FILES = (f"src/{PROJECT}", "tests/", "noxfile.py")
-RELEASERR = "releaserr @ git+https://git.sr.ht/~gotmax23/releaserr"
-# RELEASERR = "-e../releaserr"
 
-nox.options.sessions = (*LINT_SESSIONS, "dnf_test", "libdnf5_test")
+nox.options.sessions = ("lint", "covtest")
+nox.options.reuse_existing_virtualenvs = True
 
 
 # Helpers
 
 
-def install(session: nox.Session, *args, editable=False, **kwargs):
+def install(
+    session: nox.Session, *args, editable=False, constraint: str | None = None, **kwargs
+):
+    # nox --no-venv
+    if isinstance(session.virtualenv, nox.virtualenv.PassthroughEnv):
+        session.warn(f"No venv. Skipping installation of {args}")
+        return
+    largs = []
+    if constraint and PINNED:
+        largs.extend(("-c", f"requirements/{constraint}.txt"))
     if editable and ALLOW_EDITABLE:
-        args = ("-e", *args)
-    session.install(*args, **kwargs)
+        largs.append("-e")
+    session.install(*largs, *args, **kwargs)
 
 
 def git(session: nox.Session, *args, **kwargs):
     return session.run("git", *args, **kwargs, external=True)
 
 
 # General
 
 
 @nox.session(venv_params=["--system-site-packages"])
-def test(session: nox.Session, backend=None):
+def test(
+    session: nox.Session,
+    backend: str | None = None,
+    posargs: Sequence[str] | None = None,
+):
     if not backend:
         # Make sure pytest is updated, as using the version from system
         # site-packages causes problems with plugins.
-        install(session, ".[test]", "pytest", "-U", editable=True)
+        install(session, ".[test]", constraint="test", editable=True)
     tmp = Path(session.create_tmp())
     env = {"FEDRQ_BACKEND": backend} if backend else {}
     if any(i.startswith("--cov") for i in session.posargs):
         install(session, "coverage[toml]", "pytest-cov")
         env |= {"COVERAGE_FILE": str(tmp / ".coverage")}
-    session.run("pytest", *session.posargs, env=env)
+    session.run(
+        "pytest", *(posargs if posargs is not None else session.posargs), env=env
+    )
 
 
 @nox.session
 def coverage(session: nox.Session):
     install(session, "coverage[toml]")
     session.run("coverage", "combine", "--keep", *iglob(".nox/*test/tmp/.coverage"))
-    session.run("coverage", "report")
     session.run("coverage", "html")
+    session.run("coverage", "report", "--fail-under=90")
+
+
+@nox.session
+def covtest(session: nox.Session):
+    session.run("rm", "-f", *iglob(".nox/*/tmp/.coverage"), external=True)
+    for name in ("dnf_test", "libdnf5_test", "pydanticv1_test", "coverage"):
+        session.notify(name, [*session.posargs, "--cov"])
 
 
 @nox.session(venv_backend="none")
 def lint(session: nox.Session):
     """
     Run formatters, codeql, typing, and reuse sessions
     """
     for notify in LINT_SESSIONS:
         session.notify(notify)
 
 
 @nox.session()
 def codeqa(session: nox.Session):
-    install(session, ".[codeqa]")
-    session.run("ruff", *session.posargs, *LINT_FILES)
+    install(session, ".[codeqa]", constraint="codeqa")
+    session.run("ruff", "check", *session.posargs, *LINT_FILES)
     session.run("reuse", "lint")
 
 
 @nox.session
 def formatters(session: nox.Session):
-    install(session, ".[formatters]")
+    install(session, ".[formatters]", constraint="formatters")
     posargs = session.posargs
     if IN_CI:
         posargs.append("--check")
     session.run("black", *posargs, *LINT_FILES)
     session.run("isort", *posargs, *LINT_FILES)
 
 
 @nox.session
 def typing(session: nox.Session):
-    install(session, ".[typing]", editable=True)
+    install(session, ".[typing]", editable=True, constraint="typing")
     session.run("mypy", "--enable-incomplete-feature=Unpack", "src/fedrq/")
 
 
-@nox.session
+@nox.session(reuse_venv=False)
 def bump(session: nox.Session):
     version = session.posargs[0]
 
-    install(session, RELEASERR, "flit", "fclogr")
+    install(session, "releaserr", "flit", "fclogr")
 
     session.run("releaserr", "check-tag", version)
     session.run("releaserr", "ensure-clean")
     session.run("releaserr", "set-version", "-s", "file", version)
 
     install(session, ".")
 
@@ -121,18 +147,18 @@
 
     # Bump changelog, commit, and tag
     git(session, "add", SPECFILE, f"src/{PROJECT}/__init__.py")
     session.run("releaserr", "clog", version, "--tag")
     session.run("releaserr", "build", "--sign", "--backend", "flit_core")
 
 
-@nox.session
+@nox.session(reuse_venv=False)
 def publish(session: nox.Session):
     # Setup
-    install(session, RELEASERR, "twine")
+    install(session, "releaserr", "twine")
     session.run("releaserr", "ensure-clean")
 
     # Upload to PyPI
     session.run("releaserr", "upload")
 
     # Push to git, publish artifacts to sourcehut, and release to copr
     if not session.interactive or input(
@@ -156,17 +182,17 @@
     copy2(SPECFILE, dest)
     session.run("python", "contrib/fedoraify.py", str(dest))
     session.run("copr-cli", "build", "--nowait", f"gotmax23/{PROJECT}", str(dest))
 
 
 @nox.session
 def srpm(session: nox.Session, posargs=None):
-    install(session, "fclogr")
+    install(session, "-r", "requirements/srpm.in", constraint="srpm")
     posargs = posargs or session.posargs
-    session.run("fclogr", "--debug", "dev-srpm", *posargs)
+    session.run("python3", "-m", "fclogr", "--debug", "dev-srpm", *posargs)
 
 
 @nox.session
 def mockbuild(session: nox.Session):
     tmp = Path(session.create_tmp())
     srpm(session, ("-o", tmp, "--keep"))
     spec_path = tmp / "fedrq.spec"
@@ -183,56 +209,89 @@
     session.run(*margs, external=True)
 
 
 # fedrq specific
 
 
 @nox.session
-def docgen(session: nox.Session):
-    """
-    Generate extra content for the docsite
-    """
-    for i in ("1", "5"):
-        # Long, terrible pipeline to convert scdoc to markdown
-        # fmt: off
-        session.run(
-            "sh", "-euo", "pipefail", "-c",
-            # Convert scdoc to html
-            f"scd2html < doc/fedrq.{i}.scd"
-            # Remove aria-hidden attributes so pandoc doesn't try to convert them
-            "| sed 's|aria-hidden=\"true\"||'"
-            "| pandoc --from html "
-            # mkdocs doesn't support most of the pandoc markdown extensions.
-            # Use markdown_strict and only enable pipe_tables.
-            "--to markdown_strict+pipe_tables"
-            "| sed "
-            # Remove anchors that scd2html inserts
-            r"-e 's| \[¶\].*||' "
-            f"> doc/fedrq{i}.md",
-            external=True,
-        )
-        # fmt: on
-
-
-@nox.session
 def mkdocs(session: nox.Session):
-    install(session, "-e", ".[doc]")
-    docgen(session)
-    session.run("mkdocs", *session.posargs)
+    install(session, "-e", ".[doc]", constraint="doc")
+    session.run("mkdocs", *(session.posargs or ["build"]))
 
 
 @nox.session(venv_backend="none")
-def testa(session):
-    session.notify("dnf_test")
-    session.notify("libdnf5_test")
+def testa(session: nox.Session):
+    session.notify("dnf_test", ["--cov"])
+    session.notify("libdnf5_test", ["--cov"])
+    session.notify("pydanticv1_test")
+    session.notify("coverage")
 
 
 @nox.session(venv_params=["--system-site-packages"])
 def dnf_test(session: nox.Session):
-    install(session, ".[test]", "pytest", "-U", editable=True)
+    install(session, ".[test]", constraint="test", editable=True)
     test(session, "dnf")
 
 
 @nox.session
 def libdnf5_test(session: nox.Session):
-    install(session, ".[test]", "libdnf5-shim", "rpm", editable=True)
+    install(session, ".[test]", "libdnf5-shim", constraint="test", editable=True)
     test(session, "libdnf5")
+
+
+@nox.session(venv_params=["--system-site-packages"])
+def pydanticv1_test(session: nox.Session):
+    install(session, ".[test]", constraint="pydanticv1_test")
+    test(session, "dnf", ["tests/unit"])
+
+
+@nox.session(
+    name="pip-compile", python=["3.9"], venv_params=["--download"], reuse_venv=False
+)
+def pip_compile(session: nox.Session):
+    session.install("pip-tools")
+    Path("requirements").mkdir(exist_ok=True)
+
+    # Use --upgrade by default unless a user passes -P.
+    args = list(session.posargs)
+    if not any(
+        arg.startswith(("-P", "--upgrade-package", "--no-upgrade")) for arg in args
+    ):
+        args.append("--upgrade")
+
+    # fmt: off
+    session.run(
+        "pip-compile",
+        "-o", "requirements/requirements.txt",
+        *args,
+    )
+
+    extras = (
+        "codeqa",
+        "doc",
+        "formatters",
+        "typing",
+        "test",
+    )
+    for extra in extras:
+        session.run(
+            "pip-compile",
+            "-o", f"requirements/{extra}.txt",
+            f"--extra={extra}",
+            *args,
+        )
+
+    extras_a = [f"--extra={extra}" for extra in extras]
+    session.run("pip-compile", "-o", "requirements/all.txt", *extras_a, *args)
+
+    session.run(
+        "pip-compile", "-o", "requirements/srpm.txt", *args, "requirements/srpm.in"
+    )
+
+    session.run(
+        "pip-compile",
+        "-o", "requirements/pydanticv1_test.txt",
+        "-c", "requirements/pydanticv1.in",
+        "--extra=test",
+        *args,
+    )
+    # fmt: on
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fedrq-0.9.0/pyproject.toml` & `fedrq-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -18,46 +18,54 @@
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: POSIX :: Linux",
     "Development Status :: 4 - Beta",
     "Typing :: Typed",
     "Environment :: Console",
 ]
 dependencies = [
     # This cannot be installed from PyPI
     # "dnf",
-    "pydantic ~= 1.0",
+    "pydantic >= 1, < 3",
     "tomli; python_version<'3.11'",
     "requests",
+    "rpm",
     # Optional dependency for `fedrq check-config --dump`
     # "tomli-w",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 codeqa = [
     "ruff",
     "reuse",
 ]
 doc = [
     # mkdocstrings-python uses black to format function signatures
     "black",
+    # This is a transitive dependency of mkdocstrings-python
+    # 0.32.0 breaks black function signature formatting
+    "griffe !=0.32.0, !=0.32.1",
     "mkdocs",
+    "mkdocs-exclude",
+    "mkdocs-gen-files",
     "mkdocs-material",
     "mkdocstrings[python]>=0.18",
-    "mkdocs-exclude",
+    "releaserr",
 ]
 formatters = [
     "black",
-    "isort",
+    # 5.13.0 introduced https://github.com/PyCQA/isort/issues/2206
+    "isort !=5.13.0",
 ]
 typing = [
     "mypy",
     "types-requests",
     # Optional fedrq runtime dependency
     "argcomplete",
     "typing_extensions",
@@ -119,31 +127,45 @@
 profile = "black"
 add_imports = [
     'from __future__ import annotations',
 ]
 
 
 [tool.coverage.run]
+source = [
+    "fedrq",
+]
 omit = [
     "src/fedrq/_compat.py",
-    "src/fedrq/repoquery.py",
     "src/fedrq/__main__.py",
 ]
 
+[tool.coverage.paths]
+source = [
+    "src",
+    "*/site-packages",
+]
+
 [tool.coverage.report]
 # https://coverage.readthedocs.io/en/latest/excluding.html#advanced-exclusion
 # These should use single quotes in TOML, as they're regular expressions.
 exclude_lines = [
     'pragma: no cover',
     'raise NotImplementedError',
     'if __name__ == .__main__.:',
     'if TYPE_CHECKING:',
     'if t\.TYPE_CHECKING:',
     '@(abc\.)?abstractmethod',
     '@overload',
     'except ImportError',
+    'raise AssertionError\("unreachable"\)',
 ]
 omit = [
     "src/fedrq/_compat.py",
-    "src/fedrq/repoquery.py",
     "src/fedrq/__main__.py",
 ]
+
+[tool.pip-tools]
+resolver = "backtracking"
+allow-unsafe = true
+quiet = true
+strip-extras = true
```

### Comparing `fedrq-0.9.0/src/fedrq/_archive.py` & `fedrq-1.0.0/src/fedrq/_archive.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/_compat.py` & `fedrq-1.0.0/src/fedrq/_compat.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/_utils.py` & `fedrq-1.0.0/src/fedrq/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import logging
 import typing as t
+from collections import deque
 from collections.abc import Iterator, MutableMapping
 
 if t.TYPE_CHECKING:
     from fedrq.backends.base import PackageCompat, PackageQueryCompat
 
 logger = logging.getLogger(__name__)
 
@@ -38,9 +39,11 @@
         ):
             merge_dict(value, dest[key])
             continue
         dest[key] = value
 
 
 def exhaust_it(it: Iterator[t.Any]) -> None:
-    for _ in it:
-        pass
+    """
+    Exhaust an iterator in the most efficient manner possible
+    """
+    deque(it, maxlen=0)
```

### Comparing `fedrq-0.9.0/src/fedrq/backends/__init__.py` & `fedrq-1.0.0/src/fedrq/backends/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,28 +52,31 @@
 
 
 class _DefaultBackend:
     def __init__(self) -> None:
         self.backend: BackendMod | None = None
 
     def __call__(
-        self, default: str | None = None, fallback: bool = False
+        self,
+        default: str | None = None,
+        fallback: bool = False,
+        allow_multiple_backends_per_process: bool = True,
     ) -> BackendMod:
-        if not self.backend:
+        if not self.backend or (allow_multiple_backends_per_process and default):
             self.backend = self._get_backend(default, fallback)
-            LOG.info("Using %s backend", self.backend.BACKEND)
-        elif default and default != self.backend.BACKEND:
+        elif (
+            default != self.backend.BACKEND and not allow_multiple_backends_per_process
+        ):
             warnings.warn(
                 f"Falling back to {self.backend.BACKEND}. {default} cannot be used."
             )
         return self.backend
 
-    def _get_backend(
-        self, default: str | None = None, fallback: bool = False
-    ) -> BackendMod:
+    @staticmethod
+    def _get_backend(default: str | None = None, fallback: bool = False) -> BackendMod:
         default = default or DEFAULT_BACKEND
         if default not in BACKENDS:
             raise MissingBackendError(f"Invalid backend {default!r}.")
         backends = _get_backends()
         if backend := backends.available.get(default):
             return backend.get_backend()
         if not fallback:
```

### Comparing `fedrq-0.9.0/src/fedrq/backends/base.py` & `fedrq-1.0.0/src/fedrq/backends/base/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import abc
+import dataclasses
 import importlib.resources
 import logging
 from collections.abc import Callable, Collection, Iterable, Iterator
+from datetime import date
 from typing import TYPE_CHECKING, Any, Optional, Protocol, TypeVar, runtime_checkable
 from warnings import warn
 
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
     from fedrq.config import Release
@@ -22,189 +24,151 @@
 @runtime_checkable
 class PackageCompat(Protocol):  # pragma: no cover
     """
     Common interface provided by dnf.package.Package and other backends
     """
 
     @property
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
     @property
-    def arch(self) -> str:
-        ...
+    def arch(self) -> str: ...
 
     @property
-    def a(self) -> str:
-        ...
+    def a(self) -> str: ...
 
     @property
-    def epoch(self) -> int:
-        ...
+    def epoch(self) -> int: ...
 
     @property
-    def e(self) -> int:
-        ...
+    def e(self) -> int: ...
 
     @property
-    def version(self) -> str:
-        ...
+    def version(self) -> str: ...
 
     @property
-    def v(self) -> str:
-        ...
+    def v(self) -> str: ...
 
     @property
-    def release(self) -> str:
-        ...
+    def release(self) -> str: ...
 
     @property
-    def r(self) -> str:
-        ...
+    def r(self) -> str: ...
 
     @property
-    def from_repo(self) -> str:
-        ...
+    def from_repo(self) -> str: ...
 
     @property
-    def evr(self) -> str:
-        ...
+    def evr(self) -> str: ...
 
     @property
-    def debug_name(self) -> str:
-        ...
+    def debug_name(self) -> str: ...
 
     @property
-    def source_name(self) -> Optional[str]:
-        ...
+    def source_name(self) -> Optional[str]: ...
 
     @property
-    def source_debug_name(self) -> str:
-        ...
+    def source_debug_name(self) -> str: ...
 
     @property
-    def installtime(self) -> int:
-        ...
+    def installtime(self) -> int: ...
 
     @property
-    def buildtime(self) -> int:
-        ...
+    def buildtime(self) -> int: ...
 
     @property
-    def size(self) -> int:
-        ...
+    def size(self) -> int: ...
 
     @property
-    def downloadsize(self) -> int:
-        ...
+    def downloadsize(self) -> int: ...
 
     @property
-    def installsize(self) -> int:
-        ...
+    def installsize(self) -> int: ...
 
     @property
-    def provides(self) -> Iterable:
-        ...
+    def provides(self) -> Iterable: ...
 
     @property
-    def requires(self) -> Iterable:
-        ...
+    def requires(self) -> Iterable: ...
 
     @property
-    def recommends(self) -> Iterable:
-        ...
+    def recommends(self) -> Iterable: ...
 
     @property
-    def suggests(self) -> Iterable:
-        ...
+    def suggests(self) -> Iterable: ...
 
     @property
-    def supplements(self) -> Iterable:
-        ...
+    def supplements(self) -> Iterable: ...
 
     @property
-    def enhances(self) -> Iterable:
-        ...
+    def enhances(self) -> Iterable: ...
 
     @property
-    def obsoletes(self) -> Iterable:
-        ...
+    def obsoletes(self) -> Iterable: ...
 
     @property
-    def conflicts(self) -> Iterable:
-        ...
+    def conflicts(self) -> Iterable: ...
 
     @property
-    def sourcerpm(self) -> Optional[str]:
-        ...
+    def sourcerpm(self) -> Optional[str]: ...
 
     @property
-    def description(self) -> str:
-        ...
+    def description(self) -> str: ...
 
     @property
-    def summary(self) -> str:
-        ...
+    def summary(self) -> str: ...
 
     @property
-    def license(self) -> str:
-        ...
+    def license(self) -> str: ...
 
     @property
-    def url(self) -> str:
-        ...
+    def url(self) -> str: ...
 
     @property
-    def reason(self) -> Optional[str]:
-        ...
+    def reason(self) -> Optional[str]: ...
 
     @property
-    def files(self) -> Iterable[str]:
-        ...
+    def files(self) -> Iterable[str]: ...
 
     @property
-    def reponame(self) -> str:
-        ...
+    def reponame(self) -> str: ...
 
     @property
-    def repoid(self) -> str:
-        ...
+    def repoid(self) -> str: ...
 
     @property
-    def vendor(self) -> str:
-        ...
+    def vendor(self) -> str: ...
 
     @property
-    def packager(self) -> str:
-        ...
+    def packager(self) -> str: ...
 
     @property
-    def location(self) -> str:
-        ...
+    def location(self) -> str: ...
+
+    @property
+    def repo(self) -> Any:
+        """
+        Return the package's Repo object.
+        The exact object depends on which backend is used.
+        """
 
     @abc.abstractmethod
     def remote_location(
         self, schemes: Collection[str] | None = ("http", "ftp", "file", "https")
-    ) -> str | None:
-        ...
+    ) -> str | None: ...
 
-    def __hash__(self) -> int:
-        ...
+    def __hash__(self) -> int: ...
 
-    def __lt__(self, other) -> bool:
-        ...
+    def __lt__(self, other) -> bool: ...
 
-    def __le__(self, other) -> bool:
-        ...
+    def __le__(self, other) -> bool: ...
 
-    def __gt__(self, other) -> bool:
-        ...
+    def __gt__(self, other) -> bool: ...
 
-    def __ge__(self, other) -> bool:
-        ...
+    def __ge__(self, other) -> bool: ...
 
 
 @runtime_checkable
 class PackageQueryCompat(Protocol):  # pragma: no cover
     """
     Common PackageQuery interface provided by hawkey.Query and other backends.
     """
@@ -231,31 +195,37 @@
         """
         Combine two PackageQuery objects.
         Depending on the backend, this either modifies 'self' in place and
         returns 'self' or returns a new PackageQuery object.
         """
         ...
 
-    def __len__(self) -> int:
-        ...
+    def __len__(self) -> int: ...
 
-    def __iter__(self) -> Iterator[PackageCompat]:
-        ...
+    def __iter__(self) -> Iterator[PackageCompat]: ...
 
 
-class BaseMakerBase(abc.ABC):
+class BaseMakerBase(metaclass=abc.ABCMeta):
     """
     Create a Base object, set configuration, and load repos
     """
 
     base: Any
 
     def __init__(self, base=None) -> None:
         self.base = base
 
+    @property
+    @abc.abstractmethod
+    def conf(self) -> Any:
+        """
+        Return the backend's Config object
+        """
+        ...
+
     @abc.abstractmethod
     def fill_sack(
         self,
         *,
         from_cache: bool = False,
         load_system_repo: bool = False,
     ):
@@ -323,75 +293,112 @@
         """
         Load repositories from a repo file if they're not already in the
         configuration.
         """
 
     def sets(self, conf: dict[str, Any], substitutions: dict[str, Any]) -> None:
         """
-        :param conf: A dict of configuration options. Call self.set() for each
-        k-v pair.
-        :param substitutions: A dict of substitutions/vars options. Call self.set_var()
-        for each k-v pair.
+        Set options on the base object
+
+        Args:
+            conf:
+                A dict of configuration options. Call self.set() for each k-v
+                pair.
+            substitutions:
+                A dict of substitutions/vars options. Call self.set_var() for
+                each k-v pair.
         """
         for opt in conf.items():
             self.set(*opt)
         for opt in substitutions.items():
             self.set_var(*opt)
 
-    def load_filelists(self) -> None:
+    def load_filelists(self, enable: bool = True) -> None:  # noqa: ARG002
         # Can be overriden by subclasses. Purposely isn't an @abstractmethod.
         """
-        Load the filelists if they're not already enabled default
+        Load the filelists if they're not already enabled by default
+
+        Args:
+            enable:
+                Whether to enable or disable filelists
         """
         return None
 
+    @abc.abstractmethod
+    def load_changelogs(self, enable: bool = True) -> None:
+        """
+        Load changelog metadata
+
+        Args:
+            enable:
+                Whether to enable or disable filelists
+        """
+
     def load_release_repos(self, release: Release, set_releasever: bool = True) -> None:
         """
         Load the repositories from a fedrq.config.Release object
+
+        Args:
+            release:
+                [`Release`][fedrq.config.Release] object
+            set_releasever:
+                Whether to set the `$releasever` based on the release or just
+                leave it alone
         """
         if set_releasever:
             self.set_var("releasever", release.version)
         if release.release_config.system_repos:
             self.read_system_repos(
                 disable=not release.release_config.append_system_repos
             )
         for path in release.release_config.full_def_paths:
             with importlib.resources.as_file(path) as fp:
                 LOG.debug("Reading %s", fp)
                 self._read_repofile_new(fp)
         release.repog.load(self, release.config, release)
 
     @abc.abstractmethod
-    def create_repo(self, repoid: str, **kwargs) -> None:
+    def create_repo(self, repoid: str, **kwargs: Any) -> None:
         """
         Add a Repo object to the repo sack and configure it.
-        :param kwargs: key-values options that should be set on the Repo object
-                       values (like $basearch) will be substituted automatically.
+
+        Args:
+            repoid:
+                Repository ID
+            kwargs:
+                key-values options that should be set on the Repo object values
+                (like $basearch) will be substituted automatically.
         """
         ...
 
     @property
     @abc.abstractmethod
-    def backend(self) -> BackendMod:
-        ...
+    def backend(self) -> BackendMod: ...
 
     @abc.abstractmethod
-    def repolist(self, enabled: bool | None = None) -> list[str]:
-        ...
+    def repolist(self, enabled: bool | None = None) -> list[str]: ...
 
     @abc.abstractmethod
     def enable_source_repos(self) -> None:
         """
         Enable the corresponding -source repos of the currently enabled
         repositories
         """
         ...
 
 
-class RepoqueryBase(abc.ABC):
+class NEVRAFormsCompat(Protocol):
+    NEVRA: int
+    NEVR: int
+    NEV: int
+    NA: int
+    NAME: int
+
+
+class RepoqueryBase(metaclass=abc.ABCMeta):
     """
     Helpers to query a repository.
     Provides a unified repoquery interface for different backends.
     """
 
     def __init__(self, base) -> None:
         self.base = base
@@ -400,34 +407,58 @@
     @abc.abstractmethod
     def base_arches(self) -> set[str]:
         """
         Return a set of the system's arch and basearch.
         """
         ...
 
+    def _get_resolve_options(
+        self,
+        resolve: bool,
+        with_filenames: bool | None,
+        with_provides: bool | None,
+        resolve_provides: bool | None,
+    ) -> dict[str, Any]:
+        opts: dict[str, bool | None] = {
+            "with_filenames": with_filenames,
+            "with_provides": with_provides,
+            "resolve_provides": resolve_provides,
+        }
+        return {key: resolve if opt is None else opt for key, opt in opts.items()}
+
     @abc.abstractmethod
     def resolve_pkg_specs(
         self,
         specs: Collection[str],
         resolve: bool = False,
         latest: int | None = None,
         with_src: bool = True,
+        *,
+        with_filenames: bool | None = None,
+        with_provides: bool | None = None,
+        resolve_provides: bool | None = None,
     ) -> PackageQueryCompat:
         """
         Resolve pkg specs.
         See
         https://dnf.readthedocs.io/en/latest/command_ref.html?highlight=spec#specifying-packages
         or
         https://dnf5.readthedocs.io/en/latest/misc/specs.7.html
         for valid forms.
 
-        :param specs: Package specs to resolve.
-        :param resolve: Whether to resolve file paths or virtual Provides in
-                        addition to package specs
-        :param latest: Limit packages with the same name and arch.
+        Args:
+            specs:
+                Package specs to resolve.
+            resolve:
+                Whether to resolve file paths or virtual Provides in addition
+                to package specs
+            latest:
+                Limit packages with the same name and arch.
+            with_src:
+                Whether to consider `.src` packages when resolving `specs`
         """
         ...
 
     def arch_filterm(
         self, query: PackageQueryCompat, arch: str | Iterable[str] | None = None
     ) -> PackageQueryCompat:
         """
@@ -513,15 +544,17 @@
     def get_subpackages(
         self, packages: Iterable[PackageCompat], **kwargs
     ) -> PackageQueryCompat:
         """
         Return a PackageQuery containing the binary RPMS/subpackages produced
         by {packages}.
 
-        :param package: A :class:`PackageQueryCompat` containing source packages
+        Args:
+            packages:
+                An interable of `PackageCompat` containing source packages
         """
         arch = kwargs.get("arch")
         if arch == "src":
             raise ValueError("{arch} cannot be 'src'")
         elif not arch:
             kwargs.setdefault("arch__neq", "src")
         if val := kwargs.pop("sourcerpm", None):
@@ -536,26 +569,53 @@
             for package in packages
         ]
         query = self.query(sourcerpm=sourcerpms, **kwargs)
         return query
 
     @property
     @abc.abstractmethod
-    def backend(self) -> BackendMod:
+    def backend(self) -> BackendMod: ...
+
+
+@dataclasses.dataclass(frozen=True)
+class ChangelogEntry:
+    """
+    Data class for changelog entry data.
+    Do not instantiate directly!
+    """
+
+    text: str
+    author: str
+    date: date
+
+    def __str__(self) -> str:
+        date_str = format(self.date, "%a %b %d %Y")
+        return f"* {date_str} {self.author}\n{self.text}"
+
+
+class _get_changelogs(Protocol):
+    def __call__(self, package: Any) -> Iterator[ChangelogEntry]:
+        """
+        Args:
+            package:
+                A backend's Package object
+        """
         ...
 
 
 class BackendMod(Protocol):
     """
     Protocol for a fedrq backend module.
     Each backend module (e.g.
     [`fedrq.backends.dnf.backend`][fedrq.backends.dnf.backend])
     implements this interface.
     """
 
     BACKEND: str
     BaseMaker: type[BaseMakerBase]
     Package: type[PackageCompat]
+    NEVRAForms: type[NEVRAFormsCompat]
     PackageQuery: type[PackageQueryCompat]
     Repoquery: type[RepoqueryBase]
     RepoError: type[BaseException]
     get_releasever: Callable[[], str]
+    get_changelogs: _get_changelogs
```

### Comparing `fedrq-0.9.0/src/fedrq/backends/dnf/__init__.py` & `fedrq-1.0.0/src/fedrq/backends/dnf/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/backends/dnf/backend.py` & `fedrq-1.0.0/src/fedrq/backends/dnf/backend/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 """
 
 from __future__ import annotations
 
 import logging
 import sys
 import typing as t
-from collections.abc import Collection
+from collections.abc import Collection, Iterator
+from enum import Enum
 from functools import cache
 
 from fedrq._utils import filter_latest
 from fedrq.backends import MissingBackendError
 from fedrq.backends.base import (
     BackendMod,
     BaseMakerBase,
+    ChangelogEntry,
     PackageCompat,
     PackageQueryCompat,
     RepoqueryBase,
 )
 from fedrq.backends.dnf import BACKEND
 
 try:
@@ -56,17 +58,33 @@
         return self.base.conf
 
     def set(self, key: str, value: t.Any) -> None:
         setattr(self.conf, key, value)
 
     def set_var(self, key: str, value: t.Any) -> None:
         if key not in self.base.conf.substitutions:
-            raise KeyError(f"{key} is not a valid substituion")
+            raise KeyError(f"{key} is not a valid substitution")
         self.set(key, value)
 
+    def load_filelists(self, enable: bool = True) -> None:
+        # Old versions of dnf always load filelists
+        try:
+            types: list[str] = self.conf.optional_metadata_types
+        except AttributeError:
+            return
+        if enable:
+            types.append("filelists")
+            return
+        while "filelists" in types:
+            types.remove("filelists")
+
+    def load_changelogs(self, enable: bool = True) -> None:
+        for repo in self.base.repos.iter_enabled():
+            repo.load_metadata_other = enable
+
     def fill_sack(
         self,
         *,
         from_cache: bool = False,
         load_system_repo: bool = False,
     ) -> dnf.Base:
         """
@@ -141,19 +159,22 @@
             else:
                 LOG.debug("Adding %s from %s", repo.id, file)
                 self.base.repos.add(repo)
             if ensure_enabled:
                 LOG.debug("Ensuring that %s is enabled.", repo.id)
                 self.base.repos[repo.id].enable()
 
-    def create_repo(self, repoid: str, **kwargs) -> None:
+    def create_repo(self, repoid: str, **kwargs: t.Any) -> None:
         """
         Add a Repo object to the repo sack and configure it.
-        :param kwargs: key-values options that should be set on the Repo object
-                       values (like $basearch) will be substituted automatically.
+
+        Args:
+            kwargs:
+                key-values options that should be set on the Repo object values
+                (like `$basearch`) will be substituted automatically.
         """
         self.base.repos.add_new_repo(repoid, self.conf, **kwargs)
 
     @property
     def backend(self) -> BackendMod:
         return sys.modules[__name__]
 
@@ -162,14 +183,22 @@
             return list(self.base.repos)
         return [r.id for r in self.base.repos.values() if r.enabled is bool(enabled)]
 
     def enable_source_repos(self) -> None:
         self.base.repos.enable_source_repos()
 
 
+class NEVRAForms(int, Enum):
+    NEVRA = hawkey.FORM_NEVRA
+    NEVR = hawkey.FORM_NEVR
+    NEV = hawkey.FORM_NEV
+    NA = hawkey.FORM_NA
+    NAME = hawkey.FORM_NAME
+
+
 class Repoquery(RepoqueryBase):
     def __init__(self, base: dnf.Base) -> None:
         self.base: dnf.Base = base
 
     @property
     def base_arches(self) -> set[str]:
         return {self.base.conf.arch, self.base.conf.basearch}
@@ -179,28 +208,33 @@
 
     def resolve_pkg_specs(
         self,
         specs: Collection[str],
         resolve: bool = False,
         latest: int | None = None,
         with_src: bool = True,
+        *,
+        with_filenames: bool | None = None,
+        with_provides: bool | None = None,
+        resolve_provides: bool | None = None,
+        nevra_forms: list[NEVRAForms] | None = None,
     ) -> dnf.query.Query:
-        ...
-        LOG.debug(f"specs={specs}, resolve={resolve}, latest={latest}")
+        opts = self._get_resolve_options(
+            resolve, with_filenames, with_provides, resolve_provides
+        )
+        resolve_provides = opts.pop("resolve_provides")
+        opts["with_src"] = with_src
+        if nevra_forms:
+            opts["forms"] = nevra_forms
+
         query = self.query(empty=True)
         for p in specs:
-            subject = dnf.subject.Subject(p).get_best_query(
-                self.base.sack,
-                with_provides=resolve,
-                with_filenames=resolve,
-                with_src=with_src,
-            )
+            subject = dnf.subject.Subject(p).get_best_query(self.base.sack, **opts)
             query = query.union(subject)
-            # LOG.debug(f"subject query: {tuple(subject)}")
-        if resolve:
+        if resolve_provides:
             query = query.union(self.query(provides=specs))
         filter_latest(query, latest)
         return query
 
     @property
     def backend(self) -> BackendMod:
         return sys.modules[__name__]
@@ -214,19 +248,29 @@
     return dnf.rpm.detect_releasever("/")
 
 
 Package: PackageCompat = dnf.package.Package
 PackageQuery: PackageQueryCompat = dnf.query.Query
 RepoError = dnf.exceptions.RepoError
 
+
+def get_changelogs(package: t.Any) -> Iterator[ChangelogEntry]:
+    for entry in package.changelogs:
+        yield ChangelogEntry(
+            text=entry["text"], author=entry["author"], date=entry["timestamp"]
+        )
+
+
 __all__ = (
     "BACKEND",
     "BaseMaker",
     "Package",
+    "NEVRAForms",
     "PackageQuery",
     "RepoError",
     "Repoquery",
     "get_releasever",
+    "get_changelogs",
     #
     "dnf",
     "hawkey",
 )
```

### Comparing `fedrq-0.9.0/src/fedrq/backends/libdnf5/__init__.py` & `fedrq-1.0.0/src/fedrq/backends/libdnf5/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,15 @@
 import importlib.util
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from types import ModuleType
 
 BACKEND = "libdnf5"
-NEEDS = (
-    "libdnf5",
-    # Remove when https://github.com/rpm-software-management/dnf5/issues/281 is
-    # resolved
-    "rpm",
-)
+NEEDS = ("libdnf5",)
 
 
 def ensure_backend() -> None:
     from fedrq.backends import MissingBackendError
 
     needs = ", ".join(NEEDS)
     for req in NEEDS:
```

### Comparing `fedrq-0.9.0/src/fedrq/backends/libdnf5/backend.py` & `fedrq-1.0.0/src/fedrq/backends/libdnf5/backend/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 [`fedrq.backends.base.BackendMod`][fedrq.backends.base.BackendMod] interface)
 that uses the libdnf5 Python bindings.
 """
 
 from __future__ import annotations
 
 import functools
-import inspect
 import logging
 import sys
 import typing as t
 import warnings
-from collections.abc import Collection, Iterable
+from collections.abc import Collection, Iterable, Iterator
+from datetime import datetime as DT
+from datetime import timezone as TZ
+from enum import Enum
 from os.path import join as path_join
 from urllib.parse import urlparse
 
 from fedrq._utils import filter_latest
 from fedrq.backends import MissingBackendError
-from fedrq.backends.base import BackendMod, BaseMakerBase, RepoqueryBase
+from fedrq.backends.base import BackendMod, BaseMakerBase, ChangelogEntry, RepoqueryBase
 from fedrq.backends.libdnf5 import BACKEND  # noqa: F401
 
 if t.TYPE_CHECKING:
     from _typeshed import StrPath
     from typing_extensions import TypeAlias, Unpack
 
 
 try:
     import libdnf5
-    import rpm
 except ImportError as exc:
     raise MissingBackendError(str(exc)) from None
 
 LOG = logging.getLogger(__name__)
 Priority_RUNTIME = libdnf5.conf.Option.Priority_RUNTIME
 StrIter = t.Union[list[str], tuple[str], str]
 IntIter = t.Union[list[int], tuple[int], int]
 CONVERT_TO_LIST = (str, int)
-MINIMUM_NOT_DEPRECATED_VERSION = "5.0.10"
 
 
 class _QueryFilterKwargs(t.TypedDict, total=False):
     name: t.Union[StrIter, libdnf5.rpm.PackageSet]
     name__eq: t.Union[StrIter, libdnf5.rpm.PackageSet]
     name__neq: t.Union[StrIter, libdnf5.rpm.PackageSet]
     name__glob: StrIter
@@ -165,44 +165,19 @@
     reponame__contains: StrIter
 
     pkg: Iterable[libdnf5.rpm.Package]
     pkg__eq: Iterable[libdnf5.rpm.Package]
     pkg__neq: Iterable[libdnf5.rpm.Package]
 
 
-@functools.cache
-def _deprecation_warn() -> None:  # pragma: no cover
-    """
-    Warn that libdnf5 versions < MINIMUM_NOT_DEPRECATED_VERSION are deprecated.
-    This is memoized so we only warn users once.
-    """
-    warnings.warn(
-        f"Support for libdnf5 versions < {MINIMUM_NOT_DEPRECATED_VERSION}"
-        " is deprecated.",
-        stacklevel=2,
-    )
-
-
 def _get_option(config: libdnf5.conf.Config, key: str) -> libdnf5.conf.Option:
     """
     Get an Option object from a libdnf5 Config object.
-    Maintains compatability with dnf5 versions before
-    https://github.com/rpm-software-management/dnf5/pull/327
     """
-    LOG.debug("Getting option %s", key)
-    # dnf5 >= 5.0.8
-    if option := getattr(config, f"get_{key}_option", None):
-        LOG.debug(f"option = get_{key}_option")
-        return option()
-    # dnf5 <= 5.0.7
-    elif option := getattr(config, key, None):  # pragma: no cover
-        _deprecation_warn()
-        return option()
-    else:
-        raise ValueError(f"{key!r} is not a valid option.")
+    return getattr(config, f"get_{key}_option")()
 
 
 class BaseMaker(BaseMakerBase):
     """
     Create a Base object and load repos
     """
 
@@ -213,34 +188,50 @@
         base: libdnf5.base.Base | None = None,
         *,
         initialized: bool = False,
         config_loaded: bool = False,
     ) -> None:
         """
         Initialize and configure the base object.
-        :param base: Pass in a :class:`libdnf.base.Base object` to configure
-        instead of creating a new one.
-        :param initialized: Set to True if base.setup() has already been
-        called. Only applies when `base` is passed.
-        :param config_loaded: Set to True if base.load_config_from_file()
-        has already been called. Only applies when `base` is passed.
+
+        Args:
+            base:
+                Pass in a [`libdnf.base.Base`][libdnf5.base.Base] object to
+                configure instead of creating a new one.
+            initialized:
+                Set to True if `base.setup()` has already been called. Only
+                applies when `base` is passed.
+            config_loaded:
+                Set to True if base.load_config_from_file() has already been
+                called. Only applies when `base` is passed.
         """
         self.base = base or libdnf5.base.Base()
         self.initialized = initialized if base else False
         if not base or not config_loaded:
             self.base.load_config_from_file()
 
     def setup(self) -> None:
         if not self.initialized:
             self.base.setup()
             self.initialized = True
 
+    @property
+    def conf(self) -> libdnf5.config.ConfigMain:
+        return self.base.get_config()
+
     # Not part of the BaseMakerBase interface
     @property
     def config(self) -> libdnf5.config.ConfigMain:
+        """
+        **DEPRECATED: use `conf` property instead**
+        """
+        warnings.warn(
+            "The `config` property is deprecated. Use `conf` instead.",
+            DeprecationWarning,
+        )
         return self.base.get_config()
 
     # Not part of the BaseMakerBase interface
     @property
     def vars(self) -> libdnf5.conf.Vars:
         return self.base.get_vars()
 
@@ -248,15 +239,15 @@
     def _set(self, config, key: str, value: t.Any) -> None:
         self._get_option(config, key).set(Priority_RUNTIME, value)
 
     def set(self, key: str, value: t.Any) -> None:
         # if self.initialized:
         #     raise RuntimeError("The base object has already been initialized")
         LOG.debug("Setting config option %s=%r", key, value)
-        self._set(self.config, key, value)
+        self._set(self.conf, key, value)
 
     def set_var(self, key: str, value: t.Any) -> None:
         self.vars.set(key, value)
 
     # Not part of the BaseMakerBase interface
     @property
     def rs(self) -> libdnf5.repo.RepoSackWeakPtr:
@@ -365,43 +356,55 @@
                     expanded_id,
                     # base.get_vars() returns a WeakPtr, hence the .get()
                     self.base.get_vars().get(),
                     # base.get_logger() returns a WeakPtr, hence the .get()
                     self.base.get_logger().get(),
                     Priority_RUNTIME,
                 )
-                nameop = self._get_option(repo_config, "name")
+                nameop = repo_config.get_name_option()
                 if nameop.get_priority() == libdnf5.conf.Option.Priority_DEFAULT:
                     nameop.set(Priority_RUNTIME, expanded_id)
             if ensure_enabled:
                 repo.enable()
 
     def _get_repo(self, name: str) -> libdnf5.repo.Repo | None:
         """
         Get a repository. Returns None if the repository doesn't exist.
         """
         repoq = libdnf5.repo.RepoQuery(self.base)
         repoq.filter_id([name])
         return next(iter(repoq), None)
 
-    def load_filelists(self) -> None:
-        LOG.debug("Loading filelists")
-        option = self._get_option(self.config, "optional_metadata_types")
-        func = option.add_item
-        # https://github.com/rpm-software-management/dnf5/commit/ba011ff
-        if "priority" in inspect.signature(func).parameters:
-            func(Priority_RUNTIME, libdnf5.conf.METADATA_TYPE_FILELISTS)
-        else:
-            func(libdnf5.conf.METADATA_TYPE_FILELISTS)
+    def _add_metadata_type(self, metadata: t.Any, enable: bool) -> None:
+        if not enable:
+            return self._del_metadata_type(metadata)
+        LOG.debug("Loading %s metadata", metadata)
+        option = self.conf.get_optional_metadata_types_option()
+        option.add_item(Priority_RUNTIME, metadata)
+
+    def _del_metadata_type(self, metadata: t.Any) -> None:
+        LOG.debug("Disabling loading of %s metadata", metadata)
+        types: tuple[t.Any] = self.conf.optional_metadata_types
+        if metadata in types:
+            self.conf.optional_metadata_types = tuple({*types} - {metadata})
+
+    def load_filelists(self, enable: bool = True) -> None:
+        self._add_metadata_type(libdnf5.conf.METADATA_TYPE_FILELISTS, enable)
+
+    def load_changelogs(self, enable: bool = True) -> None:
+        self._add_metadata_type(libdnf5.conf.METADATA_TYPE_OTHER, enable)
 
-    def create_repo(self, repoid: str, **kwargs) -> None:
+    def create_repo(self, repoid: str, **kwargs: t.Any) -> None:
         """
         Add a Repo object to the repo sack and configure it.
-        :param kwargs: key-values options that should be set on the Repo object
-                       values (like $basearch) will be substituted automatically.
+
+        Args:
+            kwargs:
+                key-values options that should be set on the Repo object values
+                (like $basearch) will be substituted automatically.
         """
         repo = self.rs.create_repo(repoid)
         config = repo.get_config()
         for key, value in kwargs.items():
             value = self._substitute(value)
             self._set(config, key, value)
 
@@ -500,43 +503,26 @@
 
     @property
     def evr(self) -> str:
         return self.get_evr()
 
     @property
     def debug_name(self) -> str:
-        # Taken from dnf.package.Package
-        # Copyright (C) 2012-2016 Red Hat, Inc.
-        # SPDX-License-Identifier: GPL-2.0-or-later
-        """
-        Returns name of the debuginfo package for this package.
-        If this package is a debuginfo package, returns its name.
-        If this package is a debugsource package, returns the debuginfo package
-        for the base package.
-        e.g. kernel-PAE -> kernel-PAE-debuginfo
-        """
-        if self.name.endswith(self.DEBUGINFO_SUFFIX):
-            return self.name
-
-        name = self.name
-        if self.name.endswith(self.DEBUGSOURCE_SUFFIX):
-            name = name[: -len(self.DEBUGSOURCE_SUFFIX)]
-
-        return name + self.DEBUGINFO_SUFFIX
+        return self.get_debuginfo_name()
 
     @property
     def source_name(self) -> t.Optional[str]:
         # def source_name(self) -> str:
         return None if self.arch == "src" else self.get_source_name()
         # return self.get_source_name()
 
     @property
     def source_debug_name(self) -> str:
-        source_name = self.name if self.arch == "src" else self.source_name
-        return source_name + self.DEBUGSOURCE_SUFFIX  # type: ignore[operator]
+        # https://github.com/rpm-software-management/dnf5/commit/477d7e5c818c3e95b0e824f8b02d744da7b39a45
+        return self.get_debugsource_name()
 
     @property
     def installtime(self) -> int:
         return self.get_install_time()
 
     @property
     def buildtime(self) -> int:
@@ -544,19 +530,15 @@
 
     @property
     def size(self) -> int:
         return self.downloadsize
 
     @property
     def downloadsize(self) -> int:
-        # https://github.com/rpm-software-management/dnf5/pull/558
-        try:
-            return self.get_download_size()
-        except AttributeError:
-            return self.get_package_size()
+        return self.get_download_size()
 
     @property
     def installsize(self) -> int:
         return self.get_install_size()
 
     @property
     def provides(self) -> Iterable[Reldep5]:
@@ -636,25 +618,26 @@
     def packager(self) -> str:
         return self.get_packager()
 
     @property
     def location(self) -> str:
         return self.get_location()
 
+    @property
+    def repo(self) -> libdnf5.repo.RepoWeakPtr:
+        return self.get_repo()
+
     def remote_location(
         self, schemes: Collection[str] | None = ("http", "ftp", "file", "https")
     ) -> str | None:
         location = self.location
         if not location:  # pragma: no cover
             return None
-        repo_obj: libdnf5.repo.RepoWeakPtr = self.get_repo()
-        mirrors = (
-            repo_obj.get_mirrors()
-            or _get_option(repo_obj.get_config(), "baseurl").get_value()
-        )
+        repo_obj = self.repo
+        mirrors = repo_obj.get_mirrors() or repo_obj.get_config().baseurl
         if not mirrors:  # pragma: no cover
             return None
 
         for url in mirrors:
             if not schemes:
                 return path_join(url, location)
             scheme = urlparse(url).scheme
@@ -764,15 +747,15 @@
         pkgs: Iterable[libdnf5.rpm.Package],
         comp: _pkg_comps = libdnf5.common.QueryCmp_EQ,
         /,
     ):
         if isinstance(pkgs, (libdnf5.rpm.PackageSet, libdnf5.rpm.PackageQuery)):
             newquery = pkgs
         else:
-            if hasattr(self, "__rq__"):
+            if hasattr(self, "__rq__"):  # noqa SIM108
                 base = self.__rq__.base
             else:
                 base = self.get_base()
             newquery = libdnf5.rpm.PackageSet(base)
             newquery.clear()
             for p in pkgs:
                 newquery.add(p)
@@ -814,14 +797,22 @@
                 if issubclass(origin, list) and isinstance(value, sargs[0]):
                     return [value]
         if isinstance(value, sargs[0]):
             return [value]
     return value
 
 
+class NEVRAForms(int, Enum):
+    NEVRA = libdnf5.rpm.Nevra.Form_NEVRA
+    NEVR = libdnf5.rpm.Nevra.Form_NEVR
+    NEV = libdnf5.rpm.Nevra.Form_NEV
+    NA = libdnf5.rpm.Nevra.Form_NA
+    NAME = libdnf5.rpm.Nevra.Form_NAME
+
+
 class Repoquery(RepoqueryBase):
     def __init__(self, base: libdnf5.base.Base) -> None:
         self.base: libdnf5.base.Base = base
 
     @property
     def base_arches(self) -> set[str]:
         base_vars = self.base.get_vars()
@@ -839,104 +830,71 @@
 
     def resolve_pkg_specs(
         self,
         specs: Collection[str],
         resolve: bool = False,
         latest: int | None = None,
         with_src: bool = True,
+        *,
+        with_filenames: bool | None = None,
+        with_provides: bool | None = None,
+        resolve_provides: bool | None = None,
+        nevra_forms: list[NEVRAForms] | None = None,
     ) -> PackageQuery:
+        opts = self._get_resolve_options(
+            resolve, with_filenames, with_provides, resolve_provides
+        )
         settings = libdnf5.base.ResolveSpecSettings()
-        settings.with_filenames = resolve
-        settings.with_provides = resolve
+        settings.with_filenames = opts["with_filenames"]
+        settings.with_provides = opts["with_provides"]
+        if nevra_forms:
+            for form in nevra_forms:
+                settings.nevra_forms.append(form)
 
         r_query = self.query(empty=True)
         for spec in specs:
             query = self._query()
             query.resolve_pkg_spec(spec, settings, with_src)
             r_query.union(query)
-        if resolve:
+        if opts["resolve_provides"]:
             r_query = r_query.union(self.query(provides=specs))
         filter_latest(r_query, latest)
         return r_query
 
     @property
     def backend(self) -> BackendMod:
         return sys.modules[__name__]
 
 
-def _dnf_getreleasever() -> str:  # pragma: no cover
-    # This is taken from dnf and slightly modified
-    #
-    # SPDX-License-Identifier: GPL-2.0-or-later
-    # Copyright (C) 2012-2015  Red Hat, Inc.
-    DISTROVERPKG = (
-        "system-release(releasever)",
-        "system-release",
-        "distribution-release(releasever)",
-        "distribution-release",
-        "redhat-release",
-        "suse-release",
-    )
-    ts = rpm.TransactionSet("/")
-    ts.setVSFlags(~(rpm._RPMVSF_NOSIGNATURES | rpm._RPMVSF_NODIGESTS))
-    for distroverpkg in map(lambda p: p.encode("utf-8"), DISTROVERPKG):
-        idx = ts.dbMatch("provides", distroverpkg)
-        if not len(idx):
-            continue
-        try:
-            hdr = next(idx)
-        except StopIteration:
-            raise RuntimeError(
-                "Error: rpmdb failed to list provides. Try: rpm --rebuilddb"
-            ) from None
-        releasever = hdr["version"]
-        try:
-            try:
-                # header returns bytes -> look for bytes
-                # it may fail because rpm returns a decoded string since 10 Apr 2019
-                off = hdr[rpm.RPMTAG_PROVIDENAME].index(distroverpkg)
-            except ValueError:
-                # header returns a string -> look for a string
-                off = hdr[rpm.RPMTAG_PROVIDENAME].index(distroverpkg.decode("utf8"))
-            flag = hdr[rpm.RPMTAG_PROVIDEFLAGS][off]
-            ver = hdr[rpm.RPMTAG_PROVIDEVERSION][off]
-            if flag == rpm.RPMSENSE_EQUAL and ver:
-                if hdr["name"] not in (distroverpkg, distroverpkg.decode("utf8")):
-                    # override the package version
-                    releasever = ver
-        except (ValueError, KeyError, IndexError):
-            pass
-        if isinstance(releasever, bytes):
-            releasever = releasever.decode("utf-8")
-        return releasever
-    return ""
-
-
 @functools.cache
 def get_releasever() -> str:
     """
     Return the system releasever
     """
     # libdnf5 >= 5.0.10
     # https://github.com/rpm-software-management/dnf5/pull/448
-    if hasattr(libdnf5.conf.Vars, "detect_release"):
-        base = libdnf5.base.Base()
-        return libdnf5.conf.Vars.detect_release(base.get_weak_ptr(), "/").get()
-    # Fall back to our copy of dnf4's code
-    else:  # pragma: no cover
-        _deprecation_warn()
-        return _dnf_getreleasever()
+    base = libdnf5.base.Base()
+    return libdnf5.conf.Vars.detect_release(base.get_weak_ptr(), "/").get()
+
+
+def get_changelogs(package: Package) -> Iterator[ChangelogEntry]:
+    entries = package.get_changelogs()
+    for entry in entries:
+        date_obj = DT.fromtimestamp(entry.timestamp, tz=TZ.utc).date()
+        yield ChangelogEntry(text=entry.text, author=entry.author, date=date_obj)
 
 
 RepoError = RuntimeError
 
 __all__ = (
     "BACKEND",
     "BaseMaker",
     "Package",
+    "NEVRAForms",
     "PackageQuery",
     "Repoquery",
     "RepoError",
     "get_releasever",
+    "get_changelogs",
     #
     "libdnf5",
 )
```

### Comparing `fedrq-0.9.0/src/fedrq/cli/__init__.py` & `fedrq-1.0.0/src/fedrq/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     import argcomplete
 except ImportError:
     HAS_ARGCOMPLETE = False
 else:
     HAS_ARGCOMPLETE = True
 
 from fedrq.cli.base import CheckConfig, Command
+from fedrq.cli.commands.cache import MakeCacheCommand
+from fedrq.cli.commands.changelogs import ChangelogCommand
 from fedrq.cli.commands.download import DownloadCommand, DownloadSpecCommand
+from fedrq.cli.commands.formatters import FormattersCommand
 from fedrq.cli.commands.pkgs import Pkgs
 from fedrq.cli.commands.repolist import Repolist
 from fedrq.cli.commands.subpkgs import Subpkgs
 from fedrq.cli.commands.whatrequires import (
     WhatCommand,
     Whatenhances,
     Whatobsoletes,
@@ -31,16 +34,19 @@
 )
 
 __all__ = (
     "Command",
     "Pkgs",
     "Repolist",
     "Subpkgs",
+    "ChangelogCommand",
     "DownloadCommand",
     "DownloadSpecCommand",
+    "FormattersCommand",
+    "MakeCacheCommand",
     "WhatCommand",
     "Whatenhances",
     "Whatobsoletes",
     "Whatrecommends",
     "Whatrequires",
     "WhatrequiresSrc",
     "Whatsuggests",
@@ -68,17 +74,20 @@
     if HAS_ARGCOMPLETE:
         argcomplete.autocomplete(parser)
     args = parser.parse_args(argv)
     return COMMANDS[args.action](args).run()
 
 
 COMMANDS: dict[str, type[Command]] = {
+    "make-cache": MakeCacheCommand,
     "check-config": CheckConfig,
+    "changelog": ChangelogCommand,
     "download": DownloadCommand,
     "download-spec": DownloadSpecCommand,
+    "formatters": FormattersCommand,
     "pkgs": Pkgs,
     "subpkgs": Subpkgs,
     "repolist": Repolist,
     "whatenhances": Whatenhances,
     "whatobsoletes": Whatobsoletes,
     "whatrecommends": Whatrecommends,
     "whatrequires": Whatrequires,
```

### Comparing `fedrq-0.9.0/src/fedrq/cli/base.py` & `fedrq-1.0.0/src/fedrq/cli/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import logging
 import re
 import sys
 from functools import wraps
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
-from fedrq.backends.base import BaseMakerBase
+from fedrq.backends.base import BaseMakerBase, PackageCompat
 
 try:
     import tomli_w
 except ImportError:
     HAS_TOMLI_W = False
 else:
     HAS_TOMLI_W = True
@@ -103,29 +103,30 @@
         for err in fatal:
             print("FATAL ERROR:", err, file=sys.stderr)
         sys.exit(1)
 
     return wrapper
 
 
-class Command(abc.ABC):
+class Command(metaclass=abc.ABCMeta):
     config: RQConfig
     release: Release
     query: PackageQueryCompat
     formatters: Formatters = DefaultFormatters
     formatter: Formatter
 
     def __init__(self, args: argparse.Namespace):
         self.args = args
 
         self.v_logging()
         flog = mklog(__name__, self.__class__.__name__)
         flog.debug("args=%s", args)
 
-        self.get_names()
+        if hasattr(self.args, "names"):
+            self.get_names()
 
         try:
             self.config = self._get_config()
         except ValidationError as exc:
             sys.exit(str(exc))
         self._set_config("backend")
         self._set_config("smartcache")
@@ -144,16 +145,15 @@
         return get_config()
 
     @property
     def backend(self) -> BackendMod:
         return self.config.backend_mod
 
     @abc.abstractmethod
-    def run(self) -> None:
-        ...
+    def run(self) -> None: ...
 
     def _set_config(self, key: str) -> None:
         arg = getattr(self.args, key, None)
         if arg is not None:
             setattr(self.config, key, arg)
 
     def _logq(
@@ -248,30 +248,41 @@
         parser = argparse.ArgumentParser(add_help=False)
         run_parser = parser.add_mutually_exclusive_group()
         run_parser.add_argument("-y", "--assumeyes", action="store_true")
         run_parser.add_argument("-n", "--dry-run", action="store_true")
         return parser
 
     @classmethod
-    def parent_parser(cls) -> argparse.ArgumentParser:
+    def parent_parser(
+        cls, *, formatter: bool = True, latest: bool = True, name=True
+    ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             add_help=False, parents=[cls.branch_repo_parser()]
         )
-        parser.add_argument(  # type: ignore[attr-defined]
-            "names", metavar="NAME", nargs="*", help="Mutually exclusive with --stdin"
-        ).completer = lambda **_: ()
-        parser.add_argument(
-            "-i", "--stdin", help="Read package names from stdin.", action="store_true"
-        )
-        parser.add_argument("-l", "--latest", default=1, help="'all' or an integer")
-        parser.add_argument(  # type: ignore[attr-defined]
-            "-F",
-            "--formatter",
-            default="plain",
-        ).completer = cls.formatters._argcompleter
+        if name:
+            parser.add_argument(  # type: ignore[attr-defined]
+                "names",
+                metavar="NAME",
+                nargs="*",
+                help="Mutually exclusive with --stdin",
+            ).completer = lambda **_: ()
+            parser.add_argument(
+                "-i",
+                "--stdin",
+                help="Read package names from stdin.",
+                action="store_true",
+            )
+        if latest:
+            parser.add_argument("-l", "--latest", default=1, help="'all' or an integer")
+        if formatter:
+            parser.add_argument(  # type: ignore[attr-defined]
+                "-F",
+                "--formatter",
+                default="plain",
+            ).completer = cls.formatters._argcompleter
         cachedir_group = parser.add_mutually_exclusive_group()
         cachedir_group.add_argument(
             "--system-cache",
             action="store_true",
             help="Use the default dnf cachedir and ignore `smartcache` config option",
         )
         cachedir_group.add_argument(
@@ -280,28 +291,30 @@
             action="store_true",
             default=None,
             dest="smartcache",
             help="See `smartcache` in fedrq(5)."
             " smartcache is enabled by default,"
             " so this is noop unless you set `smartcache=false` in the config file.",
         )
+        cachedir_group.add_argument(
+            "--smartcache-always",
+            action="store_const",
+            dest="smartcache",
+            const="always",
+        )
         # This is mutually exclusive with --smartcache. It's still undocumented
         # and subject to change.
         cachedir_group.add_argument("--cachedir", help=argparse.SUPPRESS, type=Path)
         parser.add_argument("--debug", action="store_true")
         parser.add_argument(
             "-L",
             "--filelists",
             choices=tuple(LoadFilelists),
             dest="load_filelists",
-            help="Whether to load filelists."
-            " By default, filelists are only loaded when using the files formatter."
-            " This only applies when using the libdnf5 backend,"
-            " which doesn't load filelists by default to save memory and bandwidth."
-            " dnf4 always loads filelists.",
+            help="Whether to load filelists",
         )
         parser.add_argument("-B", "--backend", choices=tuple(BACKENDS))
         parser.add_argument(
             "--forcearch", help="Query a foreign architecture's repositories"
         )
         return parser
 
@@ -336,50 +349,58 @@
         if self.args.names and self.args.stdin:
             sys.exit("Postional NAMEs can not be used with --stdin")
         if self.args.stdin:
             self.args.names = [line.strip() for line in sys.stdin.readlines()]
         if not self.args.names:
             sys.exit("No package names were passed")
 
-    def format(self) -> cabc.Iterable[str]:
+    def format(
+        self, query: cabc.Iterable[PackageCompat] | None = None
+    ) -> cabc.Iterable[str]:
         """
         Helper to run `self.formatter.format(self.query)`
         """
-        return self.formatter.format(self.query)
+        self.formatter.rq = self.rq
+        return self.formatter.format(query if query is not None else self.query)
 
     def _v_handle_errors(self, should_exit: bool = True):
         if self._v_errors:
             for line in self._v_errors:
                 print("ERROR:", line, file=sys.stderr)
             if should_exit:
                 sys.exit(1)
 
     def v_logging(self) -> None:
         if getattr(self.args, "debug", None):
             logger.setLevel(logging.DEBUG)
 
     @v_add_errors
     def v_latest(self) -> str | None:
+        if not hasattr(self.args, "latest"):
+            return None
         try:
             self.args.latest = int(self.args.latest)
         except ValueError:
             if isinstance(self.args.latest, str) and self.args.latest.lower() in (
                 "a",
                 "all",
             ):
                 self.args.latest = None
             else:
                 return "--latest must equal 'all' or be an integer"
         return None
 
     @v_add_errors
     def v_formatters(self) -> str | None:
+        if not hasattr(self.args, "formatter"):
+            return None
         try:
             self.formatter = self.formatters.get_formatter(self.args.formatter)
         except FormatterError as err:
+            logger.debug("FormatterError", exc_info=err)
             return str(err) + "\n" + FORMATTER_ERROR_SUFFIX
         return None
 
     @v_add_errors
     def v_arch(self) -> str | None:
         # TODO: Verify that arches are actually valid RPM arches.
         if not self.args.arch:
@@ -417,15 +438,17 @@
         bvars: dict[str, Any] = {}
 
         # Set cachedir if it's explicitly passed
         if self.args.cachedir:
             conf["cachedir"] = str(self.args.cachedir)
         # Disable release based smartcache if user explicitly disabled it or if
         # forcearch is in use.
-        elif self.args.system_cache or self.args.forcearch:
+        elif self.args.system_cache or (
+            self.args.forcearch and self.config.smartcache != "always"
+        ):
             self.config.smartcache = False
 
         if self.args.forcearch:
             conf["ignorearch"] = True
             bvars["arch"] = self.args.forcearch
         bm = self.backend.BaseMaker()
         try:
@@ -451,14 +474,15 @@
 
     def v_default(self) -> None:
         self.v_formatters()
         self.v_latest()
         self.v_arch()
         # Fatal
         self.v_backend()
+        self._v_handle_errors()
         self.v_release()
         self.v_rq()
         self._v_handle_errors()
 
 
 class CheckConfig(Command):
     """
@@ -521,36 +545,7 @@
             sys.exit(f"default_branch '{self.config.default_branch}' is invalid")
         if not self.args.dump:
             print("No validation errors found!")
         else:
             flog.debug("Removing Nones from configuration dict")
             data_dict = self._strip_nones(json.loads(self.config.json()))
             tomli_w.dump(data_dict, sys.stdout.buffer)
-
-
-# class CommandBoilerplate(Command):
-#     """
-#     Help text
-#     """
-#     def __init__(self, args: argparse.Namespace) -> None:
-#         super().__init__(args)
-#         self.v_default()
-
-#     @classmethod
-#     def make_parser(
-#         cls,
-#         parser_func: cabc.Callable = argparse.ArgumentParser,
-#         *,
-#         add_help: bool = False,
-#         **kwargs,
-#     ) -> argparse.ArgumentParser:
-#         kwargs["description"] = cls.__doc__
-#         kwargs["parents"] = [cls.parent_parser()]
-#         if add_help:
-#             kwargs["help"] = cls.__doc__
-
-#         parser = parser_func(**kwargs)
-#         ...
-#         return parser
-
-#     def run(self) -> None:
-#         ...
```

### Comparing `fedrq-0.9.0/src/fedrq/cli/commands/download.py` & `fedrq-1.0.0/src/fedrq/cli/commands/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 """
 download commands
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
 import shutil
 import sys
 from collections.abc import Callable, Iterator
+from contextlib import suppress
 from pathlib import Path
 from tempfile import TemporaryDirectory
+from typing import Any
 
 import requests
 import rpm
 
 from fedrq._archive import RPMArchive
 from fedrq._utils import exhaust_it
 from fedrq.backends.base import PackageCompat
@@ -29,21 +31,37 @@
 def callback_ind(start: int, end: int) -> Callable[[Path], None]:
     def inner(destpath: Path) -> None:
         print(f"Downloading {destpath.name} ({start}/{end})")
 
     return inner
 
 
+def _get_req_kwargs(package: PackageCompat) -> dict[str, Any]:  # pragma: no cover
+    req_kwargs: dict[str, Any] = {}
+    repo_obj = package.repo
+    # libdnf5 has a .get_config() attribute
+    with suppress(AttributeError):
+        repo_obj = repo_obj.get_config()
+    if repo_obj.sslverify is False:
+        repo_obj["verify"] = False
+    elif repo_obj.sslcacert:
+        req_kwargs["verify"] = repo_obj.sslcacert
+    if repo_obj.sslclientcert and repo_obj.sslclientkey:
+        req_kwargs["cert"] = (repo_obj.sslclientcert, repo_obj.sslclientkey)
+    return req_kwargs
+
+
 def download(
     package: PackageCompat,
     destdir: Path,
     callback: Callable[[Path], None] | None = None,
 ) -> Path:
     def _remote_dl(url: str, src: Path, dest: Path) -> None:  # noqa: ARG001
-        req = requests.get(url, allow_redirects=True)
+        req_kwargs = _get_req_kwargs(package)
+        req = requests.get(url, allow_redirects=True, **req_kwargs)
         req.raise_for_status()
         dest.write_bytes(req.content)
 
     def _local_cp(url: str, src: Path, dest: Path) -> None:  # noqa: ARG001
         shutil.copy2(src, dest)
 
     url = package.remote_location()
@@ -66,15 +84,15 @@
         callback(dest)
     mode(url, src, dest)
     return dest
 
 
 class DownloadCommand(Command):
     """
-    EXPERIMENTAL: Download an (S)RPM from the repos.
+    Download an (S)RPM from the repos.
     No gpg checking is preformed.
     """
 
     def __init__(self, args: argparse.Namespace) -> None:
         super().__init__(args)
         self.v_default()
 
@@ -85,15 +103,15 @@
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
         parser = super().make_parser(
             parser_func,
             add_help=add_help,
-            help=cls.__doc__.splitlines()[0],  # type: ignore[union-attr]
+            help=(cls.__doc__ or "").strip().replace("\n", " "),
             parents=[
                 cls.parent_parser(),
                 cls.arch_parser(),
                 cls.resolve_parser(),
                 cls.assume_parser(),
             ],
             **kwargs,
@@ -144,28 +162,29 @@
         if not self._prompt():
             return
         exhaust_it(self._downloadit(self.args.destdir))
 
 
 class DownloadSpecCommand(DownloadCommand):
     """
-    Download an SRPM and extract its specfile
+    Download an SRPM and extract its specfile.
+    No gpg checking is preformed.
     """
 
     @classmethod
     def make_parser(
         cls,
         parser_func: Callable = argparse.ArgumentParser,
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
         parser = super(DownloadCommand, cls).make_parser(
             parser_func,
-            # Never add_help, as this command is EXPERIMENTAL
+            help=(cls.__doc__ or "").strip().replace("\n", " "),
             add_help=add_help,
             parents=[
                 cls.parent_parser(),
                 cls.assume_parser(),
             ],
             **kwargs,
         )
```

### Comparing `fedrq-0.9.0/src/fedrq/cli/commands/pkgs.py` & `fedrq-1.0.0/src/fedrq/cli/commands/pkgs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import argparse
 from collections import abc as cabc
 
-from fedrq._utils import filter_latest, mklog
+from fedrq._utils import filter_latest
 from fedrq.cli import Command
 
 
 class Pkgs(Command):
     """
     Find the packages that match NAMES.
     NAMES can be package package name globs or NEVRs.
@@ -24,40 +24,36 @@
     def make_parser(
         cls,
         parser_func: cabc.Callable = argparse.ArgumentParser,
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
-        kwargs.update(
-            dict(
-                description=Pkgs.__doc__,
-                parents=[cls.parent_parser(), cls.arch_parser(), cls.resolve_parser()],
-            )
+        parser = super().make_parser(
+            parser_func,
+            parents=[cls.parent_parser(), cls.arch_parser(), cls.resolve_parser()],
+            help="Find the packages that match a list of package specs",
+            add_help=add_help,
+            **kwargs,
         )
-        if add_help:
-            kwargs["help"] = "Find the packages that match a list of package specs"
-        parser = parser_func(**kwargs)
 
         return parser
 
     def run(self) -> None:
-        flog = mklog(__name__, self.__class__.__name__, "run")
         self.query = self.rq.query(empty=True)
-        # flog.debug("self.query = %s", tuple(self.query))
 
         resolved_packages = self.rq.resolve_pkg_specs(
             self.args.names, self.args.resolve_packages
         )
         self._logq(resolved_packages, "resolved_packages")
         self.query = self.query.union(resolved_packages)
 
         glob_packages = self.rq.query(name__glob=self.args.names)
         self._logq(glob_packages, "glob_packages")
         self.query = self.query.union(glob_packages)
 
         self.query = self.rq.arch_filter(self.query, self.args.arch)
         filter_latest(self.query, self.args.latest)
-        flog.debug("self.query = %s", tuple(self.query))
+        self._logq(self.query, "self.query")
 
         for p in self.format():
             print(p)
```

### Comparing `fedrq-0.9.0/src/fedrq/cli/commands/repolist.py` & `fedrq-1.0.0/src/fedrq/cli/commands/repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/cli/commands/subpkgs.py` & `fedrq-1.0.0/src/fedrq/cli/commands/subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/cli/commands/whatrequires.py` & `fedrq-1.0.0/src/fedrq/cli/commands/whatrequires.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from fedrq._utils import filter_latest, get_source_name
 from fedrq.backends.base import PackageCompat, PackageQueryCompat
 from fedrq.cli.base import Command
 from fedrq.cli.formatters import DefaultFormatters, Formatter
 
 logger = logging.getLogger(__name__)
 
+_PackageCompatT = t.TypeVar("_PackageCompatT", bound=PackageCompat)
+
 
 class BreakdownFormatter(Formatter):
     MULTILINE = True
 
     def format_line(self, package: PackageCompat) -> str:
         raise NotImplementedError
 
@@ -56,14 +58,16 @@
     formatters = WhatFormatters
     _exclude_subpackages_opt: bool = False
     _operator: str
     operator: str
 
     def __init__(self, args: argparse.Namespace) -> None:
         super().__init__(args)
+        if getattr(self.args, "extra_exact", None):
+            self.args.exact = True
         self.v_default()
 
     @classmethod
     def make_parser(
         cls,
         parser_func: cabc.Callable = argparse.ArgumentParser,
         *,
@@ -90,14 +94,21 @@
         resolve_group.add_argument(
             "-E",
             "--exact",
             action="store_true",
             help="This is the opposite extreme to --resolve-packages. "
             "E.g., yt-dlp would not match python3dist(yt-dlp) like it does by default.",
         )
+        resolve_group.add_argument(
+            "--ee",
+            "--extra-exact",
+            action="store_true",
+            dest="extra_exact",
+            help=argparse.SUPPRESS,
+        )
 
         if cls._exclude_subpackages_opt:
             parser.add_argument("-X", "--exclude-subpackages", action="store_true")
         return parser
 
     def exclude_subpackages(self, rpms: t.Optional[PackageQueryCompat]) -> None:
         import re
@@ -108,15 +119,14 @@
 
         brpm_sourcerpms = [
             re.sub(r"\.rpm$", "", t.cast(str, pkg.sourcerpm)) for pkg in brpms
         ]
         brpm_srpm_query = self.rq.resolve_pkg_specs(brpm_sourcerpms)
         subpackages = self.rq.get_subpackages(brpm_srpm_query.union(srpms))
         self.query.filterm(pkg__neq=subpackages)
-        return None
 
     def run(self) -> None:
         self.query = self.rq.query(empty=True)
         # Resolve self.args.names into Package objs.
         # This makes it so packages that depend on virtual Provides of the
         # names are included.
         if not self.args.exact:
@@ -138,18 +148,36 @@
         filter_latest(self.query, self.args.latest)
 
         if getattr(self.args, "exclude_subpackages", None):
             self.exclude_subpackages(
                 resolved_packages if self.args.resolve_packages else None
             )
 
-        for p in self.format():
+        query: cabc.Iterable[PackageCompat] | None = None
+        if getattr(self.args, "extra_exact", None):
+            query = _extra_exact(self.operator, self.args.names, self.query)
+        for p in self.format(query):
             print(p)
 
 
+def _extra_exact(
+    attr: str,
+    matches: cabc.Collection[str],
+    packages: cabc.Iterable[_PackageCompatT],
+) -> cabc.Iterable[_PackageCompatT]:
+    """
+    Filter factory to ensure exact string matches for whatrequires and whatprovides
+    """
+
+    return filter(
+        lambda package: {str(obj) for obj in getattr(package, attr)} & set(matches),
+        packages,
+    )
+
+
 class Whatrequires(WhatCommand):
     """
     By default, fedrq-whatrequires takes one or more valid package names. Then,
     it finds the packages' reverse dependencies, including dependents of their
     virtual Provides. Use the options below to modify fedrq-whatrequires exact
     search strategy.
     """
@@ -164,15 +192,15 @@
     By default, fedrq-whatrecommends takes one or more valid package names. Then,
     it finds the packages' reverse dependencies, including dependents of their
     virtual Provides. Use the options below to modify fedrq-whatrecommends exact
     search strategy.
     """
 
     _operator = "Recommend"
-    operator = "recommend"
+    operator = "recommends"
     _exclude_subpackages_opt = True
 
 
 class Whatsuggests(WhatCommand):
     """
     By default, fedrq-whatsuggests takes one or more valid package names. Then,
     it finds the packages' reverse dependencies, including dependents of their
```

### Comparing `fedrq-0.9.0/src/fedrq/cli/formatters.py` & `fedrq-1.0.0/src/fedrq/cli/formatters.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import abc
 import argparse
 import logging
-import warnings
-from collections.abc import Callable, ItemsView, Iterable, Iterator, Mapping
+from collections.abc import Callable, Container, ItemsView, Iterable, Iterator, Mapping
 from contextlib import suppress
-from typing import TYPE_CHECKING, Any, NoReturn
+from functools import partial
+from typing import TYPE_CHECKING, Any, ClassVar, NoReturn, cast
 
 from fedrq._utils import get_source_name
+from fedrq.backends.base import RepoqueryBase
 
 if TYPE_CHECKING:
     from fedrq.backends.base import PackageCompat
+else:
+    ellipsis = type(...)
 
 LOG = logging.getLogger(__name__)
 
 
 class FormatterError(Exception):
     pass
 
@@ -61,46 +64,69 @@
     "files",
     "reponame",
     "repoid",
     "vendor",
     "packager",
     "location",
 )
+_MULTILINE_ATTRS = frozenset(
+    {
+        "description",
+        "provides",
+        "requires",
+        "recommends",
+        "suggests",
+        "supplements",
+        "enhances",
+        "obsoletes",
+        "conflicts",
+        "files",
+    }
+)
+_ATTRS_SINGLE: tuple[str, ...] = tuple(set(_ATTRS) - _MULTILINE_ATTRS)
+_DEFAULT_MULTILINE_SEPERATOR = "\n---\n"
 
 
-def _stringify(value: Any, *, multiline_allowed: bool = True) -> str:
+def _stringify(
+    value: Any,
+    *,
+    multiline_allowed: bool = True,
+    multiline_seperator: str = _DEFAULT_MULTILINE_SEPERATOR,
+) -> str:
     if value is None or value == "":
         return "(none)"
     if isinstance(value, str) and "\n" in value:
         if not multiline_allowed:
             raise FormatterError("Multiline values are not allowed")
-        return value + "\n---\n"
+        return value + multiline_seperator
     return str(value)
 
 
-class Formatter(abc.ABC):
+class Formatter(metaclass=abc.ABCMeta):
     ATTRS = _ATTRS
     MULTILINE = False
 
     """
     Convert PackageCompat objects into a string representation
     for use with the fedrq CLI.
     """
 
     def __init__(
         self,
         name: str,
         seperator: str,
         args: str,
         container: Formatters | None = None,
+        repoquery: RepoqueryBase | None = None,
     ) -> None:
         self.name = name
         self.seperator = seperator
         self.args = args
         self.container: Formatters = container or Formatters({})
+        self.rq = repoquery
         self.validate()
 
     @abc.abstractmethod
     def format_line(self, package: PackageCompat) -> str:
         """
         Format a single Package object
         """
@@ -154,14 +180,20 @@
         typ = type(f"{name.upper()}Formatter", (cls,), dct)
         return typ
 
     def __str__(self) -> str:
         return f"{self.name}{self.seperator}{self.args}"
 
 
+def format_line_notimplemented(
+    self: Formatter, package: PackageCompat  # noqa: ARG001
+) -> NoReturn:
+    raise NotImplementedError
+
+
 class Formatters(Mapping[str, type[Formatter]]):
     __slots__ = ("__data", "fallback")
 
     """
     Immutable mapping like class of Formatter classes.
     Converts strings and simple functions to Formatter objects.
     Allows merging and adding other Formatters.
@@ -171,21 +203,30 @@
         self,
         formatters: Mapping[str, Callable | type[Formatter] | str],
         fallback: type[Formatter] | None = None,
     ) -> None:
         self.__data = self._formattersv(dict(formatters))
         self.fallback: type[Formatter] | None = fallback
 
-    def get_formatter(self, key: str) -> Formatter:
+    def get_formatter(
+        self,
+        key: str,
+        fallback: type[Formatter] | None | ellipsis = ...,
+        *,
+        repoquery: RepoqueryBase | None = None,
+    ) -> Formatter:
+        if fallback is ...:
+            fallback = self.fallback
+        fallback = cast("type[Formatter] | None", fallback)
         name, seperator, args = key.partition(":")
         with suppress(KeyError):
-            return self[name](name, seperator, args, self)
-        if self.fallback:
+            return self[name](name, seperator, args, self, repoquery=repoquery)
+        if fallback:
             with suppress(FormatterError):
-                return self.fallback(name, seperator, args, self)
+                return fallback(name, seperator, args, self, repoquery=repoquery)
         raise FormatterError(f"{key!r} is not a valid formatter")
 
     def __getitem__(self, key: str) -> type[Formatter]:
         return self.__data[key]
 
     def __len__(self) -> int:
         return len(self.__data)
@@ -250,21 +291,37 @@
         self,
         *,
         prefix: str,  # noqa: ARG002
         action: argparse.Action,  # noqa: ARG002
         parser: argparse.ArgumentParser,  # noqa: ARG002
         parsed_args: argparse.Namespace,  # noqa: ARG002
     ) -> list[str]:
-        opts: list[str] = [*_ATTRS]
+        return sorted(self.formatters_it())
+
+    def formatters_it(
+        self,
+        attrs: bool = True,
+        formatters: bool = True,
+        special_formatters: bool = True,
+    ) -> Iterator[str]:
+        """
+        Yields:
+            Names of formatters in this container. `SpecialFormatter`s have a
+            `:` appended to their names.
+        """
+        if attrs:
+            yield from _ATTRS
+        if {formatters, special_formatters} == {False}:
+            return
         for name, formatter in self.items():
             if issubclass(formatter, SpecialFormatter):
-                opts.append(f"{name}:")
-            else:
-                opts.append(name)
-        return opts
+                if special_formatters:
+                    yield f"{name}:"
+            elif formatters:
+                yield name
 
 
 class SourceFromatter(Formatter):
     def format(self, packages: Iterable[PackageCompat]) -> Iterable[str]:
         return sorted(set(map(self.format_line, packages)))
 
     def format_line(self, package: PackageCompat) -> str:
@@ -274,30 +331,36 @@
 class SpecialFormatter(Formatter):
     """
     Formatter that accepts arguments
     """
 
     ATTRS: tuple[str, ...] = Formatter.ATTRS
 
-    def _get_attrs(self, args: str) -> Iterator[str | Formatter]:
+    def _get_attrs(
+        self, args: str, allow_multiline: bool = False
+    ) -> Iterator[str | Formatter]:
+        attrs: Container[str] = (
+            self.container if allow_multiline else self.container.singleline()
+        )
         for attr in args.split(","):
             if attr in self.ATTRS:
                 yield attr
-            elif attr in self.container.singleline():
-                yield self.container.get_formatter(attr)
+            elif attr in attrs:
+                yield self.container.get_formatter(attr, repoquery=self.rq)
             else:
                 self.err(f"invalid argument {attr!r}")
 
     def validate(self) -> None:
         if not self.args.strip() or self.args.strip() == ",":
             self.err("received less than 1 argument")
 
 
 class AttrFormatter(SpecialFormatter):
     MULTILINE = True
+    _MULTILINE_SEPERATOR = _DEFAULT_MULTILINE_SEPERATOR
 
     def validate(self) -> None:
         super().validate()
         self._validate()
 
     def _validate(self) -> None:
         if self.args not in self.ATTRS:
@@ -308,27 +371,34 @@
         # Return one string if there's multiple lines
         return "\n".join(self.format([package]))
 
     def format(self, packages: Iterable[PackageCompat]) -> Iterable[str]:
         for p in sorted(packages):
             result = getattr(p, self.attr)
             if isinstance(result, Iterable) and not isinstance(result, str):
-                yield from map(_stringify, result)
+                yield from map(
+                    partial(_stringify, multiline_seperator=self._MULTILINE_SEPERATOR),
+                    result,
+                )
             else:
-                yield _stringify(result)
+                yield _stringify(result, multiline_seperator=self._MULTILINE_SEPERATOR)
 
 
 class AttrFallbackFormatter(AttrFormatter):
     def validate(self) -> None:
         if self.seperator:
             self.err("no arguments are accepted")
         self.args = self.name
         self._validate()
 
 
+class _AttrFallbackFormatterUnseperated(AttrFallbackFormatter):
+    _MULTILINE_SEPERATOR = ""
+
+
 class JsonFormatter(SpecialFormatter):
     MULTILINE = True
 
     def validate(self) -> None:
         super().validate()
         self.attrs: list[Formatter | str] = list(self._get_attrs(self.args))
 
@@ -344,35 +414,21 @@
 
     def format(self, packages: Iterable[PackageCompat]):
         import json
 
         data = [dict(self._format(package)) for package in packages]
         yield json.dumps(data, indent=2)
 
-    def format_line(self, package: PackageCompat):
-        raise NotImplementedError
+    format_line = format_line_notimplemented
 
 
 class SingleLineFormatter(SpecialFormatter):
     DEFAULT_DIVIDER = " : "
-    ATTRS: tuple[str, ...] = tuple(
-        set(SpecialFormatter.ATTRS)
-        - {
-            "description",
-            "provides",
-            "requires",
-            "recommends",
-            "suggests",
-            "supplements",
-            "enhances",
-            "obsoletes",
-            "conflicts",
-            "files",
-        }
-    )
+    ATTRS: tuple[str, ...] = _ATTRS_SINGLE
+    _ALLOW_MULTILINE_ATTRS: bool = False
 
     def validate(self) -> None:
         args, seperator, args2 = self.args.rpartition(":")
         LOG.debug(
             "parsing %s args: %r, %r, %r",
             "SingleLineFormatter.validate",
             args,
@@ -396,56 +452,162 @@
         #                             divider=DEFAULT_DIVIDER
         # line::: -> error
         elif args and seperator and not args2:
             LOG.debug("case 3")
             self.params = args
             self.divider = self.DEFAULT_DIVIDER
         else:
-            raise RuntimeError
-        self.attrs = list(self._get_attrs(self.params))
+            raise AssertionError("unreachable")
+        self.attrs = list(self._get_attrs(self.params, self._ALLOW_MULTILINE_ATTRS))
+
+    def _fl(
+        self,
+        package: PackageCompat,
+        index: int,
+        attr: str | Formatter,
+        divider: str,
+        multiline_allowed=False,
+    ) -> str:
+        out = ""
+        if isinstance(attr, str):
+            out += _stringify(
+                getattr(package, attr), multiline_allowed=multiline_allowed
+            )
+        else:
+            attr.rq = self.rq
+            out += attr.format_line(package)
+        if index != len(self.attrs) - 1:
+            out += divider
+        return out
 
     def format_line(self, package: PackageCompat) -> str:
         out = ""
         for index, attr in enumerate(self.attrs):
-            if isinstance(attr, str):
-                out += _stringify(getattr(package, attr), multiline_allowed=False)
-            else:
-                out += attr.format_line(package)
-            if index != len(self.attrs) - 1:
-                out += self.divider
+            out += self._fl(package, index, attr, self.divider)
         return out
 
 
+class MultilineFormatter(SingleLineFormatter):
+    ATTRS = SpecialFormatter.ATTRS
+    MULTILINE = True
+    _ALLOW_MULTILINE_ATTRS = True
+
+    format_line = format_line_notimplemented
+
+    def validate(self) -> None:
+        super().validate()
+        if len(self.attrs) != 2:
+            self.err("requires two arguments")
+
+    def format(self, packages: Iterable[PackageCompat]) -> Iterator[str]:
+        for package in sorted(packages):
+            initial = self._fl(package, 0, self.attrs[0], self.divider, False)
+            attr = self.attrs[1]
+            call: Formatter = (
+                self.container.get_formatter(
+                    attr, fallback=_AttrFallbackFormatterUnseperated
+                )
+                if isinstance(attr, str)
+                else attr
+            )
+            call.rq = self.rq
+            for line in call.format([package]):
+                sublines: list[str] = line.splitlines() if "\n" in line else [line]
+                yield from (initial + subline for subline in sublines)
+
+
 def remote_location(_, package: PackageCompat) -> str:
     return _stringify(package.remote_location())
 
 
-class _DefaultFormatters(Formatters):
-    def __call__(self) -> Any:
-        warnings.warn(
-            "DEPRECATED since 0.4.0: DefaultFormatters no longer needs to be called."
-            " It's already initialized."
-            " Just call DefaultFormatters.get_formatter() directly."
-        )
-        return self
-
+class RequiresMatchFormatter(SpecialFormatter):
+    format_line = format_line_notimplemented
+    _WRSRC: bool = False
+    MULTILINE = True
 
-DefaultFormatters = _DefaultFormatters(
-    dict(
-        plain="{0}",
-        plainwithrepo="{0} {0.reponame}",
-        nevrr="{0} {0.reponame}",
-        na="{0.name}.{0.arch}",
-        nev="{0.name}-{0.epoch}:{0.version}",
-        nevr="{0.name}-{0.evr}",
-        nevra="{0}",
-        full_nevra="{0.name}-{0.evr}.{0.arch}",
-        nv="{0.name}-{0.version}",
-        source=SourceFromatter,
-        src=SourceFromatter,
-        attr=AttrFormatter,
-        json=JsonFormatter,
-        line=SingleLineFormatter,
-        remote_location=remote_location,
-    ),
+    def format(self, packages: Iterable[PackageCompat]) -> Iterator[str]:
+        if not self.rq:
+            raise TypeError("self.rq is not set")
+        requires = {
+            str(require) for package in packages for require in package.requires
+        }
+        match_names = self.args.split(";") if ";" in self.args else self.args.split(",")
+        if self._WRSRC:
+            src_packages = self.rq.resolve_pkg_specs(match_names).filterm(arch="src")
+            match_packages = set(self.rq.get_subpackages(src_packages))
+        else:
+            match_packages = set(
+                self.rq.resolve_pkg_specs(match_names, resolve=False, with_src=False)
+            )
+        for reldep in requires:
+            if (
+                set(self.rq.resolve_pkg_specs([reldep], resolve=True, with_src=False))
+                & match_packages
+            ):
+                yield reldep
+
+
+class RequiresMatchSrcFormatter(RequiresMatchFormatter):
+    _WRSRC = True
+
+
+class _RequiresMatchPrefixFormatter(RequiresMatchFormatter):
+    PREFIX: ClassVar[str | Callable[[PackageCompat], str]]
+
+    def format(self, packages: Iterable[PackageCompat]) -> Iterator[str]:
+        for package in sorted(packages):
+            prefix_fmt = self.PREFIX
+            prefix = (
+                prefix_fmt(package)
+                if callable(prefix_fmt)
+                else prefix_fmt.format(package=package)
+            )
+            yield from (prefix + o for o in super().format([package]))
+
+
+class NARequiresMatchFormatter(_RequiresMatchPrefixFormatter):
+    PREFIX = "{package.name}.{package.arch} : "
+
+
+class SourceRequiresMatch(_RequiresMatchPrefixFormatter):
+
+    @staticmethod
+    def PREFIX(package: PackageCompat) -> str:  # type: ignore[override]
+        return f"{get_source_name(package)} : "
+
+
+class NARequiresMatchSrcFormatter(
+    RequiresMatchSrcFormatter, NARequiresMatchFormatter
+): ...
+
+
+DefaultFormatters = Formatters(
+    {
+        "plain": "{0}",
+        "plainwithrepo": "{0} {0.reponame}",
+        "nevrr": "{0} {0.reponame}",
+        "na": "{0.name}.{0.arch}",
+        "nev": "{0.name}-{0.epoch}:{0.version}",
+        "nevr": "{0.name}-{0.evr}",
+        "nevra": "{0}",
+        "full_nevra": "{0.name}-{0.evr}.{0.arch}",
+        "nv": "{0.name}-{0.version}",
+        "source": SourceFromatter,
+        "src": SourceFromatter,
+        "attr": AttrFormatter,
+        "json": JsonFormatter,
+        "line": SingleLineFormatter,
+        "remote_location": remote_location,
+        "multiline": MultilineFormatter,
+        "requiresmatch": RequiresMatchFormatter,
+        "rm": RequiresMatchFormatter,
+        "source+requiresmatch": SourceRequiresMatch,
+        "source+rm": SourceRequiresMatch,
+        "na-requiresmatch": NARequiresMatchFormatter,
+        "narm": NARequiresMatchFormatter,
+        "requiresmatch-src": RequiresMatchSrcFormatter,
+        "rmsrc": RequiresMatchSrcFormatter,
+        "narmsrc": NARequiresMatchSrcFormatter,
+        "na-requiresmatch-src": NARequiresMatchSrcFormatter,
+    },
     AttrFallbackFormatter,
 )
```

### Comparing `fedrq-0.9.0/src/fedrq/config.py` & `fedrq-1.0.0/src/fedrq/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 import importlib.resources as importlib_resources
 import itertools
 import logging
 import os
 import re
 import sys
 import typing as t
-import warnings
 import zipfile
 from collections.abc import Callable
 from enum import auto as auto_enum
-from importlib.abc import Traversable
 from pathlib import Path
 
 if sys.version_info < (3, 11):
+    from importlib.abc import Traversable
+
     import tomli as tomllib
 else:
+    from importlib.resources.abc import Traversable
+
     import tomllib
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, PrivateAttr, validator
 
 from fedrq._compat import StrEnum
 from fedrq._config import ConfigError
 from fedrq._utils import merge_dict, mklog
 from fedrq.backends import BACKENDS, get_default_backend
 from fedrq.backends.base import BaseMakerBase
 from fedrq.release_repo import AliasRepoG, DefaultRepoGs, RepoG, Repos
@@ -68,56 +70,60 @@
     matcher: t.Pattern
     repo_dirs: list[Path] = Field(
         default_factory=lambda: [
             directory.joinpath("repos") for directory in CONFIG_DIRS
         ]
     )
     defpaths: set[str] = Field(default_factory=set)
+    # full_def_paths is undocumented.
+    # It'll be set based on defpaths during model validation.
+    full_def_paths: list[t.Union[Traversable, Path]] = []
     system_repos: bool = True
     append_system_repos: bool = False
 
     koschei_collection: t.Optional[str] = None
     copr_chroot_fmt: t.Optional[str] = None
 
-    full_def_paths: t.ClassVar[list[t.Union[Traversable, Path]]] = []
     repo_aliases: dict[str, str] = {}
     repogs: Repos = Field(DefaultRepoGs, exclude=True)
 
     class Config:
         arbitrary_types_allowed = True
 
     @validator("repogs", always=True)
-    def v_repogs(cls, value: Repos, values: dict[str, t.Any]) -> Repos:
+    def _v_repogs(cls, value: Repos, values: dict[str, t.Any]) -> Repos:
         return (
             value | values["defs"] | AliasRepoG.from_str_mapping(values["repo_aliases"])
         )
 
-    @validator("defpaths")
-    def v_defpaths(cls, value, values) -> dict[str, t.Any]:
+    @validator("full_def_paths", always=True, pre=True)
+    def _v_full_def_paths(cls, value, values) -> list[t.Union[Traversable, Path]]:
+        # We don't care about what `value` is set to.
+        # It should be computed based on defpaths.
+        del value
+
+        defpaths = values["defpaths"].copy()
         flog = mklog(__name__, "ReleaseConfig", "_get_full_defpaths")
-        flog.debug(f"Getting defpaths for {values['name']}: {value}")
-        values["full_def_paths"] = cls._get_full_defpaths(
-            values["name"], value.copy(), values["repo_dirs"]
-        )
-        return value
+        flog.debug(f"Getting defpaths for {values['name']}: {defpaths}")
+        return cls._get_full_defpaths(values["name"], defpaths, values["repo_dirs"])
 
     @validator("matcher")
-    def v_matcher(cls, value: t.Pattern, values: dict[str, t.Any]) -> t.Pattern:
+    def _v_matcher(cls, value: t.Pattern, values: dict[str, t.Any]) -> t.Pattern:
         if not values["version"] and value.groups != 1:
             raise ValueError("'matcher' must have exactly one capture group")
         return value
 
     @validator("repo_dirs", pre=True)
-    def v_repo_dirs(cls, value: str | list[Path]) -> list[Path]:
+    def _v_repo_dirs(cls, value: str | list[Path]) -> list[Path]:
         if not isinstance(value, str):
             return value
         return [Path(directory) for directory in value.split(":")]
 
     @validator("append_system_repos", always=True)
-    def v_append_system_repos(cls, value: bool, values: dict[str, t.Any]) -> bool:
+    def _v_append_system_repos(cls, value: bool, values: dict[str, t.Any]) -> bool:
         if value:
             values["system_repos"] = True
         return value
 
     def is_match(self, val: str) -> bool:
         return bool(re.fullmatch(self.matcher, val))
 
@@ -250,40 +256,48 @@
         config: RQConfig | None = None,
         base_conf: dict[str, t.Any] | None = None,
         base_vars: dict[str, t.Any] | None = None,
         base_maker: BaseMakerBase | None = None,
         fill_sack: bool = True,
     ) -> dnf.Base | libdnf5.base.Base:
         """
-        :param config: An RQConfig object. If this is not passed, `self.config` is used.
-        :param base_conf: Base session configuration
-        :param base_vars: Base session vars/substitutions (arch, basearch,
+        Args:
+            config:
+                An RQConfig object. If this is not passed, `self.config` is used.
+            base_conf:
+                Base session configuration
+            base_vars:
+                Base session vars/substitutions (arch, basearch,
                                                            releasever, etc.)
-        :param base_maker: Existing BaseMaker object to configure.
-                           If base_maker is None, a new one will be created.
-        :param fill_sack: Whether to fill the Base object's package sack or
-                          just return the Base object after applying configuration.
+            base_maker:
+                Existing BaseMaker object to configure. If base_maker is None,
+                a new one will be created.
+            fill_sack:
+                Whether to fill the Base object's package sack or just return
+                the Base object after applying configuration.
         """
         if config is None:
             config = self.config
         base_conf = base_conf or {}
         base_vars = base_vars or {}
         releasever = config.backend_mod.get_releasever()
         if (
             "cachedir" not in base_conf
             and config.smartcache
-            and self.version != releasever
+            and (config.smartcache == "always" or self.version != releasever)
         ):
             logger.debug("Using smartcache")
             base_conf["cachedir"] = str(get_smartcache_basedir() / str(self.version))
         bm = base_maker or config.backend_mod.BaseMaker()
         bm.sets(base_conf, base_vars)
+        bm.load_release_repos(self, "releasever" not in base_vars)
         if config.load_filelists:
             bm.load_filelists()
-        bm.load_release_repos(self, "releasever" not in base_vars)
+        if config.load_other_metadata is not None:
+            bm.load_changelogs(config.load_other_metadata)
         return bm.fill_sack() if fill_sack else bm.base
 
     def _copr_repo(
         self, value: str, default_copr_baseurl: str = DEFAULT_COPR_BASEURL
     ) -> str:
         value = value.rstrip("/")
         if not self.copr_chroot_fmt:
@@ -309,29 +323,29 @@
         return f"{copr_baseurl}/{frag}/repo/{chroot}"
 
 
 class RQConfig(BaseModel):
     backend: t.Optional[str] = os.environ.get("FEDRQ_BACKEND")
     releases: dict[str, ReleaseConfig]
     default_branch: str = os.environ.get("FEDRQ_BRANCH", "rawhide")
-    smartcache: bool = True
+    smartcache: t.Union[bool, t.Literal["always"]] = True
+    load_other_metadata: t.Optional[bool] = None
     load_filelists: LoadFilelists = LoadFilelists.auto
-    _backend_mod = None
+    _backend_mod: BackendMod | None = PrivateAttr(None)
     copr_baseurl: str = DEFAULT_COPR_BASEURL
 
     class Config:
         json_encoders: dict[t.Any, Callable[[t.Any], str]] = {
             re.Pattern: lambda pattern: pattern.pattern,
             zipfile.Path: lambda path: str(path),
         }
-        underscore_attrs_are_private = True
         validate_assignment = True
 
     @validator("backend")
-    def v_backend(cls, value) -> str:
+    def _v_backend(cls, value) -> str:
         assert (
             value is None or value in BACKENDS
         ), f"Valid backends are: {', '.join(BACKENDS)}"
         return value
 
     @property
     def backend_mod(self) -> BackendMod:
@@ -380,19 +394,24 @@
         base_vars: dict[str, t.Any] | None = None,
     ) -> RepoqueryBase:
         """
         Higher level interface that finds the Release object that mathces
         {branch} and {repo}, creates a (lib)dnf(5).base.Base session, and
         returns a Repoquery object.
 
-        :param branch: branch name
-        :param repo: repo class. defaults to 'base'.
-        :param base_conf: Base session configuration
-        :param base_vars: Base session vars/substitutions (arch, basearch,
-                                                           releasever, etc.)
+        Args:
+            branch:
+                branch name
+            repo:
+                repo class. defaults to 'base'.
+            base_conf:
+                Base session configuration
+            base_vars:
+                Base session vars/substitutions (arch, basearch, releasever,
+                                                 etc.)
         """
         release = self.get_release(branch, repo)
         return self.backend_mod.Repoquery(release.make_base(self, base_conf, base_vars))
 
 
 def get_smartcache_basedir() -> Path:
     basedir = Path(os.environ.get("XDG_CACHE_HOME", Path("~/.cache").expanduser()))
@@ -423,44 +442,20 @@
         _get_files(importlib_resources.files("fedrq.data"), ".toml"),
         *(_get_files(p, ".toml") for p in reversed(CONFIG_DIRS)),
     ]
     flog.debug("all_files = %s", all_files)
     for path in itertools.chain.from_iterable(all_files):
         flog.debug("Loading config file: %s", path)
         with path.open("rb") as fp:
-            data = tomllib.load(fp)
+            data = tomllib.load(t.cast("t.BinaryIO", fp))
         merge_dict(data, config)
     merge_dict(overrides, config)
     config["releases"] = _get_releases(config["releases"])
     flog.debug("Final config: %s", config)
     return RQConfig(**config)
 
 
 def _get_releases(rdict: dict[str, dict[str, t.Any]]) -> dict[str, t.Any]:
     releases: dict[str, t.Any] = {}
     for name, data in rdict.items():
         releases[name] = dict(name=name, **data)
     return releases
-
-
-def get_rq(
-    branch: str | None = None,
-    repo: str = "base",
-    *,
-    smart_cache: bool | None = None,
-    load_filelists: bool | None = None,
-) -> RepoqueryBase:
-    """
-    **DEPRECATED since 0.4.0.** Use
-    [`RQConfig.get_rq()`][fedrq.config.RQConfig.get_rq] instead.
-
-    Higher level interface that creates an RQConfig object, finds the Release
-    object that mathces {branch} and {repo}, creates a dnf.Base, and finally
-    returns a Repoquery object.
-    """
-    warnings.warn("DEPRECATED since 0.4.0: use RQConfig.get_rq() instead.")
-    config = get_config()
-    if smart_cache is not None:
-        config.smartcache = smart_cache
-    if load_filelists is not None:
-        config.load_filelists = LoadFilelists.from_bool(load_filelists)
-    return config.get_rq(branch, repo)
```

### Comparing `fedrq-0.9.0/src/fedrq/data/releases.toml` & `fedrq-1.0.0/src/fedrq/data/releases.toml`

 * *Files 1% similar despite different names*

```diff
@@ -363,26 +363,33 @@
 ]
 
 
 [releases.eln]
 matcher = "^(eln)$"
 defpaths = [
     "fedora-eln.repo",
+    "eln-buildroot.repo",
 ]
 defs.no-crb = [
     "eln-baseos",
     "eln-baseos-source",
     "eln-appstream",
     "eln-appstream-source",
 ]
 defs.base = [
     "@no-crb",
     "eln-crb",
     "eln-crb-source",
 ]
+defs.buildroot = [
+    "koji-eln",
+    "koji-eln-source",
+]
+repo_aliases.koji = "@baseurl:https://kojipkgs.fedoraproject.org/repos/{}/latest/$basearch"
+repo_aliases.koji-src = "@baseurl:https://kojipkgs.fedoraproject.org/repos/{}/latest/src"
 
 [releases.local]
 matcher = "local"
 version = "$releasever"
 append_system_repos = true
 defs.base = []
```

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/almalinux.repo` & `fedrq-1.0.0/src/fedrq/data/repos/almalinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/amazonlinux.repo` & `fedrq-1.0.0/src/fedrq/data/repos/amazonlinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/centos-stream-compose.repo` & `fedrq-1.0.0/src/fedrq/data/repos/centos-stream-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/centos-stream.repo` & `fedrq-1.0.0/src/fedrq/data/repos/centos-stream.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/centos-stream8-compose.repo` & `fedrq-1.0.0/src/fedrq/data/repos/centos-stream8-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/centos-stream8.repo` & `fedrq-1.0.0/src/fedrq/data/repos/centos-stream8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/centos7.repo` & `fedrq-1.0.0/src/fedrq/data/repos/centos7.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/eln.repo` & `fedrq-1.0.0/src/fedrq/data/repos/eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/epel.repo` & `fedrq-1.0.0/src/fedrq/data/repos/epel.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/fedora-eln.repo` & `fedrq-1.0.0/src/fedrq/data/repos/fedora-eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/fedora-rawhide.repo` & `fedrq-1.0.0/src/fedrq/data/repos/fedora-rawhide.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/fedora-updates-testing.repo` & `fedrq-1.0.0/src/fedrq/data/repos/fedora-updates-testing.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/fedora-updates.repo` & `fedrq-1.0.0/src/fedrq/data/repos/fedora-updates.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/fedora.repo` & `fedrq-1.0.0/src/fedrq/data/repos/fedora.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/oraclelinux-8.repo` & `fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/oraclelinux-9.repo` & `fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-9.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/rocky.repo` & `fedrq-1.0.0/src/fedrq/data/repos/rocky.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/data/repos/ubi.repo` & `fedrq-1.0.0/src/fedrq/data/repos/ubi.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/src/fedrq/release_repo.py` & `fedrq-1.0.0/src/fedrq/release_repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         self.args = args
         self.container = container or Repos({})
         self.validate()
 
     @abc.abstractmethod
     def load(
         self, base_maker: BaseMakerBase, config: RQConfig, release: Release
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def err_fmt(self, msg: str) -> ConfigError:
         return ConfigError(msg)
 
     def err(self, msg: str, from_value: Any = ...) -> NoReturn:
         if from_value == ...:
             raise self.err_fmt(msg)
@@ -250,26 +249,28 @@
     # However, get_repo() will return a RepoG that's a subclass of
     # _ALLOWED_PLAIN even if the key doesn't start with '@'.
     _ALLOWED_PLAIN: tuple[type[RepoG]] = (MultiNameG,)
     # This RepoG will be used when get_repo() is passed a key that doesn't
     # start with '@'.
     _DEFAULT: type[RepoG] = SimpleRepoG
     # Factory function to generate a RepoG from a plain string or list.
-    _FALLBACK_FACTORY: Callable[
-        [str, Sequence[str] | str], type[RepoG]
-    ] = MultiNameG.from_names
+    _FALLBACK_FACTORY: Callable[[str, Sequence[str] | str], type[RepoG]] = (
+        MultiNameG.from_names
+    )
 
     def __init__(
         self,
         repo_classes: Mapping[str, Sequence[str] | str | type[RepoG]],
     ) -> None:
         self.__data: dict[str, type[RepoG]] = {
-            name: repos
-            if isinstance(repos, type) and issubclass(repos, RepoG)
-            else self._FALLBACK_FACTORY(name, repos)
+            name: (
+                repos
+                if isinstance(repos, type) and issubclass(repos, RepoG)
+                else self._FALLBACK_FACTORY(name, repos)
+            )
             for name, repos in ItemsView(repo_classes)
         }
 
     def get_repo(self, key: str) -> RepoG:
         if key.startswith("@"):
             name, seperator, args = key.partition(":")
             try:
```

### Comparing `fedrq-0.9.0/tests/conftest.py` & `fedrq-1.0.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
 
     monkeypatch.setattr(rqconfig, "CONFIG_DIRS", config_dirs)
     return config_dirs[0]
 
 
 @pytest.fixture
 def repo_test_rq(patch_config_dirs):
-    return rqconfig.get_config(load_filelists="always").get_rq("tester", "base")
+    return rqconfig.get_config(
+        load_filelists="always", load_other_metadata=True
+    ).get_rq("tester", "base")
 
 
 @pytest.fixture(scope="session")
 def target_cpu():
     macro = subprocess.run(
         ["rpm", "-E", "%_target_cpu"], text=True, capture_output=True, check=True
     ).stdout.strip()
```

### Comparing `fedrq-0.9.0/tests/integration/test_backends.py` & `fedrq-1.0.0/tests/integration/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,9 +49,8 @@
         skip_if_unavailable=False,
         type="rpm-md",
         gpgcheck=True,
         repo_gpgcheck=False,
     )
     rq = default_backend.Repoquery(bm.fill_sack())
     query = rq.query()
-    assert len(query) == 2
     assert {p.name for p in query} == {"copr-module-integration-dummy-package"}
```

### Comparing `fedrq-0.9.0/tests/integration/test_pkgs.py` & `fedrq-1.0.0/tests/integration/test_pkgs.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,37 @@
 
 import pytest
 
 import fedrq.cli
 
 
 @pytest.mark.skip(
-    "This test loads rawhide metadata and is expensive. We already load f37."
+    "This test loads rawhide metadata and is expensive. We already load f38."
 )
 @pytest.mark.no_rpm_mock
 def test_pkgs_basic_rawhide(capsys, target_cpu):
     fedrq.cli.main(["pkgs", "bash", "-Fna", "--sc"])
     stdout, stderr = capsys.readouterr()
     assert sorted(stdout.splitlines()) == sorted(["bash.src", f"bash.{target_cpu}"])
 
 
 @pytest.mark.no_rpm_mock
 def test_pkgs_forcearch(runs):
     stdout, stderr = runs(
-        ["pkgs", "--forcearch", "s390x", "-F", "arch", "-b", "f37", "*"], False
+        [
+            "pkgs",
+            "--forcearch",
+            "s390x",
+            "-F",
+            "arch",
+            "-b",
+            "ubi9",
+            "-r",
+            "ubi-baseos-rpms",
+            "-e",
+            "ubi-baseos-source",
+            "*",
+        ],
+        False,
     )
     assert not stderr
     assert set(stdout) == {"noarch", "s390x", "src"}
```

### Comparing `fedrq-0.9.0/tests/integration/test_subpkgs.py` & `fedrq-1.0.0/tests/integration/test_subpkgs.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,29 +13,42 @@
     "yt-dlp-zsh-completion",
 ]
 
 
 @pytest.mark.no_rpm_mock
 def test_subpkgs_match1(capsys):
     fedrq.cli.main(
-        ["subpkgs", "-b", "f37", "yt-dlp", "--match", "*completion", "-F", "name"]
+        [
+            "subpkgs",
+            "-b",
+            "f38",
+            "-r",
+            "@release",
+            "yt-dlp",
+            "--match",
+            "*completion",
+            "-F",
+            "name",
+        ]
     )
     stdout, stderr = capsys.readouterr()
     assert sorted(stdout.splitlines()) == YT_DLP_SUPKGS
     assert not stderr
 
 
 @pytest.mark.no_rpm_mock
 def test_subpkgs_match2(capsys):
     # Find the source packages that contain a subpackage that match '*-devel'
     fedrq.cli.main(
         [
             "subpkgs",
             "-b",
-            "f37",
+            "f38",
+            "-r",
+            "@release",
             "ansible-core",
             "moby-engine",
             "python-pip",
             "yt-dlp",
             "gh",  # no matches
             "-M",
             "*-fish-completion",
```

### Comparing `fedrq-0.9.0/tests/integration/test_whatrequires.py` & `fedrq-1.0.0/tests/integration/test_whatrequires.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,40 +18,55 @@
     (["-P", "python3dist(yt-dlp)"]),
     (["yt-dlp.noarch"]),
 )
 
 
 @pytest.mark.no_rpm_mock
 @pytest.mark.parametrize("args", ARGS)
-def test_whatrequires_exclude_subpackages_f37(capsys, args):
-    fedrq.cli.main(["whatrequires", "-b", "f37", "--sc", "-X", "-Fname", *args])
+def test_whatrequires_exclude_subpackages_f38(capsys, args):
+    fedrq.cli.main(
+        ["whatrequires", "-b", "f38", "-r", "@release", "--sc", "-X", "-Fname", *args]
+    )
     stdout, stderr = capsys.readouterr()
     stdout_lines = set(stdout.splitlines())
     assert not (stdout_lines & YT_DLP_SUPKGS)
     assert "celluloid" in stdout_lines
     assert not stderr
 
 
 @pytest.mark.no_rpm_mock
 @pytest.mark.parametrize("args", ARGS)
-def test_whatrequires_not_exclude_subpackages_f37(capsys, args):
-    fedrq.cli.main(["whatrequires", "-b", "f37", "--sc", "-Fname", *args])
+def test_whatrequires_not_exclude_subpackages_f38(capsys, args):
+    fedrq.cli.main(
+        ["whatrequires", "-b", "f38", "-r", "@release", "--sc", "-Fname", *args]
+    )
     stdout, stderr = capsys.readouterr()
     stdout_lines = set(stdout.splitlines())
     assert stdout_lines & YT_DLP_SUPKGS
     assert "celluloid" in stdout_lines
     assert not stderr
 
 
 @pytest.mark.no_rpm_mock
 def test_whatrequires_resolve(capsys):
     """
     Ensure that SRPM names are not considered when resolving Provides
     E.g. python-setuptools should resolve to python3-setuptools.noarch
     (Provides python-setuptools) instead of python-setuptools.src.
     """
-    fedrq.cli.main(["whatrequires", "-b", "f37", "-P", "-Fna", "python-setuptools"])
+    fedrq.cli.main(
+        [
+            "whatrequires",
+            "-b",
+            "f38",
+            "-r",
+            "@release",
+            "-P",
+            "-Fna",
+            "python-setuptools",
+        ]
+    )
     stdout, stderr = map(lambda f: f.splitlines(), capsys.readouterr())
     # 3700 as of 2023-01-23. Le
     assert len(stdout) > 3000
     assert "python-pip.src" in stdout and "yt-dlp.src" in stdout
     assert not stderr
```

### Comparing `fedrq-0.9.0/tests/integration/test_whatrequires_src.py` & `fedrq-1.0.0/tests/integration/test_whatrequires_src.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,37 +12,40 @@
     "args",
     [
         pytest.param(["ansible-core"]),
         pytest.param(["ansible-core.src"]),
     ],
 )
 def test_whatrequires_src_integration(runs, args):
-    stdout, stderr = runs(["wrsrc", "-b", "f37", "-Fna", *args], False)
+    stdout, stderr = runs(
+        ["wrsrc", "-b", "f38", "-r", "@release", "-Fna", *args], False
+    )
     assert not stderr
     assert any(p.startswith("ansible-collection") for p in stdout)
     assert {"ansible-packaging.noarch", "ansible.noarch", "ansible.src"} & set(stdout)
 
 
 @pytest.mark.no_rpm_mock
 def test_whatrequires_src_integration_exclude(runs):
     stdout, stderr = runs(
-        ["wrsrc", "-b", "f37", "-Fsource", "-X", "ansible-packaging"], False
+        ["wrsrc", "-b", "f38", "-r", "@release", "-Fsource", "-X", "ansible-packaging"],
+        False,
     )
     assert not stderr
     assert {
         "ansible-collection-ansible-posix",
         "ansible-collection-community-general",
     } & set(stdout)
     assert "ansible-packaging" not in stdout
 
 
 @pytest.mark.no_rpm_mock
 def test_whatrequires_src_integration_exclude_control(runs):
     stdout, stderr = runs(
-        ["wrsrc", "-b", "f37", "-Fsource", "ansible-packaging"], False
+        ["wrsrc", "-b", "f38", "-r", "@release", "-Fsource", "ansible-packaging"], False
     )
     assert not stderr
     assert {
         "ansible-collection-ansible-posix",
         "ansible-collection-community-general",
     } & set(stdout)
     assert "ansible-packaging" in stdout
```

### Comparing `fedrq-0.9.0/tests/test_data/build.sh` & `fedrq-1.0.0/tests/test_data/build.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+#!/usr/bin/bash
+
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
-#!/usr/bin/bash
 set -euo pipefail
-cd "$(readlink -f $(dirname ${0}))"
+HERE="$(readlink -f "$(dirname "${0}")")"
+cd "${HERE}"
 
 # Return 1 if the repodata is up to date
 # Return 0 if the repodata needs to be regenerated
 regenerate() {
     [ "${1-}" = "--force" ] && return 0
 
     { [ -f "built" ] && [ -d "repo/repodata" ]; } || return 0
 
-    local built_files="$(awk '{print $2}' built | sort)"
-    local fs_files="$(find specs/ -name '*.spec' | sort)"
+    local built_files fs_files
+    built_files="$(awk '{print $2}' built | sort)"
+    fs_files="$(find specs/ -name '*.spec' | sort)"
     [ "${built_files}" = "${fs_files}" ] || return 0
 
     sha256sum -c built &> /dev/null || return 0
 
     return 1
 }
 
 for repo in repos/*; do
     cd "${repo}"
     specs="$(find specs -name '*.spec')"
     if regenerate "$@"; then
         rm -rf repo
-        printf "${specs}\n"
+        echo "${specs}"
         while read -r spec; do
             specdir="$(dirname "${spec}")"
             base_specdir="$(basename "${specdir}")"
             rpmbuild -ba --nodeps \
                 -D "_srcrpmdir %(pwd)/repo/SRPMS/${base_specdir}" \
                 -D "_rpmdir %(pwd)/repo/RPMS/${base_specdir}" \
                 -D '_build_name_fmt %%{NAME}-%{?EPOCH:%%{EPOCH}:}%%{VERSION}-%%{RELEASE}.%%{ARCH}.rpm' \
```

### Comparing `fedrq-0.9.0/tests/test_data/repos/repo1/specs/e1/packageb.spec` & `fedrq-1.0.0/tests/test_data/repos/repo1/specs/e1/packageb.spec`

 * *Files 10% similar despite different names*

```diff
@@ -51,7 +51,9 @@
 
 %files sub
 %{_datadir}/%{name}-sub
 
 
 %changelog
 
+* Sun Jul 16 2023 Maxwell G <maxwell@gtmx.me> - 11111:2-1
+- Dummy changelog entry
```

### Comparing `fedrq-0.9.0/tests/test_data/repos/repo1/specs/packagea.spec` & `fedrq-1.0.0/tests/test_data/repos/repo1/specs/packagea.spec`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 Provides:       package(a)
 Provides:       vpackage(a) = %{version}-%{release}
 Requires:       vpackage(b)
 
 
 %description
 %{summary}.
+This is another line of text.
+Another another.
+And another.
 
 %package        sub
 Summary:        %{name}-sub is a subpackage of %{name}
 Provides:       subpackage(a)
 Provides:       vsubpackage(a) = %{version}-%{release}
 Requires:       %{name} = %{?epoch:%{epoch}:}%{version}-%{release}
 Requires:       /usr/share/packageb-sub
@@ -49,7 +52,9 @@
 
 %files sub
 %{_datadir}/%{name}-sub
 
 
 %changelog
 
+* Sun Jul 16 2023 Maxwell G <maxwell@gtmx.me> - 1-1
+- Dummy changelog entry
```

### Comparing `fedrq-0.9.0/tests/test_data/repos/repo1/specs/packageb.spec` & `fedrq-1.0.0/tests/test_data/repos/repo1/specs/packageb.spec`

 * *Files 24% similar despite different names*

```diff
@@ -50,7 +50,9 @@
 
 %files sub
 %{_datadir}/%{name}-sub
 
 
 %changelog
 
+* Sun Jul 16 2023 Maxwell G <maxwell@gtmx.me> - 1-1
+- Dummy changelog entry
```

### Comparing `fedrq-0.9.0/tests/unit/test_archive.py` & `fedrq-1.0.0/tests/unit/test_archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,13 +26,13 @@
     tmp_path: Path, data_path: Path, target_cpu: str
 ):
     repo1 = data_path / "repos/repo1/"
     invalid = repo1 / f"repo/RPMS/specs/packageb-1-1.fc36.{target_cpu}.rpm"
     assert invalid.is_file()
     dest = tmp_path / "abc"
     dest.mkdir()
-    with RPMArchive(invalid) as archive:
+    with RPMArchive(invalid) as archive:  # noqa SIM177
         with pytest.raises(
             RPMArchiveError, match=re.escape(f"{archive} is not a source rpm")
         ):
             archive.extract_specfile(dest)
     assert next(dest.iterdir(), None) is None
```

### Comparing `fedrq-0.9.0/tests/unit/test_checkconfig.py` & `fedrq-1.0.0/tests/unit/test_checkconfig.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_command.py` & `fedrq-1.0.0/tests/unit/test_command.py`

 * *Files 13% similar despite different names*

```diff
@@ -122,14 +122,17 @@
         # --system-cache is used when smartcache is disabled in the config
         ([], False, lambda _: None),
         # --system-cache is used when smartcache is disabled in the config (redundant)
         (["--system-cache"], False, lambda _: None),
         # --cachedir trumps smartcache
         (["--cachedir=blah"], True, lambda _: Path("blah")),
         (["--cachedir=blah"], False, lambda _: Path("blah")),
+        # --smartcache-always
+        (["--smartcache-always"], True, lambda d: d / "tester"),
+        (["--smartcache-always"], False, lambda d: d / "tester"),
     ),
 )
 def test_smartcache_config(
     args,
     config_smartcache,
     cachedir,
     patch_config_dirs,
@@ -166,14 +169,58 @@
 
         finally:
             shutil.rmtree("blah", ignore_errors=True)
             dest.unlink(True)
 
 
 @pytest.mark.parametrize("subcommand", SUBCOMMANDS)
+def test_smartcache_always(
+    subcommand, mocker, monkeypatch, patch_config_dirs, temp_smartcache: Path
+):
+    """
+    Ensure that the smartcache is used when the requested
+    branch's releasever is the same as the the system's releasever
+    and smartcache='always' is used.
+    """
+    assert not list(temp_smartcache.iterdir())
+
+    mocks = {}
+
+    def _set_config(self, key: str) -> None:
+        arg = getattr(self.args, key, None)
+        if arg is not None:
+            setattr(self.config, key, arg)
+        if key == "backend":
+            mocks["get_releasever"] = mocker.patch.object(
+                self.config.backend_mod, "get_releasever", return_value="tester"
+            )
+            mocks["bm_set"] = mocker.spy(self.config.backend_mod.BaseMaker, "set")
+
+    cls = fedrq.cli.COMMANDS[subcommand]
+    monkeypatch.setattr(cls, "_set_config", _set_config)
+
+    parser = cls.make_parser()
+    args = parser.parse_args(["--smartcache-always", "packageb"])
+    obj = cls(args)
+
+    mocks["get_releasever"].assert_called_once()
+
+    expected_cachedir = temp_smartcache / "fedrq" / "tester"
+
+    assert any(
+        call.args[1:] == ("cachedir", str(expected_cachedir))
+        for call in mocks["bm_set"].call_args_list
+    )
+
+    assert obj.args.smartcache
+
+    assert list(temp_smartcache.iterdir())
+
+
+@pytest.mark.parametrize("subcommand", SUBCOMMANDS)
 def test_nonexistant_formatter(subcommand, patch_config_dirs, capsys):
     with pytest.raises(SystemExit, match=r"^1$"):
         fedrq.cli.main([subcommand, "--formatter=blahblah", "*"])
     stdout, stderr = capsys.readouterr()
     assert not stdout
     assert stderr.splitlines() == [
         "ERROR: 'blahblah' is not a valid formatter",
```

### Comparing `fedrq-0.9.0/tests/unit/test_download.py` & `fedrq-1.0.0/tests/unit/test_download.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_formatters.py` & `fedrq-1.0.0/tests/unit/test_formatters.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,40 +7,50 @@
 from collections.abc import Callable, Collection
 from functools import cache
 from pathlib import Path
 
 import pytest
 
 from fedrq import config as rqconfig
+from fedrq.backends.base import PackageQueryCompat, RepoqueryBase
 from fedrq.cli import formatters
 
 
 @cache
 def get_rq():
     return rqconfig.get_config(load_filelists="always").get_rq("tester", "base")
 
 
-def formatter(query, formatter_name="plain", *args, attr=False, **kwargs):
-    result = sorted(
-        (
-            str(i)
-            for i in formatters.DefaultFormatters.get_formatter(formatter_name).format(
-                query, *args, **kwargs
-            )
-        )
-    )
+def formatter(
+    query,
+    formatter_name="plain",
+    *args,
+    attr=False,
+    sort=True,
+    repoquery: RepoqueryBase | None = None,
+    **kwargs,
+):
+    result = [
+        str(i)
+        for i in formatters.DefaultFormatters.get_formatter(
+            formatter_name, repoquery=repoquery
+        ).format(query, *args, **kwargs)
+    ]
+    if sort:
+        result.sort()
     if attr:
-        assert result == sorted(
-            (
-                str(i)
-                for i in formatters.DefaultFormatters.get_formatter(
-                    f"attr:{formatter_name}"
-                ).format(query, *args, **kwargs)
-            )
-        )
+        result2 = [
+            str(i)
+            for i in formatters.DefaultFormatters.get_formatter(
+                f"attr:{formatter_name}"
+            ).format(query, *args, **kwargs)
+        ]
+        if sort:
+            result2.sort()
+        assert result == result2
     return result
 
 
 # @pytest.mark.parametrize("special_repos", ("repo1",), indirect=["special_repos"])
 def test_plain_formatter(patch_config_dirs, target_cpu):
     repo_test_rq = get_rq()
     expected = sorted(
@@ -304,7 +314,130 @@
     repo_test_rq = get_rq()
     query = repo_test_rq.resolve_pkg_specs(["packagea*"], latest=1)
     output = formatter(
         query, "json:name,evr,arch,requires,conflicts,provides,source_name"
     )
     assert len(output) == 1
     assert json.loads(output[0]) == expected
+
+
+def test_multiline_formatter(patch_config_dirs, target_cpu: str):
+    repo_test_rq = get_rq()
+    query = repo_test_rq.resolve_pkg_specs(
+        ["packagea-1", "packageb"], with_src=False, latest=1
+    )
+    output = formatter(query, "multiline:na,description", sort=False)
+    assert output == [
+        "packagea.noarch : packagea is a test package.",
+        "packagea.noarch : This is another line of text.",
+        "packagea.noarch : Another another.",
+        "packagea.noarch : And another.",
+        f"packageb.{target_cpu} : ...",
+    ]
+
+
+@cache
+def formatter_test_query() -> PackageQueryCompat:
+    repo_test_rq = get_rq()
+    return repo_test_rq.resolve_pkg_specs(
+        ["packagea-1", "packageb"], with_src=False, latest=1
+    )
+
+
+@pytest.mark.parametrize(
+    "formatter_,expected_output",
+    [
+        pytest.param(
+            "multiline:na,description",
+            [
+                "packagea.noarch : packagea is a test package.",
+                "packagea.noarch : This is another line of text.",
+                "packagea.noarch : Another another.",
+                "packagea.noarch : And another.",
+                "packageb.{target_cpu} : ...",
+            ],
+            id="multiline",
+        ),
+        pytest.param(
+            "line:na,repoid",
+            [
+                "packagea.noarch : testrepo1",
+                "packageb.{target_cpu} : testrepo1",
+            ],
+            id="line-simple",
+        ),
+        pytest.param(
+            "line:na,repoid:",
+            [
+                "packagea.noarch : testrepo1",
+                "packageb.{target_cpu} : testrepo1",
+            ],
+            id="line-trailing",
+        ),
+        pytest.param(
+            "line:na,repoid: | ",
+            [
+                "packagea.noarch | testrepo1",
+                "packageb.{target_cpu} | testrepo1",
+            ],
+            id="line-custom-separator",
+        ),
+        pytest.param(
+            "line:na,repoid,source: | ",
+            [
+                "packagea.noarch | testrepo1 | packagea",
+                "packageb.{target_cpu} | testrepo1 | packageb",
+            ],
+            id="line-special-formatter",
+        ),
+        pytest.param(
+            "line:line:na,repoid: | ",
+            [
+                "packagea.noarch | testrepo1",
+                "packageb.{target_cpu} | testrepo1",
+            ],
+            id="line-stacked",
+        ),
+        pytest.param(
+            "description",
+            [
+                "packagea is a test package.\n"
+                "This is another line of text.\nAnother another.\nAnd another.\n---\n",
+                "...",
+            ],
+            id="description",
+        ),
+        pytest.param(
+            [
+                "requiresmatch:packageb",
+                "rm:packageb",
+                "rmsrc:packageb",
+                "requiresmatch-src:packageb",
+            ],
+            ["vpackage(b)"],
+            id="rm",
+        ),
+        pytest.param(
+            ["narm:packageb", "na-requiresmatch:packageb,packagea,jfjfjfj"],
+            ["packagea.noarch : vpackage(b)"],
+            id="narm",
+        ),
+        pytest.param(
+            ["source+requiresmatch:packageb", "source+rm:packageb"],
+            ["packagea : vpackage(b)"],
+            id="source+requiresmatch",
+        ),
+    ],
+)
+def test_formatter_p(
+    patch_config_dirs,
+    target_cpu: str,
+    formatter_: str | Collection[str],
+    expected_output: Collection[str],
+) -> None:
+    formatters = [formatter_] if isinstance(formatter_, str) else formatter_
+    query = formatter_test_query()
+    for fmt in formatters:
+        output = formatter(query, fmt, sort=False, repoquery=get_rq())
+        assert output == [
+            item.format(target_cpu=target_cpu) for item in expected_output
+        ], fmt
```

### Comparing `fedrq-0.9.0/tests/unit/test_pkgs.py` & `fedrq-1.0.0/tests/unit/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_release.py` & `fedrq-1.0.0/tests/unit/test_release.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_release_repo.py` & `fedrq-1.0.0/tests/unit/test_release_repo.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_repolist.py` & `fedrq-1.0.0/tests/unit/test_repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_subbpkgs.py` & `fedrq-1.0.0/tests/unit/test_subbpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/tests/unit/test_whatrequires.py` & `fedrq-1.0.0/tests/unit/test_whatrequires.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,7 +141,14 @@
 
 
 def test_whatrequires_exclude_subpackages(run_command):
     expected = ["packagea.noarch", "packagea.src"]
     stdout, stderr = run_command(["-X", "-F", "na", "packageb"])
     assert not stderr
     assert stdout == expected
+
+
+def test_whatrequires_extra_exact(run_command):
+    expected = ["packagea-1-1.fc36.noarch"]
+    stdout, stderr = run_command(["--ee", "vpackage(b)"])
+    assert not stderr
+    assert stdout == expected
```

### Comparing `fedrq-0.9.0/tests/unit/test_whatrequires_src.py` & `fedrq-1.0.0/tests/unit/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.9.0/PKG-INFO` & `fedrq-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 Metadata-Version: 2.1
 Name: fedrq
-Version: 0.9.0
+Version: 1.0.0
 Summary: fedrq is a tool to query the Fedora and EPEL repositories
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Classifier: Environment :: Console
-Requires-Dist: pydantic ~= 1.0
+Requires-Dist: pydantic >= 1, < 3
 Requires-Dist: tomli; python_version<'3.11'
 Requires-Dist: requests
+Requires-Dist: rpm
 Requires-Dist: ruff ; extra == "codeqa"
 Requires-Dist: reuse ; extra == "codeqa"
 Requires-Dist: fedrq[codeqa] ; extra == "dev"
 Requires-Dist: fedrq[doc] ; extra == "dev"
 Requires-Dist: fedrq[formatters] ; extra == "dev"
 Requires-Dist: fedrq[test] ; extra == "dev"
 Requires-Dist: fedrq[typing] ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: black ; extra == "doc"
+Requires-Dist: griffe !=0.32.0, !=0.32.1 ; extra == "doc"
 Requires-Dist: mkdocs ; extra == "doc"
+Requires-Dist: mkdocs-exclude ; extra == "doc"
+Requires-Dist: mkdocs-gen-files ; extra == "doc"
 Requires-Dist: mkdocs-material ; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18 ; extra == "doc"
-Requires-Dist: mkdocs-exclude ; extra == "doc"
+Requires-Dist: releaserr ; extra == "doc"
 Requires-Dist: black ; extra == "formatters"
-Requires-Dist: isort ; extra == "formatters"
+Requires-Dist: isort !=5.13.0 ; extra == "formatters"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: tomli-w ; extra == "test"
 Requires-Dist: mypy ; extra == "typing"
 Requires-Dist: types-requests ; extra == "typing"
 Requires-Dist: argcomplete ; extra == "typing"
 Requires-Dist: typing_extensions ; extra == "typing"
@@ -62,15 +67,15 @@
 A tool for querying the Fedora and EPEL repositories
 
 fedrq makes it easy to query any branch of Fedora or EPEL. It uses the dnf
 Python bindings and does not shell out to `dnf repoquery`. It allows querying
 for reverse dependencies, packages that contain a certain Provide or file,
 subpackages of an SRPM, and package metadata.
 
-The tool doesn't seek to replace every feature of dnf repoquery. It provides a
+The tool doesn't seek to replace every feature of `dnf repoquery`. It provides a
 more user friendly interface than `dnf repoquery` for certain common tasks.
 
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/fedrq/commits/main.svg)](https://builds.sr.ht/~gotmax23/fedrq/commits/main?)
 
 [![copr build status][badge-copr]][link-copr] (stable)
 
 [![copr build status][badge-copr-dev]][link-copr-dev] (dev)
@@ -84,18 +89,18 @@
 [![fedrq on lists.sr.ht][badge-list]][link-list]
 
 [![fedrq on todo.sr.ht][badge-todo]][link-todo]
 
 
 ## Installation
 
-fedrq has a copr repository at [gotmax23/fedrq][link-copr] that contains
+fedrq has a Copr repository at [gotmax23/fedrq][link-copr] that contains
 released versions.
 Development snapshots are available at [gotmax23/fedrq-dev][link-copr-dev].
-The RPM specfile is in the repository root.
+The RPM specfile is located in the repository root.
 
 fedrq is also [published to PyPI](https://pypi.org/project/fedrq/) so you can
 `pip install fedrq`.
 
 When installing the package with pip, some additional system packages
 are needed.
 
@@ -103,14 +108,17 @@
 
 - python3-dnf (dnf is currently the default Fedora package manager, so this
   should already be installed)
 
 The following additional system packages are required for the libdnf5 backend:
 
 - python3-libdnf5
+
+The following additional system packages are always required:
+
 - python3-rpm
 
 fedrq defaults to the dnf backend, but fedrq falls back to the libdnf5 backend
 if the former's dependencies aren't installed.
 Users can explicitly choose a backend with the
 `--backend` [CLI option](https://fedrq.gtmx.me/fedrq1/#shared-options)
 or globally in the [fedrq config file](https://fedrq.gtmx.me/fedrq5).
@@ -121,76 +129,88 @@
 
 `fedrq check-config --dump` requires `tomli-w`.
 The RPM package weakly depends on `python3-tomli-w`.
 
 ## Container images
 
 fedrq now provides container images.
-- `quay.io/gotmax23/fedrq:latest` is built with
+
+- [`quay.io/gotmax23/fedrq:latest`][Containerfile] is built with
   `registry.fedoraproject.org/fedora:latest`.
-- `quay.io/gotmax23/fedrq:ubi9` is built with the ubi9 image.
+- [`quay.io/gotmax23/fedrq:ubi9`][Containerfile.rhel] is built with the ubi9
+  image.
   It includes a builtin `rhel9` repository configuration that can be used to
   query the actual RHEL repositories when run on a system registered with
   subscription-manager.
 
 Both of these images use the latest fedrq RPM packages from the
 [gotmax23/fedrq][link-copr] Copr repository.
 
+``` console
+$ podman run --rm -v ~/.cache/fedrq:/fedrq-cache/fedrq:z quay.io/gotmax23/fedrq \
+    pkgs fedrq -Fnevrr
+fedrq-0.9.0-1.fc39.noarch rawhide
+fedrq-0.9.0-1.fc39.src rawhide-source
+```
+
+[Containerfile]: https://git.sr.ht/~gotmax23/fedrq/tree/main/item/contrib/container/Containerfile
+[Containerfile.rhel]: https://git.sr.ht/~gotmax23/fedrq/tree/main/item/contrib/container/Containerfile.rhel
+
 ## Versioning
 
 This project is in beta and its versioning scheme follows semver.
 
 See [NEWS.md](https://git.sr.ht/~gotmax23/fedrq/tree/main/NEWS.md).
 
 ## Python API
 
 The `fedrq.config` module and the `fedrq.backend` package are public API.
-Everything under `fedrq.cli` is internal. fedrq is a primarily a CLI tool and
-its API abstracts the specific dnf/libdnf5 functionality that it uses. The
-API's main purpose is repoquerying, but you can use the fedrq functionality
+Everything under `fedrq.cli` is internal. fedrq is primarily a CLI tool and
+its API only abstracts the specific dnf/libdnf5 functionality that the CLI uses. The
+API's main purpose is "repoquerying", but you can use the fedrq functionality
 you'd like and then access the underlying dnf Base object to preform other
 tasks if needed.
 
 See the [API Summary] on the docsite for more information. See [api-examples]
 for some example code. As always, direct any feedback, questions, or issues to
 the mailing list (see [Contributing](#contributing)).
 
 [API Summary]: https://fedrq.gtmx.me/API/Summary/
 
 
-## Documentaion
+## Documentation
 
-See our new [docsite][link-docsite] for rendered manpages, changelogs, and
+See fedrq's [documentation site][link-docsite] for rendered manpages, changelogs, and
 Python API documentation.
 
 
 ## Contributing
 
 Development, issue reporting, and project discussion happen on [the mailing
 list][link-list] ([~gotmax23/fedrq@lists.sr.ht][mailto]).
 
 See [CONTRIBUTING.md].
 
 
 ## Credits
 Thank you to the dnf maintainers. This tool is inspired by `dnf repoquery` and
-uses the `dnf` python bindings.
+uses the dnf python bindings.
 
 
 ## License
 
 This project follows the REUSE specification. In general:
 
 - Code is licensed under GPL-2.0-or-later. This is the same license as dnf.
 - Configuration and repo files in fedrq/data/ are `UNLICENSE`ed
 - fedrq.spec is licensed under MIT to match Fedora
 - The embedded repo defs in src/fedrq/data/repos from fedora-repos.rpm are MIT
   licensed.
   These are only used when the needed repo defs are not available in the system
-  config (i.e. for querying the Fedora repos from a non Fedora system).
+  config (i.e., for querying the Fedora repos from a non Fedora system).
 - `enum.StrEnum` is copied from Cpython 3.11 for older Python versions. It's
   ~30 lines of PSF-2.0 licensed code.
 
 ```
 SPDX-License-Identifier: GPL-2.0-or-later AND Unlicense AND MIT AND PSF-2.0
 ```
```

