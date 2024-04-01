# Comparing `tmp/tinta-0.1.6.tar.gz` & `tmp/tinta-0.1.7b1.tar.gz`

## Comparing `tinta-0.1.6.tar` & `tinta-0.1.7b1.tar`

### file list

```diff
@@ -1,39 +1,43 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.6/.gitattributes
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.6/.pylintrc
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.6/DESCRIPTION.rst
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.6/HIPPOCRATIC_LICENSE.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.6/MANIFEST.in
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tinta-0.1.6/Pipfile
--rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 tinta-0.1.6/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.6/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.6/requirements.txt
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 tinta-0.1.6/setup.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.6/.github/workflows/publish-test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tinta-0.1.6/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 tinta-0.1.6/.vscode/launch.json
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 tinta-0.1.6/.vscode/settings.json
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 tinta-0.1.6/.vscode/tasks.json
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 tinta-0.1.6/examples/basic_example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.6/examples/colors.ini
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 tinta-0.1.6/examples/complete_example.py
--rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.6/examples/tinta-discover.png
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 tinta-0.1.6/tests/launch.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.6/tests/test_colors_invalid.ini
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tinta-0.1.6/tests/test_discover.py
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 tinta-0.1.6/tests/test_tinta.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/__main__.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/ansi.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/colorize.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/colors.ini
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/discover.py
--rw-r--r--   0        0        0    25390 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/tinta.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 tinta-0.1.6/tinta/typ.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.6/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.6/LICENSE
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 tinta-0.1.6/README.md
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 tinta-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 tinta-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b1/DESCRIPTION.rst
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b1/HIPPOCRATIC_LICENSE.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b1/MANIFEST.in
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tinta-0.1.7b1/Pipfile
+-rw-r--r--   0        0        0    45957 2020-02-02 00:00:00.000000 tinta-0.1.7b1/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b1/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tinta-0.1.7b1/requirements-dev.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tinta-0.1.7b1/requirements.txt
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b1/setup.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.vscode/launch.json
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.vscode/settings.json
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.vscode/tasks.json
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 tinta-0.1.7b1/examples/basic_example.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b1/examples/colors.ini
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 tinta-0.1.7b1/examples/complete_example.py
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b1/examples/tinta-discover.png
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b1/junit/test-results.xml
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tests/conftest.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tests/launch.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tests/test_colors_invalid.ini
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tests/test_discover.py
+-rw-r--r--   0        0        0     9924 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tests/test_tinta.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/__main__.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/ansi.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/colorize.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/colors.ini
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/discover.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/multi_version_imports.py
+-rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/tinta.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/typ.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tinta-0.1.7b1/tinta/utils.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b1/LICENSE
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 tinta-0.1.7b1/README.md
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 tinta-0.1.7b1/pyproject.toml
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 tinta-0.1.7b1/PKG-INFO
```

### Comparing `tinta-0.1.6/CODE_OF_CONDUCT.md` & `tinta-0.1.7b1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/HIPPOCRATIC_LICENSE.md` & `tinta-0.1.7b1/HIPPOCRATIC_LICENSE.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/Pipfile.lock` & `tinta-0.1.7b1/Pipfile.lock`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8597189465408805%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'d43dc087babb30228f18b4eda5df26c38f0dcb585bdbe4bf905541c18dda801e'}}",*

 * * "'default'": "{replace: OrderedDict([('deprecated', OrderedDict([('hashes', "*

 * *              "['sha256:6fac8b097794a90302bdbb17b9b815e732d3c4720583ff1b198499d78470466c', "*

 * *              "'sha256:e5323eb936458dccc2582dc6f9c322c852a775a27065ff2b0c4970b9d53d01b3']), "*

 * *              '(\'index\', \'pypi\'), (\'markers\', "python_version >= \'2.7\' and python_version '*

 * *              'not in \'3.0 […]*

