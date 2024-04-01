# Comparing `tmp/ecuapassdocs-0.63.tar.gz` & `tmp/ecuapassdocs-0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.63.tar", last modified: Sat Mar 23 12:56:29 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.70.tar", last modified: Mon Apr  1 11:20:15 2024, max compression
```

## Comparing `ecuapassdocs-0.63.tar` & `ecuapassdocs-0.70.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.694598 ecuapassdocs-0.63/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-03-23 12:56:29.694598 ecuapassdocs-0.63/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)      335 2024-01-18 22:56:29.000000 ecuapassdocs-0.63/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.574598 ecuapassdocs-0.63/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.574598 ecuapassdocs-0.63/ecuapassdocs/ecuapassutils/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/ecuapassutils/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9831 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/ecuapassutils/pdfcreator.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.582598 ecuapassdocs-0.63/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3223 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    15937 2024-03-22 16:57:06.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     7333 2024-03-21 22:01:04.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    21753 2024-03-22 23:52:50.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1461 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2727 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    23164 2024-03-22 23:53:44.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1652 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1324 2024-03-21 21:54:52.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     5519 2024-03-19 11:55:35.000000 ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.63/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.582598 ecuapassdocs-0.63/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.602598 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.602598 ecuapassdocs-0.63/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.634598 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.670598 ecuapassdocs-0.63/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15104 2024-03-23 12:32:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/declaracion_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18023 2024-03-23 12:39:39.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)    13589 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/old-cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    12706 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/docs/old-manifiesto_input_parameters.json
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.690597 ecuapassdocs-0.63/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1906 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      418 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/resources/images/image-windows-WindowButtons.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.694598 ecuapassdocs-0.63/ecuapassdocs/utils/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/utils/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3896 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/utils/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.63/ecuapassdocs/utils/ecuapass_utils.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-03-23 12:56:29.574598 ecuapassdocs-0.63/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-03-23 12:56:29.000000 ecuapassdocs-0.63/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     6120 2024-03-23 12:56:29.000000 ecuapassdocs-0.63/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-03-23 12:56:29.000000 ecuapassdocs-0.63/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-03-23 12:56:29.000000 ecuapassdocs-0.63/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-03-23 12:56:29.000000 ecuapassdocs-0.63/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-03-23 12:56:29.694598 ecuapassdocs-0.63/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1059 2024-03-23 12:55:39.000000 ecuapassdocs-0.63/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:15.028043 ecuapassdocs-0.70/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-01 11:20:15.028043 ecuapassdocs-0.70/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)      335 2024-01-18 22:56:29.000000 ecuapassdocs-0.70/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.916045 ecuapassdocs-0.70/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.916045 ecuapassdocs-0.70/ecuapassdocs/ecuapassutils/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/ecuapassutils/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9831 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/ecuapassutils/pdfcreator.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.924045 ecuapassdocs-0.70/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3223 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    16127 2024-03-27 16:10:01.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     8031 2024-03-30 21:27:50.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    21748 2024-03-27 16:08:23.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1461 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2709 2024-03-27 15:26:41.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    23164 2024-03-22 23:53:44.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1652 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1324 2024-03-21 21:54:52.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     5519 2024-03-19 11:55:35.000000 ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.70/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.924045 ecuapassdocs-0.70/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.948045 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.948045 ecuapassdocs-0.70/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.972044 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:15.004044 ecuapassdocs-0.70/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15528 2024-03-30 13:16:38.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/declaracion_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/join.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18425 2024-03-30 18:30:32.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.70/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:15.024043 ecuapassdocs-0.70/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1906 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      418 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:15.028043 ecuapassdocs-0.70/ecuapassdocs/utils/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/utils/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3896 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/utils/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.70/ecuapassdocs/utils/ecuapass_utils.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-01 11:20:14.916045 ecuapassdocs-0.70/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-01 11:20:14.000000 ecuapassdocs-0.70/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6148 2024-04-01 11:20:14.000000 ecuapassdocs-0.70/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-04-01 11:20:14.000000 ecuapassdocs-0.70/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-04-01 11:20:14.000000 ecuapassdocs-0.70/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-04-01 11:20:14.000000 ecuapassdocs-0.70/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-04-01 11:20:15.028043 ecuapassdocs-0.70/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1144 2024-04-01 11:19:37.000000 ecuapassdocs-0.70/setup.py
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/ecuapassutils/pdfcreator.py` & `ecuapassdocs-0.70/ecuapassdocs/ecuapassutils/pdfcreator.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_data.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 	#-- Get subject (remitente, destinatario, declarante,..) info
 	#-- Info: nombre, dir, pais, ciudad, id, idNro
 	#-----------------------------------------------------------
 
 	#--  Extracts and replaces IdType and IdNumber from text-------
 	def getReplaceSubjectId (text, subject, replaceString, type):
 		try:
