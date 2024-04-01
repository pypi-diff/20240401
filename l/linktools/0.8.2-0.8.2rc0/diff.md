# Comparing `tmp/linktools-0.8.2.tar.gz` & `tmp/linktools-0.8.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.2.tar", last modified: Mon Apr  1 14:45:26 2024, max compression
+gzip compressed data, was "linktools-0.8.2rc0.tar", last modified: Sat Mar 30 15:13:58 2024, max compression
```

## Comparing `linktools-0.8.2.tar` & `linktools-0.8.2rc0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.045974 linktools-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-01 14:42:53.000000 linktools-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 14:42:53.000000 linktools-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-01 14:45:26.041974 linktools-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32666 2024-04-01 14:42:53.000000 linktools-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-01 14:42:53.000000 linktools-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:45:26.045974 linktools-0.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4274 2024-04-01 14:42:53.000000 linktools-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.017975 linktools-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.021975 linktools-0.8.2/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21585 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    18049 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.025975 linktools-0.8.2/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/android/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.025975 linktools-0.8.2/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-01 14:45:14.000000 linktools-0.8.2/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 14:45:14.000000 linktools-0.8.2/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.017975 linktools-0.8.2/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.025975 linktools-0.8.2/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.029975 linktools-0.8.2/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.029975 linktools-0.8.2/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-01 14:43:04.000000 linktools-0.8.2/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-01 14:43:04.000000 linktools-0.8.2/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.017975 linktools-0.8.2/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.029975 linktools-0.8.2/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-04-01 14:45:25.000000 linktools-0.8.2/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.029975 linktools-0.8.2/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    29658 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.029975 linktools-0.8.2/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.029975 linktools-0.8.2/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.033975 linktools-0.8.2/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/common/cntr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/common/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/common/shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.033975 linktools-0.8.2/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.033975 linktools-0.8.2/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ios/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-01 14:45:25.000000 linktools-0.8.2/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/utils/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17177 2024-04-01 14:42:53.000000 linktools-0.8.2/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:45:26.037974 linktools-0.8.2/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-01 14:45:26.000000 linktools-0.8.2/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-01 14:45:26.000000 linktools-0.8.2/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:45:26.000000 linktools-0.8.2/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-01 14:45:26.000000 linktools-0.8.2/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 14:45:26.000000 linktools-0.8.2/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 14:45:26.000000 linktools-0.8.2/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.952578 linktools-0.8.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-03-30 15:13:58.952578 linktools-0.8.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32666 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 15:13:58.952578 linktools-0.8.2rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4274 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.928578 linktools-0.8.2rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.932578 linktools-0.8.2rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21195 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-03-30 15:13:53.000000 linktools-0.8.2rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-30 15:13:53.000000 linktools-0.8.2rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.928578 linktools-0.8.2rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.936578 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-03-30 15:12:01.000000 linktools-0.8.2rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-03-30 15:12:01.000000 linktools-0.8.2rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.928578 linktools-0.8.2rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2637 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.940578 linktools-0.8.2rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/cntr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.944578 linktools-0.8.2rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17177 2024-03-30 15:11:54.000000 linktools-0.8.2rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:13:58.948578 linktools-0.8.2rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 15:13:58.000000 linktools-0.8.2rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.2/LICENSE` & `linktools-0.8.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/PKG-INFO` & `linktools-0.8.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.2
+Version: 0.8.2rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.2/README.md` & `linktools-0.8.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/pyproject.toml` & `linktools-0.8.2rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/setup.py` & `linktools-0.8.2rc0/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/__init__.py` & `linktools-0.8.2rc0/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/__main__.py` & `linktools-0.8.2rc0/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/_config.py` & `linktools-0.8.2rc0/src/linktools/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,30 +265,26 @@
         :param prefix: 环境变量前缀
         :param share: 是否共享配置
         """
         self._environ = environ
         self._config = config if share else pickle.loads(pickle.dumps(config))
         self._namespace = namespace if namespace != __missing__ else "MAIN"
         self._prefix = prefix.upper() if prefix != __missing__ else ""
-        self._reload = None
         self._cache = dict()
+        self._reload = None
         self._cache_path = self._environ.get_data_path(f"{self._environ.name}.cfg", create_parent=True)
         self.load_cache()
 
     @property
     def reload(self) -> bool:
         """
         是否重新加载配置
         """
         if self._reload is None:
-            value = False
-            key = f"{self._prefix}RELOAD_CONFIG"
-            if key in os.environ:
-                value = self.cast(os.environ[key], type=bool)
-            self._reload = value
+            self._reload = self.get("RELOAD_CONFIG", type=bool, default=False)
         return self._reload
 
     @reload.setter
     def reload(self, value: bool):
         """
         是否重新加载配置
         """
@@ -318,32 +314,29 @@
             if env_key in os.environ:
                 value = os.environ.get(env_key)
                 return self.cast(value, type=type)
 
             if key in self._cache:
                 value = self._cache.get(key)
                 prop = self._config.get(key, None)
-                if self.reload:
-                    if isinstance(prop, ConfigProperty) and prop.reloadable:
-                        with self.__lock__:
-                            value = self._cache[key] = prop.load(self, key, type=type, cache=value)
-                            return value
-                    if isinstance(default, ConfigProperty) and default.reloadable:
-                        with self.__lock__:
-                            value = self._cache[key] = default.load(self, key, type=type, cache=value)
-                            return value
-                return self.cast(value, type=type)
+                if isinstance(prop, ConfigProperty) and prop.reloadable and self.reload:
+                    with self.__lock__:
+                        value = self._cache[key] = prop.load(self, key, type=type, cache=value)
+                else:
+                    value = self.cast(value, type=type)
+                return value
 
             if key in self._config:
                 value = self._config.get(key)
                 if isinstance(value, ConfigProperty):
                     with self.__lock__:
                         value = self._cache[key] = value.load(self, key, type=type)
-                        return value
-                return self.cast(value, type=type)
+                else:
+                    value = self.cast(value, type=type)
+                return value
 
         except Exception as e:
             last_error = e
 
         if default == __missing__:
             if last_error != __missing__:
                 raise last_error
```

### Comparing `linktools-0.8.2/src/linktools/_environ.py` & `linktools-0.8.2rc0/src/linktools/_environ.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/_tools.py` & `linktools-0.8.2rc0/src/linktools/_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,25 +358,25 @@
         if not utils.is_empty(self.unpack_path):
             self._container.logger.debug(f"Delete {self.root_path}")
             shutil.rmtree(self.root_path, ignore_errors=True)
         elif self.absolute_path.startswith(self.root_path):
             self._container.logger.debug(f"Delete {self.absolute_path}")
             os.remove(self.absolute_path)
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Process:
+    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
         self.prepare()
 
         # java or other
         executable_cmdline = self.executable_cmdline
         if executable_cmdline[0] in self._container.items:
             args = [*executable_cmdline[1:], *args]
             tool = self._container.items[executable_cmdline[0]]
             return tool.popen(*args, **kwargs)
 
-        return utils.Process(*[*executable_cmdline, *args], **kwargs)
+        return utils.Popen(*[*executable_cmdline, *args], **kwargs)
 
     @utils.timeoutable
     def exec(
             self,
             *args: [Any],
             timeout: utils.Timeout = None,
             ignore_errors: bool = False,
```

### Comparing `linktools-0.8.2/src/linktools/_url.py` & `linktools-0.8.2rc0/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/android/__init__.py` & `linktools-0.8.2rc0/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/android/adb.py` & `linktools-0.8.2rc0/src/linktools/android/adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     def uid(self) -> int:
         """
         获取shell的uid
         :return: uid
         """
         return self.get_uid()
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Process:
+    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
         """
         执行命令
         :param args: 命令行参数
         :return: 打开的进程
         """
         args = ["-s", self.id, *args]
         return self._adb.popen(*args, **kwargs)
```

### Comparing `linktools-0.8.2/src/linktools/android/struct.py` & `linktools-0.8.2rc0/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/android-tools.apk` & `linktools-0.8.2rc0/src/linktools/assets/android-tools.apk`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/android-tools.json` & `linktools-0.8.2rc0/src/linktools/assets/android-tools.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'time': '2024-03-30 23:13:53'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
         "md5": "6a8c9cfb8555846bee1b972b63331027",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-04-01 22:45:14"
+        "time": "2024-03-30 23:13:53"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.2/src/linktools/assets/chrome-driver.json` & `linktools-0.8.2rc0/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.2rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.2rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.2rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/fake_useragent.json` & `linktools-0.8.2rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/frida.js` & `linktools-0.8.2rc0/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/frida.min.js` & `linktools-0.8.2rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.2rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/assets/tools.json` & `linktools-0.8.2rc0/src/linktools/assets/tools.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/__init__.py` & `linktools-0.8.2rc0/src/linktools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/argparse.py` & `linktools-0.8.2rc0/src/linktools/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/command.py` & `linktools-0.8.2rc0/src/linktools/cli/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,65 @@
     pass
 
 
 class SubCommandError(CommandError):
     pass
 
 
+class LogCommandMixin:
+
+    def add_log_options(self: "BaseCommand", parser: ArgumentParser = None):
+
+        environ = self.environ
+        parser = parser or self._argument_parser
+
+        class VerboseAction(Action):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                logging.root.setLevel(logging.DEBUG)
+
+        class DebugAction(Action):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                environ.debug = True
+                environ.logger.setLevel(logging.DEBUG)
+
+        class LogTimeAction(BooleanOptionalAction):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                if option_string in self.option_strings:
+                    value = not option_string.startswith("--no-")
+                    handler = LogHandler.get_instance()
+                    if handler:
+                        handler.show_time = value
+                    environ.set_config("SHOW_LOG_TIME", value)
+
+        class LogLevelAction(BooleanOptionalAction):
+
+            def __call__(self, parser, namespace, values, option_string=None):
+                if option_string in self.option_strings:
+                    value = not option_string.startswith("--no-")
+                    handler = LogHandler.get_instance()
+                    if handler:
+                        handler.show_level = value
+                    environ.set_config("SHOW_LOG_LEVEL", value)
+
+        group = parser.add_argument_group(title="log options")
+        group.add_argument("--verbose", action=VerboseAction, nargs=0, const=True, dest=SUPPRESS,
+                           help="increase log verbosity")
+        group.add_argument("--debug", action=DebugAction, nargs=0, const=True, dest=SUPPRESS,
+                           help=f"increase {self.environ.name}'s log verbosity, and enable debug mode")
+
+        if LogHandler.get_instance():
+            group.add_argument("--time", action=LogTimeAction, dest=SUPPRESS,
+                               help="show log time")
+            group.add_argument("--level", action=LogLevelAction, dest=SUPPRESS,
+                               help="show log level")
+
+
 def _filter_kwargs(kwargs):
     return {k: v for k, v in kwargs.items() if v != __missing__}
 
 
 _subcommand_index: int = 0
 _subcommand_map: Dict[str, Set[str]] = {}
 
@@ -492,15 +543,14 @@
             if subcommand.has_parent:
                 parent_subparsers = subparsers_map.get(subcommand.parent_id, None)
                 if not parent_subparsers:
                     raise SubCommandError(f"Subcommand {subcommand} has no parent subparser")
 
             parser = subcommand.create_parser(type=parent_subparsers.add_parser)
             parser.set_defaults(**{f"__subcommand_{id(self):x}__": subcommand})
-            self.init_common_arguments(parser)
 
             if subcommand.is_group:
                 _subparsers = parser.add_subparsers(metavar="COMMAND", help="Command Help")
                 _subparsers.required = False
                 subparsers_map[subcommand.id] = _subparsers
 
             # BaseCommand 类型单独处理，因为有可能在init_arguments中添加了子命令
@@ -606,15 +656,15 @@
             if info.children:
                 current_max_level = max_level - current_node_level if max_level is not None else None
                 self._make_subcommand_tree(current_node, info.children, SubCommand.ROOT_ID, current_max_level)
 
         return tree
 
 
-class BaseCommand(SubCommandMixin, metaclass=abc.ABCMeta):
+class BaseCommand(LogCommandMixin, SubCommandMixin, metaclass=abc.ABCMeta):
 
     @property
     def name(self):
         """
         命令名
         """
         name = self.__module__
@@ -647,28 +697,14 @@
     @property
     def known_errors(self) -> List[Type[BaseException]]:
         """
         已知错误类型
         """
         return [CommandError]
 
-    @abc.abstractmethod
-    def init_arguments(self, parser: ArgumentParser) -> None:
-        """
-        初始化参数，在调用create_parser时执行
-        """
-        pass
-
-    @abc.abstractmethod
-    def run(self, args: Namespace) -> Optional[int]:
-        """
-        业务逻辑入口
-        """
-        pass
-
     def create_parser(
             self,
             *args: Any,
             type: Callable[..., ArgumentParser] = ArgumentParser,
             formatter_class: Type[HelpFormatter] = RawDescriptionHelpFormatter,
             conflict_handler="resolve",
             **kwargs: Any
@@ -691,78 +727,35 @@
         )
         self.init_base_arguments(parser)
         self.init_arguments(parser)
         return parser
 
     @cached_property
     def _argument_parser(self) -> ArgumentParser:
-        parser = self.create_parser()
-        self.init_common_arguments(parser)
-        return parser
+        return self.create_parser()
 
     def init_base_arguments(self, parser: ArgumentParser) -> None:
         """
         初始化基础参数，在调用create_parser时执行
         """
         pass
 
-    def init_common_arguments(self, parser: ArgumentParser) -> None:
+    @abc.abstractmethod
+    def init_arguments(self, parser: ArgumentParser) -> None:
         """
