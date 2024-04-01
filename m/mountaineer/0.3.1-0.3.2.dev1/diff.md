# Comparing `tmp/mountaineer-0.3.1.tar.gz` & `tmp/mountaineer-0.3.2.dev1.tar.gz`

## Comparing `mountaineer-0.3.1.tar` & `mountaineer-0.3.2.dev1.tar`

### file list

```diff
@@ -1,222 +1,253 @@
--rw-r--r--   0     1001      127      269 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1721 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src_go/build.rs
--rw-r--r--   0     1001      127     5657 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src_go/go.sum
--rw-r--r--   0     1001      127     5750 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src_go/src/lib.rs
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 mountaineer-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.git-blame-ignore-revs
--rw-r--r--   0     1001      127       95 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.gitattributes
--rw-r--r--   0     1001      127     2100 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     1476 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.github/scripts/update_version.py
--rw-r--r--   0     1001      127    15311 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3390 2024-03-27 00:00:49.000000 mountaineer-0.3.1/.gitignore
--rw-r--r--   0     1001      127     1750 2024-03-27 00:00:49.000000 mountaineer-0.3.1/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-03-27 00:00:49.000000 mountaineer-0.3.1/LICENSE
--rw-r--r--   0     1001      127     4233 2024-03-27 00:00:49.000000 mountaineer-0.3.1/Makefile
--rw-r--r--   0     1001      127    15808 2024-03-27 00:00:49.000000 mountaineer-0.3.1/README.md
--rw-r--r--   0     1001      127      105 2024-03-27 00:00:49.000000 mountaineer-0.3.1/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-03-27 00:00:49.000000 mountaineer-0.3.1/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-03-27 00:00:49.000000 mountaineer-0.3.1/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-03-27 00:00:49.000000 mountaineer-0.3.1/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   107805 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-03-27 00:00:49.000000 mountaineer-0.3.1/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127      212 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-03-27 00:00:49.000000 mountaineer-0.3.1/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127     8582 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/client_actions.md
--rw-r--r--   0     1001      127     1541 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/core_library.md
--rw-r--r--   0     1001      127     3021 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/database.md
--rw-r--r--   0     1001      127     7696 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/error_handling.md
--rw-r--r--   0     1001      127     2270 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   675789 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/media/header.png
--rw-r--r--   0     1001      127   148261 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2501 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/metadata.md
--rw-r--r--   0     1001      127      786 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/plugins.md
--rw-r--r--   0     1001      127     1383 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/postcss.md
--rw-r--r--   0     1001      127     4057 2024-03-27 00:00:49.000000 mountaineer-0.3.1/docs/view.md
--rw-r--r--   0     1001      127      954 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    12132 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     3474 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127     8065 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2799 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6569 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     8419 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     5130 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    10618 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18501 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/cache.py
--rw-r--r--   0     1001      127    17570 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/cli.py
--rw-r--r--   0     1001      127    10656 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     3958 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127     9737 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    28180 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127     9820 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     3317 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     1665 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/config.py
--rw-r--r--   0     1001      127       40 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/constants.py
--rw-r--r--   0     1001      127    13617 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1592 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/config.py
--rw-r--r--   0     1001      127      124 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     1992 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127      530 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     2678 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    15315 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     4514 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     1566 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/logging.py
--rw-r--r--   0     1001      127    12599 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/py.typed
--rw-r--r--   0     1001      127     5413 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/render.py
--rw-r--r--   0     1001      127     2488 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     5942 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8378 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/watch_server.py
--rw-r--r--   0     1001      127      866 2024-03-27 00:00:49.000000 mountaineer-0.3.1/mountaineer/webservice.py
--rw-r--r--   0     1001      127   123447 2024-03-27 00:00:49.000000 mountaineer-0.3.1/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/lexers.rs
--rw-r--r--   0     1001      127     8366 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-03-27 00:00:49.000000 mountaineer-0.3.1/src/timeout.rs
--rw-r--r--   0     1001      127    32088 2024-03-27 00:04:19.000000 mountaineer-0.3.1/Cargo.lock
--rw-r--r--   0     1001      127     1824 2024-03-27 00:00:49.000000 mountaineer-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    16266 1970-01-01 00:00:00.000000 mountaineer-0.3.1/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src_go/build.rs
+-rw-r--r--   0     1001      127     5657 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src_go/go.sum
+-rw-r--r--   0     1001      127     5750 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 mountaineer-0.3.2.dev1/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.gitattributes
+-rw-r--r--   0     1001      127     2100 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     1476 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    18084 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3404 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/LICENSE
+-rw-r--r--   0     1001      127     4432 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/Makefile
+-rw-r--r--   0     1001      127    14891 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/README.md
+-rw-r--r--   0     1001      127      105 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      775 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      559 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       59 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   107805 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      190 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      137 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3373 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127       61 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4667 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12265 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     4080 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      485 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/media/header.png
+-rw-r--r--   0     1001      127      954 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     7884 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9707 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9074 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    12132 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     3474 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127     8065 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     5001 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2799 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     8602 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5281 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6571 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     3239 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     8419 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2565 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12321 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6835 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    11635 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    18775 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/cache.py
+-rw-r--r--   0     1001      127    18059 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/cli.py
+-rw-r--r--   0     1001      127    10656 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     3958 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127     9737 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    28180 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127     9820 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     3317 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2153 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/config.py
+-rw-r--r--   0     1001      127       40 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/constants.py
+-rw-r--r--   0     1001      127    14854 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/controller.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    15315 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     1975 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/logging.py
+-rw-r--r--   0     1001      127    12599 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/render.py
+-rw-r--r--   0     1001      127     3228 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6299 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     5942 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8378 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/watch.py
+-rw-r--r--   0     1001      127     3087 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127      866 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   123447 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/lexers.rs
+-rw-r--r--   0     1001      127     8366 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-04-01 21:03:47.000000 mountaineer-0.3.2.dev1/Cargo.lock
+-rw-r--r--   0     1001      127     1824 2024-04-01 21:00:40.000000 mountaineer-0.3.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.3.2.dev1/PKG-INFO
```

### Comparing `mountaineer-0.3.1/src_go/build.rs` & `mountaineer-0.3.2.dev1/src_go/build.rs`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     // Log the GOARCH env variable, if specified
     if let Ok(goarch) = env::var("GOARCH") {
         eprintln!("GOARCH is set to {}", goarch);
     } else {
         eprintln!("GOARCH is not set");
     }
 
+    // Print the current working directory
+    eprintln!(
+        "Current working directory: {}",
+        env::current_dir().unwrap().display()
+    );
+
+    // Print the $PATH
+    eprintln!("PATH: {}", env::var("PATH").unwrap());
+
     // Step 1: Compile the Go code into a static library.
     let status = Command::new("go")
         .args([
             "build",
             "-buildmode=c-archive",
             "-o",
             out_path.join("libgo.a").to_str().unwrap(),
@@ -28,14 +37,16 @@
             "./go/js_build.go",
         ])
         .status()
         .expect("Failed to execute go build");
 
     assert!(status.success(), "Go build failed");
 
+    eprintln!("Successful golang build");
+
     // Step 2: Generate Rust bindings using bindgen.
     let bindings = bindgen::Builder::default()
         .header(out_path.join("libgo.h").to_str().unwrap())
         .parse_callbacks(Box::new(bindgen::CargoCallbacks::new()))
         .generate()
         .expect("Unable to generate bindings");
```

### Comparing `mountaineer-0.3.1/src_go/go/js_build.go` & `mountaineer-0.3.2.dev1/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src_go/src/lib.rs` & `mountaineer-0.3.2.dev1/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/Cargo.toml` & `mountaineer-0.3.2.dev1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "mountaineer"
 # Bumped automatically by CI on a release
-version = "0.3.1"
+version = "0.3.2-dev1"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 
 lazy_static = "1.4.0"
```

### Comparing `mountaineer-0.3.1/.github/scripts/check_dependencies.py` & `mountaineer-0.3.2.dev1/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/.github/scripts/update_version.py` & `mountaineer-0.3.2.dev1/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/.github/workflows/test.yml` & `mountaineer-0.3.2.dev1/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
 
   build:
-    name: build os=${{ matrix.os }} target=${{ matrix.target }} int=${{ matrix.interpreter || 'all' }} ml=${{ matrix.manylinux || 'auto' }}
+    name: build os=${{ matrix.os }} target=${{ matrix.target }} int=${{ matrix.interpreter || 'all' }} ml=${{ matrix.manylinux || 'auto' }} release=${{ matrix.release || 'latest' }}
     if: startsWith(github.ref, 'refs/tags/') || github.ref == 'refs/heads/main' || contains(github.event.pull_request.labels.*.name, 'Full Build')
     strategy:
       fail-fast: false
       matrix:
         include:
           # The main contraint with our architecture choices at the moment is the dependency
           # on rusty_v8, which only supports x86_64 and aarch64. Deno is tracking: https://github.com/denoland/deno/issues/7517
