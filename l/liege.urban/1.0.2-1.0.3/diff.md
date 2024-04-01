# Comparing `tmp/liege.urban-1.0.2.tar.gz` & `tmp/liege.urban-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liege.urban-1.0.2.tar", last modified: Tue Nov 21 15:38:16 2023, max compression
+gzip compressed data, was "dist/liege.urban-1.0.3.tar", last modified: Mon Apr  1 09:57:04 2024, max compression
```

## Comparing `liege.urban-1.0.2.tar` & `liege.urban-1.0.3.tar`

### file list

```diff
@@ -1,345 +1,346 @@
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/
--rw-r--r--   0 mpeeters   (501) staff       (20)      681 2023-11-21 15:38:14.000000 liege.urban-1.0.2/CHANGES.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       41 2023-11-21 15:38:14.000000 liege.urban-1.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       90 2023-11-21 15:38:14.000000 liege.urban-1.0.2/MANIFEST.in
--rw-r--r--   0 mpeeters   (501) staff       (20)     1369 2023-11-21 15:38:16.000000 liege.urban-1.0.2/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/README.rst
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/docs/
--rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2023-11-21 15:38:14.000000 liege.urban-1.0.2/docs/LICENSE.GPL
--rw-r--r--   0 mpeeters   (501) staff       (20)      656 2023-11-21 15:38:14.000000 liege.urban-1.0.2/docs/LICENSE.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       74 2023-11-21 15:38:14.000000 liege.urban-1.0.2/docs/index.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)      579 2023-11-21 15:38:14.000000 liege.urban-1.0.2/pyproject.toml
--rw-r--r--   0 mpeeters   (501) staff       (20)      140 2023-11-21 15:38:16.000000 liege.urban-1.0.2/setup.cfg
--rw-r--r--   0 mpeeters   (501) staff       (20)     1944 2023-11-21 15:38:14.000000 liege.urban-1.0.2/setup.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/
--rw-r--r--   0 mpeeters   (501) staff       (20)       80 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/Extensions/
--rw-r--r--   0 mpeeters   (501) staff       (20)      362 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/catalog_stats.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1153 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/close_env_licences.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1027 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/close_old_tasks.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1025 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/event_portaltype_update.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1074 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/fix_127.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      977 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/fix_borderinglicences_state.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2072 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/fix_categorytownship.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      667 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/fix_decision.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      971 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/fix_decisions_dates.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      957 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/fix_preliminarynotice_state.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      916 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/import_architects.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      903 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/import_notaries.py
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/merge_configs.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      480 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/merge_foldermanager_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2243 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/missing_events_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2254 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/suspension_update.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      462 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/update_schedule_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3006 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/Extensions/update_task_configs.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2833 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/actionspanel/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/actionspanel/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      626 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/actionspanel/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1412 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/actionspanel/urbandoc_actions.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/adapters/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/adapters/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      462 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/adapters/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      401 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/adapters/is_archive.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      487 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/adapters/shore.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      709 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/adapters/urbain220.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/browser/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    16709 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/activity_report.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5486 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/address_search.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2071 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/codt_integratedlicenceview.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3832 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/codt_uniquelicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5568 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/browser/cron/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/cron/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1254 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/cron/activity_report.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      612 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/cron/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      702 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/inspection.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      941 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/redirects.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/browser/static/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/.gitkeep
--rw-r--r--   0 mpeeters   (501) staff       (20)      410 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/Access_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      410 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/Access_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      488 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/EDII_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      488 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/EDII_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)     3227 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/Plantation_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)     3227 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/Plantation_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      852 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/SSSP_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      852 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/SSSP_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      233 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/Voirie_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      233 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/Voirie_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      552 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/administrative_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      554 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/administrative_editors_environment.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      496 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/administrative_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      552 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/administrative_validators_environment.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      418 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/all.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      548 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/inspection_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      534 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/inspection_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)     1193 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/liege.urban.css
--rw-r--r--   0 mpeeters   (501) staff       (20)     3295 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/survey_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)     3295 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/survey_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      649 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/technical_editors.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      629 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/technical_editors_environment.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      611 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/technical_validators.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      659 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/static/technical_validators_environment.png
--rw-r--r--   0 mpeeters   (501) staff       (20)     3039 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/table.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1928 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/table.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/browser/templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1008 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/templates/activity_report.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     2203 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/browser/templates/address_search.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      306 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1724 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/content/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      908 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/article127.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2317 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/buildlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1373 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/codt_article127.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      873 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/codt_buildlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      992 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/codt_cu2.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3589 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/codt_integratedlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5565 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/codt_uniquelicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      577 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      717 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/contact.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      876 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/cu2.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     6838 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/env_base.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      616 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/env_bordering.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2258 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/factory.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      457 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/factory.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      314 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/foldermanager.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7626 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/genericlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      766 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/inquiry_event.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3092 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/inquiry_licence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2090 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/inspection.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      702 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/integratedlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2669 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/portion_out.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      496 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/preliminarynotice.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1153 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/roaddecree.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      874 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/uniquelicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2894 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/urbanevent.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      240 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/urbanevent_opinionrequest.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1886 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/content/worklocation_signaletic.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/dashboard/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/dashboard/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      293 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/dashboard/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      269 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/dashboard/vocabulary.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/documentgenerator/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/documentgenerator/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      204 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/documentgenerator/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3253 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/documentgenerator/helper_view.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/events/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/events/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      185 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/events/address_point_events.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      926 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/events/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      727 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/events/internal_opinion_request.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      301 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/events/licence_events.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      661 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/indexes.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      320 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/indexes.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1191 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/interfaces.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      833 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/interfaces.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/jbot/
--rw-r--r--   0 mpeeters   (501) staff       (20)       67 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/jbot/Products.urban.browser.licence.templates.parcels_macro.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     5266 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/jbot/Products.urban.browser.licence.templates.worklocation_macro.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/jbot/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1105 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/licence_fields_permissions.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/locales/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/
--rw-r--r--   0 mpeeters   (501) staff       (20)     5909 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)     6032 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     2977 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)     5351 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.po
--rw-r--r--   0 mpeeters   (501) staff       (20)       28 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/manual_translations.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/manual_translations.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     8136 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)     8437 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/plone.po
--rw-r--r--   0 mpeeters   (501) staff       (20)      581 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/urban.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)      680 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/urban.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     3693 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/imio.schedule.pot
--rw-r--r--   0 mpeeters   (501) staff       (20)     4616 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/liege.urban.pot
--rw-r--r--   0 mpeeters   (501) staff       (20)      663 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/manual_translations.pot
--rw-r--r--   0 mpeeters   (501) staff       (20)     5819 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/plone.pot
--rwxr-xr-x   0 mpeeters   (501) staff       (20)      674 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/update.sh
--rw-r--r--   0 mpeeters   (501) staff       (20)      748 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/locales/urban.pot
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/migration/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/migration/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      860 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/migration/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2947 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/migration/migrate_to_230.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     4410 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/migration/migrate_to_240.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/model/
--rw-r--r--   0 mpeeters   (501) staff       (20)   157827 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/model/archgenxml_profile.xmi
--rw-r--r--   0 mpeeters   (501) staff       (20)     2980 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/model/generate.conf
--rwxr-xr-x   0 mpeeters   (501) staff       (20)      336 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/model/generate.sh
--rw-r--r--   0 mpeeters   (501) staff       (20)     8722 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/model/tmp.zargo
--rw-r--r--   0 mpeeters   (501) staff       (20)    34540 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/model/workflows.zargo
--rw-r--r--   0 mpeeters   (501) staff       (20)     5276 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/overrides.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1458 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/permissions.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      142 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/browserlayer.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      304 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/catalog.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      179 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/cssregistry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      288 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/factorytool.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/liegeurban_default.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      237 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/metadata.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      632 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/registry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      504 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/rolemap.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)   215896 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/schedule_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      630 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/skins.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/types/
--rw-r--r--   0 mpeeters   (501) staff       (20)     2112 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/types/UrbanEventAcknowledgment.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2121 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/types/UrbanEventPreliminaryAdvice.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2145 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/types/UrbanEventWithEnvironmentValidation.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      454 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/types.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/acknowledgment_event_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    12381 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/acknowledgment_event_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/address_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)     5879 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/address_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/article127_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    82292 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/article127_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/buildlicence_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)   134342 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/buildlicence_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)   131347 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)   155553 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/college_event_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    13241 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/college_event_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/cu2_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)   102548 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/cu2_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/env_validation_event_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    12414 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/env_validation_event_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/envclassone_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)   135218 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/envclassone_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/envclassthree_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    46503 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/envclassthree_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inquiry_event_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    18872 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inquiry_event_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspection_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    38064 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspection_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspectionreport_event_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    10717 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspectionreport_event_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/opinion_request_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    14608 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/opinion_request_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/preliminary_notice_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    41373 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/preliminary_notice_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/preliminaryadvice_event_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    13002 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/preliminaryadvice_event_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/roaddecree_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    64630 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/roaddecree_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/ticket_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    49338 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/ticket_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urban_licence_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    41697 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urban_licence_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urbancertificateone_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)    18806 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urbancertificateone_workflow/definition.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urbandoc_workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)     4055 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urbandoc_workflow/definition.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     4986 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/default/workflows.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/profiles/tests/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/tests/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      225 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/profiles/tests/metadata.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/schedule/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    21221 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/conditions.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    37331 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/conditions.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/article127.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3491 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/buildlicence.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/declaration.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/division.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/envclassone.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/envclassthree.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/envclasstwo.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/miscdemand.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/notaryletter.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/parceloutlicence.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3547 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/roaddecree.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     4195 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/survey_schedule.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/urbancertificateone.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/config/urbancertificatetwo.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      374 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     8973 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/creation_conditions.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1289 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/default_states.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      309 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/default_states.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1522 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/default_user.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      689 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/default_user.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1331 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/end_conditions.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      711 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/indexes.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      238 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/indexes.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1260 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/licence_taskconfig.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3119 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/road_decree_conditions.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      228 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/start_conditions.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1103 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/start_date.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      690 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/start_date.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/schedule/templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1049 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/templates/create_opinions_requests_status.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/templates/send_opinions_requests_status.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     1113 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/to_icon.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      335 2023-11-21 15:38:14.000000 liege.urban-1.0.2/src/liege/urban/schedule/to_icon.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3391 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/schedule/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1265 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/schedule/vocabulary.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/scripts/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1980 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/scripts/convert_ptadresses_to_psql_9.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/services/
--rw-r--r--   0 mpeeters   (501) staff       (20)      280 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/services/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2832 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/services/address.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      414 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/services/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)    17826 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/setuphandlers.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/skins/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_images/
--rw-r--r--   0 mpeeters   (501) staff       (20)      750 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_images/UrbanEventAcknowledgment.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      750 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_images/UrbanEventPreliminaryAdvice.png
--rw-r--r--   0 mpeeters   (501) staff       (20)      750 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_images/UrbanEventWithEnvironmentValidation.png
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)      464 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_templates/urbaneventacknowledgment_edit.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      464 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_templates/urbaneventfdopinion_edit.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      464 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_templates/urbaneventpreliminaryadvice_edit.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      464 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins/liege_templates/urbaneventwithenvironmentvalidation_edit.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      259 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/skins.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     5405 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/testing.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      559 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/testing.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/tests/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/tests/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      829 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/tests/test_robot.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1410 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/tests/test_setup.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      444 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      262 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/vocabulary.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege/urban/workflows/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1132 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/FD_opinion_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2173 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/acknowledgment_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1956 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/address_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      740 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/article127_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     9678 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/buildlicence_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    17360 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/codt_uniquelicence_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2273 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/college_event_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7036 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     3760 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/env_validation_event_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7580 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/envclassone_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3552 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/envclassthree_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      179 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/followup_event_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2360 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/inquiry_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1932 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/inspection_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1079 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/inspectionreport_event_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     4122 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/licences_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     4535 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/opinionsrequest_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1337 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/preliminaryadvice_event_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2635 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/preliminarynotice_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5522 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/roaddecree_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2538 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/ticket_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1547 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/urbancertificateone_workflow.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1865 2023-11-21 15:38:15.000000 liege.urban-1.0.2/src/liege/urban/workflows/urbanevent_workflow.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1369 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)    13573 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/SOURCES.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/dependency_links.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      179 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/entry_points.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        6 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/namespace_packages.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/not-zip-safe
--rw-r--r--   0 mpeeters   (501) staff       (20)      171 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/requires.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        6 2023-11-21 15:38:16.000000 liege.urban-1.0.2/src/liege.urban.egg-info/top_level.txt
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      979 2024-04-01 09:57:02.000000 liege.urban-1.0.3/CHANGES.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       41 2024-04-01 09:57:02.000000 liege.urban-1.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       90 2024-04-01 09:57:02.000000 liege.urban-1.0.3/MANIFEST.in
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1667 2024-04-01 09:57:04.000000 liege.urban-1.0.3/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/README.rst
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/docs/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2024-04-01 09:57:02.000000 liege.urban-1.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 mpeeters   (501) staff       (20)      656 2024-04-01 09:57:02.000000 liege.urban-1.0.3/docs/LICENSE.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       74 2024-04-01 09:57:02.000000 liege.urban-1.0.3/docs/index.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)      579 2024-04-01 09:57:02.000000 liege.urban-1.0.3/pyproject.toml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      140 2024-04-01 09:57:04.000000 liege.urban-1.0.3/setup.cfg
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1944 2024-04-01 09:57:02.000000 liege.urban-1.0.3/setup.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/
+-rw-r--r--   0 mpeeters   (501) staff       (20)       80 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/Extensions/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      362 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/catalog_stats.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1153 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/close_env_licences.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1027 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/close_old_tasks.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1025 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/event_portaltype_update.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1074 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/fix_127.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      977 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/fix_borderinglicences_state.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2072 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/fix_categorytownship.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      667 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/fix_decision.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      971 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/fix_decisions_dates.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      957 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/fix_preliminarynotice_state.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      916 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/import_architects.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      903 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/import_notaries.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/merge_configs.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      480 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/merge_foldermanager_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2243 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/missing_events_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2254 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/suspension_update.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      462 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/update_schedule_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3006 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/Extensions/update_task_configs.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2833 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/actionspanel/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/actionspanel/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      626 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/actionspanel/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1412 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/actionspanel/urbandoc_actions.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/adapters/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/adapters/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      462 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/adapters/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      401 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/adapters/is_archive.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      487 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/adapters/shore.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      709 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/adapters/urbain220.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/browser/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    16709 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/activity_report.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5486 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/address_search.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2071 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/codt_integratedlicenceview.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3832 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/codt_uniquelicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5568 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/browser/cron/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/cron/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1254 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/cron/activity_report.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      612 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/cron/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      702 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/inspection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1061 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/redirects.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/browser/static/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/.gitkeep
+-rw-r--r--   0 mpeeters   (501) staff       (20)      410 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/Access_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      410 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/Access_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      488 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/EDII_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      488 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/EDII_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3227 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/Plantation_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3227 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/Plantation_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      852 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/SSSP_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      852 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/SSSP_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      233 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/Voirie_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      233 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/Voirie_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      552 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/administrative_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      554 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/administrative_editors_environment.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      496 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/administrative_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      552 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/administrative_validators_environment.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      418 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/all.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      548 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/inspection_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      534 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/inspection_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1193 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/liege.urban.css
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3295 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/survey_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3295 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/survey_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      649 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/technical_editors.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      629 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/technical_editors_environment.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      611 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/technical_validators.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      659 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/static/technical_validators_environment.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3039 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/table.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1928 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/table.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/browser/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1008 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/templates/activity_report.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2203 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/browser/templates/address_search.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      306 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1724 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/content/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      908 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/article127.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2317 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/buildlicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1373 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/codt_article127.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      873 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/codt_buildlicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      992 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/codt_cu2.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3589 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/codt_integratedlicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5565 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/codt_uniquelicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      577 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      717 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/contact.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      876 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/cu2.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6838 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/env_base.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      616 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/env_bordering.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2258 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/factory.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      457 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/factory.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      314 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/foldermanager.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7626 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/genericlicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      766 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/inquiry_event.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3092 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/inquiry_licence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2090 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/inspection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      702 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/integratedlicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2669 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/portion_out.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      496 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/preliminarynotice.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1153 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/roaddecree.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      874 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/uniquelicence.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2894 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/urbanevent.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      240 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/urbanevent_opinionrequest.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1886 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/content/worklocation_signaletic.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/dashboard/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/dashboard/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      293 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/dashboard/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      269 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/dashboard/vocabulary.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/documentgenerator/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/documentgenerator/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      204 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/documentgenerator/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3253 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/documentgenerator/helper_view.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/events/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/events/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      185 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/events/address_point_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      926 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/events/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      727 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/events/internal_opinion_request.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      301 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/events/licence_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      661 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      320 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/indexes.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1191 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/interfaces.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      833 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/interfaces.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/jbot/
+-rw-r--r--   0 mpeeters   (501) staff       (20)       67 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/jbot/Products.urban.browser.licence.templates.parcels_macro.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5266 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/jbot/Products.urban.browser.licence.templates.worklocation_macro.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/jbot/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1105 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/licence_fields_permissions.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/locales/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5909 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6032 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2977 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5444 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)       28 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/manual_translations.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/manual_translations.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8210 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8515 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/plone.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)      581 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/urban.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)      680 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/urban.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3693 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/imio.schedule.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4709 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/liege.urban.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)      663 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/manual_translations.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5880 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/plone.pot
+-rwxr-xr-x   0 mpeeters   (501) staff       (20)      674 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/update.sh
+-rw-r--r--   0 mpeeters   (501) staff       (20)      748 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/locales/urban.pot
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/migration/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/migration/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1101 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/migration/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2947 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/migration/migrate_to_230.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6095 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/migration/migrate_to_240.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1082 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/migration/utils.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/model/
+-rw-r--r--   0 mpeeters   (501) staff       (20)   157827 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/model/archgenxml_profile.xmi
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2980 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/model/generate.conf
+-rwxr-xr-x   0 mpeeters   (501) staff       (20)      336 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/model/generate.sh
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8722 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/model/tmp.zargo
+-rw-r--r--   0 mpeeters   (501) staff       (20)    34540 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/model/workflows.zargo
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5276 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/overrides.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1458 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/permissions.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      142 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/browserlayer.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      304 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/catalog.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      179 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/cssregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      288 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/factorytool.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/liegeurban_default.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      237 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      632 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/registry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      504 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/rolemap.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)   215896 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/schedule_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      630 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/skins.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/types/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2112 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/types/UrbanEventAcknowledgment.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2121 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/types/UrbanEventPreliminaryAdvice.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2145 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/types/UrbanEventWithEnvironmentValidation.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      454 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/types.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/acknowledgment_event_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    12381 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/acknowledgment_event_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/address_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5879 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/address_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/article127_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    96414 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/article127_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/buildlicence_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)   134342 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/buildlicence_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)   138982 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)   163139 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/college_event_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13241 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/college_event_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/cu2_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)   102548 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/cu2_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/env_validation_event_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    12414 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/env_validation_event_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/envclassone_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)   135218 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/envclassone_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/envclassthree_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    46503 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/envclassthree_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inquiry_event_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18872 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inquiry_event_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspection_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    44756 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspection_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspectionreport_event_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    10717 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspectionreport_event_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/opinion_request_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    14608 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/opinion_request_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/preliminary_notice_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    41373 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/preliminary_notice_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/preliminaryadvice_event_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13002 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/preliminaryadvice_event_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/roaddecree_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    64630 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/roaddecree_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/ticket_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    56029 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/ticket_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urban_licence_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    41697 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urban_licence_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urbancertificateone_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18806 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urbancertificateone_workflow/definition.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urbandoc_workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4055 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urbandoc_workflow/definition.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5000 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/default/workflows.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/profiles/tests/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/tests/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      225 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/profiles/tests/metadata.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/schedule/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    21221 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/conditions.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    37331 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/conditions.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/article127.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3491 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/buildlicence.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/declaration.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/division.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/envclassone.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/envclassthree.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/envclasstwo.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/miscdemand.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/notaryletter.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/parceloutlicence.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3547 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/roaddecree.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4195 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/survey_schedule.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/urbancertificateone.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3413 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/config/urbancertificatetwo.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      374 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8973 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/creation_conditions.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1289 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/default_states.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      309 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/default_states.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1522 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/default_user.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      689 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/default_user.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1331 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/end_conditions.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      711 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      238 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/indexes.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1260 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/licence_taskconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3119 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/road_decree_conditions.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      228 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/start_conditions.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1103 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/start_date.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      690 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/start_date.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/schedule/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1049 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/templates/create_opinions_requests_status.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/templates/send_opinions_requests_status.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1113 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/to_icon.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      335 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/to_icon.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3391 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1265 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/schedule/vocabulary.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/scripts/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1980 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/scripts/convert_ptadresses_to_psql_9.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/services/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      280 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/services/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2832 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/services/address.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      414 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/services/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)    17826 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/setuphandlers.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/skins/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_images/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      750 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_images/UrbanEventAcknowledgment.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      750 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_images/UrbanEventPreliminaryAdvice.png
+-rw-r--r--   0 mpeeters   (501) staff       (20)      750 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_images/UrbanEventWithEnvironmentValidation.png
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      464 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_templates/urbaneventacknowledgment_edit.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      464 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_templates/urbaneventfdopinion_edit.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      464 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_templates/urbaneventpreliminaryadvice_edit.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      464 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins/liege_templates/urbaneventwithenvironmentvalidation_edit.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      259 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/skins.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5405 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/testing.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      559 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/testing.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/tests/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/tests/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      829 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/tests/test_robot.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1410 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/tests/test_setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      444 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      262 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/vocabulary.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege/urban/workflows/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1132 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/FD_opinion_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2173 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/acknowledgment_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1956 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/address_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      740 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/article127_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9678 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/buildlicence_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    17360 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/codt_uniquelicence_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2273 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/college_event_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7036 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3760 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/env_validation_event_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7580 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/envclassone_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3552 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/envclassthree_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      179 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/followup_event_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2360 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/inquiry_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1932 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/inspection_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1079 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/inspectionreport_event_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4122 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/licences_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4535 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/opinionsrequest_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1337 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/preliminaryadvice_event_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2635 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/preliminarynotice_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5522 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/roaddecree_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2538 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/ticket_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1547 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/urbancertificateone_workflow.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1865 2024-04-01 09:57:02.000000 liege.urban-1.0.3/src/liege/urban/workflows/urbanevent_workflow.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-01 09:57:04.000000 liege.urban-1.0.3/src/liege.urban.egg-info/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1667 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13608 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/SOURCES.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/dependency_links.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      179 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/entry_points.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        6 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/namespace_packages.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/not-zip-safe
+-rw-r--r--   0 mpeeters   (501) staff       (20)      171 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/requires.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        6 2024-04-01 09:57:03.000000 liege.urban-1.0.3/src/liege.urban.egg-info/top_level.txt
```

### Comparing `liege.urban-1.0.2/CHANGES.rst` & `liege.urban-1.0.3/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.0.3 (2024-04-01)
+------------------
+
+New features:
+
+
+- Add caduc workflow state
+  [jchandelle,mpeeters] (URB-3007)
+- Add frozen workflow state to article127, inspection and ticket
+  [jchandelle] (URB-3023)
+
+
+Bug fixes:
+
+
+- Fix an issue with zope users on urban homepage
+  [mpeeters] (URB-2956)
+
+
 1.0.2 (2023-11-21)
 ------------------
 
 Bug fixes:
 
 
 - Ensure that every licence types can add `UrbanEventMayor` and `UrbanEventAcknowledgment`