```diff
@@ -1,71 +1,157 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "21ab7bdebcd985cd17de47821f4ac04925d0d95a1918970f91b64077845e2a7c"
+            "sha256": "d43dc087babb30228f18b4eda5df26c38f0dcb585bdbe4bf905541c18dda801e"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.6"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
-    "default": {},
+    "default": {
+        "deprecated": {
+            "hashes": [
+                "sha256:6fac8b097794a90302bdbb17b9b815e732d3c4720583ff1b198499d78470466c",
+                "sha256:e5323eb936458dccc2582dc6f9c322c852a775a27065ff2b0c4970b9d53d01b3"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.2.14"
+        },
+        "wrapt": {
+            "hashes": [
+                "sha256:0d2691979e93d06a95a26257adb7bfd0c93818e89b1406f5a28f36e0d8c1e1fc",
+                "sha256:14d7dc606219cdd7405133c713f2c218d4252f2a469003f8c46bb92d5d095d81",
+                "sha256:1a5db485fe2de4403f13fafdc231b0dbae5eca4359232d2efc79025527375b09",
+                "sha256:1acd723ee2a8826f3d53910255643e33673e1d11db84ce5880675954183ec47e",
+                "sha256:1ca9b6085e4f866bd584fb135a041bfc32cab916e69f714a7d1d397f8c4891ca",
+                "sha256:1dd50a2696ff89f57bd8847647a1c363b687d3d796dc30d4dd4a9d1689a706f0",
+                "sha256:2076fad65c6736184e77d7d4729b63a6d1ae0b70da4868adeec40989858eb3fb",
+                "sha256:2a88e6010048489cda82b1326889ec075a8c856c2e6a256072b28eaee3ccf487",
+                "sha256:3ebf019be5c09d400cf7b024aa52b1f3aeebeff51550d007e92c3c1c4afc2a40",
+                "sha256:418abb18146475c310d7a6dc71143d6f7adec5b004ac9ce08dc7a34e2babdc5c",
+                "sha256:43aa59eadec7890d9958748db829df269f0368521ba6dc68cc172d5d03ed8060",
+                "sha256:44a2754372e32ab315734c6c73b24351d06e77ffff6ae27d2ecf14cf3d229202",
+                "sha256:490b0ee15c1a55be9c1bd8609b8cecd60e325f0575fc98f50058eae366e01f41",
+                "sha256:49aac49dc4782cb04f58986e81ea0b4768e4ff197b57324dcbd7699c5dfb40b9",
+                "sha256:5eb404d89131ec9b4f748fa5cfb5346802e5ee8836f57d516576e61f304f3b7b",
+                "sha256:5f15814a33e42b04e3de432e573aa557f9f0f56458745c2074952f564c50e664",
+                "sha256:5f370f952971e7d17c7d1ead40e49f32345a7f7a5373571ef44d800d06b1899d",
+                "sha256:66027d667efe95cc4fa945af59f92c5a02c6f5bb6012bff9e60542c74c75c362",
+                "sha256:66dfbaa7cfa3eb707bbfcd46dab2bc6207b005cbc9caa2199bcbc81d95071a00",
+                "sha256:685f568fa5e627e93f3b52fda002c7ed2fa1800b50ce51f6ed1d572d8ab3e7fc",
+                "sha256:6906c4100a8fcbf2fa735f6059214bb13b97f75b1a61777fcf6432121ef12ef1",
+                "sha256:6a42cd0cfa8ffc1915aef79cb4284f6383d8a3e9dcca70c445dcfdd639d51267",
+                "sha256:6dcfcffe73710be01d90cae08c3e548d90932d37b39ef83969ae135d36ef3956",
+                "sha256:6f6eac2360f2d543cc875a0e5efd413b6cbd483cb3ad7ebf888884a6e0d2e966",
+                "sha256:72554a23c78a8e7aa02abbd699d129eead8b147a23c56e08d08dfc29cfdddca1",
+                "sha256:73870c364c11f03ed072dda68ff7aea6d2a3a5c3fe250d917a429c7432e15228",
+                "sha256:73aa7d98215d39b8455f103de64391cb79dfcad601701a3aa0dddacf74911d72",
+                "sha256:75ea7d0ee2a15733684badb16de6794894ed9c55aa5e9903260922f0482e687d",
+                "sha256:7bd2d7ff69a2cac767fbf7a2b206add2e9a210e57947dd7ce03e25d03d2de292",
+                "sha256:807cc8543a477ab7422f1120a217054f958a66ef7314f76dd9e77d3f02cdccd0",
+                "sha256:8e9723528b9f787dc59168369e42ae1c3b0d3fadb2f1a71de14531d321ee05b0",
+                "sha256:9090c9e676d5236a6948330e83cb89969f433b1943a558968f659ead07cb3b36",
+                "sha256:9153ed35fc5e4fa3b2fe97bddaa7cbec0ed22412b85bcdaf54aeba92ea37428c",
+                "sha256:9159485323798c8dc530a224bd3ffcf76659319ccc7bbd52e01e73bd0241a0c5",
+                "sha256:941988b89b4fd6b41c3f0bfb20e92bd23746579736b7343283297c4c8cbae68f",
+                "sha256:94265b00870aa407bd0cbcfd536f17ecde43b94fb8d228560a1e9d3041462d73",
+                "sha256:98b5e1f498a8ca1858a1cdbffb023bfd954da4e3fa2c0cb5853d40014557248b",
+                "sha256:9b201ae332c3637a42f02d1045e1d0cccfdc41f1f2f801dafbaa7e9b4797bfc2",
+                "sha256:a0ea261ce52b5952bf669684a251a66df239ec6d441ccb59ec7afa882265d593",
+                "sha256:a33a747400b94b6d6b8a165e4480264a64a78c8a4c734b62136062e9a248dd39",
+                "sha256:a452f9ca3e3267cd4d0fcf2edd0d035b1934ac2bd7e0e57ac91ad6b95c0c6389",
+                "sha256:a86373cf37cd7764f2201b76496aba58a52e76dedfaa698ef9e9688bfd9e41cf",
+                "sha256:ac83a914ebaf589b69f7d0a1277602ff494e21f4c2f743313414378f8f50a4cf",
+                "sha256:aefbc4cb0a54f91af643660a0a150ce2c090d3652cf4052a5397fb2de549cd89",
+                "sha256:b3646eefa23daeba62643a58aac816945cadc0afaf21800a1421eeba5f6cfb9c",
+                "sha256:b47cfad9e9bbbed2339081f4e346c93ecd7ab504299403320bf85f7f85c7d46c",
+                "sha256:b935ae30c6e7400022b50f8d359c03ed233d45b725cfdd299462f41ee5ffba6f",
+                "sha256:bb2dee3874a500de01c93d5c71415fcaef1d858370d405824783e7a8ef5db440",
+                "sha256:bc57efac2da352a51cc4658878a68d2b1b67dbe9d33c36cb826ca449d80a8465",
+                "sha256:bf5703fdeb350e36885f2875d853ce13172ae281c56e509f4e6eca049bdfb136",
+                "sha256:c31f72b1b6624c9d863fc095da460802f43a7c6868c5dda140f51da24fd47d7b",
+                "sha256:c5cd603b575ebceca7da5a3a251e69561bec509e0b46e4993e1cac402b7247b8",
+                "sha256:d2efee35b4b0a347e0d99d28e884dfd82797852d62fcd7ebdeee26f3ceb72cf3",
+                "sha256:d462f28826f4657968ae51d2181a074dfe03c200d6131690b7d65d55b0f360f8",
+                "sha256:d5e49454f19ef621089e204f862388d29e6e8d8b162efce05208913dde5b9ad6",
+                "sha256:da4813f751142436b075ed7aa012a8778aa43a99f7b36afe9b742d3ed8bdc95e",
+                "sha256:db2e408d983b0e61e238cf579c09ef7020560441906ca990fe8412153e3b291f",
+                "sha256:db98ad84a55eb09b3c32a96c576476777e87c520a34e2519d3e59c44710c002c",
+                "sha256:dbed418ba5c3dce92619656802cc5355cb679e58d0d89b50f116e4a9d5a9603e",
+                "sha256:dcdba5c86e368442528f7060039eda390cc4091bfd1dca41e8046af7c910dda8",
+                "sha256:decbfa2f618fa8ed81c95ee18a387ff973143c656ef800c9f24fb7e9c16054e2",
+                "sha256:e4fdb9275308292e880dcbeb12546df7f3e0f96c6b41197e0cf37d2826359020",
+                "sha256:eb1b046be06b0fce7249f1d025cd359b4b80fc1c3e24ad9eca33e0dcdb2e4a35",
+                "sha256:eb6e651000a19c96f452c85132811d25e9264d836951022d6e81df2fff38337d",
+                "sha256:ed867c42c268f876097248e05b6117a65bcd1e63b779e916fe2e33cd6fd0d3c3",
+                "sha256:edfad1d29c73f9b863ebe7082ae9321374ccb10879eeabc84ba3b69f2579d537",
+                "sha256:f2058f813d4f2b5e3a9eb2eb3faf8f1d99b81c3e51aeda4b168406443e8ba809",
+                "sha256:f6b2d0c6703c988d334f297aa5df18c45e97b0af3679bb75059e0e0bd8b1069d",
+                "sha256:f8212564d49c50eb4565e502814f694e240c55551a5f1bc841d4fcaabb0a9b8a",
+                "sha256:ffa565331890b90056c01db69c0fe634a776f8019c143a5ae265f9c6bc4bd6d4"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==1.16.0"
+        }
+    },
     "develop": {
         "astroid": {
             "hashes": [
                 "sha256:951798f922990137ac090c53af473db7ab4e70c770e6d7fae0cec59f74411819",
                 "sha256:ac248253bfa4bd924a0de213707e7ebeeb3138abeb48d798784ead1e56d419d4"
             ],
             "markers": "python_full_version >= '3.8.0'",
             "version": "==3.1.0"
         },
         "autopep8": {
             "hashes": [
-                "sha256:067959ca4a07b24dbd5345efa8325f5f58da4298dab0dde0443d5ed765de80cb",
-                "sha256:2913064abd97b3419d1cc83ea71f042cb821f87e45b9c88cad5ad3c4ea87fe0c"
+                "sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7",
+                "sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.4"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.1.0"
         },
         "black": {
             "hashes": [
-                "sha256:057c3dc602eaa6fdc451069bd027a1b2635028b575a6c3acfd63193ced20d9c8",
-                "sha256:08654d0797e65f2423f850fc8e16a0ce50925f9337fb4a4a176a7aa4026e63f8",
-                "sha256:163baf4ef40e6897a2a9b83890e59141cc8c2a98f2dda5080dc15c00ee1e62cd",
-                "sha256:1e08fb9a15c914b81dd734ddd7fb10513016e5ce7e6704bdd5e1251ceee51ac9",
-                "sha256:4dd76e9468d5536abd40ffbc7a247f83b2324f0c050556d9c371c2b9a9a95e31",
-                "sha256:4f9de21bafcba9683853f6c96c2d515e364aee631b178eaa5145fc1c61a3cc92",
-                "sha256:61a0391772490ddfb8a693c067df1ef5227257e72b0e4108482b8d41b5aee13f",
-                "sha256:6981eae48b3b33399c8757036c7f5d48a535b962a7c2310d19361edeef64ce29",
-                "sha256:7e53a8c630f71db01b28cd9602a1ada68c937cbf2c333e6ed041390d6968faf4",
-                "sha256:810d445ae6069ce64030c78ff6127cd9cd178a9ac3361435708b907d8a04c693",
-                "sha256:93601c2deb321b4bad8f95df408e3fb3943d85012dddb6121336b8e24a0d1218",
-                "sha256:992e451b04667116680cb88f63449267c13e1ad134f30087dec8527242e9862a",
-                "sha256:9db528bccb9e8e20c08e716b3b09c6bdd64da0dd129b11e160bf082d4642ac23",
-                "sha256:a0057f800de6acc4407fe75bb147b0c2b5cbb7c3ed110d3e5999cd01184d53b0",
-                "sha256:ba15742a13de85e9b8f3239c8f807723991fbfae24bad92d34a2b12e81904982",
-                "sha256:bce4f25c27c3435e4dace4815bcb2008b87e167e3bf4ee47ccdc5ce906eb4894",
-                "sha256:ca610d29415ee1a30a3f30fab7a8f4144e9d34c89a235d81292a1edb2b55f540",
-                "sha256:d533d5e3259720fdbc1b37444491b024003e012c5173f7d06825a77508085430",
-                "sha256:d84f29eb3ee44859052073b7636533ec995bd0f64e2fb43aeceefc70090e752b",
-                "sha256:e37c99f89929af50ffaf912454b3e3b47fd64109659026b678c091a4cd450fb2",
-                "sha256:e8a6ae970537e67830776488bca52000eaa37fa63b9988e8c487458d9cd5ace6",
-                "sha256:faf2ee02e6612577ba0181f4347bcbcf591eb122f7841ae5ba233d12c39dcb4d"
+                "sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f",
+                "sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93",
+                "sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11",
+                "sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0",
+                "sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9",
+                "sha256:56f52cfbd3dabe2798d76dbdd299faa046a901041faf2cf33288bc4e6dae57b5",
+                "sha256:65b76c275e4c1c5ce6e9870911384bff5ca31ab63d19c76811cb1fb162678213",
+                "sha256:65c02e4ea2ae09d16314d30912a58ada9a5c4fdfedf9512d23326128ac08ac3d",
+                "sha256:6905238a754ceb7788a73f02b45637d820b2f5478b20fec82ea865e4f5d4d9f7",
+                "sha256:79dcf34b33e38ed1b17434693763301d7ccbd1c5860674a8f871bd15139e7837",
+                "sha256:7bb041dca0d784697af4646d3b62ba4a6b028276ae878e53f6b4f74ddd6db99f",
+                "sha256:7d5e026f8da0322b5662fa7a8e752b3fa2dac1c1cbc213c3d7ff9bdd0ab12395",
+                "sha256:9f50ea1132e2189d8dff0115ab75b65590a3e97de1e143795adb4ce317934995",
+                "sha256:a0c9c4a0771afc6919578cec71ce82a3e31e054904e7197deacbc9382671c41f",
+                "sha256:aadf7a02d947936ee418777e0247ea114f78aff0d0959461057cae8a04f20597",
+                "sha256:b5991d523eee14756f3c8d5df5231550ae8993e2286b8014e2fdea7156ed0959",
+                "sha256:bf21b7b230718a5f08bd32d5e4f1db7fc8788345c8aea1d155fc17852b3410f5",
+                "sha256:c45f8dff244b3c431b36e3224b6be4a127c6aca780853574c00faf99258041eb",
+                "sha256:c7ed6668cbbfcd231fa0dc1b137d3e40c04c7f786e626b405c62bcd5db5857e4",
+                "sha256:d7de8d330763c66663661a1ffd432274a2f92f07feeddd89ffd085b5744f85e7",
+                "sha256:e19cb1c6365fd6dc38a6eae2dcb691d7d83935c10215aef8e6c38edee3f77abd",
+                "sha256:e2af80566f43c85f5797365077fb64a393861a3730bd110971ab7a0c94e873e7"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==24.2.0"
+            "version": "==24.3.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
                 "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
@@ -176,69 +262,69 @@
             "version": "==8.1.7"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:0209a6369ccce576b43bb227dc8322d8ef9e323d089c6f3f26a597b09cb4d2aa",
-                "sha256:062b0a75d9261e2f9c6d071753f7eef0fc9caf3a2c82d36d76667ba7b6470003",
-                "sha256:0842571634f39016a6c03e9d4aba502be652a6e4455fadb73cd3a3a49173e38f",
-                "sha256:16bae383a9cc5abab9bb05c10a3e5a52e0a788325dc9ba8499e821885928968c",
-                "sha256:18c7320695c949de11a351742ee001849912fd57e62a706d83dfc1581897fa2e",
-                "sha256:18d90523ce7553dd0b7e23cbb28865db23cddfd683a38fb224115f7826de78d0",
-                "sha256:1bf25fbca0c8d121a3e92a2a0555c7e5bc981aee5c3fdaf4bb7809f410f696b9",
-                "sha256:276f6077a5c61447a48d133ed13e759c09e62aff0dc84274a68dc18660104d52",
-                "sha256:280459f0a03cecbe8800786cdc23067a8fc64c0bd51dc614008d9c36e1659d7e",
-                "sha256:28ca2098939eabab044ad68850aac8f8db6bf0b29bc7f2887d05889b17346454",
-                "sha256:2c854ce44e1ee31bda4e318af1dbcfc929026d12c5ed030095ad98197eeeaed0",
-                "sha256:35eb581efdacf7b7422af677b92170da4ef34500467381e805944a3201df2079",
-                "sha256:37389611ba54fd6d278fde86eb2c013c8e50232e38f5c68235d09d0a3f8aa352",
-                "sha256:3b253094dbe1b431d3a4ac2f053b6d7ede2664ac559705a704f621742e034f1f",
-                "sha256:3b2eccb883368f9e972e216c7b4c7c06cabda925b5f06dde0650281cb7666a30",
-                "sha256:451f433ad901b3bb00184d83fd83d135fb682d780b38af7944c9faeecb1e0bfe",
-                "sha256:489763b2d037b164846ebac0cbd368b8a4ca56385c4090807ff9fad817de4113",
-                "sha256:4af154d617c875b52651dd8dd17a31270c495082f3d55f6128e7629658d63765",
-                "sha256:506edb1dd49e13a2d4cac6a5173317b82a23c9d6e8df63efb4f0380de0fbccbc",
-                "sha256:6679060424faa9c11808598504c3ab472de4531c571ab2befa32f4971835788e",
-                "sha256:69b9f6f66c0af29642e73a520b6fed25ff9fd69a25975ebe6acb297234eda501",
-                "sha256:6c00cdc8fa4e50e1cc1f941a7f2e3e0f26cb2a1233c9696f26963ff58445bac7",
-                "sha256:6c0cdedd3500e0511eac1517bf560149764b7d8e65cb800d8bf1c63ebf39edd2",
-                "sha256:708a3369dcf055c00ddeeaa2b20f0dd1ce664eeabde6623e516c5228b753654f",
-                "sha256:718187eeb9849fc6cc23e0d9b092bc2348821c5e1a901c9f8975df0bc785bfd4",
-                "sha256:767b35c3a246bcb55b8044fd3a43b8cd553dd1f9f2c1eeb87a302b1f8daa0524",
-                "sha256:77fbfc5720cceac9c200054b9fab50cb2a7d79660609200ab83f5db96162d20c",
-                "sha256:7cbde573904625509a3f37b6fecea974e363460b556a627c60dc2f47e2fffa51",
-                "sha256:8249b1c7334be8f8c3abcaaa996e1e4927b0e5a23b65f5bf6cfe3180d8ca7840",
-                "sha256:8580b827d4746d47294c0e0b92854c85a92c2227927433998f0d3320ae8a71b6",
-                "sha256:8640f1fde5e1b8e3439fe482cdc2b0bb6c329f4bb161927c28d2e8879c6029ee",
-                "sha256:9a9babb9466fe1da12417a4aed923e90124a534736de6201794a3aea9d98484e",
-                "sha256:a78ed23b08e8ab524551f52953a8a05d61c3a760781762aac49f8de6eede8c45",
-                "sha256:abbbd8093c5229c72d4c2926afaee0e6e3140de69d5dcd918b2921f2f0c8baba",
-                "sha256:ae7f19afe0cce50039e2c782bff379c7e347cba335429678450b8fe81c4ef96d",
-                "sha256:b3ec74cfef2d985e145baae90d9b1b32f85e1741b04cd967aaf9cfa84c1334f3",
-                "sha256:b51bfc348925e92a9bd9b2e48dad13431b57011fd1038f08316e6bf1df107d10",
-                "sha256:b9a4a8dd3dcf4cbd3165737358e4d7dfbd9d59902ad11e3b15eebb6393b0446e",
-                "sha256:ba3a8aaed13770e970b3df46980cb068d1c24af1a1968b7818b69af8c4347efb",
-                "sha256:c0524de3ff096e15fcbfe8f056fdb4ea0bf497d584454f344d59fce069d3e6e9",
-                "sha256:c0a120238dd71c68484f02562f6d446d736adcc6ca0993712289b102705a9a3a",
-                "sha256:cbbe5e739d45a52f3200a771c6d2c7acf89eb2524890a4a3aa1a7fa0695d2a47",
-                "sha256:ce8c50520f57ec57aa21a63ea4f325c7b657386b3f02ccaedeccf9ebe27686e1",
-                "sha256:cf30900aa1ba595312ae41978b95e256e419d8a823af79ce670835409fc02ad3",
-                "sha256:d25b937a5d9ffa857d41be042b4238dd61db888533b53bc76dc082cb5a15e914",
-                "sha256:d6cdecaedea1ea9e033d8adf6a0ab11107b49571bbb9737175444cea6eb72328",
-                "sha256:dec9de46a33cf2dd87a5254af095a409ea3bf952d85ad339751e7de6d962cde6",
-                "sha256:ebe7c9e67a2d15fa97b77ea6571ce5e1e1f6b0db71d1d5e96f8d2bf134303c1d",
-                "sha256:ee866acc0861caebb4f2ab79f0b94dbfbdbfadc19f82e6e9c93930f74e11d7a0",
-                "sha256:f6a09b360d67e589236a44f0c39218a8efba2593b6abdccc300a8862cffc2f94",
-                "sha256:fcc66e222cf4c719fe7722a403888b1f5e1682d1679bd780e2b26c18bb648cdc",
-                "sha256:fd6545d97c98a192c5ac995d21c894b581f1fd14cf389be90724d21808b657e2"
+                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
+                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
+                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
+                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
+                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
+                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
+                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
+                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
+                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
+                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
+                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
+                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
+                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
+                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
+                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
+                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
+                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
+                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
+                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
+                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
+                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
+                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
+                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
+                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
+                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
+                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
+                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
+                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
+                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
+                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
+                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
+                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
+                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
+                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
+                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
+                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
+                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
+                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
+                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
+                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
+                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
+                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
+                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
+                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
+                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
+                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
+                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
+                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
+                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
+                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
+                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
+                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.4.3"
+            "version": "==7.4.4"
         },
         "dill": {
             "hashes": [
                 "sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca",
                 "sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7"
             ],
             "markers": "python_version >= '3.11'",
@@ -255,38 +341,30 @@
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.20.1"
         },
-        "editables": {
-            "hashes": [
-                "sha256:309627d9b5c4adc0e668d8c6fa7bac1ba7c8c5d415c2d27f60f081f8e80d1de2",
-                "sha256:61e5ffa82629e0d8bfe09bc44a07db3c1ab8ed1ce78a6980732870f19b5e7d4c"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.5"
-        },
         "filelock": {
             "hashes": [
                 "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e",
                 "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.13.1"
         },
         "hatchling": {
             "hashes": [
-                "sha256:21e8c13f8458b219a91cb84e5b61c15bf786695d1c4fabc29e91e78f94bfe892",
-                "sha256:bba440453a224e7d4478457fa2e8d8c3633765bafa02975a6b53b9bf917980bc"
+                "sha256:5fdf7b689c1e76cf280bfe002e5e3d7efe99f63e559d2dc3e5d5f49de489d57d",
+                "sha256:f2dfce8e5d389c53c41c87f5c643c5ef2f9519510eaaddda0aac63eb52470684"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==1.21.1"
+            "version": "==1.22.2"
         },
         "idna": {
             "hashes": [
                 "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
                 "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
             ],
             "markers": "python_version >= '3.5'",
@@ -557,44 +635,44 @@
                 "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.7.1"
         },
         "ruff": {
             "hashes": [
-                "sha256:0ac06a3759c3ab9ef86bbeca665d31ad3aa9a4b1c17684aadb7e61c10baa0df4",
-                "sha256:0c1bdd9920cab5707c26c8b3bf33a064a4ca7842d91a99ec0634fec68f9f4037",
-                "sha256:1231eacd4510f73222940727ac927bc5d07667a86b0cbe822024dd00343e77e9",
-                "sha256:2c6d613b19e9a8021be2ee1d0e27710208d1603b56f47203d0abbde906929a9b",
-                "sha256:5f65103b1d76e0d600cabd577b04179ff592064eaa451a70a81085930e907d0b",
-                "sha256:77f2612752e25f730da7421ca5e3147b213dca4f9a0f7e0b534e9562c5441f01",
-                "sha256:967978ac2d4506255e2f52afe70dda023fc602b283e97685c8447d036863a302",
-                "sha256:9966b964b2dd1107797be9ca7195002b874424d1d5472097701ae8f43eadef5d",
-                "sha256:9bd640a8f7dd07a0b6901fcebccedadeb1a705a50350fb86b4003b805c81385a",
-                "sha256:b74c3de9103bd35df2bb05d8b2899bf2dbe4efda6474ea9681280648ec4d237d",
-                "sha256:b83d17ff166aa0659d1e1deaf9f2f14cbe387293a906de09bc4860717eb2e2da",
-                "sha256:bb875c6cc87b3703aeda85f01c9aebdce3d217aeaca3c2e52e38077383f7268a",
-                "sha256:be75e468a6a86426430373d81c041b7605137a28f7014a72d2fc749e47f572aa",
-                "sha256:c8439338a6303585d27b66b4626cbde89bb3e50fa3cae86ce52c1db7449330a7",
-                "sha256:de8b480d8379620cbb5ea466a9e53bb467d2fb07c7eca54a4aa8576483c35d36",
-                "sha256:f380be9fc15a99765c9cf316b40b9da1f6ad2ab9639e551703e581a5e6da6745",
-                "sha256:fa78ec9418eb1ca3db392811df3376b46471ae93792a81af2d1cbb0e5dcb5142"
+                "sha256:0171aab5fecdc54383993389710a3d1227f2da124d76a2784a7098e818f92d61",
+                "sha256:0da458989ce0159555ef224d5b7c24d3d2e4bf4c300b85467b08c3261c6bc6a8",
+                "sha256:1eca7ff7a47043cf6ce5c7f45f603b09121a7cc047447744b029d1b719278eb5",
+                "sha256:2700a804d5336bcffe063fd789ca2c7b02b552d2e323a336700abb8ae9e6a3f8",
+                "sha256:352e95ead6964974b234e16ba8a66dad102ec7bf8ac064a23f95371d8b198aab",
+                "sha256:38671be06f57a2f8aba957d9f701ea889aa5736be806f18c0cd03d6ff0cbca8d",
+                "sha256:45817af234605525cdf6317005923bf532514e1ea3d9270acf61ca2440691376",
+                "sha256:5a6cbf216b69c7090f0fe4669501a27326c34e119068c1494f35aaf4cc683778",
+                "sha256:79bca3a03a759cc773fca69e0bdeac8abd1c13c31b798d5bb3c9da4a03144a9f",
+                "sha256:8d6ab88c81c4040a817aa432484e838aaddf8bfd7ca70e4e615482757acb64f8",
+                "sha256:973a0e388b7bc2e9148c7f9be8b8c6ae7471b9be37e1cc732f8f44a6f6d7720d",
+                "sha256:b24c19e8598916d9c6f5a5437671f55ee93c212a2c4c569605dc3842b6820386",
+                "sha256:be90bcae57c24d9f9d023b12d627e958eb55f595428bafcb7fec0791ad25ddfc",
+                "sha256:cfa60d23269d6e2031129b053fdb4e5a7b0637fc6c9c0586737b962b2f834493",
+                "sha256:e7d3f6762217c1da954de24b4a1a70515630d29f71e268ec5000afe81377642d",
+                "sha256:f2831ec6a580a97f1ea82ea1eda0401c3cdf512cf2045fa3c85e8ef109e87de0",
+                "sha256:fd66469f1a18fdb9d32e22b79f486223052ddf057dc56dea0caaf1a47bdfaf4e"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
-            "version": "==0.3.2"
+            "version": "==0.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:02fa291a0471b3a18b2b2481ed902af520c69e8ae0919c13da936542754b4c56",
-                "sha256:5c0806c7d9af348e6dd3777b4f4dbb42c7ad85b190104837488eab9a7c945cf8"
+                "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e",
+                "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==69.1.1"
+            "version": "==69.2.0"
         },
         "tomlkit": {
             "hashes": [
                 "sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b",
                 "sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3"
             ],
             "markers": "python_version >= '3.7'",
@@ -612,14 +690,23 @@
                 "sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4",
                 "sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==5.0.0"
         },
+        "types-deprecated": {
+            "hashes": [
+                "sha256:0680e89989a8142707de8103f15d182445a533c1047fd9b7e8c5459101e9b90a",
+                "sha256:d7793aaf32ff8f7e49a8ac781de4872248e0694c4b75a7a8a186c51167463f9d"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '3.8'",
+            "version": "==1.2.9.20240311"
+        },
         "typing-extensions": {
             "hashes": [
                 "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475",
                 "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.10.0"
@@ -638,28 +725,28 @@
                 "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==20.25.1"
         },
         "wheel": {
             "hashes": [
-                "sha256:177f9c9b0d45c47873b619f5b650346d632cdc35fb5e4d25058e09c9e581433d",
-                "sha256:c45be39f7882c9d34243236f2d63cbd58039e360f85d0913425fbd7ceea617a8"
+                "sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85",
+                "sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==0.42.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.43.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31",
-                "sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0"
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.17.0"
+            "version": "==3.18.1"
         }
     },
     "test-packages": {
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
```

