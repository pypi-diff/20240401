# Comparing `tmp/All-in-one-chay-2.4.4.tar.gz` & `tmp/All-in-one-chay-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "All-in-one-chay-2.4.4.tar", last modified: Fri Mar 29 15:14:15 2024, max compression
+gzip compressed data, was "All-in-one-chay-2.4.5.tar", last modified: Mon Apr  1 14:34:38 2024, max compression
```

## Comparing `All-in-one-chay-2.4.4.tar` & `All-in-one-chay-2.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 15:14:15.816642 All-in-one-chay-2.4.4/
--rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 All-in-one-chay-2.4.4/LICENSE
--rw-rw-rw-   0        0        0     1859 2024-03-29 15:14:15.816642 All-in-one-chay-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2024-03-29 15:06:20.000000 All-in-one-chay-2.4.4/README.md
--rw-rw-rw-   0        0        0      622 2024-03-29 14:56:34.000000 All-in-one-chay-2.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 15:14:15.816642 All-in-one-chay-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-03-26 14:30:03.000000 All-in-one-chay-2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:14:15.801010 All-in-one-chay-2.4.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 15:14:15.801010 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/
--rw-rw-rw-   0        0        0     8523 2024-03-29 14:56:19.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/Allinone.py
--rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:14:15.816642 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/
--rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/book.py
--rw-rw-rw-   0        0        0     6351 2024-03-29 14:56:18.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/calculator.py
--rw-rw-rw-   0        0        0     1244 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
--rw-rw-rw-   0        0        0     1695 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/math_cal_py.py
--rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/student_py.py
--rw-rw-rw-   0        0        0     6957 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/tuxing_cal.py
--rw-rw-rw-   0        0        0     2804 2024-02-23 07:22:32.000000 All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/xiaogongju.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:14:15.816642 All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/
--rw-rw-rw-   0        0        0     1859 2024-03-29 15:14:15.000000 All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-03-29 15:14:15.000000 All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 15:14:15.000000 All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-03-29 15:14:15.000000 All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.652609 All-in-one-chay-2.4.5/
+-rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 All-in-one-chay-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0     1859 2024-04-01 14:34:38.650609 All-in-one-chay-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2024-03-29 15:06:20.000000 All-in-one-chay-2.4.5/README.md
+-rw-rw-rw-   0        0        0      622 2024-04-01 14:23:41.000000 All-in-one-chay-2.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:34:38.652609 All-in-one-chay-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-04-01 14:23:43.000000 All-in-one-chay-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.627608 All-in-one-chay-2.4.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.634608 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/
+-rw-rw-rw-   0        0        0     8943 2024-04-01 14:23:02.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/Allinone.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.643609 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/
+-rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/book.py
+-rw-rw-rw-   0        0        0     9096 2024-04-01 14:22:46.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/calculator.py
+-rw-rw-rw-   0        0        0     1244 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+-rw-rw-rw-   0        0        0     1695 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/math_cal_py.py
+-rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/student_py.py
+-rw-rw-rw-   0        0        0     6957 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/tuxing_cal.py
+-rw-rw-rw-   0        0        0     2804 2024-04-01 14:20:26.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/xiaogongju.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.649609 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/
+-rw-rw-rw-   0        0        0     1859 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/top_level.txt
```

### Comparing `All-in-one-chay-2.4.4/LICENSE` & `All-in-one-chay-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/PKG-INFO` & `All-in-one-chay-2.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.4
+Version: 2.4.5
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.3
+Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.4
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `All-in-one-chay-2.4.4/README.md` & `All-in-one-chay-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/pyproject.toml` & `All-in-one-chay-2.4.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "All-in-one-chay"
-version = "2.4.4"
+version = "2.4.5"
 authors = [
   { name="chay", email="lichenyi_2020@qq.com" },
 ]
 description = "多功能一体机（All-in-one）"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.4"
+Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5"
 Issues = "https://github.com/lichenyichay/All-in-one/issues"
```

