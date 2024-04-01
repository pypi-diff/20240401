# Comparing `tmp/port_ocean-0.5.8.tar.gz` & `tmp/port_ocean-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.5.8.tar", max compression
+gzip compressed data, was "port_ocean-0.5.9.tar", max compression
```

## Comparing `port_ocean-0.5.8.tar` & `port_ocean-0.5.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0    11357 2024-03-28 12:53:25.975608 port_ocean-0.5.8/LICENSE.md
--rw-r--r--   0        0        0     4668 2024-03-28 12:53:25.975608 port_ocean-0.5.8/README.md
--rw-r--r--   0        0        0      294 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/__init__.py
--rw-r--r--   0        0        0     1321 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/bootstrap.py
--rw-r--r--   0        0        0      328 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      369 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0       88 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/defaults/__init___.py
--rw-r--r--   0        0        0     1544 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/defaults/clean.py
--rw-r--r--   0        0        0     1104 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/defaults/dock.py
--rw-r--r--   0        0        0      115 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/defaults/group.py
--rw-r--r--   0        0        0     1134 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     2074 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     2193 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/__init__.py
--rw-r--r--   0        0        0      481 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0      446 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/extensions.py
--rw-r--r--   0        0        0      358 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/hooks/post_gen_project.py
--rw-r--r--   0        0        0     1034 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      497 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      326 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1773 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      468 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      906 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1928 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0      124 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/sonar-project.properties
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2863 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2640 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     4575 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     7902 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     5155 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0     1457 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/mixins/migrations.py
--rw-r--r--   0        0        0     2056 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/retry_transport.py
--rw-r--r--   0        0        0      451 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0     2373 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     6474 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/config/base.py
--rw-r--r--   0        0        0     2030 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1575 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/config/settings.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0     4710 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     5275 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/context/event.py
--rw-r--r--   0        0        0     4657 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/context/ocean.py
--rw-r--r--   0        0        0     1692 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/context/resource.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      142 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/core/defaults/__init__.py
--rw-r--r--   0        0        0     2185 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/core/defaults/clean.py
--rw-r--r--   0        0        0     3553 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/core/defaults/common.py
--rw-r--r--   0        0        0     7702 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/core/defaults/initialize.py
--rw-r--r--   0        0        0      889 2024-03-28 12:53:26.019608 port_ocean-0.5.8/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0     1327 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3697 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0     2577 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/event_listener/http.py
--rw-r--r--   0        0        0     6875 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/event_listener/kafka.py
--rw-r--r--   0        0        0     2150 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/event_listener/once.py
--rw-r--r--   0        0        0     3485 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/event_listener/polling.py
--rw-r--r--   0        0        0      610 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0      157 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/base.py
--rw-r--r--   0        0        0      173 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7928 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1751 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0     1550 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0      156 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0     1710 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     5425 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0      134 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      853 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0     1495 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1985 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     3193 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0      220 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0     2341 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     3771 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     3880 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0    13810 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/mixins/sync_raw.py
--rw-r--r--   0        0        0     2303 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0      714 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/models.py
--rw-r--r--   0        0        0      789 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      372 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      790 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      541 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      197 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/exceptions/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/helpers/__init__.py
--rw-r--r--   0        0        0     1783 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/helpers/async_client.py
--rw-r--r--   0        0        0    13155 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/helpers/retry.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/log/__init__.py
--rw-r--r--   0        0        0     2853 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/log/handlers.py
--rw-r--r--   0        0        0     2175 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/log/logger_setup.py
--rw-r--r--   0        0        0     2335 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/log/sensetive.py
--rw-r--r--   0        0        0     2480 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4072 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/ocean.py
--rw-r--r--   0        0        0        0 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/py.typed
--rw-r--r--   0        0        0     1906 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/run.py
--rw-r--r--   0        0        0       73 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/sonar-project.properties
--rw-r--r--   0        0        0       91 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/utils/__init__.py
--rw-r--r--   0        0        0     1226 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/utils/async_http.py
--rw-r--r--   0        0        0     2231 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/utils/cache.py
--rw-r--r--   0        0        0     1723 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/utils/misc.py
--rw-r--r--   0        0        0     3231 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/utils/repeat.py
--rw-r--r--   0        0        0     1515 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/utils/signal.py
--rw-r--r--   0        0        0      177 2024-03-28 12:53:26.023608 port_ocean-0.5.8/port_ocean/version.py
--rw-r--r--   0        0        0     3652 2024-03-28 12:53:26.023608 port_ocean-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 port_ocean-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 12:05:03.730788 port_ocean-0.5.9/LICENSE.md
+-rw-r--r--   0        0        0     4668 2024-04-01 12:05:03.730788 port_ocean-0.5.9/README.md
+-rw-r--r--   0        0        0      294 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/__init__.py
+-rw-r--r--   0        0        0     1321 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/bootstrap.py
+-rw-r--r--   0        0        0      328 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      369 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/defaults/__init___.py
+-rw-r--r--   0        0        0     1544 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/defaults/clean.py
+-rw-r--r--   0        0        0     1104 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/defaults/dock.py
+-rw-r--r--   0        0        0      115 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/defaults/group.py
+-rw-r--r--   0        0        0     1134 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     2074 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     2193 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0      446 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/extensions.py
+-rw-r--r--   0        0        0      358 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     1034 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      497 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      326 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1773 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      468 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      906 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1928 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/sonar-project.properties
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2640 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     4575 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     7902 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     5155 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0     1457 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/mixins/migrations.py
+-rw-r--r--   0        0        0     2056 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/retry_transport.py
+-rw-r--r--   0        0        0      451 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0     2373 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     6474 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/config/base.py
+-rw-r--r--   0        0        0     2030 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1575 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/config/settings.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0     4710 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     5275 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4657 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0     1692 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/context/resource.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      142 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/defaults/__init__.py
+-rw-r--r--   0        0        0     2185 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/defaults/clean.py
+-rw-r--r--   0        0        0     3553 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/defaults/common.py
+-rw-r--r--   0        0        0     7702 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/defaults/initialize.py
+-rw-r--r--   0        0        0      889 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0     1327 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3697 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     2577 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/http.py
+-rw-r--r--   0        0        0     6875 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/kafka.py
+-rw-r--r--   0        0        0     2150 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/once.py
+-rw-r--r--   0        0        0     3485 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/event_listener/polling.py
+-rw-r--r--   0        0        0      610 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/handlers/base.py
+-rw-r--r--   0        0        0      173 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-01 12:05:03.774788 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7928 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1751 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0     1550 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0      156 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0     1710 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     5425 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0      134 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      853 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0     1495 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1985 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     3193 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0      220 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0     2341 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     3771 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0     3880 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0    13810 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/mixins/sync_raw.py
+-rw-r--r--   0        0        0     2303 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0      714 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/models.py
+-rw-r--r--   0        0        0      789 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      372 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      790 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      541 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      197 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/exceptions/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/helpers/__init__.py
+-rw-r--r--   0        0        0     1783 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/helpers/async_client.py
+-rw-r--r--   0        0        0    13155 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/helpers/retry.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/log/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/log/handlers.py
+-rw-r--r--   0        0        0     2175 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/log/logger_setup.py
+-rw-r--r--   0        0        0     2335 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/log/sensetive.py
+-rw-r--r--   0        0        0     2480 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4072 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/ocean.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/py.typed
+-rw-r--r--   0        0        0     1906 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/run.py
+-rw-r--r--   0        0        0       73 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/sonar-project.properties
+-rw-r--r--   0        0        0       91 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/utils/__init__.py
+-rw-r--r--   0        0        0     1226 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/utils/async_http.py
+-rw-r--r--   0        0        0     2231 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/utils/cache.py
+-rw-r--r--   0        0        0     1723 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/utils/misc.py
+-rw-r--r--   0        0        0     3231 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/utils/repeat.py
+-rw-r--r--   0        0        0     1515 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/utils/signal.py
+-rw-r--r--   0        0        0      177 2024-04-01 12:05:03.778787 port_ocean-0.5.9/port_ocean/version.py
+-rw-r--r--   0        0        0     3652 2024-04-01 12:05:03.778787 port_ocean-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 port_ocean-0.5.9/PKG-INFO
```

### Comparing `port_ocean-0.5.8/LICENSE.md` & `port_ocean-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/README.md` & `port_ocean-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/bootstrap.py` & `port_ocean-0.5.9/port_ocean/bootstrap.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/defaults/clean.py` & `port_ocean-0.5.9/port_ocean/cli/commands/defaults/clean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/defaults/dock.py` & `port_ocean-0.5.9/port_ocean/cli/commands/defaults/dock.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.5.9/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/main.py` & `port_ocean-0.5.9/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/new.py` & `port_ocean-0.5.9/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/pull.py` & `port_ocean-0.5.9/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/sail.py` & `port_ocean-0.5.9/port_ocean/cli/commands/sail.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/commands/version.py` & `port_ocean-0.5.9/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore` & `port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.5.9/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/authentication.py` & `port_ocean-0.5.9/port_ocean/clients/port/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from port_ocean.utils.misc import get_time
 
 
 class TokenResponse(BaseModel):
     access_token: str = Field(alias="accessToken")
     expires_in: int = Field(alias="expiresIn")
     token_type: str = Field(alias="tokenType")
