# Comparing `tmp/slpkg-5.0.2.tar.gz` & `tmp/slpkg-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-5.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-5.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-5.0.2.tar` & `slpkg-5.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1945 2024-03-31 17:17:22.000000 slpkg-5.0.2/README.md
--rw-r--r--   0        0        0     1716 2024-03-31 17:17:22.000000 slpkg-5.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     8384 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/binaries/install.py
--rw-r--r--   0        0        0     2306 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/binaries/required.py
--rw-r--r--   0        0        0      985 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/blacklist.py
--rw-r--r--   0        0        0     6379 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/check_updates.py
--rw-r--r--   0        0        0     1374 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/checks.py
--rw-r--r--   0        0        0     1404 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/checksum.py
--rw-r--r--   0        0        0     4061 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/choose_packages.py
--rw-r--r--   0        0        0      844 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/cleanings.py
--rw-r--r--   0        0        0     5396 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/configs.py
--rw-r--r--   0        0        0     3725 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/dependees.py
--rw-r--r--   0        0        0     1906 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/dialog_box.py
--rw-r--r--   0        0        0     4967 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     4351 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/download_only.py
--rw-r--r--   0        0        0     3852 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/downloader.py
--rw-r--r--   0        0        0      430 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/error_messages.py
--rw-r--r--   0        0        0     1538 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/find_installed.py
--rw-r--r--   0        0        0     1328 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/gpg_verify.py
--rw-r--r--   0        0        0    81827 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/install_data.py
--rw-r--r--   0        0        0     3571 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/load_data.py
--rw-r--r--   0        0        0    27101 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/main.py
--rw-r--r--   0        0        0     6126 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/multi_process.py
--rw-r--r--   0        0        0    11144 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/new_configs.py
--rw-r--r--   0        0        0     2403 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/progress_bar.py
--rw-r--r--   0        0        0     5679 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/remove_packages.py
--rw-r--r--   0        0        0     4341 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/repo_info.py
--rw-r--r--   0        0        0    34786 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/repositories.py
--rw-r--r--   0        0        0        0 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0     1075 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     4561 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    11449 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     2569 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/search.py
--rw-r--r--   0        0        0      587 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/toml_errors.py
--rw-r--r--   0        0        0     4391 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/tracking.py
--rw-r--r--   0        0        0    30454 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/update_repositories.py
--rw-r--r--   0        0        0     7893 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/upgrade.py
--rw-r--r--   0        0        0     7424 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/views/__init__.py
--rw-r--r--   0        0        0     5768 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6265 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0      740 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/views/version.py
--rw-r--r--   0        0        0     6926 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/views/view_package.py
--rw-r--r--   0        0        0     9649 2024-03-31 17:17:22.000000 slpkg-5.0.2/slpkg/views/views.py
--rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 slpkg-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1945 2024-04-01 14:26:33.000000 slpkg-5.0.3/README.md
+-rw-r--r--   0        0        0     1716 2024-04-01 14:26:33.000000 slpkg-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     8384 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     2306 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/binaries/required.py
+-rw-r--r--   0        0        0      985 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/blacklist.py
+-rw-r--r--   0        0        0     6379 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/check_updates.py
+-rw-r--r--   0        0        0     1374 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/checks.py
+-rw-r--r--   0        0        0     1404 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/checksum.py
+-rw-r--r--   0        0        0     4061 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/choose_packages.py
+-rw-r--r--   0        0        0      844 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/cleanings.py
+-rw-r--r--   0        0        0     5455 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/configs.py
+-rw-r--r--   0        0        0     3725 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/dependees.py
+-rw-r--r--   0        0        0     1906 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     4967 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     4351 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/download_only.py
+-rw-r--r--   0        0        0     3852 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/downloader.py
+-rw-r--r--   0        0        0      430 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/error_messages.py
+-rw-r--r--   0        0        0     1538 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/find_installed.py
+-rw-r--r--   0        0        0     1328 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/gpg_verify.py
+-rw-r--r--   0        0        0    81814 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/install_data.py
+-rw-r--r--   0        0        0     3662 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/load_data.py
+-rw-r--r--   0        0        0    27101 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/main.py
+-rw-r--r--   0        0        0     6126 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/multi_process.py
+-rw-r--r--   0        0        0    11270 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/new_configs.py
+-rw-r--r--   0        0        0     2403 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     5679 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     4341 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/repo_info.py
+-rw-r--r--   0        0        0    34786 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/repositories.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     4561 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    11449 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     2569 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/search.py
+-rw-r--r--   0        0        0      587 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/toml_errors.py
+-rw-r--r--   0        0        0     4391 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/tracking.py
+-rw-r--r--   0        0        0    30454 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/update_repositories.py
+-rw-r--r--   0        0        0     8587 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/upgrade.py
+-rw-r--r--   0        0        0     7486 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     5768 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6265 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0      740 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/version.py
+-rw-r--r--   0        0        0     6926 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/view_package.py
+-rw-r--r--   0        0        0     9945 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/views.py
+-rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 slpkg-5.0.3/PKG-INFO
```

### Comparing `slpkg-5.0.2/README.md` & `slpkg-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/pyproject.toml` & `slpkg-5.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "slpkg"
-version = "5.0.2"
+version = "5.0.3"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
```

### Comparing `slpkg-5.0.2/slpkg/binaries/install.py` & `slpkg-5.0.3/slpkg/binaries/install.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/binaries/required.py` & `slpkg-5.0.3/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/blacklist.py` & `slpkg-5.0.3/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/check_updates.py` & `slpkg-5.0.3/slpkg/check_updates.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/checks.py` & `slpkg-5.0.3/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/checksum.py` & `slpkg-5.0.3/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/choose_packages.py` & `slpkg-5.0.3/slpkg/choose_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/cleanings.py` & `slpkg-5.0.3/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/configs.py` & `slpkg-5.0.3/slpkg/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     etc_path: Path = Path('/etc', prog_name)
     lib_path: Path = Path('/var/lib', prog_name)
     log_path: Path = Path('/var/log/', prog_name)
     log_packages: Path = Path('/var', 'log', 'packages')
 
     deps_log_file: Path = Path(log_path, 'deps.log')
     slpkg_log_file: Path = Path(log_path, 'slpkg.log')
