# Comparing `tmp/dukes-1.2.1.tar.gz` & `tmp/dukes-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukes-1.2.1.tar", last modified: Mon Apr  1 07:00:58 2024, max compression
+gzip compressed data, was "dukes-1.2.2.tar", last modified: Mon Apr  1 10:43:55 2024, max compression
```

## Comparing `dukes-1.2.1.tar` & `dukes-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 07:00:58.946892 dukes-1.2.1/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-28 13:38:04.000000 dukes-1.2.1/LICENSE
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45463 2024-04-01 07:00:58.946892 dukes-1.2.1/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4474 2024-04-01 06:09:45.000000 dukes-1.2.1/README.md
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1058 2024-04-01 07:00:32.000000 dukes-1.2.1/pyproject.toml
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-04-01 07:00:58.946892 dukes-1.2.1/setup.cfg
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 dukes-1.2.1/setup.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 07:00:58.938892 dukes-1.2.1/src/
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 07:00:58.942892 dukes-1.2.1/src/dukes/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1077 2024-04-01 07:00:32.000000 dukes-1.2.1/src/dukes/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     3146 2024-03-29 18:14:39.000000 dukes-1.2.1/src/dukes/constant.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 07:00:58.942892 dukes-1.2.1/src/dukes/dat/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       13 2024-03-28 13:38:04.000000 dukes-1.2.1/src/dukes/dat/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      619 2024-03-28 13:38:04.000000 dukes-1.2.1/src/dukes/dat/densityParamFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)  1936503 2024-03-28 13:38:04.000000 dukes-1.2.1/src/dukes/dat/galacticAreaDensityFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    19107 2024-04-01 06:38:50.000000 dukes-1.2.1/src/dukes/dukesMain.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     7115 2024-03-30 17:31:11.000000 dukes-1.2.1/src/dukes/galDensity.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     2827 2024-03-28 13:38:04.000000 dukes-1.2.1/src/dukes/galMassFunction.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      806 2024-03-28 13:38:04.000000 dukes-1.2.1/src/dukes/sysmsg.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13200 2024-03-29 17:19:14.000000 dukes-1.2.1/src/dukes/utils.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 07:00:58.946892 dukes-1.2.1/src/dukes.egg-info/
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45463 2024-04-01 07:00:58.000000 dukes-1.2.1/src/dukes.egg-info/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      463 2024-04-01 07:00:58.000000 dukes-1.2.1/src/dukes.egg-info/SOURCES.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-04-01 07:00:58.000000 dukes-1.2.1/src/dukes.egg-info/dependency_links.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-04-01 07:00:58.000000 dukes-1.2.1/src/dukes.egg-info/requires.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        6 2024-04-01 07:00:58.000000 dukes-1.2.1/src/dukes.egg-info/top_level.txt
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 10:43:55.405459 dukes-1.2.2/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-28 13:38:04.000000 dukes-1.2.2/LICENSE
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45463 2024-04-01 10:43:55.405459 dukes-1.2.2/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4474 2024-04-01 06:09:45.000000 dukes-1.2.2/README.md
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1058 2024-04-01 10:43:35.000000 dukes-1.2.2/pyproject.toml
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-04-01 10:43:55.405459 dukes-1.2.2/setup.cfg
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 dukes-1.2.2/setup.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 10:43:55.401459 dukes-1.2.2/src/
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 10:43:55.401459 dukes-1.2.2/src/dukes/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1077 2024-04-01 10:43:35.000000 dukes-1.2.2/src/dukes/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     3146 2024-03-29 18:14:39.000000 dukes-1.2.2/src/dukes/constant.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 10:43:55.401459 dukes-1.2.2/src/dukes/dat/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       13 2024-03-28 13:38:04.000000 dukes-1.2.2/src/dukes/dat/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      619 2024-03-28 13:38:04.000000 dukes-1.2.2/src/dukes/dat/densityParamFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)  1936503 2024-03-28 13:38:04.000000 dukes-1.2.2/src/dukes/dat/galacticAreaDensityFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    19107 2024-04-01 10:15:17.000000 dukes-1.2.2/src/dukes/dukesMain.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     7115 2024-03-30 17:31:11.000000 dukes-1.2.2/src/dukes/galDensity.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     2827 2024-03-28 13:38:04.000000 dukes-1.2.2/src/dukes/galMassFunction.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      806 2024-03-28 13:38:04.000000 dukes-1.2.2/src/dukes/sysmsg.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13195 2024-04-01 10:15:47.000000 dukes-1.2.2/src/dukes/utils.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-01 10:43:55.405459 dukes-1.2.2/src/dukes.egg-info/
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45463 2024-04-01 10:43:55.000000 dukes-1.2.2/src/dukes.egg-info/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      463 2024-04-01 10:43:55.000000 dukes-1.2.2/src/dukes.egg-info/SOURCES.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-04-01 10:43:55.000000 dukes-1.2.2/src/dukes.egg-info/dependency_links.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-04-01 10:43:55.000000 dukes-1.2.2/src/dukes.egg-info/requires.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        6 2024-04-01 10:43:55.000000 dukes-1.2.2/src/dukes.egg-info/top_level.txt
```

### Comparing `dukes-1.2.1/LICENSE` & `dukes-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/PKG-INFO` & `dukes-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukes
-Version: 1.2.1
+Version: 1.2.2
 Summary: This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dukes-1.2.1/README.md` & `dukes-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/pyproject.toml` & `dukes-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukes"