-			if "NIT" not in text.upper() and "RUC" not in text.upper ():
+			if not any (x in text.upper() for x in ["NIT", "RUC", "OTROS"]): 
 				return (text, subject)
 
 			reNumber = r'\d+(?:[.,]*\d*)+' # RE for extracting a float number 
-			reId     = rf"(RUC|NIT)[\s\.:\s]+({reNumber}(?:-\d)?)\s*"
+			reId     = rf"(RUC|NIT|OTROS)[\s.:]+({reNumber}(?:-\d)?)\s*"
 			result	 = re.search (reId, text, flags=re.S)
 		 
 			tipoId   = result.group (1) if result else None
 			numeroId = result.group (2) if result else None
 
 			subject ["tipoId"]   = "OTROS" if tipoId == "NIT" else tipoId
 			subject ["numeroId"] = Utils.convertToEcuapassId (numeroId)
@@ -49,15 +49,15 @@
 		try:
 			rePais = ".*?(ECUADOR|COLOMBIA|PERU)"
 			pais   = Extractor.getValueRE (rePais, text, re.I)
 			info ["pais"] = pais 
 				
 			if (pais):
 				cities = Extractor.getSubjectCitiesString (pais, resourcesPath)
-				reLocation = f"(?P<ciudad>{cities}).*(?P<pais>{pais})\s*"
+				reLocation = f"(?P<ciudad>{cities}).*(?P<pais>{pais})[.\s]*"
 				result = re.search (reLocation, text, flags=re.I)
 				info ["ciudad"] = result.group ("ciudad") if result != None else None
 			else:
 				print (">>>>>> Extracting 'ciudad' from:", text)
 				reCiudad = r"\b(\w+(?:\s+\w+)*)\b"
 				info ["ciudad"] = Extractor.getValueRE (reCiudad, text, re.I)
 
@@ -73,15 +73,15 @@
 		try:
 			rePais = ".*?(ECUADOR|COLOMBIA|PERU)"
 			pais   = Extractor.getValueRE (rePais, text, re.I)
 			subject ["pais"] = pais
 				
 			cities = Extractor.getSubjectCitiesString (pais, resourcesPath)
 
-			reLocation = f"(?P<ciudad>{cities})[\s\-,\s]+(?P<pais>{pais})\s*"
+			reLocation = f"(?P<ciudad>{cities})[\s\-,\s]+(?P<pais>{pais})[.\s]*"
 			result = re.search (reLocation, text, flags=re.I)
 			if (result == None):
 				printx (f"No se pudo localizar o no existe ciudad en: '{text}' de '{type}'")
 			else:
 			#if (type in ["06_Recepcion", "07_Embarque", "08_Entrega", "19_Emision"]):
 				subject ["ciudad"] = result.group ("ciudad") if result else None
 				text	= text.replace (result.group (0), "")
@@ -289,29 +289,28 @@
 		return result
 			
 
 	#------------------------------------------------------------------
 	# Get 'embalaje' from text with number + embalaje: NNN WWWWW
 	#------------------------------------------------------------------
 	def getTipoEmbalaje (text, resourcesPath):
-		embalaje = None
 		try:
 			# Tipo embalaje
 			#embalajeString = Extractor.getDataString ("tipos_embalaje.txt", resourcesPath)
 			#reEmbalaje = rf"\b(PALETAS|{embalajeString})$\b"
 			#reEmbalaje = r"\b(\w+)\b$"    # General string
 			reNumber    = r'\d+(?:[.,]*\d*)+' # RE for extracting a float number 
 			reEmbalaje  = rf"{reNumber}\s+(\b(\w+)\b)"    # String after number
 			embalaje   = Extractor.getValueRE (reEmbalaje, text) 
-			print (f">>> Embalaje: <{embalaje}>")
 			if "PALLETS" in embalaje:
 				embalaje   = "PALETAS"
+			return embalaje.strip ()
 		except:
-			Utils.printException ("Extrayendo embalaje desde el texto:", text)
-		return embalaje
+			Utils.printx (f"No se pudo extraer info embalaje desde texto: '{text}'")
+			return None
 
 	#------------------------------------------------------------------
 	#-- Extract numerical or text date from text ----------------------
 	#------------------------------------------------------------------
 	def getDate (text, resourcesPath):
 		numericalDate = "||LOW"
 		try:
@@ -323,31 +322,35 @@
 			reDay      = r'(?P<day>\d{1,2})'
 			reMonthNum = r'(?P<month>\d{1,2})'
 			reMonthTxt = rf'(?P<month>{monthsString})'
 			reYear     = r'(?P<year>\d[.]?\d{3})'
 			reWordSep  = r'\s+(?:DE|DEL)\s+'
 			reSep      = r'(-|/)'
 
-			reDate1 = rf'\b{reDay}\s*[-]\s*{reMonthNum}\s*[-]\s*{reYear}\b' # 31-12-2023
-			reDate2 = rf'\b{reMonthTxt}\s+{reDay}{reWordSep}{reYear}\b'     # Junio 20 del 2023
-			reDate3 = rf'\b{reDay}{reWordSep}{reMonthTxt}{reWordSep}{reYear}\b' # 20 de Junio del 2023
-			reDate4 = rf'\b{reYear}{reSep}{reMonthNum}{reSep}{reDay}\b' # 2023/31/12
-			reDateOptions = [reDate1, reDate2, reDate3, reDate4]
+			reDate0 = rf'\b{reDay}\s*[-]\s*{reMonthNum}\s*[-]\s*{reYear}\b' # 31-12-2023
+			reDate1 = rf'\b{reMonthTxt}\s+{reDay}{reWordSep}{reYear}\b'     # Junio 20 del 2023
+			reDate2 = rf'\b{reDay}{reWordSep}{reMonthTxt}{reWordSep}{reYear}\b' # 20 de Junio del 2023
+			reDate3 = rf'\b{reYear}{reSep}{reMonthNum}{reSep}{reDay}\b' # 2023/12/31
+			reDate4 = rf'\b{reYear}{reSep}{reMonthTxt}{reSep}{reDay}\b' # 2023/DICIEMBRE/31
+			reDateOptions = [reDate0, reDate1, reDate2, reDate3, reDate4]
 
 			# Evaluate all reDates and select the one with results
 			results = [re.search (x, text, re.I) for (i, x) in enumerate (reDateOptions)]
 			if results [0]:
 				result = results [0]
 				month  = result.group('month')
 			elif results [1] or results [2]:
 				result = results [1] if results [1] else results [2]
 				month  = monthsList.index (result.group('month').upper()) + 1
 			elif results [3]:
 				result = results [3]
 				month  = result.group('month')
+			elif results [4]:
+				result = results [4]
+				month  = monthsList.index (result.group('month').upper()) + 1
 			else:
 				printx (f"No existe fecha en texto '{text}'")
 				return None
 
 			year = result.group ('year').replace (".", "")
 			numericalDate = f"{result.group('day')}-{month}-{year}"
 		except Exception as e:
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,21 +167,40 @@
 					codebinFields [cbinField] = value
 
 			return codebinFields
 		except Exception as e:
 			Utils.printException ("Creando campos de CODEBIN")
 			return None
 
+	#----------------------------------------------------------------
+	#-- Create ECUAPASSDOCS fields from document fields using input parameters
+	#----------------------------------------------------------------
+	def getEcuapassdocsFields (self):
+		try:
+			inputsParams = ResourceLoader.loadJson ("docs", self.inputsParametersFile)
+			docFieldsAll = {}
+			for key in inputsParams:
+				docField   = inputsParams [key]["field"]
+				if docField == "" or "OriginalCopia" in docField:
+					continue
+				else:
+					value = self.getDocumentFieldValue (docField)
+					docFieldsAll [key] = value
+
+			return docFieldsAll
+		except Exception as e:
+			Utils.printException ("Creando campos de ECUAPASSDOCS")
+			return None
 	#-----------------------------------------------------------
 	# Implemented for each class: get the document field value
 	#-----------------------------------------------------------
 	def getDocumentFieldValue (self, docField):
 		value = None
 		if "00_Pais" in docField:
-			paises     = {"CO":"colombia", "EC":"ecuador"}
+			paises     = {"CO":"CO", "EC":"EC"}
 			codigoPais = self.fields [docField]["value"]
 			value      =  paises [codigoPais]
 
 		elif "Gastos" in docField and self.docType == "CARTAPORTE" :
 			fieldName	= docField.split (":")[0]
 			rowName		= docField.split (":")[1].split (",")[0]
 			colName		= docField.split (":")[1].split (",")[1]
