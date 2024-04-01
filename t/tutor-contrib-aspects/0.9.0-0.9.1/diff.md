# Comparing `tmp/tutor-contrib-aspects-0.9.0.tar.gz` & `tmp/tutor-contrib-aspects-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.9.0.tar", last modified: Thu Jul  6 15:04:11 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.9.1.tar", last modified: Fri Jul  7 15:00:01 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.9.0.tar` & `tutor-contrib-aspects-0.9.1.tar`

### file list

```diff
@@ -1,120 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/commands_v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/commands_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.657563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.657563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.657563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (123)    45916 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.325908 tutor-contrib-aspects-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-07-07 15:00:01.325908 tutor-contrib-aspects-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 15:00:01.325908 tutor-contrib-aspects-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-07-07 15:00:01.000000 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-07 15:00:01.000000 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:00:01.000000 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 15:00:01.000000 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 15:00:01.000000 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 15:00:01.000000 tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.309907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.309907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.313907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.309907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.309907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.317907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.309907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.321907 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.325908 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Cumulative_enrollments_by_mode_15.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Enrolled_learners_per_day_36.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Enrollment_events_per_day_16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Instructor_dashboard_9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Open_edX_Admin_Dashboard_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/OpenedX_Clickhouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Transcript_closed_captioning_usage_per_video_11.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/Watches_per_video_10.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/course_blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/course_overviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/dim_courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/fact_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/fact_enrollments_by_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/fact_transcript_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/fact_video_plays.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:00:01.325908 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/dim_courses.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/xAPI_events_by_course_11.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/xAPI_problem_events_by_block_7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-07 14:59:52.000000 tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/xapi_events_all_parsed.yaml
```

### Comparing `tutor-contrib-aspects-0.9.0/PKG-INFO` & `tutor-contrib-aspects-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.9.0
+Version: 0.9.1
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -188,15 +188,15 @@
 
 Superset supports creating virtual datasets, which are datasets defined using a SQL query instead of mapping directly to an underlying database object. Aspects leverages virtual datasets, along with `SQL templating <https://superset.apache.org/docs/installation/sql-templating/>`_, to make better use of table indexes.
 
 To make it easier for developers to manage virtual datasets, there is an extra step that can be done on the output of ``tutor aspects serialize``. The ``sql`` section of the dataset yaml can be moved to its own file in the `queries`_ directory and included in the yaml like so:
 
 .. code-block:: yaml
 
-   sql: "{% include 'aspects/apps/superset/pythonpath/queries/query.sql' %}"
+   sql: "{% include 'openedx-assets/queries/query.sql' %}"
 
 
 However, please keep in mind that the assets declaration is itself a jinja template. That means that any jinja used in the dataset definition should be escaped. There are examples of how to handle this in the existing queries, such as `dim_courses.sql`_.
 
 .. _queries: tutoraspects/templates/aspects/apps/superset/pythonpath/queries
 
 .. _dim_courses.sql: tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
```

### Comparing `tutor-contrib-aspects-0.9.0/README.rst` & `tutor-contrib-aspects-0.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
 Superset supports creating virtual datasets, which are datasets defined using a SQL query instead of mapping directly to an underlying database object. Aspects leverages virtual datasets, along with `SQL templating <https://superset.apache.org/docs/installation/sql-templating/>`_, to make better use of table indexes.
 
 To make it easier for developers to manage virtual datasets, there is an extra step that can be done on the output of ``tutor aspects serialize``. The ``sql`` section of the dataset yaml can be moved to its own file in the `queries`_ directory and included in the yaml like so:
 
 .. code-block:: yaml
 
-   sql: "{% include 'aspects/apps/superset/pythonpath/queries/query.sql' %}"
+   sql: "{% include 'openedx-assets/queries/query.sql' %}"
 
 
 However, please keep in mind that the assets declaration is itself a jinja template. That means that any jinja used in the dataset definition should be escaped. There are examples of how to handle this in the existing queries, such as `dim_courses.sql`_.
 
 .. _queries: tutoraspects/templates/aspects/apps/superset/pythonpath/queries
 
 .. _dim_courses.sql: tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
```

### Comparing `tutor-contrib-aspects-0.9.0/setup.py` & `tutor-contrib-aspects-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.9.0
+Version: 0.9.1
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -188,15 +188,15 @@
 
 Superset supports creating virtual datasets, which are datasets defined using a SQL query instead of mapping directly to an underlying database object. Aspects leverages virtual datasets, along with `SQL templating <https://superset.apache.org/docs/installation/sql-templating/>`_, to make better use of table indexes.
 
 To make it easier for developers to manage virtual datasets, there is an extra step that can be done on the output of ``tutor aspects serialize``. The ``sql`` section of the dataset yaml can be moved to its own file in the `queries`_ directory and included in the yaml like so:
 
 .. code-block:: yaml
 
-   sql: "{% include 'aspects/apps/superset/pythonpath/queries/query.sql' %}"
+   sql: "{% include 'openedx-assets/queries/query.sql' %}"
 
 
 However, please keep in mind that the assets declaration is itself a jinja template. That means that any jinja used in the dataset definition should be escaped. There are examples of how to handle this in the existing queries, such as `dim_courses.sql`_.
 
 .. _queries: tutoraspects/templates/aspects/apps/superset/pythonpath/queries
 
 .. _dim_courses.sql: tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
