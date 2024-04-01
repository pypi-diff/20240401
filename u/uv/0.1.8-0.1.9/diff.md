# Comparing `tmp/uv-0.1.8.tar.gz` & `tmp/uv-0.1.9.tar.gz`

## Comparing `uv-0.1.8.tar` & `uv-0.1.9.tar`

### file list

```diff
@@ -1,279 +1,280 @@
--rw-r--r--   0     1001      127      995 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/Cargo.toml
--rw-r--r--   0     1001      127      195 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/src/by_timestamp.rs
--rw-r--r--   0     1001      127     1376 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/src/cli.rs
--rw-r--r--   0     1001      127    27484 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/src/lib.rs
--rw-r--r--   0     1001      127     3967 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/src/removal.rs
--rw-r--r--   0     1001      127     1663 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/src/timestamp.rs
--rw-r--r--   0     1001      127     2973 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-cache/src/wheel.rs
--rw-r--r--   0     1001      127      456 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-warnings/Cargo.toml
--rw-r--r--   0     1001      127     1701 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-warnings/src/lib.rs
--rw-r--r--   0     1001      127     1751 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/Cargo.toml
--rw-r--r--   0     1001      127      112 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/README.md
--rw-r--r--   0     1001      127     5287 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/auth.rs
--rw-r--r--   0     1001      127    29382 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/cached_client.rs
--rw-r--r--   0     1001      127     7003 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/error.rs
--rw-r--r--   0     1001      127    13974 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/flat_index.rs
--rw-r--r--   0     1001      127    32917 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/html.rs
--rw-r--r--   0     1001      127    29342 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/httpcache/control.rs
--rw-r--r--   0     1001      127    60040 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/httpcache/mod.rs
--rw-r--r--   0     1001      127      537 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/lib.rs
--rw-r--r--   0     1001      127     1245 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/middleware.rs
--rw-r--r--   0     1001      127    33263 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/registry_client.rs
--rw-r--r--   0     1001      127     4495 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/remote_metadata.rs
--rw-r--r--   0     1001      127    12175 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/src/rkyvutil.rs
--rw-r--r--   0     1001      127     1076 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-client/tests/remote_metadata.rs
--rw-r--r--   0     1001      127     1020 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/Cargo.toml
--rw-r--r--   0     1001      127     2831 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/src/base_url.rs
--rw-r--r--   0     1001      127     4361 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/src/direct_url.rs
--rw-r--r--   0     1001      127    13755 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/src/lenient_requirement.rs
--rw-r--r--   0     1001      127      208 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/src/lib.rs
--rw-r--r--   0     1001      127     6749 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/src/metadata.rs
--rw-r--r--   0     1001      127     4814 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pypi-types/src/simple_json.rs
--rw-r--r--   0     1001      127     1948 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/Cargo.toml
--rw-r--r--   0     1001      127      515 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/Readme.md
--rw-r--r--   0     1001      127     3753 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/install_location.rs
--rw-r--r--   0     1001      127     7743 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/lib.rs
--rw-r--r--   0     1001      127    18729 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/linker.rs
--rw-r--r--   0     1001      127     2166 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/main.rs
--rw-r--r--   0     1001      127     1288 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/pip_compileall.py
--rw-r--r--   0     1001      127     2827 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/python_bindings.rs
--rw-r--r--   0     1001      127      446 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/record.rs
--rw-r--r--   0     1001      127     4118 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/script.rs
--rw-r--r--   0     1001      127     5436 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/uninstall.rs
--rw-r--r--   0     1001      127    49021 2024-02-22 19:12:40.000000 uv-0.1.8/crates/install-wheel-rs/src/wheel.rs
--rw-r--r--   0     1001      127     1256 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/Cargo.toml
--rw-r--r--   0     1001      127     1048 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/any.rs
--rw-r--r--   0     1001      127     5648 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/cached.rs
--rw-r--r--   0     1001      127     8047 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/direct_url.rs
--rw-r--r--   0     1001      127      983 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/editable.rs
--rw-r--r--   0     1001      127      551 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/error.rs
--rw-r--r--   0     1001      127     3104 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/file.rs
--rw-r--r--   0     1001      127     2054 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/id.rs
--rw-r--r--   0     1001      127     9984 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/index_url.rs
--rw-r--r--   0     1001      127     5890 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/installed.rs
--rw-r--r--   0     1001      127    27984 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/lib.rs
--rw-r--r--   0     1001      127    12193 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/prioritized_distribution.rs
--rw-r--r--   0     1001      127     4342 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/resolution.rs
--rw-r--r--   0     1001      127     6640 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-types/src/traits.rs
--rw-r--r--   0     1001      127      667 2024-02-22 19:12:40.000000 uv-0.1.8/crates/platform-host/Cargo.toml
--rw-r--r--   0     1001      127     6522 2024-02-22 19:12:40.000000 uv-0.1.8/crates/platform-host/src/lib.rs
--rw-r--r--   0     1001      127    11062 2024-02-22 19:12:40.000000 uv-0.1.8/crates/platform-host/src/linux.rs
--rw-r--r--   0     1001      127     1311 2024-02-22 19:12:40.000000 uv-0.1.8/crates/platform-host/src/mac_os.rs
--rw-r--r--   0     1001      127     1545 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/Cargo.toml
--rw-r--r--   0     1001      127    19122 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/distribution_database.rs
--rw-r--r--   0     1001      127     4096 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/download.rs
--rw-r--r--   0     1001      127     2304 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/error.rs
--rw-r--r--   0     1001      127     5195 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/index/built_wheel_index.rs
--rw-r--r--   0     1001      127     1393 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/index/cached_wheel.rs
--rw-r--r--   0     1001      127      162 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/index/mod.rs
--rw-r--r--   0     1001      127     5568 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/index/registry_wheel_index.rs
--rw-r--r--   0     1001      127      387 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/lib.rs
--rw-r--r--   0     1001      127      606 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/locks.rs
--rw-r--r--   0     1001      127     1206 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/reporter.rs
--rw-r--r--   0     1001      127     1541 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/source/built_wheel_metadata.rs
--rw-r--r--   0     1001      127      473 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/source/manifest.rs
--rw-r--r--   0     1001      127    39757 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/source/mod.rs
--rw-r--r--   0     1001      127      859 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-distribution/src/unzip.rs
--rw-r--r--   0     1001      127     1466 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/Cargo.toml
--rw-r--r--   0     1001      127     9791 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/downloader.rs
--rw-r--r--   0     1001      127     1827 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/editable.rs
--rw-r--r--   0     1001      127     2600 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/installer.rs
--rw-r--r--   0     1001      127      464 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/lib.rs
--rw-r--r--   0     1001      127    22276 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/plan.rs
--rw-r--r--   0     1001      127    15927 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/site_packages.rs
--rw-r--r--   0     1001      127      402 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-installer/src/uninstall.rs
--rw-r--r--   0     1001      127      439 2024-02-22 19:12:40.000000 uv-0.1.8/crates/platform-tags/Cargo.toml
--rw-r--r--   0     1001      127    18693 2024-02-22 19:12:40.000000 uv-0.1.8/crates/platform-tags/src/lib.rs
--rw-r--r--   0     1001      127     1224 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-dispatch/Cargo.toml
--rw-r--r--   0     1001      127     9549 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-dispatch/src/lib.rs
--rw-r--r--   0     1001      127      751 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/Cargo.toml
--rw-r--r--   0     1001      127     2339 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/src/lib.rs
--rw-r--r--   0     1001      127      420 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
--rw-r--r--   0     1001      127      539 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
--rw-r--r--   0     1001      127      398 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
--rw-r--r--   0     1001      127     7557 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/src/source_dist.rs
--rw-r--r--   0     1001      127    11224 2024-02-22 19:12:40.000000 uv-0.1.8/crates/distribution-filename/src/wheel.rs
--rw-r--r--   0     1001      127      626 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-fs/Cargo.toml
--rw-r--r--   0     1001      127     7970 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-fs/src/lib.rs
--rw-r--r--   0     1001      127     2629 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-fs/src/path.rs
--rw-r--r--   0     1001      127     2453 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/Cargo.toml
--rw-r--r--   0     1001      127    12186 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/candidate_selector.rs
--rw-r--r--   0     1001      127     1000 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/constraints.rs
--rw-r--r--   0     1001      127      610 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/dependency_mode.rs
--rw-r--r--   0     1001      127     1149 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/editables.rs
--rw-r--r--   0     1001      127    10250 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/error.rs
--rw-r--r--   0     1001      127     9510 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/finder.rs
--rw-r--r--   0     1001      127      948 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/manifest.rs
--rw-r--r--   0     1001      127     1815 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/options.rs
--rw-r--r--   0     1001      127     1475 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/overrides.rs
--rw-r--r--   0     1001      127     1062 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pins.rs
--rw-r--r--   0     1001      127     3855 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/prerelease_mode.rs
--rw-r--r--   0     1001      127     6979 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/dependencies.rs
--rw-r--r--   0     1001      127     1063 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/distribution.rs
--rw-r--r--   0     1001      127      498 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/mod.rs
--rw-r--r--   0     1001      127     4763 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/package.rs
--rw-r--r--   0     1001      127     1007 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/priority.rs
--rw-r--r--   0     1001      127    29263 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/report.rs
--rw-r--r--   0     1001      127     4189 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/pubgrub/specifier.rs
--rw-r--r--   0     1001      127     2780 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/python_requirement.rs
--rw-r--r--   0     1001      127    20084 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolution.rs
--rw-r--r--   0     1001      127     1613 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolution_mode.rs
--rw-r--r--   0     1001      127      881 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolver/index.rs
--rw-r--r--   0     1001      127    48590 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolver/mod.rs
--rw-r--r--   0     1001      127     7127 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolver/provider.rs
--rw-r--r--   0     1001      127     1629 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolver/reporter.rs
--rw-r--r--   0     1001      127     3601 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/resolver/urls.rs
--rw-r--r--   0     1001      127    17789 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/version_map.rs
--rw-r--r--   0     1001      127     1656 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/src/yanks.rs
--rw-r--r--   0     1001      127    20177 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-resolver/tests/resolver.rs
--rw-r--r--   0     1001      127      306 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-normalize/Cargo.toml
--rw-r--r--   0     1001      127     1652 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-normalize/src/extra_name.rs
--rw-r--r--   0     1001      127     5673 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-normalize/src/lib.rs
--rw-r--r--   0     1001      127     2899 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-normalize/src/package_name.rs
--rw-r--r--   0     1001      127     2220 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/License-BSD
--rw-r--r--   0     1001      127     3039 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/Readme.md
--rw-r--r--   0     1001      127    54264 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/src/lib.rs
--rw-r--r--   0     1001      127    65624 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/src/marker.rs
--rw-r--r--   0     1001      127    12345 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep508-rs/src/verbatim_url.rs
--rw-r--r--   0     1001      127      660 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-traits/Cargo.toml
--rw-r--r--   0     1001      127    12175 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-traits/src/lib.rs
--rw-r--r--   0     1001      127     1178 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/Cargo.toml
--rw-r--r--   0     1001      127      740 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/README.md
--rw-r--r--   0     1001      127      350 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/benchmark.sh
--rw-r--r--   0     1001      127      629 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/compare_in_git.sh
--rw-r--r--   0     1001      127      163 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/imasnake.py
--rw-r--r--   0     1001      127       96 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/oranda.json
--rw-r--r--   0     1001      127     4375 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/_virtualenv.py
--rw-r--r--   0     1001      127     2237 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activate
--rw-r--r--   0     1001      127       20 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/.gitattributes
--rw-r--r--   0     1001      127     3388 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate
--rw-r--r--   0     1001      127     2259 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate.bat
--rw-r--r--   0     1001      127     2655 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate.csh
--rw-r--r--   0     1001      127     4218 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate.fish
--rw-r--r--   0     1001      127     3903 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate.nu
--rw-r--r--   0     1001      127     2813 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate.ps1
--rw-r--r--   0     1001      127     2457 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/activate_this.py
--rw-r--r--   0     1001      127     1728 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/deactivate.bat
--rw-r--r--   0     1001      127     1215 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/activator/pydoc.bat
--rw-r--r--   0     1001      127    10282 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/bare.rs
--rw-r--r--   0     1001      127     1766 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/interpreter.rs
--rw-r--r--   0     1001      127     1777 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/lib.rs
--rw-r--r--   0     1001      127     1879 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/src/main.rs
--rw-r--r--   0     1001      127  1072094 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/static/gourgeist.png
--rw-r--r--   0     1001      127      994 2024-02-22 19:12:40.000000 uv-0.1.8/crates/gourgeist/venv_checker.py
--rw-r--r--   0     1001      127     1041 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/License-BSD
--rw-r--r--   0     1001      127     2947 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/Readme.md
--rw-r--r--   0     1001      127     2105 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/python/Readme.md
--rw-r--r--   0     1001      127     2843 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/src/lib.rs
--rw-r--r--   0     1001      127   122355 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/src/version.rs
--rw-r--r--   0     1001      127    57538 2024-02-22 19:12:40.000000 uv-0.1.8/crates/pep440-rs/src/version_specifier.rs
--rw-r--r--   0     1001      127     1271 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-build/Cargo.toml
--rw-r--r--   0     1001      127       17 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-build/.gitignore
--rw-r--r--   0     1001      127    35020 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-build/src/lib.rs
--rw-r--r--   0     1001      127     1189 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/Cargo.toml
--rw-r--r--   0     1001      127     1779 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/cfg.rs
--rw-r--r--   0     1001      127     3168 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/get_interpreter_info.py
--rw-r--r--   0     1001      127    19106 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/interpreter.rs
--rw-r--r--   0     1001      127     2444 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/lib.rs
--rw-r--r--   0     1001      127     2158 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/python_platform.rs
--rw-r--r--   0     1001      127    19212 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/python_query.rs
--rw-r--r--   0     1001      127     3476 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/python_version.rs
--rw-r--r--   0     1001      127     4792 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-interpreter/src/virtual_env.rs
--rw-r--r--   0     1001      127      507 2024-02-22 19:12:40.000000 uv-0.1.8/crates/cache-key/Cargo.toml
--rw-r--r--   0     1001      127     8335 2024-02-22 19:12:40.000000 uv-0.1.8/crates/cache-key/src/cache_key.rs
--rw-r--r--   0     1001      127     9335 2024-02-22 19:12:40.000000 uv-0.1.8/crates/cache-key/src/canonical_url.rs
--rw-r--r--   0     1001      127      620 2024-02-22 19:12:40.000000 uv-0.1.8/crates/cache-key/src/digest.rs
--rw-r--r--   0     1001      127      191 2024-02-22 19:12:40.000000 uv-0.1.8/crates/cache-key/src/lib.rs
--rw-r--r--   0     1001      127     1986 2024-02-22 19:12:40.000000 uv-0.1.8/crates/cache-key/src/stable_hash.rs
--rw-r--r--   0     1001      127      380 2024-02-22 19:12:40.000000 uv-0.1.8/crates/once-map/Cargo.toml
--rw-r--r--   0     1001      127     2863 2024-02-22 19:12:40.000000 uv-0.1.8/crates/once-map/src/lib.rs
--rw-r--r--   0     1001      127      983 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/Cargo.toml
--rw-r--r--   0     1001      127    60543 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/git.rs
--rw-r--r--   0     1001      127    37540 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/known_hosts.rs
--rw-r--r--   0     1001      127     3707 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/lib.rs
--rw-r--r--   0     1001      127      902 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/sha.rs
--rw-r--r--   0     1001      127     4946 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/source.rs
--rw-r--r--   0     1001      127     1362 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/util/errors.rs
--rw-r--r--   0     1001      127      733 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/util/mod.rs
--rw-r--r--   0     1001      127     7297 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-git/src/util/retry.rs
--rw-r--r--   0     1001      127      818 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/Cargo.toml
--rw-r--r--   0     1001      127      661 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/error.rs
--rw-r--r--   0     1001      127       98 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/lib.rs
--rw-r--r--   0     1001      127     6885 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/stream.rs
--rw-r--r--   0     1001      127     3562 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/sync.rs
--rw-r--r--   0     1001      127     1489 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/tar.rs
--rw-r--r--   0     1001      127     5650 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
--rw-r--r--   0     1001      127      112 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv-extract/src/vendor/mod.rs
--rw-r--r--   0     1001      127     1160 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/Cargo.toml
--rw-r--r--   0     1001      127    47300 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/lib.rs
--rw-r--r--   0     1001      127     4626 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
--rw-r--r--   0     1001      127     2092 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
--rw-r--r--   0     1001      127     1703 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
--rw-r--r--   0     1001      127     1960 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-editable.txt.snap
--rw-r--r--   0     1001      127      240 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
--rw-r--r--   0     1001      127     3068 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1298 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
--rw-r--r--   0     1001      127      569 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
--rw-r--r--   0     1001      127    11076 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     1703 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
--rw-r--r--   0     1001      127     1960 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
--rw-r--r--   0     1001      127     4626 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
--rw-r--r--   0     1001      127     2092 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
--rw-r--r--   0     1001      127     1703 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
--rw-r--r--   0     1001      127      240 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
--rw-r--r--   0     1001      127     3068 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1298 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
--rw-r--r--   0     1001      127      569 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
--rw-r--r--   0     1001      127    11076 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     1703 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
--rw-r--r--   0     1001      127     1960 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
--rw-r--r--   0     1001      127       90 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/basic.txt
--rw-r--r--   0     1001      127       45 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
--rw-r--r--   0     1001      127       27 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
--rw-r--r--   0     1001      127      183 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/editable.txt
--rw-r--r--   0     1001      127        0 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/empty.txt
--rw-r--r--   0     1001      127      101 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
--rw-r--r--   0     1001      127       43 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/include-a.txt
--rw-r--r--   0     1001      127        5 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/include-b.txt
--rw-r--r--   0     1001      127     1183 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
--rw-r--r--   0     1001      127       66 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/small.txt
--rw-r--r--   0     1001      127      183 2024-02-22 19:12:40.000000 uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
--rw-r--r--   0        0        0     3394 1970-01-01 00:00:00.000000 uv-0.1.8/crates/uv/Cargo.toml
--rw-r--r--   0     1001      127     4359 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/cache_clean.rs
--rw-r--r--   0     1001      127      219 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/cache_dir.rs
--rw-r--r--   0     1001      127     1903 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/mod.rs
--rw-r--r--   0     1001      127    15204 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/pip_compile.rs
--rw-r--r--   0     1001      127     1471 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/pip_freeze.rs
--rw-r--r--   0     1001      127    21983 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/pip_install.rs
--rw-r--r--   0     1001      127    15209 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/pip_sync.rs
--rw-r--r--   0     1001      127     5027 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/pip_uninstall.rs
--rw-r--r--   0     1001      127     9445 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/reporters.rs
--rw-r--r--   0     1001      127     6619 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/commands/venv.rs
--rw-r--r--   0     1001      127    11209 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/compat/mod.rs
--rw-r--r--   0     1001      127     1859 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/confirm.rs
--rw-r--r--   0     1001      127     3879 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/logging.rs
--rw-r--r--   0     1001      127    40860 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/main.rs
--rw-r--r--   0     1001      127     1223 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/printer.rs
--rw-r--r--   0     1001      127    14759 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/src/requirements.rs
--rw-r--r--   0     1001      127    14363 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/common/mod.rs
--rw-r--r--   0     1001      127   139697 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/pip_compile.rs
--rw-r--r--   0     1001      127    19304 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/pip_compile_scenarios.rs
--rw-r--r--   0     1001      127    46725 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/pip_install.rs
--rw-r--r--   0     1001      127   109909 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/pip_install_scenarios.rs
--rw-r--r--   0     1001      127    83331 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/pip_sync.rs
--rw-r--r--   0     1001      127    14422 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/pip_uninstall.rs
--rw-r--r--   0     1001      127    20227 2024-02-22 19:12:40.000000 uv-0.1.8/crates/uv/tests/venv.rs
--rw-r--r--   0     1001      127   119664 2024-02-22 19:12:40.000000 uv-0.1.8/Cargo.lock
--rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 uv-0.1.8/Cargo.toml
--rw-r--r--   0     1001      127     1362 2024-02-22 19:12:40.000000 uv-0.1.8/pyproject.toml
--rw-r--r--   0     1001      127      927 2024-02-22 19:12:40.000000 uv-0.1.8/python/uv/__main__.py
--rw-r--r--   0     1001      127      806 2024-02-22 19:12:40.000000 uv-0.1.8/python/uv/__init__.py
--rw-r--r--   0     1001      127        0 2024-02-22 19:12:40.000000 uv-0.1.8/python/uv/py.typed
--rw-r--r--   0     1001      127    17069 2024-02-22 19:12:40.000000 uv-0.1.8/README.md
--rw-r--r--   0     1001      127       29 2024-02-22 19:12:40.000000 uv-0.1.8/rust-toolchain.toml
--rw-r--r--   0        0        0    18436 1970-01-01 00:00:00.000000 uv-0.1.8/PKG-INFO
+-rw-r--r--   0     1001      127     1178 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/Cargo.toml
+-rw-r--r--   0     1001      127      740 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/README.md
+-rw-r--r--   0     1001      127      350 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/benchmark.sh
+-rw-r--r--   0     1001      127      629 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/compare_in_git.sh
+-rw-r--r--   0     1001      127      163 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/imasnake.py
+-rw-r--r--   0     1001      127       96 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/oranda.json
+-rw-r--r--   0     1001      127     4375 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/_virtualenv.py
+-rw-r--r--   0     1001      127     2237 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activate
+-rw-r--r--   0     1001      127       20 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/.gitattributes
+-rw-r--r--   0     1001      127     3388 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate
+-rw-r--r--   0     1001      127     2259 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate.bat
+-rw-r--r--   0     1001      127     2655 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate.csh
+-rw-r--r--   0     1001      127     4218 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate.fish
+-rw-r--r--   0     1001      127     3903 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate.nu
+-rw-r--r--   0     1001      127     2813 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate.ps1
+-rw-r--r--   0     1001      127     2457 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/activate_this.py
+-rw-r--r--   0     1001      127     1728 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/deactivate.bat
+-rw-r--r--   0     1001      127     1215 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/activator/pydoc.bat
+-rw-r--r--   0     1001      127    10863 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/bare.rs
+-rw-r--r--   0     1001      127     1766 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/interpreter.rs
+-rw-r--r--   0     1001      127     1911 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/lib.rs
+-rw-r--r--   0     1001      127     1891 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/src/main.rs
+-rw-r--r--   0     1001      127  1072094 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/static/gourgeist.png
+-rw-r--r--   0     1001      127      994 2024-02-23 02:30:21.000000 uv-0.1.9/crates/gourgeist/venv_checker.py
+-rw-r--r--   0     1001      127     1189 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/Cargo.toml
+-rw-r--r--   0     1001      127     1779 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/cfg.rs
+-rw-r--r--   0     1001      127     3168 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/get_interpreter_info.py
+-rw-r--r--   0     1001      127    19106 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/interpreter.rs
+-rw-r--r--   0     1001      127     2444 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/lib.rs
+-rw-r--r--   0     1001      127     2158 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/python_platform.rs
+-rw-r--r--   0     1001      127    19212 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/python_query.rs
+-rw-r--r--   0     1001      127     3476 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/python_version.rs
+-rw-r--r--   0     1001      127     4792 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-interpreter/src/virtual_env.rs
+-rw-r--r--   0     1001      127     2453 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/Cargo.toml
+-rw-r--r--   0     1001      127    12186 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/candidate_selector.rs
+-rw-r--r--   0     1001      127     1000 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/constraints.rs
+-rw-r--r--   0     1001      127      610 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/dependency_mode.rs
+-rw-r--r--   0     1001      127     1149 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/editables.rs
+-rw-r--r--   0     1001      127    10250 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/error.rs
+-rw-r--r--   0     1001      127     9510 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/finder.rs
+-rw-r--r--   0     1001      127      948 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/manifest.rs
+-rw-r--r--   0     1001      127     1815 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/options.rs
+-rw-r--r--   0     1001      127     1475 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/overrides.rs
+-rw-r--r--   0     1001      127     1062 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pins.rs
+-rw-r--r--   0     1001      127     3855 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/prerelease_mode.rs
+-rw-r--r--   0     1001      127     6979 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/dependencies.rs
+-rw-r--r--   0     1001      127     1063 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/distribution.rs
+-rw-r--r--   0     1001      127      498 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/mod.rs
+-rw-r--r--   0     1001      127     4763 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/package.rs
+-rw-r--r--   0     1001      127     1007 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/priority.rs
+-rw-r--r--   0     1001      127    29263 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/report.rs
+-rw-r--r--   0     1001      127     4189 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/pubgrub/specifier.rs
+-rw-r--r--   0     1001      127     2780 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/python_requirement.rs
+-rw-r--r--   0     1001      127    20084 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolution.rs
+-rw-r--r--   0     1001      127     1613 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolution_mode.rs
+-rw-r--r--   0     1001      127      881 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolver/index.rs
+-rw-r--r--   0     1001      127    48590 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolver/mod.rs
+-rw-r--r--   0     1001      127     7127 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolver/provider.rs
+-rw-r--r--   0     1001      127     1629 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolver/reporter.rs
+-rw-r--r--   0     1001      127     3601 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/resolver/urls.rs
+-rw-r--r--   0     1001      127    17789 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/version_map.rs
+-rw-r--r--   0     1001      127     1656 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/src/yanks.rs
+-rw-r--r--   0     1001      127    20177 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-resolver/tests/resolver.rs
+-rw-r--r--   0     1001      127     1041 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/License-BSD
+-rw-r--r--   0     1001      127     2947 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/Readme.md
+-rw-r--r--   0     1001      127     2105 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/python/Readme.md
+-rw-r--r--   0     1001      127     2843 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/src/lib.rs
+-rw-r--r--   0     1001      127   123697 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/src/version.rs
+-rw-r--r--   0     1001      127    57538 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep440-rs/src/version_specifier.rs
+-rw-r--r--   0     1001      127     2220 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/License-BSD
+-rw-r--r--   0     1001      127     3039 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/Readme.md
+-rw-r--r--   0     1001      127    54264 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/src/lib.rs
+-rw-r--r--   0     1001      127    65624 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/src/marker.rs
+-rw-r--r--   0     1001      127    12345 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pep508-rs/src/verbatim_url.rs
+-rw-r--r--   0     1001      127      507 2024-02-23 02:30:21.000000 uv-0.1.9/crates/cache-key/Cargo.toml
+-rw-r--r--   0     1001      127     8335 2024-02-23 02:30:21.000000 uv-0.1.9/crates/cache-key/src/cache_key.rs
+-rw-r--r--   0     1001      127     9335 2024-02-23 02:30:21.000000 uv-0.1.9/crates/cache-key/src/canonical_url.rs
+-rw-r--r--   0     1001      127      620 2024-02-23 02:30:21.000000 uv-0.1.9/crates/cache-key/src/digest.rs
+-rw-r--r--   0     1001      127      191 2024-02-23 02:30:21.000000 uv-0.1.9/crates/cache-key/src/lib.rs
+-rw-r--r--   0     1001      127     1986 2024-02-23 02:30:21.000000 uv-0.1.9/crates/cache-key/src/stable_hash.rs
+-rw-r--r--   0     1001      127      136 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-auth/Cargo.toml
+-rw-r--r--   0     1001      127     5870 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-auth/src/lib.rs
+-rw-r--r--   0     1001      127     1290 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/Cargo.toml
+-rw-r--r--   0     1001      127     1048 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/any.rs
+-rw-r--r--   0     1001      127     5648 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/cached.rs
+-rw-r--r--   0     1001      127     8047 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/direct_url.rs
+-rw-r--r--   0     1001      127      983 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/editable.rs
+-rw-r--r--   0     1001      127      551 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/error.rs
+-rw-r--r--   0     1001      127     3398 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/file.rs
+-rw-r--r--   0     1001      127     2054 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/id.rs
+-rw-r--r--   0     1001      127     9984 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/index_url.rs
+-rw-r--r--   0     1001      127     5890 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/installed.rs
+-rw-r--r--   0     1001      127    27984 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/lib.rs
+-rw-r--r--   0     1001      127    12193 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/prioritized_distribution.rs
+-rw-r--r--   0     1001      127     4342 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/resolution.rs
+-rw-r--r--   0     1001      127     6640 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-types/src/traits.rs
+-rw-r--r--   0     1001      127     1466 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/Cargo.toml
+-rw-r--r--   0     1001      127     9791 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/downloader.rs
+-rw-r--r--   0     1001      127     1827 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/editable.rs
+-rw-r--r--   0     1001      127     2600 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/installer.rs
+-rw-r--r--   0     1001      127      464 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/lib.rs
+-rw-r--r--   0     1001      127    22276 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/plan.rs
+-rw-r--r--   0     1001      127    15927 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/site_packages.rs
+-rw-r--r--   0     1001      127      402 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-installer/src/uninstall.rs
+-rw-r--r--   0     1001      127      751 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/Cargo.toml
+-rw-r--r--   0     1001      127     2339 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/src/lib.rs
+-rw-r--r--   0     1001      127      420 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
+-rw-r--r--   0     1001      127      539 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
+-rw-r--r--   0     1001      127      398 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
+-rw-r--r--   0     1001      127     7557 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/src/source_dist.rs
+-rw-r--r--   0     1001      127    11224 2024-02-23 02:30:21.000000 uv-0.1.9/crates/distribution-filename/src/wheel.rs
+-rw-r--r--   0     1001      127      667 2024-02-23 02:30:21.000000 uv-0.1.9/crates/platform-host/Cargo.toml
+-rw-r--r--   0     1001      127     6522 2024-02-23 02:30:21.000000 uv-0.1.9/crates/platform-host/src/lib.rs
+-rw-r--r--   0     1001      127    11062 2024-02-23 02:30:21.000000 uv-0.1.9/crates/platform-host/src/linux.rs
+-rw-r--r--   0     1001      127     1311 2024-02-23 02:30:21.000000 uv-0.1.9/crates/platform-host/src/mac_os.rs
+-rw-r--r--   0     1001      127      995 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/Cargo.toml
+-rw-r--r--   0     1001      127      195 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/src/by_timestamp.rs
+-rw-r--r--   0     1001      127     1376 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/src/cli.rs
+-rw-r--r--   0     1001      127    27484 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/src/lib.rs
+-rw-r--r--   0     1001      127     3967 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/src/removal.rs
+-rw-r--r--   0     1001      127     1663 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/src/timestamp.rs
+-rw-r--r--   0     1001      127     2973 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-cache/src/wheel.rs
+-rw-r--r--   0     1001      127      439 2024-02-23 02:30:21.000000 uv-0.1.9/crates/platform-tags/Cargo.toml
+-rw-r--r--   0     1001      127    18693 2024-02-23 02:30:21.000000 uv-0.1.9/crates/platform-tags/src/lib.rs
+-rw-r--r--   0     1001      127      456 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-warnings/Cargo.toml
+-rw-r--r--   0     1001      127     1701 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-warnings/src/lib.rs
+-rw-r--r--   0     1001      127     1948 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/Cargo.toml
+-rw-r--r--   0     1001      127      515 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/Readme.md
+-rw-r--r--   0     1001      127     3753 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/install_location.rs
+-rw-r--r--   0     1001      127     7743 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/lib.rs
+-rw-r--r--   0     1001      127    18729 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/linker.rs
+-rw-r--r--   0     1001      127     2166 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/main.rs
+-rw-r--r--   0     1001      127     1288 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/pip_compileall.py
+-rw-r--r--   0     1001      127     2827 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/python_bindings.rs
+-rw-r--r--   0     1001      127      446 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/record.rs
+-rw-r--r--   0     1001      127     4118 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/script.rs
+-rw-r--r--   0     1001      127     5436 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/uninstall.rs
+-rw-r--r--   0     1001      127    49021 2024-02-23 02:30:21.000000 uv-0.1.9/crates/install-wheel-rs/src/wheel.rs
+-rw-r--r--   0     1001      127     1293 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-build/Cargo.toml
+-rw-r--r--   0     1001      127       17 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-build/.gitignore
+-rw-r--r--   0     1001      127    35515 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-build/src/lib.rs
+-rw-r--r--   0     1001      127      626 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-fs/Cargo.toml
+-rw-r--r--   0     1001      127     7970 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-fs/src/lib.rs
+-rw-r--r--   0     1001      127     2629 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-fs/src/path.rs
+-rw-r--r--   0     1001      127      867 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-traits/Cargo.toml
+-rw-r--r--   0     1001      127    17668 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-traits/src/lib.rs
+-rw-r--r--   0     1001      127      818 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/Cargo.toml
+-rw-r--r--   0     1001      127      661 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/error.rs
+-rw-r--r--   0     1001      127       98 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/lib.rs
+-rw-r--r--   0     1001      127     6885 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/stream.rs
+-rw-r--r--   0     1001      127     3562 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/sync.rs
+-rw-r--r--   0     1001      127     1489 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/tar.rs
+-rw-r--r--   0     1001      127     5650 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
+-rw-r--r--   0     1001      127      112 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-extract/src/vendor/mod.rs
+-rw-r--r--   0     1001      127     1020 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/Cargo.toml
+-rw-r--r--   0     1001      127     2947 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/src/base_url.rs
+-rw-r--r--   0     1001      127     4361 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/src/direct_url.rs
+-rw-r--r--   0     1001      127    13755 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/src/lenient_requirement.rs
+-rw-r--r--   0     1001      127      208 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/src/lib.rs
+-rw-r--r--   0     1001      127     6749 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/src/metadata.rs
+-rw-r--r--   0     1001      127     4814 2024-02-23 02:30:21.000000 uv-0.1.9/crates/pypi-types/src/simple_json.rs
+-rw-r--r--   0     1001      127      380 2024-02-23 02:30:21.000000 uv-0.1.9/crates/once-map/Cargo.toml
+-rw-r--r--   0     1001      127     2863 2024-02-23 02:30:21.000000 uv-0.1.9/crates/once-map/src/lib.rs
+-rw-r--r--   0     1001      127     1785 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/Cargo.toml
+-rw-r--r--   0     1001      127      112 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/README.md
+-rw-r--r--   0     1001      127    29382 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/cached_client.rs
+-rw-r--r--   0     1001      127     7003 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/error.rs
+-rw-r--r--   0     1001      127    14031 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/flat_index.rs
+-rw-r--r--   0     1001      127    32917 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/html.rs
+-rw-r--r--   0     1001      127    29342 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/httpcache/control.rs
+-rw-r--r--   0     1001      127    60040 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/httpcache/mod.rs
+-rw-r--r--   0     1001      127      527 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/lib.rs
+-rw-r--r--   0     1001      127     1245 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/middleware.rs
+-rw-r--r--   0     1001      127    33190 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/registry_client.rs
+-rw-r--r--   0     1001      127     4495 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/remote_metadata.rs
+-rw-r--r--   0     1001      127    12175 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/src/rkyvutil.rs
+-rw-r--r--   0     1001      127     1076 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-client/tests/remote_metadata.rs
+-rw-r--r--   0     1001      127     1545 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/Cargo.toml
+-rw-r--r--   0     1001      127    19122 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/distribution_database.rs
+-rw-r--r--   0     1001      127     4096 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/download.rs
+-rw-r--r--   0     1001      127     2304 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/error.rs
+-rw-r--r--   0     1001      127     5195 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/index/built_wheel_index.rs
+-rw-r--r--   0     1001      127     1393 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/index/cached_wheel.rs
+-rw-r--r--   0     1001      127      162 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/index/mod.rs
+-rw-r--r--   0     1001      127     5568 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/index/registry_wheel_index.rs
+-rw-r--r--   0     1001      127      387 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/lib.rs
+-rw-r--r--   0     1001      127      606 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/locks.rs
+-rw-r--r--   0     1001      127     1206 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/reporter.rs
+-rw-r--r--   0     1001      127     1541 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/source/built_wheel_metadata.rs
+-rw-r--r--   0     1001      127      473 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/source/manifest.rs
+-rw-r--r--   0     1001      127    39757 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/source/mod.rs
+-rw-r--r--   0     1001      127      859 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-distribution/src/unzip.rs
+-rw-r--r--   0     1001      127      306 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-normalize/Cargo.toml
+-rw-r--r--   0     1001      127     1652 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-normalize/src/extra_name.rs
+-rw-r--r--   0     1001      127     5673 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-normalize/src/lib.rs
+-rw-r--r--   0     1001      127     2899 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-normalize/src/package_name.rs
+-rw-r--r--   0     1001      127      983 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/Cargo.toml
+-rw-r--r--   0     1001      127    60543 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/git.rs
+-rw-r--r--   0     1001      127    37540 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/known_hosts.rs
+-rw-r--r--   0     1001      127     3707 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/lib.rs
+-rw-r--r--   0     1001      127      902 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/sha.rs
+-rw-r--r--   0     1001      127     4946 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/source.rs
+-rw-r--r--   0     1001      127     1362 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/util/errors.rs
+-rw-r--r--   0     1001      127      733 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/util/mod.rs
+-rw-r--r--   0     1001      127     7297 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-git/src/util/retry.rs
+-rw-r--r--   0     1001      127     1160 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/Cargo.toml
+-rw-r--r--   0     1001      127    47300 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/lib.rs
+-rw-r--r--   0     1001      127     4626 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
+-rw-r--r--   0     1001      127     2092 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     1703 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
+-rw-r--r--   0     1001      127     1960 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-editable.txt.snap
+-rw-r--r--   0     1001      127      240 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
+-rw-r--r--   0     1001      127     3068 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1298 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
+-rw-r--r--   0     1001      127      569 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
+-rw-r--r--   0     1001      127    11076 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     1703 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
+-rw-r--r--   0     1001      127     1960 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
+-rw-r--r--   0     1001      127     4626 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
+-rw-r--r--   0     1001      127     2092 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     1703 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      240 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
+-rw-r--r--   0     1001      127     3068 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1298 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
+-rw-r--r--   0     1001      127      569 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
+-rw-r--r--   0     1001      127    11076 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     1703 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
+-rw-r--r--   0     1001      127     1960 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
+-rw-r--r--   0     1001      127       90 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/basic.txt
+-rw-r--r--   0     1001      127       45 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
+-rw-r--r--   0     1001      127       27 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
+-rw-r--r--   0     1001      127      183 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/editable.txt
+-rw-r--r--   0     1001      127        0 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/empty.txt
+-rw-r--r--   0     1001      127      101 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
+-rw-r--r--   0     1001      127       43 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/include-a.txt
+-rw-r--r--   0     1001      127        5 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/include-b.txt
+-rw-r--r--   0     1001      127     1183 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
+-rw-r--r--   0     1001      127       66 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/small.txt
+-rw-r--r--   0     1001      127      183 2024-02-23 02:30:21.000000 uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
+-rw-r--r--   0     1001      127     1224 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-dispatch/Cargo.toml
+-rw-r--r--   0     1001      127     9722 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv-dispatch/src/lib.rs
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 uv-0.1.9/crates/uv/Cargo.toml
+-rw-r--r--   0     1001      127     4359 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/cache_clean.rs
+-rw-r--r--   0     1001      127      219 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/cache_dir.rs
+-rw-r--r--   0     1001      127     1903 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/mod.rs
+-rw-r--r--   0     1001      127    16188 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/pip_compile.rs
+-rw-r--r--   0     1001      127     1471 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/pip_freeze.rs
+-rw-r--r--   0     1001      127    22091 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/pip_install.rs
+-rw-r--r--   0     1001      127    15288 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/pip_sync.rs
+-rw-r--r--   0     1001      127     5027 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/pip_uninstall.rs
+-rw-r--r--   0     1001      127     9445 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/reporters.rs
+-rw-r--r--   0     1001      127     6957 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/commands/venv.rs
+-rw-r--r--   0     1001      127    11209 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/compat/mod.rs
+-rw-r--r--   0     1001      127     1859 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/confirm.rs
+-rw-r--r--   0     1001      127     3879 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/logging.rs
+-rw-r--r--   0     1001      127    41927 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/main.rs
+-rw-r--r--   0     1001      127     1223 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/printer.rs
+-rw-r--r--   0     1001      127    14759 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/src/requirements.rs
+-rw-r--r--   0     1001      127    14363 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/common/mod.rs
+-rw-r--r--   0     1001      127   139730 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/pip_compile.rs
+-rw-r--r--   0     1001      127    19181 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/pip_compile_scenarios.rs
+-rw-r--r--   0     1001      127    50014 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/pip_install.rs
+-rw-r--r--   0     1001      127   109909 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/pip_install_scenarios.rs
+-rw-r--r--   0     1001      127    83331 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/pip_sync.rs
+-rw-r--r--   0     1001      127    14422 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/pip_uninstall.rs
+-rw-r--r--   0     1001      127    20780 2024-02-23 02:30:21.000000 uv-0.1.9/crates/uv/tests/venv.rs
+-rw-r--r--   0     1001      127   119809 2024-02-23 02:30:21.000000 uv-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 uv-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      127     2197 2024-02-23 02:30:21.000000 uv-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      127      927 2024-02-23 02:30:21.000000 uv-0.1.9/python/uv/__main__.py
+-rw-r--r--   0     1001      127      806 2024-02-23 02:30:21.000000 uv-0.1.9/python/uv/__init__.py
+-rw-r--r--   0     1001      127        0 2024-02-23 02:30:21.000000 uv-0.1.9/python/uv/py.typed
+-rw-r--r--   0     1001      127    17069 2024-02-23 02:30:21.000000 uv-0.1.9/README.md
+-rw-r--r--   0     1001      127       29 2024-02-23 02:30:21.000000 uv-0.1.9/rust-toolchain.toml
+-rw-r--r--   0        0        0    18436 1970-01-01 00:00:00.000000 uv-0.1.9/PKG-INFO
```