@@ -192,7 +211,8 @@
 			fieldValue = self.fields [docField]["value"]
 			value = 1 if "x" in fieldValue or "X" in fieldValue else 0
 
 		else:
 			value = self.fields [docField]["content"]
 
 		return value
+
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,19 +250,19 @@
 		return (location)
 
 	#-----------------------------------------------------------
 	# Get "Entrega" location and suggest a date if it is None
 	#-----------------------------------------------------------
 	def getEntregaLocation (self, key):
 		location = self.getLocationInfo (key)
-		print (">>>> LOCATION: ", location)
 		try:
-			# Add a week to 'embarque' date
+			# Add a week to 'entrega' from 'embarque' date
 			if location ["fecha"] == "||LOW":
 				fechaEmbarque      = self.ecudoc ["34_FechaEmbarque"]
+				print (fechaEmbarque)
 				date_obj           = datetime.strptime (fechaEmbarque, "%d-%m-%Y")
 				new_date_obj       = date_obj  # Fecha actual
 
 				if "BYZA" in self.getNombreEmpresa().upper():
 					new_date_obj       = date_obj + timedelta(weeks=2)   # 15 días
 
 				location ["fecha"] = new_date_obj.strftime("%d-%m-%Y") + "||LOW"
@@ -327,15 +327,15 @@
 	#-----------------------------------------------------------
 	def getBultosInfo (self):
 		bultos = Utils.createEmptyDic (["cantidad", "embalaje", "marcas", "descripcion"])
 		try:
 			# Cantidad
 			text             = self.fields ["10_CantidadClase_Bultos"]["value"]
 			bultos ["cantidad"] = Extractor.getNumber (text)
-			bultos ["embalaje"] = Extractor.getTipoEmbalaje (text, self.fieldsJsonFile).strip()
+			bultos ["embalaje"] = Extractor.getTipoEmbalaje (text, self.fieldsJsonFile)
 
 			# Marcas 
 			text = self.fields ["11_MarcasNumeros_Bultos"]["value"]
 			bultos ["marcas"] = "SIN MARCAS" if text == None else text
 
 			# Descripcion
 			descripcion = self.fields ["12_Descripcion_Bultos"]["content"]
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 			text    = re.sub ("\s*//\s*", "", text)   # For SILOG "//" separator cartaportes
 			text, subject = Extractor.removeSubjectId (text, subject, key)
 			text, subject = Extractor.removeSubjectCiudadPais (text, subject, self.resourcesPath, key)
 			text, subject = Extractor.removeSubjectNombreDireccion (text, subject, key)
 		except:
 			Utils.printException (f"Obteniendo datos del sujeto: '{key}' en el texto", text)
 
-		print (subject)
 		return (subject)
 
 #--------------------------------------------------------------------
 # Call main 
 #--------------------------------------------------------------------
 if __name__ == '__main__':
 	main ()
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/ecuapass_utils.py` & `ecuapassdocs-0.70/ecuapassdocs/info/ecuapass_utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.70/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/cartaporte_input_parameters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'numero'": "OrderedDict([('align', 'left'), ('class', 'input_numero'), ('field', ''), "*

 * *             "('fieldCodebin', ''), ('font', 'large'), ('fontSize', '26px'), ('height', 28), "*

 * *             "('maxChars', 10), ('maxLines', 1), ('restrictions', ['hidden', 'readonly', "*

 * *             "'color=red']), ('value', ''), ('width', 233), ('x', 300), ('y', 88)])"}*

```diff
@@ -15,14 +15,34 @@
             "color=red"
         ],
         "value": "",
         "width": 233,
         "x": 300,
         "y": 88
     },
+    "numero": {
+        "align": "left",
+        "class": "input_numero",
+        "field": "",
+        "fieldCodebin": "",
+        "font": "large",
+        "fontSize": "26px",
+        "height": 28,
+        "maxChars": 10,
+        "maxLines": 1,
+        "restrictions": [
+            "hidden",
+            "readonly",
+            "color=red"
+        ],
+        "value": "",
+        "width": 233,
+        "x": 300,
+        "y": 88
+    },
     "txt00": {
         "align": "left",
         "class": "input_numero",
         "field": "00b_Numero",
         "fieldCodebin": "nocpic",
         "font": "large",
         "fontSize": "26px",
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/declaracion_input_parameters.json` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/declaracion_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/manifiesto_input_parameters.json` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/manifiesto_input_parameters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.979085865115277%*

 * *Differences: {"'numero'": "OrderedDict([('align', 'left'), ('class', 'input_numero'), ('field', ''), "*

 * *             "('fieldCodebin', ''), ('font', 'large'), ('fontSize', '26px'), ('height', 28), "*

 * *             "('maxChars', 10), ('maxLines', 1), ('restrictions', ['hidden', 'readonly', "*

 * *             "'color=red']), ('value', ''), ('width', 233), ('x', 200), ('y', 88)])",*

 * * "'txt00'": "{'restrictions': {delete: [0]}}",*

 * * "'txt29'": "{'maxChars': 52}",*

 * * "'txt40'": "{'height': 22, 'y': 1366}"}*

```diff
@@ -15,26 +15,45 @@
             "color=red"
         ],
         "value": "",
         "width": 233,
         "x": 400,
         "y": 88
     },
