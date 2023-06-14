# Comparing `tmp/girder-3.1.9.dev6.tar.gz` & `tmp/girder-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:24 2022, max compression
+gzip compressed data, was "dist/girder-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:25 2022, max compression
```

## Comparing `girder-3.1.9.dev6.tar` & `girder-3.1.9.dev8.tar`

### file list

```diff
@@ -1,976 +1,976 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      746 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.circleci/Dockerfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11589 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.circleci/config.yml
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      710 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.circleci/create_ansible_subtree.sh
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      295 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.circleci/generatePyEnvChecksum.sh
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1118 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.circleci/publish_npm.sh
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      360 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.circleci/publish_pypi.sh
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/clients/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/clients/python/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/clients/python/girder_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    68237 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/clients/python/girder_client/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13559 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/clients/python/girder_client/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/clients/python/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1778 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/clients/python/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/defaults/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/defaults/main.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/handlers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      338 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/handlers/main.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/library/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/library/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4135 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/library/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    60897 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/library/girder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/meta/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      343 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/meta/main.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/data/test1.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/data/test2.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/data/test3.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/converge.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1278 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/molecule.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      415 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/prepare.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/requirements.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22622 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_access.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1154 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3879 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3895 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_files.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9955 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7840 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1815 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2906 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_user.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1679 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/tests/test_default.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/converge.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      980 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/molecule.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/prepare.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/pytest.ini
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/tasks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2472 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/tasks/main.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/tasks/nodejs.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/ansible-role-girder/templates/daemon/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      322 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/templates/daemon/girder.service.j2
--rw-r--r--   0 circleci  (3434) circleci  (3434)      300 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/.yamllint
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4098 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/ansible-role-girder/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/deployment-template/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      425 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/deployment-template/hosts.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1014 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/deployment-template/playbook.yml
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      267 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/deployment-template/provision.sh
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/deployment-template/requirements.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/devops/vagrant/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/vagrant/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/vagrant/ansible.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2139 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/vagrant/vagrant-playbook.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/devops/vagrant/vagrant-requirements.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/docs/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/docs/images/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   803025 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/images/dicom-viewer.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/admin-docs.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5285 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/api-docs.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/build-docs.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/changelog.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2957 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5075 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/configuration.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5135 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/dependencies.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3882 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/deployment-alternatives.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4929 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/deployment.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/dev-installation.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23254 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/developer-cookbook.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/developer-docs.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18444 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/development.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6775 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/external-web-clients.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15086 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/favicon.ico
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5179 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/license.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26436 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/migration-guide.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1714 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/mount.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37935 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/plugin-development.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22537 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/plugins.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10421 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/python-client.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/requirements-docs.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/security.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1640 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/sftp.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/user-docs.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14239 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docs/user-guide.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/api/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/api/v1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5115 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/api_key.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13379 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/assetstore.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10904 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/collection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18950 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/file.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21589 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/folder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15937 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/group.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15972 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/item.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4601 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/notification.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17212 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/resource.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20403 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/system.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2089 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19087 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/v1/user.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4373 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/access.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3384 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/api_docs.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1133 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/api_main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30580 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/describe.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4918 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/docs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/filter_logging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    50370 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7283 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/api/sftp.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/cli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      358 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/cli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4765 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/cli/build.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18972 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/cli/mount.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1577 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/cli/serve.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/cli/sftpd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1642 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/cli/shell.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/conf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2337 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/conf/girder.dist.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/mail_templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      214 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/_footer.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/_header.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/accountApproval.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/accountApproved.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/emailVerification.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/groupInvite.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/mail_templates/temporaryAccess.mako
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3289 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4849 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/api_key.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6444 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/assetstore.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16189 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/collection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19907 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/file.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    36443 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/folder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15700 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/group.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21432 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/item.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    65297 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/model_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8281 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/notification.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5551 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/setting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4721 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21446 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/upload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24569 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/models/user.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/utility/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6471 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/_cache.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6231 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/_hash_state.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16939 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/abstract_assetstore_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16405 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/acl_mixin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2501 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/assetstore_utilities.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2569 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/error.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18744 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/filesystem_assetstore_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11783 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/gridfs_assetstore_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6369 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/mail_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/model_importer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6759 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/path.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4459 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/progress.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      884 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/resource.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26545 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/s3_assetstore_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2464 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/search.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6838 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/server.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2970 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/setting_utilities.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7170 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/system.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/webroot.mako
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4603 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/webroot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8148 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/utility/ziputil.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/.npmignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4255 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       84 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/package-lock.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      613 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/eslint-config/package.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/fontello/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/.npmignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/Gruntfile.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    52625 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/fontello.config.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37050 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/package-lock.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      614 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/fontello/package.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10983 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/build.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1345 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/swagger.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2668 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/test.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6587 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/webpack.config.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/webpack.paths.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      916 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/grunt_tasks/webpack.plugins.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/.npmignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      547 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       86 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/package-lock.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/pug-lint-config/package.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/assets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7590 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/assets/Girder_Mark.png
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/collections/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/ApiKeyCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/AssetstoreCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10660 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/Collection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/CollectionCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/FileCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/FolderCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/GroupCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/ItemCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      616 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/UserCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/collections/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2841 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/AccessControlledModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1045 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/ApiKeyModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/AssetstoreModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/CollectionCreationPolicyModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      346 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/CollectionModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10910 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/FileModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      886 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/FolderModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6427 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/GroupModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2284 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/ItemModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2964 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/MetadataMixin.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5688 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/Model.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5467 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/UserModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      671 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/models/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/apidocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      821 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/apidocs/apidocs.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/adminConsole.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      792 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/assetstores.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      697 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/collectionList.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      124 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/collectionPage.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      939 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/frontPage.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      695 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/groupList.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2133 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/groupPage.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1372 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/itemPage.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1125 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/plugins.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/searchResultsList.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/systemConfig.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/userAccount.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1321 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/userList.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/userPage.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      389 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/footer.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2850 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/global.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1803 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/globalNav.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      505 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/header.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      486 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/headerUser.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1322 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/layout.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      191 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/layoutVars.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/loading.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/progressArea.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/accessWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/browserWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3727 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1713 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/markdownWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/metadataWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1359 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      723 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/taskProgress.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      786 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/timelineWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      813 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/uploadWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3816 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/adminConsole.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4103 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/assetstores.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1484 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/collectionList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1307 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/collectionPage.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1887 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/filesystemImport.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3003 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/frontPage.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      944 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/groupList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3962 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/groupPage.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1836 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/itemPage.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      949 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/plugins.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/s3Import.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      425 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/searchResults.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      505 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/searchResultsType.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11102 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/systemConfiguration.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3634 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/userAccount.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/userList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1442 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/body/userPage.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      179 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/alert.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      396 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/layout.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/layoutFooter.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/layoutGlobalNav.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/layoutHeader.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      796 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/layoutHeaderUser.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/layoutProgressArea.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/loginDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1719 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/registerDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1035 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/layout/resetPasswordDialog.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      665 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEditor.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2211 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEditorMixins.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      188 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEditorNonModal.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1711 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEntry.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1918 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/apiKeyList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1126 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/browserWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1167 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/checkedActionsMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1273 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/collectionInfoDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/confirmDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      598 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      230 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/dateTimeWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1800 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editApiKeyWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4268 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      941 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editCollectionWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editFileWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      921 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editFolderWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2662 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editGroupWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      907 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editItemWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/fileInfoDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/fileList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/folderInfoDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/folderList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupAdminList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3129 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupInviteDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupInviteList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1421 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupMemberList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupModList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      858 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      631 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/hierarchyPaginated.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3835 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/hierarchyWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      461 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/itemBreadcrumb.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1088 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/itemList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      513 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/jsonMetadatumView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/loadingAnimation.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1501 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/markdownWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/metadataWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/metadatumEditWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/metadatumView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5858 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/newAssetstore.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/paginateWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      250 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/pluginConfigBreadcrumb.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/rootSelectorWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/searchField.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      343 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/searchHelp.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/searchModeSelect.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/searchResults.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/sortCollectionWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      647 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/taskProgress.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      642 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/timeline.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      490 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/uploadWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      235 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/uploadWidgetNonModal.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      115 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/userOtpBegin.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/userOtpDisable.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1684 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/templates/widgets/userOtpEnable.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/jquery/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/jquery/girderEnable.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2134 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/jquery/girderModal.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/EventStream.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1122 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/PluginUtils.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9489 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/S3UploadHandler.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      208 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/utilities/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/views/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/AdminView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8160 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/AssetstoresView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6740 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/CollectionView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4353 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/CollectionsView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3146 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/FilesystemImportView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1679 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/FolderView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1305 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/FrontPageView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11859 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/GroupView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3535 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/GroupsView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6011 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/ItemView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/PluginsView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2907 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/S3ImportView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5544 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/SearchResultsView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7137 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/SystemConfigurationView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6266 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/UserAccountView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5437 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/UserView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4185 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/UsersView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1091 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/body/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      863 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/FooterView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3163 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/GlobalNavView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/HeaderUserView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2977 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/HeaderView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3708 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/LoginView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2190 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/ProgressListView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3805 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/RegisterView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2344 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/ResetPasswordView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/layout/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15584 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/AccessWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4632 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/ApiKeyListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14503 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/BrowserWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2441 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/CheckedMenuWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1275 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5922 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/DateTimeRangeWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3302 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/DateTimeWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4342 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditApiKeyWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5940 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3239 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditCollectionWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1959 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditFileWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4203 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditFolderWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4479 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditGroupWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3797 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditItemWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/FileInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5005 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/FileListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/FolderInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3360 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/FolderListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2901 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupAdminsWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1838 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupInvitesWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5965 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupMembersWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2518 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupModsWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    42037 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/HierarchyWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14231 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/ItemListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      446 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/LoadingAnimation.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7648 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/MarkdownWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17158 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/MetadataWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3190 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/NewAssetstoreWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1063 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/PaginateWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      928 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6455 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/RootSelectorWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13112 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/SearchFieldWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4510 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/SearchPaginateWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1619 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/SortCollectionWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3042 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/TaskProgressWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6664 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/TimelineWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13690 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/UploadWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3203 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/UserOtpManagementWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2673 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/widgets/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12010 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/App.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2552 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/View.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/views/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3905 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/auth.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/constants.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4733 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/dialog.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/events.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      682 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6698 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/misc.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1003 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/pluginUtils.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7463 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/rest.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1604 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/router.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7109 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/src/version.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/static/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/static/built/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/static/built/.gitignore
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/static/img/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1494 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/static/img/Girder_Favicon.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/static/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2634 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/static/girder-swagger.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/test/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/test/lib/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4131 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1061 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6537 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)    70934 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/fake.jpg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8364 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/specRunner.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      586 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testEnv.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testFile.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testFile.tsv
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testFile.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testFile2
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4290 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testFileBad.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)    46373 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/test/testUtils.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2332 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/Gruntfile.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/web_client/package.json.template
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11252 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8356 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10950 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/events.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2769 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6894 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/plugin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14980 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/girder/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/girder.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2244 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37832 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      328 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-02-23 16:09:23.000000 girder-3.1.9.dev6/girder.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/audit_logs/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1963 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      838 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/cleanup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/report.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1837 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/audit_logs/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/mail_templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      966 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/templates/folderActions.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1544 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      707 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4629 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/authorized_upload/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3124 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4624 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/plugin_tests/upload_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/authorized_upload/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1805 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3781 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/autojoin/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3790 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/plugin_tests/autojoinSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/plugin_tests/autojoin_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/autojoin/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1286 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13597 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      686 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9458 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/data/000000.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/data/000001.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/data/000002.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/data/000003.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11231 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/dicom_viewer/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/download_statistics/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/download_statistics/girder_download_statistics/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/download_statistics/girder_download_statistics/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/files/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/files/txt1.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/files/txt2.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6527 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/download_statistics_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/download_statistics/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/lib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2295 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      222 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2186 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      597 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      453 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/google_analytics/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      886 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/plugin_tests/google_analytics_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/google_analytics/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/models/UserModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1946 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/gravatar/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3130 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/plugin_tests/gravatar_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1794 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/gravatar/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/templates/config.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1147 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/hashsum_download/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2371 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/plugin_tests/hashsumSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13511 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/plugin_tests/hashsum_download_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1822 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/hashsum_download/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      912 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1472 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6270 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2432 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1695 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/girder_homepage/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/homepage/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6120 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/plugin_tests/homepageSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/plugin_tests/homepage_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1793 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/homepage/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      175 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2499 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/ItemLicenseWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1576 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      441 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4514 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/item_licenses/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15913 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/plugin_tests/itemLicensesSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12372 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/plugin_tests/item_licenses_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1718 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/item_licenses/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22898 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/models/job.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/collections/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      227 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/collections/JobCollection.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/collections/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/models/JobModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/models/index.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/adminViewMenuItem.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/headerUserViewMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxContent.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1940 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobList.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobsGraphWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      399 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/AdminView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2192 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4906 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8414 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12083 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8304 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11782 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/JobStatus.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/index.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      642 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1195 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8965 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/girder_jobs/job_rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/jobs/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21567 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/plugin_tests/jobsSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24912 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/plugin_tests/jobs_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/plugin_tests/local_job_impl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/jobs/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      899 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2592 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/templates/newServerTemplate.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4413 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5384 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/girder_ldap/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/ldap/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7614 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/plugin_tests/ldap_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/ldap/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      448 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9107 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3550 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/bitbucket.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2527 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3277 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/github.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2770 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/globus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2959 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/google.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2975 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/linkedin.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      458 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/stylesheets/configView.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2398 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2303 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      392 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/templates/oauthLoginView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6930 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/LoginView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2661 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/RegisterView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5015 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/girder_oauth/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/oauth/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63218 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/plugin_tests/oauth_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1832 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/oauth/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/stylesheets/readmeWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/templates/readmeWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      997 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      470 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/girder_readme/rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/readme/plugin_tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/plugin_tests/data/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/plugin_tests/readmeSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1662 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/readme/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/sentry/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      202 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2728 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      414 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/girder_sentry/settings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1758 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/sentry/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/models/CollectionModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/stylesheets/termsAcceptance.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/templates/collectionInfoWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      291 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/templates/editCollectionTermsWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/templates/termsAcceptance.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      717 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3087 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3408 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/girder_terms/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/terms/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14763 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/plugin_tests/termsSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6115 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/plugin_tests/terms_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/terms/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/models/ThumbnailModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/flowView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1510 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/flowView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/itemView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1306 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2021 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2370 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6350 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/worker.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35946 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13024 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/thumbnail_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2205 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/thumbnailsSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1886 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/thumbnails/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      154 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3788 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/stylesheets/userQuota.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      240 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1337 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3480 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/utilities/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/CollectionView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3357 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6817 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      241 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/UserView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/extendView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      559 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      898 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16560 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/quota.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/user_quota/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16489 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/plugin_tests/userQuotaSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21166 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/plugin_tests/user_quota_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1813 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/user_quota/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/virtual_folders/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/virtual_folders/girder_virtual_folders/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8194 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/virtual_folders/girder_virtual_folders/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/plugins/virtual_folders/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/virtual_folders/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6178 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/virtual_folders/plugin_tests/virtual_folders_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1764 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/virtual_folders/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      271 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/plugins/.gitignore
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/pytest_girder/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6446 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2671 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11116 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5970 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/pytest_girder/web_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1266 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/pytest_girder/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/scripts/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/scripts/midas/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1617 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/midas/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11419 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/midas/migrate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/midas/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1237 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/midas/walk_girder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1357 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/midas/walk_midas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4090 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/publicNames.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    36226 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/publicNames.txt
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      604 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/scripts/test_names.sh
--rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.codecov.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.dockerignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.editorconfig
--rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19992 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/CHANGELOG.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/CMakeLists.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4925 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/Dockerfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1468 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1427 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/Vagrantfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)      256 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/docker-compose.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)   235957 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/package-lock.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6055 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/readthedocs.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/requirements-dev.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2727 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4013 2022-02-23 16:09:15.000000 girder-3.1.9.dev6/tox.ini
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2244 2022-02-23 16:09:24.000000 girder-3.1.9.dev6/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      746 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.circleci/Dockerfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11589 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.circleci/config.yml
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      710 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.circleci/create_ansible_subtree.sh
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      295 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.circleci/generatePyEnvChecksum.sh
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1118 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.circleci/publish_npm.sh
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      360 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.circleci/publish_pypi.sh
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/clients/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/clients/python/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/clients/python/girder_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    68237 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/clients/python/girder_client/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13559 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/clients/python/girder_client/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/clients/python/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1778 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/clients/python/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/defaults/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/defaults/main.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/handlers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      338 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/handlers/main.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/library/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/library/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4135 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/library/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    60897 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/library/girder.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/meta/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      343 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/meta/main.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/data/test1.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/data/test2.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/data/test3.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/converge.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1278 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/molecule.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      415 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/prepare.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/requirements.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22622 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_access.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1154 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3879 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3895 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_files.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9955 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7840 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1815 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2906 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_user.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1679 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/tests/test_default.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/converge.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      980 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/molecule.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/prepare.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/pytest.ini
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/tasks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2472 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/tasks/main.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/tasks/nodejs.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/ansible-role-girder/templates/daemon/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      322 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/templates/daemon/girder.service.j2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      300 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/.yamllint
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4098 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/ansible-role-girder/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/deployment-template/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      425 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/deployment-template/hosts.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1014 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/deployment-template/playbook.yml
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      267 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/deployment-template/provision.sh
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/deployment-template/requirements.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/devops/vagrant/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/vagrant/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/vagrant/ansible.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2139 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/vagrant/vagrant-playbook.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/devops/vagrant/vagrant-requirements.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/docs/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/docs/images/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   803025 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/images/dicom-viewer.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/admin-docs.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5285 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/api-docs.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/build-docs.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/changelog.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2957 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/conf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5075 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/configuration.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5135 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/dependencies.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3882 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/deployment-alternatives.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4929 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/deployment.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/dev-installation.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23254 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/developer-cookbook.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/developer-docs.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18444 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/development.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6775 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/external-web-clients.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15086 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/favicon.ico
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5179 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/index.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/license.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26436 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/migration-guide.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1714 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/mount.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37935 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/plugin-development.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22537 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/plugins.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10421 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/python-client.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/requirements-docs.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/security.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1640 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/sftp.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/user-docs.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14239 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docs/user-guide.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/api/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/api/v1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5115 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/api_key.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13379 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/assetstore.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10904 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/collection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18950 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/file.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21589 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/folder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15937 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/group.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15972 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/item.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4601 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/notification.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17212 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/resource.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20403 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/system.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2089 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19087 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/v1/user.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4373 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/access.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3384 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/api_docs.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1133 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/api_main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30580 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/describe.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4918 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/docs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/filter_logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    50370 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7283 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/api/sftp.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/cli/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      358 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/cli/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4765 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/cli/build.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18972 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/cli/mount.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1577 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/cli/serve.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/cli/sftpd.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1642 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/cli/shell.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/conf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2337 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/conf/girder.dist.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/mail_templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      214 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/_footer.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/_header.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/accountApproval.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/accountApproved.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/emailVerification.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/groupInvite.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/mail_templates/temporaryAccess.mako
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3289 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4849 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/api_key.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6444 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/assetstore.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16189 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/collection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19907 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/file.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    36443 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/folder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15700 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/group.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21432 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/item.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    65297 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/model_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8281 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/notification.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5551 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/setting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4721 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21446 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/upload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24569 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/models/user.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/utility/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6471 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/_cache.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6231 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/_hash_state.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16939 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/abstract_assetstore_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16405 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/acl_mixin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2501 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/assetstore_utilities.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2569 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/error.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18744 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/filesystem_assetstore_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11783 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/gridfs_assetstore_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6369 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/mail_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/model_importer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6759 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/path.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4459 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/progress.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      884 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/resource.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26545 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/s3_assetstore_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2464 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/search.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6838 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/server.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2970 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/setting_utilities.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7170 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/system.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/webroot.mako
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4603 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/webroot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8148 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/utility/ziputil.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/.npmignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4255 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       84 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/package-lock.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      613 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/eslint-config/package.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/fontello/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/.npmignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/Gruntfile.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52625 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/fontello.config.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37050 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/package-lock.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      614 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/fontello/package.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10983 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/build.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1345 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/swagger.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2668 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/test.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6587 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/webpack.config.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/webpack.paths.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      916 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/grunt_tasks/webpack.plugins.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/.npmignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      547 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       86 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/package-lock.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/pug-lint-config/package.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/assets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7590 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/assets/Girder_Mark.png
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/collections/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/ApiKeyCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/AssetstoreCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10660 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/Collection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/CollectionCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/FileCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/FolderCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/GroupCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/ItemCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      616 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/UserCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/collections/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2841 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/AccessControlledModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1045 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/ApiKeyModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/AssetstoreModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/CollectionCreationPolicyModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      346 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/CollectionModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10910 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/FileModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      886 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/FolderModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6427 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/GroupModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2284 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/ItemModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2964 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/MetadataMixin.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5688 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/Model.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5467 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/UserModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      671 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/models/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/apidocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      821 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/apidocs/apidocs.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/adminConsole.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      792 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/assetstores.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      697 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/collectionList.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      124 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/collectionPage.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      939 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/frontPage.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      695 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/groupList.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2133 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/groupPage.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1372 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/itemPage.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1125 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/plugins.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/searchResultsList.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/systemConfig.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/userAccount.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1321 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/userList.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/userPage.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      389 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/footer.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2850 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/global.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1803 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/globalNav.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      505 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/header.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      486 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/headerUser.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1322 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/layout.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      191 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/layoutVars.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/loading.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/progressArea.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/accessWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/browserWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3727 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1713 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/markdownWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/metadataWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1359 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      723 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/taskProgress.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      786 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/timelineWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      813 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/uploadWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3816 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/adminConsole.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4103 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/assetstores.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1484 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/collectionList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1307 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/collectionPage.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1887 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/filesystemImport.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3003 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/frontPage.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      944 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/groupList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3962 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/groupPage.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1836 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/itemPage.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      949 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/plugins.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/s3Import.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      425 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/searchResults.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      505 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/searchResultsType.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11102 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/systemConfiguration.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3634 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/userAccount.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/userList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1442 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/body/userPage.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      179 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/alert.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      396 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/layout.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/layoutFooter.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/layoutGlobalNav.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/layoutHeader.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      796 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/layoutHeaderUser.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/layoutProgressArea.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/loginDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1719 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/registerDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1035 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/layout/resetPasswordDialog.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      665 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEditor.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2211 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEditorMixins.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      188 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEditorNonModal.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1711 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEntry.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1918 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/apiKeyList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1126 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/browserWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1167 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/checkedActionsMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1273 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/collectionInfoDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/confirmDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      598 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      230 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/dateTimeWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1800 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editApiKeyWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4268 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      941 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editCollectionWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editFileWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      921 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editFolderWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2662 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editGroupWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      907 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editItemWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/fileInfoDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/fileList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/folderInfoDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/folderList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupAdminList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3129 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupInviteDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupInviteList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1421 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupMemberList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupModList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      858 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      631 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/hierarchyPaginated.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3835 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/hierarchyWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      461 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/itemBreadcrumb.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1088 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/itemList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      513 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/jsonMetadatumView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/loadingAnimation.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1501 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/markdownWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/metadataWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/metadatumEditWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/metadatumView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5858 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/newAssetstore.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/paginateWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      250 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/pluginConfigBreadcrumb.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/rootSelectorWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/searchField.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      343 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/searchHelp.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/searchModeSelect.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/searchResults.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/sortCollectionWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      647 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/taskProgress.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      642 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/timeline.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      490 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/uploadWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      235 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/uploadWidgetNonModal.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      115 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/userOtpBegin.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/userOtpDisable.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1684 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/templates/widgets/userOtpEnable.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/jquery/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/jquery/girderEnable.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2134 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/jquery/girderModal.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/EventStream.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1122 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/PluginUtils.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9489 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/S3UploadHandler.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      208 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/utilities/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/views/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/AdminView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8160 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/AssetstoresView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6740 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/CollectionView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4353 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/CollectionsView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3146 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/FilesystemImportView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1679 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/FolderView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1305 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/FrontPageView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11859 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/GroupView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3535 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/GroupsView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6011 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/ItemView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/PluginsView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2907 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/S3ImportView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5544 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/SearchResultsView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7137 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/SystemConfigurationView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6266 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/UserAccountView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5437 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/UserView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4185 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/UsersView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1091 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/body/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      863 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/FooterView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3163 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/GlobalNavView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/HeaderUserView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2977 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/HeaderView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3708 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/LoginView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2190 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/ProgressListView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3805 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/RegisterView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2344 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/ResetPasswordView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/layout/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15584 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/AccessWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4632 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/ApiKeyListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14503 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/BrowserWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2441 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/CheckedMenuWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1275 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5922 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/DateTimeRangeWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3302 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/DateTimeWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4342 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditApiKeyWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5940 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3239 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1959 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditFileWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4203 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditFolderWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4479 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditGroupWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3797 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditItemWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/FileInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5005 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/FileListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/FolderInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3360 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/FolderListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2901 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupAdminsWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1838 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupInvitesWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5965 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupMembersWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2518 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupModsWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    42037 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/HierarchyWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14231 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/ItemListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      446 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/LoadingAnimation.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7648 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/MarkdownWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17158 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/MetadataWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3190 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/NewAssetstoreWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1063 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/PaginateWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      928 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6455 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/RootSelectorWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13112 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/SearchFieldWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4510 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/SearchPaginateWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1619 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/SortCollectionWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3042 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/TaskProgressWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6664 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/TimelineWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13690 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/UploadWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3203 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/UserOtpManagementWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2673 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/widgets/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12010 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/App.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2552 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/View.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/views/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3905 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/auth.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/constants.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4733 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/dialog.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/events.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      682 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6698 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/misc.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1003 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/pluginUtils.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7463 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/rest.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1604 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/router.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7109 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/src/version.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/static/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/static/built/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/static/built/.gitignore
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/static/img/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1494 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/static/img/Girder_Favicon.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/static/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2634 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/static/girder-swagger.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/test/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/test/lib/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4131 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1061 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6537 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    70934 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/fake.jpg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8364 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/specRunner.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      586 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testEnv.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testFile.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testFile.tsv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testFile.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testFile2
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4290 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testFileBad.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    46373 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/test/testUtils.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2332 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/Gruntfile.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/web_client/package.json.template
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11252 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8356 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10950 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/events.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2769 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6894 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/plugin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14980 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/girder/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2244 2022-02-23 17:41:23.000000 girder-3.1.9.dev8/girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37832 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:23.000000 girder-3.1.9.dev8/girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      328 2022-02-23 17:41:23.000000 girder-3.1.9.dev8/girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:23.000000 girder-3.1.9.dev8/girder.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2022-02-23 17:41:23.000000 girder-3.1.9.dev8/girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-02-23 17:41:23.000000 girder-3.1.9.dev8/girder.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/audit_logs/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1963 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      838 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/cleanup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/report.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1837 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/audit_logs/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/mail_templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      966 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/templates/folderActions.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1544 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      707 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4629 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/authorized_upload/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3124 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4624 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/plugin_tests/upload_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/authorized_upload/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1805 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3781 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/autojoin/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3790 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/plugin_tests/autojoinSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/plugin_tests/autojoin_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/autojoin/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1286 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13597 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      686 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9458 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/data/000000.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/data/000001.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/data/000002.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/data/000003.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11231 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/dicom_viewer/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/download_statistics/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/download_statistics/girder_download_statistics/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/download_statistics/girder_download_statistics/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/files/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/files/txt1.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/files/txt2.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6527 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/download_statistics_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/download_statistics/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/lib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2295 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      222 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2186 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      597 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      453 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/google_analytics/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      886 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/plugin_tests/google_analytics_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/google_analytics/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/models/UserModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1946 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/gravatar/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3130 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/plugin_tests/gravatar_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1794 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/gravatar/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/templates/config.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1147 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/hashsum_download/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2371 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/plugin_tests/hashsumSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13511 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/plugin_tests/hashsum_download_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1822 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/hashsum_download/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      912 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1472 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6270 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2432 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1695 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/girder_homepage/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/homepage/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6120 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/plugin_tests/homepageSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/plugin_tests/homepage_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1793 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/homepage/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      175 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2499 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/ItemLicenseWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1576 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      441 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4514 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/item_licenses/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15913 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/plugin_tests/itemLicensesSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12372 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/plugin_tests/item_licenses_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1718 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/item_licenses/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22898 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/models/job.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/collections/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      227 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/collections/JobCollection.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/collections/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/models/JobModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/models/index.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/adminViewMenuItem.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/headerUserViewMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxContent.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1940 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobList.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobsGraphWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      399 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/AdminView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2192 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4906 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8414 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12083 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8304 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11782 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/JobStatus.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/index.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      253 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      642 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1195 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1299 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8965 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/girder_jobs/job_rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/jobs/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21567 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/plugin_tests/jobsSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24912 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/plugin_tests/jobs_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/plugin_tests/local_job_impl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/jobs/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      899 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2592 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/templates/newServerTemplate.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4413 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5384 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/girder_ldap/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/ldap/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7614 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/plugin_tests/ldap_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/ldap/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      448 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9107 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3550 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/bitbucket.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2527 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3277 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/github.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2770 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/globus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2959 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/google.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2975 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/linkedin.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      458 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/stylesheets/configView.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2398 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2303 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      392 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/templates/oauthLoginView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6930 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/LoginView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2661 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/RegisterView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5015 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/girder_oauth/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/oauth/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    63218 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/plugin_tests/oauth_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1832 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/oauth/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/stylesheets/readmeWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/templates/readmeWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      997 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      470 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/girder_readme/rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/readme/plugin_tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/plugin_tests/data/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/plugin_tests/readmeSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1662 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/readme/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/sentry/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      202 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2728 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      414 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/girder_sentry/settings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1758 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/sentry/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/models/CollectionModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/stylesheets/termsAcceptance.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/templates/collectionInfoWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      291 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/templates/editCollectionTermsWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/templates/termsAcceptance.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      717 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3087 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3408 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/girder_terms/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/terms/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14763 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/plugin_tests/termsSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6115 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/plugin_tests/terms_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/terms/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/models/ThumbnailModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/flowView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1510 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/flowView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/itemView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1306 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2021 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2370 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6350 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/worker.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35946 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13024 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/thumbnail_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2205 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/thumbnailsSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1886 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/thumbnails/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/user_quota/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:24.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      154 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/models/CollectionModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/models/UserModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3788 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/stylesheets/userQuota.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      240 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1337 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3480 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/utilities/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/CollectionView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3357 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6817 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      241 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/UserView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/extendView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      559 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      898 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16560 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/quota.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/user_quota/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16489 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/plugin_tests/userQuotaSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21166 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/plugin_tests/user_quota_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1813 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/user_quota/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/virtual_folders/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/virtual_folders/girder_virtual_folders/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8194 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/virtual_folders/girder_virtual_folders/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/plugins/virtual_folders/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/virtual_folders/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6178 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/virtual_folders/plugin_tests/virtual_folders_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1764 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/virtual_folders/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      271 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/plugins/.gitignore
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/pytest_girder/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6446 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2671 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11116 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5970 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/pytest_girder/web_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1266 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/pytest_girder/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/scripts/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/scripts/midas/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1617 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/midas/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11419 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/midas/migrate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/midas/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1237 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/midas/walk_girder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1357 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/midas/walk_midas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4090 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/publicNames.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    36226 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/publicNames.txt
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      604 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/scripts/test_names.sh
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.codecov.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.dockerignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.editorconfig
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19992 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/CHANGELOG.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/CMakeLists.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4925 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/Dockerfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1468 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1427 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/Vagrantfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      256 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/docker-compose.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   235957 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/package-lock.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6055 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/readthedocs.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/requirements-dev.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2727 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4013 2022-02-23 17:41:16.000000 girder-3.1.9.dev8/tox.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2244 2022-02-23 17:41:25.000000 girder-3.1.9.dev8/PKG-INFO
```

### Comparing `girder-3.1.9.dev6/.circleci/Dockerfile` & `girder-3.1.9.dev8/.circleci/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/.circleci/config.yml` & `girder-3.1.9.dev8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/.circleci/create_ansible_subtree.sh` & `girder-3.1.9.dev8/.circleci/create_ansible_subtree.sh`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/.circleci/publish_npm.sh` & `girder-3.1.9.dev8/.circleci/publish_npm.sh`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/clients/python/girder_client/__init__.py` & `girder-3.1.9.dev8/clients/python/girder_client/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/clients/python/girder_client/cli.py` & `girder-3.1.9.dev8/clients/python/girder_client/cli.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/clients/python/setup.py` & `girder-3.1.9.dev8/clients/python/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/library/README.md` & `girder-3.1.9.dev8/devops/ansible-role-girder/library/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/library/girder.py` & `girder-3.1.9.dev8/devops/ansible-role-girder/library/girder.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/converge.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/converge.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/molecule.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/molecule.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_access.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_access.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_files.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_files.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/ansible-module/test_user.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/ansible-module/test_user.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/tests/test_default.py` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/molecule/default/molecule.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/tasks/main.yml` & `girder-3.1.9.dev8/devops/ansible-role-girder/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/LICENSE` & `girder-3.1.9.dev8/devops/ansible-role-girder/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/ansible-role-girder/README.md` & `girder-3.1.9.dev8/devops/ansible-role-girder/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/deployment-template/playbook.yml` & `girder-3.1.9.dev8/devops/deployment-template/playbook.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/devops/vagrant/vagrant-playbook.yml` & `girder-3.1.9.dev8/devops/vagrant/vagrant-playbook.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/images/dicom-viewer.png` & `girder-3.1.9.dev8/docs/images/dicom-viewer.png`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/api-docs.rst` & `girder-3.1.9.dev8/docs/api-docs.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/conf.py` & `girder-3.1.9.dev8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/configuration.rst` & `girder-3.1.9.dev8/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/dependencies.rst` & `girder-3.1.9.dev8/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/deployment-alternatives.rst` & `girder-3.1.9.dev8/docs/deployment-alternatives.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/deployment.rst` & `girder-3.1.9.dev8/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/dev-installation.rst` & `girder-3.1.9.dev8/docs/dev-installation.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/developer-cookbook.rst` & `girder-3.1.9.dev8/docs/developer-cookbook.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/development.rst` & `girder-3.1.9.dev8/docs/development.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/external-web-clients.rst` & `girder-3.1.9.dev8/docs/external-web-clients.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/favicon.ico` & `girder-3.1.9.dev8/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/index.rst` & `girder-3.1.9.dev8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/license.png` & `girder-3.1.9.dev8/docs/license.png`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/migration-guide.rst` & `girder-3.1.9.dev8/docs/migration-guide.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/mount.rst` & `girder-3.1.9.dev8/docs/mount.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/plugin-development.rst` & `girder-3.1.9.dev8/docs/plugin-development.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/plugins.rst` & `girder-3.1.9.dev8/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/python-client.rst` & `girder-3.1.9.dev8/docs/python-client.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/security.rst` & `girder-3.1.9.dev8/docs/security.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/sftp.rst` & `girder-3.1.9.dev8/docs/sftp.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/docs/user-guide.rst` & `girder-3.1.9.dev8/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/api_key.py` & `girder-3.1.9.dev8/girder/api/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/assetstore.py` & `girder-3.1.9.dev8/girder/api/v1/assetstore.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/collection.py` & `girder-3.1.9.dev8/girder/api/v1/collection.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/file.py` & `girder-3.1.9.dev8/girder/api/v1/file.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/folder.py` & `girder-3.1.9.dev8/girder/api/v1/folder.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/group.py` & `girder-3.1.9.dev8/girder/api/v1/group.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/item.py` & `girder-3.1.9.dev8/girder/api/v1/item.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/notification.py` & `girder-3.1.9.dev8/girder/api/v1/notification.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/resource.py` & `girder-3.1.9.dev8/girder/api/v1/resource.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/system.py` & `girder-3.1.9.dev8/girder/api/v1/system.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/token.py` & `girder-3.1.9.dev8/girder/api/v1/token.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/v1/user.py` & `girder-3.1.9.dev8/girder/api/v1/user.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/access.py` & `girder-3.1.9.dev8/girder/api/access.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/api_docs.mako` & `girder-3.1.9.dev8/girder/api/api_docs.mako`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/api_main.py` & `girder-3.1.9.dev8/girder/api/api_main.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/describe.py` & `girder-3.1.9.dev8/girder/api/describe.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/docs.py` & `girder-3.1.9.dev8/girder/api/docs.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/filter_logging.py` & `girder-3.1.9.dev8/girder/api/filter_logging.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/rest.py` & `girder-3.1.9.dev8/girder/api/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/api/sftp.py` & `girder-3.1.9.dev8/girder/api/sftp.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/cli/build.py` & `girder-3.1.9.dev8/girder/cli/build.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/cli/mount.py` & `girder-3.1.9.dev8/girder/cli/mount.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/cli/serve.py` & `girder-3.1.9.dev8/girder/cli/serve.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/cli/sftpd.py` & `girder-3.1.9.dev8/girder/cli/sftpd.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/cli/shell.py` & `girder-3.1.9.dev8/girder/cli/shell.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/conf/girder.dist.cfg` & `girder-3.1.9.dev8/girder/conf/girder.dist.cfg`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/__init__.py` & `girder-3.1.9.dev8/girder/models/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/api_key.py` & `girder-3.1.9.dev8/girder/models/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/assetstore.py` & `girder-3.1.9.dev8/girder/models/assetstore.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/collection.py` & `girder-3.1.9.dev8/girder/models/collection.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/file.py` & `girder-3.1.9.dev8/girder/models/file.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/folder.py` & `girder-3.1.9.dev8/girder/models/folder.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/group.py` & `girder-3.1.9.dev8/girder/models/group.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/item.py` & `girder-3.1.9.dev8/girder/models/item.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/model_base.py` & `girder-3.1.9.dev8/girder/models/model_base.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/notification.py` & `girder-3.1.9.dev8/girder/models/notification.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/setting.py` & `girder-3.1.9.dev8/girder/models/setting.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/token.py` & `girder-3.1.9.dev8/girder/models/token.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/upload.py` & `girder-3.1.9.dev8/girder/models/upload.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/models/user.py` & `girder-3.1.9.dev8/girder/models/user.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/__init__.py` & `girder-3.1.9.dev8/girder/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/_cache.py` & `girder-3.1.9.dev8/girder/utility/_cache.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/_hash_state.py` & `girder-3.1.9.dev8/girder/utility/_hash_state.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/abstract_assetstore_adapter.py` & `girder-3.1.9.dev8/girder/utility/abstract_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/acl_mixin.py` & `girder-3.1.9.dev8/girder/utility/acl_mixin.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/assetstore_utilities.py` & `girder-3.1.9.dev8/girder/utility/assetstore_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/config.py` & `girder-3.1.9.dev8/girder/utility/config.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/filesystem_assetstore_adapter.py` & `girder-3.1.9.dev8/girder/utility/filesystem_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/gridfs_assetstore_adapter.py` & `girder-3.1.9.dev8/girder/utility/gridfs_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/mail_utils.py` & `girder-3.1.9.dev8/girder/utility/mail_utils.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/model_importer.py` & `girder-3.1.9.dev8/girder/utility/model_importer.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/path.py` & `girder-3.1.9.dev8/girder/utility/path.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/progress.py` & `girder-3.1.9.dev8/girder/utility/progress.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/resource.py` & `girder-3.1.9.dev8/girder/utility/resource.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/s3_assetstore_adapter.py` & `girder-3.1.9.dev8/girder/utility/s3_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/search.py` & `girder-3.1.9.dev8/girder/utility/search.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/server.py` & `girder-3.1.9.dev8/girder/utility/server.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/setting_utilities.py` & `girder-3.1.9.dev8/girder/utility/setting_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/system.py` & `girder-3.1.9.dev8/girder/utility/system.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/webroot.mako` & `girder-3.1.9.dev8/girder/utility/webroot.mako`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/webroot.py` & `girder-3.1.9.dev8/girder/utility/webroot.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/utility/ziputil.py` & `girder-3.1.9.dev8/girder/utility/ziputil.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/eslint-config/README.md` & `girder-3.1.9.dev8/girder/web_client/eslint-config/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/eslint-config/index.js` & `girder-3.1.9.dev8/girder/web_client/eslint-config/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/eslint-config/package.json` & `girder-3.1.9.dev8/girder/web_client/eslint-config/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/fontello/Gruntfile.js` & `girder-3.1.9.dev8/girder/web_client/fontello/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/fontello/README.md` & `girder-3.1.9.dev8/girder/web_client/fontello/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/fontello/fontello.config.json` & `girder-3.1.9.dev8/girder/web_client/fontello/fontello.config.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/fontello/package-lock.json` & `girder-3.1.9.dev8/girder/web_client/fontello/package-lock.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/fontello/package.json` & `girder-3.1.9.dev8/girder/web_client/fontello/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/grunt_tasks/build.js` & `girder-3.1.9.dev8/girder/web_client/grunt_tasks/build.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/grunt_tasks/swagger.js` & `girder-3.1.9.dev8/girder/web_client/grunt_tasks/swagger.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/grunt_tasks/test.js` & `girder-3.1.9.dev8/girder/web_client/grunt_tasks/test.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/grunt_tasks/webpack.config.js` & `girder-3.1.9.dev8/girder/web_client/grunt_tasks/webpack.config.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/grunt_tasks/webpack.plugins.js` & `girder-3.1.9.dev8/girder/web_client/grunt_tasks/webpack.plugins.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/pug-lint-config/README.md` & `girder-3.1.9.dev8/girder/web_client/pug-lint-config/README.md`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/pug-lint-config/index.js` & `girder-3.1.9.dev8/girder/web_client/pug-lint-config/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/assets/Girder_Mark.png` & `girder-3.1.9.dev8/girder/web_client/src/assets/Girder_Mark.png`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/collections/Collection.js` & `girder-3.1.9.dev8/girder/web_client/src/collections/Collection.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/collections/UserCollection.js` & `girder-3.1.9.dev8/girder/web_client/src/collections/UserCollection.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/collections/index.js` & `girder-3.1.9.dev8/girder/web_client/src/collections/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/AccessControlledModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/AccessControlledModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/ApiKeyModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/ApiKeyModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/AssetstoreModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/AssetstoreModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/CollectionCreationPolicyModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/CollectionCreationPolicyModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/FileModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/FileModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/FolderModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/FolderModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/GroupModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/GroupModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/ItemModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/ItemModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/MetadataMixin.js` & `girder-3.1.9.dev8/girder/web_client/src/models/MetadataMixin.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/Model.js` & `girder-3.1.9.dev8/girder/web_client/src/models/Model.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/UserModel.js` & `girder-3.1.9.dev8/girder/web_client/src/models/UserModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/models/index.js` & `girder-3.1.9.dev8/girder/web_client/src/models/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/apidocs/apidocs.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/apidocs/apidocs.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/assetstores.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/assetstores.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/collectionList.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/collectionList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/frontPage.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/frontPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/groupList.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/groupList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/groupPage.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/groupPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/itemPage.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/itemPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/plugins.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/plugins.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/searchResultsList.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/searchResultsList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/systemConfig.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/systemConfig.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/userAccount.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/userAccount.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/body/userList.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/body/userList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/global.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/global.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/globalNav.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/globalNav.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/layout.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/layout/loading.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/layout/loading.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/accessWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/accessWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/markdownWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/markdownWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/metadataWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/taskProgress.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/taskProgress.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/timelineWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/timelineWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/uploadWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/uploadWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl` & `girder-3.1.9.dev8/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/assetstores.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/assetstores.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/collectionList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/collectionList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/collectionPage.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/collectionPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/filesystemImport.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/filesystemImport.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/frontPage.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/frontPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/groupList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/groupList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/groupPage.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/groupPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/itemPage.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/itemPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/plugins.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/plugins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/s3Import.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/s3Import.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/systemConfiguration.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/systemConfiguration.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/userAccount.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/userAccount.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/userList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/userList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/body/userPage.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/body/userPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/layout/layoutHeaderUser.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/layout/layoutHeaderUser.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/layout/loginDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/layout/loginDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/layout/registerDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/layout/registerDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/layout/resetPasswordDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/layout/resetPasswordDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEditor.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEditor.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEditorMixins.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEditorMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/accessEntry.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/accessEntry.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/apiKeyList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/apiKeyList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/browserWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/browserWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/checkedActionsMenu.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/checkedActionsMenu.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/collectionInfoDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/collectionInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/confirmDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/confirmDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editApiKeyWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editApiKeyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editCollectionWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editFileWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editFileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editFolderWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editFolderWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editGroupWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editGroupWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/editItemWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/editItemWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/fileInfoDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/fileInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/fileList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/fileList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/folderInfoDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/folderInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/folderList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/folderList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupAdminList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupAdminList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupInviteDialog.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupInviteDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupMemberList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupMemberList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/groupModList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/groupModList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/hierarchyPaginated.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/hierarchyPaginated.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/hierarchyWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/hierarchyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/itemList.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/itemList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/markdownWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/markdownWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/metadataWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/metadataWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/metadatumEditWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/metadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/newAssetstore.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/newAssetstore.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/rootSelectorWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/rootSelectorWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/sortCollectionWidget.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/sortCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/taskProgress.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/taskProgress.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/timeline.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/timeline.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/templates/widgets/userOtpEnable.pug` & `girder-3.1.9.dev8/girder/web_client/src/templates/widgets/userOtpEnable.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/utilities/jquery/girderModal.js` & `girder-3.1.9.dev8/girder/web_client/src/utilities/jquery/girderModal.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/utilities/EventStream.js` & `girder-3.1.9.dev8/girder/web_client/src/utilities/EventStream.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/utilities/PluginUtils.js` & `girder-3.1.9.dev8/girder/web_client/src/utilities/PluginUtils.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/utilities/S3UploadHandler.js` & `girder-3.1.9.dev8/girder/web_client/src/utilities/S3UploadHandler.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/AdminView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/AdminView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/AssetstoresView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/CollectionView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/CollectionsView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/CollectionsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/FilesystemImportView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/FilesystemImportView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/FolderView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/FolderView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/FrontPageView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/GroupView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/GroupView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/GroupsView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/GroupsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/ItemView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/PluginsView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/PluginsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/S3ImportView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/S3ImportView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/SearchResultsView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/SearchResultsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/SystemConfigurationView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/SystemConfigurationView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/UserAccountView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/UserAccountView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/UserView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/UserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/UsersView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/UsersView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/body/index.js` & `girder-3.1.9.dev8/girder/web_client/src/views/body/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/FooterView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/FooterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/GlobalNavView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/GlobalNavView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/HeaderUserView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/HeaderView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/LoginView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/LoginView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/ProgressListView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/ProgressListView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/RegisterView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/ResetPasswordView.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/ResetPasswordView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/layout/index.js` & `girder-3.1.9.dev8/girder/web_client/src/views/layout/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/AccessWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/AccessWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/ApiKeyListWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/ApiKeyListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/BrowserWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/BrowserWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/CheckedMenuWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/CheckedMenuWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/CollectionInfoWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/DateTimeRangeWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/DateTimeRangeWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/DateTimeWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/DateTimeWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditApiKeyWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditApiKeyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditAssetstoreWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditCollectionWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditFileWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditFileWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditFolderWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditFolderWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditGroupWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditGroupWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/EditItemWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/FileInfoWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/FileListWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/FolderInfoWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/FolderInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/FolderListWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/FolderListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupAdminsWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupAdminsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupInvitesWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupInvitesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupMembersWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupMembersWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/GroupModsWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/GroupModsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/HierarchyWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/ItemListWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/ItemListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/MarkdownWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/MarkdownWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/MetadataWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/NewAssetstoreWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/NewAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/PaginateWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/PaginateWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/RootSelectorWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/RootSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/SearchFieldWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/SearchFieldWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/SearchPaginateWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/SearchPaginateWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/SortCollectionWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/SortCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/TaskProgressWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/TaskProgressWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/TimelineWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/TimelineWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/UploadWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/UserOtpManagementWidget.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/UserOtpManagementWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/widgets/index.js` & `girder-3.1.9.dev8/girder/web_client/src/views/widgets/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/App.js` & `girder-3.1.9.dev8/girder/web_client/src/views/App.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/views/View.js` & `girder-3.1.9.dev8/girder/web_client/src/views/View.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/auth.js` & `girder-3.1.9.dev8/girder/web_client/src/auth.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/dialog.js` & `girder-3.1.9.dev8/girder/web_client/src/dialog.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/index.js` & `girder-3.1.9.dev8/girder/web_client/src/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/misc.js` & `girder-3.1.9.dev8/girder/web_client/src/misc.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/package.json` & `girder-3.1.9.dev8/girder/web_client/src/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/rest.js` & `girder-3.1.9.dev8/girder/web_client/src/rest.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/router.js` & `girder-3.1.9.dev8/girder/web_client/src/router.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/src/routes.js` & `girder-3.1.9.dev8/girder/web_client/src/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/static/img/Girder_Favicon.png` & `girder-3.1.9.dev8/girder/web_client/static/img/Girder_Favicon.png`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/static/girder-swagger.js` & `girder-3.1.9.dev8/girder/web_client/static/girder-swagger.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js` & `girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt` & `girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css` & `girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js` & `girder-3.1.9.dev8/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/specRunner.js` & `girder-3.1.9.dev8/girder/web_client/test/specRunner.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/testEnv.pug` & `girder-3.1.9.dev8/girder/web_client/test/testEnv.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/testFileBad.csv` & `girder-3.1.9.dev8/girder/web_client/test/testFileBad.csv`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/test/testUtils.js` & `girder-3.1.9.dev8/girder/web_client/test/testUtils.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/Gruntfile.js` & `girder-3.1.9.dev8/girder/web_client/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/web_client/package.json.template` & `girder-3.1.9.dev8/girder/web_client/package.json.template`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/__init__.py` & `girder-3.1.9.dev8/girder/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/constants.py` & `girder-3.1.9.dev8/girder/constants.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/events.py` & `girder-3.1.9.dev8/girder/events.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/exceptions.py` & `girder-3.1.9.dev8/girder/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/plugin.py` & `girder-3.1.9.dev8/girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder/settings.py` & `girder-3.1.9.dev8/girder/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/girder.egg-info/PKG-INFO` & `girder-3.1.9.dev8/girder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-3.1.9.dev6/girder.egg-info/SOURCES.txt` & `girder-3.1.9.dev8/girder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/__init__.py` & `girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/cleanup.py` & `girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/cleanup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/audit_logs/girder_audit_logs/report.py` & `girder-3.1.9.dev8/plugins/audit_logs/girder_audit_logs/report.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/audit_logs/setup.py` & `girder-3.1.9.dev8/plugins/audit_logs/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/main.js` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/package.json` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/__init__.py` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/girder_authorized_upload/rest.py` & `girder-3.1.9.dev8/plugins/authorized_upload/girder_authorized_upload/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js` & `girder-3.1.9.dev8/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/plugin_tests/upload_test.py` & `girder-3.1.9.dev8/plugins/authorized_upload/plugin_tests/upload_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/authorized_upload/setup.py` & `girder-3.1.9.dev8/plugins/authorized_upload/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/web_client/package.json` & `girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/__init__.py` & `girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/girder_autojoin/settings.py` & `girder-3.1.9.dev8/plugins/autojoin/girder_autojoin/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/plugin_tests/autojoinSpec.js` & `girder-3.1.9.dev8/plugins/autojoin/plugin_tests/autojoinSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/plugin_tests/autojoin_test.py` & `girder-3.1.9.dev8/plugins/autojoin/plugin_tests/autojoin_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/autojoin/setup.py` & `girder-3.1.9.dev8/plugins/autojoin/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/__init__.py` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py` & `girder-3.1.9.dev8/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py` & `girder-3.1.9.dev8/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/dicom_viewer/setup.py` & `girder-3.1.9.dev8/plugins/dicom_viewer/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/download_statistics/girder_download_statistics/__init__.py` & `girder-3.1.9.dev8/plugins/download_statistics/girder_download_statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/download_statistics/plugin_tests/download_statistics_test.py` & `girder-3.1.9.dev8/plugins/download_statistics/plugin_tests/download_statistics_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/download_statistics/setup.py` & `girder-3.1.9.dev8/plugins/download_statistics/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js` & `girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/main.js` & `girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/web_client/package.json` & `girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/girder_google_analytics/rest.py` & `girder-3.1.9.dev8/plugins/google_analytics/girder_google_analytics/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/plugin_tests/google_analytics_test.py` & `girder-3.1.9.dev8/plugins/google_analytics/plugin_tests/google_analytics_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/google_analytics/setup.py` & `girder-3.1.9.dev8/plugins/google_analytics/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/web_client/package.json` & `girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/gravatar/girder_gravatar/__init__.py` & `girder-3.1.9.dev8/plugins/gravatar/girder_gravatar/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/gravatar/plugin_tests/gravatar_test.py` & `girder-3.1.9.dev8/plugins/gravatar/plugin_tests/gravatar_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/gravatar/setup.py` & `girder-3.1.9.dev8/plugins/gravatar/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js` & `girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/main.js` & `girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/web_client/package.json` & `girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/girder_hashsum_download/__init__.py` & `girder-3.1.9.dev8/plugins/hashsum_download/girder_hashsum_download/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/plugin_tests/hashsumSpec.js` & `girder-3.1.9.dev8/plugins/hashsum_download/plugin_tests/hashsumSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/plugin_tests/hashsum_download_test.py` & `girder-3.1.9.dev8/plugins/hashsum_download/plugin_tests/hashsum_download_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/hashsum_download/setup.py` & `girder-3.1.9.dev8/plugins/hashsum_download/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/web_client/package.json` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/rest.py` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/girder_homepage/settings.py` & `girder-3.1.9.dev8/plugins/homepage/girder_homepage/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/plugin_tests/homepageSpec.js` & `girder-3.1.9.dev8/plugins/homepage/plugin_tests/homepageSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/plugin_tests/homepage_test.py` & `girder-3.1.9.dev8/plugins/homepage/plugin_tests/homepage_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/homepage/setup.py` & `girder-3.1.9.dev8/plugins/homepage/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/__init__.py` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/rest.py` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/girder_item_licenses/settings.py` & `girder-3.1.9.dev8/plugins/item_licenses/girder_item_licenses/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/plugin_tests/itemLicensesSpec.js` & `girder-3.1.9.dev8/plugins/item_licenses/plugin_tests/itemLicensesSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/plugin_tests/item_licenses_test.py` & `girder-3.1.9.dev8/plugins/item_licenses/plugin_tests/item_licenses_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/item_licenses/setup.py` & `girder-3.1.9.dev8/plugins/item_licenses/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/models/job.py` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/models/job.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/models/JobModel.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/models/JobModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobList.pug` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/JobStatus.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/JobStatus.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/package.json` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/web_client/routes.js` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/__init__.py` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/constants.py` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/constants.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/girder_jobs/job_rest.py` & `girder-3.1.9.dev8/plugins/jobs/girder_jobs/job_rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/plugin_tests/jobsSpec.js` & `girder-3.1.9.dev8/plugins/jobs/plugin_tests/jobsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/plugin_tests/jobs_test.py` & `girder-3.1.9.dev8/plugins/jobs/plugin_tests/jobs_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/jobs/setup.py` & `girder-3.1.9.dev8/plugins/jobs/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug` & `girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/girder_ldap/web_client/package.json` & `girder-3.1.9.dev8/plugins/ldap/girder_ldap/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/girder_ldap/__init__.py` & `girder-3.1.9.dev8/plugins/ldap/girder_ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/girder_ldap/settings.py` & `girder-3.1.9.dev8/plugins/ldap/girder_ldap/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/plugin_tests/ldap_test.py` & `girder-3.1.9.dev8/plugins/ldap/plugin_tests/ldap_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/ldap/setup.py` & `girder-3.1.9.dev8/plugins/ldap/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/base.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/base.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/bitbucket.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/bitbucket.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/box.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/box.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/github.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/github.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/globus.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/globus.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/google.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/google.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/providers/linkedin.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/providers/linkedin.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/views/RegisterView.js` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/views/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/web_client/package.json` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/__init__.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/rest.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/girder_oauth/settings.py` & `girder-3.1.9.dev8/plugins/oauth/girder_oauth/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/plugin_tests/oauth_test.py` & `girder-3.1.9.dev8/plugins/oauth/plugin_tests/oauth_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/oauth/setup.py` & `girder-3.1.9.dev8/plugins/oauth/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js` & `girder-3.1.9.dev8/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/readme/girder_readme/rest.py` & `girder-3.1.9.dev8/plugins/readme/girder_readme/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/readme/plugin_tests/readmeSpec.js` & `girder-3.1.9.dev8/plugins/readme/plugin_tests/readmeSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/readme/setup.py` & `girder-3.1.9.dev8/plugins/readme/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/sentry/girder_sentry/web_client/package.json` & `girder-3.1.9.dev8/plugins/sentry/girder_sentry/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/sentry/girder_sentry/rest.py` & `girder-3.1.9.dev8/plugins/sentry/girder_sentry/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/sentry/girder_sentry/settings.py` & `girder-3.1.9.dev8/plugins/sentry/girder_sentry/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/sentry/setup.py` & `girder-3.1.9.dev8/plugins/sentry/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/models/CollectionModel.js` & `girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/models/CollectionModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js` & `girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js` & `girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js` & `girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/package.json` & `girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/web_client/routes.js` & `girder-3.1.9.dev8/plugins/terms/girder_terms/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/girder_terms/__init__.py` & `girder-3.1.9.dev8/plugins/terms/girder_terms/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/plugin_tests/termsSpec.js` & `girder-3.1.9.dev8/plugins/terms/plugin_tests/termsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/plugin_tests/terms_test.py` & `girder-3.1.9.dev8/plugins/terms/plugin_tests/terms_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/terms/setup.py` & `girder-3.1.9.dev8/plugins/terms/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/web_client/package.json` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/__init__.py` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/rest.py` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/rest.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/utils.py` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/utils.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/girder_thumbnails/worker.py` & `girder-3.1.9.dev8/plugins/thumbnails/girder_thumbnails/worker.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm` & `girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/thumbnail_test.py` & `girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/thumbnail_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/plugin_tests/thumbnailsSpec.js` & `girder-3.1.9.dev8/plugins/thumbnails/plugin_tests/thumbnailsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/thumbnails/setup.py` & `girder-3.1.9.dev8/plugins/thumbnails/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/views/extendView.js` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/views/extendView.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/web_client/package.json` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/__init__.py` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/quota.py` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/quota.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/girder_user_quota/settings.py` & `girder-3.1.9.dev8/plugins/user_quota/girder_user_quota/settings.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/plugin_tests/userQuotaSpec.js` & `girder-3.1.9.dev8/plugins/user_quota/plugin_tests/userQuotaSpec.js`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/plugin_tests/user_quota_test.py` & `girder-3.1.9.dev8/plugins/user_quota/plugin_tests/user_quota_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/user_quota/setup.py` & `girder-3.1.9.dev8/plugins/user_quota/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/virtual_folders/girder_virtual_folders/__init__.py` & `girder-3.1.9.dev8/plugins/virtual_folders/girder_virtual_folders/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/virtual_folders/plugin_tests/virtual_folders_test.py` & `girder-3.1.9.dev8/plugins/virtual_folders/plugin_tests/virtual_folders_test.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/plugins/virtual_folders/setup.py` & `girder-3.1.9.dev8/plugins/virtual_folders/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/pytest_girder/assertions.py` & `girder-3.1.9.dev8/pytest_girder/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/pytest_girder/fixtures.py` & `girder-3.1.9.dev8/pytest_girder/pytest_girder/fixtures.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/pytest_girder/plugin.py` & `girder-3.1.9.dev8/pytest_girder/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/pytest_girder/plugin_registry.py` & `girder-3.1.9.dev8/pytest_girder/pytest_girder/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/pytest_girder/utils.py` & `girder-3.1.9.dev8/pytest_girder/pytest_girder/utils.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/pytest_girder/web_client.py` & `girder-3.1.9.dev8/pytest_girder/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/LICENSE` & `girder-3.1.9.dev8/pytest_girder/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/pytest_girder/setup.py` & `girder-3.1.9.dev8/pytest_girder/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/midas/README.rst` & `girder-3.1.9.dev8/scripts/midas/README.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/midas/migrate.py` & `girder-3.1.9.dev8/scripts/midas/migrate.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/midas/walk_girder.py` & `girder-3.1.9.dev8/scripts/midas/walk_girder.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/midas/walk_midas.py` & `girder-3.1.9.dev8/scripts/midas/walk_midas.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/publicNames.py` & `girder-3.1.9.dev8/scripts/publicNames.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/publicNames.txt` & `girder-3.1.9.dev8/scripts/publicNames.txt`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/scripts/test_names.sh` & `girder-3.1.9.dev8/scripts/test_names.sh`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/.codecov.yml` & `girder-3.1.9.dev8/.codecov.yml`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/CHANGELOG.rst` & `girder-3.1.9.dev8/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/CMakeLists.txt` & `girder-3.1.9.dev8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/CONTRIBUTING.rst` & `girder-3.1.9.dev8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/Dockerfile` & `girder-3.1.9.dev8/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/LICENSE` & `girder-3.1.9.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/README.rst` & `girder-3.1.9.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/Vagrantfile` & `girder-3.1.9.dev8/Vagrantfile`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/package-lock.json` & `girder-3.1.9.dev8/package-lock.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/package.json` & `girder-3.1.9.dev8/package.json`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/requirements-dev.txt` & `girder-3.1.9.dev8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/setup.cfg` & `girder-3.1.9.dev8/setup.cfg`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/setup.py` & `girder-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/tox.ini` & `girder-3.1.9.dev8/tox.ini`

 * *Files identical despite different names*

### Comparing `girder-3.1.9.dev6/PKG-INFO` & `girder-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

