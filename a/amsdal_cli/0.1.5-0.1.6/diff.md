# Comparing `tmp/amsdal_cli-0.1.5.tar.gz` & `tmp/amsdal_cli-0.1.6.tar.gz`

## Comparing `amsdal_cli-0.1.5.tar` & `amsdal_cli-0.1.6.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/.editorconfig
--rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/Third-Party Materials - AMSDAL Dependencies - License Notices.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/app.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/__init__.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/callbacks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/build/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/build/command.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/build/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/build/utils/__init__.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/build/utils/build_app.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/build/utils/build_config_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/app.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/command.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/enums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/app.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/command.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/__init__.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_add.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_delete.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/app.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/command.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/enums.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_deploy.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_destroy.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_list.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_update.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/app.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/command.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/__init__.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_add.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_delete.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/app.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/app.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/command.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/__init__.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/add.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/delete.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/app.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/command.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/__init__.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/add.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/delete.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/retrieve.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/sub_commands/__init__.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/sub_commands/expose_db.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/sub_commands/get_monitoring_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/app.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/command.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/enums.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/__init__.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_frontend_config.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_hook.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_model.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_modifier.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_property.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_transaction.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/templates/hook.pyt
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/templates/property.pyt
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/templates/transaction.pyt
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/templates/modifier/constructor.pyt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/templates/modifier/display_name.pyt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/templates/modifier/version_name.pyt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/utils/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/utils/build_base_path.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/utils/cast_to_attribute_type.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/utils/model_attributes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/app.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/command.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/constants.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/__init__.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/apply.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/make.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/show.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/command.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/.amsdal-cli
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/.gitignore
--rw-r--r--   0        0        0    21707 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/config.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/restore/__init__.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/restore/command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/__init__.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/command.py
--rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/filters/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/filters/models_watch_filter.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/filters/static_files_watch_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/services/__init__.py
--rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/services/supervisor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/__init__.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/command.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/utils/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/utils/verify_json_model.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/utils/verify_python_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/config/__init__.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/config/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/utils/__init__.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/utils/check_versions.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/utils/cli_config.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/utils/copier.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/utils/markdown_patch.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/src/amsdal_cli/utils/render_template.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/.gitignore
--rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/README.md
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    56968 2020-02-02 00:00:00.000000 amsdal_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/.editorconfig
+-rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/Third-Party Materials - AMSDAL Dependencies - License Notices.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/app.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/callbacks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/build/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/build/command.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/build/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/build/utils/__init__.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/build/utils/build_app.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/build/utils/build_config_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/app.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/command.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/enums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/app.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/command.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/__init__.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_add.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_delete.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/app.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/command.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/enums.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_deploy.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_destroy.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_list.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_update.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/app.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/command.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/__init__.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_add.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_delete.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/app.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/app.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/command.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/__init__.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/add.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/app.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/command.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/__init__.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/add.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/delete.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/retrieve.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/sub_commands/__init__.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/sub_commands/expose_db.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/sub_commands/get_monitoring_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/app.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/command.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/enums.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/__init__.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_frontend_config.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_hook.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_model.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_modifier.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_property.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_transaction.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/templates/hook.pyt
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/templates/property.pyt
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/templates/transaction.pyt
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/templates/modifier/constructor.pyt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/templates/modifier/display_name.pyt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/templates/modifier/version_name.pyt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/utils/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/utils/build_base_path.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/utils/cast_to_attribute_type.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/utils/model_attributes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/app.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/command.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/constants.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/__init__.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/apply.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/make.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/show.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/command.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/.amsdal-cli
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/.gitignore
+-rw-r--r--   0        0        0    21707 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/config.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/restore/__init__.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/restore/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/__init__.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/command.py
+-rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/filters/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/filters/models_watch_filter.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/filters/static_files_watch_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/services/__init__.py
+-rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/services/supervisor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/__init__.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/command.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/utils/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/utils/verify_json_model.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/utils/verify_python_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/config/__init__.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/config/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/utils/check_versions.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/utils/cli_config.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/utils/copier.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/utils/markdown_patch.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/src/amsdal_cli/utils/render_template.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/.gitignore
+-rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/README.md
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    56968 2020-02-02 00:00:00.000000 amsdal_cli-0.1.6/PKG-INFO
```

### Comparing `amsdal_cli-0.1.5/.editorconfig` & `amsdal_cli-0.1.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/Third-Party Materials - AMSDAL Dependencies - License Notices.md` & `amsdal_cli-0.1.6/src/amsdal_cli/Third-Party Materials - AMSDAL Dependencies - License Notices.md`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/callbacks.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/callbacks.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/build/command.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/build/command.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/build/utils/build_app.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/build/utils/build_app.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/build/utils/build_config_file.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/build/utils/build_config_file.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_add.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_add.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_delete.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_delete.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_list.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/dependency/sub_commands/dependency_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_deploy.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_deploy.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_destroy.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_destroy.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_list.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_update.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/deploy/sub_commands/deploy_update.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_add.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_add.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_delete.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_delete.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_list.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/secret/sub_commands/secret_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/add.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/add.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/delete.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/allowlist/sub_commands/delete.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/add.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/add.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/delete.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/delete.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/retrieve.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/security/basic_auth/sub_commands/retrieve.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/sub_commands/expose_db.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/sub_commands/expose_db.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/cloud/sub_commands/get_monitoring_info.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/cloud/sub_commands/get_monitoring_info.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/enums.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/enums.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/__init__.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_frontend_config.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_frontend_config.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_hook.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_hook.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_model.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_model.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_modifier.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_modifier.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_property.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_property.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/sub_commands/generate_transaction.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/sub_commands/generate_transaction.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/utils/build_base_path.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/utils/build_base_path.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/generate/utils/model_attributes.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/generate/utils/model_attributes.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/apply.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     settings.override(APP_PATH=build_dir)
     config_manager = AmsdalConfigManager()
     config_manager.load_config(config or cli_config.config_path)
     amsdal_manager = AmsdalManager()
     amsdal_manager.setup()
     amsdal_manager.authenticate()
     amsdal_manager.post_setup()
+    amsdal_manager.init_class_versions()
 
     app_migrations_loader = MigrationsLoader(
         migrations_dir=build_dir / MIGRATIONS_DIR_NAME,
         module_type=ModuleTypes.APP,
     )
     schemas = MigrationSchemas()
     executor = FileMigrationExecutorManager(
```

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/make.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/make.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/migrations/sub_commands/show.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/migrations/sub_commands/show.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/new/command.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/new/command.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/README.md` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/README.md`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/new/templates/config.yml` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/new/templates/config.yml`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/restore/command.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/restore/command.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/command.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/command.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/utils.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/filters/static_files_watch_filter.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/filters/static_files_watch_filter.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/serve/services/supervisor.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/serve/services/supervisor.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/command.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/command.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/utils/verify_json_model.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/utils/verify_json_model.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/commands/verify/utils/verify_python_file.py` & `amsdal_cli-0.1.6/src/amsdal_cli/commands/verify/utils/verify_python_file.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/config/main.py` & `amsdal_cli-0.1.6/src/amsdal_cli/config/main.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/utils/check_versions.py` & `amsdal_cli-0.1.6/src/amsdal_cli/utils/check_versions.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/utils/cli_config.py` & `amsdal_cli-0.1.6/src/amsdal_cli/utils/cli_config.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/utils/copier.py` & `amsdal_cli-0.1.6/src/amsdal_cli/utils/copier.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/src/amsdal_cli/utils/markdown_patch.py` & `amsdal_cli-0.1.6/src/amsdal_cli/utils/markdown_patch.py`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/LICENSE.txt` & `amsdal_cli-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/README.md` & `amsdal_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/pyproject.toml` & `amsdal_cli-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amsdal_cli-0.1.5/PKG-INFO` & `amsdal_cli-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: amsdal_cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: CLI for AMSDAL framework
 Project-URL: Documentation, https://pypi.org/project/amsdal_cli/#readme
 Project-URL: Issues, https://pypi.org/project/amsdal_cli/
 Project-URL: Source, https://pypi.org/project/amsdal_cli/
 Author-email: "A. Michael Salem" <ams@amsdal.com>
 License: AMSDAL End User License Agreement
```