@@ -188,15 +188,15 @@
           - os: macos
             target: aarch64
 
           # windows
           - os: windows
             target: x86_64
 
-    runs-on: ${{ (matrix.os == 'linux' && 'ubuntu') || matrix.os }}-latest
+    runs-on: ${{ (matrix.os == 'linux' && 'ubuntu') || matrix.os }}-${{ matrix.release || 'latest' }}
     steps:
       - uses: actions/checkout@v4
 
       - name: set up python
         uses: actions/setup-python@v5
         with:
           python-version: "3.11"
@@ -243,21 +243,90 @@
           args: --out dist
 
       - name: build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           manylinux: ${{ matrix.manylinux || 'auto' }}
-          args: --release --out dist --interpreter ${{ matrix.interpreter || '3.11 3.12' }}
+          args: -vv --release --out dist --interpreter ${{ matrix.interpreter || '3.11 3.12' }}
           rust-toolchain: stable
-          docker-options: -e CI -e CI_TARGET=${{ matrix.target }} -e GOARCH=${{ matrix.target }} -e GOROOT=${{ env.GOROOT }} -v ${{ env.GOROOT }}:${{ env.GOROOT }}
-          command: build -vv
+          docker-options: -e CI -e CI_TARGET=${{ matrix.target }}
+          # Already defaults to build, but we make explicit here. Any arguments should
+          # be added to args above and not here - otherwise we will affect the switch()
+          # condition handling of maturin-action.
+          command: build
           before-script-linux: |
+            # Install go within the docker container - only used for manylinux builds
+            # since they need an isolated docker context. The other build pipelines
+            # just run within the host so use the global worker's go install.
+            # Determine the machine architecture
+            echo "Raw architecture: $(uname -m)"
+
+            # Log the current glibc version
+            ldd --version
+
+            # System configs
+            uname -a
+            cat /etc/os-release
+            cat /proc/version
+
+            # Determine distribution from /etc/os-release
+            DISTRO=$(grep ^ID= /etc/os-release | cut -d= -f2 | tr -d '"')
+
+            # Install necessary packages based on the distribution
+            if [ "$DISTRO" = "centos" ]; then
+                # CentOS specific package installation
+                yum -y install wget llvm-toolset-7 centos-release-scl
+                export PATH=/opt/rh/llvm-toolset-7/root/usr/bin:/opt/rh/llvm-toolset-7/root/usr/sbin:/opt/rh/devtoolset-10/root/usr/bin:$PATH
+                export LIBCLANG_PATH=/opt/rh/llvm-toolset-7/root/usr/lib64/
+            elif [ "$DISTRO" = "ubuntu" ]; then
+                # Ubuntu specific package installation
+                # Clang is already installed as part of the base image
+                apt-get update
+                apt-get -y install wget
+            else
+                echo "Unsupported distribution: $DISTRO"
+                exit 1
+            fi
+
+            clang --version
+
+            ls -ls /usr/bin
+
+            case "${{ matrix.target }}" in
+              x86_64) export GOARCH="amd64";;
+              aarch64)
+              export GOARCH="arm64";
+              export PATH=$PATH:/usr/aarch64-unknown-linux-gnu/bin;
+              aarch64-unknown-linux-gnu-gcc --version;
+              export CC=aarch64-unknown-linux-gnu-gcc;;
+              *) echo "Unsupported architecture: ${{ matrix.target }}"; exit 1;;
+            esac
+            echo "GOARCH=${GOARCH}"
+
+            GOVERSION="1.22.1"
+
+            # Must be explicitly specified for cross-compilation
+            # Otherwise it causes the misleading "go: no Go source files" error
+            export CGO_ENABLED=1
+
+            # Download and Install Go - we will always be running on a x86_64 runner
+            # despite the build architecture
+            wget -q https://go.dev/dl/go${GOVERSION}.linux-amd64.tar.gz
+            tar -C /usr/local -xzf go${GOVERSION}.linux-amd64.tar.gz
+            rm -f go${GOVERSION}.linux-amd64.tar.gz
+
+            # Set up Go environment variables
+            export GOROOT=/usr/local/go
             export PATH=$PATH:$GOROOT/bin
+
+            go env
+
             go version
+            go tool dist list
         env:
           GOROOT: ${{ env.GOROOT }}
           GOPATH: ${{ env.GOPATH }}
           GOMODCACHE: ${{ env.GOMODCACHE }}
 
       - run: ${{ (matrix.os == 'windows' && 'dir') || 'ls -lh' }} dist/
 
@@ -429,17 +498,14 @@
           echo "GOROOT=$(go env GOROOT)" >> $GITHUB_ENV
           echo "GOPATH=$(go env GOPATH)" >> $GITHUB_ENV
           echo "GOMODCACHE=$(go env GOMODCACHE)" >> $GITHUB_ENV
 
       - name: Install Poetry
         run: |
           curl -sSL https://install.python-poetry.org | python3 -
-
-      - name: Configure Poetry
-        run: |
           echo "$HOME/.local/bin" >> $GITHUB_PATH
 
       - name: Install dependencies
         run: make install-deps-create-mountaineer-app
 
       - name: Run tests
         run: make test-create-mountaineer-app
@@ -479,17 +545,14 @@
         with:
           python-version: "3.11"
           architecture: ${{ matrix.python-architecture || 'x64' }}
 
       - name: Install Poetry
         run: |
           curl -sSL https://install.python-poetry.org | python3 -