-    _retrieved_time: int = PrivateAttr(get_time())
+    _retrieved_time: int = PrivateAttr(default_factory=lambda: int(get_time()))
 
     @property
     def expired(self) -> bool:
         return self._retrieved_time + self.expires_in < get_time()
 
     @property
     def full_token(self) -> str:
```

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/client.py` & `port_ocean-0.5.9/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.5.9/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.5.9/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.5.9/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/mixins/migrations.py` & `port_ocean-0.5.9/port_ocean/clients/port/mixins/migrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/retry_transport.py` & `port_ocean-0.5.9/port_ocean/clients/port/retry_transport.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/clients/port/utils.py` & `port_ocean-0.5.9/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/config/base.py` & `port_ocean-0.5.9/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/config/dynamic.py` & `port_ocean-0.5.9/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/config/settings.py` & `port_ocean-0.5.9/port_ocean/config/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.5.9/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/context/event.py` & `port_ocean-0.5.9/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/context/ocean.py` & `port_ocean-0.5.9/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/context/resource.py` & `port_ocean-0.5.9/port_ocean/context/resource.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/defaults/clean.py` & `port_ocean-0.5.9/port_ocean/core/defaults/clean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/defaults/common.py` & `port_ocean-0.5.9/port_ocean/core/defaults/common.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/defaults/initialize.py` & `port_ocean-0.5.9/port_ocean/core/defaults/initialize.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/base.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/factory.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/http.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/http.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/kafka.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/kafka.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/once.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/once.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/event_listener/polling.py` & `port_ocean-0.5.9/port_ocean/core/event_listener/polling.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/__init__.py` & `port_ocean-0.5.9/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.5.9/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/api.py` & `port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/api.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.5.9/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/integrations/base.py` & `port_ocean-0.5.9/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.5.9/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.5.9/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.5.9/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/integrations/mixins/sync_raw.py` & `port_ocean-0.5.9/port_ocean/core/integrations/mixins/sync_raw.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.5.9/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/models.py` & `port_ocean-0.5.9/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/ocean_types.py` & `port_ocean-0.5.9/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/core/utils.py` & `port_ocean-0.5.9/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/exceptions/core.py` & `port_ocean-0.5.9/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/exceptions/port_defaults.py` & `port_ocean-0.5.9/port_ocean/exceptions/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/helpers/async_client.py` & `port_ocean-0.5.9/port_ocean/helpers/async_client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/helpers/retry.py` & `port_ocean-0.5.9/port_ocean/helpers/retry.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/log/handlers.py` & `port_ocean-0.5.9/port_ocean/log/handlers.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/log/logger_setup.py` & `port_ocean-0.5.9/port_ocean/log/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/log/sensetive.py` & `port_ocean-0.5.9/port_ocean/log/sensetive.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/middlewares.py` & `port_ocean-0.5.9/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/ocean.py` & `port_ocean-0.5.9/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/run.py` & `port_ocean-0.5.9/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/utils/async_http.py` & `port_ocean-0.5.9/port_ocean/utils/async_http.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/utils/cache.py` & `port_ocean-0.5.9/port_ocean/utils/cache.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/utils/misc.py` & `port_ocean-0.5.9/port_ocean/utils/misc.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/utils/repeat.py` & `port_ocean-0.5.9/port_ocean/utils/repeat.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/port_ocean/utils/signal.py` & `port_ocean-0.5.9/port_ocean/utils/signal.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.5.8/pyproject.toml` & `port_ocean-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.5.8"
+version = "0.5.9"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>", "Tom Tankilevitch <tom@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.5.8/PKG-INFO` & `port_ocean-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.5.8
+Version: 0.5.9
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