+    "numero": {
+        "align": "left",
+        "class": "input_numero",
+        "field": "",
+        "fieldCodebin": "",
+        "font": "large",
+        "fontSize": "26px",
+        "height": 28,
+        "maxChars": 10,
+        "maxLines": 1,
+        "restrictions": [
+            "hidden",
+            "readonly",
+            "color=red"
+        ],
+        "value": "",
+        "width": 233,
+        "x": 200,
+        "y": 88
+    },
     "txt00": {
         "align": "left",
         "class": "input_numero",
         "field": "00b_Numero",
         "fieldCodebin": "",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 12,
         "maxLines": 1,
         "restrictions": [
-            "readonly",
             "color=red"
         ],
         "value": "",
         "width": 203,
         "x": 847,
         "y": 94
     },
@@ -544,15 +563,15 @@
         "align": "left",
         "class": "input_general",
         "field": "29_Mercancia_Descripcion",
         "fieldCodebin": "a29",
         "font": "small",
         "fontSize": "12px",
         "height": 341,
-        "maxChars": 48,
+        "maxChars": 52,
         "maxLines": 20,
         "value": "",
         "width": 380,
         "x": 155,
         "y": 857
     },
     "txt30": {
@@ -738,21 +757,21 @@
     "txt40": {
         "align": "left",
         "class": "input_fecha",
         "field": "40_Fecha_Emision",
         "fieldCodebin": "a40",
         "font": "small",
         "fontSize": "12px",
-        "height": 18,
+        "height": 22,
         "maxChars": 50,
         "maxLines": 1,
         "value": "",
         "width": 350,
         "x": 180,
-        "y": 1370
+        "y": 1366
     },
     "txt41": {
         "align": "center",
         "class": "input_tipo",
         "field": "41_OriginalCopia",
         "fieldCodebin": "",
         "font": "large",
```

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.70/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/utils/ecuapass_feedback.py` & `ecuapassdocs-0.70/ecuapassdocs/utils/ecuapass_feedback.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs/utils/ecuapass_utils.py` & `ecuapassdocs-0.70/ecuapassdocs/utils/ecuapass_utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.63/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.70/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,30 +75,31 @@
 ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
 ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
 ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
 ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
 ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
 ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
 ecuapassdocs/resources/docs/__init__.py
+ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
 ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
 ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
 ecuapassdocs/resources/docs/cartaporte_input_parameters.json
 ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
 ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
 ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
 ecuapassdocs/resources/docs/declaracion_input_parameters.json
 ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
 ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
 ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+ecuapassdocs/resources/docs/join.pdf
 ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
 ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
 ecuapassdocs/resources/docs/manifiesto_input_parameters.json
-ecuapassdocs/resources/docs/old-cartaporte_input_parameters.json
 ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
-ecuapassdocs/resources/docs/old-manifiesto_input_parameters.json
+ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
 ecuapassdocs/resources/images/__init__.py
 ecuapassdocs/resources/images/icon-colombia.png
 ecuapassdocs/resources/images/icon-ecuador.png
 ecuapassdocs/resources/images/icon-white-bot.ico
 ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
 ecuapassdocs/resources/images/image-cartaporte-vacia.png
 ecuapassdocs/resources/images/image-declaracion-ecuapass.png
```

### Comparing `ecuapassdocs-0.63/setup.py` & `ecuapassdocs-0.70/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.63',  # Package version
+    version='0.70',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -16,10 +16,13 @@
 	                               "resources/docs/*"]},
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
-	logs = {"0.63" : "Added creation of CODEBIN fields",
-			"0.60" : "Changed resource names from 'data-XXX' to data_XXX'"},
+	logs = {
+		"0.70" : "Added creation of ECUAPASSDOCS fields. Added numero to parameters",
+		"0.63" : "Added creation of CODEBIN fields",
+		"0.60" : "Changed resource names from 'data-XXX' to data_XXX'"
+		},
 )
```