-
-      - name: Configure Poetry
-        run: |
           echo "$HOME/.local/bin" >> $GITHUB_PATH
 
       - name: Update version in pyproject.toml
         if: startsWith(github.ref, 'refs/tags/v')
         run: |
           cd create_mountaineer_app
           VERSION=${GITHUB_REF#refs/tags/v}
```

### Comparing `mountaineer-0.3.1/.gitignore` & `mountaineer-0.3.2.dev1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -175,7 +175,9 @@
 _static
 
 # Ignore template files that might be used locally for testing
 # but shouldn't be added to the downstream templates
 **/create_mountaineer_app/templates/poetry.lock
 
 .DS_Store
+
+website/site
```

### Comparing `mountaineer-0.3.1/Dockerfile` & `mountaineer-0.3.2.dev1/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/LICENSE` & `mountaineer-0.3.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/Makefile` & `mountaineer-0.3.2.dev1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 CREATE_MOUNTAINEER_APP_DIR := create_mountaineer_app
 CREATE_MOUNTAINEER_APP_NAME := create_mountaineer_app
 
 CI_WEBAPP_DIR := ci_webapp
 CI_WEBAPP_NAME := ci_webapp
 
+DOCS_WEBSITE := docs_website
+DOCS_WEBSITE_NAME := docs_website
+
 # Ignore these directories in the local filesystem if they exist
 .PHONY: lint test
 
 # Main lint target
 lint: lint-lib lint-create-mountaineer-app lint-ci-webapp
 
 # Lint validation target
@@ -44,14 +47,18 @@
 	@echo "Installing dependencies for $(CREATE_MOUNTAINEER_APP_DIR)..."
 	@(cd $(CREATE_MOUNTAINEER_APP_DIR) && poetry install)
 
 install-deps-ci-webapp:
 	@echo "Installing dependencies for $(CI_WEBAPP_DIR)..."
 	@(cd $(CI_WEBAPP_DIR) && poetry install)
 
+install-deps-docs-website:
+	@echo "Installing dependencies for $(DOCS_WEBSITE)..."
+	@(cd $(DOCS_WEBSITE) && poetry install --no-root)
+
 # Clean the current poetry.lock files, useful for remote CI machines
 # where we're running on a different base architecture than when
 # developing locally
 clean-poetry-lock:
 	@echo "Cleaning poetry.lock files..."
 	@rm -f $(LIB_DIR)/poetry.lock
 	@rm -f $(CREATE_MOUNTAINEER_APP_DIR)/poetry.lock
```

### Comparing `mountaineer-0.3.1/README.md` & `mountaineer-0.3.2.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Mountaineer Header](https://raw.githubusercontent.com/piercefreeman/mountaineer/main/docs/media/header.png)
+![Mountaineer Header](https://raw.githubusercontent.com/piercefreeman/mountaineer/main/media/header.png)
 
 <p align="center"><i>Move fast. Climb mountains. Don't break things.</i></p>
 
 Mountaineer 🏔️ is a framework to easily build webapps in Python and React. If you've used either of these languages before for development, we think you'll be right at home.
 
 ## Main Features
 
@@ -257,22 +257,22 @@
 export default Home;
 ```
 
 We define a simple view to show the data coming from the backend. To accomplish this conventionally, we'd need to wire up an API layer, a Node server, or format the page with Jinja templates.
 
 Here instead we use our automatically generated `useServer()` hook. This hook payload will provide all the `HomeRender` fields as properties of serverState. And it's available instantly on page load without any roundtrip fetches. Also - if your IDE supports language servers (which most do these days), you should see the fields auto-suggesting for `serverState` as you type.
 
-<p align="center"><img src="./docs/media/ide_typehints.png" alt="IDE Typehints" width="500px" /></p>
+<p align="center"><img src="./docs_website/docs/media/ide_typehints.png" alt="IDE Typehints" width="500px" /></p>
 
 If you access this in your browser at `localhost:5006/` we can see our welcome message, but we can't really _do_ anything with the todos yet. Let's add some interactivity.
 
 > [!TIP]
 > Try disabling Javascript in your browser. The page will still render as-is with all variables intact, thanks to our server-side rendering.
 
-<p align="center"><img src="./docs/media/server_side_rendering.png" alt="Server-side rendering" height="400px" /></p>
+<p align="center"><img src="./docs_website/docs/media/server_side_rendering.png" alt="Server-side rendering" height="400px" /></p>
 
 What good is todo list that doesn't get longer? We define a `add_todo` function that accepts a pydantic model `NewTodoRequest`, which defines the required parameters for a new todo item. We then cast this to a database object and add it to the postgres table.
 
 ```python
 # my_webapp/controllers/home.py
 
 from pydantic import BaseModel
@@ -341,27 +341,18 @@
 export default Home;
 ```
 
 `useServer()` exposes our `add_todo` function so we can call our backend directly from our frontend. Also notice that we don't have to read or parse the output value of this function to render the new todo item to the list. Since the function is marked as a sideeffect, the frontend will automatically refresh its data after the function is called.
 
 Go ahead and load it in your browser. If you open up your web tools, you can create a new Todo and see POST requests sending data to the backend and receiving the current server state. The actual data updates and merging happens internally by Mountaineer.
 
-<p align="center"><img src="./docs/media/final_todo_list.png" alt="Getting Started Final TODO App" height="400px" /></p>
+<p align="center"><img src="./docs_website/docs/media/final_todo_list.png" alt="Getting Started Final TODO App" height="400px" /></p>
 
-<p align="center"><img src="./docs/media/network_debug.png" alt="Getting Started Final TODO App" height="400px" /></p>
+<p align="center"><img src="./docs_website/docs/media/network_debug.png" alt="Getting Started Final TODO App" height="400px" /></p>
 
 You can use these serverState variables anywhere you'd use dynamic React state variables (useEffect, useCallback, etc). But unlike React state, these variables are automatically updated when a relevant sideeffect is triggered.
 
 And that's it. We've just built a fully interactive web application without having to worry about an explicit API. You specify the data model and actions on the server and the appropriate frontend hooks are generated and updated automatically. It gives you the power of server rendered html and the interactivity of a virtual DOM, without having to compromise on complicated data mutations to keep everything in sync.
 
 ### Learn More
 
-We have additional documentation that does more of a technical deep dive on different features of Mountaineer. We order these roughly in the order that we anticipate you'll need them.
-
-- [Client Actions](./docs/client_actions.md): Details on @sideeffect, @passthrough, and masking @sideeffect fields for partial re-rendering.
-- [View Definition](./docs/view.md): How to define the view and use the serverState hook. Covers `page.tsx` and `layout.tsx` conventions to easily nest your site designs.
-- [Page Metadata](./docs/metadata.md): How to set the title, description, and other metadata for your pages.
-- [Link Generation](./docs/links.md): Generate links to other pages within your webapp, with typehinting and automatic URL generation.
-- [Error Handling](./docs/error_handling.md): Conventions for handling client-side errors while fetching data in your webapp.
-- [PostCSS](./docs/postcss.md): PostCSS build plugin for TailwindCSS support and other CSS processing.
-- [Database](./docs/database.md): Database conventions.
-- [Core Library](./docs/core_library.md): Details on how to do local development on the core library.
+We have additional documentation that does more of a technical deep dive on different features of Mountaineer. Check out [mountaineer.sh](https://mountaineer.sh/).
```

### Comparing `mountaineer-0.3.1/benchmarking/poetry.lock` & `mountaineer-0.3.2.dev1/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/README.md` & `mountaineer-0.3.2.dev1/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/app.py` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.3.2.dev1/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/poetry.lock` & `mountaineer-0.3.2.dev1/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/ci_webapp/pyproject.toml` & `mountaineer-0.3.2.dev1/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/README.md` & `mountaineer-0.3.2.dev1/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.3.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/poetry.lock` & `mountaineer-0.3.2.dev1/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/create_mountaineer_app/pyproject.toml` & `mountaineer-0.3.2.dev1/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/client_actions.md` & `mountaineer-0.3.2.dev1/docs_website/docs/client_actions.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 ## Action Types
 
 Anytime clients need to modify the server state, we denote these requests as "actions". Internally, they're just POST requests that are sent to the server. There's no black magic to this syntax. You can inspect them all in your browser's console as regular JSON.
 
 Your choice of action type depends on how you want to update _client_ data after your _server_ action has been executed.
 
-**@sideeffect:** Update the server data that initialized the client view. Sideeffects are also passthroughs, by definition, so they can pass back arbitrary data that is outside of the scope of the render() data payload.
+**@sideeffect:** Update the server data that initialized the client view. Sideeffects are also passthroughs, by definition, so they can pass back arbitrary data that is outside of the scope of the render() data payload. Use a sideeffect whenever the client modifies some data that lives on the server.
 
-**@passthrough:** Expose an action to the client caller but don't update the server data once the action has been completed.
+**@passthrough:** Expose an action to the client caller but don't update the server data once the action has been completed. Use a passthrough whenever you need to fetch additional data from the server, or the mutation on the server doesn't affect the local frontend state.
 
 ## Side Effect
 
 Side-effects work as if you have reloaded the page. They update the server state and then push the updated state back to the client. They will call a fully fresh `render()` on the server so you can provide the latest data state to the client. However, unlike a true refresh on the client side, there's no actual browser refresh that is performed. This allows you to receive the updated data definition and keep the rest of your variables saved in local state.
 
 `@sideeffect` can either be called with default behavior or customized via decorator arguments:
 
@@ -57,18 +57,19 @@
 });
 ```
 
 You can also manually inspect the sideeffect payload by accessing `response.sideeffect`.
 
 If the action has a passthrough, it will be supplied in `response.passthrough`. Otherwise it will be undefined.
 
-### Experimental Render Cropper
+### Experimental Render Reloader
 
-> [!TIP]
-> This feature is experimental and only supports relatively simple render() function implementations. If you use it for a more complicated render() function and it doesn't work as expected, report a bug to improve the test coverage.
+!!! tip
+
+    This feature is experimental and only supports relatively simple render() function implementations. If you use it for a more complicated render() function and it doesn't work as expected, report a bug to improve the test coverage.
 
 Render functions sometimes have heavy logic overhead: they need to fetch multiple objects from the database, do some roll-up computation, etc. If you're issuing a sideeffect that only affects a small portion of the initial data, this is wasted computation.
 
 Passing a `reload` filter to `sideeffect` prevents this redundant data from being sent to the frontend. But this feature only saves bandwidth; it doesn't actually prevent the server from doing the computation in the first place. This is where the `experimental_render_reload` comes in.
 
 When this flag is set to `True`, Mountaineer will inspect the AST ([Abstract Syntax Tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree)) of your render function. It creates a new synthetic render function that only does the computation required to calculate the `reload` parameters. If some intensive compute isn't required for your sideeffect, it will be ignored.
 
@@ -101,15 +102,15 @@
 ```json
 {
   "value_a": "Hello 1229",
   "value_b": "Hello 78498"
 }
 ```
 
-When `call_sideeffect` is called with `experimental_render_reload=True`, the compute is `0.010s`. It results in:
+When `call_sideeffect` is called with `experimental_render_reload=True`, the compute only takes `0.010s`. It results in:
 
 ```json
 {
   "value_a": "Hello 1229"
 }
 ```
 
@@ -158,19 +159,19 @@
     @passthrough
     async def stream_metadata(self) -> AsyncIterator[MyMetadata]:
         yield MyMetadata(state=1)
         await asyncio.sleep(10)
         yield MyMetadata(state=2)
 ```
 
-For the time being we only support server-events in `@passthrough` functions, not `@sideeffect`. It's ill-defined whether we should re-render() content every yield or when the iterator has finished.
+For the time being we only support server-events in `@passthrough` functions, not `@sideeffect`. It's ill-defined whether we should re-render() content every yield or when the iterator has finished. Yielding in passthrough makes it clear that you just want to stream the yielded value to the client.
 
 In your frontend, you can iterate over these responses with an async generator loop. Each response object will be parsed into your typed schema for you, so you can see typehints like you would for any regular Mountaineer action.
 