```

### Comparing `tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.9.1/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -57,20 +57,14 @@
 tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
 tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
-tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
-tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
-tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql
-tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
-tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
 tutoraspects/templates/aspects/apps/superset/security/roles.json
 tutoraspects/templates/aspects/apps/vector/file.toml
 tutoraspects/templates/aspects/apps/vector/k8s.toml
 tutoraspects/templates/aspects/apps/vector/local.toml
 tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
 tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
 tutoraspects/templates/aspects/build/.gitignore
@@ -79,8 +73,32 @@
 tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
 tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
 tutoraspects/templates/aspects/jobs/init/.gitignore
 tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
 tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
 tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
 tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
-tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+tutoraspects/templates/openedx-assets/Cumulative_enrollments_by_mode_15.yaml
+tutoraspects/templates/openedx-assets/Enrolled_learners_per_day_36.yaml
+tutoraspects/templates/openedx-assets/Enrollment_events_per_day_16.yaml
+tutoraspects/templates/openedx-assets/Instructor_dashboard_9.yaml
+tutoraspects/templates/openedx-assets/Open_edX_Admin_Dashboard_2.yaml
+tutoraspects/templates/openedx-assets/OpenedX_Clickhouse.yaml
+tutoraspects/templates/openedx-assets/Transcript_closed_captioning_usage_per_video_11.yaml
+tutoraspects/templates/openedx-assets/Watches_per_video_10.yaml
+tutoraspects/templates/openedx-assets/course_blocks.yaml
+tutoraspects/templates/openedx-assets/course_overviews.yaml
+tutoraspects/templates/openedx-assets/dim_courses.yaml
+tutoraspects/templates/openedx-assets/fact_enrollments.yaml
+tutoraspects/templates/openedx-assets/fact_enrollments_by_day.yaml
+tutoraspects/templates/openedx-assets/fact_transcript_usage.yaml
+tutoraspects/templates/openedx-assets/fact_video_plays.yaml
+tutoraspects/templates/openedx-assets/xAPI_events_by_course_11.yaml
+tutoraspects/templates/openedx-assets/xAPI_problem_events_by_block_7.yaml
+tutoraspects/templates/openedx-assets/xapi_events_all_parsed.yaml
+tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+tutoraspects/templates/openedx-assets/queries/dim_courses.sql
+tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
```

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/commands_v0.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/commands_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/commands_v1.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/commands_v1.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.9.1/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,19 @@
         ("RUN_RALPH", True),
         ("RUN_SUPERSET", True),
         ("DOCKER_IMAGE_ASPECTS", "edunext/aspects:{{ ASPECTS_VERSION }}"),
         ("DOCKER_IMAGE_CLICKHOUSE", "clickhouse/clickhouse-server:23.3"),
         ("DOCKER_IMAGE_RALPH", "fundocker/ralph:3.8.0"),
         ("DOCKER_IMAGE_SUPERSET", "edunext/aspects-superset:{{ ASPECTS_VERSION }}"),
         ("DOCKER_IMAGE_VECTOR", "timberio/vector:0.30.0-alpine"),
+        ("DOCKER_IMAGE_OPENEDX", "edunext/openedx-aspects:{{ ASPECTS_VERSION }}"),
+        (
+            "DOCKER_IMAGE_OPENEDX_DEV",
+            "edunext/openedx-aspects-dev:{{ ASPECTS_VERSION }}",
+        ),
         (
             "OPENEDX_EXTRA_PIP_REQUIREMENTS",
             [
                 "openedx-event-sink-clickhouse==0.1.0",
                 "edx-event-routing-backends==5.5.0",
             ],
         ),
```

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/dim_courses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 with courses as (
-    {% include 'aspects/apps/superset/pythonpath/queries/dim_courses.sql' %}
+    {% include 'openedx-assets/queries/dim_courses.sql' %}
 ), enrollments as (
     select
         emission_time,
         org,
         splitByString('/', course_id)[-1] as course_key,
         actor_id,
         enrollment_mode,
```

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 with enrollments as (
-    {% include 'aspects/apps/superset/pythonpath/queries/fact_enrollments.sql' %}
+    {% include 'openedx-assets/queries/fact_enrollments.sql' %}
 ), enrollments_ranked as (
   select
     emission_time,
     org,
     course_name,
     run_name,
     actor_id,
```

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 with videos as (
-    {% include 'aspects/apps/superset/pythonpath/queries/dim_course_videos.sql' %}
+    {% include 'openedx-assets/queries/dim_course_videos.sql' %}
 ), transcripts as (
     select
         emission_time,
         org,
         splitByString('/', course_id)[-1] as course_key,
         video_id,
         actor_id
```

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 with videos as (
-    {% include 'aspects/apps/superset/pythonpath/queries/dim_course_videos.sql' %}
+    {% include 'openedx-assets/queries/dim_course_videos.sql' %}
 ), plays as (
     select
         emission_time,
         org,
         splitByString('/course/', course_id)[-1] as course_key,
         actor_id,
         video_id
```

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.9.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.9.1/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

