# Comparing `tmp/beep_utils-0.0.1.tar.gz` & `tmp/beep_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beep_utils-0.0.1.tar", last modified: Mon Apr  1 20:28:24 2024, max compression
+gzip compressed data, was "beep_utils-0.0.2.tar", last modified: Mon Apr  1 20:52:07 2024, max compression
```

## Comparing `beep_utils-0.0.1.tar` & `beep_utils-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:28:24.415160 beep_utils-0.0.1/
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 20:28:24.415160 beep_utils-0.0.1/PKG-INFO
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:18:26.000000 beep_utils-0.0.1/README.md
-drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:28:24.415160 beep_utils-0.0.1/beep_utils/
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:28:19.000000 beep_utils-0.0.1/beep_utils/__init__.py
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)     3373 2024-04-01 20:28:13.000000 beep_utils-0.0.1/beep_utils/beep_utils.py
-drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:28:24.415160 beep_utils-0.0.1/beep_utils.egg-info/
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 20:28:24.000000 beep_utils-0.0.1/beep_utils.egg-info/PKG-INFO
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      202 2024-04-01 20:28:24.000000 beep_utils-0.0.1/beep_utils.egg-info/SOURCES.txt
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        1 2024-04-01 20:28:24.000000 beep_utils-0.0.1/beep_utils.egg-info/dependency_links.txt
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       11 2024-04-01 20:28:24.000000 beep_utils-0.0.1/beep_utils.egg-info/top_level.txt
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       38 2024-04-01 20:28:24.415160 beep_utils-0.0.1/setup.cfg
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      622 2024-04-01 20:18:35.000000 beep_utils-0.0.1/setup.py
+drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:52:07.845160 beep_utils-0.0.2/
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 20:52:07.845160 beep_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:18:26.000000 beep_utils-0.0.2/README.md
+drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:52:07.845160 beep_utils-0.0.2/beep_utils/
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:29:20.000000 beep_utils-0.0.2/beep_utils/__init__.py
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)     3387 2024-04-01 20:50:45.000000 beep_utils-0.0.2/beep_utils/beep_utils.py
+drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:52:07.845160 beep_utils-0.0.2/beep_utils.egg-info/
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 20:52:07.000000 beep_utils-0.0.2/beep_utils.egg-info/PKG-INFO
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      202 2024-04-01 20:52:07.000000 beep_utils-0.0.2/beep_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        1 2024-04-01 20:52:07.000000 beep_utils-0.0.2/beep_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       11 2024-04-01 20:52:07.000000 beep_utils-0.0.2/beep_utils.egg-info/top_level.txt
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       38 2024-04-01 20:52:07.845160 beep_utils-0.0.2/setup.cfg
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      622 2024-04-01 20:51:34.000000 beep_utils-0.0.2/setup.py
```

### Comparing `beep_utils-0.0.1/beep_utils/beep_utils.py` & `beep_utils-0.0.2/beep_utils/beep_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 class PostgreSQL():
     
     def __init__(self):
         pass
 
-    def create_engine(db_user=None, db_password=None):
+    def create_engine(db_user=None, db_password=None, db_name=None):
         '''
         Função para criar a chave de conexão ao banco de dados.\n
         Caso a conexão seja local (fora do airflow), é necessário incluir usuário e senha.
         '''
         import sqlalchemy
         try:
             from airflow.hooks.base_hook import BaseHook
             connection = BaseHook.get_connection("postgres_beepsaude_gcp")
             engine_bi = sqlalchemy.create_engine(f"postgresql://{connection.login}:{connection.password}@{connection.host}/{connection.schema}", echo=False)
         except ModuleNotFoundError:
             if db_user and db_password:
-                engine_bi = sqlalchemy.create_engine(f"postgresql://{db_user}:{db_password}@data-services.beepapp.com.br/beepsaude", echo=False)
+                engine_bi = sqlalchemy.create_engine(f"postgresql://{db_user}:{db_password}@data-services.beepapp.com.br/{db_name}", echo=False)
             else:
                 print('Inclua usuário e senha.')
         return engine_bi
 
     def postgres_upsert(table, conn, keys, data_iter):
         '''
         Função que permite o pd.to_sql() realizar upsert baseado na chave primária da tabela.\n
```

### Comparing `beep_utils-0.0.1/setup.py` & `beep_utils-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="beep_utils",
-    version="0.0.1",
+    version="0.0.2",
     author="Lucas Pinho",
     description="Beep Saúde ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["beep_utils"],
     classifiers=[
         "Programming Language :: Python :: 3",
```