### Comparing `All-in-one-chay-2.4.4/setup.py` & `All-in-one-chay-2.4.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding:UTF-8
 import setuptools
 
 setuptools.setup(
     name="All-in-one-chay",
-    version="2.4.3",
+    version="2.4.5",
     author="Chay",
     author_email="lichenyi_2020@qq.com",
-    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.3",
+    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5",
     description="All-in-one",
     long_description="多功能一体机",
     python_requires=">=3.0.0",
     # packages=setuptools.find_packages("src"),
     packages_dir={"": "src"},
     packages_data={"": ["*.txt", "*.info", "*.properties"], "": ["data/*.*"]},
     exclude=["*.test", "*.test.*", "test.*", "test"],
```

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/Allinone.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/Allinone.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,24 @@
         return calculator.isfab(args[0])
     elif fuwu=="判断斐波那契回文质数":
         return calculator.isfabhuiwenzhishu(args[0])
     elif fuwu=="判断斐波那契回文数":
         return calculator.isfabhuiwenshu(args[0])
     elif fuwu=="判断斐波那契质数":
         return calculator.isfabparam(args[0])
+    elif fuwu=="求泰波那契序列的第n项":
+        return calculator.tribonacci(args[0])
+    elif fuwu=="判断泰波那契数":
+        return calculator.istribonacci(args[0])
+    elif fuwu=="判断泰波那契回文质数":
+        return calculator.istribonaccihuiwenshuparam(args[0])
+    elif fuwu=="判断泰波那契回文数":
+        return calculator.istribonaccihuiwenshu(args[0])
+    elif fuwu=="判断泰波那契质数":
+        return calculator.istribonacciparam(args[0])
     elif fuwu == "图形计算器":
         while True:
             huida = args[0]
             try:
                 args2=[]
                 for i in range(1,len(args)):
                     args2.append(args[i])
@@ -72,22 +82,21 @@
                     return "不支持该功能！"
             except ValueError:
                 return ("输入无效！")
     elif fuwu == "小学学生信息管理系统":
         student_py.student()
     elif fuwu == "二分查找":
         while True:
-            d = input("请输入是否运行（运行输yes，否则输no）：")
+            d = args[0]
             if d == "yes":
                 a = args
                 b = sorted(a)
                 c = args[-1]
                 diaoyong  = erfenchazhao_py.erfenchazhao(a, b, c)
                 return(diaoyong)
-                sleep(5)
             elif d == "no":
                 return 0
             else:
                 return ("指令无效！")
     elif fuwu == "求余":
         while True:
             try:
```

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/book.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/book.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/calculator.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/calculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 '''
 函数名：FtemporCtemp
 调用形式：a = FtemporCtemp(mode,FtemporCtemp)
 :param mode 模式 ℃to℉（摄氏度转为华氏度）/℉to℃（华氏度转为摄氏度） 模式不在选择范围内会抛出异常
 :return 转换后的温度（不带单位）
 作用：华氏度与摄氏度转换
 '''
-def FtemporCtemp(mode,FtemporCtemp):
+def FtemporCtemp(mode:str,FtemporCtemp:float):
     if mode == "℃to℉":
         return FtemporCtemp*9/5+32
     elif mode == "℉to℃":
         return (FtemporCtemp-32)*5/9
     else:
         raise TypeError("TypeError:模式错误！")
 
@@ -23,15 +23,15 @@
 函数名：duihuan
 调用形式：a = duihuan(mode,money)
 :param mode 模式 1~16 对应不同的货币转换，汇率也不同 模式不在选择范围内会抛出异常
 :param money 要兑换的金额（以模式箭头前的货币单位作为1单位量）
 :return 转换后的货币数量
 作用：货币交换
 '''
-def duihuan(mode,money):
+def duihuan(mode:int,money:float):
     if mode == 1:
         return 0.14 * money #CNY to USD
     elif mode == 2:
         return 20.71 * money #CNY to JPY
     elif mode == 3:
         return 7.2 * money #USD to CNY
     elif mode == 4:
@@ -136,79 +136,85 @@
     if d1==d:
         if isparam(d):
             return True
         else:
             return False
     else:
         return False
+
 '''
 函数名：fab
 调用形式：a = fab(d)
 :param x  类型：int
 :return a[x-1] 斐波那契数列的第x位
 作用：求斐波那契数列的第x位
 '''
-def fab(x):
+def fab(x:int):
     a=[1,1]
     for i in range(2,x):
         a.append(a[i-1]+a[i-2])
     for i in range(x):
         print(a[i]," ")
     return a[x-1]
+
 '''
 函数名：isfab
 调用形式：a = isfab(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否为斐波那契数列中的一个数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数
 '''
-def isfab(x):
+def isfab(x:int):
     a=[1,1]
     for i in range(2,int(math.sqrt(x+2))):
         a.append(a[i-1]+a[i-2])
     if x not in a:
         return False
     else:
         return True
+
 '''
 函数名：isfabparam
 调用形式：a = isfabparam(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否是斐波那契质数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数且为一个质数
 '''
 def isfabparam(x:int):
     if isfab(x) and isparam(x):
         return True
     else:
         return False
+
 '''
 函数名：isfabhuiwenshu
 调用形式：a = isfabhuiwenshu(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否是斐波那契回文数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数且为一个回文数
 '''
 def isfabhuiwenshu(x:int):
     if isfab(x) and ishuiwenshu(x):
         return True
     else:
         return False
+
 '''
 函数名：isfabhuiwenzhishu
 调用形式：a = isfabhuiwenzhishu(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否是斐波那契回文质数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数且为一个回文质数
 '''
 def isfabhuiwenzhishu(x:int):
     if isfab(x) and ishuiwenzhishu(x):
         return True
     else:
         return False
+
 '''
 函数名：isleapyear
 调用形式：a = isleapyear(d)
 :param d  类型：int
 :return x 对应年份是否是闰年 类型：bool(True or False)
 作用：判断闰年
 '''   
@@ -218,8 +224,96 @@
             if x%400==0:
                 return True
             else:
                 return False
         else:
             return True
     else:
+        return False
+
+'''
+泰波那契序列 Tn 定义如下： 
+T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
+函数名：tribonacci
+调用形式：a = tribonacci(d)
+:param x  类型：int
+:return a[x-1] 泰波那契序列的第x位
+作用：求泰波那契序列的第x位
+'''
+def tribonacci(n:int):
+    d=[0,1,1]
+    if n<=2:
+        return d[n]
+    else:
+        for i in range(3,n+1):
+            d.append(d[i-3]+d[i-2]+d[i-1])
+        return d[n]
+
+'''
+泰波那契序列 Tn 定义如下： 
+T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
+函数名：istribonacci
+调用形式：a = istribonacci(d)
+:param x  类型：int
+:return x 是否属于泰波那契序列中的一个数（True or False）
+作用：判断是否属于泰波那契序列中的一个数
+'''
+def istribonacci(n:int):
+    a=[0,1,1]
+    if n>=10000:
+        for i in range(3,int(math.sqrt(n+3))):
+            a.append(a[i-1]+a[i-2]+a[i-3])
+    elif n>=1389537:
+        for i in range(3,int(math.sqrt(int(math.sqrt(n+3))))):
+            a.append(a[i-1]+a[i-2]+a[i-3])
+    else:
+        for i in range(3,int((n+3))):
+            a.append(a[i-1]+a[i-2]+a[i-3])
+    if n not in a:
+        return False
+    else:
+        return True
+
+'''
+泰波那契序列 Tn 定义如下： 
+T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
+函数名：istribonaccihuiwenshu
+调用形式：a = istribonaccihuiwenshu(d)
+:param x  类型：int
+:return x 是否是泰波那契序列回文数（True or False）
+作用：判断泰波那契序列回文数
+'''
+def istribonaccihuiwenshu(n:int):
+    if istribonacci(n) and ishuiwenshu(n):
+        return True
+    else:
+        return False
+
+'''
+泰波那契序列 Tn 定义如下： 
+T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
+函数名：istribonaccihuiwenshuparam
+调用形式：a = istribonaccihuiwenshuparam(d)
+:param x  类型：int
+:return x 是否是泰波那契序列回文质数（True or False）
+作用：判断泰波那契序列回文质数
+'''
+def istribonaccihuiwenshuparam(n:int):
+    if isfabhuiwenshu(n) and isparam(n):
+        return True
+    else:
+        return False
+
+'''
+泰波那契序列 Tn 定义如下： 
+T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
+函数名：istribonacciparam
+调用形式：a = istribonacciparam(d)
+:param x  类型：int
+:return x 是否是泰波那契序列质数（True or False）
+作用：判断泰波那契序列质数
+'''
+def istribonacciparam(n:int):
+    if istribonacci(n) and isparam(n):
+        return True
+    else:
         return False
```

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/math_cal_py.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/math_cal_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/student_py.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/student_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/tuxing_cal.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/tuxing_cal.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/src/All-in-one_chayLichenyi/module/xiaogongju.py` & `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/xiaogongju.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/PKG-INFO` & `All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.4
+Version: 2.4.5
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.3
+Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.4
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `All-in-one-chay-2.4.4/src/All_in_one_chay.egg-info/SOURCES.txt` & `All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

