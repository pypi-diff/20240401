# Comparing `tmp/harp_proxy-0.5.0b3.tar.gz` & `tmp/harp_proxy-0.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harp_proxy-0.5.0b3.tar", max compression
+gzip compressed data, was "harp_proxy-0.5.0b4.tar", max compression
```

## Comparing `harp_proxy-0.5.0b3.tar` & `harp_proxy-0.5.0b4.tar`

### file list

```diff
@@ -1,420 +1,420 @@
--rw-r--r--   0        0        0     2001 2024-04-01 15:23:22.909828 harp_proxy-0.5.0b3/LICENSE.rst
--rw-r--r--   0        0        0     3940 2024-04-01 15:23:22.910412 harp_proxy-0.5.0b3/README.rst
--rw-r--r--   0        0        0     2959 2024-04-01 15:23:22.935097 harp_proxy-0.5.0b3/harp/__init__.py
--rw-r--r--   0        0        0       85 2024-04-01 15:23:22.935153 harp_proxy-0.5.0b3/harp/__main__.py
--rw-r--r--   0        0        0     2871 2024-04-01 15:23:22.935221 harp_proxy-0.5.0b3/harp/_logging.py
--rw-r--r--   0        0        0       84 2024-04-01 15:23:22.935305 harp_proxy-0.5.0b3/harp/asgi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.935360 harp_proxy-0.5.0b3/harp/asgi/bridge/__init__.py
--rw-r--r--   0        0        0     2874 2024-04-01 15:23:22.935429 harp_proxy-0.5.0b3/harp/asgi/bridge/requests.py
--rw-r--r--   0        0        0     1313 2024-04-01 15:23:22.935491 harp_proxy-0.5.0b3/harp/asgi/bridge/responses.py
--rw-r--r--   0        0        0     2072 2024-04-01 15:23:22.935550 harp_proxy-0.5.0b3/harp/asgi/events.py
--rw-r--r--   0        0        0     6633 2024-04-01 15:23:22.935623 harp_proxy-0.5.0b3/harp/asgi/kernel.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.935680 harp_proxy-0.5.0b3/harp/asgi/tests/__init__.py
--rw-r--r--   0        0        0     6987 2024-04-01 15:23:22.935760 harp_proxy-0.5.0b3/harp/asgi/tests/test_http_bridge_asgi_request.py
--rw-r--r--   0        0        0     1734 2024-04-01 15:23:22.935860 harp_proxy-0.5.0b3/harp/commandline/__init__.py
--rw-r--r--   0        0        0      352 2024-04-01 15:23:22.935919 harp_proxy-0.5.0b3/harp/commandline/install_dev.py
--rw-r--r--   0        0        0     4305 2024-04-01 15:23:22.935986 harp_proxy-0.5.0b3/harp/commandline/start.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.936045 harp_proxy-0.5.0b3/harp/commandline/utils/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-01 15:23:22.936290 harp_proxy-0.5.0b3/harp/commandline/utils/_hacks.py
--rw-r--r--   0        0        0     4794 2024-04-01 15:23:22.936364 harp_proxy-0.5.0b3/harp/commandline/utils/manager.py
--rw-r--r--   0        0        0      538 2024-04-01 15:23:22.936455 harp_proxy-0.5.0b3/harp/config/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.936515 harp_proxy-0.5.0b3/harp/config/adapters/__init__.py
--rw-r--r--   0        0        0      952 2024-04-01 15:23:22.936582 harp_proxy-0.5.0b3/harp/config/adapters/hypercorn.py
--rw-r--r--   0        0        0     2398 2024-04-01 15:23:22.936644 harp_proxy-0.5.0b3/harp/config/application.py
--rw-r--r--   0        0        0    12157 2024-04-01 15:23:22.936956 harp_proxy-0.5.0b3/harp/config/config.py
--rw-r--r--   0        0        0     1533 2024-04-01 15:23:22.937020 harp_proxy-0.5.0b3/harp/config/events.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.937078 harp_proxy-0.5.0b3/harp/config/factories/__init__.py
--rw-r--r--   0        0        0     4159 2024-04-01 15:23:22.937157 harp_proxy-0.5.0b3/harp/config/factories/kernel_factory.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.937213 harp_proxy-0.5.0b3/harp/config/factories/tests/__init__.py
--rw-r--r--   0        0        0     2026 2024-04-01 15:23:22.937287 harp_proxy-0.5.0b3/harp/config/factories/tests/test_configuration.py
--rw-r--r--   0        0        0     1385 2024-04-01 15:23:22.937349 harp_proxy-0.5.0b3/harp/config/factories/tests/test_settings.py
--rw-r--r--   0        0        0      235 2024-04-01 15:23:22.937435 harp_proxy-0.5.0b3/harp/config/settings/__init__.py
--rw-r--r--   0        0        0      166 2024-04-01 15:23:22.937490 harp_proxy-0.5.0b3/harp/config/settings/base.py
--rw-r--r--   0        0        0      256 2024-04-01 15:23:22.937548 harp_proxy-0.5.0b3/harp/config/settings/disabled.py
--rw-r--r--   0        0        0      626 2024-04-01 15:23:22.937606 harp_proxy-0.5.0b3/harp/config/settings/from_file.py
--rw-r--r--   0        0        0     1381 2024-04-01 15:23:22.937843 harp_proxy-0.5.0b3/harp/controllers/__init__.py
--rw-r--r--   0        0        0      583 2024-04-01 15:23:22.937904 harp_proxy-0.5.0b3/harp/controllers/default.py
--rw-r--r--   0        0        0     1112 2024-04-01 15:23:22.937963 harp_proxy-0.5.0b3/harp/controllers/resolvers.py
--rw-r--r--   0        0        0     3889 2024-04-01 15:23:22.938031 harp_proxy-0.5.0b3/harp/controllers/routing.py
--rw-r--r--   0        0        0      156 2024-04-01 15:23:22.938296 harp_proxy-0.5.0b3/harp/controllers/typing.py
--rw-r--r--   0        0        0      438 2024-04-01 15:23:22.938366 harp_proxy-0.5.0b3/harp/errors.py
--rw-r--r--   0        0        0     1423 2024-04-01 15:23:22.938430 harp_proxy-0.5.0b3/harp/event_dispatcher.py
--rw-r--r--   0        0        0      598 2024-04-01 15:23:22.938530 harp_proxy-0.5.0b3/harp/http/__init__.py
--rw-r--r--   0        0        0      739 2024-04-01 15:23:22.938593 harp_proxy-0.5.0b3/harp/http/errors.py
--rw-r--r--   0        0        0     3907 2024-04-01 15:23:22.938667 harp_proxy-0.5.0b3/harp/http/requests.py
--rw-r--r--   0        0        0     1210 2024-04-01 15:23:22.938726 harp_proxy-0.5.0b3/harp/http/responses.py
--rw-r--r--   0        0        0     3150 2024-04-01 15:23:22.938800 harp_proxy-0.5.0b3/harp/http/serializers.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.938859 harp_proxy-0.5.0b3/harp/http/tests/__init__.py
--rw-r--r--   0        0        0     1671 2024-04-01 15:23:22.938929 harp_proxy-0.5.0b3/harp/http/tests/stubs.py
--rw-r--r--   0        0        0     6125 2024-04-01 15:23:22.938999 harp_proxy-0.5.0b3/harp/http/tests/test_requests.py
--rw-r--r--   0        0        0     3214 2024-04-01 15:23:22.939067 harp_proxy-0.5.0b3/harp/http/tests/test_requests_wrapped.py
--rw-r--r--   0        0        0     3069 2024-04-01 15:23:22.939132 harp_proxy-0.5.0b3/harp/http/tests/test_utils_cookies.py
--rw-r--r--   0        0        0      286 2024-04-01 15:23:22.939221 harp_proxy-0.5.0b3/harp/http/typing/__init__.py
--rw-r--r--   0        0        0      847 2024-04-01 15:23:22.939499 harp_proxy-0.5.0b3/harp/http/typing/bridges.py
--rw-r--r--   0        0        0      591 2024-04-01 15:23:22.939566 harp_proxy-0.5.0b3/harp/http/typing/messages.py
--rw-r--r--   0        0        0      255 2024-04-01 15:23:22.939640 harp_proxy-0.5.0b3/harp/http/typing/serializers.py
--rw-r--r--   0        0        0      123 2024-04-01 15:23:22.939727 harp_proxy-0.5.0b3/harp/http/utils/__init__.py
--rw-r--r--   0        0        0      617 2024-04-01 15:23:22.939787 harp_proxy-0.5.0b3/harp/http/utils/cookies.py
--rw-r--r--   0        0        0     3913 2024-04-01 15:23:22.939855 harp_proxy-0.5.0b3/harp/http/utils/methods.py
--rw-r--r--   0        0        0      794 2024-04-01 15:23:22.939944 harp_proxy-0.5.0b3/harp/meta/__init__.py
--rw-r--r--   0        0        0      470 2024-04-01 15:23:22.940033 harp_proxy-0.5.0b3/harp/models/__init__.py
--rw-r--r--   0        0        0      481 2024-04-01 15:23:22.940097 harp_proxy-0.5.0b3/harp/models/base.py
--rw-r--r--   0        0        0     1732 2024-04-01 15:23:22.940158 harp_proxy-0.5.0b3/harp/models/blobs.py
--rw-r--r--   0        0        0      274 2024-04-01 15:23:22.940214 harp_proxy-0.5.0b3/harp/models/messages.py
--rw-r--r--   0        0        0     1065 2024-04-01 15:23:22.940492 harp_proxy-0.5.0b3/harp/models/transactions.py
--rw-r--r--   0        0        0      365 2024-04-01 15:23:22.940559 harp_proxy-0.5.0b3/harp/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.940618 harp_proxy-0.5.0b3/harp/tests/__init__.py
--rw-r--r--   0        0        0     1684 2024-04-01 15:23:22.940696 harp_proxy-0.5.0b3/harp/tests/test_asgi_kernel.py
--rw-r--r--   0        0        0      988 2024-04-01 15:23:22.940759 harp_proxy-0.5.0b3/harp/tests/test_settings.py
--rw-r--r--   0        0        0      358 2024-04-01 15:23:22.941053 harp_proxy-0.5.0b3/harp/typing/__init__.py
--rw-r--r--   0        0        0      342 2024-04-01 15:23:22.941111 harp_proxy-0.5.0b3/harp/typing/global_settings.py
--rw-r--r--   0        0        0      199 2024-04-01 15:23:22.941164 harp_proxy-0.5.0b3/harp/typing/signs.py
--rw-r--r--   0        0        0     1768 2024-04-01 15:23:22.941369 harp_proxy-0.5.0b3/harp/typing/storage.py
--rw-r--r--   0        0        0      266 2024-04-01 15:23:22.941465 harp_proxy-0.5.0b3/harp/utils/__init__.py
--rw-r--r--   0        0        0      443 2024-04-01 15:23:22.941676 harp_proxy-0.5.0b3/harp/utils/apdex.py
--rw-r--r--   0        0        0      278 2024-04-01 15:23:22.941739 harp_proxy-0.5.0b3/harp/utils/arguments.py
--rw-r--r--   0        0        0     1055 2024-04-01 15:23:22.941804 harp_proxy-0.5.0b3/harp/utils/background.py
--rw-r--r--   0        0        0      188 2024-04-01 15:23:22.941866 harp_proxy-0.5.0b3/harp/utils/bytes.py
--rw-r--r--   0        0        0     2082 2024-04-01 15:23:22.941935 harp_proxy-0.5.0b3/harp/utils/collections.py
--rw-r--r--   0        0        0      739 2024-04-01 15:23:22.942166 harp_proxy-0.5.0b3/harp/utils/dates.py
--rw-r--r--   0        0        0       94 2024-04-01 15:23:22.942232 harp_proxy-0.5.0b3/harp/utils/guids.py
--rw-r--r--   0        0        0      102 2024-04-01 15:23:22.942297 harp_proxy-0.5.0b3/harp/utils/identifiers.py
--rw-r--r--   0        0        0      200 2024-04-01 15:23:22.942382 harp_proxy-0.5.0b3/harp/utils/json.py
--rw-r--r--   0        0        0     1273 2024-04-01 15:23:22.942457 harp_proxy-0.5.0b3/harp/utils/network.py
--rw-r--r--   0        0        0      330 2024-04-01 15:23:22.942524 harp_proxy-0.5.0b3/harp/utils/processes.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.942605 harp_proxy-0.5.0b3/harp/utils/testing/__init__.py
--rw-r--r--   0        0        0      943 2024-04-01 15:23:22.942686 harp_proxy-0.5.0b3/harp/utils/testing/applications.py
--rw-r--r--   0        0        0     2958 2024-04-01 15:23:22.942760 harp_proxy-0.5.0b3/harp/utils/testing/benchmarking.py
--rw-r--r--   0        0        0      217 2024-04-01 15:23:22.942868 harp_proxy-0.5.0b3/harp/utils/testing/communicators/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-01 15:23:22.942939 harp_proxy-0.5.0b3/harp/utils/testing/communicators/asgi.py
--rw-r--r--   0        0        0     2150 2024-04-01 15:23:22.943012 harp_proxy-0.5.0b3/harp/utils/testing/communicators/http.py
--rw-r--r--   0        0        0     4572 2024-04-01 15:23:22.943088 harp_proxy-0.5.0b3/harp/utils/testing/http.py
--rw-r--r--   0        0        0      177 2024-04-01 15:23:22.943198 harp_proxy-0.5.0b3/harp/utils/testing/mixins/__init__.py
--rw-r--r--   0        0        0     2264 2024-04-01 15:23:22.943278 harp_proxy-0.5.0b3/harp/utils/testing/mixins/controllers.py
--rw-r--r--   0        0        0      874 2024-04-01 15:23:22.943393 harp_proxy-0.5.0b3/harp/utils/testing/stub_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.943482 harp_proxy-0.5.0b3/harp/utils/tests/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-01 15:23:22.943566 harp_proxy-0.5.0b3/harp/utils/tests/test_collections.py
--rw-r--r--   0        0        0      691 2024-04-01 15:23:22.943657 harp_proxy-0.5.0b3/harp/utils/tests/test_dates.py
--rw-r--r--   0        0        0      261 2024-04-01 15:23:22.943719 harp_proxy-0.5.0b3/harp/utils/tests/test_urls.py
--rw-r--r--   0        0        0      106 2024-04-01 15:23:22.943787 harp_proxy-0.5.0b3/harp/utils/urls.py
--rw-r--r--   0        0        0      261 2024-04-01 15:23:22.943904 harp_proxy-0.5.0b3/harp/views/__init__.py
--rw-r--r--   0        0        0     1745 2024-04-01 15:23:22.944180 harp_proxy-0.5.0b3/harp/views/json.py
--rw-r--r--   0        0        0      409 2024-04-01 15:23:22.944251 harp_proxy-0.5.0b3/harp/views/strings.py
--rw-r--r--   0        0        0       19 2024-04-01 15:23:22.944360 harp_proxy-0.5.0b3/harp_apps/__init__.py
--rw-r--r--   0        0        0       22 2024-04-01 15:23:22.944466 harp_proxy-0.5.0b3/harp_apps/contrib/__init__.py
--rw-r--r--   0        0        0      728 2024-04-01 15:23:22.944574 harp_proxy-0.5.0b3/harp_apps/contrib/sentry/__app__.py
--rw-r--r--   0        0        0       21 2024-04-01 15:23:22.944637 harp_proxy-0.5.0b3/harp_apps/contrib/sentry/__init__.py
--rw-r--r--   0        0        0       82 2024-04-01 15:23:22.944705 harp_proxy-0.5.0b3/harp_apps/contrib/sentry/settings.py
--rw-r--r--   0        0        0     1248 2024-04-01 15:23:22.944821 harp_proxy-0.5.0b3/harp_apps/dashboard/__app__.py
--rw-r--r--   0        0        0       24 2024-04-01 15:23:22.944883 harp_proxy-0.5.0b3/harp_apps/dashboard/__init__.py
--rw-r--r--   0        0        0     5503 2024-04-01 15:23:22.945026 harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/__init__.py
--rw-r--r--   0        0        0      874 2024-04-01 15:23:22.945114 harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/blobs.py
--rw-r--r--   0        0        0     4732 2024-04-01 15:23:22.945396 harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/overview.py
--rw-r--r--   0        0        0     2757 2024-04-01 15:23:22.945477 harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/system.py
--rw-r--r--   0        0        0     3407 2024-04-01 15:23:22.945558 harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/transactions.py
--rw-r--r--   0        0        0      450 2024-04-01 15:23:22.945884 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/development/index.rst
--rw-r--r--   0        0        0     5487 2024-04-01 15:23:22.945973 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/development/tests_e2e.rst
--rw-r--r--   0        0        0     6937 2024-04-01 15:23:22.946066 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/development/tests_unit.rst
--rw-r--r--   0        0        0      179 2024-04-01 15:23:22.946197 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/examples/auth.basic.yml
--rw-r--r--   0        0        0       99 2024-04-01 15:23:22.946317 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/examples/auth.yml
--rw-r--r--   0        0        0      125 2024-04-01 15:23:22.946392 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/examples/devserver.yml
--rw-r--r--   0        0        0      146 2024-04-01 15:23:22.946465 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/examples/main.yml
--rw-r--r--   0        0        0     2140 2024-04-01 15:23:22.946544 harp_proxy-0.5.0b3/harp_apps/dashboard/docs/index.rst
--rw-r--r--   0        0        0      421 2024-04-01 15:23:22.946824 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/__init__.py
--rw-r--r--   0        0        0      817 2024-04-01 15:23:22.946900 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/base.py
--rw-r--r--   0        0        0      717 2024-04-01 15:23:22.946979 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/transaction_endpoint.py
--rw-r--r--   0        0        0      122 2024-04-01 15:23:22.947045 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/transaction_flag.py
--rw-r--r--   0        0        0      155 2024-04-01 15:23:22.947150 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/transaction_method.py
--rw-r--r--   0        0        0      142 2024-04-01 15:23:22.947215 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/transaction_status.py
--rw-r--r--   0        0        0      168 2024-04-01 15:23:22.947283 harp_proxy-0.5.0b3/harp_apps/dashboard/filters/utils.py
--rw-r--r--   0        0        0     1236 2024-04-01 15:23:22.947412 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      341 2024-04-01 15:23:22.947640 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/.gitignore
--rw-r--r--   0        0        0      268 2024-04-01 15:23:22.947745 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/.ladle/components.tsx
--rw-r--r--   0        0        0       59 2024-04-01 15:23:22.947966 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/.ladle/index.css
--rw-r--r--   0        0        0      188 2024-04-01 15:23:22.948034 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/.prettierrc
--rw-r--r--   0        0        0      357 2024-04-01 15:23:22.948104 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/index.html
--rw-r--r--   0        0        0     7672 2024-04-01 15:23:22.948198 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/mockServiceWorker.js
--rw-r--r--   0        0        0     3803 2024-04-01 15:23:22.948487 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/package.json
--rw-r--r--   0        0        0     2155 2024-04-01 15:23:22.948576 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/playwright.config.ts
--rw-r--r--   0        0        0   272272 2024-04-01 15:23:22.949767 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       81 2024-04-01 15:23:22.949851 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/postcss.config.js
--rw-r--r--   0        0        0     2519 2024-04-01 15:23:22.949955 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/public/harp.svg
--rw-r--r--   0        0        0     2726 2024-04-01 15:23:22.950087 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Assets/logo.svg
--rw-r--r--   0        0        0      808 2024-04-01 15:23:22.950419 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/ApdexBadge.tsx
--rw-r--r--   0        0        0      588 2024-04-01 15:23:22.950638 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/RequestMethodBadge.tsx
--rw-r--r--   0        0        0      877 2024-04-01 15:23:22.950707 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/ResponseStatusBadge.tsx
--rw-r--r--   0        0        0      766 2024-04-01 15:23:22.950959 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/StyledJumboBadge.tsx
--rw-r--r--   0        0        0      616 2024-04-01 15:23:22.951204 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/constants.ts
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.951233 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/index.ts
--rw-r--r--   0        0        0      444 2024-04-01 15:23:22.951340 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Layout/Layout.test.tsx
--rw-r--r--   0        0        0     1901 2024-04-01 15:23:22.951615 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Layout/Layout.tsx
--rw-r--r--   0        0        0     5132 2024-04-01 15:23:22.951914 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Layout/__snapshots__/Layout.test.tsx.snap
--rw-r--r--   0        0        0       49 2024-04-01 15:23:22.951970 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Layout/index.ts
--rw-r--r--   0        0        0     1369 2024-04-01 15:23:22.952074 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/Page.test.tsx
--rw-r--r--   0        0        0     1749 2024-04-01 15:23:22.952141 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/Page.tsx
--rw-r--r--   0        0        0      562 2024-04-01 15:23:22.952327 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/PageTitle.tsx
--rw-r--r--   0        0        0      695 2024-04-01 15:23:22.952488 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/__snapshots__/Page.test.tsx.snap
--rw-r--r--   0        0        0      101 2024-04-01 15:23:22.952545 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/index.tsx
--rw-r--r--   0        0        0     1452 2024-04-01 15:23:22.952648 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Utilities/OnQuerySuccess.tsx
--rw-r--r--   0        0        0       46 2024-04-01 15:23:22.952818 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Api/Types/ItemList.ts
--rw-r--r--   0        0        0       43 2024-04-01 15:23:22.952872 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Api/Types/index.ts
--rw-r--r--   0        0        0       37 2024-04-01 15:23:22.952927 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Api/index.ts
--rw-r--r--   0        0        0     1246 2024-04-01 15:23:22.952989 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Api/useApi.ts
--rw-r--r--   0        0        0       62 2024-04-01 15:23:22.953232 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Overview/index.ts
--rw-r--r--   0        0        0      651 2024-04-01 15:23:22.953639 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Overview/useOverviewDataQuery.ts
--rw-r--r--   0        0        0      491 2024-04-01 15:23:22.953913 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Overview/useSummaryDataQuery.tsx
--rw-r--r--   0        0        0      266 2024-04-01 15:23:22.954013 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/System/index.ts
--rw-r--r--   0        0        0      293 2024-04-01 15:23:22.954076 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/System/useSystemDependenciesQuery.ts
--rw-r--r--   0        0        0      290 2024-04-01 15:23:22.954135 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/System/useSystemQuery.ts
--rw-r--r--   0        0        0      420 2024-04-01 15:23:22.954195 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/System/useSystemSettingsQuery.ts
--rw-r--r--   0        0        0      243 2024-04-01 15:23:22.954256 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/System/useSystemStorageQuery.ts
--rw-r--r--   0        0        0      372 2024-04-01 15:23:22.954393 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/Utils/getRequestFromTransactionMessages.tsx
--rw-r--r--   0        0        0      493 2024-04-01 15:23:22.954453 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/Utils/getResponseFromTransactionMessages.tsx
--rw-r--r--   0        0        0      186 2024-04-01 15:23:22.954509 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/Utils/index.ts
--rw-r--r--   0        0        0      298 2024-04-01 15:23:22.954566 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/index.ts
--rw-r--r--   0        0        0      544 2024-04-01 15:23:22.954634 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useBlobQuery.ts
--rw-r--r--   0        0        0      448 2024-04-01 15:23:22.954697 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useSetUserFlagMutation.ts
--rw-r--r--   0        0        0      371 2024-04-01 15:23:22.954755 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsDetailQuery.ts
--rw-r--r--   0        0        0      439 2024-04-01 15:23:22.954814 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsFiltersQuery.ts
--rw-r--r--   0        0        0     1213 2024-04-01 15:23:22.954882 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsListQuery.ts
--rw-r--r--   0        0        0      323 2024-04-01 15:23:22.955178 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Models/Overview.d.ts
--rw-r--r--   0        0        0     1851 2024-04-01 15:23:22.955418 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Models/Schemas/Transaction.json
--rw-r--r--   0        0        0     1142 2024-04-01 15:23:22.955671 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Models/Transaction.d.ts
--rw-r--r--   0        0        0      586 2024-04-01 15:23:22.955983 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.test.tsx
--rw-r--r--   0        0        0     1379 2024-04-01 15:23:22.956230 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.tsx
--rw-r--r--   0        0        0     1589 2024-04-01 15:23:22.956326 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.test.tsx
--rw-r--r--   0        0        0     3056 2024-04-01 15:23:22.956593 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.tsx
--rw-r--r--   0        0        0    12406 2024-04-01 15:23:22.956860 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/__snapshots__/TransactionsChart.test.tsx.snap
--rw-r--r--   0        0        0       56 2024-04-01 15:23:22.957037 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/index.ts
--rw-r--r--   0        0        0      615 2024-04-01 15:23:22.957303 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/PerformancesSummary.tsx
--rw-r--r--   0        0        0      890 2024-04-01 15:23:22.957528 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/RateSummary.tsx
--rw-r--r--   0        0        0     1184 2024-04-01 15:23:22.957829 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/__snapshots__/BaseTransactionsOverview.test.tsx.snap
--rw-r--r--   0        0        0       70 2024-04-01 15:23:22.957889 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/index.ts
--rw-r--r--   0        0        0      620 2024-04-01 15:23:22.957985 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.test.tsx
--rw-r--r--   0        0        0      700 2024-04-01 15:23:22.958046 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.tsx
--rw-r--r--   0        0        0     1220 2024-04-01 15:23:22.958297 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/__snapshots__/TransactionsOverview.test.tsx.snap
--rw-r--r--   0        0        0       62 2024-04-01 15:23:22.958354 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/index.ts
--rw-r--r--   0        0        0      348 2024-04-01 15:23:22.958423 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/OverviewPage.test.tsx
--rw-r--r--   0        0        0     3785 2024-04-01 15:23:22.958688 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/OverviewPage.tsx
--rw-r--r--   0        0        0    30379 2024-04-01 15:23:22.959037 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/__snapshots__/OverviewPage.test.tsx.snap
--rw-r--r--   0        0        0       50 2024-04-01 15:23:22.959110 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/index.ts
--rw-r--r--   0        0        0      103 2024-04-01 15:23:22.959321 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/utils.ts
--rw-r--r--   0        0        0     1596 2024-04-01 15:23:22.959463 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.test.tsx
--rw-r--r--   0        0        0     1558 2024-04-01 15:23:22.959527 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.tsx
--rw-r--r--   0        0        0      945 2024-04-01 15:23:22.959623 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.test.tsx
--rw-r--r--   0        0        0     2287 2024-04-01 15:23:22.959696 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.tsx
--rw-r--r--   0        0        0       38 2024-04-01 15:23:22.959757 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/index.ts
--rw-r--r--   0        0        0       52 2024-04-01 15:23:22.959810 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/index.ts
--rw-r--r--   0        0        0      636 2024-04-01 15:23:22.959876 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.test.tsx
--rw-r--r--   0        0        0      651 2024-04-01 15:23:22.959952 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.tsx
--rw-r--r--   0        0        0      839 2024-04-01 15:23:22.960013 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.test.tsx
--rw-r--r--   0        0        0      828 2024-04-01 15:23:22.960265 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.tsx
--rw-r--r--   0        0        0      628 2024-04-01 15:23:22.960326 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.test.tsx
--rw-r--r--   0        0        0      596 2024-04-01 15:23:22.960389 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.tsx
--rw-r--r--   0        0        0      718 2024-04-01 15:23:22.960454 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemStorageTabPanel.tsx
--rw-r--r--   0        0        0      628 2024-04-01 15:23:22.960519 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.test.tsx
--rw-r--r--   0        0        0      993 2024-04-01 15:23:22.960578 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.tsx
--rw-r--r--   0        0        0     2196 2024-04-01 15:23:22.960835 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemDependenciesTabPanel.test.tsx.snap
--rw-r--r--   0        0        0    13743 2024-04-01 15:23:22.961107 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemPage.test.tsx.snap
--rw-r--r--   0        0        0     8798 2024-04-01 15:23:22.961173 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemSettingsTabPanel.test.tsx.snap
--rw-r--r--   0        0        0     2957 2024-04-01 15:23:22.961239 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemTopologyTabPanel.test.tsx.snap
--rw-r--r--   0        0        0       46 2024-04-01 15:23:22.961300 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/index.ts
--rw-r--r--   0        0        0     1338 2024-04-01 15:23:22.961456 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Buttons.tsx
--rw-r--r--   0        0        0      355 2024-04-01 15:23:22.961555 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/Facet.test.tsx
--rw-r--r--   0        0        0     3205 2024-04-01 15:23:22.961628 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/Facet.tsx
--rw-r--r--   0        0        0      417 2024-04-01 15:23:22.961695 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetInnerLightButton.test.tsx
--rw-r--r--   0        0        0      397 2024-04-01 15:23:22.961755 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetInnerLightButton.tsx
--rw-r--r--   0        0        0      324 2024-04-01 15:23:22.961814 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetLabel.test.tsx
--rw-r--r--   0        0        0      378 2024-04-01 15:23:22.961871 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetLabel.tsx
--rw-r--r--   0        0        0      893 2024-04-01 15:23:22.961984 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/Facet.test.tsx.snap
--rw-r--r--   0        0        0      230 2024-04-01 15:23:22.962050 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/FacetInnerLightButton.test.tsx.snap
--rw-r--r--   0        0        0      159 2024-04-01 15:23:22.962117 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/FacetLabel.test.tsx.snap
--rw-r--r--   0        0        0       74 2024-04-01 15:23:22.962172 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/index.ts
--rw-r--r--   0        0        0     1162 2024-04-01 15:23:22.962245 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Foldable.tsx
--rw-r--r--   0        0        0     2300 2024-04-01 15:23:22.962355 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.test.tsx
--rw-r--r--   0        0        0     3634 2024-04-01 15:23:22.962625 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.tsx
--rw-r--r--   0        0        0       62 2024-04-01 15:23:22.962683 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/index.ts
--rw-r--r--   0        0        0      493 2024-04-01 15:23:22.962866 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageBody.tsx
--rw-r--r--   0        0        0      866 2024-04-01 15:23:22.963037 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageHeaders.tsx
--rw-r--r--   0        0        0     1258 2024-04-01 15:23:22.963103 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageSummary.tsx
--rw-r--r--   0        0        0      517 2024-04-01 15:23:22.963166 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/OptionalPaginator.tsx
--rw-r--r--   0        0        0     1819 2024-04-01 15:23:22.963377 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/PrettyBody.tsx
--rw-r--r--   0        0        0      546 2024-04-01 15:23:22.963487 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/__snapshots__/HeadersTable.test.tsx.snap
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.963514 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/index.ts
--rw-r--r--   0        0        0      623 2024-04-01 15:23:22.963614 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.test.tsx
--rw-r--r--   0        0        0     2995 2024-04-01 15:23:22.963680 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.tsx
--rw-r--r--   0        0        0    16323 2024-04-01 15:23:22.963794 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/__snapshots__/FiltersSidebar.test.tsx.snap
--rw-r--r--   0        0        0       50 2024-04-01 15:23:22.963849 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/index.ts
--rw-r--r--   0        0        0     1729 2024-04-01 15:23:22.963920 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailOnQuerySuccess.tsx
--rw-r--r--   0        0        0      618 2024-04-01 15:23:22.963982 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.test.tsx
--rw-r--r--   0        0        0      665 2024-04-01 15:23:22.964056 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.tsx
--rw-r--r--   0        0        0     2639 2024-04-01 15:23:22.964128 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListOnQuerySuccess.tsx
--rw-r--r--   0        0        0      460 2024-04-01 15:23:22.964192 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListPage.test.tsx
--rw-r--r--   0        0        0     2217 2024-04-01 15:23:22.964269 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListPage.tsx
--rw-r--r--   0        0        0    10800 2024-04-01 15:23:22.964554 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionListPage.test.tsx.snap
--rw-r--r--   0        0        0    10564 2024-04-01 15:23:22.964697 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsDetailPage.test.tsx.snap
--rw-r--r--   0        0        0    13658 2024-04-01 15:23:22.964838 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsListPage.test.tsx.snap
--rw-r--r--   0        0        0      132 2024-04-01 15:23:22.964912 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/index.ts
--rw-r--r--   0        0        0      365 2024-04-01 15:23:22.965040 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Styles/GlobalStyles.tsx
--rw-r--r--   0        0        0      176 2024-04-01 15:23:22.965170 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Types/filters.d.ts
--rw-r--r--   0        0        0      441 2024-04-01 15:23:22.965291 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Utils/Strings.ts
--rw-r--r--   0        0        0      125 2024-04-01 15:23:22.965363 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/index.css
--rw-r--r--   0        0        0     1987 2024-04-01 15:23:22.965440 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/main.tsx
--rw-r--r--   0        0        0      102 2024-04-01 15:23:22.965863 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/api/index.ts
--rw-r--r--   0        0        0      542 2024-04-01 15:23:22.966153 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/api/overview.ts
--rw-r--r--   0        0        0      687 2024-04-01 15:23:22.966431 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/api/summary.ts
--rw-r--r--   0        0        0      201 2024-04-01 15:23:22.966506 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/browser.ts
--rw-r--r--   0        0        0     4644 2024-04-01 15:23:22.966802 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/handlers.ts
--rw-r--r--   0        0        0      126 2024-04-01 15:23:22.966872 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/node.ts
--rw-r--r--   0        0        0      889 2024-04-01 15:23:22.966945 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/utils.tsx
--rw-r--r--   0        0        0      683 2024-04-01 15:23:22.967347 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.stories.tsx
--rw-r--r--   0        0        0      492 2024-04-01 15:23:22.967423 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.test.tsx
--rw-r--r--   0        0        0      875 2024-04-01 15:23:22.967494 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.tsx
--rw-r--r--   0        0        0      200 2024-04-01 15:23:22.967607 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/__snapshots__/Badge.test.tsx.snap
--rw-r--r--   0        0        0       49 2024-04-01 15:23:22.967669 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/index.ts
--rw-r--r--   0        0        0      303 2024-04-01 15:23:22.967774 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.stories.tsx
--rw-r--r--   0        0        0      675 2024-04-01 15:23:22.967846 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.test.tsx
--rw-r--r--   0        0        0     1084 2024-04-01 15:23:22.967915 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.tsx
--rw-r--r--   0        0        0      189 2024-04-01 15:23:22.968025 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/__snapshots__/Button.test.tsx.snap
--rw-r--r--   0        0        0       34 2024-04-01 15:23:22.968088 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/index.ts
--rw-r--r--   0        0        0      564 2024-04-01 15:23:22.968215 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.stories.tsx
--rw-r--r--   0        0        0     1242 2024-04-01 15:23:22.968299 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.test.tsx
--rw-r--r--   0        0        0     1180 2024-04-01 15:23:22.968377 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.tsx
--rw-r--r--   0        0        0      481 2024-04-01 15:23:22.968491 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/__snapshots__/ButtonGroup.test.tsx.snap
--rw-r--r--   0        0        0       44 2024-04-01 15:23:22.968556 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/index.ts
--rw-r--r--   0        0        0      723 2024-04-01 15:23:22.968663 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.stories.tsx
--rw-r--r--   0        0        0     4620 2024-04-01 15:23:22.968749 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.test.tsx
--rw-r--r--   0        0        0     3528 2024-04-01 15:23:22.968825 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.tsx
--rw-r--r--   0        0        0     2393 2024-04-01 15:23:22.968938 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/__snapshots__/DataTable.test.tsx.snap
--rw-r--r--   0        0        0       53 2024-04-01 15:23:22.969003 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/index.ts
--rw-r--r--   0        0        0     1990 2024-04-01 15:23:22.969129 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.test.tsx
--rw-r--r--   0        0        0     1934 2024-04-01 15:23:22.969215 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.tsx
--rw-r--r--   0        0        0     1864 2024-04-01 15:23:22.969294 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/FormWidgets.stories.tsx
--rw-r--r--   0        0        0     1365 2024-04-01 15:23:22.969365 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.test.tsx
--rw-r--r--   0        0        0      737 2024-04-01 15:23:22.969435 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.tsx
--rw-r--r--   0        0        0      672 2024-04-01 15:23:22.969556 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/__snapshots__/Checkbox.test.tsx.snap
--rw-r--r--   0        0        0      492 2024-04-01 15:23:22.969633 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/__snapshots__/Radio.test.tsx.snap
--rw-r--r--   0        0        0       70 2024-04-01 15:23:22.969714 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/index.ts
--rw-r--r--   0        0        0      947 2024-04-01 15:23:22.969935 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Assets/logo.svg
--rw-r--r--   0        0        0      253 2024-04-01 15:23:22.970014 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.stories.tsx
--rw-r--r--   0        0        0     1235 2024-04-01 15:23:22.970091 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.test.tsx
--rw-r--r--   0        0        0     3938 2024-04-01 15:23:22.970170 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.tsx
--rw-r--r--   0        0        0     2349 2024-04-01 15:23:22.970309 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/__snapshots__/Navbar.test.tsx.snap
--rw-r--r--   0        0        0       34 2024-04-01 15:23:22.970373 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/index.ts
--rw-r--r--   0        0        0      523 2024-04-01 15:23:22.970496 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Pagination.stories.tsx
--rw-r--r--   0        0        0     1925 2024-04-01 15:23:22.970574 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.test.tsx
--rw-r--r--   0        0        0     4971 2024-04-01 15:23:22.970644 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.tsx
--rw-r--r--   0        0        0     4947 2024-04-01 15:23:22.970763 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/__snapshots__/Paginator.test.tsx.snap
--rw-r--r--   0        0        0       40 2024-04-01 15:23:22.970821 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/index.ts
--rw-r--r--   0        0        0     2234 2024-04-01 15:23:22.970964 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.stories.tsx
--rw-r--r--   0        0        0      412 2024-04-01 15:23:22.971034 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.test.tsx
--rw-r--r--   0        0        0      381 2024-04-01 15:23:22.971108 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.tsx
--rw-r--r--   0        0        0      157 2024-04-01 15:23:22.971216 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pane/__snapshots__/Pane.test.tsx.snap
--rw-r--r--   0        0        0       30 2024-04-01 15:23:22.971270 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pane/index.ts
--rw-r--r--   0        0        0      163 2024-04-01 15:23:22.971368 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.stories.tsx
--rw-r--r--   0        0        0      296 2024-04-01 15:23:22.971433 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.test.tsx
--rw-r--r--   0        0        0     1620 2024-04-01 15:23:22.971505 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.tsx
--rw-r--r--   0        0        0      783 2024-04-01 15:23:22.971613 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/__snapshots__/SearchBar.test.tsx.snap
--rw-r--r--   0        0        0       40 2024-04-01 15:23:22.971674 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/index.ts
--rw-r--r--   0        0        0     5048 2024-04-01 15:23:22.971809 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.stories.tsx
--rw-r--r--   0        0        0     1162 2024-04-01 15:23:22.971881 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.test.tsx
--rw-r--r--   0        0        0     1135 2024-04-01 15:23:22.971953 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.tsx
--rw-r--r--   0        0        0      870 2024-04-01 15:23:22.972074 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/__snapshots__/Tabs.test.tsx.snap
--rw-r--r--   0        0        0       29 2024-04-01 15:23:22.972140 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/index.ts
--rw-r--r--   0        0        0      109 2024-04-01 15:23:22.972245 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/Paragraphs.ts
--rw-r--r--   0        0        0       97 2024-04-01 15:23:22.972305 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/Section.ts
--rw-r--r--   0        0        0      627 2024-04-01 15:23:22.972372 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/Titles.ts
--rw-r--r--   0        0        0     1248 2024-04-01 15:23:22.972436 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/Typography.stories.tsx
--rw-r--r--   0        0        0      119 2024-04-01 15:23:22.972488 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/index.ts
--rw-r--r--   0        0        0      120 2024-04-01 15:23:22.972585 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Utilities/index.ts
--rw-r--r--   0        0        0      388 2024-04-01 15:23:22.972783 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/playwright.config.ts
--rw-r--r--   0        0        0     1207 2024-04-01 15:23:22.972899 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts
--rw-r--r--   0        0        0    15116 2024-04-01 15:23:22.973055 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/badge--default-darwin.png
--rw-r--r--   0        0        0     8638 2024-04-01 15:23:22.973146 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--default-darwin.png
--rw-r--r--   0        0        0     6157 2024-04-01 15:23:22.973240 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--primary-darwin.png
--rw-r--r--   0        0        0     6204 2024-04-01 15:23:22.973318 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--secondary-darwin.png
--rw-r--r--   0        0        0     7137 2024-04-01 15:23:22.973416 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button-group--button-group-darwin.png
--rw-r--r--   0        0        0    22924 2024-04-01 15:23:22.973559 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/data-table--default-darwin.png
--rw-r--r--   0        0        0    22499 2024-04-01 15:23:22.973875 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-darwin.png
--rw-r--r--   0        0        0    27926 2024-04-01 15:23:22.974084 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-with-style-darwin.png
--rw-r--r--   0        0        0    25968 2024-04-01 15:23:22.974270 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--radios-darwin.png
--rw-r--r--   0        0        0     8570 2024-04-01 15:23:22.974395 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/navbar--default-darwin.png
--rw-r--r--   0        0        0    20836 2024-04-01 15:23:22.974648 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pagination--paginator-darwin.png
--rw-r--r--   0        0        0   121076 2024-04-01 15:23:22.975466 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pane--default-darwin.png
--rw-r--r--   0        0        0     8281 2024-04-01 15:23:22.975580 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/search-bar--default-darwin.png
--rw-r--r--   0        0        0   200590 2024-04-01 15:23:22.978141 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/tabs--default-darwin.png
--rw-r--r--   0        0        0    23837 2024-04-01 15:23:22.978318 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-darwin.png
--rw-r--r--   0        0        0    44912 2024-04-01 15:23:22.978777 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-with-paragraphs-darwin.png
--rw-r--r--   0        0        0       38 2024-04-01 15:23:22.978851 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0     1479 2024-04-01 15:23:22.978930 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tailwind.config.js
--rw-r--r--   0        0        0      196 2024-04-01 15:23:22.979023 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tests/overviewPage.spec.ts
--rw-r--r--   0        0        0     1034 2024-04-01 15:23:22.979088 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tests/systemDependenciesPage.spec.ts
--rw-r--r--   0        0        0     1147 2024-04-01 15:23:22.979173 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tests/transactionsPage.spec.ts
--rw-r--r--   0        0        0      755 2024-04-01 15:23:22.979238 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tsconfig.json
--rw-r--r--   0        0        0      213 2024-04-01 15:23:22.979308 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tsconfig.node.json
--rw-r--r--   0        0        0      485 2024-04-01 15:23:22.979408 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/types/twin.d.ts
--rw-r--r--   0        0        0     2682 2024-04-01 15:23:22.979478 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/vite.config.ts
--rw-r--r--   0        0        0      725 2024-04-01 15:23:22.979540 harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/vitest.setup.ts
--rw-r--r--   0        0        0       90 2024-04-01 15:23:22.979638 harp_proxy-0.5.0b3/harp_apps/dashboard/schemas/__init__.py
--rw-r--r--   0        0        0      232 2024-04-01 15:23:22.979707 harp_proxy-0.5.0b3/harp_apps/dashboard/schemas/transactions_grouped_by.py
--rw-r--r--   0        0        0     3547 2024-04-01 15:23:22.979781 harp_proxy-0.5.0b3/harp_apps/dashboard/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.979848 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/__init__.py
--rw-r--r--   0        0        0     1752 2024-04-01 15:23:22.979926 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_controllers_blobs.py
--rw-r--r--   0        0        0     2402 2024-04-01 15:23:22.980001 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_controllers_transactions.py
--rw-r--r--   0        0        0      967 2024-04-01 15:23:22.980070 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_settings.py
--rw-r--r--   0        0        0     4039 2024-04-01 15:23:22.980137 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_utils_dependencies.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.980196 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/utils/__init__.py
--rw-r--r--   0        0        0     3101 2024-04-01 15:23:22.980267 harp_proxy-0.5.0b3/harp_apps/dashboard/tests/utils/test_dates.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.980330 harp_proxy-0.5.0b3/harp_apps/dashboard/utils/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-01 15:23:22.980661 harp_proxy-0.5.0b3/harp_apps/dashboard/utils/dates.py
--rw-r--r--   0        0        0     1061 2024-04-01 15:23:22.980724 harp_proxy-0.5.0b3/harp_apps/dashboard/utils/dependencies.py
--rw-r--r--   0        0        0      653 2024-04-01 15:23:22.980828 harp_proxy-0.5.0b3/harp_apps/http_client/__app__.py
--rw-r--r--   0        0        0       26 2024-04-01 15:23:22.980892 harp_proxy-0.5.0b3/harp_apps/http_client/__init__.py
--rw-r--r--   0        0        0      555 2024-04-01 15:23:22.980991 harp_proxy-0.5.0b3/harp_apps/janitor/__app__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.981017 harp_proxy-0.5.0b3/harp_apps/janitor/__init__.py
--rw-r--r--   0        0        0      186 2024-04-01 15:23:22.981083 harp_proxy-0.5.0b3/harp_apps/janitor/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.981145 harp_proxy-0.5.0b3/harp_apps/janitor/tests/__init__.py
--rw-r--r--   0        0        0     3505 2024-04-01 15:23:22.981213 harp_proxy-0.5.0b3/harp_apps/janitor/tests/test_worker.py
--rw-r--r--   0        0        0     3911 2024-04-01 15:23:22.981288 harp_proxy-0.5.0b3/harp_apps/janitor/worker.py
--rw-r--r--   0        0        0     1023 2024-04-01 15:23:22.981631 harp_proxy-0.5.0b3/harp_apps/proxy/__app__.py
--rw-r--r--   0        0        0       20 2024-04-01 15:23:22.981694 harp_proxy-0.5.0b3/harp_apps/proxy/__init__.py
--rw-r--r--   0        0        0     7425 2024-04-01 15:23:22.981990 harp_proxy-0.5.0b3/harp_apps/proxy/controllers.py
--rw-r--r--   0        0        0       88 2024-04-01 15:23:22.982119 harp_proxy-0.5.0b3/harp_apps/proxy/docs/examples/swapi.yml
--rw-r--r--   0        0        0      862 2024-04-01 15:23:22.982188 harp_proxy-0.5.0b3/harp_apps/proxy/docs/index.rst
--rw-r--r--   0        0        0      164 2024-04-01 15:23:22.982246 harp_proxy-0.5.0b3/harp_apps/proxy/events.py
--rw-r--r--   0        0        0      633 2024-04-01 15:23:22.982303 harp_proxy-0.5.0b3/harp_apps/proxy/settings.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.982361 harp_proxy-0.5.0b3/harp_apps/proxy/tests/__init__.py
--rw-r--r--   0        0        0     8497 2024-04-01 15:23:22.982669 harp_proxy-0.5.0b3/harp_apps/proxy/tests/test_controllers_http_proxy.py
--rw-r--r--   0        0        0     1061 2024-04-01 15:23:22.982774 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/__app__.py
--rw-r--r--   0        0        0       33 2024-04-01 15:23:22.982832 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/__init__.py
--rw-r--r--   0        0        0      160 2024-04-01 15:23:22.982890 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/constants.py
--rw-r--r--   0        0        0     1033 2024-04-01 15:23:22.982987 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/docs/index.rst
--rw-r--r--   0        0        0      877 2024-04-01 15:23:22.983078 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/__init__.py
--rw-r--r--   0        0        0     2194 2024-04-01 15:23:22.983147 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/base.py
--rw-r--r--   0        0        0     1928 2024-04-01 15:23:22.983217 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/blobs.py
--rw-r--r--   0        0        0     1082 2024-04-01 15:23:22.983278 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/flags.py
--rw-r--r--   0        0        0     2413 2024-04-01 15:23:22.983349 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/messages.py
--rw-r--r--   0        0        0     1425 2024-04-01 15:23:22.983415 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/metrics.py
--rw-r--r--   0        0        0      934 2024-04-01 15:23:22.983477 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/tags.py
--rw-r--r--   0        0        0     6198 2024-04-01 15:23:22.983781 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/transactions.py
--rw-r--r--   0        0        0      882 2024-04-01 15:23:22.983847 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/users.py
--rw-r--r--   0        0        0      633 2024-04-01 15:23:22.983907 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/settings.py
--rw-r--r--   0        0        0    17727 2024-04-01 15:23:22.984248 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/storage.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.984324 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/__init__.py
--rw-r--r--   0        0        0     1143 2024-04-01 15:23:22.984394 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_application.py
--rw-r--r--   0        0        0     2928 2024-04-01 15:23:22.984461 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_models_base.py
--rw-r--r--   0        0        0      829 2024-04-01 15:23:22.984528 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py
--rw-r--r--   0        0        0     1487 2024-04-01 15:23:22.984594 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py
--rw-r--r--   0        0        0      504 2024-04-01 15:23:22.984662 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_storage_usage.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.984731 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/utils/__init__.py
--rw-r--r--   0        0        0     2920 2024-04-01 15:23:22.984802 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/utils/dates.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.984861 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/utils/testing/__init__.py
--rw-r--r--   0        0        0     1884 2024-04-01 15:23:22.984930 harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/utils/testing/mixins.py
--rw-r--r--   0        0        0     1032 2024-04-01 15:23:22.985038 harp_proxy-0.5.0b3/harp_apps/telemetry/__app__.py
--rw-r--r--   0        0        0       24 2024-04-01 15:23:22.985091 harp_proxy-0.5.0b3/harp_apps/telemetry/__init__.py
--rw-r--r--   0        0        0     2735 2024-04-01 15:23:22.985158 harp_proxy-0.5.0b3/harp_apps/telemetry/manager.py
--rw-r--r--   0        0        0        0 2024-04-01 15:23:22.985215 harp_proxy-0.5.0b3/harp_apps/telemetry/tests/__init__.py
--rw-r--r--   0        0        0      160 2024-04-01 15:23:22.985288 harp_proxy-0.5.0b3/harp_apps/telemetry/tests/test_application.py
--rw-r--r--   0        0        0     1768 2024-04-01 15:23:22.985354 harp_proxy-0.5.0b3/harp_apps/telemetry/tests/test_manager.py
--rw-r--r--   0        0        0     2692 2024-04-01 15:23:22.988597 harp_proxy-0.5.0b3/pyproject.toml
--rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 harp_proxy-0.5.0b3/PKG-INFO
+-rw-r--r--   0        0        0     2001 2024-04-01 15:30:57.960268 harp_proxy-0.5.0b4/LICENSE.rst
+-rw-r--r--   0        0        0     3940 2024-04-01 15:30:57.960821 harp_proxy-0.5.0b4/README.rst
+-rw-r--r--   0        0        0     2959 2024-04-01 15:30:57.985112 harp_proxy-0.5.0b4/harp/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-01 15:30:57.985173 harp_proxy-0.5.0b4/harp/__main__.py
+-rw-r--r--   0        0        0     2871 2024-04-01 15:30:57.985238 harp_proxy-0.5.0b4/harp/_logging.py
+-rw-r--r--   0        0        0       84 2024-04-01 15:30:57.985321 harp_proxy-0.5.0b4/harp/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.985381 harp_proxy-0.5.0b4/harp/asgi/bridge/__init__.py
+-rw-r--r--   0        0        0     2874 2024-04-01 15:30:57.985463 harp_proxy-0.5.0b4/harp/asgi/bridge/requests.py
+-rw-r--r--   0        0        0     1313 2024-04-01 15:30:57.985534 harp_proxy-0.5.0b4/harp/asgi/bridge/responses.py
+-rw-r--r--   0        0        0     2072 2024-04-01 15:30:57.985612 harp_proxy-0.5.0b4/harp/asgi/events.py
+-rw-r--r--   0        0        0     6633 2024-04-01 15:30:57.985699 harp_proxy-0.5.0b4/harp/asgi/kernel.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.985775 harp_proxy-0.5.0b4/harp/asgi/tests/__init__.py
+-rw-r--r--   0        0        0     6987 2024-04-01 15:30:57.985874 harp_proxy-0.5.0b4/harp/asgi/tests/test_http_bridge_asgi_request.py
+-rw-r--r--   0        0        0     1734 2024-04-01 15:30:57.985990 harp_proxy-0.5.0b4/harp/commandline/__init__.py
+-rw-r--r--   0        0        0      352 2024-04-01 15:30:57.986063 harp_proxy-0.5.0b4/harp/commandline/install_dev.py
+-rw-r--r--   0        0        0     4305 2024-04-01 15:30:57.986141 harp_proxy-0.5.0b4/harp/commandline/start.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.986211 harp_proxy-0.5.0b4/harp/commandline/utils/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-01 15:30:57.986448 harp_proxy-0.5.0b4/harp/commandline/utils/_hacks.py
+-rw-r--r--   0        0        0     4794 2024-04-01 15:30:57.986539 harp_proxy-0.5.0b4/harp/commandline/utils/manager.py
+-rw-r--r--   0        0        0      538 2024-04-01 15:30:57.986650 harp_proxy-0.5.0b4/harp/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.986726 harp_proxy-0.5.0b4/harp/config/adapters/__init__.py
+-rw-r--r--   0        0        0      952 2024-04-01 15:30:57.986807 harp_proxy-0.5.0b4/harp/config/adapters/hypercorn.py
+-rw-r--r--   0        0        0     2398 2024-04-01 15:30:57.986881 harp_proxy-0.5.0b4/harp/config/application.py
+-rw-r--r--   0        0        0    12157 2024-04-01 15:30:57.988911 harp_proxy-0.5.0b4/harp/config/config.py
+-rw-r--r--   0        0        0     1533 2024-04-01 15:30:57.988983 harp_proxy-0.5.0b4/harp/config/events.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.989045 harp_proxy-0.5.0b4/harp/config/factories/__init__.py
+-rw-r--r--   0        0        0     4159 2024-04-01 15:30:57.989126 harp_proxy-0.5.0b4/harp/config/factories/kernel_factory.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.989183 harp_proxy-0.5.0b4/harp/config/factories/tests/__init__.py
+-rw-r--r--   0        0        0     2026 2024-04-01 15:30:57.989253 harp_proxy-0.5.0b4/harp/config/factories/tests/test_configuration.py
+-rw-r--r--   0        0        0     1385 2024-04-01 15:30:57.989313 harp_proxy-0.5.0b4/harp/config/factories/tests/test_settings.py
+-rw-r--r--   0        0        0      235 2024-04-01 15:30:57.989403 harp_proxy-0.5.0b4/harp/config/settings/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-01 15:30:57.989575 harp_proxy-0.5.0b4/harp/config/settings/base.py
+-rw-r--r--   0        0        0      256 2024-04-01 15:30:57.989648 harp_proxy-0.5.0b4/harp/config/settings/disabled.py
+-rw-r--r--   0        0        0      626 2024-04-01 15:30:57.989719 harp_proxy-0.5.0b4/harp/config/settings/from_file.py
+-rw-r--r--   0        0        0     1381 2024-04-01 15:30:57.989971 harp_proxy-0.5.0b4/harp/controllers/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-01 15:30:57.990037 harp_proxy-0.5.0b4/harp/controllers/default.py
+-rw-r--r--   0        0        0     1112 2024-04-01 15:30:57.990100 harp_proxy-0.5.0b4/harp/controllers/resolvers.py
+-rw-r--r--   0        0        0     3889 2024-04-01 15:30:57.990172 harp_proxy-0.5.0b4/harp/controllers/routing.py
+-rw-r--r--   0        0        0      156 2024-04-01 15:30:57.990440 harp_proxy-0.5.0b4/harp/controllers/typing.py
+-rw-r--r--   0        0        0      438 2024-04-01 15:30:57.990505 harp_proxy-0.5.0b4/harp/errors.py
+-rw-r--r--   0        0        0     1423 2024-04-01 15:30:57.990572 harp_proxy-0.5.0b4/harp/event_dispatcher.py
+-rw-r--r--   0        0        0      598 2024-04-01 15:30:57.990665 harp_proxy-0.5.0b4/harp/http/__init__.py
+-rw-r--r--   0        0        0      739 2024-04-01 15:30:57.990725 harp_proxy-0.5.0b4/harp/http/errors.py
+-rw-r--r--   0        0        0     3907 2024-04-01 15:30:57.990792 harp_proxy-0.5.0b4/harp/http/requests.py
+-rw-r--r--   0        0        0     1210 2024-04-01 15:30:57.990852 harp_proxy-0.5.0b4/harp/http/responses.py
+-rw-r--r--   0        0        0     3150 2024-04-01 15:30:57.990917 harp_proxy-0.5.0b4/harp/http/serializers.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.990974 harp_proxy-0.5.0b4/harp/http/tests/__init__.py
+-rw-r--r--   0        0        0     1671 2024-04-01 15:30:57.991047 harp_proxy-0.5.0b4/harp/http/tests/stubs.py
+-rw-r--r--   0        0        0     6125 2024-04-01 15:30:57.991123 harp_proxy-0.5.0b4/harp/http/tests/test_requests.py
+-rw-r--r--   0        0        0     3214 2024-04-01 15:30:57.991191 harp_proxy-0.5.0b4/harp/http/tests/test_requests_wrapped.py
+-rw-r--r--   0        0        0     3069 2024-04-01 15:30:57.991260 harp_proxy-0.5.0b4/harp/http/tests/test_utils_cookies.py
+-rw-r--r--   0        0        0      286 2024-04-01 15:30:57.991349 harp_proxy-0.5.0b4/harp/http/typing/__init__.py
+-rw-r--r--   0        0        0      847 2024-04-01 15:30:57.991773 harp_proxy-0.5.0b4/harp/http/typing/bridges.py
+-rw-r--r--   0        0        0      591 2024-04-01 15:30:57.991836 harp_proxy-0.5.0b4/harp/http/typing/messages.py
+-rw-r--r--   0        0        0      255 2024-04-01 15:30:57.991918 harp_proxy-0.5.0b4/harp/http/typing/serializers.py
+-rw-r--r--   0        0        0      123 2024-04-01 15:30:57.992013 harp_proxy-0.5.0b4/harp/http/utils/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-01 15:30:57.992141 harp_proxy-0.5.0b4/harp/http/utils/cookies.py
+-rw-r--r--   0        0        0     3913 2024-04-01 15:30:57.992236 harp_proxy-0.5.0b4/harp/http/utils/methods.py
+-rw-r--r--   0        0        0      794 2024-04-01 15:30:57.992342 harp_proxy-0.5.0b4/harp/meta/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-01 15:30:57.992459 harp_proxy-0.5.0b4/harp/models/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-01 15:30:57.992527 harp_proxy-0.5.0b4/harp/models/base.py
+-rw-r--r--   0        0        0     1732 2024-04-01 15:30:57.992598 harp_proxy-0.5.0b4/harp/models/blobs.py
+-rw-r--r--   0        0        0      274 2024-04-01 15:30:57.992663 harp_proxy-0.5.0b4/harp/models/messages.py
+-rw-r--r--   0        0        0     1065 2024-04-01 15:30:57.992954 harp_proxy-0.5.0b4/harp/models/transactions.py
+-rw-r--r--   0        0        0      365 2024-04-01 15:30:57.993055 harp_proxy-0.5.0b4/harp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.993124 harp_proxy-0.5.0b4/harp/tests/__init__.py
+-rw-r--r--   0        0        0     1684 2024-04-01 15:30:57.993214 harp_proxy-0.5.0b4/harp/tests/test_asgi_kernel.py
+-rw-r--r--   0        0        0      988 2024-04-01 15:30:57.993288 harp_proxy-0.5.0b4/harp/tests/test_settings.py
+-rw-r--r--   0        0        0      358 2024-04-01 15:30:57.993605 harp_proxy-0.5.0b4/harp/typing/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-01 15:30:57.993670 harp_proxy-0.5.0b4/harp/typing/global_settings.py
+-rw-r--r--   0        0        0      199 2024-04-01 15:30:57.993728 harp_proxy-0.5.0b4/harp/typing/signs.py
+-rw-r--r--   0        0        0     1768 2024-04-01 15:30:57.993973 harp_proxy-0.5.0b4/harp/typing/storage.py
+-rw-r--r--   0        0        0      266 2024-04-01 15:30:57.994108 harp_proxy-0.5.0b4/harp/utils/__init__.py
+-rw-r--r--   0        0        0      443 2024-04-01 15:30:57.994372 harp_proxy-0.5.0b4/harp/utils/apdex.py
+-rw-r--r--   0        0        0      278 2024-04-01 15:30:57.994433 harp_proxy-0.5.0b4/harp/utils/arguments.py
+-rw-r--r--   0        0        0     1055 2024-04-01 15:30:57.994497 harp_proxy-0.5.0b4/harp/utils/background.py
+-rw-r--r--   0        0        0      188 2024-04-01 15:30:57.994559 harp_proxy-0.5.0b4/harp/utils/bytes.py
+-rw-r--r--   0        0        0     2082 2024-04-01 15:30:57.994629 harp_proxy-0.5.0b4/harp/utils/collections.py
+-rw-r--r--   0        0        0      739 2024-04-01 15:30:57.994812 harp_proxy-0.5.0b4/harp/utils/dates.py
+-rw-r--r--   0        0        0       94 2024-04-01 15:30:57.994874 harp_proxy-0.5.0b4/harp/utils/guids.py
+-rw-r--r--   0        0        0      102 2024-04-01 15:30:57.994934 harp_proxy-0.5.0b4/harp/utils/identifiers.py
+-rw-r--r--   0        0        0      200 2024-04-01 15:30:57.994995 harp_proxy-0.5.0b4/harp/utils/json.py
+-rw-r--r--   0        0        0     1273 2024-04-01 15:30:57.995060 harp_proxy-0.5.0b4/harp/utils/network.py
+-rw-r--r--   0        0        0      330 2024-04-01 15:30:57.995127 harp_proxy-0.5.0b4/harp/utils/processes.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.995187 harp_proxy-0.5.0b4/harp/utils/testing/__init__.py
+-rw-r--r--   0        0        0      943 2024-04-01 15:30:57.995261 harp_proxy-0.5.0b4/harp/utils/testing/applications.py
+-rw-r--r--   0        0        0     2958 2024-04-01 15:30:57.995335 harp_proxy-0.5.0b4/harp/utils/testing/benchmarking.py
+-rw-r--r--   0        0        0      217 2024-04-01 15:30:57.995432 harp_proxy-0.5.0b4/harp/utils/testing/communicators/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-01 15:30:57.995499 harp_proxy-0.5.0b4/harp/utils/testing/communicators/asgi.py
+-rw-r--r--   0        0        0     2150 2024-04-01 15:30:57.995564 harp_proxy-0.5.0b4/harp/utils/testing/communicators/http.py
+-rw-r--r--   0        0        0     4572 2024-04-01 15:30:57.995629 harp_proxy-0.5.0b4/harp/utils/testing/http.py
+-rw-r--r--   0        0        0      177 2024-04-01 15:30:57.995715 harp_proxy-0.5.0b4/harp/utils/testing/mixins/__init__.py
+-rw-r--r--   0        0        0     2264 2024-04-01 15:30:57.995784 harp_proxy-0.5.0b4/harp/utils/testing/mixins/controllers.py
+-rw-r--r--   0        0        0      874 2024-04-01 15:30:57.995878 harp_proxy-0.5.0b4/harp/utils/testing/stub_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:57.995939 harp_proxy-0.5.0b4/harp/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-01 15:30:57.996010 harp_proxy-0.5.0b4/harp/utils/tests/test_collections.py
+-rw-r--r--   0        0        0      691 2024-04-01 15:30:57.996068 harp_proxy-0.5.0b4/harp/utils/tests/test_dates.py
+-rw-r--r--   0        0        0      261 2024-04-01 15:30:57.996127 harp_proxy-0.5.0b4/harp/utils/tests/test_urls.py
+-rw-r--r--   0        0        0      106 2024-04-01 15:30:57.996185 harp_proxy-0.5.0b4/harp/utils/urls.py
+-rw-r--r--   0        0        0      261 2024-04-01 15:30:57.996280 harp_proxy-0.5.0b4/harp/views/__init__.py
+-rw-r--r--   0        0        0     1745 2024-04-01 15:30:57.996571 harp_proxy-0.5.0b4/harp/views/json.py
+-rw-r--r--   0        0        0      409 2024-04-01 15:30:57.996634 harp_proxy-0.5.0b4/harp/views/strings.py
+-rw-r--r--   0        0        0       19 2024-04-01 15:30:57.996732 harp_proxy-0.5.0b4/harp_apps/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-01 15:30:57.996822 harp_proxy-0.5.0b4/harp_apps/contrib/__init__.py
+-rw-r--r--   0        0        0      728 2024-04-01 15:30:57.996918 harp_proxy-0.5.0b4/harp_apps/contrib/sentry/__app__.py
+-rw-r--r--   0        0        0       21 2024-04-01 15:30:57.996974 harp_proxy-0.5.0b4/harp_apps/contrib/sentry/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-01 15:30:57.997029 harp_proxy-0.5.0b4/harp_apps/contrib/sentry/settings.py
+-rw-r--r--   0        0        0     1248 2024-04-01 15:30:57.997122 harp_proxy-0.5.0b4/harp_apps/dashboard/__app__.py
+-rw-r--r--   0        0        0       24 2024-04-01 15:30:57.997180 harp_proxy-0.5.0b4/harp_apps/dashboard/__init__.py
+-rw-r--r--   0        0        0     5503 2024-04-01 15:30:57.997320 harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-01 15:30:57.997402 harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/blobs.py
+-rw-r--r--   0        0        0     4732 2024-04-01 15:30:57.997711 harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/overview.py
+-rw-r--r--   0        0        0     2757 2024-04-01 15:30:57.997790 harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/system.py
+-rw-r--r--   0        0        0     3407 2024-04-01 15:30:57.997868 harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/transactions.py
+-rw-r--r--   0        0        0      450 2024-04-01 15:30:57.998156 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/development/index.rst
+-rw-r--r--   0        0        0     5487 2024-04-01 15:30:57.998249 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/development/tests_e2e.rst
+-rw-r--r--   0        0        0     6937 2024-04-01 15:30:57.998334 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/development/tests_unit.rst
+-rw-r--r--   0        0        0      179 2024-04-01 15:30:57.998435 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/examples/auth.basic.yml
+-rw-r--r--   0        0        0       99 2024-04-01 15:30:57.998494 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/examples/auth.yml
+-rw-r--r--   0        0        0      125 2024-04-01 15:30:57.998554 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/examples/devserver.yml
+-rw-r--r--   0        0        0      146 2024-04-01 15:30:57.998611 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/examples/main.yml
+-rw-r--r--   0        0        0     2140 2024-04-01 15:30:57.998681 harp_proxy-0.5.0b4/harp_apps/dashboard/docs/index.rst
+-rw-r--r--   0        0        0      421 2024-04-01 15:30:57.998912 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/__init__.py
+-rw-r--r--   0        0        0      817 2024-04-01 15:30:57.998989 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/base.py
+-rw-r--r--   0        0        0      717 2024-04-01 15:30:57.999055 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/transaction_endpoint.py
+-rw-r--r--   0        0        0      122 2024-04-01 15:30:57.999117 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/transaction_flag.py
+-rw-r--r--   0        0        0      155 2024-04-01 15:30:57.999178 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/transaction_method.py
+-rw-r--r--   0        0        0      142 2024-04-01 15:30:57.999241 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/transaction_status.py
+-rw-r--r--   0        0        0      168 2024-04-01 15:30:57.999304 harp_proxy-0.5.0b4/harp_apps/dashboard/filters/utils.py
+-rw-r--r--   0        0        0     1236 2024-04-01 15:30:57.999415 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      341 2024-04-01 15:30:57.999688 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/.gitignore
+-rw-r--r--   0        0        0      268 2024-04-01 15:30:57.999787 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/.ladle/components.tsx
+-rw-r--r--   0        0        0       59 2024-04-01 15:30:57.999946 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/.ladle/index.css
+-rw-r--r--   0        0        0      188 2024-04-01 15:30:58.000173 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/.prettierrc
+-rw-r--r--   0        0        0      357 2024-04-01 15:30:58.000237 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/index.html
+-rw-r--r--   0        0        0     7672 2024-04-01 15:30:58.000326 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/mockServiceWorker.js
+-rw-r--r--   0        0        0     3803 2024-04-01 15:30:58.000598 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/package.json
+-rw-r--r--   0        0        0     2155 2024-04-01 15:30:58.000666 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/playwright.config.ts
+-rw-r--r--   0        0        0   272272 2024-04-01 15:30:58.002224 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       81 2024-04-01 15:30:58.002336 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/postcss.config.js
+-rw-r--r--   0        0        0     2519 2024-04-01 15:30:58.002439 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/public/harp.svg
+-rw-r--r--   0        0        0     2726 2024-04-01 15:30:58.002578 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Assets/logo.svg
+-rw-r--r--   0        0        0      808 2024-04-01 15:30:58.002933 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/ApdexBadge.tsx
+-rw-r--r--   0        0        0      588 2024-04-01 15:30:58.003111 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/RequestMethodBadge.tsx
+-rw-r--r--   0        0        0      877 2024-04-01 15:30:58.003177 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/ResponseStatusBadge.tsx
+-rw-r--r--   0        0        0      766 2024-04-01 15:30:58.003438 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/StyledJumboBadge.tsx
+-rw-r--r--   0        0        0      616 2024-04-01 15:30:58.003690 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/constants.ts
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.003724 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/index.ts
+-rw-r--r--   0        0        0      444 2024-04-01 15:30:58.003827 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Layout/Layout.test.tsx
+-rw-r--r--   0        0        0     1901 2024-04-01 15:30:58.004112 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Layout/Layout.tsx
+-rw-r--r--   0        0        0     5132 2024-04-01 15:30:58.004415 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Layout/__snapshots__/Layout.test.tsx.snap
+-rw-r--r--   0        0        0       49 2024-04-01 15:30:58.004471 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Layout/index.ts
+-rw-r--r--   0        0        0     1369 2024-04-01 15:30:58.004563 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/Page.test.tsx
+-rw-r--r--   0        0        0     1749 2024-04-01 15:30:58.004632 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/Page.tsx
+-rw-r--r--   0        0        0      562 2024-04-01 15:30:58.004795 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/PageTitle.tsx
+-rw-r--r--   0        0        0      695 2024-04-01 15:30:58.004968 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/__snapshots__/Page.test.tsx.snap
+-rw-r--r--   0        0        0      101 2024-04-01 15:30:58.005035 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/index.tsx
+-rw-r--r--   0        0        0     1452 2024-04-01 15:30:58.005151 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Utilities/OnQuerySuccess.tsx
+-rw-r--r--   0        0        0       46 2024-04-01 15:30:58.005318 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Api/Types/ItemList.ts
+-rw-r--r--   0        0        0       43 2024-04-01 15:30:58.005379 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Api/Types/index.ts
+-rw-r--r--   0        0        0       37 2024-04-01 15:30:58.005436 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Api/index.ts
+-rw-r--r--   0        0        0     1246 2024-04-01 15:30:58.005517 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Api/useApi.ts
+-rw-r--r--   0        0        0       62 2024-04-01 15:30:58.005732 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Overview/index.ts
+-rw-r--r--   0        0        0      651 2024-04-01 15:30:58.006117 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Overview/useOverviewDataQuery.ts
+-rw-r--r--   0        0        0      491 2024-04-01 15:30:58.006371 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Overview/useSummaryDataQuery.tsx
+-rw-r--r--   0        0        0      266 2024-04-01 15:30:58.006461 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/System/index.ts
+-rw-r--r--   0        0        0      293 2024-04-01 15:30:58.006520 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/System/useSystemDependenciesQuery.ts
+-rw-r--r--   0        0        0      290 2024-04-01 15:30:58.006579 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/System/useSystemQuery.ts
+-rw-r--r--   0        0        0      420 2024-04-01 15:30:58.007025 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/System/useSystemSettingsQuery.ts
+-rw-r--r--   0        0        0      243 2024-04-01 15:30:58.007115 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/System/useSystemStorageQuery.ts
+-rw-r--r--   0        0        0      372 2024-04-01 15:30:58.007254 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/Utils/getRequestFromTransactionMessages.tsx
+-rw-r--r--   0        0        0      493 2024-04-01 15:30:58.007433 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/Utils/getResponseFromTransactionMessages.tsx
+-rw-r--r--   0        0        0      186 2024-04-01 15:30:58.007501 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/Utils/index.ts
+-rw-r--r--   0        0        0      298 2024-04-01 15:30:58.007566 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/index.ts
+-rw-r--r--   0        0        0      544 2024-04-01 15:30:58.008684 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useBlobQuery.ts
+-rw-r--r--   0        0        0      448 2024-04-01 15:30:58.008754 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useSetUserFlagMutation.ts
+-rw-r--r--   0        0        0      371 2024-04-01 15:30:58.008817 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsDetailQuery.ts
+-rw-r--r--   0        0        0      439 2024-04-01 15:30:58.008881 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsFiltersQuery.ts
+-rw-r--r--   0        0        0     1213 2024-04-01 15:30:58.009463 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsListQuery.ts
+-rw-r--r--   0        0        0      323 2024-04-01 15:30:58.010001 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Models/Overview.d.ts
+-rw-r--r--   0        0        0     1851 2024-04-01 15:30:58.010256 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Models/Schemas/Transaction.json
+-rw-r--r--   0        0        0     1142 2024-04-01 15:30:58.010511 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Models/Transaction.d.ts
+-rw-r--r--   0        0        0      586 2024-04-01 15:30:58.010838 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.test.tsx
+-rw-r--r--   0        0        0     1379 2024-04-01 15:30:58.011098 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.tsx
+-rw-r--r--   0        0        0     1589 2024-04-01 15:30:58.011201 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.test.tsx
+-rw-r--r--   0        0        0     3056 2024-04-01 15:30:58.011472 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.tsx
+-rw-r--r--   0        0        0    12406 2024-04-01 15:30:58.011751 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/__snapshots__/TransactionsChart.test.tsx.snap
+-rw-r--r--   0        0        0       56 2024-04-01 15:30:58.012001 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/index.ts
+-rw-r--r--   0        0        0      615 2024-04-01 15:30:58.012266 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/PerformancesSummary.tsx
+-rw-r--r--   0        0        0      890 2024-04-01 15:30:58.012487 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/RateSummary.tsx
+-rw-r--r--   0        0        0     1184 2024-04-01 15:30:58.012802 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/__snapshots__/BaseTransactionsOverview.test.tsx.snap
+-rw-r--r--   0        0        0       70 2024-04-01 15:30:58.012863 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/index.ts
+-rw-r--r--   0        0        0      620 2024-04-01 15:30:58.012960 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.test.tsx
+-rw-r--r--   0        0        0      700 2024-04-01 15:30:58.013020 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.tsx
+-rw-r--r--   0        0        0     1220 2024-04-01 15:30:58.013258 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/__snapshots__/TransactionsOverview.test.tsx.snap
+-rw-r--r--   0        0        0       62 2024-04-01 15:30:58.013317 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/index.ts
+-rw-r--r--   0        0        0      348 2024-04-01 15:30:58.013386 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/OverviewPage.test.tsx
+-rw-r--r--   0        0        0     3785 2024-04-01 15:30:58.013639 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/OverviewPage.tsx
+-rw-r--r--   0        0        0    30379 2024-04-01 15:30:58.013981 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/__snapshots__/OverviewPage.test.tsx.snap
+-rw-r--r--   0        0        0       50 2024-04-01 15:30:58.014055 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/index.ts
+-rw-r--r--   0        0        0      103 2024-04-01 15:30:58.014246 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/utils.ts
+-rw-r--r--   0        0        0     1596 2024-04-01 15:30:58.014379 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.test.tsx
+-rw-r--r--   0        0        0     1558 2024-04-01 15:30:58.014445 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.tsx
+-rw-r--r--   0        0        0      945 2024-04-01 15:30:58.014541 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.test.tsx
+-rw-r--r--   0        0        0     2287 2024-04-01 15:30:58.014613 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.tsx
+-rw-r--r--   0        0        0       38 2024-04-01 15:30:58.014675 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/index.ts
+-rw-r--r--   0        0        0       52 2024-04-01 15:30:58.014743 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/index.ts
+-rw-r--r--   0        0        0      636 2024-04-01 15:30:58.014809 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.test.tsx
+-rw-r--r--   0        0        0      651 2024-04-01 15:30:58.014883 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.tsx
+-rw-r--r--   0        0        0      839 2024-04-01 15:30:58.014945 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.test.tsx
+-rw-r--r--   0        0        0      828 2024-04-01 15:30:58.015197 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.tsx
+-rw-r--r--   0        0        0      628 2024-04-01 15:30:58.015258 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.test.tsx
+-rw-r--r--   0        0        0      596 2024-04-01 15:30:58.015312 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.tsx
+-rw-r--r--   0        0        0      718 2024-04-01 15:30:58.015377 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemStorageTabPanel.tsx
+-rw-r--r--   0        0        0      628 2024-04-01 15:30:58.015439 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.test.tsx
+-rw-r--r--   0        0        0      993 2024-04-01 15:30:58.015498 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.tsx
+-rw-r--r--   0        0        0     2196 2024-04-01 15:30:58.015744 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemDependenciesTabPanel.test.tsx.snap
+-rw-r--r--   0        0        0    13743 2024-04-01 15:30:58.016021 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemPage.test.tsx.snap
+-rw-r--r--   0        0        0     8798 2024-04-01 15:30:58.016082 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemSettingsTabPanel.test.tsx.snap
+-rw-r--r--   0        0        0     2957 2024-04-01 15:30:58.016147 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemTopologyTabPanel.test.tsx.snap
+-rw-r--r--   0        0        0       46 2024-04-01 15:30:58.016202 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/index.ts
+-rw-r--r--   0        0        0     1338 2024-04-01 15:30:58.016345 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Buttons.tsx
+-rw-r--r--   0        0        0      355 2024-04-01 15:30:58.016440 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/Facet.test.tsx
+-rw-r--r--   0        0        0     3205 2024-04-01 15:30:58.016508 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/Facet.tsx
+-rw-r--r--   0        0        0      417 2024-04-01 15:30:58.016570 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetInnerLightButton.test.tsx
+-rw-r--r--   0        0        0      397 2024-04-01 15:30:58.016630 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetInnerLightButton.tsx
+-rw-r--r--   0        0        0      324 2024-04-01 15:30:58.016691 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetLabel.test.tsx
+-rw-r--r--   0        0        0      378 2024-04-01 15:30:58.016753 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/FacetLabel.tsx
+-rw-r--r--   0        0        0      893 2024-04-01 15:30:58.016864 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/Facet.test.tsx.snap
+-rw-r--r--   0        0        0      230 2024-04-01 15:30:58.016933 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/FacetInnerLightButton.test.tsx.snap
+-rw-r--r--   0        0        0      159 2024-04-01 15:30:58.016997 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/FacetLabel.test.tsx.snap
+-rw-r--r--   0        0        0       74 2024-04-01 15:30:58.017055 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/index.ts
+-rw-r--r--   0        0        0     1162 2024-04-01 15:30:58.017124 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Foldable.tsx
+-rw-r--r--   0        0        0     2300 2024-04-01 15:30:58.017245 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.test.tsx
+-rw-r--r--   0        0        0     3634 2024-04-01 15:30:58.017539 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.tsx
+-rw-r--r--   0        0        0       62 2024-04-01 15:30:58.017711 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/index.ts
+-rw-r--r--   0        0        0      493 2024-04-01 15:30:58.017951 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageBody.tsx
+-rw-r--r--   0        0        0      866 2024-04-01 15:30:58.018122 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageHeaders.tsx
+-rw-r--r--   0        0        0     1258 2024-04-01 15:30:58.018188 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageSummary.tsx
+-rw-r--r--   0        0        0      517 2024-04-01 15:30:58.018267 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/OptionalPaginator.tsx
+-rw-r--r--   0        0        0     1819 2024-04-01 15:30:58.018499 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/PrettyBody.tsx
+-rw-r--r--   0        0        0      546 2024-04-01 15:30:58.018643 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/__snapshots__/HeadersTable.test.tsx.snap
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.018683 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/index.ts
+-rw-r--r--   0        0        0      623 2024-04-01 15:30:58.018811 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.test.tsx
+-rw-r--r--   0        0        0     2995 2024-04-01 15:30:58.018901 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.tsx
+-rw-r--r--   0        0        0    16323 2024-04-01 15:30:58.019209 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/__snapshots__/FiltersSidebar.test.tsx.snap
+-rw-r--r--   0        0        0       50 2024-04-01 15:30:58.019275 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/index.ts
+-rw-r--r--   0        0        0     1729 2024-04-01 15:30:58.019364 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailOnQuerySuccess.tsx
+-rw-r--r--   0        0        0      618 2024-04-01 15:30:58.019441 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.test.tsx
+-rw-r--r--   0        0        0      665 2024-04-01 15:30:58.019527 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.tsx
+-rw-r--r--   0        0        0     2639 2024-04-01 15:30:58.019612 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListOnQuerySuccess.tsx
+-rw-r--r--   0        0        0      460 2024-04-01 15:30:58.019683 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListPage.test.tsx
+-rw-r--r--   0        0        0     2217 2024-04-01 15:30:58.019772 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListPage.tsx
+-rw-r--r--   0        0        0    10800 2024-04-01 15:30:58.020070 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionListPage.test.tsx.snap
+-rw-r--r--   0        0        0    10564 2024-04-01 15:30:58.020207 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsDetailPage.test.tsx.snap
+-rw-r--r--   0        0        0    13658 2024-04-01 15:30:58.020342 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsListPage.test.tsx.snap
+-rw-r--r--   0        0        0      132 2024-04-01 15:30:58.020420 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/index.ts
+-rw-r--r--   0        0        0      365 2024-04-01 15:30:58.020579 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Styles/GlobalStyles.tsx
+-rw-r--r--   0        0        0      176 2024-04-01 15:30:58.020692 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Types/filters.d.ts
+-rw-r--r--   0        0        0      441 2024-04-01 15:30:58.020841 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Utils/Strings.ts
+-rw-r--r--   0        0        0      125 2024-04-01 15:30:58.020908 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/index.css
+-rw-r--r--   0        0        0     1987 2024-04-01 15:30:58.020986 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/main.tsx
+-rw-r--r--   0        0        0      102 2024-04-01 15:30:58.021378 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/api/index.ts
+-rw-r--r--   0        0        0      542 2024-04-01 15:30:58.021819 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/api/overview.ts
+-rw-r--r--   0        0        0      687 2024-04-01 15:30:58.022094 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/api/summary.ts
+-rw-r--r--   0        0        0      201 2024-04-01 15:30:58.022174 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/browser.ts
+-rw-r--r--   0        0        0     4644 2024-04-01 15:30:58.022473 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/handlers.ts
+-rw-r--r--   0        0        0      126 2024-04-01 15:30:58.022541 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/node.ts
+-rw-r--r--   0        0        0      889 2024-04-01 15:30:58.022622 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/utils.tsx
+-rw-r--r--   0        0        0      683 2024-04-01 15:30:58.022947 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.stories.tsx
+-rw-r--r--   0        0        0      492 2024-04-01 15:30:58.023039 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.test.tsx
+-rw-r--r--   0        0        0      875 2024-04-01 15:30:58.023115 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.tsx
+-rw-r--r--   0        0        0      200 2024-04-01 15:30:58.023253 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/__snapshots__/Badge.test.tsx.snap
+-rw-r--r--   0        0        0       49 2024-04-01 15:30:58.023323 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/index.ts
+-rw-r--r--   0        0        0      303 2024-04-01 15:30:58.023434 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.stories.tsx
+-rw-r--r--   0        0        0      675 2024-04-01 15:30:58.023510 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.test.tsx
+-rw-r--r--   0        0        0     1084 2024-04-01 15:30:58.023581 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.tsx
+-rw-r--r--   0        0        0      189 2024-04-01 15:30:58.023707 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/__snapshots__/Button.test.tsx.snap
+-rw-r--r--   0        0        0       34 2024-04-01 15:30:58.023783 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/index.ts
+-rw-r--r--   0        0        0      564 2024-04-01 15:30:58.023918 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.stories.tsx
+-rw-r--r--   0        0        0     1242 2024-04-01 15:30:58.023990 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.test.tsx
+-rw-r--r--   0        0        0     1180 2024-04-01 15:30:58.024057 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.tsx
+-rw-r--r--   0        0        0      481 2024-04-01 15:30:58.024154 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/__snapshots__/ButtonGroup.test.tsx.snap
+-rw-r--r--   0        0        0       44 2024-04-01 15:30:58.024217 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/index.ts
+-rw-r--r--   0        0        0      723 2024-04-01 15:30:58.024338 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.stories.tsx
+-rw-r--r--   0        0        0     4620 2024-04-01 15:30:58.024429 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.test.tsx
+-rw-r--r--   0        0        0     3528 2024-04-01 15:30:58.024509 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.tsx
+-rw-r--r--   0        0        0     2393 2024-04-01 15:30:58.024628 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/__snapshots__/DataTable.test.tsx.snap
+-rw-r--r--   0        0        0       53 2024-04-01 15:30:58.024702 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/index.ts
+-rw-r--r--   0        0        0     1990 2024-04-01 15:30:58.024813 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.test.tsx
+-rw-r--r--   0        0        0     1934 2024-04-01 15:30:58.024895 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.tsx
+-rw-r--r--   0        0        0     1864 2024-04-01 15:30:58.024969 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/FormWidgets.stories.tsx
+-rw-r--r--   0        0        0     1365 2024-04-01 15:30:58.025040 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.test.tsx
+-rw-r--r--   0        0        0      737 2024-04-01 15:30:58.025111 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.tsx
+-rw-r--r--   0        0        0      672 2024-04-01 15:30:58.025241 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/__snapshots__/Checkbox.test.tsx.snap
+-rw-r--r--   0        0        0      492 2024-04-01 15:30:58.025349 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/__snapshots__/Radio.test.tsx.snap
+-rw-r--r--   0        0        0       70 2024-04-01 15:30:58.025412 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/index.ts
+-rw-r--r--   0        0        0      947 2024-04-01 15:30:58.025544 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Assets/logo.svg
+-rw-r--r--   0        0        0      253 2024-04-01 15:30:58.025605 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.stories.tsx
+-rw-r--r--   0        0        0     1235 2024-04-01 15:30:58.025682 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.test.tsx
+-rw-r--r--   0        0        0     3938 2024-04-01 15:30:58.025763 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.tsx
+-rw-r--r--   0        0        0     2349 2024-04-01 15:30:58.025903 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/__snapshots__/Navbar.test.tsx.snap
+-rw-r--r--   0        0        0       34 2024-04-01 15:30:58.025961 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/index.ts
+-rw-r--r--   0        0        0      523 2024-04-01 15:30:58.026066 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Pagination.stories.tsx
+-rw-r--r--   0        0        0     1925 2024-04-01 15:30:58.026244 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.test.tsx
+-rw-r--r--   0        0        0     4971 2024-04-01 15:30:58.026331 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.tsx
+-rw-r--r--   0        0        0     4947 2024-04-01 15:30:58.026488 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/__snapshots__/Paginator.test.tsx.snap
+-rw-r--r--   0        0        0       40 2024-04-01 15:30:58.026661 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/index.ts
+-rw-r--r--   0        0        0     2234 2024-04-01 15:30:58.026801 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.stories.tsx
+-rw-r--r--   0        0        0      412 2024-04-01 15:30:58.026955 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.test.tsx
+-rw-r--r--   0        0        0      381 2024-04-01 15:30:58.027022 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.tsx
+-rw-r--r--   0        0        0      157 2024-04-01 15:30:58.027166 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pane/__snapshots__/Pane.test.tsx.snap
+-rw-r--r--   0        0        0       30 2024-04-01 15:30:58.027230 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pane/index.ts
+-rw-r--r--   0        0        0      163 2024-04-01 15:30:58.027479 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.stories.tsx
+-rw-r--r--   0        0        0      296 2024-04-01 15:30:58.027547 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.test.tsx
+-rw-r--r--   0        0        0     1620 2024-04-01 15:30:58.027619 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.tsx
+-rw-r--r--   0        0        0      783 2024-04-01 15:30:58.027732 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/__snapshots__/SearchBar.test.tsx.snap
+-rw-r--r--   0        0        0       40 2024-04-01 15:30:58.027795 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/index.ts
+-rw-r--r--   0        0        0     5048 2024-04-01 15:30:58.027956 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.stories.tsx
+-rw-r--r--   0        0        0     1162 2024-04-01 15:30:58.028029 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.test.tsx
+-rw-r--r--   0        0        0     1135 2024-04-01 15:30:58.028099 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.tsx
+-rw-r--r--   0        0        0      870 2024-04-01 15:30:58.028233 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/__snapshots__/Tabs.test.tsx.snap
+-rw-r--r--   0        0        0       29 2024-04-01 15:30:58.028295 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/index.ts
+-rw-r--r--   0        0        0      109 2024-04-01 15:30:58.028391 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/Paragraphs.ts
+-rw-r--r--   0        0        0       97 2024-04-01 15:30:58.028446 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/Section.ts
+-rw-r--r--   0        0        0      627 2024-04-01 15:30:58.028504 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/Titles.ts
+-rw-r--r--   0        0        0     1248 2024-04-01 15:30:58.028571 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/Typography.stories.tsx
+-rw-r--r--   0        0        0      119 2024-04-01 15:30:58.028628 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/index.ts
+-rw-r--r--   0        0        0      120 2024-04-01 15:30:58.028864 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Utilities/index.ts
+-rw-r--r--   0        0        0      388 2024-04-01 15:30:58.029038 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/playwright.config.ts
+-rw-r--r--   0        0        0     1207 2024-04-01 15:30:58.029133 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts
+-rw-r--r--   0        0        0    15116 2024-04-01 15:30:58.029264 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/badge--default-darwin.png
+-rw-r--r--   0        0        0     8638 2024-04-01 15:30:58.029343 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--default-darwin.png
+-rw-r--r--   0        0        0     6157 2024-04-01 15:30:58.029533 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--primary-darwin.png
+-rw-r--r--   0        0        0     6204 2024-04-01 15:30:58.029601 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--secondary-darwin.png
+-rw-r--r--   0        0        0     7137 2024-04-01 15:30:58.029813 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button-group--button-group-darwin.png
+-rw-r--r--   0        0        0    22924 2024-04-01 15:30:58.030086 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/data-table--default-darwin.png
+-rw-r--r--   0        0        0    22499 2024-04-01 15:30:58.030265 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-darwin.png
+-rw-r--r--   0        0        0    27926 2024-04-01 15:30:58.030475 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-with-style-darwin.png
+-rw-r--r--   0        0        0    25968 2024-04-01 15:30:58.030679 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--radios-darwin.png
+-rw-r--r--   0        0        0     8570 2024-04-01 15:30:58.030791 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/navbar--default-darwin.png
+-rw-r--r--   0        0        0    20836 2024-04-01 15:30:58.030979 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pagination--paginator-darwin.png
+-rw-r--r--   0        0        0   121076 2024-04-01 15:30:58.031817 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pane--default-darwin.png
+-rw-r--r--   0        0        0     8281 2024-04-01 15:30:58.031915 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/search-bar--default-darwin.png
+-rw-r--r--   0        0        0   200590 2024-04-01 15:30:58.033174 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/tabs--default-darwin.png
+-rw-r--r--   0        0        0    23837 2024-04-01 15:30:58.033372 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-darwin.png
+-rw-r--r--   0        0        0    44912 2024-04-01 15:30:58.033708 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-with-paragraphs-darwin.png
+-rw-r--r--   0        0        0       38 2024-04-01 15:30:58.035233 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0     1479 2024-04-01 15:30:58.035312 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tailwind.config.js
+-rw-r--r--   0        0        0      196 2024-04-01 15:30:58.035412 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tests/overviewPage.spec.ts
+-rw-r--r--   0        0        0     1034 2024-04-01 15:30:58.035482 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tests/systemDependenciesPage.spec.ts
+-rw-r--r--   0        0        0     1147 2024-04-01 15:30:58.035575 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tests/transactionsPage.spec.ts
+-rw-r--r--   0        0        0      755 2024-04-01 15:30:58.035655 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-04-01 15:30:58.035725 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      485 2024-04-01 15:30:58.035815 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/types/twin.d.ts
+-rw-r--r--   0        0        0     2682 2024-04-01 15:30:58.035884 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/vite.config.ts
+-rw-r--r--   0        0        0      725 2024-04-01 15:30:58.035944 harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/vitest.setup.ts
+-rw-r--r--   0        0        0       90 2024-04-01 15:30:58.036036 harp_proxy-0.5.0b4/harp_apps/dashboard/schemas/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-01 15:30:58.036093 harp_proxy-0.5.0b4/harp_apps/dashboard/schemas/transactions_grouped_by.py
+-rw-r--r--   0        0        0     3547 2024-04-01 15:30:58.036164 harp_proxy-0.5.0b4/harp_apps/dashboard/settings.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.036228 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/__init__.py
+-rw-r--r--   0        0        0     1752 2024-04-01 15:30:58.036296 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_controllers_blobs.py
+-rw-r--r--   0        0        0     2402 2024-04-01 15:30:58.036366 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_controllers_transactions.py
+-rw-r--r--   0        0        0      967 2024-04-01 15:30:58.036427 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_settings.py
+-rw-r--r--   0        0        0     4039 2024-04-01 15:30:58.036494 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_utils_dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.036551 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3101 2024-04-01 15:30:58.036618 harp_proxy-0.5.0b4/harp_apps/dashboard/tests/utils/test_dates.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.036677 harp_proxy-0.5.0b4/harp_apps/dashboard/utils/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-01 15:30:58.036970 harp_proxy-0.5.0b4/harp_apps/dashboard/utils/dates.py
+-rw-r--r--   0        0        0     1061 2024-04-01 15:30:58.037040 harp_proxy-0.5.0b4/harp_apps/dashboard/utils/dependencies.py
+-rw-r--r--   0        0        0      653 2024-04-01 15:30:58.037136 harp_proxy-0.5.0b4/harp_apps/http_client/__app__.py
+-rw-r--r--   0        0        0       26 2024-04-01 15:30:58.037190 harp_proxy-0.5.0b4/harp_apps/http_client/__init__.py
+-rw-r--r--   0        0        0      555 2024-04-01 15:30:58.037289 harp_proxy-0.5.0b4/harp_apps/janitor/__app__.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.037317 harp_proxy-0.5.0b4/harp_apps/janitor/__init__.py
+-rw-r--r--   0        0        0      186 2024-04-01 15:30:58.037379 harp_proxy-0.5.0b4/harp_apps/janitor/settings.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.037437 harp_proxy-0.5.0b4/harp_apps/janitor/tests/__init__.py
+-rw-r--r--   0        0        0     3505 2024-04-01 15:30:58.037511 harp_proxy-0.5.0b4/harp_apps/janitor/tests/test_worker.py
+-rw-r--r--   0        0        0     3911 2024-04-01 15:30:58.037584 harp_proxy-0.5.0b4/harp_apps/janitor/worker.py
+-rw-r--r--   0        0        0     1023 2024-04-01 15:30:58.037892 harp_proxy-0.5.0b4/harp_apps/proxy/__app__.py
+-rw-r--r--   0        0        0       20 2024-04-01 15:30:58.037948 harp_proxy-0.5.0b4/harp_apps/proxy/__init__.py
+-rw-r--r--   0        0        0     7425 2024-04-01 15:30:58.038236 harp_proxy-0.5.0b4/harp_apps/proxy/controllers.py
+-rw-r--r--   0        0        0       88 2024-04-01 15:30:58.038487 harp_proxy-0.5.0b4/harp_apps/proxy/docs/examples/swapi.yml
+-rw-r--r--   0        0        0      862 2024-04-01 15:30:58.038548 harp_proxy-0.5.0b4/harp_apps/proxy/docs/index.rst
+-rw-r--r--   0        0        0      164 2024-04-01 15:30:58.038601 harp_proxy-0.5.0b4/harp_apps/proxy/events.py
+-rw-r--r--   0        0        0      633 2024-04-01 15:30:58.038662 harp_proxy-0.5.0b4/harp_apps/proxy/settings.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.038722 harp_proxy-0.5.0b4/harp_apps/proxy/tests/__init__.py
+-rw-r--r--   0        0        0     8497 2024-04-01 15:30:58.039018 harp_proxy-0.5.0b4/harp_apps/proxy/tests/test_controllers_http_proxy.py
+-rw-r--r--   0        0        0     1061 2024-04-01 15:30:58.039121 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/__app__.py
+-rw-r--r--   0        0        0       33 2024-04-01 15:30:58.039176 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-01 15:30:58.039228 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/constants.py
+-rw-r--r--   0        0        0     1033 2024-04-01 15:30:58.039322 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/docs/index.rst
+-rw-r--r--   0        0        0      877 2024-04-01 15:30:58.039415 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-01 15:30:58.039484 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/base.py
+-rw-r--r--   0        0        0     1928 2024-04-01 15:30:58.039545 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/blobs.py
+-rw-r--r--   0        0        0     1082 2024-04-01 15:30:58.039602 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/flags.py
+-rw-r--r--   0        0        0     2413 2024-04-01 15:30:58.039666 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/messages.py
+-rw-r--r--   0        0        0     1425 2024-04-01 15:30:58.039726 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/metrics.py
+-rw-r--r--   0        0        0      934 2024-04-01 15:30:58.039782 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/tags.py
+-rw-r--r--   0        0        0     6198 2024-04-01 15:30:58.040021 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/transactions.py
+-rw-r--r--   0        0        0      882 2024-04-01 15:30:58.040084 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/users.py
+-rw-r--r--   0        0        0      633 2024-04-01 15:30:58.040145 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/settings.py
+-rw-r--r--   0        0        0    17727 2024-04-01 15:30:58.040494 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/storage.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.040567 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/__init__.py
+-rw-r--r--   0        0        0     1143 2024-04-01 15:30:58.040754 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_application.py
+-rw-r--r--   0        0        0     2928 2024-04-01 15:30:58.040819 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_models_base.py
+-rw-r--r--   0        0        0      829 2024-04-01 15:30:58.040881 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py
+-rw-r--r--   0        0        0     1487 2024-04-01 15:30:58.040940 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py
+-rw-r--r--   0        0        0      504 2024-04-01 15:30:58.040995 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_storage_usage.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.041055 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/utils/__init__.py
+-rw-r--r--   0        0        0     2920 2024-04-01 15:30:58.041125 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/utils/dates.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.041187 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/utils/testing/__init__.py
+-rw-r--r--   0        0        0     1884 2024-04-01 15:30:58.041259 harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/utils/testing/mixins.py
+-rw-r--r--   0        0        0     1032 2024-04-01 15:30:58.041370 harp_proxy-0.5.0b4/harp_apps/telemetry/__app__.py
+-rw-r--r--   0        0        0       24 2024-04-01 15:30:58.041429 harp_proxy-0.5.0b4/harp_apps/telemetry/__init__.py
+-rw-r--r--   0        0        0     2735 2024-04-01 15:30:58.041643 harp_proxy-0.5.0b4/harp_apps/telemetry/manager.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:58.041715 harp_proxy-0.5.0b4/harp_apps/telemetry/tests/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-01 15:30:58.041792 harp_proxy-0.5.0b4/harp_apps/telemetry/tests/test_application.py
+-rw-r--r--   0        0        0     1768 2024-04-01 15:30:58.041861 harp_proxy-0.5.0b4/harp_apps/telemetry/tests/test_manager.py
+-rw-r--r--   0        0        0     2782 2024-04-01 15:30:58.045623 harp_proxy-0.5.0b4/pyproject.toml
+-rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 harp_proxy-0.5.0b4/PKG-INFO
```

### Comparing `harp_proxy-0.5.0b3/LICENSE.rst` & `harp_proxy-0.5.0b4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/README.rst` & `harp_proxy-0.5.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/__init__.py` & `harp_proxy-0.5.0b4/harp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         if "-" in version:
             return _parse_version(version.rsplit("-", 1)[0], default=default)
         return default
 
 
 # last release
 __title__ = "Core"