```

### Comparing `liege.urban-1.0.2/PKG-INFO` & `liege.urban-1.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liege.urban
-Version: 1.0.2
+Version: 1.0.3
 Summary: Liège urban profile
 Home-page: https://pypi.python.org/pypi/liege.urban
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -29,14 +29,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.0.3 (2024-04-01)
+------------------
+
+New features:
+
+
+- Add caduc workflow state
+  [jchandelle,mpeeters] (URB-3007)
+- Add frozen workflow state to article127, inspection and ticket
+  [jchandelle] (URB-3023)
+
+
+Bug fixes:
+
+
+- Fix an issue with zope users on urban homepage
+  [mpeeters] (URB-2956)
+
+
 1.0.2 (2023-11-21)
 ------------------
 
 Bug fixes:
 
 
 - Ensure that every licence types can add `UrbanEventMayor` and `UrbanEventAcknowledgment`
```

### Comparing `liege.urban-1.0.2/docs/LICENSE.GPL` & `liege.urban-1.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/docs/LICENSE.rst` & `liege.urban-1.0.3/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/pyproject.toml` & `liege.urban-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/setup.py` & `liege.urban-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     '\n' +
     open('CHANGES.rst').read() +
     '\n')
 
 
 setup(
     name='liege.urban',
-    version='1.0.2',
+    version='1.0.3',
     description="Liège urban profile",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/close_env_licences.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/close_env_licences.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/close_old_tasks.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/close_old_tasks.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/event_portaltype_update.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/event_portaltype_update.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/fix_127.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/fix_127.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/fix_borderinglicences_state.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/fix_borderinglicences_state.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/fix_categorytownship.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/fix_categorytownship.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/fix_decision.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/fix_decision.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/fix_decisions_dates.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/fix_decisions_dates.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/fix_preliminarynotice_state.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/fix_preliminarynotice_state.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/import_architects.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/import_architects.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/import_notaries.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/import_notaries.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/missing_events_config.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/missing_events_config.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/suspension_update.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/suspension_update.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/Extensions/update_task_configs.py` & `liege.urban-1.0.3/src/liege/urban/Extensions/update_task_configs.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/__init__.py` & `liege.urban-1.0.3/src/liege/urban/__init__.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/actionspanel/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/actionspanel/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/actionspanel/urbandoc_actions.py` & `liege.urban-1.0.3/src/liege/urban/actionspanel/urbandoc_actions.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/adapters/urbain220.py` & `liege.urban-1.0.3/src/liege/urban/adapters/urbain220.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/activity_report.py` & `liege.urban-1.0.3/src/liege/urban/browser/activity_report.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/address_search.py` & `liege.urban-1.0.3/src/liege/urban/browser/address_search.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/codt_integratedlicenceview.py` & `liege.urban-1.0.3/src/liege/urban/browser/codt_integratedlicenceview.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/codt_uniquelicence.py` & `liege.urban-1.0.3/src/liege/urban/browser/codt_uniquelicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/cron/activity_report.py` & `liege.urban-1.0.3/src/liege/urban/browser/cron/activity_report.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/cron/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/browser/cron/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/inspection.py` & `liege.urban-1.0.3/src/liege/urban/browser/inspection.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/redirects.py` & `liege.urban-1.0.3/src/liege/urban/browser/redirects.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
     def get_redirection_path(self):
         """
         """
         if self.user.getId() is None:
             return None
         else:
-            user_groups = api.group.get_groups(user=self.user)
+            try:
+                user_groups = api.group.get_groups(user=self.user)
+            except AttributeError:  # This happen with admin user
+                user_groups = []
             group_ids = [g.id for g in user_groups]
             if 'survey_editors' in group_ids:
                 return 'urban/survey_schedule'
             if 'urban_readers' in group_ids or 'environment_readers' in group_ids:
                 return 'urban'
             if 'opinions_editors' in group_ids:
                 return 'urban/opinions_schedule'
```

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/Plantation_editors.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/Plantation_editors.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/Plantation_validators.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/Plantation_validators.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/SSSP_editors.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/SSSP_editors.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/SSSP_validators.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/SSSP_validators.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/administrative_editors.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/administrative_editors.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/administrative_editors_environment.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/administrative_editors_environment.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/administrative_validators_environment.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/administrative_validators_environment.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/inspection_editors.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/inspection_editors.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/inspection_validators.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/inspection_validators.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/liege.urban.css` & `liege.urban-1.0.3/src/liege/urban/browser/static/liege.urban.css`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/survey_editors.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/survey_editors.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/survey_validators.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/survey_validators.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/technical_editors.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/technical_editors.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/technical_editors_environment.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/technical_editors_environment.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/technical_validators.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/technical_validators.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/static/technical_validators_environment.png` & `liege.urban-1.0.3/src/liege/urban/browser/static/technical_validators_environment.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/table.py` & `liege.urban-1.0.3/src/liege/urban/browser/table.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/table.zcml` & `liege.urban-1.0.3/src/liege/urban/browser/table.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/templates/activity_report.pt` & `liege.urban-1.0.3/src/liege/urban/browser/templates/activity_report.pt`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/browser/templates/address_search.pt` & `liege.urban-1.0.3/src/liege/urban/browser/templates/address_search.pt`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/article127.py` & `liege.urban-1.0.3/src/liege/urban/content/article127.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/buildlicence.py` & `liege.urban-1.0.3/src/liege/urban/content/buildlicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/codt_article127.py` & `liege.urban-1.0.3/src/liege/urban/content/codt_article127.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/codt_buildlicence.py` & `liege.urban-1.0.3/src/liege/urban/content/codt_buildlicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/codt_cu2.py` & `liege.urban-1.0.3/src/liege/urban/content/codt_cu2.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/codt_integratedlicence.py` & `liege.urban-1.0.3/src/liege/urban/content/codt_integratedlicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/codt_uniquelicence.py` & `liege.urban-1.0.3/src/liege/urban/content/codt_uniquelicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/contact.py` & `liege.urban-1.0.3/src/liege/urban/content/contact.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/cu2.py` & `liege.urban-1.0.3/src/liege/urban/content/cu2.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/env_base.py` & `liege.urban-1.0.3/src/liege/urban/content/env_base.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/env_bordering.py` & `liege.urban-1.0.3/src/liege/urban/content/env_bordering.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/factory.py` & `liege.urban-1.0.3/src/liege/urban/content/factory.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/genericlicence.py` & `liege.urban-1.0.3/src/liege/urban/content/genericlicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/inquiry_event.py` & `liege.urban-1.0.3/src/liege/urban/content/inquiry_event.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/inquiry_licence.py` & `liege.urban-1.0.3/src/liege/urban/content/inquiry_licence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/inspection.py` & `liege.urban-1.0.3/src/liege/urban/content/inspection.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/integratedlicence.py` & `liege.urban-1.0.3/src/liege/urban/content/integratedlicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/portion_out.py` & `liege.urban-1.0.3/src/liege/urban/content/portion_out.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/roaddecree.py` & `liege.urban-1.0.3/src/liege/urban/content/roaddecree.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/uniquelicence.py` & `liege.urban-1.0.3/src/liege/urban/content/uniquelicence.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/urbanevent.py` & `liege.urban-1.0.3/src/liege/urban/content/urbanevent.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/content/worklocation_signaletic.py` & `liege.urban-1.0.3/src/liege/urban/content/worklocation_signaletic.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/documentgenerator/helper_view.py` & `liege.urban-1.0.3/src/liege/urban/documentgenerator/helper_view.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/events/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/events/internal_opinion_request.py` & `liege.urban-1.0.3/src/liege/urban/events/internal_opinion_request.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/indexes.py` & `liege.urban-1.0.3/src/liege/urban/indexes.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/interfaces.py` & `liege.urban-1.0.3/src/liege/urban/interfaces.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/interfaces.zcml` & `liege.urban-1.0.3/src/liege/urban/interfaces.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/jbot/Products.urban.browser.licence.templates.worklocation_macro.pt` & `liege.urban-1.0.3/src/liege/urban/jbot/Products.urban.browser.licence.templates.worklocation_macro.pt`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/licence_fields_permissions.py` & `liege.urban-1.0.3/src/liege/urban/licence_fields_permissions.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.mo` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.mo`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.po` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/imio.schedule.po`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.mo` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-03-21 11:02+0000\n"
+"POT-Creation-Date: 2023-12-14 09:17+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
```

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.po` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/liege.urban.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-03-21 11:02+0000\n"
+"POT-Creation-Date: 2023-12-14 09:17+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
+#: ../interfaces.py:41
+msgid "AcknowledgmentEvent workflow type marker interface"
+msgstr ""
+
 #: ../browser/activity_report.py:34
 msgid "Date end"
 msgstr ""
 
 #: ../browser/activity_report.py:39
 msgid "Date index"
 msgstr ""
```

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/plone.mo` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/plone.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -223,17 +223,23 @@
 
 msgid "is_inacceptable"
 msgstr "Irrecevable"
 
 msgid "is_incomplete"
 msgstr "déclarer incomplet"
 
+msgid "make_obsolete"
+msgstr "Rendre caduc"
+
 msgid "notification"
 msgstr "Notification du permis"
 
+msgid "obsolete"
+msgstr "Caduc"
+
 msgid "opinion_given"
 msgstr "Avis rendu"
 
 msgid "opinion_validation"
 msgstr "validation"
 
 msgid "preliminary_advice_sent"
```

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/plone.po` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -423,7 +423,13 @@
 msgstr "En attente de l'avis"
 
 msgid "waiting_to_finalize"
 msgstr "En attente de finalisation"
 
 msgid "writing_report"
 msgstr "En rédaction"
+
+msgid "obsolete"
+msgstr "Caduc"
+
+msgid "make_obsolete"
+msgstr "Rendre caduc"
```

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/urban.mo` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/urban.mo`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/fr/LC_MESSAGES/urban.po` & `liege.urban-1.0.3/src/liege/urban/locales/fr/LC_MESSAGES/urban.po`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/imio.schedule.pot` & `liege.urban-1.0.3/src/liege/urban/locales/imio.schedule.pot`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/liege.urban.pot` & `liege.urban-1.0.3/src/liege/urban/locales/liege.urban.pot`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-03-21 11:02+0000\n"
+"POT-Creation-Date: 2023-12-14 09:17+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: liege.urban\n"
 
+#: ../interfaces.py:41
+msgid "AcknowledgmentEvent workflow type marker interface"
+msgstr ""
+
 #: ../browser/activity_report.py:34
 msgid "Date end"
 msgstr ""
 
 #: ../browser/activity_report.py:39
 msgid "Date index"
 msgstr ""
```

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/manual_translations.pot` & `liege.urban-1.0.3/src/liege/urban/locales/manual_translations.pot`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/plone.pot` & `liege.urban-1.0.3/src/liege/urban/locales/plone.pot`

 * *Files 2% similar despite different names*

```diff
@@ -426,7 +426,13 @@
 msgstr ""
 
 msgid "to_technical_analysis_post_investigation"
 msgstr ""
 
 msgid "technical_analysis_post_investigation"
 msgstr ""
+
+msgid "obsolete"
+msgstr ""
+
+msgid "make_obsolete"
+msgstr ""
```

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/update.sh` & `liege.urban-1.0.3/src/liege/urban/locales/update.sh`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/locales/urban.pot` & `liege.urban-1.0.3/src/liege/urban/locales/urban.pot`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/migration/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/migration/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -23,8 +23,16 @@
         title="Upgrade liege urban 2.4.1"
         description="urban upgrade step"
         source="*"
         destination="241"
         handler=".migrate_to_240.upgrade_to_241"
         profile="liege.urban:default" />
 
+    <gs:upgradeStep
+        title="Upgrade liege urban 2.4.2"
+        description="urban upgrade step"
+        source="241"
+        destination="242"
+        handler=".migrate_to_240.upgrade_to_242"
+        profile="liege.urban:default" />
+
 </configure>
```

### Comparing `liege.urban-1.0.2/src/liege/urban/migration/migrate_to_230.py` & `liege.urban-1.0.3/src/liege/urban/migration/migrate_to_230.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/migration/migrate_to_240.py` & `liege.urban-1.0.3/src/liege/urban/migration/migrate_to_240.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from imio.schedule.config import states_by_status
 from imio.schedule.config import STARTED
 from imio.schedule.interfaces import TaskConfigNotFound
 
 from Products.urban.interfaces import IUrbanEventType
 from Products.urban.interfaces import ILicenceConfig
 
+from liege.urban.migration.utils import refresh_workflow_permissions
 from plone import api
 
 
 import logging
 import re
 
 logger = logging.getLogger('urban: migrations')
@@ -94,7 +95,61 @@
 
 def upgrade_to_241(context):
     logger = logging.getLogger('urban: migrate to 2.4.1')
     logger.info("starting migration steps")
     from liege.urban.setuphandlers import setAllowedTypes
     setAllowedTypes(context)
     logger.info("migration done!")
+
+
+def upgrade_to_242(context):
+    logger = logging.getLogger('urban: migrate to 2.4.2')
+    logger.info("starting migration steps")
+    setup_tool = api.portal.get_tool('portal_setup')
+    setup_tool.runImportStepFromProfile('profile-liege.urban:default', 'workflow')
+    refresh_workflow_permissions(
+        "article127_workflow",
+        for_states=[
+            "complete",
+            "decision_in_progress",
+            "deposit",
+            "procedure_choosen",
+            "procedure_validated",
+            "report_written",
+            "validating_address",
+            "waiting_address",
+        ],
+    )
+    refresh_workflow_permissions(
+        "codt_buildlicence_workflow",
+        for_states=[
+            "FD_opinion",
+            "checking_completion",
+            "complete",
+            "decision_in_progress",
+            "deposit",
+            "incomplete",
+            "procedure_choosen",
+            "procedure_validated",
+            "report_written",
+            "suspension",
+            "validating_address",
+            "waiting_address",
+        ],
+    )
+    refresh_workflow_permissions(
+        "codt_uniquelicence_workflow",
+        for_states=[
+            "college_in_progress",
+            "complete",
+            "deposit",
+            "final_decision_in_progress",
+            "incomplete",
+            "internal_advice_done",
+            "internal_preliminary_advice",
+            "technical_report_validation",
+            "technical_synthesis_validation",
+            "validating_address",
+            "waiting_address",
+        ],
+    )
+    logger.info("migration done!")
```

### Comparing `liege.urban-1.0.2/src/liege/urban/model/archgenxml_profile.xmi` & `liege.urban-1.0.3/src/liege/urban/model/archgenxml_profile.xmi`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/model/generate.conf` & `liege.urban-1.0.3/src/liege/urban/model/generate.conf`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/model/tmp.zargo` & `liege.urban-1.0.3/src/liege/urban/model/tmp.zargo`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/model/workflows.zargo` & `liege.urban-1.0.3/src/liege/urban/model/workflows.zargo`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/overrides.zcml` & `liege.urban-1.0.3/src/liege/urban/overrides.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/permissions.zcml` & `liege.urban-1.0.3/src/liege/urban/permissions.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/registry.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/schedule_config.py` & `liege.urban-1.0.3/src/liege/urban/profiles/default/schedule_config.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/skins.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/types/UrbanEventAcknowledgment.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/types/UrbanEventAcknowledgment.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/types/UrbanEventPreliminaryAdvice.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/types/UrbanEventPreliminaryAdvice.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/types/UrbanEventWithEnvironmentValidation.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/types/UrbanEventWithEnvironmentValidation.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/acknowledgment_event_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/acknowledgment_event_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/address_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/address_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/article127_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/article127_workflow/definition.xml`

 * *Files 1% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/article127_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/article127_workflow/definition.xml`

```diff
@@ -315,14 +315,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="complete" title="complete">
     <exit-transition transition_id="invalidate_completion"/>
     <exit-transition transition_id="propose_procedure_choice"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -464,14 +465,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="decision_in_progress" title="decision_in_progress">
     <exit-transition transition_id="refuse_licence"/>
     <exit-transition transition_id="accept_licence"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -613,14 +615,15 @@
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="deposit" title="deposit">
     <exit-transition transition_id="ask_address_validation"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -756,14 +759,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="procedure_choosen" title="procedure_choosen">
     <exit-transition transition_id="invalidate_procedure_choice"/>
     <exit-transition transition_id="validate_procedure_choice"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -904,14 +908,15 @@
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="procedure_validated" title="procedure_validated">
     <exit-transition transition_id="propose_report"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1203,14 +1208,15 @@
     </permission-map>
   </state>
   <state state_id="report_written" title="report_written">
     <exit-transition transition_id="refuse_report"/>
     <exit-transition transition_id="validate_report_2"/>
     <exit-transition transition_id="validate_report_1"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1349,18 +1355,164 @@
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
+  <state state_id="frozen_suspension" title="frozen_suspension">
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Description Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+  </state>
   <state state_id="validating_address" title="validating_address">
     <exit-transition transition_id="validate_address"/>
     <exit-transition transition_id="ask_temporary_address"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1495,14 +1647,15 @@
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="waiting_address" title="waiting_address">
     <exit-transition transition_id="validate_temporary_address"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1632,14 +1785,162 @@
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
+  <state state_id="obsolete" title="obsolete">
+    <exit-transition transition_id="resume"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Description Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="True"/>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+  </state>
+  <transition transition_id="make_obsolete" title="make_obsolete" new_state="obsolete" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">make_obsolete</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
   <transition transition_id="abandon" title="abandon" new_state="abandoned" trigger="USER" before_script="" after_script="">
     <action url="" category="workflow" icon="">abandon</action>
     <guard/>
   </transition>
   <transition transition_id="accept_licence" title="accept_licence" new_state="accepted" trigger="USER" before_script="" after_script="">
     <action url="" category="workflow" icon="">accept_licence</action>
     <guard/>
```

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/buildlicence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/buildlicence_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/definition.xml`

 * *Files 1% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_buildlicence_workflow/definition.xml`

```diff
@@ -24,14 +24,15 @@
   <permission>urban: Add UrbanEvent</permission>
   <permission>urban: Add UrbanEventOpinionRequest</permission>
   <permission>List folder contents</permission>
   <state state_id="FD_opinion" title="FD_opinion">
     <exit-transition transition_id="receive_FD_opinion"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -613,14 +614,15 @@
     </permission-map>
   </state>
   <state state_id="checking_completion" title="checking_completion">
     <exit-transition transition_id="ask_complements"/>
     <exit-transition transition_id="propose_complete"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -761,14 +763,15 @@
     </permission-map>
   </state>
   <state state_id="complete" title="complete">
     <exit-transition transition_id="invalidate_completion"/>
     <exit-transition transition_id="propose_procedure_choice"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -908,14 +911,15 @@
     </permission-map>
   </state>
   <state state_id="decision_in_progress" title="decision_in_progress">
     <exit-transition transition_id="refuse_licence"/>
     <exit-transition transition_id="authorize_licence"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1058,14 +1062,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="deposit" title="deposit">
     <exit-transition transition_id="ask_address_validation"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1300,14 +1305,15 @@
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="True"/>
   </state>
   <state state_id="incomplete" title="incomplete">
     <exit-transition transition_id="receive_complements"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1444,14 +1450,15 @@
     </permission-map>
   </state>
   <state state_id="procedure_choosen" title="procedure_choosen">
     <exit-transition transition_id="invalidate_procedure_choice"/>
     <exit-transition transition_id="validate_procedure_choice"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1591,14 +1598,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="procedure_validated" title="procedure_validated">
     <exit-transition transition_id="propose_report"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1889,14 +1897,15 @@
   </state>
   <state state_id="report_written" title="report_written">
     <exit-transition transition_id="refuse_report"/>
     <exit-transition transition_id="validate_report_2"/>
     <exit-transition transition_id="validate_report_1"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -2038,14 +2047,15 @@
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="suspension" title="suspension">
     <exit-transition transition_id="resume"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -2332,14 +2342,15 @@
     </permission-map>
   </state>
   <state state_id="validating_address" title="validating_address">
     <exit-transition transition_id="validate_address"/>
     <exit-transition transition_id="ask_temporary_address"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -2481,14 +2492,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="waiting_address" title="waiting_address">
     <exit-transition transition_id="validate_temporary_address"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -2626,14 +2638,162 @@
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
+  <state state_id="obsolete" title="obsolete">
+    <exit-transition transition_id="resume"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Description Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="True"/>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+  </state>
+  <transition transition_id="make_obsolete" title="make_obsolete" new_state="obsolete" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">make_obsolete</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
   <transition transition_id="abandon" title="abandon" new_state="abandoned" trigger="USER" before_script="" after_script="">
     <action url="" category="workflow" icon="">abandon</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
   <transition transition_id="accept_licence" title="accept_licence" new_state="accepted" trigger="USER" before_script="" after_script="">
```

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/definition.xml`

 * *Files 1% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/codt_uniquelicence_workflow/definition.xml`

```diff
@@ -31,14 +31,15 @@
   <permission>urban: Add UrbanEvent</permission>
   <permission>urban: Add UrbanEventOpinionRequest</permission>
   <permission>List folder contents</permission>
   <state state_id="deposit" title="deposit">
     <exit-transition transition_id="ask_address_validation"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -216,14 +217,15 @@
     </permission-map>
   </state>
   <state state_id="validating_address" title="validating_address">
     <exit-transition transition_id="validate_address"/>
     <exit-transition transition_id="ask_temporary_address"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -400,14 +402,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="waiting_address" title="waiting_address">
     <exit-transition transition_id="validate_temporary_address"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -584,14 +587,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="internal_preliminary_advice" title="internal_preliminary_advice">
     <exit-transition transition_id="send_preliminary_advice"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -771,14 +775,15 @@
   </state>
   <state state_id="internal_advice_done" title="internal_advice_done">
     <exit-transition transition_id="is_incomplete"/>
     <exit-transition transition_id="is_complete"/>
     <exit-transition transition_id="isinacceptable"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -955,14 +960,15 @@
     </permission-map>
   </state>
   <state state_id="incomplete" title="incomplete">
     <exit-transition transition_id="is_complete"/>
     <exit-transition transition_id="isinacceptable"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1140,14 +1146,15 @@
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="complete" title="complete">
     <exit-transition transition_id="propose_technical_report"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1326,14 +1333,15 @@
     </permission-map>
   </state>
   <state state_id="technical_report_validation" title="technical_report_validation">
     <exit-transition transition_id="validate_technical_report"/>
     <exit-transition transition_id="refuse_technical_report"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1512,14 +1520,15 @@
   </state>
   <state state_id="college_in_progress" title="college_in_progress">
     <exit-transition transition_id="propose_technical_synthesis"/>
     <exit-transition transition_id="authorize_licence_FT"/>
     <exit-transition transition_id="refuse_licence_FT"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1696,14 +1705,15 @@
     </permission-map>
   </state>
   <state state_id="technical_synthesis_validation" title="technical_synthesis_validation">
     <exit-transition transition_id="validate_technical_synthesis"/>
     <exit-transition transition_id="refuse_technical_synthesis"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -1879,14 +1889,15 @@
     </permission-map>
   </state>
   <state state_id="final_decision_in_progress" title="final_decision_in_progress">
     <exit-transition transition_id="authorize_licence"/>
     <exit-transition transition_id="refuse_licence"/>
     <exit-transition transition_id="suspend"/>
     <exit-transition transition_id="abandon"/>
+    <exit-transition transition_id="make_obsolete"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
@@ -3129,14 +3140,162 @@
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
+  <state state_id="obsolete" title="obsolete">
+    <exit-transition transition_id="reopen"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Description Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="True"/>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+  </state>
+  <transition transition_id="make_obsolete" title="make_obsolete" new_state="obsolete" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">make_obsolete</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
   <transition transition_id="abandon" title="abandon" new_state="abandoned" trigger="USER" before_script="" after_script="">
     <action url="" category="workflow" icon="">abandon</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
   <transition transition_id="ask_address_validation" title="ask_address_validation" new_state="validating_address" trigger="USER" before_script="" after_script="">
```

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/college_event_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/college_event_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/cu2_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/cu2_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/env_validation_event_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/env_validation_event_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/envclassone_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/envclassone_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/envclassthree_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/envclassthree_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inquiry_event_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inquiry_event_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspection_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspection_workflow/definition.xml`

 * *Files 1% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspection_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspection_workflow/definition.xml`

```diff
@@ -730,14 +730,159 @@
     </permission-map>
     <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
+  <state state_id="frozen_suspension" title="frozen_suspension">
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Description Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>RoadEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+  </state>
   <transition transition_id="give_administrative_answer" title="give_administrative_answer" new_state="first_administrative_answer" trigger="USER" before_script="" after_script="">
     <action url="" category="workflow" icon="">give_administrative_answer</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
       <guard-expression>python: 'plainte' in here.getInspection_context()</guard-expression>
     </guard>
   </transition>
```

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/inspectionreport_event_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/inspectionreport_event_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/opinion_request_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/opinion_request_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/preliminary_notice_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/preliminary_notice_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/preliminaryadvice_event_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/preliminaryadvice_event_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/roaddecree_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/roaddecree_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/ticket_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urban_licence_workflow/definition.xml`

 * *Files 2% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/ticket_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urban_licence_workflow/definition.xml`

```diff
@@ -1,219 +1,125 @@
 <?xml version="1.0" encoding="utf-8"?>
-<dc-workflow workflow_id="inspection_workflow" title="inspection_workflow" description="" state_variable="review_state" initial_state="creation" manager_bypass="False">
-  <permission>ATContentTypes: Add File</permission>
-  <permission>ATContentTypes: Add Image</permission>
+<dc-workflow workflow_id="urban_licence_workflow" title="urban_licence_workflow" description="" state_variable="review_state" initial_state="in_progress" manager_bypass="False">
+  <permission>Acces contents information</permission>
   <permission>Access contents information</permission>
   <permission>Add portal content</permission>
   <permission>Delete objects</permission>
   <permission>Modify portal content</permission>
+  <permission>Modify view template</permission>
+  <permission>Review portal content</permission>
   <permission>View</permission>
   <permission>liege.urban: External Reader</permission>
   <permission>liege.urban: Internal Editor</permission>
   <permission>liege.urban: Internal Reader</permission>
-  <permission>liege.urban: Validate</permission>
+  <permission>liege.urban: Description Editor</permission>
+  <permission>liege.urban: Habitation Editor</permission>
+  <permission>urban: Add Contact</permission>
   <permission>urban: Add Applicant</permission>
   <permission>urban: Add Couple</permission>
-  <permission>urban: Add Contact</permission>
   <permission>urban: Add Corporation</permission>
+  <permission>urban: Add Inquiry</permission>
+  <permission>urban: Add CODT_UniqueLicenceInquiry</permission>
   <permission>urban: Add PortionOut</permission>
   <permission>urban: Add UrbanEvent</permission>
-  <permission>urban: Add UrbanEventInspectionReport</permission>
   <permission>urban: Add UrbanEventOpinionRequest</permission>
-  <permission>List folder contents</permission>
-  <state state_id="creation" title="creation">
-    <exit-transition transition_id="send_to_prosecutor"/>
+  <permission>ATContentTypes: Add File</permission>
+  <permission>ATContentTypes: Add Image</permission>
+  <state state_id="accepted" title="accepted">
+    <exit-transition transition_id="reopen"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map name="Acces contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Add portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
-    </permission-map>
-    <permission-map name="Delete objects" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: External Reader" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Internal Editor" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Internal Reader" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>InternalReader</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Applicant" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Couple" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Contact" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Corporation" acquired="False">
+    <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add UrbanEvent" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-  </state>
-  <state state_id="prosecution_analysis" title="prosecution_analysis">
-    <exit-transition transition_id="follow_to_technical_analysis"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
+    <permission-map name="Modify view template" acquired="False"/>
+    <permission-map name="Review portal content" acquired="False">
       <permission-role>Manager</permission-role>
+      <permission-role>Reviewer</permission-role>
     </permission-map>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Add portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
-    </permission-map>
-    <permission-map name="Delete objects" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: External Reader" acquired="False">
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
+      <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Editor" acquired="False">
+    <permission-map name="liege.urban: Description Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Reader" acquired="False">
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>InternalReader</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -227,230 +133,128 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="urban: Add Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
-      <permission-role>AddressEditor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
   </state>
-  <state state_id="technical_analysis" title="technical_analysis">
-    <exit-transition transition_id="propose_analysis"/>
+  <state state_id="in_progress" title="in_progress">
+    <exit-transition transition_id="refuse"/>
+    <exit-transition transition_id="accept"/>
+    <exit-transition transition_id="isincomplete"/>
+    <exit-transition transition_id="retire"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Access contents information" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
-    </permission-map>
-    <permission-map name="Add portal content" acquired="False">
+    <permission-map name="Acces contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Delete objects" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="List folder contents" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
-    </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: External Reader" acquired="False">
+    <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Editor" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Internal Reader" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>InternalReader</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Applicant" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Couple" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Contact" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add Corporation" acquired="False">
+    <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
-      <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEvent" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
+    <permission-map name="Modify view template" acquired="False">
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+    <permission-map name="Review portal content" acquired="False">
       <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reviewer</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-  </state>
-  <state state_id="technical_validation" title="technical_validation">
-    <exit-transition transition_id="validate_analysis"/>
-    <exit-transition transition_id="refuse_analysis"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="Access contents information" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
-    </permission-map>
-    <permission-map name="Add portal content" acquired="False">
+    <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Delete objects" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: External Reader" acquired="False">
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
+      <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Editor" acquired="False">
+    <permission-map name="liege.urban: Description Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Reader" acquired="False">
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>InternalReader</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -464,114 +268,127 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="urban: Add Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
+  </state>
+  <state state_id="incomplete" title="incomplete">
+    <exit-transition transition_id="reopen"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="waiting_for_agreement" title="waiting_for_agreement">
-    <exit-transition transition_id="finalize"/>
-    <exit-transition transition_id="back_to_technical_analysis"/>
-    <exit-transition transition_id="follow_in_court"/>
-    <exit-transition transition_id="close"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+    <permission-map name="Acces contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
+    <permission-map name="Modify view template" acquired="False">
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Review portal content" acquired="False">
       <permission-role>Manager</permission-role>
+      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
+    <permission-map name="liege.urban: Description Editor" acquired="False">
       <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -585,111 +402,125 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="urban: Add Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
-      <permission-role>AddressEditor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
+  </state>
+  <state state_id="refused" title="refused">
+    <exit-transition transition_id="reopen"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="waiting_to_finalize" title="waiting_to_finalize">
-    <exit-transition transition_id="close"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+    <permission-map name="Acces contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="Modify view template" acquired="False">
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Review portal content" acquired="False">
       <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
+    <permission-map name="liege.urban: Description Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
       <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -703,111 +534,124 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="urban: Add Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
-      <permission-role>AddressEditor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
+  </state>
+  <state state_id="inacceptable" title="inacceptable">
+    <exit-transition transition_id="reopen"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="in_court" title="in_court">
-    <exit-transition transition_id="close"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+    <permission-map name="Acces contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
+    <permission-map name="Modify view template" acquired="False">
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Review portal content" acquired="False">
       <permission-role>Manager</permission-role>
+      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
+    <permission-map name="liege.urban: Description Editor" acquired="False">
       <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -821,113 +665,127 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="urban: Add Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add PortionOut" acquired="False">
-      <permission-role>AddressEditor</permission-role>
+    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEvent" acquired="False">
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
-  <state state_id="ended" title="ended">
+  <state state_id="retired" title="retired">
     <exit-transition transition_id="reopen"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map name="Acces contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Add portal content" acquired="False">
+    <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Delete objects" acquired="False">
+    <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="List folder contents" acquired="False">
+    <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="Modify view template" acquired="False">
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Review portal content" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Validate" acquired="False">
+    <permission-map name="liege.urban: Description Editor" acquired="False">
       <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -941,95 +799,73 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+    <permission-map name="urban: Add Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add PortionOut" acquired="False">
-      <permission-role>AddressEditor</permission-role>
+    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEvent" acquired="False">
+    <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
-  <transition transition_id="send_to_prosecutor" title="send_to_prosecutor" new_state="prosecution_analysis" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
-    <guard>
-      <guard-permission>Modify portal content</guard-permission>
-    </guard>
-  </transition>
-  <transition transition_id="follow_to_technical_analysis" title="follow_to_technical_analysis" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
-    <guard>
-      <guard-permission>Modify portal content</guard-permission>
-    </guard>
-  </transition>
-  <transition transition_id="propose_analysis" title="propose_analysis" new_state="technical_validation" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
-    <guard>
-      <guard-permission>Modify portal content</guard-permission>
-    </guard>
-  </transition>
-  <transition transition_id="validate_analysis" title="validate_analysis" new_state="waiting_for_agreement" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
-    <guard>
-      <guard-permission>Modify portal content</guard-permission>
-    </guard>
-  </transition>
-  <transition transition_id="refuse_analysis" title="refuse_analysis" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
+  <transition transition_id="accept" title="accept" new_state="accepted" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="%(portal_url)s/accept.png">accept</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="finalize" title="finalize" new_state="waiting_to_finalize" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
+  <transition transition_id="isincomplete" title="isincomplete" new_state="incomplete" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="%(portal_url)s/isincomplete.png">isincomplete</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="follow_in_court" title="follow_in_court" new_state="in_court" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
+  <transition transition_id="refuse" title="refuse" new_state="refused" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="%(portal_url)s/refuse.png">refuse</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="back_to_technical_analysis" title="back_to_technical_analysis" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">analyse</action>
+  <transition transition_id="reopen" title="reopen" new_state="in_progress" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="%(portal_url)s/reopen.png">reopen</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="close" title="close" new_state="ended" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="">close</action>
+  <transition transition_id="isinacceptable" title="isinacceptable" new_state="inacceptable" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="%(portal_url)s/isincomplete.png">retire</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="reopen" title="reopen" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
-    <action url="" icon="" category="workflow">reopen</action>
+  <transition transition_id="retire" title="retire" new_state="retired" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="%(portal_url)s/retire.png">retire</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
   <variable variable_id="action" for_catalog="False" for_status="True" update_always="True">
     <description>The last transition</description>
     <default>
```

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urban_licence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/ticket_workflow/definition.xml`

 * *Files 11% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urban_licence_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/ticket_workflow/definition.xml`

```diff
@@ -1,260 +1,337 @@
 <?xml version="1.0" encoding="utf-8"?>
-<dc-workflow workflow_id="urban_licence_workflow" title="urban_licence_workflow" description="" state_variable="review_state" initial_state="in_progress" manager_bypass="False">
-  <permission>Acces contents information</permission>
+<dc-workflow workflow_id="inspection_workflow" title="inspection_workflow" description="" state_variable="review_state" initial_state="creation" manager_bypass="False">
+  <permission>ATContentTypes: Add File</permission>
+  <permission>ATContentTypes: Add Image</permission>
   <permission>Access contents information</permission>
   <permission>Add portal content</permission>
   <permission>Delete objects</permission>
   <permission>Modify portal content</permission>
-  <permission>Modify view template</permission>
-  <permission>Review portal content</permission>
   <permission>View</permission>
   <permission>liege.urban: External Reader</permission>
   <permission>liege.urban: Internal Editor</permission>
   <permission>liege.urban: Internal Reader</permission>
-  <permission>liege.urban: Description Editor</permission>
-  <permission>liege.urban: Habitation Editor</permission>
-  <permission>urban: Add Contact</permission>
+  <permission>liege.urban: Validate</permission>
   <permission>urban: Add Applicant</permission>
   <permission>urban: Add Couple</permission>
+  <permission>urban: Add Contact</permission>
   <permission>urban: Add Corporation</permission>
-  <permission>urban: Add Inquiry</permission>
-  <permission>urban: Add CODT_UniqueLicenceInquiry</permission>
   <permission>urban: Add PortionOut</permission>
   <permission>urban: Add UrbanEvent</permission>
+  <permission>urban: Add UrbanEventInspectionReport</permission>
   <permission>urban: Add UrbanEventOpinionRequest</permission>
-  <permission>ATContentTypes: Add File</permission>
-  <permission>ATContentTypes: Add Image</permission>
-  <state state_id="accepted" title="accepted">
-    <exit-transition transition_id="reopen"/>
+  <permission>List folder contents</permission>
+  <state state_id="creation" title="creation">
+    <exit-transition transition_id="send_to_prosecutor"/>
     <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Acces contents information" acquired="False">
+    <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Add portal content" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Delete objects" acquired="False">
+    <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify view template" acquired="False"/>
-    <permission-map name="Review portal content" acquired="False">
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reviewer</permission-role>
     </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+  </state>
+  <state state_id="prosecution_analysis" title="prosecution_analysis">
+    <exit-transition transition_id="follow_to_technical_analysis"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: External Reader" acquired="False">
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
-      <permission-role>RoadEditor</permission-role>
-      <permission-role>RoadReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Editor" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Internal Reader" acquired="False">
+    <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
+      <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Description Editor" acquired="False">
+    <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Applicant" acquired="False">
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Couple" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Contact" acquired="False">
+    <permission-map name="urban: Add Couple" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Corporation" acquired="False">
+    <permission-map name="urban: Add Contact" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Inquiry" acquired="False">
+    <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="in_progress" title="in_progress">
-    <exit-transition transition_id="refuse"/>
-    <exit-transition transition_id="accept"/>
-    <exit-transition transition_id="isincomplete"/>
-    <exit-transition transition_id="retire"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+  </state>
+  <state state_id="technical_analysis" title="technical_analysis">
+    <exit-transition transition_id="propose_analysis"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Acces contents information" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="Modify view template" acquired="False">
-      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Review portal content" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
-      <permission-role>RoadEditor</permission-role>
-      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Description Editor" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
       <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Habitation Editor" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -268,390 +345,589 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Inquiry" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="incomplete" title="incomplete">
-    <exit-transition transition_id="reopen"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+  </state>
+  <state state_id="technical_validation" title="technical_validation">
+    <exit-transition transition_id="validate_analysis"/>
+    <exit-transition transition_id="refuse_analysis"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Acces contents information" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="Modify view template" acquired="False">
-      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Review portal content" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
-      <permission-role>RoadEditor</permission-role>
-      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Description Editor" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Applicant" acquired="False">
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Couple" acquired="False">
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Contact" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Corporation" acquired="False">
+  </state>
+  <state state_id="waiting_for_agreement" title="waiting_for_agreement">
+    <exit-transition transition_id="finalize"/>
+    <exit-transition transition_id="back_to_technical_analysis"/>
+    <exit-transition transition_id="follow_in_court"/>
+    <exit-transition transition_id="close"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Inquiry" acquired="False">
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="refused" title="refused">
-    <exit-transition transition_id="reopen"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+  </state>
+  <state state_id="waiting_to_finalize" title="waiting_to_finalize">
+    <exit-transition transition_id="close"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Acces contents information" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="Modify view template" acquired="False">
-      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Review portal content" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
       <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
-      <permission-role>ExternalReader</permission-role>
-      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
-      <permission-role>RoadEditor</permission-role>
-      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Description Editor" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Habitation Editor" acquired="False">
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
+      <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Applicant" acquired="False">
+    <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Couple" acquired="False">
+    <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Contact" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Corporation" acquired="False">
+  </state>
+  <state state_id="in_court" title="in_court">
+    <exit-transition transition_id="close"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="Access contents information" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Add portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Delete objects" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="List folder contents" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="View" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
+      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Inquiry" acquired="False">
+    <permission-map name="liege.urban: Internal Editor" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Couple" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Contact" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Corporation" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
+      <permission-role>AddressEditor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="inacceptable" title="inacceptable">
-    <exit-transition transition_id="reopen"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+  </state>
+  <state state_id="ended" title="ended">
+    <exit-transition transition_id="reopen"/>
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Acces contents information" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="Modify view template" acquired="False">
-      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
     </permission-map>
-    <permission-map name="Review portal content" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reviewer</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
-      <permission-role>RoadEditor</permission-role>
-      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>InternalReader</permission-role>
     </permission-map>
-    <permission-map name="liege.urban: Description Editor" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
       <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="liege.urban: Habitation Editor" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Couple" acquired="False">
@@ -665,103 +941,103 @@
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Inquiry" acquired="False">
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
-      <permission-role>Manager</permission-role>
-    </permission-map>
-    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-  </state>
-  <state state_id="retired" title="retired">
-    <exit-transition transition_id="reopen"/>
-    <permission-map name="ATContentTypes: Add File" acquired="False">
+    <permission-map name="urban: Add UrbanEventInspectionReport" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="ATContentTypes: Add Image" acquired="False">
+  </state>
+  <state state_id="frozen_suspension" title="frozen_suspension">
+    <permission-map name="ATContentTypes: Add File" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Acces contents information" acquired="False">
+    <permission-map name="ATContentTypes: Add Image" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Access contents information" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="Add portal content" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
     </permission-map>
     <permission-map name="Delete objects" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map name="List folder contents" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
-    </permission-map>
-    <permission-map name="Modify view template" acquired="False">
-      <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
-    <permission-map name="Review portal content" acquired="False">
+    <permission-map name="Modify portal content" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>Reviewer</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="View" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
+      <permission-role>ExternalReader</permission-role>
+      <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: External Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>ExternalReader</permission-role>
       <permission-role>InternalReader</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>Reader</permission-role>
-      <permission-role>RoadEditor</permission-role>
       <permission-role>RoadReader</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Internal Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
@@ -774,98 +1050,131 @@
     <permission-map name="liege.urban: Description Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
       <permission-role>AddressEditor</permission-role>
     </permission-map>
     <permission-map name="liege.urban: Habitation Editor" acquired="False">
+      <permission-role>Manager</permission-role>
+      <permission-role>AddressEditor</permission-role>
+    </permission-map>
+    <permission-map name="liege.urban: Road Editor" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
-      <permission-role>AddressEditor</permission-role>
+      <permission-role>RoadEditor</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Applicant" acquired="False">
+    <permission-map name="liege.urban: Road Reader" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
+      <permission-role>Reader</permission-role>
+      <permission-role>RoadEditor</permission-role>
+      <permission-role>RoadReader</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Couple" acquired="False">
+    <permission-map name="liege.urban: Validate" acquired="False">
+      <permission-role>Contributor</permission-role>
+      <permission-role>Manager</permission-role>
+    </permission-map>
+    <permission-map name="urban: Add Applicant" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Contact" acquired="False">
+    <permission-map name="urban: Add Couple" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Corporation" acquired="False">
+    <permission-map name="urban: Add Contact" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add Inquiry" acquired="False">
+    <permission-map name="urban: Add Corporation" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="urban: Add CODT_UniqueLicenceInquiry" acquired="False">
+    <permission-map name="urban: Add CODT_Inquiry" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add PortionOut" acquired="False">
       <permission-role>AddressEditor</permission-role>
-      <permission-role>Contributor</permission-role>
-      <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEvent" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
     <permission-map name="urban: Add UrbanEventOpinionRequest" acquired="False">
       <permission-role>Contributor</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
-  <transition transition_id="accept" title="accept" new_state="accepted" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="%(portal_url)s/accept.png">accept</action>
+  <transition transition_id="send_to_prosecutor" title="send_to_prosecutor" new_state="prosecution_analysis" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
+  <transition transition_id="follow_to_technical_analysis" title="follow_to_technical_analysis" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
+  <transition transition_id="propose_analysis" title="propose_analysis" new_state="technical_validation" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
+  <transition transition_id="validate_analysis" title="validate_analysis" new_state="waiting_for_agreement" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
+    <guard>
+      <guard-permission>Modify portal content</guard-permission>
+    </guard>
+  </transition>
+  <transition transition_id="refuse_analysis" title="refuse_analysis" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="isincomplete" title="isincomplete" new_state="incomplete" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="%(portal_url)s/isincomplete.png">isincomplete</action>
+  <transition transition_id="finalize" title="finalize" new_state="waiting_to_finalize" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="refuse" title="refuse" new_state="refused" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="%(portal_url)s/refuse.png">refuse</action>
+  <transition transition_id="follow_in_court" title="follow_in_court" new_state="in_court" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="reopen" title="reopen" new_state="in_progress" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="%(portal_url)s/reopen.png">reopen</action>
+  <transition transition_id="back_to_technical_analysis" title="back_to_technical_analysis" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">analyse</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="isinacceptable" title="isinacceptable" new_state="inacceptable" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="%(portal_url)s/isincomplete.png">retire</action>
+  <transition transition_id="close" title="close" new_state="ended" trigger="USER" before_script="" after_script="">
+    <action url="" category="workflow" icon="">close</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="retire" title="retire" new_state="retired" trigger="USER" before_script="" after_script="">
-    <action url="" category="workflow" icon="%(portal_url)s/retire.png">retire</action>
+  <transition transition_id="reopen" title="reopen" new_state="technical_analysis" trigger="USER" before_script="" after_script="">
+    <action url="" icon="" category="workflow">reopen</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
   <variable variable_id="action" for_catalog="False" for_status="True" update_always="True">
     <description>The last transition</description>
     <default>
```

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urbancertificateone_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urbancertificateone_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows/urbandoc_workflow/definition.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows/urbandoc_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows.xml`

 * *Files 1% similar despite different names*

#### Comparing `liege.urban-1.0.2/src/liege/urban/profiles/default/workflows.xml` & `liege.urban-1.0.3/src/liege/urban/profiles/default/workflows.xml`

```diff
@@ -36,16 +36,16 @@
     </type>
     <type type_id="CODT_Article127">
       <bound-workflow workflow_id="article127_workflow"/>
     </type>
     <type type_id="CODT_IntegratedLicence">
       <bound-workflow workflow_id="urban_licence_workflow"/>
     </type>
-    <type type_id="COTD_UrbanCertificateTwo">
-      <bound-workflow workflow_id="cu2_workflow"/>
+    <type type_id="CODT_UrbanCertificateTwo">
+      <bound-workflow workflow_id="codt_buildlicence_workflow"/>
     </type>
     <type type_id="EnvClassOne">
       <bound-workflow workflow_id="envclassone_workflow"/>
     </type>
     <!-- use same workflow for envclassone, envclasstwo and envclassbordering-->
     <type type_id="EnvClassTwo">
       <bound-workflow workflow_id="envclassone_workflow"/>
```

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/conditions.py` & `liege.urban-1.0.3/src/liege/urban/schedule/conditions.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/conditions.zcml` & `liege.urban-1.0.3/src/liege/urban/schedule/conditions.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/article127.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/article127.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/buildlicence.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/buildlicence.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/declaration.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/declaration.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/division.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/division.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/envclassone.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/envclassone.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/envclassthree.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/envclassthree.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/envclasstwo.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/envclasstwo.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/miscdemand.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/miscdemand.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/notaryletter.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/notaryletter.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/parceloutlicence.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/parceloutlicence.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/roaddecree.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/roaddecree.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/survey_schedule.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/survey_schedule.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/urbancertificateone.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/urbancertificateone.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/config/urbancertificatetwo.xml` & `liege.urban-1.0.3/src/liege/urban/schedule/config/urbancertificatetwo.xml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/creation_conditions.py` & `liege.urban-1.0.3/src/liege/urban/schedule/creation_conditions.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/default_states.py` & `liege.urban-1.0.3/src/liege/urban/schedule/default_states.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/default_user.py` & `liege.urban-1.0.3/src/liege/urban/schedule/default_user.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/default_user.zcml` & `liege.urban-1.0.3/src/liege/urban/schedule/default_user.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/end_conditions.py` & `liege.urban-1.0.3/src/liege/urban/schedule/end_conditions.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/indexes.py` & `liege.urban-1.0.3/src/liege/urban/schedule/indexes.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/licence_taskconfig.py` & `liege.urban-1.0.3/src/liege/urban/schedule/licence_taskconfig.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/road_decree_conditions.py` & `liege.urban-1.0.3/src/liege/urban/schedule/road_decree_conditions.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/start_date.py` & `liege.urban-1.0.3/src/liege/urban/schedule/start_date.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/start_date.zcml` & `liege.urban-1.0.3/src/liege/urban/schedule/start_date.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/templates/create_opinions_requests_status.pt` & `liege.urban-1.0.3/src/liege/urban/schedule/templates/create_opinions_requests_status.pt`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/to_icon.py` & `liege.urban-1.0.3/src/liege/urban/schedule/to_icon.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/vocabulary.py` & `liege.urban-1.0.3/src/liege/urban/schedule/vocabulary.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/schedule/vocabulary.zcml` & `liege.urban-1.0.3/src/liege/urban/schedule/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/scripts/convert_ptadresses_to_psql_9.py` & `liege.urban-1.0.3/src/liege/urban/scripts/convert_ptadresses_to_psql_9.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/services/address.py` & `liege.urban-1.0.3/src/liege/urban/services/address.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/setuphandlers.py` & `liege.urban-1.0.3/src/liege/urban/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/skins/liege_images/UrbanEventAcknowledgment.png` & `liege.urban-1.0.3/src/liege/urban/skins/liege_images/UrbanEventAcknowledgment.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/skins/liege_images/UrbanEventPreliminaryAdvice.png` & `liege.urban-1.0.3/src/liege/urban/skins/liege_images/UrbanEventPreliminaryAdvice.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/skins/liege_images/UrbanEventWithEnvironmentValidation.png` & `liege.urban-1.0.3/src/liege/urban/skins/liege_images/UrbanEventWithEnvironmentValidation.png`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/testing.py` & `liege.urban-1.0.3/src/liege/urban/testing.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/testing.zcml` & `liege.urban-1.0.3/src/liege/urban/testing.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/tests/test_robot.py` & `liege.urban-1.0.3/src/liege/urban/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/tests/test_setup.py` & `liege.urban-1.0.3/src/liege/urban/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/FD_opinion_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/FD_opinion_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/acknowledgment_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/acknowledgment_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/address_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/address_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/article127_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/article127_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/buildlicence_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/buildlicence_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/codt_uniquelicence_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/codt_uniquelicence_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/college_event_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/college_event_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/configure.zcml` & `liege.urban-1.0.3/src/liege/urban/workflows/configure.zcml`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/env_validation_event_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/env_validation_event_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/envclassone_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/envclassone_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/envclassthree_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/envclassthree_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/inquiry_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/inquiry_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/inspection_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/inspection_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/inspectionreport_event_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/inspectionreport_event_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/licences_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/licences_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/opinionsrequest_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/opinionsrequest_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/preliminaryadvice_event_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/preliminaryadvice_event_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/preliminarynotice_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/preliminarynotice_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/roaddecree_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/roaddecree_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/ticket_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/ticket_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/urbancertificateone_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/urbancertificateone_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege/urban/workflows/urbanevent_workflow.py` & `liege.urban-1.0.3/src/liege/urban/workflows/urbanevent_workflow.py`

 * *Files identical despite different names*

### Comparing `liege.urban-1.0.2/src/liege.urban.egg-info/PKG-INFO` & `liege.urban-1.0.3/src/liege.urban.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liege.urban
-Version: 1.0.2
+Version: 1.0.3
 Summary: Liège urban profile
 Home-page: https://pypi.python.org/pypi/liege.urban
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -29,14 +29,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.0.3 (2024-04-01)
+------------------
+
+New features:
+
+
+- Add caduc workflow state
+  [jchandelle,mpeeters] (URB-3007)
+- Add frozen workflow state to article127, inspection and ticket
+  [jchandelle] (URB-3023)
+
+
+Bug fixes:
+
+
+- Fix an issue with zope users on urban homepage
+  [mpeeters] (URB-2956)
+
+
 1.0.2 (2023-11-21)
 ------------------
 
 Bug fixes:
 
 
 - Ensure that every licence types can add `UrbanEventMayor` and `UrbanEventAcknowledgment`
```

### Comparing `liege.urban-1.0.2/src/liege.urban.egg-info/SOURCES.txt` & `liege.urban-1.0.3/src/liege.urban.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 src/liege/urban/locales/fr/LC_MESSAGES/plone.po
 src/liege/urban/locales/fr/LC_MESSAGES/urban.mo
 src/liege/urban/locales/fr/LC_MESSAGES/urban.po
 src/liege/urban/migration/__init__.py
 src/liege/urban/migration/configure.zcml
 src/liege/urban/migration/migrate_to_230.py
 src/liege/urban/migration/migrate_to_240.py
+src/liege/urban/migration/utils.py
 src/liege/urban/model/archgenxml_profile.xmi
 src/liege/urban/model/generate.conf
 src/liege/urban/model/generate.sh
 src/liege/urban/model/tmp.zargo
 src/liege/urban/model/workflows.zargo
 src/liege/urban/profiles/__init__.py
 src/liege/urban/profiles/default/__init__.py
```