-```tsx
+```typescript
 import React, { useState, useEffect } from "react";
 
 const Page = () => {
   const [currentState, setCurrentState] = useState(-1);
 
   useEffect(() => {
       const runStream = async () => {
@@ -192,28 +193,37 @@
 
 When defining your action functions themselves in your controller, we support typehinting via:
 
 - Query parameters
 - Pydantic models for JSON payloads
 - Dependency injection via `fastapi.Depends`
 
-We also support both sync and async functions. A common sideeffect pattern might look like this:
+We also support both sync and async functions. Sync functions will be spawned into a thread pool by default - which processes them in parallel but can tax system resources with GIL locking. Where possible, use async functions with libraries that support await constructs.
+
+A common sideeffect pattern might look like this:
 
 ```python
-from fastapi import Depends
+from mountaineer import ControllerBase, Depends
 from my_website.models import User
+from my_website.deps import get_current_user
 
 class IncrementCountRequest:
     count: int
 
-@sideeffect
-async def increment_count(
-    self,
-    payload: IncrementCountRequest,
-    query_param: int,
-    user: User = Depends(get_current_user)
-) -> None:
-    self.global_count += payload.count
+class MyController(ControllerBase):
+    def __init__(self):
+        super().__init__()
+        self.global_count = 0
+
+    @sideeffect
+    async def increment_count(
+        self,
+        payload: IncrementCountRequest,
+        query_param: int,
+        user: User = Depends(get_current_user)
+    ) -> None:
+        self.global_count += payload.count
 ```
 
-> [!CAUTION]
-> Actions are publicly exposed to the Internet by default. It's up to you to secure them with authentication if they should only be accessible by a certain portion of your userbase.
+!!! warning
+
+    Actions are publicly exposed to the Internet by default. It's up to you to secure them with authentication if they should only be accessible by a certain portion of your userbase.
```

### Comparing `mountaineer-0.3.1/docs/core_library.md` & `mountaineer-0.3.2.dev1/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/database.md` & `mountaineer-0.3.2.dev1/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/error_handling.md` & `mountaineer-0.3.2.dev1/docs_website/docs/error_handling.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Error handling
+# Error Handling
 
 Errors are a fundamental part of computer science, but nowhere is that more evident than when building websites. There are so many factors you don't have control over: client latency, malformed payloads, spiky server load, resource contention for the same user. The list goes on. Any one can bring a user experience to its knees.
 
-All that to say - it's not a question of _if_ you'll see errors but _when_. mountaineer provides some handy utilities that make it a bit easier to handle the errors you may encounter in production.
+All that to say - it's not a question of _if_ you'll see errors but _when_. Mountaineer provides some handy utilities that make it a bit easier to handle the errors you may encounter in production.
 
 ## Client->Server exceptions
 
 When client actions call server actions (either sideeffects or passthroughs), their browser needs to make an outgoing fetch request to your server. Your server can throw an error in response to this payload for any reason: validation failures, unexpected state, or just because some internal logic failed.
 
 When your server returns an error, your async action will raise the relevant error. Let's say you have the following component that issues an invalid call to a server action:
 
@@ -55,30 +55,31 @@
     }
   }}
 >
   Invalid Increment
 </button>
 ```
 
-mountaineer will convert the error into a custom error class and expose it in `_server/actions` for you to import. This class helps you switch logic depending on the type of error that was raised. Using a class here also has the benefit of typeguarding your error handling, so you'll see IDE recommendations specific to that ValidationError.
+Mountaineer will convert the error into a custom error class and expose it in `_server/actions` for you to import. This class helps you switch logic depending on the type of error that was raised. Using a class here also has the benefit of typeguarding your error handling, so you'll see IDE recommendations specific to that ValidationError.
 
 You can find the error payload itself within `error.body`, which will be typehinted with all the metadata (if any) that the server is expected to return as part of this error code. In the above example, that looks like this:
 
 ```
 Validation Error (2) ['body', 'count'] Input should be a valid integer, unable to parse string as an integer
 ```
 
 Internally, we generate `HTTPValidationErrorException` as a subclass of FetchErrorBase. This provided the common error handling, while typehinting it for your specific API errors.
 
 ```typescript title="_server/actions.ts"
 class HTTPValidationErrorException extends FetchErrorBase<HTTPValidationError> {}
 ```
 
-> [!TIP]
-> For more information on error typehinting and custom handling, see the FastAPI [documentation](https://fastapi.tiangolo.com/tutorial/handling-errors/).
+!!! tip
+
+    For more information on error typehinting and custom handling, see the FastAPI [documentation](https://fastapi.tiangolo.com/tutorial/handling-errors/).
 
 ## Custom Errors
 
 A 422 ValidationError is a special error that is included in every action, because your function signature is verified every time a client sends a new payload to your server. To implement a custom error that is specific to your application, you can subclass `APIException`:
 
 ```python
 from mountaineer.exceptions import APIException
@@ -93,15 +94,15 @@
     @passthrough(exception_models=[LoginInvalid])
     def login(self, login_payload: LoginRequest):
         raise LoginInvalid(invalid_reason="Login not implemented")
 ```
 
 Provide all the exceptions that your function may throw to `@passthrough(exception_models=[])`. The `@sideeffect` decorator accepts the same argument.
 
-When specified like this, mountaineer turns your exception into a client-side exception just like `HTTPValidationErrorException`. You can now use it in the same way.
+When specified like this, Mountaineer turns your exception into a client-side exception just like `HTTPValidationErrorException`. You can now use it in the same way.
 
 ## SSR timeouts
 
 To render each page on the server side, we have to execute your view's Javascript in a V8 engine. This is the same Javascript interpreter that powers Chrome. As such, you have the full freedom to write any Javascript in your view that will help you render your page - loops, calculations, package calls, etc.
 
 As is the case with Turing-complete languages, with great power comes great responsibility.
```

### Comparing `mountaineer-0.3.1/docs/links.md` & `mountaineer-0.3.2.dev1/docs_website/docs/links.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # Links
 
-> "What is a webapp without links?"</br>
-> "Probably a lineapp or something."</br>
-> &mdash; William Shakespeare
-
 In a typical webapp, you'll have a lot of links. Most will be internal to your site: detail pages, settings, profiles, etc. Traditionally, developers format these links manually and hope they don't break over time as routes update.
 
-In mountaineer, generating links is baked into the client side routes. For every controller you define, we'll generate a link interface that defines the parameters that controller accepts. This interface will update as your route declarations do, so you're guaranteed to always generate the latest links to successfully resolve that controller.
+In Mountaineer, generating links is baked into the client side routes. For every controller you define, we'll generate a link interface that defines the parameters that controller accepts. This interface will update as your route declarations do, so you're guaranteed to always generate the latest links to successfully resolve that controller.
 
 Controllers set the parameters that they need to render their views by configuring the `render()` function with the required parameters:
 
 ```python
 class DetailController:
     url = "/detail/{detail_id}"
 
     def render(self, detail_id: int, checking_out: bool = False) -> MyDetailData:
         ...
 ```
 
-Alongside generating the appropriate API and router files, mountaineer will detect this render signature and produce a link generator.
+Alongside generating the appropriate API and router files, Mountaineer will detect this render signature and produce a link generator.
 
 This particular generator will require a `detail_id` and support an optional `checking_out` boolean. The `detail_id` is required because it's a part of the controller url. `checking_out` on the other hand is optional, since it has a default keyword argument in the case that another value isn't provided.
 
 On the client side, you can now create these dynamic links anywhere within your application. Mount the server state of the current view and use the included `linkGenerator`.
 
 ```typescript
 const MyHomeRoute = () => {
```

### Comparing `mountaineer-0.3.1/docs/media/final_todo_list.png` & `mountaineer-0.3.2.dev1/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/media/header.png` & `mountaineer-0.3.2.dev1/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/media/ide_typehints.png` & `mountaineer-0.3.2.dev1/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/media/network_debug.png` & `mountaineer-0.3.2.dev1/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/media/server_side_rendering.png` & `mountaineer-0.3.2.dev1/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/docs/metadata.md` & `mountaineer-0.3.2.dev1/docs_website/docs/metadata.md`

 * *Files 27% similar despite different names*

```diff
@@ -44,34 +44,15 @@
                 "og:meta",
                 content="Some meta content",
             )
         )
     )
 ```
 
-We have a limited number of helper <meta> constructors, particularly in cases where there are standard definitions of complex meta values:
-
-**ThemeColorMeta:** Customizes the default color that is attached to the page.
-
-```python
-ThemeColorMeta(
-    color="white",
-    media="light",
-)
-```
-
-**ViewportMeta:** Defines the bounds on the current page and how much users are able to zoom.
-
-```python
-ViewportMeta(
-    initial_scale=1.0,
-    maximum_scale=2.0,
-    user_scalable=True,
-)
-```
+We have a limited number of helper <meta> constructors, particularly in cases where there are standard definitions of complex meta values. For more details on the supported Metadata and rendering options, check out the [API Docs](./api/render.md).
 
 ## Global Metadata
 
 For metadata that you know should appear on every page (like stylesheets or global scripts), you can add a metadata tag to your app controller:
 
 ```python
 controller = AppController(
```

### Comparing `mountaineer-0.3.1/docs/postcss.md` & `mountaineer-0.3.2.dev1/docs_website/docs/postcss.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,20 @@
-# postcss
+# PostCSS & Tailwind
+
+## PostCSS
 
 [PostCSS](https://postcss.org/) is a compiler for CSS. It enables buildtime transformation of CSS files to convert SCSS, LESS, or other CSS-like languages into standard CSS. It also has utilities for polyfills and browser-specific prefixes. I think of it like a swiss-army knife for CSS: it helps assure that your styling intentions are actually rendered uniformily across browsers.
 
-PostCSS support is handled as a buildtime plugin with mountaineer. It's disabled by default. To enable, make sure you have `postcss-cli` installed within your `views/project.json` file. You'll also need to properly `npm install` the dependencies before running.
+PostCSS support is handled as a buildtime plugin with Mountaineer. It's disabled by default. To enable, make sure you have `postcss-cli` installed within your `views` project:
+
+```bash
+npm install postcss-cli
+```
+
+After this you can leverage the `PostCSSBundler` within your custom build pipeline:
 
 ```python
 from mountaineer.js_compiler.postcss import PostCSSBundler
 
 controller = AppController(
     custom_builders=[
         PostCSSBundler(),
@@ -25,7 +33,41 @@
 
 ```
 /views/_static/home_style.css
 /views/_static/detail_style.css
 ```
 
 You can then import this CSS file in whatever <meta> tag is relevant to your project. See the [metadata documentation](./metadata.md) for more details on how to do this.
+
+## Tailwind
+
+Tailwind uses PostCSS to handle the tree shaking and project analysis that allows it to output the minimal amount of CSS tags to correctly render your project. If you set up the PostCSS extension like described above, you should be able to follow the typical Tailwind [setup](https://tailwindcss.com/docs/installation) steps.
+
+```typescript title="views/app/tailwind.config.ts"
+module.exports = {
+  content: ["./app/**/*.{html,tsx,jsx,ts,js}"],
+  theme: {
+    extend: {},
+  },
+  plugins: [],
+}
+```
+
+```css title="views/app/main.css"
+@tailwind base;
+@tailwind components;
+@tailwind utilities;
+```
+
+Then export the built styles into your global metadata:
+
+```python
+controller = AppController(
+    config=AppConfig(),
+    global_metadata=Metadata(
+        links=[LinkAttribute(rel="stylesheet", href="/static/app_main.css")]
+    ),
+    custom_builders=[
+        PostCSSBundler(),
+    ],
+)
+```
```

### Comparing `mountaineer-0.3.1/docs/view.md` & `mountaineer-0.3.2.dev1/docs_website/docs/views.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Views
+# Frontend Views
 
-Your React app should be initialized in the `/views` folder of your mountaineer project. This is the directory where we look for package.json and tsconfig.json, and where esbuild looks for specific build-time overrides. In other words, the views folder should look just like your frontend application if you were building a Single-Page-App (SPA). It's just embedded within your larger mountaineer project.
+Your React app should be initialized in the `/views` folder of your Mountaineer project. This is the directory where we look for package.json and tsconfig.json, and where esbuild looks for specific build-time overrides. In other words, the views folder should look just like your frontend application if you were building a Single-Page-App (SPA). It's just embedded within your larger Mountaineer project and rendered separately.
 
 We expect that all controller views will be labeled as a `page.tsx`, so they'll typically sit in a folder with themselves and other tightly connected React components. These views should have one default export, which is your page constructor:
 
 ```typescript title="/views/app/home/page.tsx"
 import React from "react";
 
 const Home = () => {
@@ -84,15 +84,15 @@
     /layout.tsx
 ```
 
 When rendering `dashboard/home/page.tsx`, the view will be wrapped in the `app/dashboard/layout.tsx` layout alongside `app/layout.tsx`. These layouts should only provide styling. Since the use of `useServer` would be ambiguous for layouts that are rendered by multiple components, they should not contain any logic or data fetching.
 
 ## Typescript Configuration
 
-If you want to customize how mountaineer builds your view files into raw client-side javascript, add a `tsconfig.json` file. The Typescript website includes a [full list](https://www.typescriptlang.org/tsconfig) of the available options here. A good place to start is:
+If you want to customize how Mountaineer builds your view files into raw client-side javascript, add a `tsconfig.json` file. The Typescript website includes a [full list](https://www.typescriptlang.org/tsconfig) of the available options here. A good place to start is:
 
 ```json
 {
   "compilerOptions": {
     "target": "es2017",
     "lib": ["dom", "dom.iterable", "esnext"],
     "allowJs": true,
@@ -108,15 +108,15 @@
     "jsx": "preserve",
     "incremental": true,
   },
   "exclude": ["node_modules"]
 }
 ```
 
-A common extension is wanting to import all your view paths with absolute paths (like `@/components/myfile`) instead of having to do relative imports (`../../../components/myfile`). This can be easily achieved by adding a `paths` key to your `tsconfig.json`. Your import becomes relative to all paths in the root directory.
+A common convention is importing all your view paths with absolute paths (like `@/components/myfile`) instead of having to do relative imports (`../../components/myfile`). This can be easily achieved by adding a `paths` key to your `tsconfig.json`. Your import becomes relative to all paths in the root directory.
 
 ```json
 {
   "compilerOptions": {
     "target": "es2017",
     ...
     "paths": {
```

### Comparing `mountaineer-0.3.1/mountaineer/__init__.py` & `mountaineer-0.3.2.dev1/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_app.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_cache.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_cli.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_controller.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 '<script src="/script4.js" test-attr="test-value"></script>',
             ],
         ),
     ],
 )
 def test_build_header(metadata: Metadata, expected_tags: list[str]):
     controller = StubController()