### Comparing `uv-0.1.8/crates/uv-cache/Cargo.toml` & `uv-0.1.9/crates/uv-cache/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-cache/src/cli.rs` & `uv-0.1.9/crates/uv-cache/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-cache/src/lib.rs` & `uv-0.1.9/crates/uv-cache/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 impl CacheBucket {
     fn to_str(self) -> &'static str {
         match self {
             CacheBucket::BuiltWheels => "built-wheels-v0",
             CacheBucket::FlatIndex => "flat-index-v0",
             CacheBucket::Git => "git-v0",
             CacheBucket::Interpreter => "interpreter-v0",
-            CacheBucket::Simple => "simple-v1",
+            CacheBucket::Simple => "simple-v2",
             CacheBucket::Wheels => "wheels-v0",
             CacheBucket::Archive => "archive-v0",
         }
     }
 
     /// Remove a package from the cache bucket.
     ///
```

### Comparing `uv-0.1.8/crates/uv-cache/src/removal.rs` & `uv-0.1.9/crates/uv-cache/src/removal.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-cache/src/timestamp.rs` & `uv-0.1.9/crates/uv-cache/src/timestamp.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-cache/src/wheel.rs` & `uv-0.1.9/crates/uv-cache/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-warnings/src/lib.rs` & `uv-0.1.9/crates/uv-warnings/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/Cargo.toml` & `uv-0.1.9/crates/uv-dispatch/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 [package]
-name = "uv-client"
+name = "uv-dispatch"
 version = "0.0.1"