-__version__ = "0.5.0b3"
+__version__ = "0.5.0b4"
 __revision__ = __version__  # we can't commit the not yet known revision
 
 # override with version.txt if available (after docker build for example)
 if os.path.exists(os.path.join(ROOT_DIR, "version.txt")):
     with open(os.path.join(ROOT_DIR, "version.txt")) as f:
         __version__ = f.read().strip()
```

### Comparing `harp_proxy-0.5.0b3/harp/_logging.py` & `harp_proxy-0.5.0b4/harp/_logging.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/asgi/bridge/requests.py` & `harp_proxy-0.5.0b4/harp/asgi/bridge/requests.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/asgi/bridge/responses.py` & `harp_proxy-0.5.0b4/harp/asgi/bridge/responses.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/asgi/events.py` & `harp_proxy-0.5.0b4/harp/asgi/events.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/asgi/kernel.py` & `harp_proxy-0.5.0b4/harp/asgi/kernel.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/asgi/tests/test_http_bridge_asgi_request.py` & `harp_proxy-0.5.0b4/harp/asgi/tests/test_http_bridge_asgi_request.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/commandline/__init__.py` & `harp_proxy-0.5.0b4/harp/commandline/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/commandline/start.py` & `harp_proxy-0.5.0b4/harp/commandline/start.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/commandline/utils/_hacks.py` & `harp_proxy-0.5.0b4/harp/commandline/utils/_hacks.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/commandline/utils/manager.py` & `harp_proxy-0.5.0b4/harp/commandline/utils/manager.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/__init__.py` & `harp_proxy-0.5.0b4/harp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/adapters/hypercorn.py` & `harp_proxy-0.5.0b4/harp/config/adapters/hypercorn.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/application.py` & `harp_proxy-0.5.0b4/harp/config/application.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/config.py` & `harp_proxy-0.5.0b4/harp/config/config.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/events.py` & `harp_proxy-0.5.0b4/harp/config/events.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/factories/kernel_factory.py` & `harp_proxy-0.5.0b4/harp/config/factories/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/factories/tests/test_configuration.py` & `harp_proxy-0.5.0b4/harp/config/factories/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/factories/tests/test_settings.py` & `harp_proxy-0.5.0b4/harp/config/factories/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/config/settings/from_file.py` & `harp_proxy-0.5.0b4/harp/config/settings/from_file.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/controllers/__init__.py` & `harp_proxy-0.5.0b4/harp/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/controllers/default.py` & `harp_proxy-0.5.0b4/harp/controllers/default.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/controllers/resolvers.py` & `harp_proxy-0.5.0b4/harp/controllers/resolvers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/controllers/routing.py` & `harp_proxy-0.5.0b4/harp/controllers/routing.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/event_dispatcher.py` & `harp_proxy-0.5.0b4/harp/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/__init__.py` & `harp_proxy-0.5.0b4/harp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/errors.py` & `harp_proxy-0.5.0b4/harp/http/errors.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/requests.py` & `harp_proxy-0.5.0b4/harp/http/requests.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/responses.py` & `harp_proxy-0.5.0b4/harp/http/responses.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/serializers.py` & `harp_proxy-0.5.0b4/harp/http/serializers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/tests/stubs.py` & `harp_proxy-0.5.0b4/harp/http/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/tests/test_requests.py` & `harp_proxy-0.5.0b4/harp/http/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/tests/test_requests_wrapped.py` & `harp_proxy-0.5.0b4/harp/http/tests/test_requests_wrapped.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/tests/test_utils_cookies.py` & `harp_proxy-0.5.0b4/harp/http/tests/test_utils_cookies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/typing/bridges.py` & `harp_proxy-0.5.0b4/harp/http/typing/bridges.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/typing/messages.py` & `harp_proxy-0.5.0b4/harp/http/typing/messages.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/utils/cookies.py` & `harp_proxy-0.5.0b4/harp/http/utils/cookies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/http/utils/methods.py` & `harp_proxy-0.5.0b4/harp/http/utils/methods.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/meta/__init__.py` & `harp_proxy-0.5.0b4/harp/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/models/blobs.py` & `harp_proxy-0.5.0b4/harp/models/blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/models/transactions.py` & `harp_proxy-0.5.0b4/harp/models/transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/tests/test_asgi_kernel.py` & `harp_proxy-0.5.0b4/harp/tests/test_asgi_kernel.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/tests/test_settings.py` & `harp_proxy-0.5.0b4/harp/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/typing/storage.py` & `harp_proxy-0.5.0b4/harp/typing/storage.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/background.py` & `harp_proxy-0.5.0b4/harp/utils/background.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/collections.py` & `harp_proxy-0.5.0b4/harp/utils/collections.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/dates.py` & `harp_proxy-0.5.0b4/harp/utils/dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/network.py` & `harp_proxy-0.5.0b4/harp/utils/network.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/applications.py` & `harp_proxy-0.5.0b4/harp/utils/testing/applications.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/benchmarking.py` & `harp_proxy-0.5.0b4/harp/utils/testing/benchmarking.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/communicators/asgi.py` & `harp_proxy-0.5.0b4/harp/utils/testing/communicators/asgi.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/communicators/http.py` & `harp_proxy-0.5.0b4/harp/utils/testing/communicators/http.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/http.py` & `harp_proxy-0.5.0b4/harp/utils/testing/http.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/mixins/controllers.py` & `harp_proxy-0.5.0b4/harp/utils/testing/mixins/controllers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/testing/stub_api/__init__.py` & `harp_proxy-0.5.0b4/harp/utils/testing/stub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/tests/test_collections.py` & `harp_proxy-0.5.0b4/harp/utils/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/utils/tests/test_dates.py` & `harp_proxy-0.5.0b4/harp/utils/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp/views/json.py` & `harp_proxy-0.5.0b4/harp/views/json.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/contrib/sentry/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/contrib/sentry/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/__init__.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/blobs.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/overview.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/overview.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/system.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/system.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/controllers/transactions.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/controllers/transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/docs/development/tests_e2e.rst` & `harp_proxy-0.5.0b4/harp_apps/dashboard/docs/development/tests_e2e.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/docs/development/tests_unit.rst` & `harp_proxy-0.5.0b4/harp_apps/dashboard/docs/development/tests_unit.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/docs/index.rst` & `harp_proxy-0.5.0b4/harp_apps/dashboard/docs/index.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/filters/base.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/filters/base.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/filters/transaction_endpoint.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/filters/transaction_endpoint.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/.eslintrc.cjs` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/.eslintrc.cjs`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/mockServiceWorker.js` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/mockServiceWorker.js`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/package.json` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/package.json`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/playwright.config.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/pnpm-lock.yaml` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/public/harp.svg` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/public/harp.svg`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Assets/logo.svg` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Assets/logo.svg`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/ApdexBadge.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/ApdexBadge.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/RequestMethodBadge.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/RequestMethodBadge.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/ResponseStatusBadge.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/ResponseStatusBadge.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/StyledJumboBadge.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/StyledJumboBadge.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Badges/constants.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Badges/constants.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Layout/Layout.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Layout/Layout.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Layout/__snapshots__/Layout.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Layout/__snapshots__/Layout.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/Page.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/Page.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/Page.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/Page.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/PageTitle.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/PageTitle.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Page/__snapshots__/Page.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Page/__snapshots__/Page.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Components/Utilities/OnQuerySuccess.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Components/Utilities/OnQuerySuccess.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Api/useApi.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Api/useApi.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Overview/useOverviewDataQuery.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Overview/useOverviewDataQuery.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useBlobQuery.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useBlobQuery.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsListQuery.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Domain/Transactions/useTransactionsListQuery.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Models/Schemas/Transaction.json` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Models/Schemas/Transaction.json`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Models/Transaction.d.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Models/Transaction.d.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/BaseTransactionsOverview.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/TransactionsChart.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/__snapshots__/TransactionsChart.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/Charts/__snapshots__/TransactionsChart.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/PerformancesSummary.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/PerformancesSummary.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/RateSummary.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/RateSummary.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Components/__snapshots__/BaseTransactionsOverview.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Components/__snapshots__/BaseTransactionsOverview.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/TransactionsOverview.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/__snapshots__/TransactionsOverview.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/Containers/__snapshots__/TransactionsOverview.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/OverviewPage.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/OverviewPage.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Overview/__snapshots__/OverviewPage.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Overview/__snapshots__/OverviewPage.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/SettingsTable.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/Components/Topology/Topology.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemDependenciesTabPanel.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemPage.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemSettingsTabPanel.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemStorageTabPanel.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemStorageTabPanel.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/SystemTopologyTabPanel.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemDependenciesTabPanel.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemDependenciesTabPanel.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemPage.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemPage.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemSettingsTabPanel.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemSettingsTabPanel.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemTopologyTabPanel.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/System/__snapshots__/SystemTopologyTabPanel.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Buttons.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Buttons.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/Facet.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/Facet.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/Facet.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Facets/__snapshots__/Facet.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Foldable.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/Foldable.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/List/TransactionDataTable.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageHeaders.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageHeaders.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageSummary.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/MessageSummary.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/OptionalPaginator.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/OptionalPaginator.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/PrettyBody.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/PrettyBody.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/__snapshots__/HeadersTable.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Components/__snapshots__/HeadersTable.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/FiltersSidebar.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/__snapshots__/FiltersSidebar.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/Containers/__snapshots__/FiltersSidebar.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailOnQuerySuccess.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailOnQuerySuccess.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionDetailPage.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListOnQuerySuccess.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListOnQuerySuccess.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListPage.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/TransactionListPage.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionListPage.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionListPage.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsDetailPage.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsDetailPage.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsListPage.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/Pages/Transactions/__snapshots__/TransactionsListPage.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/main.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/main.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/api/overview.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/api/overview.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/api/summary.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/api/summary.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/mocks/handlers.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/mocks/handlers.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/tests/utils.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Badge/Badge.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Button/Button.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/ButtonGroup/ButtonGroup.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/DataTable.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/DataTable/__snapshots__/DataTable.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/DataTable/__snapshots__/DataTable.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Checkbox.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/FormWidgets.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/FormWidgets.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/Radio.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/__snapshots__/Checkbox.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/FormWidgets/__snapshots__/Checkbox.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Assets/logo.svg` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Assets/logo.svg`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/Navbar.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Navbar/__snapshots__/Navbar.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Navbar/__snapshots__/Navbar.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Pagination.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Pagination.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/Paginator.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pagination/__snapshots__/Paginator.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pagination/__snapshots__/Paginator.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Pane/Pane.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/SearchBar.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/__snapshots__/SearchBar.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/SearchBar/__snapshots__/SearchBar.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.test.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.test.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/Tabs.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Tabs/__snapshots__/Tabs.test.tsx.snap` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Tabs/__snapshots__/Tabs.test.tsx.snap`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/Titles.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/Titles.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/Components/Typography/Typography.stories.tsx` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/Components/Typography/Typography.stories.tsx`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/badge--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/badge--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--primary-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--primary-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--secondary-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button--secondary-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button-group--button-group-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/button-group--button-group-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/data-table--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/data-table--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-with-style-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--checkboxes-with-style-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--radios-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/form-widgets--radios-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/navbar--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/navbar--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pagination--paginator-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pagination--paginator-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pane--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/pane--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/search-bar--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/search-bar--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/tabs--default-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/tabs--default-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-with-paragraphs-darwin.png` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/src/ui/tests/snapshot.spec.ts-snapshots/typography--titles-with-paragraphs-darwin.png`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tailwind.config.js` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tests/systemDependenciesPage.spec.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tests/systemDependenciesPage.spec.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tests/transactionsPage.spec.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tests/transactionsPage.spec.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/tsconfig.json` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/vite.config.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/vite.config.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/frontend/vitest.setup.ts` & `harp_proxy-0.5.0b4/harp_apps/dashboard/frontend/vitest.setup.ts`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/settings.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_controllers_blobs.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_controllers_blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_controllers_transactions.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_controllers_transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_settings.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/tests/test_utils_dependencies.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/tests/test_utils_dependencies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/tests/utils/test_dates.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/utils/dates.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/utils/dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/dashboard/utils/dependencies.py` & `harp_proxy-0.5.0b4/harp_apps/dashboard/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/http_client/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/http_client/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/janitor/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/janitor/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/janitor/tests/test_worker.py` & `harp_proxy-0.5.0b4/harp_apps/janitor/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/janitor/worker.py` & `harp_proxy-0.5.0b4/harp_apps/janitor/worker.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/proxy/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/proxy/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/proxy/controllers.py` & `harp_proxy-0.5.0b4/harp_apps/proxy/controllers.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/proxy/docs/index.rst` & `harp_proxy-0.5.0b4/harp_apps/proxy/docs/index.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/proxy/settings.py` & `harp_proxy-0.5.0b4/harp_apps/proxy/settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/proxy/tests/test_controllers_http_proxy.py` & `harp_proxy-0.5.0b4/harp_apps/proxy/tests/test_controllers_http_proxy.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/docs/index.rst` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/docs/index.rst`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/__init__.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/base.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/base.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/blobs.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/blobs.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/flags.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/flags.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/messages.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/messages.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/metrics.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/metrics.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/tags.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/tags.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/transactions.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/models/users.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/models/users.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/settings.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/settings.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/storage.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/storage.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_application.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_models_base.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_models_base.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_storage_tags.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/tests/test_storage_transactions.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/utils/dates.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/utils/dates.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/sqlalchemy_storage/utils/testing/mixins.py` & `harp_proxy-0.5.0b4/harp_apps/sqlalchemy_storage/utils/testing/mixins.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/telemetry/__app__.py` & `harp_proxy-0.5.0b4/harp_apps/telemetry/__app__.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/telemetry/manager.py` & `harp_proxy-0.5.0b4/harp_apps/telemetry/manager.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/harp_apps/telemetry/tests/test_manager.py` & `harp_proxy-0.5.0b4/harp_apps/telemetry/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `harp_proxy-0.5.0b3/pyproject.toml` & `harp_proxy-0.5.0b4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "harp-proxy"
-version = "0.5.0b3"
-description = ""
+version = "0.5.0b4"
+description = "Harp is an API Runtime Proxy – A toolkit for Fast, Reliable and Observable external APIs"
 authors = ["Romain Dorgueil <romain@makersquad.fr>"]
 readme = "README.rst"
 packages = [
     { include = "harp" },
     { include = "harp_apps" },
 ]
 
@@ -19,33 +19,34 @@
 aiosqlite = ">=0.19,<0.21"
 anyio = "^4.3.0"
 asgimiddlewarestaticfile = "^0.6.0"
 asgiref = "^3.8.1"
 asyncpg = "^0.29.0"
 dataclasses-json = "^0.6.3"
 dataclasses-jsonschema = "^2.16.0"
+essentials-configuration = "^2.0.4"
+hishel = ">=0.0.21,<0.0.26"
 honcho = { version = "^1.1.0", optional = true }
 http-router = "^4.1.2"
 httpx = ">=0.26,<0.28"
 hypercorn = "^0.16.0"
 multidict = "^6.0.5"
+orjson = "^3.10.0"
 passlib = "^1.7.4"
 psycopg2-binary = "^2.9.9"
+pyyaml = "^6.0.1"
 rich = "^13.7.1"
+rich-click = "^1.7.4"
+rodi = "^2.0.6"
+sentry-sdk = "^1.44.0"
 sqlalchemy = { extras = ["asyncio"], version = "^2.0.29" }
 sqlalchemy-utils = "^0.41.1"
 structlog = "^24.1.0"
 svix-ksuid = "^0.6.2"
 watchfiles = { version = "^0.21.0", optional = true }
-orjson = "^3.10.0"
-hishel = ">=0.0.21,<0.0.26"
-sentry-sdk = "^1.44.0"
-essentials-configuration = "^2.0.4"
-rodi = "^2.0.6"
-pyyaml = "^6.0.1"
 whistle = { version = "2.0.0a1", allow-prereleases = true }
 
 
 [tool.poetry.group.dev.dependencies]
 asgi-tools = "^0.76.0"
 black = ">=23.12,<25.0"
 furo = ">=2023.9.10,<2025.0.0"
@@ -63,15 +64,14 @@
 sphinx-copybutton = "^0.5.2"
 sphinx-sitemap = "^2.5.1"
 ruff = "^0.1.9"
 pytest-xdist = {version = "^3.5.0", extras = ["psutil"]}
 freezegun = "^1.4.0"
 testcontainers = {extras = ["postgres"], version = ">=3.7.1,<5.0.0"}
 sphinx-click = "^5.1.0"
-rich-click = "^1.7.4"
 
 
 [tool.poetry.group.mysql.dependencies]
 asyncmy = "^0.2.9"
 aiomysql = "^0.2.0"
 cryptography = ">=41.0.7,<43.0.0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `harp_proxy-0.5.0b3/PKG-INFO` & `harp_proxy-0.5.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: harp-proxy
-Version: 0.5.0b3
-Summary: 
+Version: 0.5.0b4
+Summary: Harp is an API Runtime Proxy – A toolkit for Fast, Reliable and Observable external APIs
 Author: Romain Dorgueil
 Author-email: romain@makersquad.fr
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
@@ -25,14 +25,15 @@
 Requires-Dist: hypercorn (>=0.16.0,<0.17.0)
 Requires-Dist: multidict (>=6.0.5,<7.0.0)
 Requires-Dist: orjson (>=3.10.0,<4.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: rich-click (>=1.7.4,<2.0.0)
 Requires-Dist: rodi (>=2.0.6,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.44.0,<2.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.29,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: svix-ksuid (>=0.6.2,<0.7.0)
 Requires-Dist: watchfiles (>=0.21.0,<0.22.0) ; extra == "dev"
```

