# Comparing `tmp/intel-power-control-1.0.1.tar.gz` & `tmp/intel-power-control-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel-power-control-1.0.1.tar", last modified: Mon Mar 11 20:50:41 2024, max compression
+gzip compressed data, was "intel-power-control-1.0.2.tar", last modified: Mon Apr  1 21:32:16 2024, max compression
```

## Comparing `intel-power-control-1.0.1.tar` & `intel-power-control-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:50:41.559969 intel-power-control-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:50:41.555969 intel-power-control-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:50:41.555969 intel-power-control-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/.github/workflows/code-quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-11 20:50:41.559969 intel-power-control-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    32617 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/intel-power-control
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/intel-power-control-helper.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1910 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/intel-power-control-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:50:41.559969 intel-power-control-1.0.1/intel_power_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-11 20:50:41.000000 intel-power-control-1.0.1/intel_power_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-11 20:50:41.000000 intel-power-control-1.0.1/intel_power_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 20:50:41.000000 intel-power-control-1.0.1/intel_power_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 20:50:41.000000 intel-power-control-1.0.1/intel_power_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-11 20:50:41.000000 intel-power-control-1.0.1/intel_power_control.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:50:41.559969 intel-power-control-1.0.1/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/misc/intel-power-control.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/misc/intel-power-control.png
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/misc/intel-power-control.sudoers
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/misc/intel-power-control.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48877 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/misc/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 20:50:41.559969 intel-power-control-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-11 20:50:33.000000 intel-power-control-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:32:16.339810 intel-power-control-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:32:16.335810 intel-power-control-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:32:16.339810 intel-power-control-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/.github/workflows/code-quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-01 21:32:16.339810 intel-power-control-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34057 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/intel-power-control
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/intel-power-control-helper.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1910 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/intel-power-control-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:32:16.339810 intel-power-control-1.0.2/intel_power_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-01 21:32:16.000000 intel-power-control-1.0.2/intel_power_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-01 21:32:16.000000 intel-power-control-1.0.2/intel_power_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:32:16.000000 intel-power-control-1.0.2/intel_power_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:32:16.000000 intel-power-control-1.0.2/intel_power_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 21:32:16.000000 intel-power-control-1.0.2/intel_power_control.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:32:16.339810 intel-power-control-1.0.2/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/misc/intel-power-control.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/misc/intel-power-control.png
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/misc/intel-power-control.sudoers
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/misc/intel-power-control.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48877 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/misc/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:32:16.339810 intel-power-control-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-01 21:32:07.000000 intel-power-control-1.0.2/setup.py
```

### Comparing `intel-power-control-1.0.1/.github/workflows/code-quality.yml` & `intel-power-control-1.0.2/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/.github/workflows/publish-to-test-pypi.yml` & `intel-power-control-1.0.2/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/LICENSE` & `intel-power-control-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/Makefile` & `intel-power-control-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/PKG-INFO` & `intel-power-control-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-power-control
-Version: 1.0.1
+Version: 1.0.2
 Summary: GPU power management for Intel hardware on Linux
 Home-page: https://github.com/jmechnich/intel-power-control
 Author: Joerg Mechnich
 Author-email: joerg.mechnich@gmail.com
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `intel-power-control-1.0.1/README.md` & `intel-power-control-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/intel-power-control` & `intel-power-control-1.0.2/intel-power-control`

 * *Files 4% similar despite different names*