-    assert controller.build_header(metadata) == expected_tags
+    assert controller._build_header(metadata) == expected_tags
 
 
 COMPLEX_METADATA = Metadata(
     title="MyTitle",
     links=[
         LinkAttribute(
             rel="stylesheet",
@@ -185,15 +185,15 @@
             ],
             Metadata(title="Primary"),
         ),
     ],
 )
 def test_merge_metadatas(metadatas: list[Metadata], expected_metadata: Metadata):
     controller = StubController()
-    assert controller.merge_metadatas(metadatas) == expected_metadata
+    assert controller._merge_metadatas(metadatas) == expected_metadata
 
 
 def test_resolve_paths(tmp_path: Path):
     view_base = tmp_path / "views"
     ssr_base = view_base / "_ssr"
     static_base = view_base / "_static"
```

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_paths.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/__tests__/test_watch.py` & `mountaineer-0.3.2.dev1/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/actions/fields.py` & `mountaineer-0.3.2.dev1/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/actions/passthrough.py` & `mountaineer-0.3.2.dev1/mountaineer/actions/passthrough.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
     Coroutine,
+    Literal,
     ParamSpec,
     Type,
     TypeVar,
     overload,
 )
 
 from fastapi.responses import JSONResponse, Response, StreamingResponse
@@ -40,24 +41,24 @@
 
 RawResponseR = TypeVar("RawResponseR", bound=Response)
 
 
 @overload
 def passthrough(  # type: ignore
     *,
-    response_model: Type[BaseModel] | None = None,
+    response_model: Type[BaseModel] | None = None,  # Deprecated
     exception_models: list[Type[APIException]] | None = None,
 ) -> Callable[[Callable[P, R | Coroutine[Any, Any, R]]], Callable[P, Awaitable[R]]]:
     ...
 
 
 @overload
 def passthrough(
     *,
-    raw_response: bool = True,
+    raw_response: Literal[True] = True,
 ) -> Callable[
     [Callable[P, RawResponseR | Coroutine[Any, Any, RawResponseR]]],
     Callable[P, Awaitable[RawResponseR]],
 ]:
     ...
 
 
@@ -66,19 +67,57 @@
     func: Callable[P, R | Coroutine[Any, Any, R]],
 ) -> Callable[P, Awaitable[R]]:
     ...
 
 
 def passthrough(*args, **kwargs):  # type: ignore
     """
-    By default, we mask out function return values to avoid leaking any unintended data to client applications. This
-    decorator marks a function .
-
-    :response_model: Like in FastAPI, the response model to use for this endpoint. If not provided, will
-        try to convert the response object into the proper JSON response as-is.
+    Only functions that are explicitly marked as actions will be accessable by the frontend. The
+    @passthrough decorator indicates that this function should be called by the frontend and will
+    return an explicit data payload. It will NOT update the render() state of the frontend.
+
+    Decorate functions within your ControllerBase that you want to expose. Each of these functions should specify
+    a return type. Normal passthrough endpoints can return with either a `None`, a `BaseModel` object, or a
+    `JSONResponse` if you need full flexibility on return headers and content structure.
+
+    If you do return a JSONResponse note that we will handle the merging of the response for you - so
+    on the client side you will still access your endpoint contents with:
+
+    ```typescript
+    const response = await serverState.my_action({});
+    console.log(response.passthrough);
+    ```
+
+    Usage:
+
+    ```python
+    from pydantic import BaseModel
+
+    class ResponseModel(BaseModel):
+        pass
+
+    class MyController(ControllerBase):
+        @passthrough
+        async def my_action(self) -> ResponseModel:
+            ...
+    ```
+
+    :param exception_models: List of APIException subclasses that this function is known
+        to throw. These will be parsed and available to frontend clients.
+    :type exception_models: list[Type[APIException]] | None
+
+    :param raw_response: If specified, you can return a generic fastapi.Response object. There's
+        no constraint this endpoint returns JSON - you can return html or a custom protocol. This
+        lets you treat this API as a generic POST endpoint for you to fully control the output.
+    :type raw_response: bool
+
+    :return: The response model to use for this endpoint. If a BaseModel is not provided (you pass
+        a dictionary or a SQLModel object ofr instance), we will try to convert the response object
+        into the proper JSON response based on your typehint.
+    :rtype: BaseModel | None | fastapi.JSONResponse
 
     """
 
     def decorator_with_args(
         response_model: Type[BaseModel] | None,
         exception_models: list[Type[APIException]] | None,
         raw_response: bool | None,
```

