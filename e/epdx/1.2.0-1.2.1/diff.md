# Comparing `tmp/epdx-1.2.0.tar.gz` & `tmp/epdx-1.2.1.tar.gz`

## Comparing `epdx-1.2.0.tar` & `epdx-1.2.1.tar`

### file list

```diff
@@ -1,76 +1,78 @@
--rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 epdx-1.2.0/Cargo.toml
--rw-r--r--   0     1001      127       11 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/CODEOWNERS
--rw-r--r--   0     1001      127       64 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127      842 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/build_javascript.yaml
--rw-r--r--   0     1001      127     1171 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/build_python.yaml
--rw-r--r--   0     1001      127      527 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/build_rust.yaml
--rw-r--r--   0     1001      127     1993 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/cicd.yaml
--rw-r--r--   0     1001      127     2867 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/create_release.yaml
--rw-r--r--   0     1001      127      739 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/publish_javascript.yaml
--rw-r--r--   0     1001      127      946 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/publish_python.yaml
--rw-r--r--   0     1001      127     2138 2024-03-24 14:33:20.000000 epdx-1.2.0/.github/workflows/release_docs.yaml
--rw-r--r--   0     1001      127      187 2024-03-24 14:33:20.000000 epdx-1.2.0/.gitignore
--rw-r--r--   0     1001      127      788 2024-03-24 14:33:20.000000 epdx-1.2.0/.releaserc.yaml
--rw-r--r--   0     1001      127     2441 2024-03-24 14:33:20.000000 epdx-1.2.0/CHANGELOG.md
--rw-r--r--   0     1001      127    21353 2024-03-24 14:33:20.000000 epdx-1.2.0/Cargo.lock
--rw-r--r--   0     1001      127     9723 2024-03-24 14:33:20.000000 epdx-1.2.0/LICENSE
--rw-r--r--   0     1001      127     2671 2024-03-24 14:33:20.000000 epdx-1.2.0/README.md
--rw-r--r--   0     1001      127   334123 2024-03-24 14:34:24.000000 epdx-1.2.0/dist/epdx-1.2.0-cp310-abi3-manylinux_2_34_x86_64.whl
--rwxr-xr-x   0     1001      127    69619 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/code/data/ilcd.json
--rw-r--r--   0     1001      127      229 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/code/javascript/usage.js
--rw-r--r--   0     1001      127      468 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/code/python/usage.py
--rw-r--r--   0     1001      127     1946 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/index.md
--rw-r--r--   0     1001      127      122 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/overrides/partials/integrations/analytics/custom.html
--rw-r--r--   0     1001      127      335 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/overrides/stylesheets/extra.css
--rw-r--r--   0     1001      127        0 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/schemas/.gitkeep
--rw-r--r--   0     1001      127      224 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/schemas.md
--rw-r--r--   0     1001      127     7974 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/usage/custom_parser_python.md
--rw-r--r--   0     1001      127      157 2024-03-24 14:33:20.000000 epdx-1.2.0/docs/usage/usage.md
--rw-r--r--   0     1001      127     1072 2024-03-24 14:33:20.000000 epdx-1.2.0/mkdocs.yml
--rw-r--r--   0     1001      127     9723 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/LICENSE
--rw-r--r--   0     1001      127     2634 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/README.md
--rw-r--r--   0     1001      127    50597 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/package-lock.json
--rw-r--r--   0     1001      127      688 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/package.json
--rw-r--r--   0     1001      127     2151 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/src/epdx.d.ts
--rw-r--r--   0     1001      127      139 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/src/epdx.js
--rw-r--r--   0     1001      127     4252 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/src/epdx_bg.js
--rw-r--r--   0     1001      127   228368 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/src/epdx_bg.wasm
--rw-r--r--   0     1001      127      427 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/src/epdx_bg.wasm.d.ts
--rwxr-xr-x   0     1001      127    69619 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
--rwxr-xr-x   0     1001      127    47820 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/tests/datafixtures/f63ac879_test.json
--rw-r--r--   0     1001      127      772 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/tests/epdx.spec.tsx
--rw-r--r--   0     1001      127      309 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/javascript/vitest.config.js
--rw-r--r--   0     1001      127      933 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/python/src/epdx/__init__.py
--rw-r--r--   0     1001      127      129 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/python/src/epdx/epdx.pyi
--rw-r--r--   0     1001      127     2871 2024-03-24 14:33:21.000000 epdx-1.2.0/packages/python/src/epdx/pydantic.py
--rw-r--r--   0     1001      127        0 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/python/tests/conftest.py
--rwxr-xr-x   0     1001      127    69619 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/python/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
--rw-r--r--   0     1001      127     1009 2024-03-24 14:33:20.000000 epdx-1.2.0/packages/python/tests/test_parse.py
--rw-r--r--   0     1001      127    20836 2024-03-24 14:33:20.000000 epdx-1.2.0/src/epd.rs
--rw-r--r--   0     1001      127     5605 2024-03-24 14:33:20.000000 epdx-1.2.0/src/ilcd.rs
--rw-r--r--   0     1001      127      587 2024-03-24 14:33:20.000000 epdx-1.2.0/src/javascript.rs
--rw-r--r--   0     1001      127     4377 2024-03-24 14:33:20.000000 epdx-1.2.0/src/lcabyg.rs
--rw-r--r--   0     1001      127      412 2024-03-24 14:33:20.000000 epdx-1.2.0/src/lib.rs
--rw-r--r--   0     1001      127      397 2024-03-24 14:33:20.000000 epdx-1.2.0/src/parse.rs
--rw-r--r--   0     1001      127      720 2024-03-24 14:33:20.000000 epdx-1.2.0/src/python.rs
--rw-r--r--   0     1001      127      184 2024-03-24 14:33:20.000000 epdx-1.2.0/src/schemars.rs
--rw-r--r--   0     1001      127      686 2024-03-24 14:33:20.000000 epdx-1.2.0/src/utils.rs
--rw-r--r--   0     1001      127    64785 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
--rw-r--r--   0     1001      127    68643 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
--rw-r--r--   0     1001      127    70431 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0b488798-140f-4efa-96e2-55aa46ed129a.json
--rw-r--r--   0     1001      127    70200 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
--rw-r--r--   0     1001      127    84820 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0cb92770-9007-48c6-bc03-466af8894419.json
--rw-r--r--   0     1001      127    50733 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0d1e4a59-4901-4973-a26f-1698f65a780f.json
--rw-r--r--   0     1001      127    80754 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
--rw-r--r--   0     1001      127   102497 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
--rw-r--r--   0     1001      127    88446 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0e85f255-4d11-4973-9daa-c03889948351.json
--rw-r--r--   0     1001      127   111759 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/0e9fd868-9656-489e-be6c-8251b3d43283.json
--rw-r--r--   0     1001      127    52735 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
--rwxr-xr-x   0     1001      127    69619 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
--rwxr-xr-x   0     1001      127    47820 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/ilcd/f63ac879_test.json
--rw-r--r--   0     1001      127     2779 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/datafixtures/lcabyg/5aa09d72.json
--rw-r--r--   0     1001      127     2628 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/test_parse_ilcd.rs
--rw-r--r--   0     1001      127     1536 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/test_parse_lcabyg.rs
--rw-r--r--   0     1001      127      251 2024-03-24 14:33:20.000000 epdx-1.2.0/tests/web.rs
--rw-r--r--   0     1001      127      946 2024-03-24 14:33:20.000000 epdx-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3632 1970-01-01 00:00:00.000000 epdx-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 epdx-1.2.1/Cargo.toml
+-rw-r--r--   0     1001      127       11 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/CODEOWNERS
+-rw-r--r--   0     1001      127       64 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      842 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/build_javascript.yaml
+-rw-r--r--   0     1001      127     1171 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/build_python.yaml
+-rw-r--r--   0     1001      127      527 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/build_rust.yaml
+-rw-r--r--   0     1001      127     1993 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/cicd.yaml
+-rw-r--r--   0     1001      127     2867 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/create_release.yaml
+-rw-r--r--   0     1001      127      739 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/publish_javascript.yaml
+-rw-r--r--   0     1001      127      946 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/publish_python.yaml
+-rw-r--r--   0     1001      127     2138 2024-04-01 18:50:35.000000 epdx-1.2.1/.github/workflows/release_docs.yaml
+-rw-r--r--   0     1001      127      187 2024-04-01 18:50:35.000000 epdx-1.2.1/.gitignore
+-rw-r--r--   0     1001      127      788 2024-04-01 18:50:35.000000 epdx-1.2.1/.releaserc.yaml
+-rw-r--r--   0     1001      127     2972 2024-04-01 18:50:35.000000 epdx-1.2.1/CHANGELOG.md
+-rw-r--r--   0     1001      127    21353 2024-04-01 18:50:36.000000 epdx-1.2.1/Cargo.lock
+-rw-r--r--   0     1001      127     9723 2024-04-01 18:50:35.000000 epdx-1.2.1/LICENSE
+-rw-r--r--   0     1001      127     2672 2024-04-01 18:50:35.000000 epdx-1.2.1/README.md
+-rw-r--r--   0     1001      127   392121 2024-04-01 18:51:21.000000 epdx-1.2.1/dist/epdx-1.2.1-cp310-abi3-manylinux_2_34_x86_64.whl
+-rwxr-xr-x   0     1001      127    69619 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/code/data/ilcd.json
+-rw-r--r--   0     1001      127      229 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/code/javascript/usage.js
+-rw-r--r--   0     1001      127      468 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/code/python/usage.py
+-rw-r--r--   0     1001      127     1946 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/index.md
+-rw-r--r--   0     1001      127      122 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/overrides/partials/integrations/analytics/custom.html
+-rw-r--r--   0     1001      127      335 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/overrides/stylesheets/extra.css
+-rw-r--r--   0     1001      127        0 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/schemas/.gitkeep
+-rw-r--r--   0     1001      127      224 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/schemas.md
+-rw-r--r--   0     1001      127     7974 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/usage/custom_parser_python.md
+-rw-r--r--   0     1001      127      157 2024-04-01 18:50:35.000000 epdx-1.2.1/docs/usage/usage.md
+-rw-r--r--   0     1001      127     1072 2024-04-01 18:50:35.000000 epdx-1.2.1/mkdocs.yml
+-rw-r--r--   0     1001      127     9723 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/LICENSE
+-rw-r--r--   0     1001      127     2634 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/README.md
+-rw-r--r--   0     1001      127    50597 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/package-lock.json
+-rw-r--r--   0     1001      127      688 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/package.json
+-rw-r--r--   0     1001      127     2151 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/src/epdx.d.ts
+-rw-r--r--   0     1001      127      139 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/src/epdx.js
+-rw-r--r--   0     1001      127     4252 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/src/epdx_bg.js
+-rw-r--r--   0     1001      127   228368 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/src/epdx_bg.wasm
+-rw-r--r--   0     1001      127      427 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/src/epdx_bg.wasm.d.ts
+-rwxr-xr-x   0     1001      127    69619 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rwxr-xr-x   0     1001      127    47820 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/tests/datafixtures/f63ac879_test.json
+-rw-r--r--   0     1001      127      772 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/tests/epdx.spec.tsx
+-rw-r--r--   0     1001      127      309 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/javascript/vitest.config.js
+-rw-r--r--   0     1001      127      933 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/python/src/epdx/__init__.py
+-rw-r--r--   0     1001      127      129 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/python/src/epdx/epdx.pyi
+-rw-r--r--   0     1001      127     2871 2024-04-01 18:50:36.000000 epdx-1.2.1/packages/python/src/epdx/pydantic.py
+-rw-r--r--   0     1001      127        0 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/python/tests/conftest.py
+-rwxr-xr-x   0     1001      127    69619 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/python/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rw-r--r--   0     1001      127     1009 2024-04-01 18:50:35.000000 epdx-1.2.1/packages/python/tests/test_parse.py
+-rw-r--r--   0     1001      127    21042 2024-04-01 18:50:35.000000 epdx-1.2.1/src/epd.rs
+-rw-r--r--   0     1001      127     5596 2024-04-01 18:50:35.000000 epdx-1.2.1/src/ilcd.rs
+-rw-r--r--   0     1001      127      587 2024-04-01 18:50:35.000000 epdx-1.2.1/src/javascript.rs
+-rw-r--r--   0     1001      127     4377 2024-04-01 18:50:35.000000 epdx-1.2.1/src/lcabyg.rs
+-rw-r--r--   0     1001      127      412 2024-04-01 18:50:35.000000 epdx-1.2.1/src/lib.rs
+-rw-r--r--   0     1001      127      397 2024-04-01 18:50:35.000000 epdx-1.2.1/src/parse.rs
+-rw-r--r--   0     1001      127      720 2024-04-01 18:50:35.000000 epdx-1.2.1/src/python.rs
+-rw-r--r--   0     1001      127      184 2024-04-01 18:50:35.000000 epdx-1.2.1/src/schemars.rs
+-rw-r--r--   0     1001      127      686 2024-04-01 18:50:35.000000 epdx-1.2.1/src/utils.rs
+-rw-r--r--   0     1001      127    64785 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
+-rw-r--r--   0     1001      127    68643 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
+-rw-r--r--   0     1001      127    81962 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
+-rw-r--r--   0     1001      127    70431 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0b488798-140f-4efa-96e2-55aa46ed129a.json
+-rw-r--r--   0     1001      127    70200 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
+-rw-r--r--   0     1001      127    84820 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0cb92770-9007-48c6-bc03-466af8894419.json
+-rw-r--r--   0     1001      127    50733 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0d1e4a59-4901-4973-a26f-1698f65a780f.json
+-rw-r--r--   0     1001      127    80754 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
+-rw-r--r--   0     1001      127   102497 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
+-rw-r--r--   0     1001      127    88446 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0e85f255-4d11-4973-9daa-c03889948351.json
+-rw-r--r--   0     1001      127   111759 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/0e9fd868-9656-489e-be6c-8251b3d43283.json
+-rw-r--r--   0     1001      127    87077 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/335241f9-db84-486c-9a19-cd5ebb791903.json
+-rw-r--r--   0     1001      127    52735 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
+-rwxr-xr-x   0     1001      127    69619 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rwxr-xr-x   0     1001      127    47820 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/ilcd/f63ac879_test.json
+-rw-r--r--   0     1001      127     2779 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/datafixtures/lcabyg/5aa09d72.json
+-rw-r--r--   0     1001      127     2762 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/test_parse_ilcd.rs
+-rw-r--r--   0     1001      127     1536 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/test_parse_lcabyg.rs
+-rw-r--r--   0     1001      127      251 2024-04-01 18:50:35.000000 epdx-1.2.1/tests/web.rs
+-rw-r--r--   0     1001      127      946 2024-04-01 18:50:35.000000 epdx-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 epdx-1.2.1/PKG-INFO
```