```diff
@@ -156,167 +156,181 @@
         if self.systray and self.minimizetray.isChecked():
             ev.ignore()
             self.hide()
         else:
             ev.accept()
 
     def initCPUs(self):
+        self.cpulabels = {}
         box = QGroupBox("CPU State")
         layout = QHBoxLayout()
-        self.cpulabels = {}
-        cpus = [
-            c for c in os.listdir(self.cpubasepath) if re.match(r"^cpu\d+$", c)
-        ]
-        self.cpumapper = QSignalMapper()
-        for i in natural_sort(cpus):
-            l = QPushButton(i)
-            if not self.suidhelper:
-                l.setDisabled(True)
-            self.cpumapper.setMapping(l, i)
-            l.clicked.connect(self.cpumapper.map)
+        if not os.path.isdir(self.cpubasepath):
+            l = QLabel(f"No cpu info at '{self.cpubasepath}'")
             layout.addWidget(l)
-            self.cpulabels[i] = (l, "green")
-        self.cpumapper.mappedString.connect(self.toggleCPU)
+        else:
+            cpus = [
+                c for c in os.listdir(self.cpubasepath) if re.match(r"^cpu\d+$", c)
+            ]
+            self.cpumapper = QSignalMapper()
+            for i in natural_sort(cpus):
+                l = QPushButton(i)
+                if not self.suidhelper:
+                    l.setDisabled(True)
+                self.cpumapper.setMapping(l, i)
+                l.clicked.connect(self.cpumapper.map)
+                layout.addWidget(l)
+                self.cpulabels[i] = (l, "green")
+            self.cpumapper.mappedString.connect(self.toggleCPU)
         box.setLayout(layout)
         self.layout.addWidget(box)
 
     def initThermals(self):
-        box = QGroupBox("Thermal Zones")
-        layout = QGridLayout()
         self.thermals = {}
-        thermals = [
-            t.strip()
-            for t in os.listdir(self.thermalbasepath)
-            if t.startswith("thermal_zone")
-        ]
-        layout.addWidget(QLabel("Temperature"), 0, 1)
-        layout.addWidget(QLabel("Type"), 0, 2)
-        i = 1
-        for t in sorted(thermals):
-            layout.addWidget(QLabel(t), i, 0)
-            tlabel = QLabel("0°C")
-            layout.addWidget(tlabel, i, 1)
-            typename = self.readValue(
-                os.path.join(self.thermalbasepath, t, "type")
-            )
-            layout.addWidget(QLabel(typename), i, 2)
-            self.thermals[t] = (tlabel, 0, typename)
-            i += 1
-        layout.setColumnStretch(2, 1)
+        box = QGroupBox("Thermal Zones")
+        if not os.path.isdir(self.thermalbasepath):
+            layout = QHBoxLayout()
+            l = QLabel(f"No thermal zone info at '{self.thermalbasepath}'")
+            layout.addWidget(l)
+        else:
+            layout = QGridLayout()
+            thermals = [
+                t.strip()
+                for t in os.listdir(self.thermalbasepath)
+                if t.startswith("thermal_zone")
+            ]
+            layout.addWidget(QLabel("Temperature"), 0, 1)
+            layout.addWidget(QLabel("Type"), 0, 2)
+            i = 1
+            for t in sorted(thermals):
+                layout.addWidget(QLabel(t), i, 0)
+                tlabel = QLabel("0°C")
+                layout.addWidget(tlabel, i, 1)
+                typename = self.readValue(
+                    os.path.join(self.thermalbasepath, t, "type")
+                )
+                layout.addWidget(QLabel(typename), i, 2)
+                self.thermals[t] = (tlabel, 0, typename)
+                i += 1
+            layout.setColumnStretch(2, 1)
         box.setLayout(layout)
         self.layout.addWidget(box)
 
     def initGPUs(self):
-        box = QGroupBox("GPU Clock")
-        layout = QGridLayout()
         self.gpulabels = {}
         self.gpusliders = {}
-        gpulabels = [
-            g for g in os.listdir(self.gpubasepath) if re.match(r"^card\d$", g)
-        ]
-        self.gpuminmapper = QSignalMapper()
-        self.gpumaxmapper = QSignalMapper()
-        self.gpuboostmapper = QSignalMapper()
-        layout.addWidget(QLabel("Current"), 0, Cols.CUR + 1)
-        layout.addWidget(QLabel("Minimum"), 0, Cols.MIN + 1)
-        layout.addWidget(QLabel("Maximum"), 0, Cols.MAX + 1)
-        layout.addWidget(QLabel("Boost"), 0, Cols.BST + 1)
-        row = 1
-        for card in sorted(gpulabels):
-            dirname = os.path.join(self.gpubasepath, card)
-            # check if card vendor is Intel
-            with open(os.path.join(dirname, "device", "vendor")) as f:
-                vendor = f.readline().strip()
-            if vendor != "0x8086":
-                continue
-            # check for minimal control file availability
-            if not os.path.exists(os.path.join(dirname, "gt_cur_freq_mhz")):
-                continue
-            if not os.path.exists(os.path.join(dirname, "gt_min_freq_mhz")):
-                continue
-            if not os.path.exists(os.path.join(dirname, "gt_max_freq_mhz")):
-                continue
-            if not os.path.exists(os.path.join(dirname, "gt_boost_freq_mhz")):
-                continue
-            layout.addWidget(QLabel(card), row, 0)
-            l0 = QLabel("0 MHz")
-            layout.addWidget(l0, row, Cols.CUR + 1)
-            l1 = QLabel("0 MHz")
-            layout.addWidget(l1, row, Cols.MIN + 1)
-            l2 = QLabel("0 MHz")
-            layout.addWidget(l2, row, Cols.MAX + 1)
-            l3 = QLabel("0 MHz")
-            layout.addWidget(l3, row, Cols.BST + 1)
-            self.gpulabels[card] = ((l0, 0), (l1, 0), (l2, 0), (l3, 0))
-            gts = [g for g in os.listdir(dirname) if g.startswith("gt_RP")]
-            if not len(gts):
-                continue
-
-            states = {}
-            for g in gts:
-                state = re.match(r"gt_(RP[n\d])_freq_mhz", g).groups()[0]
-                states[state] = self.readValue(os.path.join(dirname, g))
-            rps = sorted(states.keys())
-            rps_max = int(states[rps[0]])
-            rps_min = int(states[rps[-1]])
-            row += 1
-            minslider = QSlider(Qt.Orientation.Horizontal)
-            minslider.setRange(
-                round(rps_min / self.gpuclkdiv), round(rps_max / self.gpuclkdiv)
-            )
-            minslider.setTickPosition(QSlider.TickPosition.TicksBelow)
-            minslider.setTickInterval(1)
-            minslider.setPageStep(1)
-            if not self.suidhelper:
-                minslider.setDisabled(True)
-            self.gpuminmapper.setMapping(minslider, card)
-            minslider.valueChanged.connect(self.gpuminmapper.map)
-            layout.addWidget(minslider, row, 1, 1, len(Cols))
-            row += 1
-            maxslider = QSlider(Qt.Orientation.Horizontal)
-            maxslider.setRange(
-                round(rps_min / self.gpuclkdiv), round(rps_max / self.gpuclkdiv)
-            )
-            maxslider.setTickPosition(QSlider.TickPosition.TicksBelow)
-            maxslider.setTickInterval(1)
-            maxslider.setPageStep(1)
-            if not self.suidhelper:
-                maxslider.setDisabled(True)
-            self.gpumaxmapper.setMapping(maxslider, card)
-            maxslider.valueChanged.connect(self.gpumaxmapper.map)
-            layout.addWidget(maxslider, row, 1, 1, len(Cols))
-            row += 1
-            boostslider = QSlider(Qt.Orientation.Horizontal)
-            boostslider.setRange(
-                round(rps_min / self.gpuclkdiv), round(rps_max / self.gpuclkdiv)
-            )
-            boostslider.setTickPosition(QSlider.TickPosition.TicksBelow)
-            boostslider.setTickInterval(1)
-            boostslider.setPageStep(1)
-            if not self.suidhelper:
-                boostslider.setDisabled(True)
-            self.gpuboostmapper.setMapping(boostslider, card)
-            boostslider.valueChanged.connect(self.gpuboostmapper.map)
-            resetBtn = QPushButton("Reset")
-            resetBtn.clicked.connect(
-                lambda: (
-                    minslider.setValue(minslider.minimum()),
-                    maxslider.setValue(maxslider.maximum()),
-                    boostslider.setValue(boostslider.maximum()),
+        box = QGroupBox("GPU Clock")
+        if not os.path.isdir(self.thermalbasepath):
+            layout = QHBoxLayout()
+            l = QLabel(f"No gpu info at '{self.gpubasepath}'")
+            layout.addWidget(l)
+        else:
+            layout = QGridLayout()
+            gpulabels = [
+                g for g in os.listdir(self.gpubasepath) if re.match(r"^card\d$", g)
+            ]
+            self.gpuminmapper = QSignalMapper()
+            self.gpumaxmapper = QSignalMapper()
+            self.gpuboostmapper = QSignalMapper()
+            layout.addWidget(QLabel("Current"), 0, Cols.CUR + 1)
+            layout.addWidget(QLabel("Minimum"), 0, Cols.MIN + 1)
+            layout.addWidget(QLabel("Maximum"), 0, Cols.MAX + 1)
+            layout.addWidget(QLabel("Boost"), 0, Cols.BST + 1)
+            row = 1
+            for card in sorted(gpulabels):
+                dirname = os.path.join(self.gpubasepath, card)
+                # check if card vendor is Intel
+                with open(os.path.join(dirname, "device", "vendor")) as f:
+                    vendor = f.readline().strip()
+                if vendor != "0x8086":
+                    continue
+                # check for minimal control file availability
+                if not os.path.exists(os.path.join(dirname, "gt_cur_freq_mhz")):
+                    continue
+                if not os.path.exists(os.path.join(dirname, "gt_min_freq_mhz")):
+                    continue
+                if not os.path.exists(os.path.join(dirname, "gt_max_freq_mhz")):
+                    continue
+                if not os.path.exists(os.path.join(dirname, "gt_boost_freq_mhz")):
+                    continue
+                layout.addWidget(QLabel(card), row, 0)
+                l0 = QLabel("0 MHz")
+                layout.addWidget(l0, row, Cols.CUR + 1)
+                l1 = QLabel("0 MHz")
+                layout.addWidget(l1, row, Cols.MIN + 1)
+                l2 = QLabel("0 MHz")
+                layout.addWidget(l2, row, Cols.MAX + 1)
+                l3 = QLabel("0 MHz")
+                layout.addWidget(l3, row, Cols.BST + 1)
+                self.gpulabels[card] = ((l0, 0), (l1, 0), (l2, 0), (l3, 0))
+                gts = [g for g in os.listdir(dirname) if g.startswith("gt_RP")]
+                if not len(gts):
+                    continue
+
+                states = {}
+                for g in gts:
+                    state = re.match(r"gt_(RP[n\d])_freq_mhz", g).groups()[0]
+                    states[state] = self.readValue(os.path.join(dirname, g))
+                rps = sorted(states.keys())
+                rps_max = int(states[rps[0]])
+                rps_min = int(states[rps[-1]])
+                row += 1
+                minslider = QSlider(Qt.Orientation.Horizontal)
+                minslider.setRange(
+                    round(rps_min / self.gpuclkdiv), round(rps_max / self.gpuclkdiv)
                 )
-            )
-            layout.addWidget(resetBtn, row, 0)
-            layout.addWidget(boostslider, row, 1, 1, len(Cols))
-            row += 1
-            self.gpusliders[card] = (minslider, maxslider, boostslider)
-        self.gpuminmapper.mappedString.connect(self.setMinimumClock)
-        self.gpumaxmapper.mappedString.connect(self.setMaximumClock)
-        self.gpuboostmapper.mappedString.connect(self.setBoostClock)
-        # layout.setColumnStretch(3,1)
-        layout.setHorizontalSpacing(10)
+                minslider.setTickPosition(QSlider.TickPosition.TicksBelow)
+                minslider.setTickInterval(1)
+                minslider.setPageStep(1)
+                if not self.suidhelper:
+                    minslider.setDisabled(True)
+                self.gpuminmapper.setMapping(minslider, card)
+                minslider.valueChanged.connect(self.gpuminmapper.map)
+                layout.addWidget(minslider, row, 1, 1, len(Cols))
+                row += 1
+                maxslider = QSlider(Qt.Orientation.Horizontal)
+                maxslider.setRange(
+                    round(rps_min / self.gpuclkdiv), round(rps_max / self.gpuclkdiv)
+                )
+                maxslider.setTickPosition(QSlider.TickPosition.TicksBelow)
+                maxslider.setTickInterval(1)
+                maxslider.setPageStep(1)
+                if not self.suidhelper:
+                    maxslider.setDisabled(True)
+                self.gpumaxmapper.setMapping(maxslider, card)
+                maxslider.valueChanged.connect(self.gpumaxmapper.map)
+                layout.addWidget(maxslider, row, 1, 1, len(Cols))
+                row += 1
+                boostslider = QSlider(Qt.Orientation.Horizontal)
+                boostslider.setRange(
+                    round(rps_min / self.gpuclkdiv), round(rps_max / self.gpuclkdiv)
+                )
+                boostslider.setTickPosition(QSlider.TickPosition.TicksBelow)
+                boostslider.setTickInterval(1)
+                boostslider.setPageStep(1)
+                if not self.suidhelper:
+                    boostslider.setDisabled(True)
+                self.gpuboostmapper.setMapping(boostslider, card)
+                boostslider.valueChanged.connect(self.gpuboostmapper.map)
+                resetBtn = QPushButton("Reset")
+                resetBtn.clicked.connect(
+                    lambda: (
+                        minslider.setValue(minslider.minimum()),
+                        maxslider.setValue(maxslider.maximum()),
+                        boostslider.setValue(boostslider.maximum()),
+                    )
+                )
+                layout.addWidget(resetBtn, row, 0)
+                layout.addWidget(boostslider, row, 1, 1, len(Cols))
+                row += 1
+                self.gpusliders[card] = (minslider, maxslider, boostslider)
+            self.gpuminmapper.mappedString.connect(self.setMinimumClock)
+            self.gpumaxmapper.mappedString.connect(self.setMaximumClock)
+            self.gpuboostmapper.mappedString.connect(self.setBoostClock)
+            # layout.setColumnStretch(3,1)
+            layout.setHorizontalSpacing(10)
         box.setLayout(layout)
         self.layout.addWidget(box)
 
     def brightnessAvailable(self):
         if not os.path.exists(self.backlightpath):
             return False
         if not os.path.exists(os.path.join(self.backlightpath, "brightness")):
@@ -438,38 +452,36 @@
         s = QSettings()
         s.setValue(name, state)
 
     def toggleSyncBoostToMax(self, state):
         self.syncboosttomax.setChecked(state)
         for k, v in self.gpusliders.items():
             v[Vars.BST].setEnabled(not state)
-        s = QSettings()
-        s.setValue("syncboosttomax", int(state))
+        self.updateSettings("syncboosttomax", int(state))
 
     def toggleAlwaysOnTop(self, state):
         self.alwaysontop.setChecked(state)
         hidden = self.isHidden()
         flags = self.windowFlags()
         if state:
             flags |= Qt.WindowType.WindowStaysOnTopHint
         else:
             flags &= ~Qt.WindowType.WindowStaysOnTopHint
         self.setWindowFlags(flags)
         if not hidden:
             self.show()
-        s = QSettings()
-        s.setValue("alwaysontop", int(state))
+        self.updateSettings("alwaysontop", int(state))
 
     def createSystray(self):
         if not QSystemTrayIcon.isSystemTrayAvailable():
             return
         if self.systray:
             self.destroySystray()
         self.systray = QSystemTrayIcon()
-        pix = QPixmap(22, 22)
+        pix = QPixmap(self.systraySize, self.systraySize)
         pix.fill(QColorConstants.Transparent)
         self.systray.setIcon(QIcon(pix))
         self.systray.activated.connect(self.systrayActivated)
         m = QMenu()
         m.addAction("Quit", QApplication.quit)
         self.systray.setContextMenu(m)
         self.systray.show()
@@ -485,29 +497,32 @@
         self.showsystray.setChecked(state)
         self.minimizetray.setEnabled(state)
         self.starthidden.setEnabled(state)
         if state:
             self.createSystray()
         else:
             self.destroySystray()
-        s = QSettings()
-        s.setValue("systray", int(state))
+        self.updateSettings("systray", int(state))
 
     def systrayActivated(self, reason):
         if reason == QSystemTrayIcon.ActivationReason.Trigger:
             if self.isHidden():
                 self.show()
             else:
                 self.hide()
 
     def loadSettings(self):
         self.status.showMessage("Loading settings", self.msgtimeout)
         s = QSettings()
         self.fgColor = QColor(s.value("fgColor", QColor("#33b0dc")))
         self.bgColor = QColor(s.value("bgColor", QColor("#144556")))
+        self.fontSize = int(s.value("fontsize", 6))
+        self.systraySize = int(s.value("systraysize", 22))
+        self.updateSettings("fontsize", self.fontSize)
+        self.updateSettings("systraysize", self.systraySize)
         self.setMaxTemp(int(s.value("maxtemp", 80)))
         self.setHyst(int(s.value("hyst", -5)))
         self.toggleThrottling(int(s.value("throttlegpu", 1)))
         self.setActiveThermal(int(s.value("tzindex", -1)))
         self.toggleSyncBoostToMax(int(s.value("syncboosttomax", 0)))
         self.toggleAlwaysOnTop(int(s.value("alwaysontop", 0)))
         self.toggleSystray(int(s.value("systray", 0)))
@@ -518,57 +533,53 @@
         self.maxtemp.setValue(newmax)
         for k, v in self.thermals.items():
             label, val, typename = v
             stylesheet = "QLabel { color: %s }" % (
                 hexColor(self.textColor) if val < newmax else "red"
             )
             label.setStyleSheet(stylesheet)
-        s = QSettings()
-        s.setValue("maxtemp", newmax)
+        self.updateSettings("maxtemp", newmax)
 
     def setHyst(self, hyst):
         self.hyst.setValue(hyst)
-        s = QSettings()
-        s.setValue("hyst", hyst)
+        self.updateSettings("hyst", hyst)
 
     def toggleThrottling(self, state):
         self.throttlegpu.setChecked(state)
         if self.throttlegpu.isEnabled():
             self.maxtemp.setEnabled(state)
             self.hyst.setEnabled(state)
             self.tz.setEnabled(state)
-        s = QSettings()
-        s.setValue("throttlegpu", int(state))
+        self.updateSettings("throttlegpu", int(state))
         if state == False:
             for k, v in self.thermals.items():
                 label, val, typename = v
                 stylesheet = f"QLabel {{ color: {hexColor(self.textColor)} }}"
                 label.setStyleSheet(stylesheet)
 
     def setActiveThermal(self, index):
         self.tz.setCurrentIndex(index)
-        s = QSettings()
-        s.setValue("tzindex", index)
+        self.updateSettings("tzindex", index)
 
     def updateAll(self):
         self.updateValues()
         self.updateGUI()
         if self.throttlegpu.isChecked() and self.suidhelper:
             self.throttleGPUs()
         if self.systray:
             self.updateSystray()
 
     def updateSystray(self):
         if not self.systray:
             return
         self.systray.show()
-        pix = QPixmap(22, 22)
+        pix = QPixmap(self.systraySize, self.systraySize)
         pix.fill(self.bgColor)
         p = QPainter(pix)
-        f = QFont("Dejavu Sans", 6)
+        f = QFont("Dejavu Sans", self.fontSize)
         p.setFont(f)
         p.setPen(self.fgColor)
         p.drawText(
             pix.rect(),
             Qt.AlignmentFlag.AlignTop | Qt.AlignmentFlag.AlignHCenter,
             "GPU",
         )
@@ -595,19 +606,22 @@
             p.drawText(
                 pix.rect(),
                 Qt.AlignmentFlag.AlignBottom | Qt.AlignmentFlag.AlignHCenter,
                 "CLK",
             )
         elif self.systrayCycle == 3:
             p.save()
-            gpu = min(self.gpulabels.values(), key=lambda x: x[0][0].text())
-            curclock = gpu[Cols.CUR][0].text().split()[0]
-            maxclock = gpu[Cols.MAX][0].text().split()[0]
-            if curclock == maxclock:
-                p.setPen(QColorConstants.Red)
+            if len(self.gpulabels):
+                gpu = min(self.gpulabels.values(), key=lambda x: x[0][0].text())
+                curclock = gpu[Cols.CUR][0].text().split()[0]
+                maxclock = gpu[Cols.MAX][0].text().split()[0]
+                if curclock == maxclock:
+                    p.setPen(QColorConstants.Red)
+            else:
+                curclock = '-'
             p.drawText(
                 pix.rect(),
                 Qt.AlignmentFlag.AlignBottom | Qt.AlignmentFlag.AlignHCenter,
                 "%s" % curclock,
             )
             p.restore()
         self.systrayCycle = (self.systrayCycle + 1) % 4
@@ -716,15 +730,16 @@
         if self.tz.isEnabled() and (self.tz.currentIndex() != -1):
             v = self.thermals.get(str(self.tz.currentText()), (0, 0))
             self.sumtemp += v[1]
         else:
             temp = 0
             for k, v in self.thermals.items():
                 temp += v[1]
-            temp /= float(len(self.thermals))
+            if len(self.thermals):
+                temp /= float(len(self.thermals))
             self.sumtemp += temp
         self.counter = (self.counter + 1) % self.max_count
         if self.counter == 0:
             self.avgtemp = float(self.sumtemp) / self.max_count
             # print ("Average temperature:", self.avgtemp)
             self.sumtemp = 0.0
         # brightness
```

### Comparing `intel-power-control-1.0.1/intel-power-control-helper.c` & `intel-power-control-1.0.2/intel-power-control-helper.c`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/intel-power-control-setup` & `intel-power-control-1.0.2/intel-power-control-setup`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/intel_power_control.egg-info/PKG-INFO` & `intel-power-control-1.0.2/intel_power_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-power-control
-Version: 1.0.1
+Version: 1.0.2
 Summary: GPU power management for Intel hardware on Linux
 Home-page: https://github.com/jmechnich/intel-power-control
 Author: Joerg Mechnich
 Author-email: joerg.mechnich@gmail.com
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `intel-power-control-1.0.1/intel_power_control.egg-info/SOURCES.txt` & `intel-power-control-1.0.2/intel_power_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/misc/intel-power-control.png` & `intel-power-control-1.0.2/misc/intel-power-control.png`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/misc/intel-power-control.svg` & `intel-power-control-1.0.2/misc/intel-power-control.svg`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/misc/screenshot.png` & `intel-power-control-1.0.2/misc/screenshot.png`

 * *Files identical despite different names*

### Comparing `intel-power-control-1.0.1/setup.py` & `intel-power-control-1.0.2/setup.py`

 * *Files identical despite different names*