### Comparing `mountaineer-0.3.1/mountaineer/actions/sideeffect.py` & `mountaineer-0.3.2.dev1/mountaineer/actions/sideeffect.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 R = TypeVar("R", bound=BaseModel | JSONResponse | None)
 
 
 @overload
 def sideeffect(
     *,
     reload: tuple[Any, ...] | None = None,
-    response_model: Type[BaseModel] | None = None,
+    response_model: Type[BaseModel] | None = None,  # deprecated
     exception_models: list[Type[APIException]] | None = None,
     experimental_render_reload: bool | None = None,
 ) -> Callable[[Callable[P, R | Coroutine[Any, Any, R]]], Callable[P, Awaitable[R]]]:
     ...
 
 
 @overload
@@ -57,25 +57,46 @@
 
 
 def sideeffect(*args, **kwargs):  # type: ignore
     """
     Mark a function as causing a sideeffect to the data. This will force a reload of the full (or partial) server state
     and sync these changes down to the client page.
 
-    :reload: If provided, will ONLY reload these fields on the client side. By default will reload all fields. Otherwise, why
+    Like passthroughs, @sideeffect accepts return values of None, BaseModel, or a JSONResponse if you need full flexibility
+    on return headers and content structure. Unlike @passthrough, it does not allow you to provide a non-JSON response since we need
+    to internally merge it with render() sideeffect update.
+
+    :param exception_models: List of APIException subclasses that this function is known
+        to throw. These will be parsed and available to frontend clients.
+    :type exception_models: list[Type[APIException]] | None
+
+    :param reload:
+
+        If provided, will ONLY reload these fields on the client side. By default will reload all fields. Otherwise, why
         specify a sideeffect at all? Note that even if this is provided, we will still regenerate a fully full state on the server
         as if render() is called again. This parameter only controls the data that is streamed back to the client in order to help
         reduce bandwidth of data that won't be changed.
 
-    Experimental options. Disabled by default:
+    :type reload: tuple[FieldClassDefinition, ...] | None
+
+    :param experimental_render_reload:
 
-    :experimental_render_reload: If True, will attempt to only execute the logic in render() that is required to calculate your
+        Experimental options. Disabled by default.<br/><br/>
+
+        If True, will attempt to only execute the logic in render() that is required to calculate your
         `reload` parameters. Other logic will be short-circuited. If your render function has significant computation for other
         properties this can be a significant performance improvement. However, it is experimental and may not work in all cases.
 
+    :type experimental_render_reload: bool
+
+    :return: The response model to use for this endpoint. If a BaseModel is not provided (you pass
+        a dictionary or a SQLModel object ofr instance), we will try to convert the response object
+        into the proper JSON response based on your typehint.
+    :rtype: BaseModel | None | fastapi.JSONResponse
+
     """
 
     def decorator_with_args(
         reload: tuple[FieldClassDefinition, ...] | None = None,
         response_model: Type[BaseModel] | None = None,
         exception_models: list[Type[APIException]] | None = None,
         experimental_render_reload: bool = False,
```

### Comparing `mountaineer-0.3.1/mountaineer/annotation_helpers.py` & `mountaineer-0.3.2.dev1/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/app.py` & `mountaineer-0.3.2.dev1/mountaineer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,21 @@
         self.app.exception_handler(APIException)(self.handle_exception)
 
         self.app.openapi = self.generate_openapi  # type: ignore
 
     def register(self, controller: ControllerBase):
         """
         Register a new controller. This will:
-            - Mount the html of the controller to the main application service
-            - Mount all actions (ie. @sideeffect and @passthrough decorated functions) to their public API
+
+        - Mount the html of the controller to the main application service
+        - Mount all actions (ie. @sideeffect and @passthrough decorated functions) to their public API
+
+        :param controller: The controller instance that should be added to your webapp. The class accepts a full
+        instance instead of just a class, so you're able to perform any kind of runtime initialization of the
+        kwarg args that you need before it's registered.
 
         """
         # Since the controller name is used to build dependent files, we ensure
         # that we only register one controller of a given name
         controller_name = controller.__class__.__name__
         if controller_name in self.controller_names:
             raise ValueError(
```

### Comparing `mountaineer-0.3.1/mountaineer/cache.py` & `mountaineer-0.3.2.dev1/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/cli.py` & `mountaineer-0.3.2.dev1/mountaineer/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -272,16 +272,21 @@
     package: str,
     webcontroller: str,
     subscribe_to_mountaineer: bool = False,
 ):
     """
     Watch the file directory and rebuild auto-generated files.
 
-    :param client_package: "ci_webapp"
-    :param client_controller: "ci_webapp.app:controller"
+    :param package: Ex. "ci_webapp"
+    :param webcontroller: Ex. "ci_webapp.app:controller"
+    :param subscribe_to_mountaineer:
+        If True, will subscribe the local build server to changes in
+        the `mountaineer` package. This is useful when doing concurrent
+        development in `mountaineer` and a client package. Rarely
+        used otherwise.
 
     """
     update_multiprocessing_settings()
 
     current_process: IsolatedEnvProcess | None = None
 
     # The global cache will let us keep cache files warm across
@@ -326,17 +331,19 @@
     package: str,
     webservice: str,
     webcontroller: str,
     port: int,
     subscribe_to_mountaineer: bool = False,
 ):
     """
-    :param client_package: "ci_webapp"
-    :param client_webservice: "ci_webapp.app:app"
-    :param client_controller: "ci_webapp.app:controller"
+    :param package: Ex. "ci_webapp"
+    :param webservice: Ex. "ci_webapp.app:app"
+    :param webcontroller: Ex. "ci_webapp.app:controller"
+    :param port: Desired port for the webapp while running locally
+    :param subscribe_to_mountaineer: See `handle_watch` for more details.
 
     """
     update_multiprocessing_settings()
 
     current_process: IsolatedEnvProcess | None = None
 
     # The global cache will let us keep cache files warm across
@@ -398,14 +405,18 @@
         watchdog.start_watching()
 
 
 def handle_build(
     *,
     webcontroller: str,
 ):
+    """
+    Handle a one-off build. Most often used in production CI pipelines.
+
+    """
     app_controller = import_from_string(webcontroller)
     js_compiler = ClientBuilder(
         app_controller,
         live_reload_port=None,
     )
     start = time()
     js_compiler.build()
```

### Comparing `mountaineer-0.3.1/mountaineer/client_builder/build_actions.py` & `mountaineer-0.3.2.dev1/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/client_builder/build_links.py` & `mountaineer-0.3.2.dev1/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.3.2.dev1/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/client_builder/builder.py` & `mountaineer-0.3.2.dev1/mountaineer/client_builder/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/client_builder/openapi.py` & `mountaineer-0.3.2.dev1/mountaineer/client_builder/openapi.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/client_builder/typescript.py` & `mountaineer-0.3.2.dev1/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/config.py` & `mountaineer-0.3.2.dev1/mountaineer/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,26 @@
         instance = super().__call__(*args, **kwargs)
         register_config(instance)
         return instance
 
 
 @dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
 class ConfigBase(BaseSettings, metaclass=ConfigMeta):
+    """
+    Base class for the running application's configuration. By convention
+    all configuration parameters should be specified here in one payload.
+    You'll often call your subclass `ConfigBase`.
+
+    Users are responsible for instantiating an AppConfig with your desired
+    settings. This instance will be registered into the global space so it's
+    accessible to your controllers. An error will be thrown if you attempt to
+    instantiate more than one AppConfig.
+
+    """
+
     # Name of the python package
     PACKAGE: str | None = None
 
     model_config = {"frozen": True}
 
 
 # One global config object