-        初始化公共参数，会在命令本身和所有子命令中调用
+        初始化参数，在调用create_parser时执行
         """
-        environ = self.environ
-        prefix = parser.prefix_chars
-
-        class VerboseAction(Action):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                logging.root.setLevel(logging.DEBUG)
-
-        class DebugAction(Action):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                environ.debug = True
-                environ.logger.setLevel(logging.DEBUG)
-
-        class LogTimeAction(BooleanOptionalAction):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                if option_string in self.option_strings:
-                    value = not option_string.startswith("--no-")
-                    handler = LogHandler.get_instance()
-                    if handler:
-                        handler.show_time = value
-                    environ.set_config("SHOW_LOG_TIME", value)
-
-        class LogLevelAction(BooleanOptionalAction):
-
-            def __call__(self, parser, namespace, values, option_string=None):
-                if option_string in self.option_strings:
-                    value = not option_string.startswith("--no-")
-                    handler = LogHandler.get_instance()
-                    if handler:
-                        handler.show_level = value
-                    environ.set_config("SHOW_LOG_LEVEL", value)
-
-        group = parser.add_argument_group(title="log options")
-        group.add_argument(f"{prefix}{prefix}verbose", action=VerboseAction, nargs=0, const=True, dest=SUPPRESS,
-                           help="increase log verbosity")
-        group.add_argument(f"{prefix}{prefix}debug", action=DebugAction, nargs=0, const=True, dest=SUPPRESS,
-                           help=f"increase {self.environ.name}'s log verbosity, and enable debug mode")
-
-        if LogHandler.get_instance():
-            group.add_argument(f"{prefix}{prefix}time", action=LogTimeAction, dest=SUPPRESS,
-                               help="show log time")
-            group.add_argument(f"{prefix}{prefix}level", action=LogLevelAction, dest=SUPPRESS,
-                               help="show log level")
+        pass
 
-        if self.environ.version != NotImplemented:
-            parser.add_argument(
-                f"{prefix}{prefix}version", action="version", version=self.environ.version
-            )
+    @abc.abstractmethod
+    def run(self, args: Namespace) -> Optional[int]:
+        """
+        业务逻辑入口
+        """
+        pass
 
     def main(self, *args, **kwargs) -> None:
         """
         main命令入口
         """
         if is_terminal():
             logging.basicConfig(
@@ -774,35 +767,42 @@
         else:
             logging.basicConfig(
                 level=logging.INFO,
                 format="[%(asctime)s] %(levelname)s %(module)s %(funcName)s %(message)s",
                 datefmt="%H:%M:%S"
             )
 
+        self.add_log_options()
+
+        if self.environ.version != NotImplemented:
+            self._argument_parser.add_argument(
+                "--version", action="version", version=self.environ.version
+            )
+
         try:
-            result = self(*args, **kwargs)
+            exit_code = self(*args, **kwargs)
         except SystemExit as e:
-            result = e.code
+            exit_code = e.code
 
         except (KeyboardInterrupt, EOFError) as e:
-            result = 1
+            exit_code = 1
             error_type, error_message = e.__class__.__name__, str(e).strip()
             self.logger.error(
                 f"{error_type}: {error_message}" if error_message else error_type,
             )
 
         except:
-            result = 1
+            exit_code = 1
             if environ.debug:
                 console = get_console()
                 console.print_exception(show_locals=True)
             else:
                 self.logger.error(traceback.format_exc())
 
-        exit(result)
+        exit(exit_code)
 
     def __call__(self, args: Union[List[str], Namespace] = None) -> int:
         """
         内部调用命令入口
         """
         try:
             if not isinstance(args, Namespace):
```

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/app.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         device.shell("am", "force-stop", args.package, log_output=True)
         device.shell("am", "start", "-D", "-n", "{}/{}".format(args.package, args.activity), log_output=True)
 
         pid = utils.int(device.shell("top", "-n", "1", "|", "grep", args.package).split()[0])
         with device.forward(f"tcp:{args.port}", f"jdwp:{pid}"):
             data = input("jdb connect? [Y/n]: ").strip()
             if data in ["", "Y", "y"]:
-                process = utils.Process(
-                    "jdb", "-connect", f"com.sun.jdi.SocketAttach:hostname=127.0.0.1,port={args.port}")
+                process = utils.Popen("jdb", "-connect",
+                                      "com.sun.jdi.SocketAttach:hostname=127.0.0.1,port={}".format(args.port))
                 return process.call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/info.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/intent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/objection.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             if args.redirect_address or args.redirect_port:
                 # 如果需要重定向到本地端口
                 address = args.redirect_address
                 port = args.redirect_port or 8080
                 info = device.get_package(package)
                 uid = info.user_id if info else None
                 with device.redirect(address, port, uid):
-                    return utils.Process(*objection_args).call()
+                    return utils.Popen(*objection_args).call()
             else:
-                return utils.Process(*objection_args).call()
+                return utils.Popen(*objection_args).call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/android/top.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/android/top.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/common/cntr.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         self.logger.info(f"Remove {', '.join(keys)} success")
 
     @subcommand("list", help="list container configs")
     def on_command_list(self):
         keys = set()
         for container in manager.prepare_installed_containers():
             keys.update(container.configs.keys())
-            if hasattr(container, "keys") and isinstance(container.keys, (Tuple, List, Dict)):
+            if hasattr(container, "keys") and isinstance(container.keys, (Tuple, List)):
                 keys.update([key for key in container.keys if key in manager.config])
         for key in sorted(keys):
             value = manager.config.get(key)
             self.logger.info(f"{key}: {value}")
 
     @subcommand("reload", help="reload container configs")
     def on_command_reload(self):
```

### Comparing `linktools-0.8.2/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/common/shell.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/common/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,20 +37,20 @@
                 self._shell_path = os.environ["ComSpec"]
 
     def init_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-c", "--command", action="store", default=None, help="shell command")
 
     def run(self, args: Namespace) -> Optional[int]:
         if args.command:
-            process = utils.Process(args.command, shell=True)
+            process = utils.Popen(args.command, shell=True)
             return process.call()
 
         if not self._shell_path or not os.path.exists(self._shell_path):
             raise NotImplementedError(f"unsupported system {environ.system}")
 
-        process = utils.Process(self._shell_path)
+        process = utils.Popen(self._shell_path)
         return process.call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/common/tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
             if args.file_commands:
                 objection_args += ["--file-commands", args.file_commands]
             if args.startup_script:
                 objection_args += ["--startup-script", args.startup_script]
             if args.plugin_folder:
                 objection_args += ["--plugin-folder", args.plugin_folder]
 
-            return utils.Process(*objection_args).call()
+            return utils.Popen(*objection_args).call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.2/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.2rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/cli/device.py` & `linktools-0.8.2rc0/src/linktools/cli/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -120,16 +120,14 @@
 
 
 class DeviceCommandMixin:
 
     def add_device_options(self: "BaseCommand", parser: ArgumentParser):
 
         parser = parser or self._argument_parser
-        prefix = parser.prefix_chars
-
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "mobile",
                 create_parent=True
             )
         )
 
@@ -188,27 +186,25 @@
                 device_parser = DevicePicker.copy_on_write(namespace, self.dest)
                 device_parser.func = pick
 
         option_group = parser.add_argument_group(title="mobile device options")
         option_group.set_defaults(device_picker=DevicePicker(pick))
 
         device_group = option_group.add_mutually_exclusive_group()
-        device_group.add_argument(f"{prefix}i", f"{prefix}{prefix}id", metavar="ID", dest="device_picker",
-                                  action=IDAction, help="specify unique device identifier")
-        device_group.add_argument(f"{prefix}l", f"{prefix}{prefix}last", dest="device_picker", nargs=0, const=True,
-                                  action=LastAction, help="use last device")
+        device_group.add_argument("-i", "--id", metavar="ID", dest="device_picker", action=IDAction,
+                                  help="specify unique device identifier")
+        device_group.add_argument("-l", "--last", dest="device_picker", nargs=0, const=True, action=LastAction,
+                                  help="use last device")
 
 
 class AndroidCommandMixin:
 
     def add_android_options(self: BaseCommand, parser: ArgumentParser) -> None:
 
         parser = parser or self._argument_parser
-        prefix = parser.prefix_chars
-
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "android",
                 create_parent=True
             )
         )
 
@@ -306,46 +302,44 @@
                     device_parser.options.extend(values)
                 else:
                     device_parser.options.append(str(values))
 
         option_group = parser.add_argument_group(title="adb options")
         option_group.set_defaults(device_picker=AndroidPicker(pick))
 
-        option_group.add_argument(f"{prefix}a", f"{prefix}{prefix}all-interfaces", dest="device_picker", nargs=0, action=OptionAction,
+        option_group.add_argument("-a", "--all-interfaces", dest="device_picker", nargs=0, action=OptionAction,
                                   help="listen on all network interfaces, not just localhost (adb -a option)")
 
         device_group = option_group.add_mutually_exclusive_group()
-        device_group.add_argument(f"{prefix}d", f"{prefix}{prefix}device", dest="device_picker", nargs=0, action=DeviceAction,
+        device_group.add_argument("-d", "--device", dest="device_picker", nargs=0, action=DeviceAction,
                                   help="use USB device (adb -d option)")
-        device_group.add_argument(f"{prefix}s", f"{prefix}{prefix}serial", metavar="SERIAL", dest="device_picker", action=SerialAction,
+        device_group.add_argument("-s", "--serial", metavar="SERIAL", dest="device_picker", action=SerialAction,
                                   help="use device with given serial (adb -s option)")
-        device_group.add_argument(f"{prefix}e", f"{prefix}{prefix}emulator", dest="device_picker", nargs=0, action=EmulatorAction,
+        device_group.add_argument("-e", "--emulator", dest="device_picker", nargs=0, action=EmulatorAction,
                                   help="use TCP/IP device (adb -e option)")
-        device_group.add_argument(f"{prefix}c", f"{prefix}{prefix}connect", metavar="IP[:PORT]", dest="device_picker", action=ConnectAction,
+        device_group.add_argument("-c", "--connect", metavar="IP[:PORT]", dest="device_picker", action=ConnectAction,
                                   help="use device with TCP/IP")
-        device_group.add_argument(f"{prefix}l", f"{prefix}{prefix}last", dest="device_picker", nargs=0, action=LastAction,
+        device_group.add_argument("-l", "--last", dest="device_picker", nargs=0, action=LastAction,
                                   help="use last device")
 
-        option_group.add_argument(f"{prefix}t", f"{prefix}{prefix}transport", metavar="ID", dest="device_picker", action=OptionAction,
+        option_group.add_argument("-t", "--transport", metavar="ID", dest="device_picker", action=OptionAction,
                                   help="use device with given transport ID (adb -t option)")
-        option_group.add_argument(f"{prefix}H", metavar="HOST", dest="device_picker", action=OptionAction,
+        option_group.add_argument("-H", metavar="HOST", dest="device_picker", action=OptionAction,
                                   help="name of adb server host [default=localhost] (adb -H option)")
-        option_group.add_argument(f"{prefix}P", metavar="PORT", dest="device_picker", action=OptionAction,
+        option_group.add_argument("-P", metavar="PORT", dest="device_picker", action=OptionAction,
                                   help="port of adb server [default=5037] (adb -P option)")
-        option_group.add_argument(f"{prefix}L", metavar="SOCKET", dest="device_picker", action=OptionAction,
+        option_group.add_argument("-L", metavar="SOCKET", dest="device_picker", action=OptionAction,
                                   help="listen on given socket for adb server [default=tcp:localhost:5037] (adb -L option)")
 
 
 class IOSCommandMixin:
 
     def add_ios_options(self: BaseCommand, parser: ArgumentParser):
 
         parser = parser or self._argument_parser
-        prefix = parser.prefix_chars
-
         cache = DeviceCache(
             self.environ.get_temp_path(
                 "cache", "device", "ios",
                 create_parent=True
             )
         )
 
@@ -412,19 +406,19 @@
                 device_parser = IOSPicker.copy_on_write(namespace, self.dest)
                 device_parser.func = pick
 
         option_group = parser.add_argument_group(title="sib options")
         option_group.set_defaults(device_picker=IOSPicker(pick))
 
         device_group = option_group.add_mutually_exclusive_group()
-        device_group.add_argument(f"{prefix}u", f"{prefix}{prefix}udid", metavar="UDID", dest="device_picker", action=UdidAction,
+        device_group.add_argument("-u", "--udid", metavar="UDID", dest="device_picker", action=UdidAction,
                                   help="specify unique device identifier")
-        device_group.add_argument(f"{prefix}c", f"{prefix}{prefix}connect", metavar="IP:PORT", dest="device_picker", action=ConnectAction,
+        device_group.add_argument("-c", "--connect", metavar="IP:PORT", dest="device_picker", action=ConnectAction,
                                   help="use device with TCP/IP")
-        device_group.add_argument(f"{prefix}l", f"{prefix}{prefix}last", dest="device_picker", nargs=0, const=True, action=LastAction,
+        device_group.add_argument("-l", "--last", dest="device_picker", nargs=0, const=True, action=LastAction,
                                   help="use last device")
 
 
 class AndroidNamespace(Namespace):
     device_picker: AndroidPicker = None
```

### Comparing `linktools-0.8.2/src/linktools/container/__init__.py` & `linktools-0.8.2rc0/src/linktools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/container/container.py` & `linktools-0.8.2rc0/src/linktools/container/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/container/manager.py` & `linktools-0.8.2rc0/src/linktools/container/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,26 +352,26 @@
         )
 
     def create_process(
             self,
             *args,
             privilege: bool = None,
             **kwargs
-    ) -> utils.Process:
+    ) -> utils.Popen:
         if privilege:
             if self.system in ("darwin", "linux") and self.uid != 0:
                 args = ["sudo", *args]
-        return utils.Process(*args, **kwargs)
+        return utils.Popen(*args, **kwargs)
 
     def create_docker_process(
             self,
             *args,
             privilege: bool = None,
             **kwargs
-    ) -> utils.Process:
+    ) -> utils.Popen:
         commands = []
         if self.container_type in ("docker", "docker-rootless"):
             commands.extend(["docker"])
             if privilege is None:
                 privilege = self.container_type == "docker"
         elif self.container_type == "podman":
             commands.extend(["podman"])
@@ -381,15 +381,15 @@
 
     def create_docker_compose_process(
             self,
             containers: List[BaseContainer],
             *args: str,
             privilege: bool = None,
             **kwargs: Any
-    ) -> utils.Process:
+    ) -> utils.Popen:
         commands = []
         if self.container_type in ("docker", "docker-rootless"):
             commands.extend(["docker", "compose"])
             if privilege is None:
                 privilege = self.container_type == "docker"
         elif self.container_type == "podman":
             commands.extend(["podman", "compose"])
```

### Comparing `linktools-0.8.2/src/linktools/container/repository.py` & `linktools-0.8.2rc0/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/decorator.py` & `linktools-0.8.2rc0/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/device.py` & `linktools-0.8.2rc0/src/linktools/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         from .android import Adb
         from .ios import Sib
         for device in Adb().list_devices(alive=alive):
             yield device
         for device in Sib().list_devices(alive=alive):
             yield device
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Process:
+    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
         if self._tool is None:
             raise self._error_type("tool not found")
         return self._tool.popen(
             *(*self._options, *args),
             **kwargs
         )
```

### Comparing `linktools-0.8.2/src/linktools/frida/__init__.py` & `linktools-0.8.2rc0/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/frida/android.py` & `linktools-0.8.2rc0/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/frida/app.py` & `linktools-0.8.2rc0/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/frida/ios.py` & `linktools-0.8.2rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/frida/script.py` & `linktools-0.8.2rc0/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/frida/server.py` & `linktools-0.8.2rc0/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/ida/__init__.py` & `linktools-0.8.2rc0/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/ida/ida.py` & `linktools-0.8.2rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/ios/ipa.py` & `linktools-0.8.2rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/ios/sib.py` & `linktools-0.8.2rc0/src/linktools/ios/sib.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 return device.info
         raise SibError(f"device '{self.id}' not found")
 
     @cached_property
     def detail(self) -> dict:
         return self.info.get("deviceDetail")
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Process:
+    def popen(self, *args: [Any], **kwargs) -> utils.Popen:
         """
         执行命令
         :param args: 命令行参数
         :return: 打开的进程
         """
         args = ["--udid", self.id, *args]
         return self._sib.popen(*args, **kwargs)
```

### Comparing `linktools-0.8.2/src/linktools/metadata.py` & `linktools-0.8.2rc0/src/linktools/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.2"
+__version__ = "0.8.2rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.2)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.2rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.2/src/linktools/reactor.py` & `linktools-0.8.2rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.2rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.2rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/rich.py` & `linktools-0.8.2rc0/src/linktools/rich.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/ssh.py` & `linktools-0.8.2rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/utils/__init__.py` & `linktools-0.8.2rc0/src/linktools/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 )
 
 from ._lazy import (
     get_derived_type, lazy_load, lazy_iter, lazy_raise, lazy_import, lazy_import_file
 )
 
 from ._subprocess import (
-    Process,
+    Popen,
     list2cmdline,
 )
 
 from ._port import (
     is_port_free,
     pick_unused_port,
     NoFreePortFoundError,
```

### Comparing `linktools-0.8.2/src/linktools/utils/_lazy.py` & `linktools-0.8.2rc0/src/linktools/utils/_lazy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/utils/_port.py` & `linktools-0.8.2rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools/utils/_subprocess.py` & `linktools-0.8.2rc0/src/linktools/utils/_subprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 flag, data = self._queue.get_nowait()
                 if flag is not None:
                     yield flag, data
             except queue.Empty:
                 break
 
 
-class Process(subprocess.Popen):
+class Popen(subprocess.Popen):
 
     def __init__(self, *args, **kwargs):
         capture_output = kwargs.pop("capture_output", False)
         if capture_output is True:
             if kwargs.get("stdout") is not None or kwargs.get("stderr") is not None:
                 raise ValueError("stdout and stderr arguments may not be used "
                                  "with capture_output.")
@@ -98,19 +98,17 @@
             kwargs["stderr"] = subprocess.PIPE
         if "cwd" not in kwargs:
             try:
                 kwargs["cwd"] = os.getcwd()
             except FileNotFoundError:
                 kwargs["cwd"] = environ.get_temp_dir(create=True)
         if "append_env" in kwargs:
-            env = kwargs.pop("env", None)
-            env = dict(env) if env else dict()
+            env = os.environ.copy()
+            env.update(kwargs.pop("env", {}))
             env.update(kwargs.pop("append_env"))
-            for key, value in os.environ.items():
-                env.setdefault(key, value)
             kwargs["env"] = env
 
         args = [str(arg) for arg in args]
         environ.logger.debug(f"Exec cmdline: {list2cmdline(args)}")
 
         super().__init__(args, **kwargs)
```

### Comparing `linktools-0.8.2/src/linktools/utils/_utils.py` & `linktools-0.8.2rc0/src/linktools/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.2rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.2
+Version: 0.8.2rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.2/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.2rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.2rc0/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.2/src/linktools.egg-info/requires.txt` & `linktools-0.8.2rc0/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