### Comparing `tinta-0.1.6/setup.py` & `tinta-0.1.7b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from setuptools import setup
 
 with Path("README.md").open(encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="tinta",
-    version="0.1.6",
+    version="0.1.7b1",
     description="Tinta, a magical console output tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/brandonscript/tinta",
     author="Brandon Shelley",
     author_email="brandon@pacificaviator.co",
     install_requires=[],
```

### Comparing `tinta-0.1.6/.github/workflows/publish-test.yml` & `tinta-0.1.7b1/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/.github/workflows/publish.yml` & `tinta-0.1.7b1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/.github/workflows/run-tests.yml` & `tinta-0.1.7b1/.github/workflows/run-tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -22,19 +22,19 @@
           python-version: ${{ matrix.python-version }}
           cache: "pip"
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pylint pytest
+          pip install pytest deprecated
       - name: Test with pytest
         run: |
-          pip install pytest pytest-cov
-          pytest -xv --doctest-modules --junitxml=junit/test-results.xml --cov=com --cov-report=xml --cov-report=html
+          pip install pytest
+          pytest -xv -s
 
   build-newer-python:
     runs-on: ubuntu-22.04
     strategy:
       matrix:
         python-version: ["3.11", "3.12"]
 
@@ -46,12 +46,12 @@
           python-version: ${{ matrix.python-version }}
           cache: "pip"
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pylint pytest
+          pip install pytest deprecated
       - name: Test with pytest
         run: |
-          pip install pytest pytest-cov
-          pytest -xv --doctest-modules --junitxml=junit/test-results.xml --cov=com --cov-report=xml --cov-report=html
+          pip install pytest
+          pytest -xv -s
```

### Comparing `tinta-0.1.6/.vscode/launch.json` & `tinta-0.1.7b1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/.vscode/settings.json` & `tinta-0.1.7b1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/examples/basic_example.py` & `tinta-0.1.7b1/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/examples/complete_example.py` & `tinta-0.1.7b1/examples/complete_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/examples/tinta-discover.png` & `tinta-0.1.7b1/examples/tinta-discover.png`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/tests/conftest.py` & `tinta-0.1.7b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/tests/launch.json` & `tinta-0.1.7b1/tests/launch.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/tests/test_tinta.py` & `tinta-0.1.7b1/tests/test_tinta.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,14 +80,39 @@
     def test_black(self):
         Tinta().black("black").print()
 
     def test_white(self):
         Tinta().white("white").print()
 
 
+class TestLowerLevel:
+
+    ITS_NOT_EASY = "it's not easy being green"
+
+    def assert_its_not_easy_being_green(self, out: str):
+        assert self.ITS_NOT_EASY in out
+        assert "\x1b[38;5;35m" in out
+
+    def test_tint_takes_int_arg0_as_color(self):
+        out = Tinta().tint(35, self.ITS_NOT_EASY).to_str()
+        self.assert_its_not_easy_being_green(out)
+
+    def test_tint_takes_str_arg0_as_color(self):
+        out = Tinta().tint("green", self.ITS_NOT_EASY).to_str()
+        self.assert_its_not_easy_being_green(out)
+
+    def test_tint_takes_int_color_kwarg(self):
+        out = Tinta().tint(self.ITS_NOT_EASY, color=35).to_str()
+        self.assert_its_not_easy_being_green(out)
+
+    def test_tint_takes_str_color_kwarg(self):
+        out = Tinta().tint(self.ITS_NOT_EASY, color="green").to_str()
+        self.assert_its_not_easy_being_green(out)
+
+
 class TestEdgeCases:
 
     @pytest.mark.xfail()
     def test_missing_color(self):
         Tinta().sparkle().print()
 
     @pytest.mark.xfail()
@@ -249,43 +274,43 @@
         dog = "cat"
         assert (
             Tinta(f"A {dog} is a human's best friend").get_plaintext()
             == "A cat is a human's best friend"
         )
         assert Tinta(f"A {Tinta().red('hologram').to_str()} is a human's best friend")
 
-    def test_add(self):
+    def test_push(self):
         t = Tinta().push("How long").push("can two people talk about nothing?")
         assert t.get_plaintext() == "How long can two people talk about nothing?"
 
         assert len(t.parts) == 2
         assert len(t.parts_fmt) == 2
         assert len(t.parts_pln) == 2
 
         t = Tinta().push("How long", "can two people talk about nothing?")
         assert t.get_plaintext() == "How long can two people talk about nothing?"
 
         assert len(t.parts) == 1
         assert len(t.parts_fmt) == 1
         assert len(t.parts_pln) == 1
 
-    def test_remove(self):
+    def test_pop(self):
         t = Tinta().push("How long").push("can two people talk about nothing?")
-        t.remove()
+        t.pop()
         assert t.get_plaintext() == "How long"
         assert len(t.parts) == 1
         assert len(t.parts_fmt) == 1
         assert len(t.parts_pln) == 1
 
         t = Tinta()
         for p in range(10):
             t.push(str(p))
 
         assert len(t.parts) == 10
-        t.remove(10)
+        t.pop(10)
 
         assert len(t.parts) == 0
 
         t.remove(2)  # Shouldn't error if we remove more than we have
 
         assert len(t.parts) == 0
```

### Comparing `tinta-0.1.6/tinta/__init__.py` & `tinta-0.1.7b1/tinta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = "0.1.6"
+__version__ = "0.1.7b1"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 
     assert bool(Tinta)
```

### Comparing `tinta-0.1.6/tinta/__main__.py` & `tinta-0.1.7b1/tinta/__main__.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/tinta/ansi.py` & `tinta-0.1.7b1/tinta/ansi.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/tinta/colorize.py` & `tinta-0.1.7b1/tinta/colorize.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/tinta/discover.py` & `tinta-0.1.7b1/tinta/discover.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,113 +39,103 @@
         172  173  174  175  176  177     190  191  192  193  194  195
         208  209  210  211  212  213     226  227  228  229  230  231
 
     Greyscale:  232   233   234   235   236   237   238   239   240   241   242   243
                 244   245   246   247   248   249   250   251   252   253   254   255
 """
 
-import sys
-from collections.abc import Iterable
-from typing import List, Union
-
-if sys.version_info >= (3, 8):
-    from typing import Literal, TypeVar
-elif sys.version_info >= (3, 5):
-    from typing import TypeVar
+from typing import cast, List
 
-    from typing_extensions import Literal
+from .multi_version_imports import Literal
+from .utils import flatmap
+
+STANDARD: List[int] = list(range(8))
+BRIGHT: List[int] = list(range(8, 16))
+DARK_GREYSCALE: List[int] = list(range(232, 244))
+DARK_COLOR1: List[List[int]] = [
+    [16, 17, 18, 19, 20, 21],
+    [52, 53, 54, 55, 56, 57],
+    [88, 89, 90, 91, 92, 93],
+    [124, 125, 126, 127, 128, 129],
+    [160, 161, 162, 163, 164, 165],
+    [196, 197, 198, 199, 200, 201],
+]
+
+DARK_COLOR2: List[List[int]] = [
+    [22, 23, 24, 25, 26, 27],
+    [58, 59, 60, 61, 62, 63],
+    [94, 95, 96, 97, 98, 99],
+    [130, 131, 132, 133, 134, 135],
+    [166, 167, 168, 169, 170, 171],
+    [202, 203, 204, 205, 206, 207],
+]
+
+DARK_COLOR3: List[List[int]] = [
+    [28, 29, 30, 31, 32, 33],
+    [64, 65, 66, 67, 68, 69],
+    [100, 101, 102, 103, 104, 105],
+    [136, 137, 138, 139, 140, 141],
+    [172, 173, 174, 175, 176, 177],
+    [208, 209, 210, 211, 212, 213],
+]
+DARK_COLORS = sorted(
+    flatmap(DARK_COLOR1)
+    + flatmap(DARK_COLOR2)
+    + flatmap(DARK_COLOR3)
+    + DARK_GREYSCALE
+    + STANDARD
+)
+
+LIGHT_GREYSCALE: List[int] = list(range(244, 256))
+LIGHT_COLOR1: List[List[int]] = [
+    [34, 35, 36, 37, 38, 39],
+    [70, 71, 72, 73, 74, 75],
+    [106, 107, 108, 109, 110, 111],
+    [142, 143, 144, 145, 146, 147],
+    [178, 179, 180, 181, 182, 183],
+    [214, 215, 216, 217, 218, 219],
+]
+
+LIGHT_COLOR2: List[List[int]] = [
+    [40, 41, 42, 43, 44, 45],
+    [76, 77, 78, 79, 80, 81],
+    [112, 113, 114, 115, 116, 117],
+    [148, 149, 150, 151, 152, 153],
+    [184, 185, 186, 187, 188, 189],
+    [220, 221, 222, 223, 224, 225],
+]
+
+LIGHT_COLOR3: List[List[int]] = [
+    [46, 47, 48, 49, 50, 51],
+    [82, 83, 84, 85, 86, 87],
+    [118, 119, 120, 121, 122, 123],
+    [154, 155, 156, 157, 158, 159],
+    [190, 191, 192, 193, 194, 195],
+    [226, 227, 228, 229, 230, 231],
+]
 
 color_sets = {
-    "standard": [0, 1, 2, 3, 4, 5, 6, 7],
-    "bright": [8, 9, 10, 11, 12, 13, 14, 15],
     "dark": {
-        "greyscale": [232, 233, 234, 235, 236, 237, 238, 239, 240, 241, 242, 243],
-        "color1": [
-            [16, 17, 18, 19, 20, 21],
-            [52, 53, 54, 55, 56, 57],
-            [88, 89, 90, 91, 92, 93],
-            [124, 125, 126, 127, 128, 129],
-            [160, 161, 162, 163, 164, 165],
-            [196, 197, 198, 199, 200, 201],
-        ],
-        "color2": [
-            [22, 23, 24, 25, 26, 27],
-            [58, 59, 60, 61, 62, 63],
-            [94, 95, 96, 97, 98, 99],
-            [130, 131, 132, 133, 134, 135],
-            [166, 167, 168, 169, 170, 171],
-            [202, 203, 204, 205, 206, 207],
-        ],
-        "color3": [
-            [28, 29, 30, 31, 32, 33],
-            [64, 65, 66, 67, 68, 69],
-            [100, 101, 102, 103, 104, 105],
-            [136, 137, 138, 139, 140, 141],
-            [172, 173, 174, 175, 176, 177],
-            [208, 209, 210, 211, 212, 213],
-        ],
+        "color1": DARK_COLOR1,
+        "color2": DARK_COLOR2,
+        "color3": DARK_COLOR3,
+        "greyscale": DARK_GREYSCALE,
     },
     "light": {
-        "greyscale": [244, 245, 246, 247, 248, 249, 250, 251, 252, 253, 254, 255],
-        "color1": [
-            [34, 35, 36, 37, 38, 39],
-            [70, 71, 72, 73, 74, 75],
-            [106, 107, 108, 109, 110, 111],
-            [142, 143, 144, 145, 146, 147],
-            [178, 179, 180, 181, 182, 183],
-            [214, 215, 216, 217, 218, 219],
-        ],
-        "color2": [
-            [40, 41, 42, 43, 44, 45],
-            [76, 77, 78, 79, 80, 81],
-            [112, 113, 114, 115, 116, 117],
-            [148, 149, 150, 151, 152, 153],
-            [184, 185, 186, 187, 188, 189],
-            [220, 221, 222, 223, 224, 225],
-        ],
-        "color3": [
-            [46, 47, 48, 49, 50, 51],
-            [82, 83, 84, 85, 86, 87],
-            [118, 119, 120, 121, 122, 123],
-            [154, 155, 156, 157, 158, 159],
-            [190, 191, 192, 193, 194, 195],
-            [226, 227, 228, 229, 230, 231],
-        ],
+        "color1": LIGHT_COLOR1,
+        "color2": LIGHT_COLOR2,
+        "color3": LIGHT_COLOR3,
+        "greyscale": LIGHT_GREYSCALE,
     },
 }
 
-T = TypeVar("T")
-
-
-def flatten(lst: Union[List[T], List[List[T]]]) -> List[T]:
-    """Flattens a list of lists into a single list. If the list is already flat,
-    it is returned as is.
-    """
-
-    flattened = []
-    for item in lst:
-        if isinstance(item, Iterable) and not isinstance(item, (str, bytes)):
-            for sub_x in flatten(item):  # type: ignore
-                flattened.append(sub_x)
-        else:
-            flattened.append(item)
-    return flattened
-
 
 def is_dark(code: int) -> bool:
     """Returns True if the given color is a dark color, False otherwise."""
-    dark_colors = sorted(
-        flatten(color_sets["dark"]["color1"])
-        + flatten(color_sets["dark"]["color2"])
-        + flatten(color_sets["dark"]["color3"])
-        + color_sets["dark"]["greyscale"]
-        + [0, 1, 2, 3, 4, 5, 6, 8, 9]
-    )
-
-    return code in dark_colors
+    return code in DARK_COLORS
 
 
 def colorbox(code: int, background: bool = False) -> str:
     """Returns a padded, styled box for the given color. If the color is
     too dark, the text is white, otherwise dark grey.
     """
 
@@ -160,28 +150,33 @@
         return f"\033[0m\033[38;5;{code}m{text}\033[0m"
 
 
 def discover(background: bool = False):
     """Prints all 256 colors in a matrix on your system."""
 
     print("Standard: ", end="")
-    for col in color_sets["standard"]:
+    for col in STANDARD:
         print(colorbox(col, background), end="")
 
     print("\nBright:   ", end="")
-    for col in color_sets["bright"]:
+    for col in BRIGHT:
         print(colorbox(col, background), end="")
 
     print("\n")
 
     def print_row(brightness: Literal["light", "dark"], cset: int, row: int, i: int):
         cset_key = "color" + str(cset)
         col = (row * 6) + i
+        colorset = cast(List[List[int]], color_sets[brightness][cset_key])
         print(
-            colorbox(flatten(color_sets[brightness][cset_key])[col], background), end=""
+            colorbox(
+                flatmap(colorset)[col],
+                background,
+            ),
+            end="",
         )
 
     for cset in range(1, 4):
         # printing 18 lines of colors:
         # [16, 17, 18, 19, 20, 21]   [34, 35, 36, 37, 38, 39]
         # [52, 53, 54, 55, 56, 57]   [70, 71, 72, 73, 74, 75]
         # .. etc. for the other 4 color sets
@@ -192,15 +187,15 @@
             print(str().rjust(1 if background else 4), end="")
             for i in range(6):
                 print_row("light", cset, row, i)
             print("")
         print("")
 
     print("Greyscale: ", end="")
-    for grey in color_sets["dark"]["greyscale"]:
+    for grey in DARK_GREYSCALE:
         print(colorbox(grey, background), end="")
 
     print("\n           ", end="")
-    for grey in color_sets["light"]["greyscale"]:
+    for grey in LIGHT_GREYSCALE:
         print(colorbox(grey, background), end="")
 
     print("\n")
```

### Comparing `tinta-0.1.6/tinta/tinta.py` & `tinta-0.1.7b1/tinta/tinta.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,36 +21,15 @@
 import os
 import re
 import sys
 from itertools import zip_longest
 from pathlib import Path
 from typing import Any, cast, List, Optional, overload, Union
 
-try:
-    from typing import deprecated
-except ImportError:
-    try:
-        from typing_extensions import deprecated
-    except ImportError:
-        from typing import cast
-
-        def deprecated(msg: str) -> Any:
-            def _decorator(func: Any) -> Any:
-                return cast(Any, func)
-
-            return _decorator
-
-
-try:
-    from typing import Self
-except ImportError:
-    try:
-        from typing_extensions import Self
-    except ImportError:
-        Self = "Tinta"
+from deprecated import deprecated
 
 from .ansi import AnsiColors
 from .colorize import ANSI_RESET_HEX, colorize
 from .discover import discover as _discover
 from .typ import copy_kwargs, MissingColorError, parse_bool, StringType
 
 config = configparser.ConfigParser()
@@ -429,38 +408,52 @@
             self._parts.pop()
         return self
 
     @deprecated("Use pop() instead.")
     def remove(self, qty: int = 1) -> "Tinta":
         return self.pop(qty)
 
+    @overload
+    def tint(self, *s: Any, color: Union[str, int], sep: str = SEP) -> "Tinta": ...
+
+    @overload
+    def tint(self, color: Union[str, int], *s: Any, sep: str = SEP) -> "Tinta": ...
+
     # pylint: disable=redefined-outer-name
-    def tint(
-        self, color: Optional[Union[str, int]] = None, *s: Any, sep: str = SEP
-    ) -> "Tinta":
+    def tint(self, *args, **kwargs) -> "Tinta":
         """Adds segments of text colored with the specified color.
         Can be used in place of calling named color methods.
 
         Args:
             color (str | int, optional): A color name or ANSI color index. Defaults to first argument.
             *s: Any: Segments of text to add.
             sep (str, optional): Used to join strings. Defaults to ' '.
 
         Returns:
             self
         """
 
+        # color: Optional[Union[str, int]] = None, *s: Any, sep: str = SEP
+
+        # check if the first argument is a known color or valid ANSI code, or comes from kwargs
+        s = args
+        color = kwargs.get("color", None)
+        sep = kwargs.get("sep", SEP)
         if color is None:
             if not len(s) > 1:
                 raise AttributeError(
                     "If no color is specified, tint() requires at least two arguments."
                 )
-
-            color = s[0]
-            s = s[1:]
+            if args and isinstance(args[0], (str, int)):
+                color = s[0]
+                s = s[1:]
+            else:
+                raise AttributeError(
+                    "Could not determine color from arguments. Either pass a color as the first argument, or use the color keyword argument."
+                )
 
         # if color is numeric integer string, assume it's an ANSI color code
         if isinstance(color, int) or (isinstance(color, str) and color.isdigit()):
             self.color = int(color)
 
         # Check if color_name is a valid color if color is a string
         if isinstance(color, str):
@@ -677,38 +670,38 @@
             flush=flush,
         )
 
         self.clear()
         self._parts = []
         print("\033[0m", end="", file=file, flush=flush)
 
-    def __getattr__(self, name: str) -> Self:
+    def __getattr__(self, name: str) -> "Tinta":
         """Returns a tinted segment of text.
 
         Args:
             name (str): Name of the color.
 
         Returns:
             Tinta: A Tinta instance.
         """
 
         if not name.startswith("_"):
             if hasattr(self.colors, name):
-                return cast(Self, self.tint(color=name))
+                return cast("Tinta", self.tint(color=name))
 
             else:
                 try:
-                    return self.__getattribute__(name)
+                    return self.__getattribute__(name)  # type: ignore
                 except AttributeError as e:
                     known_colors = f"- {'- '.join(self.colors.list_colors())}"
                     raise AttributeError(
                         f"Attribute '{name}' not found. Did you try and access a color that doesn't exist? Available colors:\n{known_colors}"
                     ) from e
 
-        return self.__getattribute__(name)
+        return self.__getattribute__(name)  # type: ignore
 
     @staticmethod
     def discover(background=False):
         """Prints all 256 colors in a matrix on your system. If background is True,
         it will print background colors with numbers on top."""
         _discover(background)
 
@@ -759,18 +752,18 @@
         def esc(self):
             return esc(self.fmt)
 
         @property
         def has_formatting(self) -> bool:
             return self.fmt != self.pln
 
-
-def escape_ansi(line):
-    ansi_escape = re.compile(r"(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]")
-    return ansi_escape.sub("", line)
+    @staticmethod
+    def strip_ansi(s: str) -> str:
+        """A utility method that strips ANSI escape codes from a string, converting a styled string into plaintext."""
+        return re.sub(r"(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]", "", s, re.I, re.M)
 
 
 def esc(string: str, replace: bool = False) -> str:
     """Returns the raw representation of a string. If replace is true,
     replace a double backslash with a single backslash."""
     r = repr(string)[1:-1]  # Strip the quotes from representation
     if replace:
```

### Comparing `tinta-0.1.6/tinta/typ.py` & `tinta-0.1.7b1/tinta/typ.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,34 +9,17 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # If you use this software, you must also agree under the terms of the Hippocratic License 3.0 to not use this software in a way that directly or indirectly causes harm. You can find the full text of the license at https://firstdonoharm.dev.
 
 """This module contains type hints and utility functions for Tinta."""
 import functools
-import inspect
-import sys
 from typing import Any, Callable, cast
 
-if sys.version_info >= (3, 10):
-    from typing import Literal, ParamSpec, TypeVar
-
-    P = ParamSpec("P") if sys.version_info >= (3, 10) else ...  # type: ignore
-    R = TypeVar("R")  # type: ignore
-
-    GenericCallable = Callable[P, R]
-elif sys.version_info >= (3, 8):
-    from typing import Literal
-
-    GenericCallable = Any
-else:
-    from typing_extensions import Literal
-
-    GenericCallable = Any
-
+from .multi_version_imports import GenericCallable, Literal
 
 StringType = Literal["pln", "esc", "fmt"]  # type: ignore
 
 
 class MissingColorError(Exception):
     """Raised when a color is not found in the colors.ini file."""
 
@@ -46,18 +29,20 @@
 def copy_kwargs(func: GenericCallable) -> Callable[..., GenericCallable]:
     """Decorator does nothing but casts the original function to match the given function signature"""
 
     @functools.wraps(func, updated=())
     def _cast_func(_func: Callable[..., Any]) -> GenericCallable:
         return cast(GenericCallable, _func)
 
-    if inspect.isfunction(func):
-        return _cast_func
+    if not callable(func):
+        raise RuntimeError(
+            f"You must pass a function to this decorator, got {func} instead."
+        )
 
-    raise RuntimeError("You must pass a function to this decorator.")
+    return _cast_func
 
 
 def parse_bool(value: Any) -> bool:
     """Parses a string value to a boolean value."""
     if isinstance(value, bool):
         return value
     return str(value).lower() in ("true", "1", "t", "y", "yes")
```

### Comparing `tinta-0.1.6/.gitignore` & `tinta-0.1.7b1/.gitignore`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/LICENSE` & `tinta-0.1.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinta-0.1.6/README.md` & `tinta-0.1.7b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.6-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b1-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -170,32 +170,34 @@
 Tinta().red()
 Tinta().blue()
 Tinta().wine()
 Tinta().my_color()
 # etc.
 ```
 
-A note on linters like Pylance or pylint: these methods are dynamically generated, so they won't be recognized by your linter. Until Python natively supports type definitions for dynamically generated code, you will have to suppress these warnings:
+A note on linters like Pylance or pylint: these methods are dynamically generated, so they won't be recognized by your linter as built-in methods. Until Python natively supports type definitions for dynamically generated code, you may have to suppress these warnings:
 
 ```python
 # pyright: reportGeneralTypeIssues=false
 Tinta().green() # or
 # pylint: disable=no-member
 Tinta().green()
+
+Tinta().green() # type: ignore
 ```
 
-If this is frustrating, you can always use the `Tinta.code(<int>)` or the `Tinta.tint(<color>)` methods, which are not dynamically generated.
+If this is frustrating, you can always use the `Tinta.tint(<color>)` methods, which are not dynamically generated.
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.6 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b1 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -222,15 +224,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.6 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b1 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
 
@@ -320,14 +322,21 @@
 Just set the `color` kwarg to specify an ANSI color code or string name:
 
 ```python
 Tinta().tint('A bear who knows all the answers', color=42).print()
 Tinta().tint('A brown bear', color='brown').print()
 ```
 
+If you don't pass a color kwarg, the first argument will be used as the color:
+
+```python
+Tinta().tint(42, 'A bear who knows all the answers').print()
+Tinta().tint('brown', 'A brown bear').print()
+```
+
 ## Environment Variables
 
 Sometimes it's useful to globally configure `Tinta` on a system where you might want it to behave differently, without changing your source code. If these Environment variables are present on the system, they will be considered True.
 
 `TINTA_STEALTH` – Disables console output globally
 
 `TINTA_PLAINTEXT` – Disables rich console output, only printing plain text.
```

### Comparing `tinta-0.1.6/pyproject.toml` & `tinta-0.1.7b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 [project]
 name = "tinta"
-version = "0.1.6"
+version = "0.1.7b1"
 description = "Tinta, a magical console output tool."
 authors = [{ name = "Brandon Shelley", email = "brandon@pacificaviator.co" }]
 license = "MIT"
 readme = "README.md"
 keywords = [
   "console",
   "colors",
@@ -63,58 +63,59 @@
 [tool.hatchling.build]
 packages = ["tinta"]
 include = ["tinta/**/*.py", "tinta/**/*.pyi", "tinta/colors.ini", "/tests"]
 exclude = [".*", "dist"]
 
 [tool.hatchling.dependencies]
 python = "^3.6"
+deprecated = "^1.2.14"
 
 [tool.hatchling.dev-dependencies]
 pytest = "^6.2.4"
 twine = "^3.4.2"
 wheel = "^0.36.2"
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 warn_return_any = true
 warn_unused_configs = true
 explicit_package_bases = true
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.mypy-applications]
 ignore_missing_imports = false
 
 [tool.mypy-common]
 ignore_missing_imports = false
 check_untyped_defs = true
 
 [tool.black]
-target-version = ['py310']
+target-version = ['py311']
 preview = true
 
 [tool.isort]
 profile = "black"
 order_by_type = false
 combine_as_imports = true
 case_sensitive = false
 skip_magic_trailing_comma = true
 force_sort_within_sections = false
 
 [tool.pyright]
 # verboseOutput = true
-pythonVersion = "3.10"
+pythonVersion = "3.11"
 extraPaths = [".venv/lib/python3.11/site-packages", "tinta", "**/*.py"]
 reportUnusedImport = "error"
 reportUnusedClass = "error"
 reportUnusedFunction = "error"
 reportUnusedVariable = "error"
 
 [tool.ruff]
-target-version = "py310"
+target-version = "py311"
 line-length = 100
 indent-width = 4
 preview = true
 
 [tool.ruff.lint]
 fixable = ["ALL"]
 select = [
@@ -150,12 +151,12 @@
 line-ending = "auto"
 skip-magic-trailing-comma = false
 quote-style = "double"
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 minversion = "7.0"
-addopts = "-rP -vv --color=yes"
+addopts = "-s -rP -x -vv --color=yes"
 testpaths = ["tests"]
 python_files = ["*_test.py", "test_*.py"]
 python_classes = ["test_", "_test", "Test*"]
 python_functions = ["test_", "_test"]
```

### Comparing `tinta-0.1.6/PKG-INFO` & `tinta-0.1.7b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tinta
-Version: 0.1.6
+Version: 0.1.7b1
 Summary: Tinta, a magical console output tool.
 Project-URL: homepage, https://github.com/brandonscript/tinta
 Project-URL: repository, https://github.com/brandonscript/tinta
 Author-email: Brandon Shelley <brandon@pacificaviator.co>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ansi,cli,colors,console,development,print,term,terminal
@@ -25,15 +25,15 @@
 
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.6-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b1-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -195,32 +195,34 @@
 Tinta().red()
 Tinta().blue()
 Tinta().wine()
 Tinta().my_color()
 # etc.
 ```
 
-A note on linters like Pylance or pylint: these methods are dynamically generated, so they won't be recognized by your linter. Until Python natively supports type definitions for dynamically generated code, you will have to suppress these warnings:
+A note on linters like Pylance or pylint: these methods are dynamically generated, so they won't be recognized by your linter as built-in methods. Until Python natively supports type definitions for dynamically generated code, you may have to suppress these warnings:
 
 ```python
 # pyright: reportGeneralTypeIssues=false
 Tinta().green() # or
 # pylint: disable=no-member
 Tinta().green()
+
+Tinta().green() # type: ignore
 ```
 
-If this is frustrating, you can always use the `Tinta.code(<int>)` or the `Tinta.tint(<color>)` methods, which are not dynamically generated.
+If this is frustrating, you can always use the `Tinta.tint(<color>)` methods, which are not dynamically generated.
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.6 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b1 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -247,15 +249,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.6 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b1 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
 
@@ -345,14 +347,21 @@
 Just set the `color` kwarg to specify an ANSI color code or string name:
 
 ```python
 Tinta().tint('A bear who knows all the answers', color=42).print()
 Tinta().tint('A brown bear', color='brown').print()
 ```
 
+If you don't pass a color kwarg, the first argument will be used as the color:
+
+```python
+Tinta().tint(42, 'A bear who knows all the answers').print()
+Tinta().tint('brown', 'A brown bear').print()
+```
+
 ## Environment Variables
 
 Sometimes it's useful to globally configure `Tinta` on a system where you might want it to behave differently, without changing your source code. If these Environment variables are present on the system, they will be considered True.
 
 `TINTA_STEALTH` – Disables console output globally
 
 `TINTA_PLAINTEXT` – Disables rich console output, only printing plain text.
```