```

### Comparing `mountaineer-0.3.1/mountaineer/controller.py` & `mountaineer-0.3.2.dev1/mountaineer/controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     # with state metadata
     definition: Optional["ControllerDefinition"] = None
 
     def __init__(
         self, slow_ssr_threshold: float = 0.1, hard_ssr_timeout: float | None = 10.0
     ):
         """
+        One Controller should be created for every frontend page in your webapp. Clients can override
+        this `__init__` function so long as they call `super().__init__()` at the start of their init
+        to setup the internal handlers.
+
         :param slow_ssr_threshold: Each python process has a single V8 runtime associated with
         it, so SSR rendering can become a bottleneck if it requires processing. We log a warning
         if we detect that an SSR render took longer than this threshold.
         :param hard_ssr_timeout: If the SSR render takes longer than this threshold, we will
         automatically kill the V8 runtime and return an error to the client. This is useful for
         avoiding blocking the reset of the server process if the React render logic hangs.
 
@@ -83,17 +87,20 @@
         self.resolve_paths()
 
     @abstractmethod
     def render(
         self, *args: RenderInput.args, **kwargs: RenderInput.kwargs
     ) -> RenderBase | None | Coroutine[Any, Any, RenderBase | None]:
         """
-        Client implementations must override render() to define the data that will
-        be pushed from the server to the client. This function must be typehinted with
-        your response type:
+        Render provides the raw data payload that will be sent to the frontend on initial
+        render and during any sideeffect update. In most cases, you should return a RenderBase
+        instance. If you have no data to display you can also return None.
+
+        This function must be explicitly typehinted with your response type, which allows the
+        AppController to generate the correct TypeScript types for the frontend:
 
         ```python
         class MyServerData(RenderBase):
             pass
 
         class MyController:
             def render(self) -> MyServerData:
@@ -105,14 +112,31 @@
 
         ```python
         class MyController:
             def render(self) -> None:
                 pass
         ```
 
+        Render functions accept any number of arguments and keyword arguments, following the FastAPI
+        route parameter style. This includes query parameters, path parameters, and request bodies.
+
+        ```python
+        class MyController:
+            url = "/my-url/{path_param}"
+
+            def render(
+                self,
+                query_param: str,
+                path_param: int,
+                dependency: MyDependency = Depends(MyDependency),
+            ) -> MyServerData:
+                ...
+        ```
+
+        :return: A RenderBase instance or None
         """
         pass
 
     async def _generate_html(self, *args, global_metadata: Metadata | None, **kwargs):
         # Because JSON is a subset of JavaScript, we can just dump the model as JSON and
         # insert it into the page.
         server_data = self.render(*args, **kwargs)
@@ -137,15 +161,15 @@
             metadatas.append(server_data.metadata)
         if global_metadata and (
             server_data.metadata is None
             or not server_data.metadata.ignore_global_metadata
         ):
             metadatas.append(global_metadata)
 
-        header_str = "\n".join(self.build_header(self.merge_metadatas(metadatas)))
+        header_str = "\n".join(self._build_header(self._merge_metadatas(metadatas)))
 
         ssr_html = self._generate_ssr_html(server_data)
 
         # Client-side react scripts that will hydrate the server side contents on load
         server_data_json = server_data.model_dump_json()
         optional_scripts = "\n".join(
             [
@@ -204,15 +228,15 @@
         if ssr_duration > self.slow_ssr_threshold:
             LOGGER.warning(f"Slow SSR render detected: {ssr_duration:.2f}s")
         else:
             LOGGER.debug(f"SSR render took {ssr_duration:.2f}s")
 
         return cast(str, ssr_html)
 
-    def build_header(self, metadata: Metadata) -> list[str]:
+    def _build_header(self, metadata: Metadata) -> list[str]:
         """
         Builds the header for this controller. Returns the list of tags that will be injected into the
         <head> tag of the rendered page.
 
         """
         tags: list[str] = []
 
@@ -278,18 +302,19 @@
                 }:
                     yield name, func, metadata
             except AttributeError:
                 continue
 
     def resolve_paths(self, view_base: Path | None = None, force: bool = True) -> bool:
         """
-        Given the path to the root /view directory, resolve our various
-        on-disk paths.
+        Typically used internally by the Mountaineer build pipeline. Calling this function
+        sets the active `view_base` of the frontend project, which allows us to resolve the
+        built javascripts that are required for this controller.
 
-        Returns a boolean for whether we have fully updated the controller state.
+        :return: Whether we have found all necessary files and fully updated the controller state.
 
         """
         if not force and self.view_base_path is not None:
             return False
 
         # Try to resolve the view base path from the global config
         if view_base is None:
@@ -336,15 +361,15 @@
                 f"[{self.__class__.__name__}] Resolved paths... {self.bundled_scripts}"
             )
         else:
             found_dependencies = False
 
         return found_dependencies
 
-    def merge_metadatas(self, metadatas: list[Metadata]):
+    def _merge_metadatas(self, metadatas: list[Metadata]):
         """
         Merges a list of metadata objects, sorted by priority. Some fields will
         take the union (like scripts) - others will prioritize earlier entries (title).
 
         """
         # Keep track of the unique values we've seen already to ensure that we are:
         # 1. Only including unique values
```

### Comparing `mountaineer-0.3.1/mountaineer/controllers/exception_controller.py` & `mountaineer-0.3.2.dev1/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/cropper.py` & `mountaineer-0.3.2.dev1/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/database/cli.py` & `mountaineer-0.3.2.dev1/mountaineer/database/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,17 +18,22 @@
 @overload
 async def handle_createdb(models: list[SQLModel]) -> None:
     ...
 
 
 async def handle_createdb(*args, **kwargs):
     """
-    Strictly speaking, passing a list of models isn't required. We just encourage
-    an explicit passing of either the models module or the SQLModels themselves to make
-    sure they are in-scope of the table registry when this function is run.
+    Strictly speaking, passing a list of models isn't required for this function. We'll happily
+    accept being called with `handle_createdb()`. We just encourage an explicit passing of either
+    the models module or the SQLModels themselves to make sure they are in-scope of the table
+    registry when this function is run. This is how we determine which tables to create at runtime.
+
+    :param model_module: The module containing the SQLModels to create
+
+    :param models: An explicit list of SQLModels to create
 
     """
 
     async def run_migrations(
         engine: AsyncEngine = Depends(DatabaseDependencies.get_db),
     ):
         async with engine.begin() as connection:
```

### Comparing `mountaineer-0.3.1/mountaineer/database/config.py` & `mountaineer-0.3.2.dev1/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/database/sqlmodel.py` & `mountaineer-0.3.2.dev1/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/database/validator.py` & `mountaineer-0.3.2.dev1/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/dependencies/base.py` & `mountaineer-0.3.2.dev1/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/exceptions.py` & `mountaineer-0.3.2.dev1/mountaineer/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,14 +60,37 @@
             }
         )
         setattr(instance, "internal_model", internal_model)
         return instance
 
 
 class APIException(HTTPException, metaclass=InternalModelMeta):
+    """
+    Base class for user defined APIExceptions that can be thrown
+    in server actions and should provide some metadata back to
+    the client caller.
+
+    ```python
+    class PostNotFound(APIException):
+        status_code: int = 404
+        detail: str = "The post was not found"
+        post_id: int
+        is_deleted: bool
+
+    class MyController(ControllerBase):
+        @passthrough
+        def get_post(self, post_id: int) -> Post:
+            post = self.post_service.get_post(post_id)
+            if not post:
+                raise PostNotFound(post_id=post_id, is_deleted=True)
+            return post
+    ```
+
+    """
+
     status_code: int = 500
     detail: str = "A server error occurred"
     headers: dict[str, str] = Field(default_factory=dict)
 
     InternalModel: Type[APIExceptionInternalModelBase]
     internal_model: APIExceptionInternalModelBase
```

### Comparing `mountaineer-0.3.1/mountaineer/io.py` & `mountaineer-0.3.2.dev1/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/js_compiler/base.py` & `mountaineer-0.3.2.dev1/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/js_compiler/javascript.py` & `mountaineer-0.3.2.dev1/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/js_compiler/postcss.py` & `mountaineer-0.3.2.dev1/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/paths.py` & `mountaineer-0.3.2.dev1/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/render.py` & `mountaineer-0.3.2.dev1/mountaineer/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,27 +78,52 @@
 class MetaAttribute(HashableAttribute, BaseModel):
     name: str | None = None
     content: str | None = None
     optional_attributes: dict[str, str] = {}
 
 
 class ThemeColorMeta(MetaAttribute):
+    """
+    Customizes the default color that is attached to the page.
+
+    ```python
+    ThemeColorMeta(
+        color="white",
+        media="light",
+    )
+    ```
+
+    """
+
     color: str
     media: str | None = None
 
     @model_validator(mode="after")
     def create_attribute(self):
         self.name = "theme-color"
         self.content = self.color
         if self.media:
             self.optional_attributes = {"media": self.media}
         return self
 
 
 class ViewportMeta(MetaAttribute):
+    """
+    Defines the bounds on the current page and how much users are able to zoom.
+
+    ```python
+    ViewportMeta(
+        initial_scale=1.0,
+        maximum_scale=2.0,
+        user_scalable=True,
+    )
+    ```
+
+    """
+
     width: str = "device-width"
     initial_scale: float = 1.0
     maximum_scale: float = 1.0
     user_scalable: bool = False
 
     @model_validator(mode="after")
     def create_attribute(self):