### Comparing `epdx-1.2.0/Cargo.toml` & `epdx-1.2.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "epdx"
 description = "EPDx is a library for parsing EPD files into a common exchange format."
-version = "1.2.0"
+version = "1.2.1"
 authors = ["Christian Kongsgaard <christian@kongsgaard.eu>"]
 edition = "2018"
 readme = "README.md"
 license-file = "LICENSE"
 homepage = "https://epdx.kongsgaard.eu"
 documentation = "https://epdx.kongsgaard.eu"
 repository = "https://github.com/ocni-dtu/epdx"
```

### Comparing `epdx-1.2.0/.github/workflows/build_javascript.yaml` & `epdx-1.2.1/.github/workflows/build_javascript.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/build_python.yaml` & `epdx-1.2.1/.github/workflows/build_python.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/build_rust.yaml` & `epdx-1.2.1/.github/workflows/build_rust.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/cicd.yaml` & `epdx-1.2.1/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/create_release.yaml` & `epdx-1.2.1/.github/workflows/create_release.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/publish_javascript.yaml` & `epdx-1.2.1/.github/workflows/publish_javascript.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/publish_python.yaml` & `epdx-1.2.1/.github/workflows/publish_python.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.github/workflows/release_docs.yaml` & `epdx-1.2.1/.github/workflows/release_docs.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/.releaserc.yaml` & `epdx-1.2.1/.releaserc.yaml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/CHANGELOG.md` & `epdx-1.2.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## [1.2.0](https://github.com/ocni-dtu/epdx/compare/v1.1.5...v1.2.0) (2024-03-24)
+
+
+### Features
+
+* added functionality for LCAbyg data ([0ac8276](https://github.com/ocni-dtu/epdx/commit/0ac82760bb10992be92c70654a14b8efb9e3e904))
+* added functionality to parse LCAbyg EPDs (LCAByg stages) ([b2184ba](https://github.com/ocni-dtu/epdx/commit/b2184bae7aae4e7724ec46ead02b9c15c989fe42))
+
+
+### Bug Fixes
+
+* bug fix in as_type error handling ([4334de6](https://github.com/ocni-dtu/epdx/commit/4334de6232c2b005ee5f9c8dae52447ecc54a73e))
+
 ## [1.1.5](https://github.com/ocni-dtu/epdx/compare/v1.1.4...v1.1.5) (2024-02-22)
 
 
 ### Bug Fixes
 
 * handling non-english EPDs ([87fe672](https://github.com/ocni-dtu/epdx/commit/87fe67207d712c53726314d772cf183b9206f897))
```

### Comparing `epdx-1.2.0/Cargo.lock` & `epdx-1.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 name = "dyn-clone"
 version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "545b22097d44f8a9581187cdf93de7a71e4722bf51200cfaba810865b49a495d"
 
 [[package]]
 name = "epdx"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = [
  "chrono",
  "console_error_panic_hook",
  "pkg-version",
  "pyo3",
  "schemars",
  "serde",
```

### Comparing `epdx-1.2.0/LICENSE` & `epdx-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/README.md` & `epdx-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,23 +71,23 @@
 cargo test --package epdx --target x86_64-unknown-linux-gnu
 ```
 
 ## Run Python Tests
 
 ```bash
 maturin develop --extras tests --target x86_64-unknown-linux-gnu
-source .venv/bin/active .
+source .venv/bin/activate .
 cd packages/python
 pytest tests/
 ```
 
 ## Build Documentation
 
 ```bash
-maturin develop --extras doc,code-gen --target x86_64-unknown-linux-gnu
+maturin develop --extras doc,codegen --target x86_64-unknown-linux-gnu
 mkdocs develop
 ```
 
 ## Build JS Package
 
 ```bash
 wasm-pack build --features jsbindings
```

### Comparing `epdx-1.2.0/docs/code/data/ilcd.json` & `epdx-1.2.1/docs/code/data/ilcd.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/docs/index.md` & `epdx-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/docs/usage/custom_parser_python.md` & `epdx-1.2.1/docs/usage/custom_parser_python.md`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/mkdocs.yml` & `epdx-1.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/LICENSE` & `epdx-1.2.1/packages/javascript/LICENSE`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/README.md` & `epdx-1.2.1/packages/javascript/README.md`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/package-lock.json` & `epdx-1.2.1/packages/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/package.json` & `epdx-1.2.1/packages/javascript/package.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/src/epdx.d.ts` & `epdx-1.2.1/packages/javascript/src/epdx.d.ts`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/src/epdx_bg.js` & `epdx-1.2.1/packages/javascript/src/epdx_bg.js`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/src/epdx_bg.wasm` & `epdx-1.2.1/packages/javascript/src/epdx_bg.wasm`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json` & `epdx-1.2.1/packages/javascript/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/tests/datafixtures/f63ac879_test.json` & `epdx-1.2.1/packages/javascript/tests/datafixtures/f63ac879_test.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/javascript/tests/epdx.spec.tsx` & `epdx-1.2.1/packages/javascript/tests/epdx.spec.tsx`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/python/src/epdx/__init__.py` & `epdx-1.2.1/packages/python/src/epdx/__init__.py`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/python/src/epdx/pydantic.py` & `epdx-1.2.1/packages/python/src/epdx/pydantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  epdx.schema.json
-#   timestamp: 2024-03-24T14:31:55+00:00
+#   timestamp: 2024-04-01T18:48:52+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
```

### Comparing `epdx-1.2.0/packages/python/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json` & `epdx-1.2.1/packages/python/tests/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/packages/python/tests/test_parse.py` & `epdx-1.2.1/packages/python/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/src/epd.rs` & `epdx-1.2.1/src/epd.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 use chrono::prelude::*;
 use chrono::{DateTime, Utc};
 use pkg_version::*;
 use schemars::JsonSchema;
 use serde::{Deserialize, Deserializer, Serialize};
 use std::collections::HashMap;
 
-use crate::ilcd::{Exchange, LCIAResult, ModuleAnie, ILCD};
+use crate::ilcd::{Exchange, LCIAResult, ModuleAnie, ILCD, DataSetName};
 
 #[cfg(feature = "jsbindings")]
 use tsify::Tsify;
 
 #[derive(Serialize, JsonSchema, Clone)]
 #[cfg_attr(
-    feature = "jsbindings",
-    derive(Tsify),
-    tsify(into_wasm_abi, from_wasm_abi)
+feature = "jsbindings",
+derive(Tsify),
+tsify(into_wasm_abi, from_wasm_abi)
 )]
 pub struct EPD {
     pub id: String,
     pub name: String,
     pub declared_unit: Unit,
     pub version: String,
 
@@ -321,16 +321,16 @@
     pub value: f64,
     pub to: Unit,
     pub meta_data: String,
 }
 
 impl<'de> Deserialize<'de> for EPD {
     fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
-    where
-        D: Deserializer<'de>,
+        where
+            D: Deserializer<'de>,
     {
         let helper = ILCD::deserialize(deserializer)?;
         let subtype = helper
             .modelling_and_validation
             .lci_method_and_allocation
             .other
             .anies
@@ -369,23 +369,15 @@
             mer,
             eee,
             eet,
         ) = collect_from_exchanges(&helper.exchanges.exchange);
 
         Ok(EPD {
             id: helper.process_information.data_set_information.uuid,
-            name: helper
-                .process_information
-                .data_set_information
-                .name
-                .base_name
-                .first()
-                .unwrap()
-                .value
-                .to_string(),
+            name: get_name(helper.process_information.data_set_information.name),
             version: helper.version,
             format_version,
             declared_unit,
             reference_service_life: None,
             conversions: Some(conversions),
             standard,
             comment: None,
@@ -449,15 +441,15 @@
 fn get_ilcd_standard(helper: &ILCD) -> Standard {
     for compliance in &helper
         .modelling_and_validation
         .compliance_declarations
         .compliance
     {
         for description in &compliance.reference_to_compliance_system.short_description {
-            match Standard::from(&description.value) {
+            match Standard::from(&description.value.clone().unwrap()) {
                 Standard::UNKNOWN => continue,
                 standard => return standard,
             }
         }
     }
 
     return Standard::UNKNOWN;
@@ -496,15 +488,15 @@
 fn get_ilcd_declared_unit(exchange: &Exchange) -> Unit {
     for flow_property in exchange.flow_properties.as_ref().unwrap() {
         match (
             flow_property.reference_flow_property,
             &flow_property.reference_unit,
         ) {
             (Some(reference_flow), Some(reference_unit)) if reference_flow == true => {
-                return Unit::from(reference_unit)
+                return Unit::from(reference_unit);
             }
             _ => continue,
         }
     }
 
     Unit::UNKNOWN
 }
@@ -531,23 +523,23 @@
     for lcia_result in lcia_result {
         for description in &lcia_result
             .reference_to_lcia_method_dataset
             .short_description
         {
             let impact_value = Some(ImpactCategory::from(&lcia_result.other.anies));
             match &description.value {
-                value if value.contains("(GWP)") || value.contains("(GWP-total)") => {
+                Some(value) if value.contains("(GWP)") || value.contains("(GWP-total)") => {
                     gwp = impact_value
                 }
-                value if value.contains("(ODP)") => odp = impact_value,
-                value if value.contains("(AP)") => ap = impact_value,
-                value if value.contains("(EP)") => ep = impact_value,
-                value if value.contains("(POCP)") => pocp = impact_value,
-                value if value.contains("(ADPE)") => adpe = impact_value,
-                value if value.contains("(ADPF)") => adpf = impact_value,
+                Some(value) if value.contains("(ODP)") => odp = impact_value,
+                Some(value) if value.contains("(AP)") => ap = impact_value,
+                Some(value) if value.contains("(EP)") => ep = impact_value,
+                Some(value) if value.contains("(POCP)") => pocp = impact_value,
+                Some(value) if value.contains("(ADPE)") => adpe = impact_value,
+                Some(value) if value.contains("(ADPF)") => adpf = impact_value,
                 _ => continue,
             }
         }
     }
 
     (gwp, odp, ap, ep, pocp, adpe, adpf)
 }
@@ -606,32 +598,32 @@
             _ => {
                 for description in &exchange.reference_to_flow_data_set.short_description {
                     let impact_value = match &exchange.other {
                         Some(_anies) => Some(ImpactCategory::from(&_anies.anies)),
                         _ => continue,
                     };
                     match &description.value {
-                        _description if _description == "Use of renewable primary energy (PERE)" => pere = impact_value,
-                        _description if _description == "Use of renewable primary energy resources used as raw materials (PERM)" => perm = impact_value,
-                        _description if _description == "Total use of renewable primary energy resources (PERT)" => pert = impact_value,
-                        _description if _description == "Use of non renewable primary energy (PENRE)" => penre = impact_value,
-                        _description if _description == "Use of non renewable primary energy resources used as raw materials (PENRM)" => penrm = impact_value,
-                        _description if _description == "Total use of non renewable primary energy resource (PENRT)" => penrt = impact_value,
-                        _description if _description == "Use of secondary material (SM)" => sm = impact_value,
-                        _description if _description == "Use of renewable secondary fuels (RSF)" => rsf = impact_value,
-                        _description if _description == "Use of non renewable secondary fuels (NRSF)" => nrsf = impact_value,
-                        _description if _description == "Use of net fresh water (FW)" => fw = impact_value,
-                        _description if _description == "Hazardous waste disposed (HWD)" => hwd = impact_value,
-                        _description if _description == "Non hazardous waste dispose (NHWD)" => nhwd = impact_value,
-                        _description if _description == "Radioactive waste disposed (RWD)" => rwd = impact_value,
-                        _description if _description == "Components for re-use (CRU)" => cru = impact_value,
-                        _description if _description == "Materials for recycling (MFR)" => mfr = impact_value,
-                        _description if _description == "Materials for energy recovery (MER)" => mer = impact_value,
-                        _description if _description == "Exported electrical energy (EEE)" => eee = impact_value,
-                        _description if _description == "Exported thermal energy (EET)" => eet = impact_value,
+                        Some(_description) if _description == "Use of renewable primary energy (PERE)" => pere = impact_value,
+                        Some(_description) if _description == "Use of renewable primary energy resources used as raw materials (PERM)" => perm = impact_value,
+                        Some(_description) if _description == "Total use of renewable primary energy resources (PERT)" => pert = impact_value,
+                        Some(_description) if _description == "Use of non renewable primary energy (PENRE)" => penre = impact_value,
+                        Some(_description) if _description == "Use of non renewable primary energy resources used as raw materials (PENRM)" => penrm = impact_value,
+                        Some(_description) if _description == "Total use of non renewable primary energy resource (PENRT)" => penrt = impact_value,
+                        Some(_description) if _description == "Use of secondary material (SM)" => sm = impact_value,
+                        Some(_description) if _description == "Use of renewable secondary fuels (RSF)" => rsf = impact_value,
+                        Some(_description) if _description == "Use of non renewable secondary fuels (NRSF)" => nrsf = impact_value,
+                        Some(_description) if _description == "Use of net fresh water (FW)" => fw = impact_value,
+                        Some(_description) if _description == "Hazardous waste disposed (HWD)" => hwd = impact_value,
+                        Some(_description) if _description == "Non hazardous waste dispose (NHWD)" => nhwd = impact_value,
+                        Some(_description) if _description == "Radioactive waste disposed (RWD)" => rwd = impact_value,
+                        Some(_description) if _description == "Components for re-use (CRU)" => cru = impact_value,
+                        Some(_description) if _description == "Materials for recycling (MFR)" => mfr = impact_value,
+                        Some(_description) if _description == "Materials for energy recovery (MER)" => mer = impact_value,
+                        Some(_description) if _description == "Exported electrical energy (EEE)" => eee = impact_value,
+                        Some(_description) if _description == "Exported thermal energy (EET)" => eet = impact_value,
                         _ => continue
                     }
                 }
             }
         };
     }
 
@@ -654,7 +646,14 @@
         cru,
         mfr,
         mer,
         eee,
         eet,
     )
 }
+
+fn get_name(base_name: DataSetName) -> String {
+    match base_name.base_name.first() {
+        Some(name) if name.value.is_some() => name.value.clone().unwrap(),
+        _ => "".to_string()
+    }
+}
```

### Comparing `epdx-1.2.0/src/ilcd.rs` & `epdx-1.2.1/src/ilcd.rs`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,14 @@
 }
 
 #[derive(Debug, Deserialize)]
 #[serde(rename_all = "camelCase")]
 pub struct ValueObject {
     _type: String,
     ref_object_id: String,
-    uri: String,
 }
 
 #[derive(Deserialize, Debug)]
 pub enum ModuleValue {
     Value(String),
     Name(ModuleMap),
 }
@@ -221,10 +220,10 @@
 #[serde(rename_all = "camelCase")]
 pub struct DataSetName {
     pub base_name: Vec<ValueLang>,
 }
 
 #[derive(Deserialize, Debug)]
 pub struct ValueLang {
-    pub value: String,
+    pub value: Option<String>,
     pub lang: String,
 }
```

### Comparing `epdx-1.2.0/src/javascript.rs` & `epdx-1.2.1/src/javascript.rs`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/src/lcabyg.rs` & `epdx-1.2.1/src/lcabyg.rs`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/src/python.rs` & `epdx-1.2.1/src/python.rs`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/src/utils.rs` & `epdx-1.2.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/00c28f1f-1d49-4c81-9208-138922a1dd6c.json` & `epdx-1.2.1/tests/datafixtures/ilcd/00c28f1f-1d49-4c81-9208-138922a1dd6c.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json` & `epdx-1.2.1/tests/datafixtures/ilcd/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0b488798-140f-4efa-96e2-55aa46ed129a.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0b488798-140f-4efa-96e2-55aa46ed129a.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0b4c397d-c7a1-4ceb-9718-184334f6364e.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0b4c397d-c7a1-4ceb-9718-184334f6364e.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0cb92770-9007-48c6-bc03-466af8894419.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0cb92770-9007-48c6-bc03-466af8894419.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0d1e4a59-4901-4973-a26f-1698f65a780f.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0d1e4a59-4901-4973-a26f-1698f65a780f.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0e85f255-4d11-4973-9daa-c03889948351.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0e85f255-4d11-4973-9daa-c03889948351.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/0e9fd868-9656-489e-be6c-8251b3d43283.json` & `epdx-1.2.1/tests/datafixtures/ilcd/0e9fd868-9656-489e-be6c-8251b3d43283.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json` & `epdx-1.2.1/tests/datafixtures/ilcd/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/f63ac879-fa7d-4f91-813e-e816cbdf1927.json` & `epdx-1.2.1/tests/datafixtures/ilcd/f63ac879-fa7d-4f91-813e-e816cbdf1927.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/ilcd/f63ac879_test.json` & `epdx-1.2.1/tests/datafixtures/ilcd/f63ac879_test.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/datafixtures/lcabyg/5aa09d72.json` & `epdx-1.2.1/tests/datafixtures/lcabyg/5aa09d72.json`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/tests/test_parse_ilcd.rs` & `epdx-1.2.1/tests/test_parse_ilcd.rs`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         ilcd_0d1e4a59: "0d1e4a59-4901-4973-a26f-1698f65a780f.json"
         ilcd_0e85f255: "0e85f255-4d11-4973-9daa-c03889948351.json"
         ilcd_0b4c397d: "0b4c397d-c7a1-4ceb-9718-184334f6364e.json"
         ilcd_0e0c4e37: "0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json"
         ilcd_0e9fd868: "0e9fd868-9656-489e-be6c-8251b3d43283.json"
         ilcd_023f3b97: "023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json"
         ilcd_c23b2987: "c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json"
+        ilcd_0aa8b645: "0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json"
+        ilcd_335241f9: "335241f9-db84-486c-9a19-cd5ebb791903.json"
     }
 
     #[test]
     fn test_parse_ilcd_short() -> Result<(), String> {
         let root_dir = Path::new(env!("CARGO_MANIFEST_DIR"));
         let file_path = root_dir.join("tests/datafixtures/ilcd/f63ac879_test.json");
         let contents =
```

### Comparing `epdx-1.2.0/tests/test_parse_lcabyg.rs` & `epdx-1.2.1/tests/test_parse_lcabyg.rs`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/pyproject.toml` & `epdx-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epdx-1.2.0/PKG-INFO` & `epdx-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: epdx
-Version: 1.2.0
+Version: 1.2.1
 Requires-Dist: pydantic >=2.0.0
 Requires-Dist: mkdocs-material >=8.1.4, <9.0.0 ; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1, <2.0.0 ; extra == 'doc'
 Requires-Dist: datamodel-code-generator ; extra == 'codegen'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-datafixtures ; extra == 'tests'
 Provides-Extra: doc
@@ -95,23 +95,23 @@
 cargo test --package epdx --target x86_64-unknown-linux-gnu
 ```
 
 ## Run Python Tests
 
 ```bash
 maturin develop --extras tests --target x86_64-unknown-linux-gnu
-source .venv/bin/active .
+source .venv/bin/activate .
 cd packages/python
 pytest tests/
 ```
 
 ## Build Documentation
 
 ```bash
-maturin develop --extras doc,code-gen --target x86_64-unknown-linux-gnu
+maturin develop --extras doc,codegen --target x86_64-unknown-linux-gnu
 mkdocs develop
 ```
 
 ## Build JS Package
 
 ```bash
 wasm-pack build --features jsbindings
```