+    upgrade_log_file: Path = Path(log_path, 'upgrade.log')
 
     file_list_suffix: str = '.pkgs'
     installpkg: str = 'upgradepkg --install-new'
     reinstall: str = 'upgradepkg --reinstall'
     removepkg: str = 'removepkg'
     colors: bool = True
     makeflags: str = '-j4'
```

### Comparing `slpkg-5.0.2/slpkg/dependees.py` & `slpkg-5.0.3/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/dialog_box.py` & `slpkg-5.0.3/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/dialog_configs.py` & `slpkg-5.0.3/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/download_only.py` & `slpkg-5.0.3/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/downloader.py` & `slpkg-5.0.3/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/find_installed.py` & `slpkg-5.0.3/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/gpg_verify.py` & `slpkg-5.0.3/slpkg/gpg_verify.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/install_data.py` & `slpkg-5.0.3/slpkg/install_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         for line in lines:
             if line.startswith(days):
                 last_date: str = line.replace('\n', '')
                 break
 
         last_update_json[repo]: dict = last_date
         if self.repos.last_update_json.is_file():
-            last_update_json: dict = json.loads(self.repos.last_update_json.read_text(encoding='utf-8'))
+            last_update_json: dict = self.utils.read_json_file(self.repos.last_update_json)
             last_update_json[repo] = last_date
 
         self.repos.last_update_json.write_text(json.dumps(last_update_json, indent=4))
 
     def view_done_message(self) -> None:
         print(f'{self.bgreen}{self.ascii.done}{self.endc}\n')
```

### Comparing `slpkg-5.0.2/slpkg/load_data.py` & `slpkg-5.0.3/slpkg/load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,25 @@
         """
         Read JSON data from the file.
         Args:
             file: Path file for reading.
         Returns:
             Dictionary with data.
         """
+        json_data: dict = {}
         try:
             json_data: dict = json.loads(file.read_text(encoding='utf-8'))
         except FileNotFoundError:
             print(f'{self.bred}{self.ascii.failed}{self.endc}')
             print(f'\nFile {file} not found!')
             print('\nNeed to update the database first, please run:\n')
             print(f"{'':>2} $ {self.green}slpkg update{self.endc}\n")
             raise SystemExit(1)
+        except json.decoder.JSONDecodeError:
+            pass
         return json_data
 
     def _remove_blacklist_from_all_repos(self, data: dict) -> dict:
         # Remove blacklist packages from keys.
         for name, repo in data.items():
             blacklist_packages: list = self.utils.ignore_packages(list(data[name].keys()))
             for pkg in blacklist_packages:
```

### Comparing `slpkg-5.0.2/slpkg/main.py` & `slpkg-5.0.3/slpkg/main.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/multi_process.py` & `slpkg-5.0.3/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/new_configs.py` & `slpkg-5.0.3/slpkg/new_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,18 +41,18 @@
             self.bgreen: str = ''
             self.yellow: str = ''
             self.byellow: str = ''
             self.endc: str = ''
 
     def check(self) -> None:
         """ Checks for .new files. """