```

### Comparing `mountaineer-0.3.1/mountaineer/ssr.py` & `mountaineer-0.3.2.dev1/mountaineer/ssr.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 
 from mountaineer import mountaineer as mountaineer_rs  # type: ignore
 from mountaineer.cache import extended_lru_cache
 from mountaineer.static import get_static_path
 
 
 class V8RuntimeError(Exception):
+    """
+    An exception thrown by the V8 runtime in the case of a permanent failure that
+    involves the content of the script.
+
+    """
+
     pass
 
 
 def fix_exception_lines(*, exception: str, injected_script: str):
     """
     Since we create a synthetic script to run in the V8 runtime, the line numbers
     of the in-application stack trace will be offset by however long our
@@ -38,21 +44,29 @@
 
 
 @extended_lru_cache(maxsize=128, max_size_mb=5)
 def render_ssr(
     script: str, render_data: BaseModel, hard_timeout: int | float | None = None
 ) -> str:
     """
-    Render the react component in the provided SSR javascript bundle. This file will
+    Render the React component in the provided SSR javascript bundle. This file will
     be directly executed within the V8 runtime.
 
-    To speed up requests for the same exact content in the same time (ie. same react and same data)
-    we cache the result of the render_ssr_rust call.
+    To speed up requests for the same exact content (ie. same react and same data)
+    we cache the result of the render_ssr_rust call by default for a limited amount of
+    previous calls. We limit the overall size of this cache to 5MB.
+
+    :param script: The raw code of the javascript bundle to execute. Should be pre-compiled into an
+        SSR compatible package with a single entrypoint.
+    :param render_data: The data to inject into the SSR javascript bundle
+    :param hard_timeout: The maximum time to allow the render to take in seconds. If the render takes
+        longer than this time, our thread supervisor will kick in and terminate the rust worker.
 
     :raises TimeoutError: If the render takes longer than the hard_timeout
+    :raises V8RuntimeError: If the V8 runtime throws an exception during the render
 
     """
     polyfill_script = get_static_path("ssr_polyfills.js").read_text()
     data_json = render_data.model_dump_json()
 
     injected_script = f"const SERVER_DATA = {data_json};\n{polyfill_script}\n"
     full_script = f"{injected_script}{script}"
```

### Comparing `mountaineer-0.3.1/mountaineer/static/api.ts` & `mountaineer-0.3.2.dev1/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/static/live_reload.ts` & `mountaineer-0.3.2.dev1/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/test_utilities.py` & `mountaineer-0.3.2.dev1/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/views/package-lock.json` & `mountaineer-0.3.2.dev1/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/watch.py` & `mountaineer-0.3.2.dev1/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/watch_server.py` & `mountaineer-0.3.2.dev1/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/mountaineer/webservice.py` & `mountaineer-0.3.2.dev1/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/poetry.lock` & `mountaineer-0.3.2.dev1/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.3.2.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.3.2.dev1/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/benches/lexers_benchmark.rs` & `mountaineer-0.3.2.dev1/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/benches/source_map_benchmark.rs` & `mountaineer-0.3.2.dev1/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/benches/ssr_benchmark.rs` & `mountaineer-0.3.2.dev1/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/lexers.rs` & `mountaineer-0.3.2.dev1/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/lib.rs` & `mountaineer-0.3.2.dev1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/logging.rs` & `mountaineer-0.3.2.dev1/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/source_map.rs` & `mountaineer-0.3.2.dev1/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/ssr.rs` & `mountaineer-0.3.2.dev1/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/src/timeout.rs` & `mountaineer-0.3.2.dev1/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/Cargo.lock` & `mountaineer-0.3.2.dev1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.3.1"
+version = "0.3.2-dev1"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.3.1/pyproject.toml` & `mountaineer-0.3.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.1/PKG-INFO` & `mountaineer-0.3.2.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.3.1
+Version: 0.3.2.dev1
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: tqdm
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
@@ -12,15 +12,15 @@
 Requires-Dist: pydantic-settings
 Requires-Dist: sqlmodel
 Requires-Dist: asyncpg
 Requires-Dist: sqlalchemy[asyncio]
 License-File: LICENSE
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-![Mountaineer Header](https://raw.githubusercontent.com/piercefreeman/mountaineer/main/docs/media/header.png)
+![Mountaineer Header](https://raw.githubusercontent.com/piercefreeman/mountaineer/main/media/header.png)
 
 <p align="center"><i>Move fast. Climb mountains. Don't break things.</i></p>
 
 Mountaineer 🏔️ is a framework to easily build webapps in Python and React. If you've used either of these languages before for development, we think you'll be right at home.
 
 ## Main Features
 
@@ -275,22 +275,22 @@
 export default Home;
 ```
 
 We define a simple view to show the data coming from the backend. To accomplish this conventionally, we'd need to wire up an API layer, a Node server, or format the page with Jinja templates.
 
 Here instead we use our automatically generated `useServer()` hook. This hook payload will provide all the `HomeRender` fields as properties of serverState. And it's available instantly on page load without any roundtrip fetches. Also - if your IDE supports language servers (which most do these days), you should see the fields auto-suggesting for `serverState` as you type.
 
-<p align="center"><img src="./docs/media/ide_typehints.png" alt="IDE Typehints" width="500px" /></p>
+<p align="center"><img src="./docs_website/docs/media/ide_typehints.png" alt="IDE Typehints" width="500px" /></p>
 
 If you access this in your browser at `localhost:5006/` we can see our welcome message, but we can't really _do_ anything with the todos yet. Let's add some interactivity.
 
 > [!TIP]
 > Try disabling Javascript in your browser. The page will still render as-is with all variables intact, thanks to our server-side rendering.
 
-<p align="center"><img src="./docs/media/server_side_rendering.png" alt="Server-side rendering" height="400px" /></p>
+<p align="center"><img src="./docs_website/docs/media/server_side_rendering.png" alt="Server-side rendering" height="400px" /></p>
 
 What good is todo list that doesn't get longer? We define a `add_todo` function that accepts a pydantic model `NewTodoRequest`, which defines the required parameters for a new todo item. We then cast this to a database object and add it to the postgres table.
 
 ```python
 # my_webapp/controllers/home.py
 
 from pydantic import BaseModel
@@ -359,28 +359,19 @@
 export default Home;
 ```
 
 `useServer()` exposes our `add_todo` function so we can call our backend directly from our frontend. Also notice that we don't have to read or parse the output value of this function to render the new todo item to the list. Since the function is marked as a sideeffect, the frontend will automatically refresh its data after the function is called.
 
 Go ahead and load it in your browser. If you open up your web tools, you can create a new Todo and see POST requests sending data to the backend and receiving the current server state. The actual data updates and merging happens internally by Mountaineer.
 
-<p align="center"><img src="./docs/media/final_todo_list.png" alt="Getting Started Final TODO App" height="400px" /></p>
+<p align="center"><img src="./docs_website/docs/media/final_todo_list.png" alt="Getting Started Final TODO App" height="400px" /></p>
 
-<p align="center"><img src="./docs/media/network_debug.png" alt="Getting Started Final TODO App" height="400px" /></p>
+<p align="center"><img src="./docs_website/docs/media/network_debug.png" alt="Getting Started Final TODO App" height="400px" /></p>
 
 You can use these serverState variables anywhere you'd use dynamic React state variables (useEffect, useCallback, etc). But unlike React state, these variables are automatically updated when a relevant sideeffect is triggered.
 
 And that's it. We've just built a fully interactive web application without having to worry about an explicit API. You specify the data model and actions on the server and the appropriate frontend hooks are generated and updated automatically. It gives you the power of server rendered html and the interactivity of a virtual DOM, without having to compromise on complicated data mutations to keep everything in sync.
 
 ### Learn More
 
-We have additional documentation that does more of a technical deep dive on different features of Mountaineer. We order these roughly in the order that we anticipate you'll need them.
-
-- [Client Actions](./docs/client_actions.md): Details on @sideeffect, @passthrough, and masking @sideeffect fields for partial re-rendering.
-- [View Definition](./docs/view.md): How to define the view and use the serverState hook. Covers `page.tsx` and `layout.tsx` conventions to easily nest your site designs.
-- [Page Metadata](./docs/metadata.md): How to set the title, description, and other metadata for your pages.
-- [Link Generation](./docs/links.md): Generate links to other pages within your webapp, with typehinting and automatic URL generation.
-- [Error Handling](./docs/error_handling.md): Conventions for handling client-side errors while fetching data in your webapp.
-- [PostCSS](./docs/postcss.md): PostCSS build plugin for TailwindCSS support and other CSS processing.
-- [Database](./docs/database.md): Database conventions.
-- [Core Library](./docs/core_library.md): Details on how to do local development on the core library.
+We have additional documentation that does more of a technical deep dive on different features of Mountaineer. Check out [mountaineer.sh](https://mountaineer.sh/).
```