-edition = "2021"
+description = "Avoid cyclic crate dependencies between resolver, installer and builder"
+edition = { workspace = true }
+rust-version = { workspace = true }
+homepage = { workspace = true }
+documentation = { workspace = true }
+repository = { workspace = true }
+authors = { workspace = true }
+license = { workspace = true }
+
+[lints]
+workspace = true
 
 [dependencies]
-cache-key = { path = "../cache-key" }
-distribution-filename = { path = "../distribution-filename", features = ["rkyv", "serde"] }
 distribution-types = { path = "../distribution-types" }
-install-wheel-rs = { path = "../install-wheel-rs" }
-pep440_rs = { path = "../pep440-rs" }
+gourgeist = { path = "../gourgeist" }
 pep508_rs = { path = "../pep508-rs" }
+platform-host = { path = "../platform-host" }
 platform-tags = { path = "../platform-tags" }
+uv-build = { path = "../uv-build" }
 uv-cache = { path = "../uv-cache" }
-uv-fs = { path = "../uv-fs", features = ["tokio"] }
-uv-normalize = { path = "../uv-normalize" }
-uv-warnings = { path = "../uv-warnings" }
+uv-client = { path = "../uv-client" }
+uv-distribution = { path = "../uv-distribution" }
+uv-installer = { path = "../uv-installer" }
+uv-interpreter = { path = "../uv-interpreter" }
+uv-resolver = { path = "../uv-resolver" }
+uv-traits = { path = "../uv-traits" }
 pypi-types = { path = "../pypi-types" }
 
-async-trait = { workspace = true }
-async_http_range_reader = { workspace = true }
-async_zip = { workspace = true, features = ["tokio"] }
-chrono = { workspace = true }
-fs-err = { workspace = true, features = ["tokio"] }
+anyhow = { workspace = true }
+fs-err = { workspace = true }
 futures = { workspace = true }
-html-escape = { workspace = true }
-http = { workspace = true }
-reqwest = { workspace = true }
-reqwest-middleware = { workspace = true }
-reqwest-retry = { workspace = true }
-rkyv = { workspace = true, features = ["strict", "validation"] }
-rmp-serde = { workspace = true }
-rustc-hash = { workspace = true }
-serde = { workspace = true }
-serde_json = { workspace = true }
-sha2 = { workspace = true }
-task-local-extensions = { workspace = true }
+itertools = { workspace = true }
 tempfile = { workspace = true }
-thiserror = { workspace = true }
-tl = { workspace = true }
-tokio = { workspace = true, features = ["fs"] }
-tokio-util = { workspace = true }
+tokio = { workspace = true }
 tracing = { workspace = true }
-url = { workspace = true }
-urlencoding = { workspace = true }
-
-[dev-dependencies]
-anyhow = { workspace = true }
-insta = { version = "1.34.0" }
-tokio = { workspace = true, features = ["fs", "macros"] }
```

### Comparing `uv-0.1.8/crates/uv-client/src/auth.rs` & `uv-0.1.9/crates/uv-auth/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,84 @@
+/// HTTP authentication utilities.
 use tracing::warn;
 use url::Url;
 
-/// HTTP authentication utilities.
+/// Optimized version of [`safe_copy_url_auth`] which avoids parsing a string
+/// into a URL unless the given URL has authentication to copy. Useful for patterns
+/// where the returned URL would immediately be cast into a string.
+///
+/// Returns [`Err`] if there is authentication to copy and `new_url` is not a valid URL.
+/// Returns [`None`] if there is no authentication to copy.
+pub fn safe_copy_url_auth_to_str(
+    trusted_url: &Url,
+    new_url: &str,
+) -> Result<Option<Url>, url::ParseError> {
+    if trusted_url.username().is_empty() && trusted_url.password().is_none() {
+        return Ok(None);
+    }
+
+    let new_url = Url::parse(new_url)?;
+    Ok(Some(safe_copy_url_auth(trusted_url, new_url)))
+}
 
 /// Copy authentication from one URL to another URL if applicable.
 ///
 /// See [`should_retain_auth`] for details on when authentication is retained.
 #[must_use]
