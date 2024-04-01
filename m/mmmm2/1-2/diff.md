# Comparing `tmp/mmmm2-1.tar.gz` & `tmp/mmmm2-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmmm2-1.tar", last modified: Mon Apr  1 20:19:01 2024, max compression
+gzip compressed data, was "mmmm2-2.tar", last modified: Mon Apr  1 20:22:18 2024, max compression
```

## Comparing `mmmm2-1.tar` & `mmmm2-2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:19:01.608039 mmmm2-1/
--rw-rw-rw-   0        0        0       98 2024-04-01 20:19:01.607038 mmmm2-1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 20:19:01.590785 mmmm2-1/mmmm2/
--rw-rw-rw-   0        0        0     9952 2024-04-01 20:17:14.000000 mmmm2-1/mmmm2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:19:01.607038 mmmm2-1/mmmm2.egg-info/
--rw-rw-rw-   0        0        0       98 2024-04-01 20:19:01.000000 mmmm2-1/mmmm2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-01 20:19:01.000000 mmmm2-1/mmmm2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:19:01.000000 mmmm2-1/mmmm2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-01 20:19:01.000000 mmmm2-1/mmmm2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-04-01 20:19:01.000000 mmmm2-1/mmmm2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 20:19:01.609039 mmmm2-1/setup.cfg
--rw-rw-rw-   0        0        0      208 2024-04-01 20:18:32.000000 mmmm2-1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:18.472610 mmmm2-2/
+-rw-rw-rw-   0        0        0       98 2024-04-01 20:22:18.472610 mmmm2-2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:18.461783 mmmm2-2/mmmm2/
+-rw-rw-rw-   0        0        0     9956 2024-04-01 20:22:05.000000 mmmm2-2/mmmm2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:18.471107 mmmm2-2/mmmm2.egg-info/
+-rw-rw-rw-   0        0        0       98 2024-04-01 20:22:18.000000 mmmm2-2/mmmm2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-01 20:22:18.000000 mmmm2-2/mmmm2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:22:18.000000 mmmm2-2/mmmm2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-01 20:22:18.000000 mmmm2-2/mmmm2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-04-01 20:22:18.000000 mmmm2-2/mmmm2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:22:18.473611 mmmm2-2/setup.cfg
+-rw-rw-rw-   0        0        0      208 2024-04-01 20:21:27.000000 mmmm2-2/setup.py
```

### Comparing `mmmm2-1/mmmm2/__init__.py` & `mmmm2-2/mmmm2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,21 +227,23 @@
 Lagr = p*Y - w*L - r*K
 L_max = solve(diff(Lagr, L), L)[0]
 display((Y.subs(L, L_max)))
     '''
     return pc.copy(s)
 
 
-def kobb_duglas_y0():    s = '''L, K, alpha, beta, lamda= symbols('L, K, alpha, beta, lamda')
+def kobb_duglas_y0():
+    s = '''L, K, alpha, beta, lamda= symbols('L, K, alpha, beta, lamda')
 alpha, beta = 0.7, 0.5  #опциональноY = K **alpha*L**beta
 w = 4
 r = 6C = w*L + r*K
 Y0 = 420Lagrange = w*L + r*K + lamda*(Y0 - Y)
 Sl = nsolve([diff(Lagrange, K), diff(Lagrange, L), diff(Lagrange, lamda)], [L, K, lamda], [1, 1, 1], dict = True)[0]print(Sl)
 L, K, alpha, beta, lamda= symbols('L, K, alpha, beta, lamda')Y = K **alpha*L**beta
 MPK = diff(Y, K)display(MPK)
 MPL = diff(Y, L)display(MPL)
 MRS = MPL/MPKdisplay(MRS)
 #Показатель степени $α$ показывает, насколько сильно выпуск зависит от количества используемого капитала.#Чем больше значение $α$, тем больше влияние капитала на объём производства.
 Показатель степени $β$ показывает, насколько сильно выпуск зависит от количества используемого труда.
-#Чем больше значение $β$, тем больше влияние труда на объём производства.    '''
+#Чем больше значение $β$, тем больше влияние труда на объём производства.
+    '''
     return pc.copy(s)
```