-version = "1.2.1"
+version = "1.2.2"
 description = "This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe"
 readme = "README.md"
 authors = [{ name = "Yen-Hsun Lin", email = "yenhsun@phys.ncku.edu.tw" }]
 license = { file = "LICENSE" }
 dependencies = [
     "numpy >= 1.20.0",
     "scipy >= 1.10.0",
     "vegas >= 6.0.1",]
 requires-python = ">=3.6"
 
 [project.urls]
 Homepage = "https://github.com/yenhsunlin/dukes"
 
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `dukes-1.2.1/src/dukes/__init__.py` & `dukes-1.2.2/src/dukes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 __name__         = 'dukes'
-__version__      = '1.2.1'
+__version__      = '1.2.2'
 __description__  = 'This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe'
 __author__       = 'Yen-Hsun Lin'
 __email__        = 'yenhsun@phys.ncku.edu.tw'
 __url__          = 'https://github.com/yenhsunlin/dukes'
 __license__      = 'GNU GPL-3.0'
 
 from .dukesMain import *
```

### Comparing `dukes-1.2.1/src/dukes/constant.py` & `dukes-1.2.2/src/dukes/constant.py`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/src/dukes/dat/densityParamFit.py` & `dukes-1.2.2/src/dukes/dat/densityParamFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/src/dukes/dat/galacticAreaDensityFit.py` & `dukes-1.2.2/src/dukes/dat/galacticAreaDensityFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/src/dukes/dukesMain.py` & `dukes-1.2.2/src/dukes/dukesMain.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,44 +417,44 @@
         pass
     
     def _diffSpectrum(self,Tx,mx,MG,R,l,theta,thetaCM,is_spike,sigv,tBH,rhosMW,rsMW,eta):
         """
         dNx/dTx
         """
         r = _get_r(l,R,theta)
-        if r >= 1e-8:
+        if 1-8 <= r < 100:
             Ev = snNuEenergy(Tx,mx,thetaCM)
             dEvdTx = _dEv(Tx,mx,thetaCM)
             vx = vBDM(Tx,mx)  #  
             nx = dmNumberDensity(r,mx,MG,is_spike,sigv,tBH,rhosMW,rsMW,eta)
             dsigma0 = constant.sigma0  # differential DM-nu cross section in CM frame, cm^2/sr
             return l**2*_np.sin(theta)*_np.sin(thetaCM)*nx*dsigma0*supernovaNuFlux(Ev,l)*(dEvdTx*vx)
         else:
             return 0
     
     def _dbdmSpectrum(self,z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,tBH,rhosMW,rsMW,eta):
         """
         DBDM spectrume yielded by SN at arbitrary position R
         """
         Txp = (1 + z)*Tx 
-        if Txp < 500:  # discard the BDM signature if it requires Ev > 500 MeV at z 
+        if Txp < 150:  # discard the BDM signature if it requires Ev > 130 MeV at z 
             MG = 10**m
             return MG*rhoDotSFR(z)*dnG(m,z)/_E(z)*self._diffSpectrum(Txp,mx,
                                                                      MG,R,l,theta,
                                                                      thetaCM,
                                                                      is_spike,sigv,tBH,rhosMW,rsMW,eta)
         else:
             return 0
         
     def _dbdmSpectrumWeighted(self,z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,tBH,rhosMW,rsMW,eta,usefit):
         """
         DBDM spectrume yielded by SN at position R weighted by galactic baryonic distribution
         """
         Txp = (1 + z)*Tx 
-        if Txp < 500:  # discard the BDM signature if it requires Ev > 500 MeV at z
+        if Txp < 150:  # discard the BDM signature if it requires Ev > 130 MeV at z
             MG = 10**m
             # adopt fitting data for galactic area density?
             if usefit is True:
                 galArealDensity = galacticAreaDensityFit((R,m))
             elif usefit is False:
                 galArealDensity = galacticAreaDensity(R,zRange=[-10,10],MG=MG)
             else:
@@ -473,15 +473,15 @@
         elif is_weighted is False:
             return self._dbdmSpectrum(z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,tBH,rhosMW,rsMW,eta)
         else:
             raise FlagError('Flag \'is_weighted\' must be a boolean.')
 
 
 def flux(Tx,mx,                                                           \
-         R=0,Rmax=500,rmax=500,tau=10,is_spike=True,is_average=True,      \
+         R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,      \
          sigv=None,tBH=1e9,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True, \
          nitn=10,neval=50000):
     """
     DBDM flux for given (Tx,mx) assuming isotropic and energy-independent
     differential DM-nuetrino cross section in CM frame with the value
     1e-35/4/pi cm^2/std
     
@@ -527,15 +527,15 @@
         flux = 4*_np.pi**2*tau*result*constant.kpc2cm**3*vBDM(Tx,mx)*preFactor
     else:
         raise FlagError('Flag \'is_average\' must be a boolean.')
     return flux
 
 
 def event(mx,                                                                          \
-          TxRange=[5,100],R=0,Rmax=500,rmax=500,tau=10,is_spike=True,is_average=True,  \
+          TxRange=[5,30],R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,  \
           sigv=None,tBH=1e9,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True,             \
           nitn=10,neval=50000):
     """
     DBDM event per electron per second for given mx assuming isotropic
     and energy-independent differential DM-nuetrino cross section in CM
     frame with the value 1e-35/4/pi cm^2/std. The total DM-electron cross
     section is assumed 1e-35 cm^2
```

### Comparing `dukes-1.2.1/src/dukes/galDensity.py` & `dukes-1.2.2/src/dukes/galDensity.py`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/src/dukes/galMassFunction.py` & `dukes-1.2.2/src/dukes/galMassFunction.py`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/src/dukes/sysmsg.py` & `dukes-1.2.2/src/dukes/sysmsg.py`

 * *Files identical despite different names*

### Comparing `dukes-1.2.1/src/dukes/utils.py` & `dukes-1.2.2/src/dukes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,27 +148,27 @@
             return 0
     
     def _dbdmSpectrum(self,z,m,Tx,mx,R,l,theta,thetaCM_vx,is_spike,sigv,tBH,rhosMW,rsMW,eta) -> float:
         """
         DBDM spectrume yielded by SN at arbitrary position R
         """
         Txp = (1 + z)*Tx 
-        if Txp < 200:  # discard the BDM signature if it requires Ev > 200 MeV at z 
+        if Txp < 150:  # discard the BDM signature if it requires Ev > 150 MeV at z 
             MG = 10**m
             return MG*dnG(m,z)/_E(z)*rhoDotSFR(z)*self._diffSpectrum(Txp,mx,MG,R,l,theta,thetaCM_vx,is_spike,sigv,
                                                                      tBH,rhosMW,rsMW,eta)
         else:
             return 0
         
     def _dbdmSpectrumWeighted(self,z,m,Tx,mx,R,l,theta,thetaCM_vx,is_spike,sigv,tBH,rhosMW,rsMW,eta,usefit) -> float:
         """
         DBDM spectrume yielded by SN at position R weighted by galactic baryonic distribution
         """
         Txp = (1 + z)*Tx 
-        if Txp < 200:  # discard the BDM signature if it requires Ev > 200 MeV at z
+        if Txp < 150:  # discard the BDM signature if it requires Ev > 150 MeV at z
             MG = 10**m
             # adopt fitting data for galactic area density?
             if usefit is True:
                 galArealDensity = galacticAreaDensityFit((R,m))
             elif usefit is False:
                 galArealDensity = galacticAreaDensity(R,zRange=[-10,10],MG=MG)
             else:
@@ -176,15 +176,15 @@
             
             return 2*_np.pi*R*galArealDensity*dnG(m,z)/_E(z)*rhoDotSFR(z)*self._diffSpectrum(Tx,mx,MG,R,l,theta,thetaCM_vx, 
                                                                                              is_spike,sigv,tBH,rhosMW,rsMW,eta)
         else:
             return 0
 
     def flux(self,Tx,mx,                                                           
-             R=0,Rmax=500,rmax=500,tau=10,is_spike=True,is_average=True,      
+             R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,      
              sigv=None,tBH=1e9,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True, 
              nitn=10,neval=50000) -> float:
         """
         DBDM flux for given (Tx,mx) for model-dependent DM-nu and DM-e differential cross
         sections
     
         In
@@ -226,15 +226,15 @@
                                 nitn=nitn,neval=neval).mean
             flux = 4*_np.pi**2*tau*result*self.kpc2cm**3*vBDM(Tx,mx)*preFactor
         else:
             raise FlagError('Flag \'is_average\' must be a boolean.')
         return flux
 
     def event(self,mx,                                                                                                                
-          TxRange=[5,100],R=0,Rmax=500,rmax=500,tau=10,is_spike=True,is_average=True,  
+          TxRange=[5,30],R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,  
           sigv=None,tBH=1e9,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True,             
           nitn=10,neval=50000) -> float:
         """
         DBDM event per electron per second for given mx for model-dependent DM-nu and DM-e
         differential cross sections 
     
         In
```

### Comparing `dukes-1.2.1/src/dukes.egg-info/PKG-INFO` & `dukes-1.2.2/src/dukes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukes
-Version: 1.2.1
+Version: 1.2.2
 Summary: This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

