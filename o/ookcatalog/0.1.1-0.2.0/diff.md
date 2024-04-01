# Comparing `tmp/ookcatalog-0.1.1.tar.gz` & `tmp/ookcatalog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ookcatalog-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ookcatalog-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ookcatalog-0.1.1.tar` & `ookcatalog-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6567 2024-03-25 22:00:50.388439 ookcatalog-0.1.1/README.md
--rw-r--r--   0        0        0     2039 2024-03-25 22:00:50.388439 ookcatalog-0.1.1/ookcatalog/__init__.py
--rw-r--r--   0        0        0     1651 2024-03-25 22:00:50.388439 ookcatalog-0.1.1/ookcatalog/catalog.py
--rw-r--r--   0        0        0     3549 2024-03-24 17:14:54.231014 ookcatalog-0.1.1/ookcatalog/commands.py
--rw-r--r--   0        0        0    18694 2024-03-30 14:59:04.955366 ookcatalog-0.1.1/ookcatalog/db.py
--rw-r--r--   0        0        0      804 2024-03-21 20:22:07.828265 ookcatalog-0.1.1/ookcatalog/templates/home.html
--rw-r--r--   0        0        0     1740 2024-03-21 20:22:07.828265 ookcatalog-0.1.1/ookcatalog/templates/layout.html
--rw-r--r--   0        0        0      791 2024-03-21 20:22:07.828265 ookcatalog-0.1.1/ookcatalog/templates/search.html
--rw-r--r--   0        0        0     1770 2024-03-22 18:53:21.298932 ookcatalog-0.1.1/ookcatalog/templates/table.html
--rw-r--r--   0        0        0     1653 2024-03-24 14:39:13.706038 ookcatalog-0.1.1/ookcatalog/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2693 2024-03-24 14:39:04.366052 ookcatalog-0.1.1/ookcatalog/translations/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      742 2024-03-30 15:00:41.398123 ookcatalog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7142 1970-01-01 00:00:00.000000 ookcatalog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6567 2024-03-25 22:00:50.388439 ookcatalog-0.2.0/README.md
+-rw-r--r--   0        0        0     2039 2024-03-25 22:00:50.388439 ookcatalog-0.2.0/ookcatalog/__init__.py
+-rw-r--r--   0        0        0     1651 2024-03-25 22:00:50.388439 ookcatalog-0.2.0/ookcatalog/catalog.py
+-rw-r--r--   0        0        0     3549 2024-03-24 17:14:54.231014 ookcatalog-0.2.0/ookcatalog/commands.py
+-rw-r--r--   0        0        0    19204 2024-04-01 13:09:11.388778 ookcatalog-0.2.0/ookcatalog/db.py
+-rw-r--r--   0        0        0     1673 2024-04-01 11:03:40.686560 ookcatalog-0.2.0/ookcatalog/templates/home.html
+-rw-r--r--   0        0        0     1736 2024-04-01 10:23:07.451392 ookcatalog-0.2.0/ookcatalog/templates/layout.html
+-rw-r--r--   0        0        0      791 2024-03-21 20:22:07.828265 ookcatalog-0.2.0/ookcatalog/templates/search.html
+-rw-r--r--   0        0        0     1770 2024-03-22 18:53:21.298932 ookcatalog-0.2.0/ookcatalog/templates/table.html
+-rw-r--r--   0        0        0     1653 2024-03-24 14:39:13.706038 ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2693 2024-03-24 14:39:04.366052 ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      742 2024-04-01 13:13:04.482602 ookcatalog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7142 1970-01-01 00:00:00.000000 ookcatalog-0.2.0/PKG-INFO
```

### Comparing `ookcatalog-0.1.1/README.md` & `ookcatalog-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/__init__.py` & `ookcatalog-0.2.0/ookcatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/catalog.py` & `ookcatalog-0.2.0/ookcatalog/catalog.py`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/commands.py` & `ookcatalog-0.2.0/ookcatalog/commands.py`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/db.py` & `ookcatalog-0.2.0/ookcatalog/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,28 +61,34 @@
 
 
 def db_read_schema(db) -> dict:
     """Read schemas list and associated tables from database.
 
     The SQL request pulls the information from information_schema.tables and aggregates the tables in an array.
     :param db: database connection, it should be the one returned by `get_db()`
-    :return: a dictionary with keys being the name of the schema and values being the list of tables inside this schema
+    :return: a list of all schemas in the database. Each schema is a dictionary with the following keys: 'schema_name',
+    'schema_description' (schema comment), 'tables'. 'tables' is a list of all tables in the schema, and each table is a
+    list with two values: the table name, and the table comment/description.
     """
     with db.cursor() as cur:
         # Reading the schemas from the information schema
         cur.execute(
             """
-        SELECT table_schema as schema_name, array_agg(table_name order by table_name)::text[] as tables
-        FROM information_schema.tables
-        WHERE table_schema NOT IN ('information_schema', 'pg_catalog', 'topology')
-        GROUP BY schema_name
-        ORDER BY schema_name;"""
+            SELECT table_schema                                                   as schema_name,
+                   obj_description(to_regnamespace(table_schema), 'pg_namespace') as schema_description,
+                   array_agg(array [table_name, obj_description(to_regclass(table_schema || '.' || table_name), 'pg_class')]
+                             order by table_name)::text[][]                       as tables
+            FROM information_schema.tables
+            WHERE table_schema NOT IN ('information_schema', 'pg_catalog', 'topology')
+            GROUP BY schema_name
+            ORDER BY schema_name;
+            """
         )
         # Fetching the result
-        schemas = {schema["schema_name"]: schema["tables"] for schema in cur.fetchall()}
+        schemas = cur.fetchall()
         # Sending back the result
         return schemas
 
 
 def db_read_columns(db, schema: str, table: str) -> list[dict]:
     """Read columns name, type and comment for a given schema and table.
 
@@ -135,15 +141,15 @@
         are sorted in calendar order
     """
     with db.cursor() as cur:
         # Reading the table information from the ookcatalog table
         cur.execute(
             """
             SELECT description, description_long, array_agg(updates.month) AS update_months
-            FROM (VALUES (obj_description(to_regclass((%s))))) AS table_comment (description)
+            FROM (VALUES (obj_description(to_regclass((%s)), 'pg_class'))) AS table_comment (description)
                      LEFT JOIN public.ookcatalog AS details ON details.table_schema = (%s) AND details.table_name = (%s)
                      LEFT JOIN LATERAL (SELECT DISTINCT unnest(update_months) AS month ORDER BY month) AS updates ON TRUE
             GROUP BY description, description_long
             """,
             (
                 f"{schema}.{table}",
                 schema,
@@ -201,16 +207,16 @@
                          setweight(to_tsvector(%(text_search_lang)s, table_name), 'A') ||
                          setweight(to_tsvector(%(text_search_lang)s, table_comment), 'A') ||
                          setweight(to_tsvector(%(text_search_lang)s, description_long), 'B') ||
                          setweight(to_tsvector(%(text_search_lang)s, column_names), 'C') ||
                          setweight(to_tsvector(%(text_search_lang)s, column_comments), 'C') as vector
                   FROM (SELECT tables.table_schema,
                                tables.table_name,
-                               coalesce(obj_description(to_regclass(tables.table_schema || '.' || tables.table_name)),
-                                        '')                                  AS table_comment,
+                               coalesce(obj_description(to_regclass(tables.table_schema || '.' || tables.table_name),
+                               'pg_class'), '')                              AS table_comment,
                                coalesce(cat.description_long, '')            AS description_long,
                                coalesce(string_agg(column_name, ' '), '')    as column_names,
                                coalesce(string_agg(column_comment, ' '), '') as column_comments
                         FROM information_schema.tables
                                  LEFT JOIN public.ookcatalog cat
                                            on tables.table_schema = cat.table_schema AND tables.table_name = cat.table_name
                                  CROSS JOIN LATERAL (
@@ -312,15 +318,15 @@
     with db.cursor() as cur:
         cur.execute(  # PostgreSQL request to get table without a comment
             """
             SELECT table_schema,
                    table_name
             FROM information_schema.tables
             WHERE table_schema NOT IN ('information_schema', 'pg_catalog', 'topology')
-              AND obj_description(to_regclass(table_schema || '.' || table_name)) IS NULL
+              AND obj_description(to_regclass(table_schema || '.' || table_name), 'pg_class') IS NULL
             ORDER BY table_schema, table_name
             """
         )
         tables_missing_comment = (
             cur.fetchall()
         )  # Execute the query and fetch the result
         return tables_missing_comment
```

### Comparing `ookcatalog-0.1.1/ookcatalog/templates/layout.html` & `ookcatalog-0.2.0/ookcatalog/templates/layout.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="fr">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@1.0.0/css/bulma.css">
     <title>{% block title %}{% endblock %} | OokCatalog</title>
 </head>
 <body>
 <main>
     <header class="section">
         <div class="container is-max-desktop">
             <nav class="level">
```

### Comparing `ookcatalog-0.1.1/ookcatalog/templates/search.html` & `ookcatalog-0.2.0/ookcatalog/templates/search.html`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/templates/table.html` & `ookcatalog-0.2.0/ookcatalog/templates/table.html`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/translations/fr/LC_MESSAGES/messages.mo` & `ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/ookcatalog/translations/fr/LC_MESSAGES/messages.po` & `ookcatalog-0.2.0/ookcatalog/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ookcatalog-0.1.1/pyproject.toml` & `ookcatalog-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ookcatalog"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     { name="Moté", email="automates@petitmote.fr"}
 ]
 description = "Light and hassle-free PostgreSQL data catalog"
 readme = "README.md"
 licens = {file = "LICENSE.txt"}
 requires-python = ">=3.8"
```

### Comparing `ookcatalog-0.1.1/PKG-INFO` & `ookcatalog-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ookcatalog
-Version: 0.1.1
+Version: 0.2.0
 Summary: Light and hassle-free PostgreSQL data catalog
 Author-email: Moté <automates@petitmote.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