-        print('\nChecking for NEW configuration files...')
+        print('Checking for NEW configuration files...\n')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
                 or self.repositories_config_new.is_file()):
-            print('\nThere are NEW files:\n')
+            print('There are NEW files:\n')
 
             if self.slpkg_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.slpkg_config_new}{self.endc}")
 
             if self.repositories_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.repositories_config_new}{self.endc}")
 
@@ -189,14 +189,15 @@
             print()  # new line
         if make.lower() == 'r':
             print()  # new line
             self.remove_config_new_file()
             print()  # new line
         if make.lower() == 'd':
             self.diff_files(self.slpkg_config_new, self.slpkg_config)
+            self.prompt_slpkg_config()
         if make.lower() == 'v':
             self.vimdiff(self.slpkg_config_new, self.slpkg_config)
 
     def prompt_repositories_config(self) -> None:
         make: str = input(f'{self.bgreen}{self.repositories_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
@@ -209,14 +210,15 @@
             print()  # new line
         if make.lower() == 'r':
             print()  # new line
             self.remove_repositories_new_file()
             print()  # new line
         if make.lower() == 'd':
             self.diff_files(self.repositories_config_new, self.repositories_config)
+            self.prompt_repositories_config()
         if make.lower() == 'v':
             self.vimdiff(self.repositories_config_new, self.repositories_config)
 
     def prompt_blacklist_config(self) -> None:
         make: str = input(f'{self.bgreen}{self.blacklist_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
@@ -229,14 +231,15 @@
             print()  # new line
         if make.lower() == 'r':
             print()  # new line
             self.remove_blacklist_new_file()
             print()  # new line
         if make.lower() == 'd':
             self.diff_files(self.blacklist_config_new, self.blacklist_config)
+            self.prompt_blacklist_config()
         if make.lower() == 'v':
             self.vimdiff(self.blacklist_config_new, self.blacklist_config)
 
     @staticmethod
     def diff_files(file2: Any, file1: Any) -> None:
         """ Diff the .new and the current file. """
         with open(file1, 'r') as f1:
```

### Comparing `slpkg-5.0.2/slpkg/progress_bar.py` & `slpkg-5.0.3/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/remove_packages.py` & `slpkg-5.0.3/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/repo_info.py` & `slpkg-5.0.3/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/repositories.py` & `slpkg-5.0.3/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/sbos/dependencies.py` & `slpkg-5.0.3/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/sbos/sbo_generate.py` & `slpkg-5.0.3/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/sbos/slackbuild.py` & `slpkg-5.0.3/slpkg/sbos/slackbuild.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/search.py` & `slpkg-5.0.3/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/toml_errors.py` & `slpkg-5.0.3/slpkg/toml_errors.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/tracking.py` & `slpkg-5.0.3/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/update_repositories.py` & `slpkg-5.0.3/slpkg/update_repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/upgrade.py` & `slpkg-5.0.3/slpkg/upgrade.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,32 @@
         self.sum_upgrade: int = 0
         self.sum_removed: int = 0
         self.sum_added: int = 0
         self.installed_names: list = []
         self.installed_packages: list = []
 
     def load_installed_packages(self, repository: str) -> None:
-        if repository == self.repos.slack_repo_name:
+        if repository in [self.repos.slack_repo_name, self.repos.salixos_repo_name]:
             installed: dict = self.utils.all_installed()
 
             for name, package in installed.items():
                 tag: str = self.utils.split_package(package)['tag']
                 if not tag:
                     self.installed_packages.append(Path(package))
                     self.installed_names.append(name)
         else:
             repo_tag: str = self.repos.repositories[repository]['repo_tag']
             self.installed_packages: list = list(self.log_packages.glob(f'*{repo_tag}'))
 
     def packages(self) -> Generator:
         """ Returns the upgradable packages. """
+        # Delete log file before starts.
+        if self.upgrade_log_file.is_file():
+            self.upgrade_log_file.unlink()
+
         self.load_installed_packages(self.repository)
 
         for inst in self.installed_packages:
             name: str = self.utils.split_package(inst.name)['name']
             if self.is_package_upgradeable(inst.name):
                 yield name
 
@@ -56,30 +60,40 @@
         if self.repository == self.repos.slack_repo_name and self.new_packages:
             for name in self.data.keys():
                 # if not self.utils.is_package_installed(name):
                 if name not in self.installed_names:
                     yield name
 
     def is_package_upgradeable(self, installed: str) -> bool:
+        """ Returns True for upgradeable packages. """
         inst_name: str = self.utils.split_package(installed)['name']
         if self.data.get(inst_name):
             repo_version: str = self.data[inst_name]['version']
             repo_build: str = self.data[inst_name]['build']
             inst_version: str = self.utils.split_package(installed)['version']
             inst_build: str = self.utils.split_package(installed)['build']
             try:
                 if parse(repo_version) > parse(inst_version):
                     return True
 
                 if parse(repo_version) == parse(inst_version) and int(repo_build) > int(inst_build):
                     return True
-            except InvalidVersion:
+            except InvalidVersion as err:
+                self._write_log_file(installed, inst_name, err)
                 return False
         return False
 
+    def _write_log_file(self, installed: str, name: str, err: InvalidVersion) -> None:
+        """ Writes a log file for invalid versions. """
+        if self.log_path.is_dir():
+            with self.upgrade_log_file.open('a') as log:
+                log.write(f"Installed: {installed}, "
+                          f"Repository: {self.data[name]['package']}, "
+                          f"Error: {err}\n")
+
     def check_packages(self) -> None:
         repo_data: dict = {}
         found_packages: dict = {}
 
         if self.repository == '*':
             repo_data: dict = self.data
         else:
```

### Comparing `slpkg-5.0.2/slpkg/utilities.py` & `slpkg-5.0.3/slpkg/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,16 @@
             Dictionary with data.
         """
         json_data: dict = {}
         try:
             json_data: dict = json.loads(file.read_text(encoding='utf-8'))
         except FileNotFoundError:
             self.errors.raise_error_message(f'{file} not found.', exit_status=1)
+        except json.decoder.JSONDecodeError:
+            pass
         return json_data
 
     def ignore_packages(self, packages: list) -> list:
         """
         Matching packages using regular expression.
         Args:
             packages: Tha packages to apply the pattern.
```

### Comparing `slpkg-5.0.2/slpkg/views/asciibox.py` & `slpkg-5.0.3/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/views/cli_menu.py` & `slpkg-5.0.3/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/views/version.py` & `slpkg-5.0.3/slpkg/views/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (5, 0, 2)
+        self.version_info: tuple = (5, 0, 3)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'GNU General Public License v3 (GPLv3)'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
         self.email: str = 'dslackw@gmail.com'
 
     def view(self) -> None:
```

### Comparing `slpkg-5.0.2/slpkg/views/view_package.py` & `slpkg-5.0.3/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.2/slpkg/views/views.py` & `slpkg-5.0.3/slpkg/views/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+import shutil
 from typing import Any
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
@@ -28,14 +29,15 @@
 
         self.sum_install = 0
         self.sum_upgrade = 0
         self.sum_remove = 0
         self.sum_size_comp = 0
         self.sum_size_uncomp = 0
         self.sum_size_remove = 0
+        self.columns, self.rows = shutil.get_terminal_size()
 
         self.download_only = None
         self.summary_message: str = ''
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
@@ -197,19 +199,22 @@
 
     def set_summary_for_build(self, packages: list) -> None:
         self.summary_message: str = (
             f'{self.grey}Total {len(packages)} packages '
             f'will be build in {self.tmp_path} folder.{self.endc}')
 
     def set_summary_for_install_and_upgrade(self, install: int, upgrade: int, size_comp: int, size_uncomp: int) -> None:
-        self.summary_message: str = (
-            f'{self.grey}Total {install} packages will be '
-            f'installed and {upgrade} will be upgraded, and total '
-            f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
-            f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc}')
+        split_message: str = '\n'
+        if self.columns > 80:
+            split_message: str = ''
+        total_packages: str = (f'{self.grey}Total {install} packages will be installed and {upgrade} '
+                               f'will be upgraded, while a total ')
+        total_sizes: str = (f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
+                            f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc}')
+        self.summary_message: str = f'{total_packages}{split_message}{total_sizes}'
 
     def set_summary_for_remove(self, remove: int, size_rmv: int) -> None:
         self.summary_message: str = (
             f'{self.grey}Total {remove} packages '
             f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
             f'of space will be freed up.{self.endc}')
```

### Comparing `slpkg-5.0.2/PKG-INFO` & `slpkg-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 5.0.2
+Version: 5.0.3
 Summary: Package manager utility for Slackware Linux
 Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slpkg Version: 5.0.2 Summary: Package manager
+Metadata-Version: 2.1 Name: slpkg Version: 5.0.3 Summary: Package manager
 utility for Slackware Linux Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis
 gmail.com> Maintainer-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Environment :: Console
 Classifier: Operating System :: POSIX Classifier: Operating System :: POSIX ::
```

