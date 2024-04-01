# Comparing `tmp/girder-3.2.3.dev5.tar.gz` & `tmp/girder-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-3.2.3.dev5.tar", last modified: Wed Feb 14 15:48:37 2024, max compression
+gzip compressed data, was "girder-3.2.3.dev7.tar", last modified: Wed Feb 14 18:46:58 2024, max compression
```

## Comparing `girder-3.2.3.dev5.tar` & `girder-3.2.3.dev7.tar`

### file list

```diff
@@ -1,975 +1,975 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.642939 girder-3.2.3.dev5/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.circleci/Dockerfile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14387 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.circleci/config.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      710 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.circleci/create_ansible_subtree.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      316 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.circleci/generatePyEnvChecksum.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1118 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.circleci/publish_npm.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      360 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.circleci/publish_pypi.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.codecov.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.dockerignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.editorconfig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      258 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20024 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/CMakeLists.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4925 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/Dockerfile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2721 2024-02-14 15:48:37.642939 girder-3.2.3.dev5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1427 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/Vagrantfile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.510938 girder-3.2.3.dev5/clients/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/clients/python/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/clients/python/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/clients/python/girder_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/clients/python/girder_client/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/clients/python/girder_client/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/clients/python/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.510938 girder-3.2.3.dev5/devops/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/devops/ansible-role-girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/.yamllint
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/devops/ansible-role-girder/defaults/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/defaults/main.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/devops/ansible-role-girder/handlers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/handlers/main.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/devops/ansible-role-girder/library/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/library/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4135 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/library/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60712 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/library/girder.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.530938 girder-3.2.3.dev5/devops/ansible-role-girder/meta/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/meta/main.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.510938 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/converge.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/data/test1.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/data/test2.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/data/test3.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/molecule.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/prepare.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/requirements.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22622 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_access.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1154 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3879 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3895 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_files.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9955 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7840 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1815 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2906 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_user.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/converge.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/molecule.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      276 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/prepare.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/pytest.ini
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/tests/test_default.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/ansible-role-girder/tasks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2472 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/tasks/main.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/tasks/nodejs.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.510938 girder-3.2.3.dev5/devops/ansible-role-girder/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/ansible-role-girder/templates/daemon/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/ansible-role-girder/templates/daemon/girder.service.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/deployment-template/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/deployment-template/hosts.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/deployment-template/playbook.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      267 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/deployment-template/provision.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/deployment-template/requirements.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.534938 girder-3.2.3.dev5/devops/vagrant/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/vagrant/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/vagrant/ansible.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2139 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/vagrant/vagrant-playbook.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/devops/vagrant/vagrant-requirements.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.538938 girder-3.2.3.dev5/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/admin-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5288 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/api-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/build-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/changelog.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2379 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6551 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/configuration.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5131 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/dependencies.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/deployment-alternatives.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/deployment.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/dev-installation.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23262 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/developer-cookbook.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/developer-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18444 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/external-web-clients.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15086 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/favicon.ico
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.538938 girder-3.2.3.dev5/docs/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   803025 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/images/dicom-viewer.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5181 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/license.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26440 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/migration-guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/mount.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38303 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/plugin-development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22537 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/plugins.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10888 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/python-client.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/requirements-docs.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5707 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/security.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1640 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/sftp.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/user-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14123 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/docs/user-guide.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.542938 girder-3.2.3.dev5/girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11228 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.542938 girder-3.2.3.dev5/girder/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4349 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/access.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/api_docs.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/api_main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33164 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/describe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5196 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/docs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3483 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/filter_logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    51261 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7259 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/sftp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.546938 girder-3.2.3.dev5/girder/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13355 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/assetstore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19091 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21532 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/folder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15915 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4577 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17147 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/resource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20748 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19063 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/api/v1/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.546938 girder-3.2.3.dev5/girder/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      358 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4755 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/cli/build.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24990 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/cli/mount.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/cli/serve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/cli/sftpd.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/cli/shell.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.546938 girder-3.2.3.dev5/girder/conf/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2337 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/conf/girder.dist.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8332 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10926 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.546938 girder-3.2.3.dev5/girder/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/_footer.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/_header.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      306 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/accountApproval.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/accountApproved.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/emailVerification.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/groupInvite.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/mail_templates/temporaryAccess.mako
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.550938 girder-3.2.3.dev5/girder/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3265 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4825 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6420 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/assetstore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16104 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20118 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36301 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/folder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15676 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21408 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65695 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/model_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8257 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/setting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4697 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22152 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/upload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24488 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6889 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15380 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.554938 girder-3.2.3.dev5/girder/utility/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6447 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1450 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/_cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/_hash_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17371 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/abstract_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16381 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/acl_mixin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2477 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/assetstore_utilities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2545 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/error.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18720 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/filesystem_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/gridfs_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6345 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/mail_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/model_importer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6735 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4435 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/progress.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27265 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/s3_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6879 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2946 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/setting_utilities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7267 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/webroot.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/webroot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/utility/ziputil.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.554938 girder-3.2.3.dev5/girder/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2332 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/Gruntfile.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.554938 girder-3.2.3.dev5/girder/web_client/eslint-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/eslint-config/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/eslint-config/.npmignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/eslint-config/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4715 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/eslint-config/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/eslint-config/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/eslint-config/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.554938 girder-3.2.3.dev5/girder/web_client/fontello/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/.npmignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/Gruntfile.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1225 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58174 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/fontello.config.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45252 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      641 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/fontello/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.554938 girder-3.2.3.dev5/girder/web_client/grunt_tasks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11066 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/grunt_tasks/build.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1717 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/grunt_tasks/swagger.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2742 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/grunt_tasks/test.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6587 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/grunt_tasks/webpack.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/grunt_tasks/webpack.paths.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/grunt_tasks/webpack.plugins.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/package.json.template
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.558938 girder-3.2.3.dev5/girder/web_client/pug-lint-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/pug-lint-config/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/pug-lint-config/.npmignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/pug-lint-config/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1017 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/pug-lint-config/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/pug-lint-config/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      432 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/pug-lint-config/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.558938 girder-3.2.3.dev5/girder/web_client/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.558938 girder-3.2.3.dev5/girder/web_client/src/assets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7590 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/assets/Girder_Mark.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4106 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/auth.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.562938 girder-3.2.3.dev5/girder/web_client/src/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/ApiKeyCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/AssetstoreCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10660 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/Collection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/CollectionCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/FileCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/FolderCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/GroupCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/ItemCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/UserCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/constants.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/dialog.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/events.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6698 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/misc.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.562938 girder-3.2.3.dev5/girder/web_client/src/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2841 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/AccessControlledModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/ApiKeyModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/AssetstoreModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/CollectionCreationPolicyModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10910 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/FileModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      886 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/FolderModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/GroupModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/ItemModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/MetadataMixin.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5688 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/Model.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5467 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/pluginUtils.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7581 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/rest.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/router.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7109 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.514938 girder-3.2.3.dev5/girder/web_client/src/stylesheets/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.562938 girder-3.2.3.dev5/girder/web_client/src/stylesheets/apidocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      831 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/apidocs/apidocs.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.566938 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/adminConsole.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/assetstores.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/collectionList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/collectionPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      939 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/frontPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/groupList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/groupPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/itemPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/plugins.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/searchResultsList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/systemConfig.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/userAccount.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/userList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/userPage.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.566938 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/footer.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/global.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/globalNav.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/header.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/headerUser.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/layout.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/layoutVars.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      622 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/loading.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/progressArea.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.566938 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1788 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/accessWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/browserWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/markdownWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1662 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/metadataWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/taskProgress.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/timelineWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/uploadWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3818 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.514938 girder-3.2.3.dev5/girder/web_client/src/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.570938 girder-3.2.3.dev5/girder/web_client/src/templates/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/adminConsole.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4103 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/assetstores.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/collectionList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/collectionPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/filesystemImport.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3003 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/frontPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/groupList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3962 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/groupPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1836 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/itemPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/plugins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/s3Import.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/searchResults.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/searchResultsType.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/systemConfiguration.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/userAccount.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/userList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/body/userPage.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.570938 girder-3.2.3.dev5/girder/web_client/src/templates/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/alert.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/layout.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/layoutFooter.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/layoutGlobalNav.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/layoutHeader.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      796 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/layoutHeaderUser.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/layoutProgressArea.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/loginDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1719 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/registerDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/layout/resetPasswordDialog.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.578938 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEditor.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEditorMixins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEditorNonModal.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEntry.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1918 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/apiKeyList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/browserWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/checkedActionsMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/collectionInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      565 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/confirmDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/dateTimeWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editApiKeyWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editCollectionWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editFileWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editFolderWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editGroupWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editItemWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/fileInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1229 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/fileList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/folderInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/folderList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupAdminList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3129 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupInviteDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupInviteList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupMemberList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupModList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/hierarchyPaginated.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3835 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/hierarchyWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      461 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/itemBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1088 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/itemList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/jsonMetadatumView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/loadingAnimation.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/markdownWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/metadataWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/metadatumEditWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/metadatumView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5858 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/newAssetstore.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/paginateWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/pluginConfigBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/rootSelectorWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/searchField.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/searchHelp.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/searchModeSelect.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/searchResults.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/sortCollectionWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/taskProgress.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/timeline.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/uploadWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/uploadWidgetNonModal.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      115 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/userOtpBegin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/userOtpDisable.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/templates/widgets/userOtpEnable.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.578938 girder-3.2.3.dev5/girder/web_client/src/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/utilities/EventStream.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/utilities/PluginUtils.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9489 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/utilities/S3UploadHandler.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/utilities/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.582938 girder-3.2.3.dev5/girder/web_client/src/utilities/jquery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/utilities/jquery/girderEnable.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2134 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/utilities/jquery/girderModal.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/version.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.582938 girder-3.2.3.dev5/girder/web_client/src/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/App.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2552 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/View.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.582938 girder-3.2.3.dev5/girder/web_client/src/views/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8160 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/AssetstoresView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6740 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/CollectionsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/FilesystemImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/FolderView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/FrontPageView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11859 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/GroupView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/GroupsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/PluginsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/S3ImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/SearchResultsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7137 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/SystemConfigurationView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6266 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/UserAccountView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/UsersView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/body/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.586938 girder-3.2.3.dev5/girder/web_client/src/views/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/FooterView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3163 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/GlobalNavView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/HeaderView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3708 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/ProgressListView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/RegisterView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2344 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/ResetPasswordView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/layout/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.590938 girder-3.2.3.dev5/girder/web_client/src/views/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15584 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/AccessWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4632 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/ApiKeyListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14503 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/BrowserWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2441 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/CheckedMenuWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5922 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/DateTimeRangeWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3302 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/DateTimeWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditApiKeyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5940 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditFileWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4203 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditFolderWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditGroupWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3797 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/FileInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5005 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/FolderInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3360 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/FolderListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupAdminsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1838 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupInvitesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5965 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupMembersWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2518 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupModsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42297 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14233 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/ItemListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/LoadingAnimation.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7648 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/MarkdownWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17158 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/MetadataWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3190 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/NewAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/PaginateWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6455 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/RootSelectorWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13112 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/SearchFieldWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4510 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/SearchPaginateWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1619 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/SortCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3042 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/TaskProgressWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6664 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/TimelineWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13690 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/UserOtpManagementWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2673 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/src/views/widgets/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.590938 girder-3.2.3.dev5/girder/web_client/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/static/.gitignore
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.590938 girder-3.2.3.dev5/girder/web_client/static/built/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/static/built/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/static/girder-swagger.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.590938 girder-3.2.3.dev5/girder/web_client/static/img/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/static/img/Girder_Favicon.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/girder/web_client/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/fake.jpg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.514938 girder-3.2.3.dev5/girder/web_client/test/lib/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4131 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6537 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70934 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8361 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/specRunner.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/testEnv.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/testFile.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/testFile.tsv
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/testFile.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/testFile2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46373 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/girder/web_client/test/testUtils.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.642939 girder-3.2.3.dev5/girder.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2721 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37817 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      327 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-02-14 15:48:37.000000 girder-3.2.3.dev5/girder.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   230120 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3293 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      271 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/.gitignore
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/audit_logs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/cleanup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1710 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/audit_logs/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4605 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/templates/folderActions.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.594938 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/authorized_upload/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3124 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/plugin_tests/upload_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/authorized_upload/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3781 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/autojoin/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3790 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/plugin_tests/autojoinSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/plugin_tests/autojoin_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/autojoin/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/dicom_viewer/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9428 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1286 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.598938 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13597 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      686 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/data/000000.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/data/000001.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/data/000002.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/data/000003.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11077 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/dicom_viewer/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/download_statistics/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/download_statistics/girder_download_statistics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/download_statistics/girder_download_statistics/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6503 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/download_statistics_test.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/files/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/files/txt1.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/files/txt2.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/download_statistics/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/lib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2186 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/google_analytics/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/plugin_tests/google_analytics_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/google_analytics/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/gravatar/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.602939 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1922 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2103 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/gravatar/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/plugin_tests/gravatar_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/gravatar/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7455 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/templates/config.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2070 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/hashsum_download/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-3.2.3.dev5/plugins/hashsum_download/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2371 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/hashsum_download/plugin_tests/hashsumSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/hashsum_download/plugin_tests/hashsum_download_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/hashsum_download/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/homepage/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.606938 girder-3.2.3.dev5/plugins/homepage/girder_homepage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2408 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      912 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6270 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1267 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/homepage/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6120 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/plugin_tests/homepageSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/plugin_tests/homepage_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1674 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/homepage/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/item_licenses/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2831 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.610938 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2499 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1480 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/ItemLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/item_licenses/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/plugin_tests/itemLicensesSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/plugin_tests/item_licenses_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/item_licenses/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/job_rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23250 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/models/job.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/JobStatus.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/collections/JobCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/models/JobModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.614939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/adminViewMenuItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/headerUserViewMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxContent.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2232 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobsGraphWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4906 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8414 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12083 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/jobs/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21567 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/plugin_tests/jobsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/plugin_tests/jobs_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/plugin_tests/local_job_impl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/jobs/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/girder_ldap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6318 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/templates/newServerTemplate.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4955 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/ldap/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/plugin_tests/ldap_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/ldap/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.618939 girder-3.2.3.dev5/plugins/oauth/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/girder_oauth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/bitbucket.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/box.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/github.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/globus.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/google.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/linkedin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/microsoft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/stylesheets/configView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2668 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2762 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/templates/oauthLoginView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/RegisterView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/oauth/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/plugin_tests/oauth_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/oauth/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.622938 girder-3.2.3.dev5/plugins/readme/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/girder_readme/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      470 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/stylesheets/readmeWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      101 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/templates/readmeWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/plugin_tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/readme/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/plugin_tests/data/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/plugin_tests/readmeSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/readme/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/sentry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/sentry/girder_sentry/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/sentry/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/terms/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/terms/girder_terms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.626939 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3270 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/stylesheets/termsAcceptance.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/templates/collectionInfoWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/templates/editCollectionTermsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/templates/termsAcceptance.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      717 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/terms/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14763 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/plugin_tests/termsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/plugin_tests/terms_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/terms/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/thumbnails/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3080 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/models/ThumbnailModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/flowView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.630939 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1510 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/flowView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/itemView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1306 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2021 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/worker.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13000 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/thumbnail_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/thumbnailsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/thumbnails/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16648 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/quota.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/stylesheets/userQuota.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3480 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.634939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2168 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      677 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/extendView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/plugins/user_quota/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16489 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/plugin_tests/userQuotaSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21142 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/plugin_tests/user_quota_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/user_quota/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/plugins/virtual_folders/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/plugins/virtual_folders/girder_virtual_folders/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/virtual_folders/girder_virtual_folders/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/plugins/virtual_folders/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/virtual_folders/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/virtual_folders/plugin_tests/virtual_folders_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/plugins/virtual_folders/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/MANIFEST.in
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/pytest_girder/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11468 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/pytest_girder/web_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/pytest_girder/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/requirements-dev.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.638939 girder-3.2.3.dev5/scripts/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:37.642939 girder-3.2.3.dev5/scripts/midas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/midas/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11413 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/midas/migrate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/midas/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/midas/walk_girder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1357 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/midas/walk_midas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/publicNames.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36686 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/publicNames.txt
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      604 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/scripts/test_names.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-02-14 15:48:37.642939 girder-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2614 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2024-02-14 15:48:27.000000 girder-3.2.3.dev5/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.205259 girder-3.2.3.dev7/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14387 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/config.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      710 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/create_ansible_subtree.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      316 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/generatePyEnvChecksum.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1118 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/publish_npm.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/publish_pypi.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.codecov.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.editorconfig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      258 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20024 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/CMakeLists.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4925 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2721 2024-02-14 18:46:58.205259 girder-3.2.3.dev7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1427 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/Vagrantfile
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/clients/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/clients/python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/clients/python/girder_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/girder_client/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/girder_client/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/devops/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/.yamllint
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/defaults/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/defaults/main.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/handlers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/handlers/main.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/library/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/library/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4135 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/library/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60712 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/library/girder.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/meta/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/meta/main.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/converge.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/test1.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/test2.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/test3.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/molecule.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/prepare.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/requirements.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22622 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_access.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1154 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3879 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3895 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_files.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9955 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7840 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1815 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2906 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_user.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/converge.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/molecule.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      276 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/prepare.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/pytest.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/tests/test_default.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/tasks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2472 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/tasks/main.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/tasks/nodejs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/devops/ansible-role-girder/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/templates/daemon/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/templates/daemon/girder.service.j2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/deployment-template/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/hosts.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/playbook.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      267 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/provision.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/requirements.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/vagrant/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/ansible.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2139 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/vagrant-playbook.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/vagrant-requirements.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.109259 girder-3.2.3.dev7/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/admin-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5288 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/api-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/build-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/changelog.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2379 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6551 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/configuration.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5131 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/dependencies.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/deployment-alternatives.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/deployment.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/dev-installation.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23262 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/developer-cookbook.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/developer-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18444 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/external-web-clients.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15086 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.109259 girder-3.2.3.dev7/docs/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   803025 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/images/dicom-viewer.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5181 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/license.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26440 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/migration-guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/mount.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38303 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/plugin-development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22537 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/plugins.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10888 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/python-client.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/requirements-docs.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5707 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/security.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1640 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/sftp.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/user-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14123 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/user-guide.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.109259 girder-3.2.3.dev7/girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11228 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.113259 girder-3.2.3.dev7/girder/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4349 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/access.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/api_docs.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/api_main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33164 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/describe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5196 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/docs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3483 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/filter_logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    51261 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7259 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/sftp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.113259 girder-3.2.3.dev7/girder/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13355 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/assetstore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19091 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21532 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/folder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15915 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4577 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17147 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/resource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20748 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/system.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19063 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      358 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4755 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/build.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24990 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/mount.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/serve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/sftpd.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/shell.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2337 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/conf/girder.dist.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8332 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10926 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/mail_templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/_footer.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/_header.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      306 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/accountApproval.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/accountApproved.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/emailVerification.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/groupInvite.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/temporaryAccess.mako
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3265 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4825 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6420 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/assetstore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16104 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20118 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36301 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/folder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15676 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21408 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65695 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/model_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8257 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/setting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4697 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22152 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/upload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24488 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6889 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15380 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.121259 girder-3.2.3.dev7/girder/utility/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6447 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1450 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/_hash_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17371 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/abstract_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16381 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/acl_mixin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2477 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/assetstore_utilities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2545 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/error.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18720 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/filesystem_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/gridfs_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6345 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/mail_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/model_importer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6735 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4435 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/progress.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27265 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/s3_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6879 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2946 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/setting_utilities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7267 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/system.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/webroot.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/webroot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/ziputil.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.121259 girder-3.2.3.dev7/girder/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2332 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/Gruntfile.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.121259 girder-3.2.3.dev7/girder/web_client/eslint-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/.npmignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4715 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.125259 girder-3.2.3.dev7/girder/web_client/fontello/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/.npmignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/Gruntfile.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1225 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    58174 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/fontello.config.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45252 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      641 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.125259 girder-3.2.3.dev7/girder/web_client/grunt_tasks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11066 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/build.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1717 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/swagger.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2742 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/test.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6587 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.paths.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.plugins.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/package.json.template
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.125259 girder-3.2.3.dev7/girder/web_client/pug-lint-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/.npmignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1017 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      432 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7590 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/assets/Girder_Mark.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4106 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/auth.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/collections/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/ApiKeyCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/AssetstoreCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10660 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/Collection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/CollectionCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/FileCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/FolderCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/GroupCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/ItemCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/UserCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/constants.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/dialog.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/events.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6698 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/misc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2841 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/AccessControlledModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/ApiKeyModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/AssetstoreModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/CollectionCreationPolicyModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10910 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/FileModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      886 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/FolderModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/GroupModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/ItemModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/MetadataMixin.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5688 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/Model.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5467 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/pluginUtils.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7581 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/rest.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/router.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7109 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.085259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/apidocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      831 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/apidocs/apidocs.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.133259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/adminConsole.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/assetstores.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/collectionList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/collectionPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      939 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/frontPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/itemPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/plugins.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/searchResultsList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/systemConfig.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userAccount.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userPage.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.133259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/footer.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/global.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/globalNav.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/header.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/headerUser.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/layout.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/layoutVars.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      622 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/loading.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/progressArea.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.137259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1788 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/accessWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/browserWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/markdownWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1662 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/metadataWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/taskProgress.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/timelineWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/uploadWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3818 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.085259 girder-3.2.3.dev7/girder/web_client/src/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.137259 girder-3.2.3.dev7/girder/web_client/src/templates/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/adminConsole.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4103 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/assetstores.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/filesystemImport.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3003 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/frontPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/groupList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3962 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/groupPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1836 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/itemPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/plugins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/s3Import.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/searchResults.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/searchResultsType.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/systemConfiguration.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/userAccount.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/userList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/userPage.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.137259 girder-3.2.3.dev7/girder/web_client/src/templates/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/alert.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layout.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutFooter.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutGlobalNav.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutHeader.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      796 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutHeaderUser.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutProgressArea.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/loginDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1719 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/registerDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/resetPasswordDialog.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.145259 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditor.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditorMixins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditorNonModal.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEntry.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1918 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/apiKeyList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/browserWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/checkedActionsMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/collectionInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      565 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/confirmDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/dateTimeWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editApiKeyWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editCollectionWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFileWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFolderWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editGroupWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editItemWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1229 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupAdminList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3129 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupInviteDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupInviteList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupMemberList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupModList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyPaginated.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3835 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      461 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/itemBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1088 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/itemList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/jsonMetadatumView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/loadingAnimation.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/markdownWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadataWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadatumEditWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadatumView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5858 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/newAssetstore.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/paginateWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/pluginConfigBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/rootSelectorWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchField.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchHelp.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchModeSelect.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchResults.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/sortCollectionWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/taskProgress.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/timeline.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidgetNonModal.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      115 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpBegin.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpDisable.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpEnable.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/EventStream.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/PluginUtils.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9489 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/S3UploadHandler.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/girderEnable.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2134 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/girderModal.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/version.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/App.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2552 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/View.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/views/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/AdminView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8160 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/AssetstoresView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6740 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/FilesystemImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/FolderView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/FrontPageView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11859 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/GroupView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/GroupsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/PluginsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/S3ImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/SearchResultsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7137 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/SystemConfigurationView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6266 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/UserAccountView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/UserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/UsersView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.153259 girder-3.2.3.dev7/girder/web_client/src/views/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/FooterView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3163 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/GlobalNavView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderUserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3708 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/LoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/ProgressListView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/RegisterView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2344 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/ResetPasswordView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/src/views/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15584 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/AccessWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4632 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/ApiKeyListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14503 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/BrowserWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2441 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/CheckedMenuWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5922 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeRangeWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3302 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditApiKeyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5940 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFileWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4203 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFolderWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditGroupWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3797 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditItemWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5005 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupAdminsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1838 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupInvitesWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5965 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupMembersWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2518 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupModsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42297 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/HierarchyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14233 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/LoadingAnimation.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7648 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/MarkdownWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17158 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/MetadataWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3190 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/NewAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/PaginateWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6455 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/RootSelectorWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13112 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchFieldWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4510 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchPaginateWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1619 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/SortCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3042 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/TaskProgressWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6664 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/TimelineWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13690 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/UploadWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/UserOtpManagementWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2673 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/.gitignore
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/static/built/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/built/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/girder-swagger.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/static/img/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/img/Girder_Favicon.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/fake.jpg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.085259 girder-3.2.3.dev7/girder/web_client/test/lib/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4131 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6537 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70934 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8361 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/specRunner.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testEnv.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile.tsv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    46373 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testUtils.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/girder.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2721 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37817 2024-02-14 18:46:58.000000 girder-3.2.3.dev7/girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      327 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   230120 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3293 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      271 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/.gitignore
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/audit_logs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/cleanup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1710 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4605 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/mail_templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/folderActions.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3124 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/upload_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/autojoin/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3781 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3790 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/autojoinSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/autojoin_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9428 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1286 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13597 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      686 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000000.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000001.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000002.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000003.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11077 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/download_statistics/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/download_statistics/girder_download_statistics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/girder_download_statistics/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6503 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/download_statistics_test.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/files/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/files/txt1.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/files/txt2.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/lib/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2186 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/google_analytics_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1922 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2103 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/plugin_tests/gravatar_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/hashsum_download/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7455 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/templates/config.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2070 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2371 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/hashsumSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/hashsum_download_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2408 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      912 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6270 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1267 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6120 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/plugin_tests/homepageSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/plugin_tests/homepage_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1674 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/item_licenses/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2831 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2499 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1480 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ItemLicenseWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/itemLicensesSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/item_licenses_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/job_rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23250 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/job.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/JobStatus.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/collections/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/collections/JobCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/collections/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/JobModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/adminViewMenuItem.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/headerUserViewMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxContent.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2232 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobsGraphWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/AdminView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4906 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8414 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12083 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21567 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/jobsSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/jobs_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/local_job_impl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/ldap/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6318 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/newServerTemplate.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4955 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/plugin_tests/ldap_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/bitbucket.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/box.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/github.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/globus.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/google.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/linkedin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/microsoft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/configView.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2668 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2762 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/oauthLoginView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/LoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/RegisterView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/oauth/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/plugin_tests/oauth_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      470 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/stylesheets/readmeWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      101 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/templates/readmeWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/plugin_tests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/plugin_tests/data/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/plugin_tests/readmeSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/terms/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/terms/girder_terms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3270 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/termsAcceptance.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/collectionInfoWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/editCollectionTermsWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/termsAcceptance.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      717 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14763 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/plugin_tests/termsSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/plugin_tests/terms_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3080 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/models/ThumbnailModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/flowView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1510 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/flowView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/itemView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1306 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2021 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/worker.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13000 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/thumbnail_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/thumbnailsSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16648 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/quota.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/stylesheets/userQuota.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3480 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2168 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/CollectionView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      677 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/UserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/extendView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16489 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/userQuotaSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21142 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/user_quota_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/virtual_folders/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/virtual_folders/girder_virtual_folders/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/girder_virtual_folders/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/virtual_folders_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/MANIFEST.in
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/pytest_girder/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11468 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/web_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/requirements-dev.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/scripts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/scripts/midas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11413 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/migrate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/walk_girder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1357 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/walk_midas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/publicNames.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36686 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/publicNames.txt
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      604 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/test_names.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-02-14 18:46:58.205259 girder-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2614 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/tox.ini
```

### Comparing `girder-3.2.3.dev5/.circleci/Dockerfile` & `girder-3.2.3.dev7/.circleci/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/.circleci/config.yml` & `girder-3.2.3.dev7/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/.circleci/create_ansible_subtree.sh` & `girder-3.2.3.dev7/.circleci/create_ansible_subtree.sh`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/.circleci/publish_npm.sh` & `girder-3.2.3.dev7/.circleci/publish_npm.sh`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/.codecov.yml` & `girder-3.2.3.dev7/.codecov.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/CHANGELOG.rst` & `girder-3.2.3.dev7/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/CMakeLists.txt` & `girder-3.2.3.dev7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/CONTRIBUTING.rst` & `girder-3.2.3.dev7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/Dockerfile` & `girder-3.2.3.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/LICENSE` & `girder-3.2.3.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/PKG-INFO` & `girder-3.2.3.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-3.2.3.dev5/README.rst` & `girder-3.2.3.dev7/README.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/Vagrantfile` & `girder-3.2.3.dev7/Vagrantfile`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/clients/python/girder_client/__init__.py` & `girder-3.2.3.dev7/clients/python/girder_client/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/clients/python/girder_client/cli.py` & `girder-3.2.3.dev7/clients/python/girder_client/cli.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/clients/python/setup.py` & `girder-3.2.3.dev7/clients/python/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/LICENSE` & `girder-3.2.3.dev7/devops/ansible-role-girder/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/README.md` & `girder-3.2.3.dev7/devops/ansible-role-girder/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/library/README.md` & `girder-3.2.3.dev7/devops/ansible-role-girder/library/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/library/girder.py` & `girder-3.2.3.dev7/devops/ansible-role-girder/library/girder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/converge.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/converge.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/molecule.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/molecule.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_access.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_access.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_files.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_files.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/ansible-module/test_user.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_user.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/molecule.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/molecule/default/tests/test_default.py` & `girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/ansible-role-girder/tasks/main.yml` & `girder-3.2.3.dev7/devops/ansible-role-girder/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/deployment-template/playbook.yml` & `girder-3.2.3.dev7/devops/deployment-template/playbook.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/devops/vagrant/vagrant-playbook.yml` & `girder-3.2.3.dev7/devops/vagrant/vagrant-playbook.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/api-docs.rst` & `girder-3.2.3.dev7/docs/api-docs.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/conf.py` & `girder-3.2.3.dev7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/configuration.rst` & `girder-3.2.3.dev7/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/dependencies.rst` & `girder-3.2.3.dev7/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/deployment-alternatives.rst` & `girder-3.2.3.dev7/docs/deployment-alternatives.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/deployment.rst` & `girder-3.2.3.dev7/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/dev-installation.rst` & `girder-3.2.3.dev7/docs/dev-installation.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/developer-cookbook.rst` & `girder-3.2.3.dev7/docs/developer-cookbook.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/development.rst` & `girder-3.2.3.dev7/docs/development.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/external-web-clients.rst` & `girder-3.2.3.dev7/docs/external-web-clients.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/favicon.ico` & `girder-3.2.3.dev7/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/images/dicom-viewer.png` & `girder-3.2.3.dev7/docs/images/dicom-viewer.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/index.rst` & `girder-3.2.3.dev7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/license.png` & `girder-3.2.3.dev7/docs/license.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/migration-guide.rst` & `girder-3.2.3.dev7/docs/migration-guide.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/mount.rst` & `girder-3.2.3.dev7/docs/mount.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/plugin-development.rst` & `girder-3.2.3.dev7/docs/plugin-development.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/plugins.rst` & `girder-3.2.3.dev7/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/python-client.rst` & `girder-3.2.3.dev7/docs/python-client.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/security.rst` & `girder-3.2.3.dev7/docs/security.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/sftp.rst` & `girder-3.2.3.dev7/docs/sftp.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/docs/user-guide.rst` & `girder-3.2.3.dev7/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/__init__.py` & `girder-3.2.3.dev7/girder/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/access.py` & `girder-3.2.3.dev7/girder/api/access.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/api_docs.mako` & `girder-3.2.3.dev7/girder/api/api_docs.mako`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/api_main.py` & `girder-3.2.3.dev7/girder/api/api_main.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/describe.py` & `girder-3.2.3.dev7/girder/api/describe.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/docs.py` & `girder-3.2.3.dev7/girder/api/docs.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/filter_logging.py` & `girder-3.2.3.dev7/girder/api/filter_logging.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/rest.py` & `girder-3.2.3.dev7/girder/api/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/sftp.py` & `girder-3.2.3.dev7/girder/api/sftp.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/api_key.py` & `girder-3.2.3.dev7/girder/api/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/assetstore.py` & `girder-3.2.3.dev7/girder/api/v1/assetstore.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/collection.py` & `girder-3.2.3.dev7/girder/api/v1/collection.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/file.py` & `girder-3.2.3.dev7/girder/api/v1/file.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/folder.py` & `girder-3.2.3.dev7/girder/api/v1/folder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/group.py` & `girder-3.2.3.dev7/girder/api/v1/group.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/item.py` & `girder-3.2.3.dev7/girder/api/v1/item.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/notification.py` & `girder-3.2.3.dev7/girder/api/v1/notification.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/resource.py` & `girder-3.2.3.dev7/girder/api/v1/resource.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/system.py` & `girder-3.2.3.dev7/girder/api/v1/system.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/token.py` & `girder-3.2.3.dev7/girder/api/v1/token.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/api/v1/user.py` & `girder-3.2.3.dev7/girder/api/v1/user.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/cli/build.py` & `girder-3.2.3.dev7/girder/cli/build.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/cli/mount.py` & `girder-3.2.3.dev7/girder/cli/mount.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/cli/serve.py` & `girder-3.2.3.dev7/girder/cli/serve.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/cli/sftpd.py` & `girder-3.2.3.dev7/girder/cli/sftpd.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/cli/shell.py` & `girder-3.2.3.dev7/girder/cli/shell.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/conf/girder.dist.cfg` & `girder-3.2.3.dev7/girder/conf/girder.dist.cfg`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/constants.py` & `girder-3.2.3.dev7/girder/constants.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/events.py` & `girder-3.2.3.dev7/girder/events.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/exceptions.py` & `girder-3.2.3.dev7/girder/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/__init__.py` & `girder-3.2.3.dev7/girder/models/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/api_key.py` & `girder-3.2.3.dev7/girder/models/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/assetstore.py` & `girder-3.2.3.dev7/girder/models/assetstore.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/collection.py` & `girder-3.2.3.dev7/girder/models/collection.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/file.py` & `girder-3.2.3.dev7/girder/models/file.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/folder.py` & `girder-3.2.3.dev7/girder/models/folder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/group.py` & `girder-3.2.3.dev7/girder/models/group.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/item.py` & `girder-3.2.3.dev7/girder/models/item.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/model_base.py` & `girder-3.2.3.dev7/girder/models/model_base.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/notification.py` & `girder-3.2.3.dev7/girder/models/notification.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/setting.py` & `girder-3.2.3.dev7/girder/models/setting.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/token.py` & `girder-3.2.3.dev7/girder/models/token.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/upload.py` & `girder-3.2.3.dev7/girder/models/upload.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/models/user.py` & `girder-3.2.3.dev7/girder/models/user.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/plugin.py` & `girder-3.2.3.dev7/girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/settings.py` & `girder-3.2.3.dev7/girder/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/__init__.py` & `girder-3.2.3.dev7/girder/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/_cache.py` & `girder-3.2.3.dev7/girder/utility/_cache.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/_hash_state.py` & `girder-3.2.3.dev7/girder/utility/_hash_state.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/abstract_assetstore_adapter.py` & `girder-3.2.3.dev7/girder/utility/abstract_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/acl_mixin.py` & `girder-3.2.3.dev7/girder/utility/acl_mixin.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/assetstore_utilities.py` & `girder-3.2.3.dev7/girder/utility/assetstore_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/config.py` & `girder-3.2.3.dev7/girder/utility/config.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/filesystem_assetstore_adapter.py` & `girder-3.2.3.dev7/girder/utility/filesystem_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/gridfs_assetstore_adapter.py` & `girder-3.2.3.dev7/girder/utility/gridfs_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/mail_utils.py` & `girder-3.2.3.dev7/girder/utility/mail_utils.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/model_importer.py` & `girder-3.2.3.dev7/girder/utility/model_importer.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/path.py` & `girder-3.2.3.dev7/girder/utility/path.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/progress.py` & `girder-3.2.3.dev7/girder/utility/progress.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/s3_assetstore_adapter.py` & `girder-3.2.3.dev7/girder/utility/s3_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/search.py` & `girder-3.2.3.dev7/girder/utility/search.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/server.py` & `girder-3.2.3.dev7/girder/utility/server.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/setting_utilities.py` & `girder-3.2.3.dev7/girder/utility/setting_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/system.py` & `girder-3.2.3.dev7/girder/utility/system.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/webroot.mako` & `girder-3.2.3.dev7/girder/utility/webroot.mako`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/webroot.py` & `girder-3.2.3.dev7/girder/utility/webroot.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/utility/ziputil.py` & `girder-3.2.3.dev7/girder/utility/ziputil.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/Gruntfile.js` & `girder-3.2.3.dev7/girder/web_client/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/eslint-config/README.md` & `girder-3.2.3.dev7/girder/web_client/eslint-config/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/eslint-config/index.js` & `girder-3.2.3.dev7/girder/web_client/eslint-config/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/eslint-config/package.json` & `girder-3.2.3.dev7/girder/web_client/eslint-config/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/fontello/Gruntfile.js` & `girder-3.2.3.dev7/girder/web_client/fontello/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/fontello/README.md` & `girder-3.2.3.dev7/girder/web_client/fontello/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/fontello/fontello.config.json` & `girder-3.2.3.dev7/girder/web_client/fontello/fontello.config.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/fontello/package-lock.json` & `girder-3.2.3.dev7/girder/web_client/fontello/package-lock.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/fontello/package.json` & `girder-3.2.3.dev7/girder/web_client/fontello/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/grunt_tasks/build.js` & `girder-3.2.3.dev7/girder/web_client/grunt_tasks/build.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/grunt_tasks/swagger.js` & `girder-3.2.3.dev7/girder/web_client/grunt_tasks/swagger.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/grunt_tasks/test.js` & `girder-3.2.3.dev7/girder/web_client/grunt_tasks/test.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/grunt_tasks/webpack.config.js` & `girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.config.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/grunt_tasks/webpack.plugins.js` & `girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.plugins.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/package.json.template` & `girder-3.2.3.dev7/girder/web_client/package.json.template`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/pug-lint-config/README.md` & `girder-3.2.3.dev7/girder/web_client/pug-lint-config/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/pug-lint-config/index.js` & `girder-3.2.3.dev7/girder/web_client/pug-lint-config/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/assets/Girder_Mark.png` & `girder-3.2.3.dev7/girder/web_client/src/assets/Girder_Mark.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/auth.js` & `girder-3.2.3.dev7/girder/web_client/src/auth.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/collections/Collection.js` & `girder-3.2.3.dev7/girder/web_client/src/collections/Collection.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/collections/UserCollection.js` & `girder-3.2.3.dev7/girder/web_client/src/collections/UserCollection.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/collections/index.js` & `girder-3.2.3.dev7/girder/web_client/src/collections/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/dialog.js` & `girder-3.2.3.dev7/girder/web_client/src/dialog.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/index.js` & `girder-3.2.3.dev7/girder/web_client/src/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/misc.js` & `girder-3.2.3.dev7/girder/web_client/src/misc.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/AccessControlledModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/AccessControlledModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/ApiKeyModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/ApiKeyModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/AssetstoreModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/AssetstoreModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/CollectionCreationPolicyModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/CollectionCreationPolicyModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/FileModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/FileModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/FolderModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/FolderModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/GroupModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/GroupModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/ItemModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/ItemModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/MetadataMixin.js` & `girder-3.2.3.dev7/girder/web_client/src/models/MetadataMixin.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/Model.js` & `girder-3.2.3.dev7/girder/web_client/src/models/Model.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/UserModel.js` & `girder-3.2.3.dev7/girder/web_client/src/models/UserModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/models/index.js` & `girder-3.2.3.dev7/girder/web_client/src/models/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/package.json` & `girder-3.2.3.dev7/girder/web_client/src/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/rest.js` & `girder-3.2.3.dev7/girder/web_client/src/rest.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/router.js` & `girder-3.2.3.dev7/girder/web_client/src/router.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/routes.js` & `girder-3.2.3.dev7/girder/web_client/src/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/apidocs/apidocs.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/apidocs/apidocs.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/assetstores.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/assetstores.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/collectionList.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/collectionList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/frontPage.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/frontPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/groupList.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/groupPage.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/itemPage.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/itemPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/plugins.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/plugins.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/searchResultsList.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/searchResultsList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/systemConfig.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/systemConfig.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/userAccount.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userAccount.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/body/userList.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/global.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/global.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/globalNav.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/globalNav.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/layout.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/layout/loading.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/loading.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/accessWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/accessWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/markdownWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/markdownWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/metadataWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/taskProgress.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/taskProgress.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/timelineWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/timelineWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/uploadWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/uploadWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl` & `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/assetstores.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/assetstores.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/collectionList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/collectionPage.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/filesystemImport.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/filesystemImport.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/frontPage.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/frontPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/groupList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/groupList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/groupPage.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/groupPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/itemPage.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/itemPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/plugins.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/plugins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/s3Import.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/s3Import.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/systemConfiguration.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/systemConfiguration.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/userAccount.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/userAccount.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/userList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/userList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/body/userPage.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/body/userPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/layout/layoutHeaderUser.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutHeaderUser.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/layout/loginDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/layout/loginDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/layout/registerDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/layout/registerDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/layout/resetPasswordDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/layout/resetPasswordDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEditor.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditor.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEditorMixins.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditorMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/accessEntry.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEntry.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/apiKeyList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/apiKeyList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/browserWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/browserWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/checkedActionsMenu.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/checkedActionsMenu.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/collectionInfoDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/collectionInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/confirmDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/confirmDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editApiKeyWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editApiKeyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editCollectionWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editFileWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editFolderWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFolderWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editGroupWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editGroupWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/editItemWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editItemWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/fileInfoDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/fileList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/folderInfoDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/folderList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupAdminList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupAdminList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupInviteDialog.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupInviteDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupMemberList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupMemberList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/groupModList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupModList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/hierarchyPaginated.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyPaginated.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/hierarchyWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/itemList.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/itemList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/markdownWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/markdownWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/metadataWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadataWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/metadatumEditWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/newAssetstore.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/newAssetstore.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/rootSelectorWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/rootSelectorWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/sortCollectionWidget.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/sortCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/taskProgress.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/taskProgress.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/timeline.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/timeline.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/templates/widgets/userOtpEnable.pug` & `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpEnable.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/utilities/EventStream.js` & `girder-3.2.3.dev7/girder/web_client/src/utilities/EventStream.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/utilities/PluginUtils.js` & `girder-3.2.3.dev7/girder/web_client/src/utilities/PluginUtils.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/utilities/S3UploadHandler.js` & `girder-3.2.3.dev7/girder/web_client/src/utilities/S3UploadHandler.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/utilities/jquery/girderModal.js` & `girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/girderModal.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/App.js` & `girder-3.2.3.dev7/girder/web_client/src/views/App.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/View.js` & `girder-3.2.3.dev7/girder/web_client/src/views/View.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/AdminView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/AdminView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/AssetstoresView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/CollectionView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/CollectionsView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/FilesystemImportView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/FilesystemImportView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/FolderView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/FolderView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/FrontPageView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/GroupView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/GroupView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/GroupsView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/GroupsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/ItemView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/PluginsView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/PluginsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/S3ImportView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/S3ImportView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/SearchResultsView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/SearchResultsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/SystemConfigurationView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/SystemConfigurationView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/UserAccountView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/UserAccountView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/UserView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/UserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/UsersView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/UsersView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/body/index.js` & `girder-3.2.3.dev7/girder/web_client/src/views/body/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/FooterView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/FooterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/GlobalNavView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/GlobalNavView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/HeaderUserView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/HeaderView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/LoginView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/LoginView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/ProgressListView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/ProgressListView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/RegisterView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/ResetPasswordView.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/ResetPasswordView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/layout/index.js` & `girder-3.2.3.dev7/girder/web_client/src/views/layout/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/AccessWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/AccessWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/ApiKeyListWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/ApiKeyListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/BrowserWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/BrowserWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/CheckedMenuWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/CheckedMenuWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/CollectionInfoWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/DateTimeRangeWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeRangeWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/DateTimeWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditApiKeyWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditApiKeyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditAssetstoreWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditCollectionWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditFileWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFileWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditFolderWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFolderWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditGroupWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditGroupWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/EditItemWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/FileInfoWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/FileListWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/FolderInfoWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/FolderListWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupAdminsWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupAdminsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupInvitesWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupInvitesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupMembersWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupMembersWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/GroupModsWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupModsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/HierarchyWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/ItemListWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/MarkdownWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/MarkdownWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/MetadataWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/NewAssetstoreWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/NewAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/PaginateWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/PaginateWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/RootSelectorWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/RootSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/SearchFieldWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchFieldWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/SearchPaginateWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchPaginateWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/SortCollectionWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/SortCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/TaskProgressWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/TaskProgressWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/TimelineWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/TimelineWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/UploadWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/UserOtpManagementWidget.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/UserOtpManagementWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/src/views/widgets/index.js` & `girder-3.2.3.dev7/girder/web_client/src/views/widgets/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/static/girder-swagger.js` & `girder-3.2.3.dev7/girder/web_client/static/girder-swagger.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/static/img/Girder_Favicon.png` & `girder-3.2.3.dev7/girder/web_client/static/img/Girder_Favicon.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js` & `girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt` & `girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css` & `girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js` & `girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/specRunner.js` & `girder-3.2.3.dev7/girder/web_client/test/specRunner.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/testEnv.pug` & `girder-3.2.3.dev7/girder/web_client/test/testEnv.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder/web_client/test/testUtils.js` & `girder-3.2.3.dev7/girder/web_client/test/testUtils.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/girder.egg-info/PKG-INFO` & `girder-3.2.3.dev7/girder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-3.2.3.dev5/girder.egg-info/SOURCES.txt` & `girder-3.2.3.dev7/girder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/package-lock.json` & `girder-3.2.3.dev7/package-lock.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/package.json` & `girder-3.2.3.dev7/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/__init__.py` & `girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/cleanup.py` & `girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/cleanup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/audit_logs/girder_audit_logs/report.py` & `girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/report.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/audit_logs/setup.py` & `girder-3.2.3.dev7/plugins/audit_logs/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/__init__.py` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/rest.py` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/main.js` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/package.json` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js` & `girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js` & `girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/plugin_tests/upload_test.py` & `girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/upload_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/authorized_upload/setup.py` & `girder-3.2.3.dev7/plugins/authorized_upload/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/__init__.py` & `girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/settings.py` & `girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/package.json` & `girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/plugin_tests/autojoinSpec.js` & `girder-3.2.3.dev7/plugins/autojoin/plugin_tests/autojoinSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/plugin_tests/autojoin_test.py` & `girder-3.2.3.dev7/plugins/autojoin/plugin_tests/autojoin_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/autojoin/setup.py` & `girder-3.2.3.dev7/plugins/autojoin/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/__init__.py` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js` & `girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py` & `girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/dicom_viewer/setup.py` & `girder-3.2.3.dev7/plugins/dicom_viewer/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/download_statistics/girder_download_statistics/__init__.py` & `girder-3.2.3.dev7/plugins/download_statistics/girder_download_statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/download_statistics/plugin_tests/download_statistics_test.py` & `girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/download_statistics_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/download_statistics/setup.py` & `girder-3.2.3.dev7/plugins/download_statistics/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/rest.py` & `girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js` & `girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/main.js` & `girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/package.json` & `girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/plugin_tests/google_analytics_test.py` & `girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/google_analytics_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/google_analytics/setup.py` & `girder-3.2.3.dev7/plugins/google_analytics/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/__init__.py` & `girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/package.json` & `girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/gravatar/plugin_tests/gravatar_test.py` & `girder-3.2.3.dev7/plugins/gravatar/plugin_tests/gravatar_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/gravatar/setup.py` & `girder-3.2.3.dev7/plugins/gravatar/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/__init__.py` & `girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/main.js` & `girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/package.json` & `girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js` & `girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/plugin_tests/hashsumSpec.js` & `girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/hashsumSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/plugin_tests/hashsum_download_test.py` & `girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/hashsum_download_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/hashsum_download/setup.py` & `girder-3.2.3.dev7/plugins/hashsum_download/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/rest.py` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/settings.py` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/package.json` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js` & `girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/plugin_tests/homepageSpec.js` & `girder-3.2.3.dev7/plugins/homepage/plugin_tests/homepageSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/plugin_tests/homepage_test.py` & `girder-3.2.3.dev7/plugins/homepage/plugin_tests/homepage_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/homepage/setup.py` & `girder-3.2.3.dev7/plugins/homepage/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/__init__.py` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/rest.py` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/settings.py` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js` & `girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/plugin_tests/itemLicensesSpec.js` & `girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/itemLicensesSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/plugin_tests/item_licenses_test.py` & `girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/item_licenses_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/item_licenses/setup.py` & `girder-3.2.3.dev7/plugins/item_licenses/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/__init__.py` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/constants.py` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/constants.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/job_rest.py` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/job_rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/models/job.py` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/job.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/JobStatus.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/JobStatus.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/models/JobModel.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/JobModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/package.json` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/routes.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobList.pug` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js` & `girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/plugin_tests/jobsSpec.js` & `girder-3.2.3.dev7/plugins/jobs/plugin_tests/jobsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/plugin_tests/jobs_test.py` & `girder-3.2.3.dev7/plugins/jobs/plugin_tests/jobs_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/jobs/setup.py` & `girder-3.2.3.dev7/plugins/jobs/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/girder_ldap/__init__.py` & `girder-3.2.3.dev7/plugins/ldap/girder_ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/girder_ldap/settings.py` & `girder-3.2.3.dev7/plugins/ldap/girder_ldap/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/package.json` & `girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug` & `girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/girder_ldap/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/plugin_tests/ldap_test.py` & `girder-3.2.3.dev7/plugins/ldap/plugin_tests/ldap_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/ldap/setup.py` & `girder-3.2.3.dev7/plugins/ldap/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/__init__.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/base.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/base.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/bitbucket.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/bitbucket.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/box.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/box.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/github.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/github.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/globus.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/globus.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/google.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/google.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/linkedin.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/linkedin.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/providers/microsoft.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/microsoft.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/rest.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/settings.py` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/main.js` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/package.json` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/girder_oauth/web_client/views/RegisterView.js` & `girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/plugin_tests/oauth_test.py` & `girder-3.2.3.dev7/plugins/oauth/plugin_tests/oauth_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/oauth/setup.py` & `girder-3.2.3.dev7/plugins/oauth/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/readme/girder_readme/rest.py` & `girder-3.2.3.dev7/plugins/readme/girder_readme/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js` & `girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/readme/plugin_tests/readmeSpec.js` & `girder-3.2.3.dev7/plugins/readme/plugin_tests/readmeSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/readme/setup.py` & `girder-3.2.3.dev7/plugins/readme/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/sentry/girder_sentry/rest.py` & `girder-3.2.3.dev7/plugins/sentry/girder_sentry/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/sentry/girder_sentry/settings.py` & `girder-3.2.3.dev7/plugins/sentry/girder_sentry/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/package.json` & `girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/sentry/girder_sentry/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/sentry/setup.py` & `girder-3.2.3.dev7/plugins/sentry/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/__init__.py` & `girder-3.2.3.dev7/plugins/terms/girder_terms/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/models/CollectionModel.js` & `girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/models/CollectionModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/package.json` & `girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/routes.js` & `girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js` & `girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js` & `girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js` & `girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/plugin_tests/termsSpec.js` & `girder-3.2.3.dev7/plugins/terms/plugin_tests/termsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/plugin_tests/terms_test.py` & `girder-3.2.3.dev7/plugins/terms/plugin_tests/terms_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/terms/setup.py` & `girder-3.2.3.dev7/plugins/terms/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/__init__.py` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/rest.py` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/utils.py` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/utils.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/package.json` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/girder_thumbnails/worker.py` & `girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/worker.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm` & `girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/thumbnail_test.py` & `girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/thumbnail_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/plugin_tests/thumbnailsSpec.js` & `girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/thumbnailsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/thumbnails/setup.py` & `girder-3.2.3.dev7/plugins/thumbnails/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/__init__.py` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/quota.py` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/quota.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/settings.py` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/package.json` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/girder_user_quota/web_client/views/extendView.js` & `girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/extendView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/plugin_tests/userQuotaSpec.js` & `girder-3.2.3.dev7/plugins/user_quota/plugin_tests/userQuotaSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/plugin_tests/user_quota_test.py` & `girder-3.2.3.dev7/plugins/user_quota/plugin_tests/user_quota_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/user_quota/setup.py` & `girder-3.2.3.dev7/plugins/user_quota/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/virtual_folders/girder_virtual_folders/__init__.py` & `girder-3.2.3.dev7/plugins/virtual_folders/girder_virtual_folders/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/virtual_folders/plugin_tests/virtual_folders_test.py` & `girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/virtual_folders_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/plugins/virtual_folders/setup.py` & `girder-3.2.3.dev7/plugins/virtual_folders/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/LICENSE` & `girder-3.2.3.dev7/pytest_girder/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/pytest_girder/assertions.py` & `girder-3.2.3.dev7/pytest_girder/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/pytest_girder/fixtures.py` & `girder-3.2.3.dev7/pytest_girder/pytest_girder/fixtures.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/pytest_girder/plugin.py` & `girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/pytest_girder/plugin_registry.py` & `girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/pytest_girder/utils.py` & `girder-3.2.3.dev7/pytest_girder/pytest_girder/utils.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/pytest_girder/web_client.py` & `girder-3.2.3.dev7/pytest_girder/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/pytest_girder/setup.py` & `girder-3.2.3.dev7/pytest_girder/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/requirements-dev.txt` & `girder-3.2.3.dev7/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/midas/README.rst` & `girder-3.2.3.dev7/scripts/midas/README.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/midas/migrate.py` & `girder-3.2.3.dev7/scripts/midas/migrate.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/midas/walk_girder.py` & `girder-3.2.3.dev7/scripts/midas/walk_girder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/midas/walk_midas.py` & `girder-3.2.3.dev7/scripts/midas/walk_midas.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/publicNames.py` & `girder-3.2.3.dev7/scripts/publicNames.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/publicNames.txt` & `girder-3.2.3.dev7/scripts/publicNames.txt`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/scripts/test_names.sh` & `girder-3.2.3.dev7/scripts/test_names.sh`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/setup.cfg` & `girder-3.2.3.dev7/setup.cfg`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/setup.py` & `girder-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev5/tox.ini` & `girder-3.2.3.dev7/tox.ini`

 * *Files identical despite different names*