-pub(crate) fn safe_copy_auth(request_url: &Url, mut response_url: Url) -> Url {
-    if should_retain_auth(request_url, &response_url) {
-        response_url
-            .set_username(request_url.username())
-            .unwrap_or_else(|_| {
-                warn!("Failed to transfer username to response URL: {response_url}")
-            });
-        response_url
-            .set_password(request_url.password())
-            .unwrap_or_else(|_| {
-                warn!("Failed to transfer password to response URL: {response_url}")
-            });
+pub fn safe_copy_url_auth(trusted_url: &Url, mut new_url: Url) -> Url {
+    if should_retain_auth(trusted_url, &new_url) {
+        new_url
+            .set_username(trusted_url.username())
+            .unwrap_or_else(|_| warn!("Failed to transfer username to response URL: {new_url}"));
+        new_url
+            .set_password(trusted_url.password())
+            .unwrap_or_else(|_| warn!("Failed to transfer password to response URL: {new_url}"));
     }
-    response_url
+    new_url
 }
 
 /// Determine if authentication information should be retained on a new URL.
 /// Implements the specification defined in RFC 7235 and 7230.
 ///
 /// <https://datatracker.ietf.org/doc/html/rfc7235#section-2.2>
 /// <https://datatracker.ietf.org/doc/html/rfc7230#section-5.5>
-fn should_retain_auth(request_url: &Url, response_url: &Url) -> bool {
+fn should_retain_auth(trusted_url: &Url, new_url: &Url) -> bool {
     // The "scheme" and "authority" components must match to retain authentication
     // The "authority", is composed of the host and port.
 
     // Check the scheme.
     // The scheme must always be an exact match.
     // Note some clients such as Python's `requests` library allow an upgrade
     // from `http` to `https` but this is not spec-compliant.
     // <https://github.com/pypa/pip/blob/75f54cae9271179b8cc80435f92336c97e349f9d/src/pip/_vendor/requests/sessions.py#L133-L136>
-    if request_url.scheme() != response_url.scheme() {
+    if trusted_url.scheme() != new_url.scheme() {
         return false;
     }
 
     // The host must always be an exact match.
-    if request_url.host() != response_url.host() {
+    if trusted_url.host() != new_url.host() {
         return false;
     }
 
     // Check the port.
     // The port is only allowed to differ if it it matches the "default port" for the scheme.
     // However, `reqwest` sets the `port` to `None` if it matches the default port so we do
     // not need any special handling here.
-    if request_url.port() != response_url.port() {
+    if trusted_url.port() != new_url.port() {
         return false;
     }
 
     true
 }
 
 #[cfg(test)]
 mod tests {
     use url::{ParseError, Url};
 
-    use crate::auth::should_retain_auth;
+    use crate::should_retain_auth;
 
     #[test]
     fn test_should_retain_auth() -> Result<(), ParseError> {
         // Exact match (https)
         assert!(should_retain_auth(
             &Url::parse("https://example.com")?,
             &Url::parse("https://example.com")?,
```

### Comparing `uv-0.1.8/crates/uv-client/src/cached_client.rs` & `uv-0.1.9/crates/uv-client/src/cached_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/error.rs` & `uv-0.1.9/crates/uv-client/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/flat_index.rs` & `uv-0.1.9/crates/uv-client/src/flat_index.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 use distribution_types::{
     BuiltDist, Dist, File, FileLocation, FlatIndexLocation, IndexUrl, PrioritizedDist,
     RegistryBuiltDist, RegistrySourceDist, SourceDist,
 };
 use pep440_rs::Version;
 use platform_tags::Tags;
 use pypi_types::{Hashes, Yanked};
+use uv_auth::safe_copy_url_auth;
 use uv_cache::{Cache, CacheBucket};
 use uv_normalize::PackageName;
 
-use crate::auth::safe_copy_auth;
 use crate::cached_client::{CacheControl, CachedClientError};
 use crate::html::SimpleHtml;
 use crate::{Connectivity, Error, ErrorKind, RegistryClient};
 
 #[derive(Debug, thiserror::Error)]
 pub enum FlatIndexError {
     #[error("Failed to read `--find-links` directory: {0}")]
@@ -152,24 +152,25 @@
             .header("Accept", "text/html")
             .build()
             .map_err(ErrorKind::RequestError)?;
         let parse_simple_response = |response: Response| {
             async {
                 // Use the response URL, rather than the request URL, as the base for relative URLs.
                 // This ensures that we handle redirects and other URL transformations correctly.
-                let url = safe_copy_auth(url, response.url().clone());
+                let url = safe_copy_url_auth(url, response.url().clone());
 
                 let text = response.text().await.map_err(ErrorKind::RequestError)?;
                 let SimpleHtml { base, files } = SimpleHtml::parse(&text, &url)
                     .map_err(|err| Error::from_html_err(err, url.clone()))?;
 
+                let base = safe_copy_url_auth(&url, base.into_url());
                 let files: Vec<File> = files
                     .into_iter()
                     .filter_map(|file| {
-                        match File::try_from(file, base.as_url().as_str()) {
+                        match File::try_from(file, &base) {
                             Ok(file) => Some(file),
                             Err(err) => {
                                 // Ignore files with unparsable version specifiers.
                                 warn!("Skipping file in {url}: {err}");
                                 None
                             }
                         }
```

### Comparing `uv-0.1.8/crates/uv-client/src/html.rs` & `uv-0.1.9/crates/uv-client/src/html.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/httpcache/control.rs` & `uv-0.1.9/crates/uv-client/src/httpcache/control.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/httpcache/mod.rs` & `uv-0.1.9/crates/uv-client/src/httpcache/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/lib.rs` & `uv-0.1.9/crates/uv-client/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pub use flat_index::{FlatDistributions, FlatIndex, FlatIndexClient, FlatIndexError};
 pub use registry_client::{
     Connectivity, RegistryClient, RegistryClientBuilder, SimpleMetadata, SimpleMetadatum,
     VersionFiles,
 };
 pub use rkyvutil::OwnedArchive;
 
-mod auth;
 mod cached_client;
 mod error;
 mod flat_index;
 mod html;
 mod httpcache;
 mod middleware;
 mod registry_client;
```

### Comparing `uv-0.1.8/crates/uv-client/src/middleware.rs` & `uv-0.1.9/crates/uv-client/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/registry_client.rs` & `uv-0.1.9/crates/uv-client/src/registry_client.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 use url::Url;
 
 use distribution_filename::{DistFilename, SourceDistFilename, WheelFilename};
 use distribution_types::{BuiltDist, File, FileLocation, IndexUrl, IndexUrls, Name};
 use install_wheel_rs::{find_dist_info, is_metadata_entry};
 use pep440_rs::Version;
 use pypi_types::{Metadata21, SimpleJson};
+use uv_auth::safe_copy_url_auth;
 use uv_cache::{Cache, CacheBucket, WheelCache};
 use uv_normalize::PackageName;
 use uv_warnings::warn_user_once;
 
-use crate::auth::safe_copy_auth;
 use crate::cached_client::CacheControl;
 use crate::html::SimpleHtml;
 use crate::middleware::OfflineMiddleware;
 use crate::remote_metadata::wheel_metadata_from_remote_zip;
 use crate::rkyvutil::OwnedArchive;
 use crate::{CachedClient, CachedClientError, Error, ErrorKind};
 
@@ -245,15 +245,15 @@
             .header("Accept", MediaType::accepts())
             .build()
             .map_err(ErrorKind::RequestError)?;
         let parse_simple_response = |response: Response| {
             async {
                 // Use the response URL, rather than the request URL, as the base for relative URLs.
                 // This ensures that we handle redirects and other URL transformations correctly.
-                let url = safe_copy_auth(&url, response.url().clone());
+                let url = safe_copy_url_auth(&url, response.url().clone());
 
                 let content_type = response
                     .headers()
                     .get("content-type")
                     .ok_or_else(|| Error::from(ErrorKind::MissingContentType(url.clone())))?;
                 let content_type = content_type.to_str().map_err(|err| {
                     Error::from(ErrorKind::InvalidContentTypeHeader(url.clone(), err))
@@ -267,25 +267,24 @@
                 })?;
 
                 let unarchived = match media_type {
                     MediaType::Json => {
                         let bytes = response.bytes().await.map_err(ErrorKind::RequestError)?;
                         let data: SimpleJson = serde_json::from_slice(bytes.as_ref())
                             .map_err(|err| Error::from_json_err(err, url.clone()))?;
-                        let metadata =
-                            SimpleMetadata::from_files(data.files, package_name, url.as_str());
-                        metadata
+
+                        SimpleMetadata::from_files(data.files, package_name, &url)
                     }
                     MediaType::Html => {
                         let text = response.text().await.map_err(ErrorKind::RequestError)?;
                         let SimpleHtml { base, files } = SimpleHtml::parse(&text, &url)
                             .map_err(|err| Error::from_html_err(err, url.clone()))?;
-                        let metadata =
-                            SimpleMetadata::from_files(files, package_name, base.as_url().as_str());
-                        metadata
+                        let base = safe_copy_url_auth(&url, base.into_url());
+
+                        SimpleMetadata::from_files(files, package_name, &base)
                     }
                 };
                 OwnedArchive::from_unarchived(&unarchived)
             }
             .boxed()
             .instrument(info_span!("parse_simple_api", package = %package_name))
         };
@@ -666,15 +665,15 @@
 }
 
 impl SimpleMetadata {
     pub fn iter(&self) -> impl DoubleEndedIterator<Item = &SimpleMetadatum> {
         self.0.iter()
     }
 
-    fn from_files(files: Vec<pypi_types::File>, package_name: &PackageName, base: &str) -> Self {
+    fn from_files(files: Vec<pypi_types::File>, package_name: &PackageName, base: &Url) -> Self {
         let mut map: BTreeMap<Version, VersionFiles> = BTreeMap::default();
 
         // Group the distributions by version and kind
         for file in files {
             if let Some(filename) =
                 DistFilename::try_from_filename(file.filename.as_str(), package_name)
             {
@@ -806,19 +805,19 @@
               "url": "https://files.pythonhosted.org/packages/ad/39/17180d9806a1c50197bc63b25d0f1266f745fc3b23f11439fccb3d6baa50/pyflyby-1.7.8.tar.gz",
               "yanked": false
             }
           ]
         }
         "#;
         let data: SimpleJson = serde_json::from_str(response).unwrap();
-        let base = "https://pypi.org/simple/pyflyby/";
+        let base = Url::parse("https://pypi.org/simple/pyflyby/").unwrap();
         let simple_metadata = SimpleMetadata::from_files(
             data.files,
             &PackageName::from_str("pyflyby").unwrap(),
-            base,
+            &base,
         );
         let versions: Vec<String> = simple_metadata
             .iter()
             .map(|SimpleMetadatum { version, .. }| version.to_string())
             .collect();
         assert_eq!(versions, ["1.7.8".to_string()]);
     }
```

### Comparing `uv-0.1.8/crates/uv-client/src/remote_metadata.rs` & `uv-0.1.9/crates/uv-client/src/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/src/rkyvutil.rs` & `uv-0.1.9/crates/uv-client/src/rkyvutil.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-client/tests/remote_metadata.rs` & `uv-0.1.9/crates/uv-client/tests/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pypi-types/Cargo.toml` & `uv-0.1.9/crates/pypi-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pypi-types/src/base_url.rs` & `uv-0.1.9/crates/pypi-types/src/base_url.rs`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,20 @@
         }
     }
 
     /// Return the underlying [`Url`].
     pub fn as_url(&self) -> &Url {
         &self.0
     }
+
+    /// Convert to the underlying [`Url`].
+    #[must_use]
+    pub fn into_url(self) -> Url {
+        self.0
+    }
 }
 
 impl From<Url> for BaseUrl {
     fn from(url: Url) -> Self {
         Self(url)
     }
 }
```

### Comparing `uv-0.1.8/crates/pypi-types/src/direct_url.rs` & `uv-0.1.9/crates/pypi-types/src/direct_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pypi-types/src/lenient_requirement.rs` & `uv-0.1.9/crates/pypi-types/src/lenient_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pypi-types/src/metadata.rs` & `uv-0.1.9/crates/pypi-types/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pypi-types/src/simple_json.rs` & `uv-0.1.9/crates/pypi-types/src/simple_json.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/Cargo.toml` & `uv-0.1.9/crates/install-wheel-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/Readme.md` & `uv-0.1.9/crates/install-wheel-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/install_location.rs` & `uv-0.1.9/crates/install-wheel-rs/src/install_location.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/lib.rs` & `uv-0.1.9/crates/install-wheel-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/linker.rs` & `uv-0.1.9/crates/install-wheel-rs/src/linker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/main.rs` & `uv-0.1.9/crates/install-wheel-rs/src/main.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/pip_compileall.py` & `uv-0.1.9/crates/install-wheel-rs/src/pip_compileall.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/python_bindings.rs` & `uv-0.1.9/crates/install-wheel-rs/src/python_bindings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/script.rs` & `uv-0.1.9/crates/install-wheel-rs/src/script.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/uninstall.rs` & `uv-0.1.9/crates/install-wheel-rs/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/install-wheel-rs/src/wheel.rs` & `uv-0.1.9/crates/install-wheel-rs/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/Cargo.toml` & `uv-0.1.9/crates/distribution-types/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 [dependencies]
 cache-key = { path = "../cache-key" }
 distribution-filename = { path = "../distribution-filename", features = ["serde"] }
 pep440_rs = { path = "../pep440-rs" }
 pep508_rs = { path = "../pep508-rs" }
 platform-tags = { path = "../platform-tags" }
+uv-auth = { path = "../uv-auth" }
 uv-fs = { path = "../uv-fs" }
 uv-git = { path = "../uv-git", features = ["vendored-openssl"] }
 uv-normalize = { path = "../uv-normalize" }
 pypi-types = { path = "../pypi-types" }
 
 anyhow = { workspace = true }
 data-encoding = { workspace = true }
```

### Comparing `uv-0.1.8/crates/distribution-types/src/any.rs` & `uv-0.1.9/crates/distribution-types/src/any.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/cached.rs` & `uv-0.1.9/crates/distribution-types/src/cached.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/direct_url.rs` & `uv-0.1.9/crates/distribution-types/src/direct_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/editable.rs` & `uv-0.1.9/crates/distribution-types/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/error.rs` & `uv-0.1.9/crates/distribution-types/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/file.rs` & `uv-0.1.9/crates/distribution-types/src/file.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 use std::path::PathBuf;
 
 use serde::{Deserialize, Serialize};
 use thiserror::Error;
 
 use pep440_rs::{VersionSpecifiers, VersionSpecifiersParseError};
 use pypi_types::{DistInfoMetadata, Hashes, Yanked};
+use url::Url;
+use uv_auth::safe_copy_url_auth_to_str;
 
 /// Error converting [`pypi_types::File`] to [`distribution_type::File`].
 #[derive(Debug, Error)]
 pub enum FileConversionError {
     #[error("Failed to parse 'requires-python': {0}")]
     RequiresPython(String, #[source] VersionSpecifiersParseError),
     #[error("Failed to parse URL: {0}")]
@@ -35,27 +37,32 @@
     pub upload_time_utc_ms: Option<i64>,
     pub url: FileLocation,
     pub yanked: Option<Yanked>,
 }
 
 impl File {
     /// `TryFrom` instead of `From` to filter out files with invalid requires python version specifiers
-    pub fn try_from(file: pypi_types::File, base: &str) -> Result<Self, FileConversionError> {
+    pub fn try_from(file: pypi_types::File, base: &Url) -> Result<Self, FileConversionError> {
         Ok(Self {
             dist_info_metadata: file.dist_info_metadata,
             filename: file.filename,
             hashes: file.hashes,
             requires_python: file
                 .requires_python
                 .transpose()
                 .map_err(|err| FileConversionError::RequiresPython(err.line().clone(), err))?,
             size: file.size,
             upload_time_utc_ms: file.upload_time.map(|dt| dt.timestamp_millis()),
             url: if file.url.contains("://") {
-                FileLocation::AbsoluteUrl(file.url)
+                let url = safe_copy_url_auth_to_str(base, &file.url)
+                    .map_err(|err| FileConversionError::Url(file.url.clone(), err))?
+                    .map(|url| url.to_string())
+                    .unwrap_or(file.url);
+
+                FileLocation::AbsoluteUrl(url)
             } else {
                 FileLocation::RelativeUrl(base.to_string(), file.url)
             },
             yanked: file.yanked,
         })
     }
 }
```

### Comparing `uv-0.1.8/crates/distribution-types/src/id.rs` & `uv-0.1.9/crates/distribution-types/src/id.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/index_url.rs` & `uv-0.1.9/crates/distribution-types/src/index_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/installed.rs` & `uv-0.1.9/crates/distribution-types/src/installed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/lib.rs` & `uv-0.1.9/crates/distribution-types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/prioritized_distribution.rs` & `uv-0.1.9/crates/distribution-types/src/prioritized_distribution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/resolution.rs` & `uv-0.1.9/crates/distribution-types/src/resolution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-types/src/traits.rs` & `uv-0.1.9/crates/distribution-types/src/traits.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/platform-host/Cargo.toml` & `uv-0.1.9/crates/platform-host/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/platform-host/src/lib.rs` & `uv-0.1.9/crates/platform-host/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/platform-host/src/linux.rs` & `uv-0.1.9/crates/platform-host/src/linux.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/platform-host/src/mac_os.rs` & `uv-0.1.9/crates/platform-host/src/mac_os.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/Cargo.toml` & `uv-0.1.9/crates/uv-distribution/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/distribution_database.rs` & `uv-0.1.9/crates/uv-distribution/src/distribution_database.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/download.rs` & `uv-0.1.9/crates/uv-distribution/src/download.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/error.rs` & `uv-0.1.9/crates/uv-distribution/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/index/built_wheel_index.rs` & `uv-0.1.9/crates/uv-distribution/src/index/built_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/index/cached_wheel.rs` & `uv-0.1.9/crates/uv-distribution/src/index/cached_wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/index/registry_wheel_index.rs` & `uv-0.1.9/crates/uv-distribution/src/index/registry_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/locks.rs` & `uv-0.1.9/crates/uv-distribution/src/locks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/reporter.rs` & `uv-0.1.9/crates/uv-distribution/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/source/built_wheel_metadata.rs` & `uv-0.1.9/crates/uv-distribution/src/source/built_wheel_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/source/mod.rs` & `uv-0.1.9/crates/uv-distribution/src/source/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-distribution/src/unzip.rs` & `uv-0.1.9/crates/uv-distribution/src/unzip.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-installer/Cargo.toml` & `uv-0.1.9/crates/uv-installer/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-installer/src/downloader.rs` & `uv-0.1.9/crates/uv-installer/src/downloader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-installer/src/editable.rs` & `uv-0.1.9/crates/uv-installer/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-installer/src/installer.rs` & `uv-0.1.9/crates/uv-installer/src/installer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-installer/src/plan.rs` & `uv-0.1.9/crates/uv-installer/src/plan.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-installer/src/site_packages.rs` & `uv-0.1.9/crates/uv-installer/src/site_packages.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/platform-tags/src/lib.rs` & `uv-0.1.9/crates/platform-tags/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-dispatch/Cargo.toml` & `uv-0.1.9/crates/uv-traits/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 [package]
-name = "uv-dispatch"
+name = "uv-traits"
 version = "0.0.1"
-description = "Avoid cyclic crate dependencies between resolver, installer and builder"
 edition = { workspace = true }
 rust-version = { workspace = true }
 homepage = { workspace = true }
 documentation = { workspace = true }
 repository = { workspace = true }
 authors = { workspace = true }
 license = { workspace = true }
 
 [lints]
 workspace = true
 
 [dependencies]
+clap = { workspace = true, optional = true }
 distribution-types = { path = "../distribution-types" }
-gourgeist = { path = "../gourgeist" }
+once-map = { path = "../once-map" }
 pep508_rs = { path = "../pep508-rs" }
-platform-host = { path = "../platform-host" }
-platform-tags = { path = "../platform-tags" }
-uv-build = { path = "../uv-build" }
 uv-cache = { path = "../uv-cache" }
-uv-client = { path = "../uv-client" }
-uv-distribution = { path = "../uv-distribution" }
-uv-installer = { path = "../uv-installer" }
 uv-interpreter = { path = "../uv-interpreter" }
-uv-resolver = { path = "../uv-resolver" }
-uv-traits = { path = "../uv-traits" }
-pypi-types = { path = "../pypi-types" }
+uv-normalize = { path = "../uv-normalize" }
 
 anyhow = { workspace = true }
-fs-err = { workspace = true }
-futures = { workspace = true }
-itertools = { workspace = true }
-tempfile = { workspace = true }
-tokio = { workspace = true }
-tracing = { workspace = true }
+serde = { workspace = true, optional = true }
+serde_json = { workspace = true, optional = true }
+tokio = { workspace = true, features = ["sync"] }
+
+[features]
+default = []
+serde = ["dep:serde", "dep:serde_json"]
```

### Comparing `uv-0.1.8/crates/uv-dispatch/src/lib.rs` & `uv-0.1.9/crates/uv-dispatch/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 use pep508_rs::Requirement;
 use uv_build::{SourceBuild, SourceBuildContext};
 use uv_cache::Cache;
 use uv_client::{FlatIndex, RegistryClient};
 use uv_installer::{Downloader, Installer, NoBinary, Plan, Planner, Reinstall, SitePackages};
 use uv_interpreter::{Interpreter, Virtualenv};
 use uv_resolver::{InMemoryIndex, Manifest, Options, Resolver};
-use uv_traits::{BuildContext, BuildKind, InFlight, NoBuild, SetupPyStrategy};
+use uv_traits::{BuildContext, BuildKind, ConfigSettings, InFlight, NoBuild, SetupPyStrategy};
 
 /// The main implementation of [`BuildContext`], used by the CLI, see [`BuildContext`]
 /// documentation.
 pub struct BuildDispatch<'a> {
     client: &'a RegistryClient,
     cache: &'a Cache,
     interpreter: &'a Interpreter,
@@ -30,14 +30,15 @@
     flat_index: &'a FlatIndex,
     index: &'a InMemoryIndex,
     in_flight: &'a InFlight,
     base_python: PathBuf,
     setup_py: SetupPyStrategy,
     no_build: &'a NoBuild,
     no_binary: &'a NoBinary,
+    config_settings: &'a ConfigSettings,
     source_build_context: SourceBuildContext,
     options: Options,
 }
 
 impl<'a> BuildDispatch<'a> {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
@@ -46,27 +47,29 @@
         interpreter: &'a Interpreter,
         index_locations: &'a IndexLocations,
         flat_index: &'a FlatIndex,
         index: &'a InMemoryIndex,
         in_flight: &'a InFlight,
         base_python: PathBuf,
         setup_py: SetupPyStrategy,
+        config_settings: &'a ConfigSettings,
         no_build: &'a NoBuild,
         no_binary: &'a NoBinary,
     ) -> Self {
         Self {
             client,
             cache,
             interpreter,
             index_locations,
             flat_index,
             index,
             in_flight,
             base_python,
             setup_py,
+            config_settings,
             no_build,
             no_binary,
             source_build_context: SourceBuildContext::default(),
             options: Options::default(),
         }
     }
 
@@ -275,14 +278,15 @@
             source,
             subdirectory,
             self.interpreter,
             self,
             self.source_build_context.clone(),
             package_id.to_string(),
             self.setup_py,
+            self.config_settings.clone(),
             build_kind,
         )
         .boxed()
         .await?;
         Ok(builder)
     }
 }
```

### Comparing `uv-0.1.8/crates/distribution-filename/Cargo.toml` & `uv-0.1.9/crates/distribution-filename/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-filename/src/lib.rs` & `uv-0.1.9/crates/distribution-filename/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap` & `uv-0.1.9/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-filename/src/source_dist.rs` & `uv-0.1.9/crates/distribution-filename/src/source_dist.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/distribution-filename/src/wheel.rs` & `uv-0.1.9/crates/distribution-filename/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-fs/Cargo.toml` & `uv-0.1.9/crates/uv-fs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-fs/src/lib.rs` & `uv-0.1.9/crates/uv-fs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-fs/src/path.rs` & `uv-0.1.9/crates/uv-fs/src/path.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/Cargo.toml` & `uv-0.1.9/crates/uv-resolver/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/candidate_selector.rs` & `uv-0.1.9/crates/uv-resolver/src/candidate_selector.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/constraints.rs` & `uv-0.1.9/crates/uv-resolver/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/dependency_mode.rs` & `uv-0.1.9/crates/uv-resolver/src/dependency_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/editables.rs` & `uv-0.1.9/crates/uv-resolver/src/editables.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/error.rs` & `uv-0.1.9/crates/uv-resolver/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/finder.rs` & `uv-0.1.9/crates/uv-resolver/src/finder.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/lib.rs` & `uv-0.1.9/crates/uv-resolver/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/manifest.rs` & `uv-0.1.9/crates/uv-resolver/src/manifest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/options.rs` & `uv-0.1.9/crates/uv-resolver/src/options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/overrides.rs` & `uv-0.1.9/crates/uv-resolver/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pins.rs` & `uv-0.1.9/crates/uv-resolver/src/pins.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/prerelease_mode.rs` & `uv-0.1.9/crates/uv-resolver/src/prerelease_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pubgrub/dependencies.rs` & `uv-0.1.9/crates/uv-resolver/src/pubgrub/dependencies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pubgrub/distribution.rs` & `uv-0.1.9/crates/uv-resolver/src/pubgrub/distribution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pubgrub/package.rs` & `uv-0.1.9/crates/uv-resolver/src/pubgrub/package.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pubgrub/priority.rs` & `uv-0.1.9/crates/uv-resolver/src/pubgrub/priority.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pubgrub/report.rs` & `uv-0.1.9/crates/uv-resolver/src/pubgrub/report.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/pubgrub/specifier.rs` & `uv-0.1.9/crates/uv-resolver/src/pubgrub/specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/python_requirement.rs` & `uv-0.1.9/crates/uv-resolver/src/python_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolution.rs` & `uv-0.1.9/crates/uv-resolver/src/resolution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolution_mode.rs` & `uv-0.1.9/crates/uv-resolver/src/resolution_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolver/index.rs` & `uv-0.1.9/crates/uv-resolver/src/resolver/index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolver/mod.rs` & `uv-0.1.9/crates/uv-resolver/src/resolver/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolver/provider.rs` & `uv-0.1.9/crates/uv-resolver/src/resolver/provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolver/reporter.rs` & `uv-0.1.9/crates/uv-resolver/src/resolver/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/resolver/urls.rs` & `uv-0.1.9/crates/uv-resolver/src/resolver/urls.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/version_map.rs` & `uv-0.1.9/crates/uv-resolver/src/version_map.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/src/yanks.rs` & `uv-0.1.9/crates/uv-resolver/src/yanks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-resolver/tests/resolver.rs` & `uv-0.1.9/crates/uv-resolver/tests/resolver.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-normalize/src/extra_name.rs` & `uv-0.1.9/crates/uv-normalize/src/extra_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-normalize/src/lib.rs` & `uv-0.1.9/crates/uv-normalize/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-normalize/src/package_name.rs` & `uv-0.1.9/crates/uv-normalize/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/Cargo.toml` & `uv-0.1.9/crates/pep508-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/License-Apache` & `uv-0.1.9/crates/pep440-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/License-BSD` & `uv-0.1.9/crates/pep440-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/Readme.md` & `uv-0.1.9/crates/pep508-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/src/lib.rs` & `uv-0.1.9/crates/pep508-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/src/marker.rs` & `uv-0.1.9/crates/pep508-rs/src/marker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep508-rs/src/verbatim_url.rs` & `uv-0.1.9/crates/pep508-rs/src/verbatim_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-traits/Cargo.toml` & `uv-0.1.9/crates/uv-client/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,51 @@
 [package]
-name = "uv-traits"
+name = "uv-client"
 version = "0.0.1"
-edition = { workspace = true }
-rust-version = { workspace = true }
-homepage = { workspace = true }
-documentation = { workspace = true }
-repository = { workspace = true }
-authors = { workspace = true }
-license = { workspace = true }
-
-[lints]
-workspace = true
+edition = "2021"
 
 [dependencies]
+cache-key = { path = "../cache-key" }
+distribution-filename = { path = "../distribution-filename", features = ["rkyv", "serde"] }
 distribution-types = { path = "../distribution-types" }
-once-map = { path = "../once-map" }
+install-wheel-rs = { path = "../install-wheel-rs" }
+pep440_rs = { path = "../pep440-rs" }
 pep508_rs = { path = "../pep508-rs" }
+platform-tags = { path = "../platform-tags" }
+uv-auth = { path = "../uv-auth" }
 uv-cache = { path = "../uv-cache" }
-uv-interpreter = { path = "../uv-interpreter" }
+uv-fs = { path = "../uv-fs", features = ["tokio"] }
 uv-normalize = { path = "../uv-normalize" }
+uv-warnings = { path = "../uv-warnings" }
+pypi-types = { path = "../pypi-types" }
+
+async-trait = { workspace = true }
+async_http_range_reader = { workspace = true }
+async_zip = { workspace = true, features = ["tokio"] }
+chrono = { workspace = true }
+fs-err = { workspace = true, features = ["tokio"] }
+futures = { workspace = true }
+html-escape = { workspace = true }
+http = { workspace = true }
+reqwest = { workspace = true }
+reqwest-middleware = { workspace = true }
+reqwest-retry = { workspace = true }
+rkyv = { workspace = true, features = ["strict", "validation"] }
+rmp-serde = { workspace = true }
+rustc-hash = { workspace = true }
+serde = { workspace = true }
+serde_json = { workspace = true }
+sha2 = { workspace = true }
+task-local-extensions = { workspace = true }
+tempfile = { workspace = true }
+thiserror = { workspace = true }
+tl = { workspace = true }
+tokio = { workspace = true, features = ["fs"] }
+tokio-util = { workspace = true }
+tracing = { workspace = true }
+url = { workspace = true }
+urlencoding = { workspace = true }
 
+[dev-dependencies]
 anyhow = { workspace = true }
-tokio = { workspace = true, features = ["sync"] }
+insta = { version = "1.34.0" }
+tokio = { workspace = true, features = ["fs", "macros"] }
```

### Comparing `uv-0.1.8/crates/gourgeist/Cargo.toml` & `uv-0.1.9/crates/gourgeist/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/README.md` & `uv-0.1.9/crates/gourgeist/README.md`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/compare_in_git.sh` & `uv-0.1.9/crates/gourgeist/compare_in_git.sh`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/_virtualenv.py` & `uv-0.1.9/crates/gourgeist/src/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activate` & `uv-0.1.9/crates/gourgeist/src/activate`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate` & `uv-0.1.9/crates/gourgeist/src/activator/activate`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate.bat` & `uv-0.1.9/crates/gourgeist/src/activator/activate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate.csh` & `uv-0.1.9/crates/gourgeist/src/activator/activate.csh`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate.fish` & `uv-0.1.9/crates/gourgeist/src/activator/activate.fish`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate.nu` & `uv-0.1.9/crates/gourgeist/src/activator/activate.nu`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate.ps1` & `uv-0.1.9/crates/gourgeist/src/activator/activate.ps1`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/activate_this.py` & `uv-0.1.9/crates/gourgeist/src/activator/activate_this.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/deactivate.bat` & `uv-0.1.9/crates/gourgeist/src/activator/deactivate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/activator/pydoc.bat` & `uv-0.1.9/crates/gourgeist/src/activator/pydoc.bat`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/bare.rs` & `uv-0.1.9/crates/gourgeist/src/bare.rs`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 use fs_err as fs;
 use fs_err::File;
 use tracing::info;
 use uv_fs::Normalized;
 
 use uv_interpreter::Interpreter;
 
-use crate::Prompt;
+use crate::{Error, Prompt};
 
 /// The bash activate scripts with the venv dependent paths patches out
 const ACTIVATE_TEMPLATES: &[(&str, &str)] = &[
     ("activate", include_str!("activator/activate")),
     ("activate.csh", include_str!("activator/activate.csh")),
     ("activate.fish", include_str!("activator/activate.fish")),
     ("activate.nu", include_str!("activator/activate.nu")),
@@ -29,25 +29,18 @@
         "activate_this.py",
         include_str!("activator/activate_this.py"),
     ),
 ];
 const VIRTUALENV_PATCH: &str = include_str!("_virtualenv.py");
 
 /// Very basic `.cfg` file format writer.
-fn write_cfg(
-    f: &mut impl Write,
-    data: &[(&str, String); 8],
-    prompt: Option<String>,
-) -> io::Result<()> {
+fn write_cfg(f: &mut impl Write, data: &[(String, String)]) -> io::Result<()> {
     for (key, value) in data {
         writeln!(f, "{key} = {value}")?;
     }
-    if let Some(prompt) = prompt {
-        writeln!(f, "prompt = {prompt}")?;
-    }
     Ok(())
 }
 
 /// Absolute paths of the virtualenv
 #[derive(Debug)]
 pub struct VenvPaths {
     /// The location of the virtualenv, e.g. `.venv`
@@ -69,51 +62,52 @@
 }
 
 /// Write all the files that belong to a venv without any packages installed.
 pub fn create_bare_venv(
     location: &Utf8Path,
     interpreter: &Interpreter,
     prompt: Prompt,
-) -> io::Result<VenvPaths> {
+    extra_cfg: Vec<(String, String)>,
+) -> Result<VenvPaths, Error> {
     // We have to canonicalize the interpreter path, otherwise the home is set to the venv dir instead of the real root.
     // This would make python-build-standalone fail with the encodings module not being found because its home is wrong.
     let base_python: Utf8PathBuf = fs_err::canonicalize(interpreter.sys_executable())?
         .try_into()
         .map_err(|err: FromPathBufError| err.into_io_error())?;
 
     // Validate the existing location.
     match location.metadata() {
         Ok(metadata) => {
             if metadata.is_file() {
-                return Err(io::Error::new(
+                return Err(Error::IO(io::Error::new(
                     io::ErrorKind::AlreadyExists,
                     format!("File exists at `{location}`"),
-                ));
+                )));
             } else if metadata.is_dir() {
                 if location.join("pyvenv.cfg").is_file() {
                     info!("Removing existing directory");
                     fs::remove_dir_all(location)?;
                     fs::create_dir_all(location)?;
                 } else if location
                     .read_dir()
                     .is_ok_and(|mut dir| dir.next().is_none())
                 {
                     info!("Ignoring empty directory");
                 } else {
-                    return Err(io::Error::new(
+                    return Err(Error::IO(io::Error::new(
                         io::ErrorKind::AlreadyExists,
                         format!("The directory `{location}` exists, but it's not a virtualenv"),
-                    ));
+                    )));
                 }
             }
         }
         Err(err) if err.kind() == io::ErrorKind::NotFound => {
             fs::create_dir_all(location)?;
         }
-        Err(err) => return Err(err),
+        Err(err) => return Err(Error::IO(err)),
     }
 
     // TODO(konstin): I bet on windows we'll have to strip the prefix again
     let location = location.canonicalize_utf8()?;
     let bin_name = if cfg!(unix) {
         "bin"
     } else if cfg!(windows) {
@@ -222,39 +216,66 @@
         // `sys.base_prefix` was the same as the parent of `sys._base_executable`, but a much simpler logic and
         // documented.
         // https://github.com/pypa/virtualenv/blob/d9fdf48d69f0d0ca56140cf0381edbb5d6fe09f5/src/virtualenv/discovery/py_info.py#L136-L156
         interpreter.base_prefix().display().to_string()
     } else {
         unimplemented!("Only Windows and Unix are supported")
     };
-    let pyvenv_cfg_data = &[
-        ("home", python_home),
+
+    // Validate extra_cfg
+    let reserved_keys = [
+        "home",
+        "implementation",
+        "version_info",
+        "include-system-site-packages",
+        "base-prefix",
+        "base-exec-prefix",
+        "base-executable",
+        "prompt",
+    ];
+    for (key, _) in &extra_cfg {
+        if reserved_keys.contains(&key.as_str()) {
+            return Err(Error::ReservedConfigKey(key.to_string()));
+        }
+    }
+
+    let mut pyvenv_cfg_data: Vec<(String, String)> = vec![
+        ("home".to_string(), python_home),
         (
-            "implementation",
+            "implementation".to_string(),
             interpreter.markers().platform_python_implementation.clone(),
         ),
         (
-            "version_info",
+            "version_info".to_string(),
             interpreter.markers().python_version.string.clone(),
         ),
-        ("gourgeist", env!("CARGO_PKG_VERSION").to_string()),
-        // I wouldn't allow this option anyway
-        ("include-system-site-packages", "false".to_string()),
         (
-            "base-prefix",
+            "include-system-site-packages".to_string(),
+            "false".to_string(),
+        ),
+        (
+            "base-prefix".to_string(),
             interpreter.base_prefix().to_string_lossy().to_string(),
         ),
         (
-            "base-exec-prefix",
+            "base-exec-prefix".to_string(),
             interpreter.base_exec_prefix().to_string_lossy().to_string(),
         ),
-        ("base-executable", base_python.to_string()),
-    ];
+        ("base-executable".to_string(), base_python.to_string()),
+    ]
+    .into_iter()
+    .chain(extra_cfg)
+    .collect();
+
+    if let Some(prompt) = prompt {
+        pyvenv_cfg_data.push(("prompt".to_string(), prompt));
+    }
+
     let mut pyvenv_cfg = BufWriter::new(File::create(location.join("pyvenv.cfg"))?);
-    write_cfg(&mut pyvenv_cfg, pyvenv_cfg_data, prompt)?;
+    write_cfg(&mut pyvenv_cfg, &pyvenv_cfg_data)?;
     drop(pyvenv_cfg);
 
     let site_packages = if cfg!(unix) {
         location
             .join("lib")
             .join(format!(
                 "python{}.{}",
```

### Comparing `uv-0.1.8/crates/gourgeist/src/interpreter.rs` & `uv-0.1.9/crates/gourgeist/src/interpreter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/src/lib.rs` & `uv-0.1.9/crates/gourgeist/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 pub enum Error {
     #[error(transparent)]
     IO(#[from] io::Error),
     #[error("Failed to determine python interpreter to use")]
     InvalidPythonInterpreter(#[source] Box<dyn std::error::Error + Sync + Send>),
     #[error(transparent)]
     Platform(#[from] PlatformError),
+    #[error("Reserved key used for pyvenv.cfg: {0}")]
+    ReservedConfigKey(String),
 }
 
 /// The value to use for the shell prompt when inside a virtual environment.
 #[derive(Debug)]
 pub enum Prompt {
     /// Use the current directory name as the prompt.
     CurrentDirectoryName,
@@ -47,17 +49,18 @@
 }
 
 /// Create a virtualenv.
 pub fn create_venv(
     location: &Path,
     interpreter: Interpreter,
     prompt: Prompt,
+    extra_cfg: Vec<(String, String)>,
 ) -> Result<Virtualenv, Error> {
     let location: &Utf8Path = location
         .try_into()
         .map_err(|err: FromPathError| err.into_io_error())?;
-    let paths = create_bare_venv(location, &interpreter, prompt)?;
+    let paths = create_bare_venv(location, &interpreter, prompt, extra_cfg)?;
     Ok(Virtualenv::from_interpreter(
         interpreter,
         paths.root.as_std_path(),
     ))
 }
```

### Comparing `uv-0.1.8/crates/gourgeist/src/main.rs` & `uv-0.1.9/crates/gourgeist/src/main.rs`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     let platform = Platform::current()?;
     let cache = if let Some(project_dirs) = ProjectDirs::from("", "", "gourgeist") {
         Cache::from_path(project_dirs.cache_dir())?
     } else {
         Cache::from_path(".gourgeist_cache")?
     };
     let info = Interpreter::query(python.as_std_path(), &platform, &cache).unwrap();
-    create_bare_venv(&location, &info, Prompt::from_args(cli.prompt))?;
+    create_bare_venv(&location, &info, Prompt::from_args(cli.prompt), Vec::new())?;
     Ok(())
 }
 
 fn main() -> ExitCode {
     tracing_subscriber::registry()
         .with(fmt::layer())
         .with(EnvFilter::from_default_env())
```

### Comparing `uv-0.1.8/crates/gourgeist/static/gourgeist.png` & `uv-0.1.9/crates/gourgeist/static/gourgeist.png`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/gourgeist/venv_checker.py` & `uv-0.1.9/crates/gourgeist/venv_checker.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/Cargo.toml` & `uv-0.1.9/crates/pep440-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/License-Apache` & `uv-0.1.9/crates/pep508-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/License-BSD` & `uv-0.1.9/crates/pep508-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/Readme.md` & `uv-0.1.9/crates/pep440-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/python/Readme.md` & `uv-0.1.9/crates/pep440-rs/python/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/src/lib.rs` & `uv-0.1.9/crates/pep440-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/pep440-rs/src/version.rs` & `uv-0.1.9/crates/pep440-rs/src/version.rs`

 * *Files 2% similar despite different names*

```diff
@@ -739,43 +739,38 @@
 /// We pack versions fitting the above constraints into a `u64` in such a way
 /// that it preserves the ordering between versions as prescribed in PEP 440.
 /// Namely:
 ///
 /// * Bytes 6 and 7 correspond to the first release segment as a `u16`.
 /// * Bytes 5, 4 and 3 correspond to the second, third and fourth release
 /// segments, respectively.
-/// * Byte 2 corresponds to the post-release segment. If there is no
-/// post-release segment, then byte 2 is set to 0x00. This makes "no
-/// post-release" sort before "has post-release." The numeric value
-/// (constrained to be <u8::MAX) has 1 added to it so that 0x00 is reserved to
-/// indicate absence.
-/// * Byte 1 corresponds to the pre-release segment. If there is no pre-release
-/// segment, then byte 1 is set to 0xFF. This makes "no pre-release" sort
-/// after "has pre-release." The most significant two bits of byte 1 encode
-/// the type of pre-release (alpha, beta, rc) while the low 6 bits encode the
-/// pre-release numeric value.
-/// * Byte 0 corresponds to the dev-release segment. If there is no dev-release
-/// segment, then byte 0 is set to 0xFF. This makes "no dev-release" sort after
-/// "has dev-release." The dev-release value (constrained to be <u8::MAX) is
-/// stored in byte 0 as-is.
-///
-/// The order of the encoding above is significant. For example, the
-/// post-release segment is encoded at a more significant byte in the `u64`
-/// than the pre-release segment because `1.2.3.post1 > 1.2.3rc9999`.
-///
-/// Notice also that nothing about the representation inherently prohibits
-/// storing any combination of pre, dev or post release components. We
-/// could absolutely store all three (assuming they fit into their various
-/// constraints outlined above). But, if we did that, a simple `u64::cmp` would
-/// no longer be correct. For example, `1.0.post456.dev34 < 1.0.post456`, but
-/// in the representation above, it would treat `1.0.post456.dev34` as greater
-/// than `1.0.post456`. To make comparisons cheap for multi-component versions
-/// like that, we'd need to use more space. Thankfully, such versions are
-/// incredibly rare. Virtually all versions have zero or one pre, dev or post
-/// release components.
+/// * Bytes 2, 1 and 0 represent *one* of the following:
+///   `.devN, aN, bN, rcN, <no suffix>, .postN`. Its representation is thus:
+///   * The most significant 3 bits of Byte 2 corresponds to a value in
+///   the range 0-5 inclusive, corresponding to dev, pre-a, pre-b, pre-rc,
+///   no-suffix or post releases, respectively.
+///   * The low 5 bits combined with the bits in bytes 1 and 0 correspond
+///   to the release number of the suffix, if one exists. If there is no
+///   suffix, then this bits are always 0.
+///
+/// The order of the encoding above is significant. For example, suffixes are
+/// encoded at a less significant location than the release numbers, so that
+/// `1.2.3 < 1.2.3.post4`.
+///
+/// In a previous representation, we tried to enocode the suffixes in different
+/// locations so that, in theory, you could represent `1.2.3.dev2.post3` in the
+/// packed form. But getting the ordering right for this is difficult (perhaps
+/// impossible without extra space?). So we limited to only storing one suffix.
+/// But even then, we wound up with a bug where `1.0dev1 > 1.0a1`, when of
+/// course, all dev releases should compare less than pre releases. This was
+/// because the encoding recorded the pre-release as "absent", and this in turn
+/// screwed up the order comparisons.
+///
+/// Thankfully, such versions are incredibly rare. Virtually all versions have
+/// zero or one pre, dev or post release components.
 #[derive(Clone, Debug)]
 #[cfg_attr(
     feature = "rkyv",
     derive(rkyv::Archive, rkyv::Deserialize, rkyv::Serialize)
 )]
 #[cfg_attr(feature = "rkyv", archive(check_bytes))]
 #[cfg_attr(
@@ -811,18 +806,26 @@
     /// to truncate the zero components. And always filling out to 4
     /// places somewhat exposes internal details, since the "full" version
     /// representation would not do that.
     len: u8,
 }
 
 impl VersionSmall {
+    const SUFFIX_DEV: u64 = 0;
+    const SUFFIX_PRE_ALPHA: u64 = 1;
+    const SUFFIX_PRE_BETA: u64 = 2;
+    const SUFFIX_PRE_RC: u64 = 3;
+    const SUFFIX_NONE: u64 = 4;
+    const SUFFIX_POST: u64 = 5;
+    const SUFFIX_MAX_VERSION: u64 = 0x1FFFFF;
+
     #[inline]
     fn new() -> VersionSmall {
         VersionSmall {
-            repr: 0x00000000_0000FFFF,
+            repr: 0x00000000_00800000,
             release: [0, 0, 0, 0],
             len: 0,
         }
     }
 
     #[inline]
     fn epoch(&self) -> u64 {
@@ -872,119 +875,158 @@
             self.len += 1;
             true
         }
     }
 
     #[inline]
     fn post(&self) -> Option<u64> {
-        let v = (self.repr >> 16) & 0xFF;
-        if v == 0 {
-            None
+        if self.suffix_kind() == VersionSmall::SUFFIX_POST {
+            Some(self.suffix_version())
         } else {
-            Some(v - 1)
+            None
         }
     }
 
     #[inline]
     fn set_post(&mut self, value: Option<u64>) -> bool {
-        if value.is_some() && (self.pre().is_some() || self.dev().is_some()) {
-            return false;
+        if self.pre().is_some() || self.dev().is_some() {
+            return value.is_none();
         }
         match value {
             None => {
-                self.repr &= !(0xFF << 16);
+                self.set_suffix_kind(VersionSmall::SUFFIX_NONE);
             }
             Some(number) => {
-                if number > 0b1111_1110 {
+                if number > VersionSmall::SUFFIX_MAX_VERSION {
                     return false;
                 }
-                self.repr &= !(0xFF << 16);
-                self.repr |= (number + 1) << 16;
+                self.set_suffix_kind(VersionSmall::SUFFIX_POST);
+                self.set_suffix_version(number);
             }
         }
         true
     }
 
     #[inline]
     fn pre(&self) -> Option<PreRelease> {
-        let v = (self.repr >> 8) & 0xFF;
-        if v == 0xFF {
-            return None;
+        let (kind, number) = (self.suffix_kind(), self.suffix_version());
+        if kind == VersionSmall::SUFFIX_PRE_ALPHA {
+            Some(PreRelease {
+                kind: PreReleaseKind::Alpha,
+                number,
+            })
+        } else if kind == VersionSmall::SUFFIX_PRE_BETA {
+            Some(PreRelease {
+                kind: PreReleaseKind::Beta,
+                number,
+            })
+        } else if kind == VersionSmall::SUFFIX_PRE_RC {
+            Some(PreRelease {
+                kind: PreReleaseKind::Rc,
+                number,
+            })
+        } else {
+            None
         }
-        let number = v & 0b0011_1111;
-        let kind = match v >> 6 {
-            0 => PreReleaseKind::Alpha,
-            1 => PreReleaseKind::Beta,
-            2 => PreReleaseKind::Rc,
-            _ => unreachable!(),
-        };
-        Some(PreRelease { kind, number })
     }
 
     #[inline]
     fn set_pre(&mut self, value: Option<PreRelease>) -> bool {
-        if value.is_some() && (self.post().is_some() || self.dev().is_some()) {
-            return false;
+        if self.dev().is_some() || self.post().is_some() {
+            return value.is_none();
         }
         match value {
             None => {
-                self.repr |= 0xFF << 8;
+                self.set_suffix_kind(VersionSmall::SUFFIX_NONE);
             }
             Some(PreRelease { kind, number }) => {
-                if number > 0b0011_1111 {
+                if number > VersionSmall::SUFFIX_MAX_VERSION {
                     return false;
                 }
-                let kind = match kind {
-                    PreReleaseKind::Alpha => 0,
-                    PreReleaseKind::Beta => 1,
-                    PreReleaseKind::Rc => 2,
-                };
-                self.repr &= !(0xFF << 8);
-                self.repr |= ((kind << 6) | number) << 8;
+                match kind {
+                    PreReleaseKind::Alpha => {
+                        self.set_suffix_kind(VersionSmall::SUFFIX_PRE_ALPHA);
+                    }
+                    PreReleaseKind::Beta => {
+                        self.set_suffix_kind(VersionSmall::SUFFIX_PRE_BETA);
+                    }
+                    PreReleaseKind::Rc => {
+                        self.set_suffix_kind(VersionSmall::SUFFIX_PRE_RC);
+                    }
+                }
+                self.set_suffix_version(number);
             }
         }
         true
     }
 
     #[inline]
     fn dev(&self) -> Option<u64> {
-        let v = self.repr & 0xFF;
-        if v == 0xFF {
-            None
+        if self.suffix_kind() == VersionSmall::SUFFIX_DEV {
+            Some(self.suffix_version())
         } else {
-            Some(v)
+            None
         }
     }
 
     #[inline]
     fn set_dev(&mut self, value: Option<u64>) -> bool {
-        if value.is_some() && (self.pre().is_some() || self.post().is_some()) {
-            return false;
+        if self.pre().is_some() || self.post().is_some() {
+            return value.is_none();
         }
         match value {
             None => {
-                self.repr |= 0xFF;
+                self.set_suffix_kind(VersionSmall::SUFFIX_NONE);
             }
             Some(number) => {
-                if number > 0b1111_1110 {
+                if number > VersionSmall::SUFFIX_MAX_VERSION {
                     return false;
                 }
-                self.repr &= !0xFF;
-                self.repr |= number;
+                self.set_suffix_kind(VersionSmall::SUFFIX_DEV);
+                self.set_suffix_version(number);
             }
         }
         true
     }
 
     #[inline]
     fn local(&self) -> &[LocalSegment] {
         // A "small" version is never used if the version has a non-zero number
         // of local segments.
         &[]
     }
+
+    #[inline]
+    fn suffix_kind(&self) -> u64 {
+        let kind = (self.repr >> 21) & 0b111;
+        debug_assert!(kind <= VersionSmall::SUFFIX_POST);
+        kind
+    }
+
+    #[inline]
+    fn set_suffix_kind(&mut self, kind: u64) {
+        debug_assert!(kind <= VersionSmall::SUFFIX_POST);
+        self.repr &= !0xE00000;
+        self.repr |= kind << 21;
+        if kind == VersionSmall::SUFFIX_NONE {
+            self.set_suffix_version(0);
+        }
+    }
+
+    #[inline]
+    fn suffix_version(&self) -> u64 {
+        self.repr & 0x1FFFFF
+    }
+
+    #[inline]
+    fn set_suffix_version(&mut self, value: u64) {
+        debug_assert!(value <= 0x1FFFFF);
+        self.repr &= !0x1FFFFF;
+        self.repr |= value;
+    }
 }
 
 /// The "full" representation of a version.
 ///
 /// This can represent all possible versions, but is a bit beefier because of
 /// it. It also uses some indirection for variable length data such as the
 /// release numbers and the local segments.
@@ -1364,17 +1406,17 @@
             // think it makes the bit logic much clearer, and makes it
             // explicit that nothing was forgotten.
             #[allow(clippy::identity_op)]
             repr: (u64::from(release[0]) << 48)
                 | (u64::from(release[1]) << 40)
                 | (u64::from(release[2]) << 32)
                 | (u64::from(release[3]) << 24)
-                | (0x00 << 16)
-                | (0xFF << 8)
-                | (0xFF << 0),
+                | (0x80 << 16)
+                | (0x00 << 8)
+                | (0x00 << 0),
             release: [
                 u64::from(release[0]),
                 u64::from(release[1]),
                 u64::from(release[2]),
                 u64::from(release[3]),
             ],
             len,
@@ -3449,24 +3491,26 @@
             "1.0+abc.7",
             "1.0+5",
             "1.0.post456.dev34",
             "1.0.post456",
             "1.0.15",
             "1.1.dev1",
         ];
-        for pair in versions.windows(2) {
-            let less = pair[0].parse::<Version>().unwrap();
-            let greater = pair[1].parse::<Version>().unwrap();
-            assert_eq!(
-                less.cmp(&greater),
-                Ordering::Less,
-                "less: {:?}\ngreater: {:?}",
-                less.as_bloated_debug(),
-                greater.as_bloated_debug()
-            );
+        for (i, v1) in versions.iter().enumerate() {
+            for v2 in versions[i + 1..].iter() {
+                let less = v1.parse::<Version>().unwrap();
+                let greater = v2.parse::<Version>().unwrap();
+                assert_eq!(
+                    less.cmp(&greater),
+                    Ordering::Less,
+                    "less: {:?}\ngreater: {:?}",
+                    less.as_bloated_debug(),
+                    greater.as_bloated_debug()
+                );
+            }
         }
     }
 
     // Tests our bespoke u64 decimal integer parser.
     #[test]
     fn parse_number_u64() {
         let p = |s: &str| parse_u64(s.as_bytes());
```

### Comparing `uv-0.1.8/crates/pep440-rs/src/version_specifier.rs` & `uv-0.1.9/crates/pep440-rs/src/version_specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-build/Cargo.toml` & `uv-0.1.9/crates/uv-build/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 distribution-types = { path = "../distribution-types" }
 gourgeist = { path = "../gourgeist" }
 pep508_rs = { path = "../pep508-rs" }
 platform-host = { path = "../platform-host" }
 uv-extract = { path = "../uv-extract" }
 uv-fs = { path = "../uv-fs" }
 uv-interpreter = { path = "../uv-interpreter" }
-uv-traits = { path = "../uv-traits" }
+uv-traits = { path = "../uv-traits", features = ["serde"] }
 pypi-types = { path = "../pypi-types" }
 
 anyhow = { workspace = true }
 fs-err = { workspace = true }
 indoc = { workspace = true }
 itertools = { workspace = true }
 once_cell = { workspace = true }
```

### Comparing `uv-0.1.8/crates/uv-build/src/lib.rs` & `uv-0.1.9/crates/uv-build/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 use tokio::sync::Mutex;
 use tracing::{debug, info_span, instrument, Instrument};
 
 use distribution_types::Resolution;
 use pep508_rs::Requirement;
 use uv_fs::Normalized;
 use uv_interpreter::{Interpreter, Virtualenv};
-use uv_traits::{BuildContext, BuildKind, SetupPyStrategy, SourceBuildTrait};
+use uv_traits::{BuildContext, BuildKind, ConfigSettings, SetupPyStrategy, SourceBuildTrait};
 
 /// e.g. `pygraphviz/graphviz_wrap.c:3020:10: fatal error: graphviz/cgraph.h: No such file or directory`
 static MISSING_HEADER_RE: Lazy<Regex> = Lazy::new(|| {
     Regex::new(
         r".*\.(?:c|c..|h|h..):\d+:\d+: fatal error: (.*\.(?:h|h..)): No such file or directory",
     )
     .unwrap()
@@ -243,14 +243,15 @@
 /// invocation.
 ///
 /// This keeps both the temp dir and the result of a potential `prepare_metadata_for_build_wheel`
 /// call which changes how we call `build_wheel`.
 pub struct SourceBuild {
     temp_dir: TempDir,
     source_tree: PathBuf,
+    config_settings: ConfigSettings,
     /// If performing a PEP 517 build, the backend to use.
     pep517_backend: Option<Pep517Backend>,
     /// The virtual environment in which to build the source distribution.
     venv: Virtualenv,
     /// Populated if `prepare_metadata_for_build_wheel` was called.
     ///
     /// > If the build frontend has previously called prepare_metadata_for_build_wheel and depends
@@ -277,14 +278,15 @@
         source: &Path,
         subdirectory: Option<&Path>,
         interpreter: &Interpreter,
         build_context: &impl BuildContext,
         source_build_context: SourceBuildContext,
         package_id: String,
         setup_py: SetupPyStrategy,
+        config_settings: ConfigSettings,
         build_kind: BuildKind,
     ) -> Result<SourceBuild, Error> {
         let temp_dir = tempdir_in(build_context.cache().root())?;
 
         let metadata = match fs::metadata(source) {
             Ok(metadata) => metadata,
             Err(err) if err.kind() == io::ErrorKind::NotFound => {
@@ -325,14 +327,15 @@
         let pep517_backend = Self::get_pep517_backend(setup_py, &source_tree, &default_backend)
             .map_err(|err| *err)?;
 
         let venv = gourgeist::create_venv(
             &temp_dir.path().join(".venv"),
             interpreter.clone(),
             gourgeist::Prompt::None,
+            Vec::new(),
         )?;
 
         // Setup the build environment.
         let resolved_requirements = Self::get_resolved_requirements(
             build_context,
             source_build_context,
             &default_backend,
@@ -349,24 +352,26 @@
             create_pep517_build_environment(
                 &source_tree,
                 &venv,
                 pep517_backend,
                 build_context,
                 &package_id,
                 build_kind,
+                &config_settings,
             )
             .await?;
         }
 
         Ok(Self {
             temp_dir,
             source_tree,
             pep517_backend,
             venv,
             build_kind,
+            config_settings,
             metadata_directory: None,
             package_id,
         })
     }
 
     async fn get_resolved_requirements(
         build_context: &impl BuildContext,
@@ -487,18 +492,21 @@
         );
         let script = formatdoc! {
             r#"{}
             import json
 
             prepare_metadata_for_build_wheel = getattr(backend, "prepare_metadata_for_build_wheel", None)
             if prepare_metadata_for_build_wheel:
-                print(prepare_metadata_for_build_wheel("{}"))
+                print(prepare_metadata_for_build_wheel("{}", config_settings={}))
             else:
                 print()
-            "#, pep517_backend.backend_import(), escape_path_for_python(&metadata_directory)
+            "#,
+            pep517_backend.backend_import(),
+            escape_path_for_python(&metadata_directory),
+            self.config_settings.escape_for_python(),
         };
         let span = info_span!(
             "run_python_script",
             script="prepare_metadata_for_build_wheel",
             python_version = %self.venv.interpreter().python_version()
         );
         let output = run_python_script(&self.venv, &script, &self.source_tree)
@@ -614,16 +622,21 @@
         debug!(
             "Calling `{}.build_{}(metadata_directory={})`",
             pep517_backend.backend, self.build_kind, metadata_directory
         );
         let escaped_wheel_dir = escape_path_for_python(wheel_dir);
         let script = formatdoc! {
             r#"{}
-            print(backend.build_{}("{}", metadata_directory={}))
-            "#, pep517_backend.backend_import(), self.build_kind, escaped_wheel_dir, metadata_directory
+            print(backend.build_{}("{}", metadata_directory={}, config_settings={}))
+            "#,
+            pep517_backend.backend_import(),
+            self.build_kind,
+            escaped_wheel_dir,
+            metadata_directory,
+            self.config_settings.escape_for_python()
         };
         let span = info_span!(
             "run_python_script",
             script=format!("build_{}", self.build_kind),
             python_version = %self.venv.interpreter().python_version()
         );
         let output = run_python_script(&self.venv, &script, &self.source_tree)
@@ -677,31 +690,32 @@
 async fn create_pep517_build_environment(
     source_tree: &Path,
     venv: &Virtualenv,
     pep517_backend: &Pep517Backend,
     build_context: &impl BuildContext,
     package_id: &str,
     build_kind: BuildKind,
+    config_settings: &ConfigSettings,
 ) -> Result<(), Error> {
     debug!(
         "Calling `{}.get_requires_for_build_{}()`",
         pep517_backend.backend, build_kind
     );
     let script = formatdoc! {
         r#"
             {}
             import json
 
             get_requires_for_build = getattr(backend, "get_requires_for_build_{}", None)
             if get_requires_for_build:
-                requires = get_requires_for_build()
+                requires = get_requires_for_build(config_settings={})
             else:
                 requires = []
             print(json.dumps(requires))
-        "#, pep517_backend.backend_import(), build_kind
+        "#, pep517_backend.backend_import(), build_kind, config_settings.escape_for_python()
     };
     let span = info_span!(
         "run_python_script",
         script=format!("get_requires_for_build_{}", build_kind),
         python_version = %venv.interpreter().python_version()
     );
     let output = run_python_script(venv, &script, source_tree)
```

### Comparing `uv-0.1.8/crates/uv-interpreter/Cargo.toml` & `uv-0.1.9/crates/uv-interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/cfg.rs` & `uv-0.1.9/crates/uv-interpreter/src/cfg.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/get_interpreter_info.py` & `uv-0.1.9/crates/uv-interpreter/src/get_interpreter_info.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/interpreter.rs` & `uv-0.1.9/crates/uv-interpreter/src/interpreter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/lib.rs` & `uv-0.1.9/crates/uv-interpreter/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/python_platform.rs` & `uv-0.1.9/crates/uv-interpreter/src/python_platform.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/python_query.rs` & `uv-0.1.9/crates/uv-interpreter/src/python_query.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/python_version.rs` & `uv-0.1.9/crates/uv-interpreter/src/python_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-interpreter/src/virtual_env.rs` & `uv-0.1.9/crates/uv-interpreter/src/virtual_env.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/cache-key/src/cache_key.rs` & `uv-0.1.9/crates/cache-key/src/cache_key.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/cache-key/src/canonical_url.rs` & `uv-0.1.9/crates/cache-key/src/canonical_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/cache-key/src/digest.rs` & `uv-0.1.9/crates/cache-key/src/digest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/cache-key/src/stable_hash.rs` & `uv-0.1.9/crates/cache-key/src/stable_hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/once-map/src/lib.rs` & `uv-0.1.9/crates/once-map/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/Cargo.toml` & `uv-0.1.9/crates/uv-git/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/git.rs` & `uv-0.1.9/crates/uv-git/src/git.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/known_hosts.rs` & `uv-0.1.9/crates/uv-git/src/known_hosts.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/lib.rs` & `uv-0.1.9/crates/uv-git/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/sha.rs` & `uv-0.1.9/crates/uv-git/src/sha.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/source.rs` & `uv-0.1.9/crates/uv-git/src/source.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/util/errors.rs` & `uv-0.1.9/crates/uv-git/src/util/errors.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/util/mod.rs` & `uv-0.1.9/crates/uv-git/src/util/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-git/src/util/retry.rs` & `uv-0.1.9/crates/uv-git/src/util/retry.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-extract/Cargo.toml` & `uv-0.1.9/crates/uv-extract/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-extract/src/error.rs` & `uv-0.1.9/crates/uv-extract/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-extract/src/stream.rs` & `uv-0.1.9/crates/uv-extract/src/stream.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-extract/src/sync.rs` & `uv-0.1.9/crates/uv-extract/src/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-extract/src/tar.rs` & `uv-0.1.9/crates/uv-extract/src/tar.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs` & `uv-0.1.9/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/Cargo.toml` & `uv-0.1.9/crates/requirements-txt/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/lib.rs` & `uv-0.1.9/crates/requirements-txt/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-editable.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap` & `uv-0.1.9/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt` & `uv-0.1.9/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/Cargo.toml` & `uv-0.1.9/crates/uv/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uv"
-version = "0.1.8"
+version = "0.1.9"
 edition = { workspace = true }
 rust-version = { workspace = true }
 homepage = { workspace = true }
 documentation = { workspace = true }
 repository = { workspace = true }
 authors = { workspace = true }
 license = { workspace = true }
@@ -78,19 +78,20 @@
 assert_cmd = { version = "2.0.12" }
 assert_fs = { version = "1.1.0" }
 filetime = { version = "0.2.23" }
 indoc = { version = "2.0.4" }
 insta = { version = "1.34.0", features = ["filters"] }
 predicates = { version = "3.0.4" }
 regex = { version = "1.10.3" }
-reqwest = { version = "0.11.23", features = ["blocking", "rustls"], default-features = false }
+reqwest = { version = "0.11.23", features = ["blocking"], default-features = false }
 
 [features]
 default = ["flate2/zlib-ng", "python", "pypi", "git", "maturin"]
 # Introduces a dependency on a local Python installation.
 python = []
 # Introduces a dependency on PyPI.
 pypi = []
 # Introduces a dependency on Git.
 git = []
 # Introduces a dependency on Maturin.
 maturin = []
+
```

### Comparing `uv-0.1.8/crates/uv/src/commands/cache_clean.rs` & `uv-0.1.9/crates/uv/src/commands/cache_clean.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/commands/mod.rs` & `uv-0.1.9/crates/uv/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/commands/pip_compile.rs` & `uv-0.1.9/crates/uv/src/commands/pip_compile.rs`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 use uv_installer::{Downloader, NoBinary};
 use uv_interpreter::{Interpreter, PythonVersion};
 use uv_normalize::{ExtraName, PackageName};
 use uv_resolver::{
     AnnotationStyle, DependencyMode, DisplayResolutionGraph, InMemoryIndex, Manifest,
     OptionsBuilder, PreReleaseMode, ResolutionMode, Resolver,
 };
-use uv_traits::{InFlight, NoBuild, SetupPyStrategy};
+use uv_traits::{ConfigSettings, InFlight, NoBuild, SetupPyStrategy};
 use uv_warnings::warn_user;
 
 use crate::commands::reporters::{DownloadReporter, ResolverReporter};
 use crate::commands::{elapsed, ExitStatus};
 use crate::printer::Printer;
 use crate::requirements::{ExtrasSpecification, RequirementsSource, RequirementsSpecification};
 
@@ -54,14 +54,15 @@
     generate_hashes: bool,
     include_annotations: bool,
     include_header: bool,
     include_index_url: bool,
     include_find_links: bool,
     index_locations: IndexLocations,
     setup_py: SetupPyStrategy,
+    config_settings: ConfigSettings,
     connectivity: Connectivity,
     no_build: &NoBuild,
     python_version: Option<PythonVersion>,
     exclude_newer: Option<DateTime<Utc>>,
     annotation_style: AnnotationStyle,
     cache: Cache,
     mut printer: Printer,
@@ -215,14 +216,15 @@
         &interpreter,
         &index_locations,
         &flat_index,
         &source_index,
         &in_flight,
         interpreter.sys_executable().to_path_buf(),
         setup_py,
+        &config_settings,
         no_build,
         &NoBinary::None,
     )
     .with_options(OptionsBuilder::new().exclude_newer(exclude_newer).build());
 
     // Build the editables and add their requirements
     let editable_metadata = if editables.is_empty() {
@@ -346,22 +348,15 @@
             writer,
             "{}",
             "# This file was autogenerated by uv via the following command:".green()
         )?;
         writeln!(
             writer,
             "{}",
-            format!(
-                "#    uv {}",
-                env::args_os()
-                    .skip(1)
-                    .map(|arg| arg.normalized_display().to_string())
-                    .join(" ")
-            )
-            .green()
+            format!("#    {}", cmd(include_index_url)).green()
         )?;
     }
 
     // Write the index locations to the output channel.
     let mut wrote_index = false;
 
     // If necessary, include the `--index-url` and `--extra-index-url` locations.
@@ -392,21 +387,51 @@
     write!(
         writer,
         "{}",
         DisplayResolutionGraph::new(
             &resolution,
             generate_hashes,
             include_annotations,
-            annotation_style
+            annotation_style,
         )
     )?;
 
     Ok(ExitStatus::Success)
 }
 
+/// Format the `uv` command used to generate the output file.
+fn cmd(include_index_url: bool) -> String {
+    let args = env::args_os()
+        .skip(1)
+        .map(|arg| arg.normalized_display().to_string())
+        .scan(None, move |skip_next, arg| {
+            if let Some(true) = skip_next {
+                // Reset state; skip this iteration.
+                *skip_next = None;
+                Some(None)
+            } else if !include_index_url
+                && (arg.starts_with("--extra-index-url=") || arg.starts_with("--index-url="))
+            {
+                // Reset state; skip this iteration.
+                *skip_next = None;
+                Some(None)
+            } else if !include_index_url && (arg == "--extra-index-url" || arg == "--index-url") {
+                // Mark the next item as (to be) skipped.
+                *skip_next = Some(true);
+                Some(None)
+            } else {
+                // Return the argument.
+                Some(Some(arg))
+            }
+        })
+        .flatten()
+        .join(" ");
+    format!("uv {args}")
+}
+
 /// Whether to allow package upgrades.
 #[derive(Debug)]
 pub(crate) enum Upgrade {
     /// Prefer pinned versions from the existing lockfile, if possible.
     None,
 
     /// Allow package upgrades for all packages, ignoring the existing lockfile.
```

### Comparing `uv-0.1.8/crates/uv/src/commands/pip_freeze.rs` & `uv-0.1.9/crates/uv/src/commands/pip_freeze.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/commands/pip_install.rs` & `uv-0.1.9/crates/uv/src/commands/pip_install.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 };
 use uv_interpreter::{Interpreter, Virtualenv};
 use uv_normalize::PackageName;
 use uv_resolver::{
     DependencyMode, InMemoryIndex, Manifest, Options, OptionsBuilder, PreReleaseMode,
     ResolutionGraph, ResolutionMode, Resolver,
 };
-use uv_traits::{InFlight, NoBuild, SetupPyStrategy};
+use uv_traits::{ConfigSettings, InFlight, NoBuild, SetupPyStrategy};
 
 use crate::commands::reporters::{DownloadReporter, InstallReporter, ResolverReporter};
 use crate::commands::{elapsed, ChangeEvent, ChangeEventKind, ExitStatus};
 use crate::printer::Printer;
 use crate::requirements::{ExtrasSpecification, RequirementsSource, RequirementsSpecification};
 
 use super::Upgrade;
@@ -54,14 +54,15 @@
     dependency_mode: DependencyMode,
     upgrade: Upgrade,
     index_locations: IndexLocations,
     reinstall: &Reinstall,
     link_mode: LinkMode,
     setup_py: SetupPyStrategy,
     connectivity: Connectivity,
+    config_settings: &ConfigSettings,
     no_build: &NoBuild,
     no_binary: &NoBinary,
     strict: bool,
     exclude_newer: Option<DateTime<Utc>>,
     cache: Cache,
     mut printer: Printer,
 ) -> Result<ExitStatus> {
@@ -169,14 +170,15 @@
         &interpreter,
         &index_locations,
         &flat_index,
         &index,
         &in_flight,
         venv.python_executable(),
         setup_py,
+        config_settings,
         no_build,
         no_binary,
     )
     .with_options(OptionsBuilder::new().exclude_newer(exclude_newer).build());
 
     // Build all editable distributions. The editables are shared between resolution and
     // installation, and should live for the duration of the command. If an editable is already
@@ -251,14 +253,15 @@
             &interpreter,
             &index_locations,
             &flat_index,
             &index,
             &in_flight,
             venv.python_executable(),
             setup_py,
+            config_settings,
             no_build,
             no_binary,
         )
         .with_options(OptionsBuilder::new().exclude_newer(exclude_newer).build())
     };
 
     // Sync the environment.
```

### Comparing `uv-0.1.8/crates/uv/src/commands/pip_sync.rs` & `uv-0.1.9/crates/uv/src/commands/pip_sync.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 use uv_dispatch::BuildDispatch;
 use uv_fs::Normalized;
 use uv_installer::{
     Downloader, NoBinary, Plan, Planner, Reinstall, ResolvedEditable, SitePackages,
 };
 use uv_interpreter::Virtualenv;
 use uv_resolver::InMemoryIndex;
-use uv_traits::{InFlight, NoBuild, SetupPyStrategy};
+use uv_traits::{ConfigSettings, InFlight, NoBuild, SetupPyStrategy};
 
 use crate::commands::reporters::{DownloadReporter, FinderReporter, InstallReporter};
 use crate::commands::{elapsed, ChangeEvent, ChangeEventKind, ExitStatus};
 use crate::printer::Printer;
 use crate::requirements::{RequirementsSource, RequirementsSpecification};
 
 /// Install a set of locked requirements into the current Python environment.
@@ -32,14 +32,15 @@
 pub(crate) async fn pip_sync(
     sources: &[RequirementsSource],
     reinstall: &Reinstall,
     link_mode: LinkMode,
     index_locations: IndexLocations,
     setup_py: SetupPyStrategy,
     connectivity: Connectivity,
+    config_settings: &ConfigSettings,
     no_build: &NoBuild,
     no_binary: &NoBinary,
     strict: bool,
     cache: Cache,
     mut printer: Printer,
 ) -> Result<ExitStatus> {
     let start = std::time::Instant::now();
@@ -108,14 +109,15 @@
         venv.interpreter(),
         &index_locations,
         &flat_index,
         &index,
         &in_flight,
         venv.python_executable(),
         setup_py,
+        config_settings,
         no_build,
         no_binary,
     );
 
     // Determine the set of installed packages.
     let site_packages =
         SitePackages::from_executable(&venv).context("Failed to list installed packages")?;
```

### Comparing `uv-0.1.8/crates/uv/src/commands/pip_uninstall.rs` & `uv-0.1.9/crates/uv/src/commands/pip_uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/commands/reporters.rs` & `uv-0.1.9/crates/uv/src/commands/reporters.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/commands/venv.rs` & `uv-0.1.9/crates/uv/src/commands/venv.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 use uv_cache::Cache;
 use uv_client::{Connectivity, FlatIndex, FlatIndexClient, RegistryClientBuilder};
 use uv_dispatch::BuildDispatch;
 use uv_fs::Normalized;
 use uv_installer::NoBinary;
 use uv_interpreter::{find_default_python, find_requested_python, Error};
 use uv_resolver::{InMemoryIndex, OptionsBuilder};
-use uv_traits::{BuildContext, InFlight, NoBuild, SetupPyStrategy};
+use uv_traits::{BuildContext, ConfigSettings, InFlight, NoBuild, SetupPyStrategy};
 
 use crate::commands::ExitStatus;
 use crate::printer::Printer;
 
 /// Create a virtual environment.
 #[allow(clippy::unnecessary_wraps, clippy::too_many_arguments)]
 pub(crate) async fn venv(
@@ -115,16 +115,20 @@
     writeln!(
         printer,
         "Creating virtualenv at: {}",
         path.normalized_display().cyan()
     )
     .into_diagnostic()?;
 
+    // Extra cfg for pyvenv.cfg to specify uv version
+    let extra_cfg = vec![("uv".to_string(), env!("CARGO_PKG_VERSION").to_string())];
+
     // Create the virtual environment.
-    let venv = gourgeist::create_venv(path, interpreter, prompt).map_err(VenvError::Creation)?;
+    let venv = gourgeist::create_venv(path, interpreter, prompt, extra_cfg)
+        .map_err(VenvError::Creation)?;
 
     // Install seed packages.
     if seed {
         // Extract the interpreter.
         let interpreter = venv.interpreter();
 
         // Instantiate a client.
@@ -146,25 +150,29 @@
 
         // Create a shared in-memory index.
         let index = InMemoryIndex::default();
 
         // Track in-flight downloads, builds, etc., across resolutions.
         let in_flight = InFlight::default();
 
+        // For seed packages, assume the default settings are sufficient.
+        let config_settings = ConfigSettings::default();
+
         // Prep the build context.
         let build_dispatch = BuildDispatch::new(
             &client,
             cache,
             interpreter,
             index_locations,
             &flat_index,
             &index,
             &in_flight,
             venv.python_executable(),
             SetupPyStrategy::default(),
+            &config_settings,
             &NoBuild::All,
             &NoBinary::None,
         )
         .with_options(OptionsBuilder::new().exclude_newer(exclude_newer).build());
 
         // Resolve the seed packages.
         let mut requirements = vec![Requirement::from_str("pip").unwrap()];
```

### Comparing `uv-0.1.8/crates/uv/src/compat/mod.rs` & `uv-0.1.9/crates/uv/src/compat/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/confirm.rs` & `uv-0.1.9/crates/uv/src/confirm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/logging.rs` & `uv-0.1.9/crates/uv/src/logging.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/main.rs` & `uv-0.1.9/crates/uv/src/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 use requirements::ExtrasSpecification;
 use uv_cache::{Cache, CacheArgs, Refresh};
 use uv_client::Connectivity;
 use uv_installer::{NoBinary, Reinstall};
 use uv_interpreter::PythonVersion;
 use uv_normalize::{ExtraName, PackageName};
 use uv_resolver::{AnnotationStyle, DependencyMode, PreReleaseMode, ResolutionMode};
-use uv_traits::{NoBuild, PackageNameSpecifier, SetupPyStrategy};
+use uv_traits::{
+    ConfigSettingEntry, ConfigSettings, NoBuild, PackageNameSpecifier, SetupPyStrategy,
+};
 
 use crate::commands::{extra_name_with_clap_error, ExitStatus, Upgrade};
 use crate::compat::CompatArgs;
 use crate::requirements::RequirementsSource;
 
 #[cfg(target_os = "windows")]
 #[global_allocator]
@@ -327,14 +329,18 @@
     /// exit with an error.
     ///
     /// Multiple packages may be provided. Disable binaries for all packages with `:all:`.
     /// Clear previously specified packages with `:none:`.
     #[clap(long, conflicts_with = "no_build")]
     only_binary: Vec<PackageNameSpecifier>,
 
+    /// Settings to pass to the PEP 517 build backend, specified as `KEY=VALUE` pairs.
+    #[clap(long, short = 'C', alias = "config-settings")]
+    config_setting: Vec<ConfigSettingEntry>,
+
     /// The minimum Python version that should be supported by the compiled requirements (e.g.,
     /// `3.7` or `3.7.9`).
     ///
     /// If a patch version is omitted, the most recent known patch version for that minor version
     /// is assumed. For example, `3.7` is mapped to `3.7.17`.
     #[arg(long, short)]
     python_version: Option<PythonVersion>,
@@ -452,14 +458,18 @@
     /// exit with an error.
     ///
     /// Multiple packages may be provided. Disable binaries for all packages with `:all:`.
     /// Clear previously specified packages with `:none:`.
     #[clap(long, conflicts_with = "no_build")]
     only_binary: Vec<PackageNameSpecifier>,
 
+    /// Settings to pass to the PEP 517 build backend, specified as `KEY=VALUE` pairs.
+    #[clap(long, short = 'C', alias = "config-settings")]
+    config_setting: Vec<ConfigSettingEntry>,
+
     /// Validate the virtual environment after completing the installation, to detect packages with
     /// missing dependencies or other issues.
     #[clap(long)]
     strict: bool,
 
     #[command(flatten)]
     compat_args: compat::PipSyncCompatArgs,
@@ -617,14 +627,18 @@
     /// exit with an error.
     ///
     /// Multiple packages may be provided. Disable binaries for all packages with `:all:`.
     /// Clear previously specified packages with `:none:`.
     #[clap(long, conflicts_with = "no_build")]
     only_binary: Vec<PackageNameSpecifier>,
 
+    /// Settings to pass to the PEP 517 build backend, specified as `KEY=VALUE` pairs.
+    #[clap(long, short = 'C', alias = "config-settings")]
+    config_setting: Vec<ConfigSettingEntry>,
+
     /// Validate the virtual environment after completing the installation, to detect packages with
     /// missing dependencies or other issues.
     #[clap(long)]
     strict: bool,
 
     /// Limit candidate packages to those that were uploaded prior to the given date.
     ///
@@ -869,14 +883,20 @@
             let upgrade = Upgrade::from_args(args.upgrade, args.upgrade_package);
             let no_build = NoBuild::from_args(args.only_binary, args.no_build);
             let dependency_mode = if args.no_deps {
                 DependencyMode::Direct
             } else {
                 DependencyMode::Transitive
             };
+            let setup_py = if args.legacy_setup_py {
+                SetupPyStrategy::Setuptools
+            } else {
+                SetupPyStrategy::Pep517
+            };
+            let config_settings = args.config_setting.into_iter().collect::<ConfigSettings>();
             commands::pip_compile(
                 &requirements,
                 &constraints,
                 &overrides,
                 extras,
                 args.output_file.as_deref(),
                 args.resolution,
@@ -885,19 +905,16 @@
                 upgrade,
                 args.generate_hashes,
                 !args.no_annotate,
                 !args.no_header,
                 args.emit_index_url,
                 args.emit_find_links,
                 index_urls,
-                if args.legacy_setup_py {
-                    SetupPyStrategy::Setuptools
-                } else {
-                    SetupPyStrategy::Pep517
-                },
+                setup_py,
+                config_settings,
                 if args.offline {
                     Connectivity::Offline
                 } else {
                     Connectivity::Online
                 },
                 &no_build,
                 args.python_version,
@@ -924,29 +941,33 @@
                 .src_file
                 .into_iter()
                 .map(RequirementsSource::from_path)
                 .collect::<Vec<_>>();
             let reinstall = Reinstall::from_args(args.reinstall, args.reinstall_package);
             let no_binary = NoBinary::from_args(args.no_binary);
             let no_build = NoBuild::from_args(args.only_binary, args.no_build);
+            let setup_py = if args.legacy_setup_py {
+                SetupPyStrategy::Setuptools
+            } else {
+                SetupPyStrategy::Pep517
+            };
+            let config_settings = args.config_setting.into_iter().collect::<ConfigSettings>();
+
             commands::pip_sync(
                 &sources,
                 &reinstall,
                 args.link_mode,
                 index_urls,
-                if args.legacy_setup_py {
-                    SetupPyStrategy::Setuptools
-                } else {
-                    SetupPyStrategy::Pep517
-                },
+                setup_py,
                 if args.offline {
                     Connectivity::Offline
                 } else {
                     Connectivity::Online
                 },
+                &config_settings,
                 &no_build,
                 &no_binary,
                 args.strict,
                 cache,
                 printer,
             )
             .await
@@ -994,36 +1015,40 @@
             let no_binary = NoBinary::from_args(args.no_binary);
             let no_build = NoBuild::from_args(args.only_binary, args.no_build);
             let dependency_mode = if args.no_deps {
                 DependencyMode::Direct
             } else {
                 DependencyMode::Transitive
             };
+            let setup_py = if args.legacy_setup_py {
+                SetupPyStrategy::Setuptools
+            } else {
+                SetupPyStrategy::Pep517
+            };
+            let config_settings = args.config_setting.into_iter().collect::<ConfigSettings>();
+
             commands::pip_install(
                 &requirements,
                 &constraints,
                 &overrides,
                 &extras,
                 args.resolution,
                 args.prerelease,
                 dependency_mode,
                 upgrade,
                 index_urls,
                 &reinstall,
                 args.link_mode,
-                if args.legacy_setup_py {
-                    SetupPyStrategy::Setuptools
-                } else {
-                    SetupPyStrategy::Pep517
-                },
+                setup_py,
                 if args.offline {
                     Connectivity::Offline
                 } else {
                     Connectivity::Online
                 },
+                &config_settings,
                 &no_build,
                 &no_binary,
                 args.strict,
                 args.exclude_newer,
                 cache,
                 printer,
             )
```

### Comparing `uv-0.1.8/crates/uv/src/printer.rs` & `uv-0.1.9/crates/uv/src/printer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/src/requirements.rs` & `uv-0.1.9/crates/uv/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/tests/common/mod.rs` & `uv-0.1.9/crates/uv/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/tests/pip_compile.rs` & `uv-0.1.9/crates/uv/tests/pip_compile.rs`

 * *Files 0% similar despite different names*

```diff
@@ -646,17 +646,17 @@
     let filters: Vec<_> = [
         // 3.7 may not be installed
         (
             "warning: The requested Python version 3.7 is not available; .* will be used to build dependencies instead.\n",
             "",
         ),
     ]
-    .into_iter()
-    .chain(INSTA_FILTERS.to_vec())
-    .collect();
+        .into_iter()
+        .chain(INSTA_FILTERS.to_vec())
+        .collect();
 
     uv_snapshot!(filters, context.compile()
             .arg("requirements.in")
             .arg("--python-version")
             .arg("3.7"), @r###"
     success: false
     exit_code: 1
@@ -2604,15 +2604,15 @@
             .arg("https://download.pytorch.org/whl")
             .env("VIRTUAL_ENV", context.venv.as_os_str())
             .current_dir(context.temp_dir.path()), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile requirements.in --cache-dir [CACHE_DIR] --index-url https://download.pytorch.org/whl
+    #    uv pip compile requirements.in --cache-dir [CACHE_DIR]
     jinja2==3.1.2
     markupsafe==2.1.3
         # via jinja2
 
     ----- stderr -----
     Resolved 2 packages in [TIME]
     "###
@@ -2632,15 +2632,15 @@
             .arg("requirements.in")
             .arg("--index-url")
             .arg("https://test.pypi.org/simple"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in --index-url https://test.pypi.org/simple
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in
     jinja2==3.1.2
     markupsafe==2.1.3
         # via jinja2
 
     ----- stderr -----
     Resolved 2 packages in [TIME]
     "###
@@ -2650,15 +2650,15 @@
             .arg("requirements.in")
             .arg("--index-url")
             .arg("https://test.pypi.org/simple/"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in --index-url https://test.pypi.org/simple/
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in
     jinja2==3.1.2
     markupsafe==2.1.3
         # via jinja2
 
     ----- stderr -----
     Resolved 2 packages in [TIME]
     "###
@@ -3389,14 +3389,15 @@
     "###
     );
 
     Ok(())
 }
 
 /// Emit the `--index-url` and `--extra-index-url` locations.
+/// Also, preserve the `--index-url` and `--extra-index-url` flags in the command in the header.
 #[test]
 fn emit_index_urls() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str("black==23.10.1")?;
 
     uv_snapshot!(context.compile()
@@ -3495,30 +3496,31 @@
     "###
     );
 
     Ok(())
 }
 
 /// Prefer the `--index-url` from the command line over the `--index-url` in a `requirements.txt`
-/// file.
+/// file. Also, `--index-url` and `--extra-index-url` should not be presented in the output
+/// unless we specify `--emit-index-url`.
 #[test]
 fn index_url_requirements_txt() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str("--index-url https://google.com\ntqdm")?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in")
             .arg("--index-url")
             .arg("https://pypi.org/simple"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in --index-url https://pypi.org/simple
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in
     tqdm==4.66.1
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     "###
     );
 
@@ -3901,15 +3903,15 @@
             .arg("requirements.in")
             .arg("--index-url")
             .arg("https://pypi.org/simple"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in --index-url https://pypi.org/simple
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2023-11-18T12:00:00Z requirements.in
     anyio==3.7.1
     idna==3.4
         # via anyio
     sniffio==1.3.0
         # via anyio
 
     ----- stderr -----
```

### Comparing `uv-0.1.8/crates/uv/tests/pip_compile_scenarios.rs` & `uv-0.1.9/crates/uv/tests/pip_compile_scenarios.rs`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     let output = uv_snapshot!(filters, command(&context, python_versions)
         .arg("--python-version=3.11")
         , @r###"
                  success: true
                  exit_code: 0
                  ----- stdout -----
                  # This file was autogenerated by uv via the following command:
-                 #    uv pip compile requirements.in --index-url https://test.pypi.org/simple --find-links https://raw.githubusercontent.com/zanieb/packse/de0bab473eeaa4445db5a8febd732c655fad3d52/vendor/links.html --cache-dir [CACHE_DIR] --python-version=3.11
+                 #    uv pip compile requirements.in --find-links https://raw.githubusercontent.com/zanieb/packse/de0bab473eeaa4445db5a8febd732c655fad3d52/vendor/links.html --cache-dir [CACHE_DIR] --python-version=3.11
                  albatross==1.0.0
 
                  ----- stderr -----
                  warning: The requested Python version 3.11 is not available; 3.9.18 will be used to build dependencies instead.
                  Resolved 1 package in [TIME]
                  "###
     );
@@ -240,15 +240,15 @@
     let output = uv_snapshot!(filters, command(&context, python_versions)
         .arg("--python-version=3.11")
         , @r###"
                  success: true
                  exit_code: 0
                  ----- stdout -----
                  # This file was autogenerated by uv via the following command:
-                 #    uv pip compile requirements.in --index-url https://test.pypi.org/simple --find-links https://raw.githubusercontent.com/zanieb/packse/de0bab473eeaa4445db5a8febd732c655fad3d52/vendor/links.html --cache-dir [CACHE_DIR] --python-version=3.11
+                 #    uv pip compile requirements.in --find-links https://raw.githubusercontent.com/zanieb/packse/de0bab473eeaa4445db5a8febd732c655fad3d52/vendor/links.html --cache-dir [CACHE_DIR] --python-version=3.11
                  albatross==1.0.0
 
                  ----- stderr -----
                  Resolved 1 package in [TIME]
                  "###
     );
 
@@ -460,15 +460,15 @@
     let output = uv_snapshot!(filters, command(&context, python_versions)
         .arg("--python-version=3.8.0")
         , @r###"
                  success: true
                  exit_code: 0
                  ----- stdout -----
                  # This file was autogenerated by uv via the following command:
-                 #    uv pip compile requirements.in --index-url https://test.pypi.org/simple --find-links https://raw.githubusercontent.com/zanieb/packse/de0bab473eeaa4445db5a8febd732c655fad3d52/vendor/links.html --cache-dir [CACHE_DIR] --python-version=3.8.0
+                 #    uv pip compile requirements.in --find-links https://raw.githubusercontent.com/zanieb/packse/de0bab473eeaa4445db5a8febd732c655fad3d52/vendor/links.html --cache-dir [CACHE_DIR] --python-version=3.8.0
                  albatross==1.0.0
 
                  ----- stderr -----
                  warning: The requested Python version 3.8.0 is not available; 3.8.18 will be used to build dependencies instead.
                  Resolved 1 package in [TIME]
                  "###
     );
```

### Comparing `uv-0.1.8/crates/uv/tests/pip_install.rs` & `uv-0.1.9/crates/uv/tests/pip_install.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1594,7 +1594,109 @@
     Hi from the simple launcher!
 
     ----- stderr -----
     "###);
 
     Ok(())
 }
+
+#[test]
+#[cfg(unix)]
+fn config_settings() -> Result<()> {
+    let context = TestContext::new("3.12");
+
+    let current_dir = std::env::current_dir()?;
+    let workspace_dir = regex::escape(
+        Url::from_directory_path(current_dir.join("..").join("..").canonicalize()?)
+            .unwrap()
+            .as_str(),
+    );
+
+    let filters = [(workspace_dir.as_str(), "file://[WORKSPACE_DIR]/")]
+        .into_iter()
+        .chain(INSTA_FILTERS.to_vec())
+        .collect::<Vec<_>>();
+
+    // Install the editable package.
+    uv_snapshot!(filters, Command::new(get_bin())
+        .arg("pip")
+        .arg("install")
+        .arg("-e")
+        .arg("../../scripts/editable-installs/setuptools_editable")
+        .arg("--cache-dir")
+        .arg(context.cache_dir.path())
+        .arg("--exclude-newer")
+        .arg(EXCLUDE_NEWER)
+        .env("VIRTUAL_ENV", context.venv.as_os_str())
+        .env("CARGO_TARGET_DIR", "../../../target/target_install_editable"), @r###"
+    success: true
+    exit_code: 0
+    ----- stdout -----
+
+    ----- stderr -----
+    Built 1 editable in [TIME]
+    Resolved 2 packages in [TIME]
+    Downloaded 1 package in [TIME]
+    Installed 2 packages in [TIME]
+     + iniconfig==2.0.0
+     + setuptools-editable==0.1.0 (from file://[WORKSPACE_DIR]/scripts/editable-installs/setuptools_editable)
+    "###
+    );
+
+    // When installed without `--editable_mode=compat`, the `finder.py` file should be present.
+    let finder = context
+        .venv
+        .join("lib/python3.12/site-packages")
+        .join("__editable___setuptools_editable_0_1_0_finder.py");
+    assert!(finder.exists());
+
+    // Install the editable package with `--editable_mode=compat`.
+    let context = TestContext::new("3.12");
+
+    let current_dir = std::env::current_dir()?;
+    let workspace_dir = regex::escape(
+        Url::from_directory_path(current_dir.join("..").join("..").canonicalize()?)
+            .unwrap()
+            .as_str(),
+    );
+
+    let filters = [(workspace_dir.as_str(), "file://[WORKSPACE_DIR]/")]
+        .into_iter()
+        .chain(INSTA_FILTERS.to_vec())
+        .collect::<Vec<_>>();
+
+    uv_snapshot!(filters, Command::new(get_bin())
+        .arg("pip")
+        .arg("install")
+        .arg("-e")
+        .arg("../../scripts/editable-installs/setuptools_editable")
+        .arg("-C")
+        .arg("editable_mode=compat")
+        .arg("--cache-dir")
+        .arg(context.cache_dir.path())
+        .arg("--exclude-newer")
+        .arg(EXCLUDE_NEWER)
+        .env("VIRTUAL_ENV", context.venv.as_os_str())
+        .env("CARGO_TARGET_DIR", "../../../target/target_install_editable"), @r###"
+    success: true
+    exit_code: 0
+    ----- stdout -----
+
+    ----- stderr -----
+    Built 1 editable in [TIME]
+    Resolved 2 packages in [TIME]
+    Downloaded 1 package in [TIME]
+    Installed 2 packages in [TIME]
+     + iniconfig==2.0.0
+     + setuptools-editable==0.1.0 (from file://[WORKSPACE_DIR]/scripts/editable-installs/setuptools_editable)
+    "###
+    );
+
+    // When installed without `--editable_mode=compat`, the `finder.py` file should _not_ be present.
+    let finder = context
+        .venv
+        .join("lib/python3.12/site-packages")
+        .join("__editable___setuptools_editable_0_1_0_finder.py");
+    assert!(!finder.exists());
+
+    Ok(())
+}
```

### Comparing `uv-0.1.8/crates/uv/tests/pip_install_scenarios.rs` & `uv-0.1.9/crates/uv/tests/pip_install_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/tests/pip_sync.rs` & `uv-0.1.9/crates/uv/tests/pip_sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/tests/pip_uninstall.rs` & `uv-0.1.9/crates/uv/tests/pip_uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/crates/uv/tests/venv.rs` & `uv-0.1.9/crates/uv/tests/venv.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 use std::process::Command;
 
 use anyhow::Result;
 use assert_fs::prelude::*;
 
 use uv_fs::Normalized;
 
-use crate::common::{create_bin_with_executables, get_bin, uv_snapshot, EXCLUDE_NEWER};
+use crate::common::{
+    create_bin_with_executables, get_bin, uv_snapshot, TestContext, EXCLUDE_NEWER,
+};
 
 mod common;
 
 #[test]
 fn create_venv() -> Result<()> {
     let temp_dir = assert_fs::TempDir::new()?;
     let cache_dir = assert_fs::TempDir::new()?;
@@ -640,7 +642,24 @@
     "###
     );
 
     venv.assert(predicates::path::is_dir());
 
     Ok(())
 }
+
+#[test]
+fn verify_pyvenv_cfg() {
+    let context = TestContext::new("3.12");
+    let venv = context.temp_dir.child(".venv");
+    let pyvenv_cfg = venv.child("pyvenv.cfg");
+
+    venv.assert(predicates::path::is_dir());
+
+    // Check pyvenv.cfg exists
+    pyvenv_cfg.assert(predicates::path::is_file());
+
+    // Check if "uv = version" is present in the file
+    let version = env!("CARGO_PKG_VERSION").to_string();
+    let search_string = format!("uv = {version}");
+    pyvenv_cfg.assert(predicates::str::contains(search_string));
+}
```

### Comparing `uv-0.1.8/Cargo.lock` & `uv-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -905,14 +905,15 @@
  "serde",
  "serde_json",
  "sha2",
  "thiserror",
  "tracing",
  "url",
  "urlencoding",
+ "uv-auth",
  "uv-fs",
  "uv-git",
  "uv-normalize",
 ]
 
 [[package]]
 name = "doc-comment"
@@ -4123,15 +4124,15 @@
 name = "uuid"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 
 [[package]]
 name = "uv"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "anstream",
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "base64 0.21.7",
  "chrono",
@@ -4190,14 +4191,22 @@
  "uv-resolver",
  "uv-traits",
  "uv-warnings",
  "which",
 ]
 
 [[package]]
+name = "uv-auth"
+version = "0.0.1"
+dependencies = [
+ "tracing",
+ "url",
+]
+
+[[package]]
 name = "uv-build"
 version = "0.0.1"
 dependencies = [
  "anyhow",
  "distribution-types",
  "fs-err",
  "gourgeist",
@@ -4280,14 +4289,15 @@
  "thiserror",
  "tl",
  "tokio",
  "tokio-util",
  "tracing",
  "url",
  "urlencoding",
+ "uv-auth",
  "uv-cache",
  "uv-fs",
  "uv-normalize",
  "uv-warnings",
 ]
 
 [[package]]
@@ -4586,17 +4596,20 @@
 ]
 
 [[package]]
 name = "uv-traits"
 version = "0.0.1"
 dependencies = [
  "anyhow",
+ "clap",
  "distribution-types",
  "once-map",
  "pep508_rs",
+ "serde",
+ "serde_json",
  "tokio",
  "uv-cache",
  "uv-interpreter",
  "uv-normalize",
 ]
 
 [[package]]
```

### Comparing `uv-0.1.8/Cargo.toml` & `uv-0.1.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/python/uv/__main__.py` & `uv-0.1.9/python/uv/__main__.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/python/uv/__init__.py` & `uv-0.1.9/python/uv/__init__.py`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/README.md` & `uv-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `uv-0.1.8/PKG-INFO` & `uv-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uv
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

