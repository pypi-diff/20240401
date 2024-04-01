# Comparing `tmp/offspot_config-1.8.2.tar.gz` & `tmp/offspot_config-1.9.0.tar.gz`

## Comparing `offspot_config-1.8.2.tar` & `offspot_config-1.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-1.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 offspot_config-1.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-1.8.2/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/__init__.py
--rw-r--r--   0        0        0    27503 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/builder.py
--rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/catalog.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/catalog.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/constants.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/file.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/inputs.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/oci_images.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/packages.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/zim.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/utils/__init__.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/utils/download.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/utils/misc.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/utils/sizes.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_config/utils/yaml.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/__init__.py
--rwxr-xr-x   0        0        0    17655 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/ap.py
--rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/checks.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/configlib.py
--rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/containers.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/dnsmasqspoof.py
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/ethernet.py
--rwxr-xr-x   0        0        0     7595 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/fromfile.py
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/hostname.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-1.8.2/src/offspot_runtime/timezone.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-1.8.2/tests/test_catalog.py
--rw-r--r--   0        0        0    20227 2020-02-02 00:00:00.000000 offspot_config-1.8.2/tests/test_checks.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-1.8.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-1.8.2/LICENSE
--rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 offspot_config-1.8.2/README.md
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 offspot_config-1.8.2/pyproject.toml
--rw-r--r--   0        0        0    10636 2020-02-02 00:00:00.000000 offspot_config-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 offspot_config-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-1.9.0/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/__init__.py
+-rw-r--r--   0        0        0    27601 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/builder.py
+-rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/catalog.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/catalog.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/constants.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/file.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/inputs.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/oci_images.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/packages.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/zim.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/__init__.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/download.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/misc.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/sizes.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/yaml.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/__init__.py
+-rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/ap.py
+-rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/checks.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/configlib.py
+-rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/containers.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/dnsmasqspoof.py
+-rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/ethernet.py
+-rwxr-xr-x   0        0        0     7627 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/fromfile.py
+-rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/hostname.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/timezone.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-1.9.0/tests/test_catalog.py
+-rw-r--r--   0        0        0    20270 2020-02-02 00:00:00.000000 offspot_config-1.9.0/tests/test_checks.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-1.9.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 offspot_config-1.9.0/README.md
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 offspot_config-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 offspot_config-1.9.0/PKG-INFO
```

### Comparing `offspot_config-1.8.2/.pre-commit-config.yaml` & `offspot_config-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/CHANGELOG.md` & `offspot_config-1.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.9.0] - 2024-02-09
+
+### Added
+
+- [builder] AP welcome_domain now settable (defaulting to `goto.kiwix`)
+- [ap] `captured-address` allows setting the DNS fallback target for when offline
+
+## Changed
+
+- [ap] Auto `spoof` dnsmasq switcher now toggles by uncommenting what's commented and commenting what's not.
+- [ap] `no-resolv` and `dhcp-athoritative` added to DNSmasq config
+- [ap] Upstream `server` for DNSmasq only set when Online
+
 ## [1.8.2] - 2024-02-05
 
 ### Changed
 
 - [builder] Using reverse-proxy 1.6
 
 ## [1.8.1] - 2024-02-05
```

### Comparing `offspot_config-1.8.2/tasks.py` & `offspot_config-1.9.0/tasks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/builder.py` & `offspot_config-1.9.0/src/offspot_config/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     def __init__(
         self,
         *,
         base: BaseConfig,
         name: str = "My Offspot",
         tld: str | None = "offspot",
         domain: str | None = "my-offspot",
+        welcome_domain: str | None = "goto.kiwix",
         ssid: str | None = "my-offspot",
         passphrase: str | None = None,
         timezone: str | None = "UTC",  # noqa: ARG002
         as_gateway: bool | None = False,
         environ: dict[str, str] | None = None,
         write_config: bool | None = False,
         kiwix_zim_mirror: str | None = None,
@@ -107,14 +108,15 @@
             "write_config": write_config,
             "offspot": {
                 "timezone": "UTC",
                 "hostname": domain,
                 "ethernet": {"type": "dhcp"},
                 "ap": {
                     "domain": domain,
+                    "welcome": welcome_domain,
                     "tld": tld,
                     "ssid": ssid,
                     "passphrase": passphrase,
                     "as-gateway": as_gateway,
                 },
                 "containers": {"name": "offspot", "services": {}},
             },
```

### Comparing `offspot_config-1.8.2/src/offspot_config/catalog.json` & `offspot_config-1.9.0/src/offspot_config/catalog.json`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/catalog.py` & `offspot_config-1.9.0/src/offspot_config/catalog.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/constants.py` & `offspot_config-1.9.0/src/offspot_config/constants.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/file.py` & `offspot_config-1.9.0/src/offspot_config/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/inputs.py` & `offspot_config-1.9.0/src/offspot_config/inputs.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/oci_images.py` & `offspot_config-1.9.0/src/offspot_config/oci_images.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/packages.py` & `offspot_config-1.9.0/src/offspot_config/packages.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/zim.py` & `offspot_config-1.9.0/src/offspot_config/zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/utils/download.py` & `offspot_config-1.9.0/src/offspot_config/utils/download.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/utils/misc.py` & `offspot_config-1.9.0/src/offspot_config/utils/misc.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/utils/sizes.py` & `offspot_config-1.9.0/src/offspot_config/utils/sizes.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_config/utils/yaml.py` & `offspot_config-1.9.0/src/offspot_config/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_runtime/ap.py` & `offspot_config-1.9.0/src/offspot_runtime/ap.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 NAME = pathlib.Path(__file__).stem
 
 RFKILL_PATH = pathlib.Path("/usr/sbin/rfkill")
 IPTABLES_PATH = pathlib.Path("/usr/sbin/iptables")
 DEFAULT_CHANNEL = 11
 DEFAULT_ADDRESS = "192.168.2.1"
+DEFAULT_CAPTURED_ADDRESS = "198.51.100.1"
 DEFAULT_DNS = ["8.8.8.8", "1.1.1.1"]
 DEFAULT_TLD = "offspot"
 DEFAULT_DOMAIN = "generic"
 DEFAULT_WELCOME_DOMAIN = "goto.generic"
 HOSTAPD_CONF_PATH = pathlib.Path("/etc/hostapd/hostapd.conf")
 NF_MASQUERADE_RULES_PATH = IPTABLES_DIR / "offspot-masquerade.rules"
 NF_FORWARDING_RULES_PATH = IPTABLES_DIR / "offspot-forwarding.rules"
@@ -98,18 +99,18 @@
 {other_interfaces_ranges_lines}
 {nodhcp_interfaces_lines}
 
 expand-hosts
 bogus-priv
 domain={tld},{network},local
 
-address=/{welcome_fqdn}/{address}
-address=/{fqdn}/{address}
-{servers}
+address=/{welcome_fqdn}/{fqdn}/{address}
 no-hosts
+no-resolv
+dhcp-authoritative
 conf-file={DNSMASQ_SPOOF_CONFIG_PATH}
 """
 INTERFACES_CONF = """
 allow-hotplug {interface}
 iface {interface} inet static
 address {address}
 netmask {netmask}
@@ -193,21 +194,30 @@
 
     return 0
 
 
 def write_dnsmasq_spoof_conf(dnsmasq_spoof_conf_path: pathlib.Path, **kwargs) -> int:
     """std-returncode writing dnsmasq-spoof.conf
 
-    at this stage, we only enable spoof is spoof was unconditionaly requested.
+    at this stage, we only enable spoof if spoof was unconditionaly requested.
     auto-spoof would be triggered externaly"""
-    line = "address=/#/1.1.1.1"
-    if not kwargs["spoof"]:
-        line = f"# {line}"
 
-    dnsmasq_spoof_conf_path.write_text(f"{line}\n")
+    lines = ["## use similar ## prefix for manual comments"]
+    line = "" if kwargs["spoof"] else "# "  # address is enabled on spoof
+    line += f"address=/#/{kwargs['captured_address']}"
+    lines.append(line)
+
+    for server in kwargs["servers"]:
+        line = "# " if kwargs["spoof"] else ""  # servers are disabled on spoof
+        line += f"server={server}"
+        lines.append(line)
+
+    lines.append("")  # end fine on a new line
+
+    dnsmasq_spoof_conf_path.write_text("\n".join(lines))
 
     return 0
 
 
 def write_dnsmasq_conf(dnsmasq_conf_path: pathlib.Path, **kwargs) -> int:
     """std-returncode, building and writing dnsmasq.conf from kwargs"""
 
@@ -228,20 +238,14 @@
     kwargs["except_interfaces_lines"] = "\n".join(
         [f"except-interface={iface}" for iface in kwargs["except_interfaces"]]
     )
     kwargs["nodhcp_interfaces_lines"] = "\n".join(
         [f"no-dhcp-interface={iface}" for iface in kwargs["nodhcp_interfaces"]]
     )
 
-    if kwargs["as_gateway"]:
-        kwargs["servers"] = "\n".join([f"server={server}" for server in kwargs["dns"]])
-    # no internet, no need for DNS
-    else:
-        kwargs["servers"] = ""
-
     # additional, static/local records
     kwargs["fqdn"] = f"{kwargs['domain']}.{kwargs['tld']}"
     kwargs["welcome_fqdn"] = f"{kwargs['welcome_domain']}.{kwargs['tld']}"
 
     # write to a temp file and check syntax first
     temp_conf = pathlib.Path(tempfile.NamedTemporaryFile(suffix=".conf").name)
     temp_conf.write_text(DNSMASQ_CONF_TEMPLATE.format(**kwargs))
@@ -337,14 +341,15 @@
         welcome=kwargs["welcome_domain"],
         channel=kwargs["channel"],
         country=kwargs["country_code"],
         interface=kwargs["interface"],
         dhcp_range=kwargs["dhcp_range"],
         network=kwargs["network"],
         dns=kwargs["dns"],
+        captured_address=kwargs["captured_address"],
         other_interfaces=kwargs["other_interfaces"],
         except_interfaces=kwargs["except_interfaces"],
         nodhcp_interfaces=kwargs["nodhcp_interfaces"],
     )
     if not check.passed:
         fail_invalid(check.help_text)
 
@@ -362,14 +367,20 @@
         fail_error("hostapd restart failed")
     logger.debug("hostapd restarted")
 
     if set_ip_address(kwargs["interface"], kwargs["address"]) != 0:
         fail_error("failed to set {kwargs['address']=} on {kwargs['interface']=}")
     logger.debug("ip-address set")
 
+    if kwargs["as_gateway"]:
+        kwargs["servers"] = kwargs["dns"]
+    # no internet, no need for DNS
+    else:
+        kwargs["servers"] = []
+
     _str_spoof = str(kwargs["spoof"]).strip().lower()
     kwargs["auto_spoof"] = _str_spoof == "auto"
     kwargs["spoof"] = not kwargs["auto_spoof"] and _str_spoof == "true"
     if (
         write_dnsmasq_spoof_conf(
             dnsmasq_spoof_conf_path=DNSMASQ_SPOOF_CONFIG_PATH, **kwargs
         )
@@ -549,14 +560,22 @@
         dest="dns",
         default=[],
         required=False,
         action="append",
     )
 
     parser.add_argument(
+        "--captured-address",
+        help="IP address to send all HTTP/s traffic to when offline",
+        dest="captured_address",
+        required=False,
+        default=DEFAULT_CAPTURED_ADDRESS,
+    )
+
+    parser.add_argument(
         "--other-interfaces",
         help="Additional interfaces to provide DNS and DHCP on.",
         dest="other_interfaces",
         default=[],
         required=False,
         action="append",
     )
```

### Comparing `offspot_config-1.8.2/src/offspot_runtime/checks.py` & `offspot_config-1.9.0/src/offspot_runtime/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,14 +464,15 @@
     welcome: str,
     channel: int,
     country: str,
     interface: str,
     dhcp_range: str,
     network: str,
     dns: list[str],
+    captured_address: str,
     other_interfaces: list[str],
     except_interfaces: list[str],
     nodhcp_interfaces: list[str],
 ) -> CheckResponse:
     """whether valid ap config values"""
     check = is_valid_ssid(ssid)
     if not check.passed:
@@ -528,14 +529,17 @@
     if not isinstance(dns, list):
         return CheckResponse(False, "DNS: Incorrect type")
     for index, server in enumerate(dns):
         check = is_valid_ipv4(server)
         if not check.passed:
             return CheckResponse(False, f"DNS #{index}: {check.help_text}")
 
+    if not is_valid_ipv4(captured_address):
+        return CheckResponse(False, "Invalid IPv4 captured_address")
+
     if not isinstance(other_interfaces, list):
         return CheckResponse(False, "Other-interfaces: Incorrect type")
     for index, iface in enumerate(other_interfaces):
         check = is_valid_interface_name(iface)
         if not check.passed:
             return CheckResponse(False, f"Other-interfaces #{index}: {check.help_text}")
```

### Comparing `offspot_config-1.8.2/src/offspot_runtime/configlib.py` & `offspot_config-1.9.0/src/offspot_runtime/configlib.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_runtime/containers.py` & `offspot_config-1.9.0/src/offspot_runtime/containers.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_runtime/dnsmasqspoof.py` & `offspot_config-1.9.0/src/offspot_runtime/dnsmasqspoof.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,29 +42,29 @@
     if (spoof and is_spoof) or (not spoof and not is_spoof):
         logger.info(f"already in correct mode: {is_spoof=} {spoof=}")
         return False
 
     logger.info(f"toggling from {is_spoof=} into {spoof=}")
 
     # turning non-spoof into spoof by removing comment on address
-    if spoof and not is_spoof:
-        for line in content.splitlines():
-            m = re.match(r"^\s*#\s+(?P<line>address=/#/.+)$", line)
-            if m:
-                content = f"{m.groupdict()['line']}\n"
-                break
-
-    # turning spoof into non-spoof
-    else:
-        for line in content.splitlines():
-            if line.startswith("address=/#/"):
-                content = f"# {line}\n"
-                break
+    fixed_lines = []
+    for line in content.splitlines():
+        # keep manual comments as-is
+        if line.startswith("##"):
+            fixed_lines.append(line)
+            continue
+
+        # uncomment commented lines
+        comment_match = re.match(r"^#\s(?P<line>.+)$", line)
+        if comment_match:
+            fixed_lines.append(comment_match.groupdict()["line"])
+        else:
+            fixed_lines.append(f"# {line}")
 
-    dnsmasq_conf_path.write_text(content)
+    dnsmasq_conf_path.write_text("\n".join(fixed_lines))
 
     return True
 
 
 def restart_dnsmasq():
     return (
         subprocess.run(
```

### Comparing `offspot_config-1.8.2/src/offspot_runtime/ethernet.py` & `offspot_config-1.9.0/src/offspot_runtime/ethernet.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_runtime/fromfile.py` & `offspot_config-1.9.0/src/offspot_runtime/fromfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
             "welcome",
             "channel",
             "country",
             "interface",
             "dhcp-range",
             "network",
             "spoof",
+            "captured-address",
         ):
             if item.get(key) is not None:
                 command += [f"--{key}", str(item.get(key))]
 
         for key in ("hide", "as-gateway"):
             if item.get(key):
                 command += [f"--{key}"]
```

### Comparing `offspot_config-1.8.2/src/offspot_runtime/hostname.py` & `offspot_config-1.9.0/src/offspot_runtime/hostname.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/src/offspot_runtime/timezone.py` & `offspot_config-1.9.0/src/offspot_runtime/timezone.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/tests/test_checks.py` & `offspot_config-1.9.0/tests/test_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,14 +386,15 @@
         "welcome": "goto.generic",
         "channel": 11,
         "country": "US",
         "interface": "wlan0",
         "dhcp_range": "192.168.2.2,192.168.2.254,255.255.255.0,1h",
         "network": "192.168.2.0/24",
         "dns": ["8.8.8.8", "1.1.1.1"],
+        "captured_address": "192.168.0.1",
         "other_interfaces": [],
         "except_interfaces": [],
         "nodhcp_interfaces": [],
     }
     config = defaults.copy()
     assert not is_valid_ap_config(**config)
```

### Comparing `offspot_config-1.8.2/.gitignore` & `offspot_config-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/LICENSE` & `offspot_config-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/README.md` & `offspot_config-1.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -158,32 +158,35 @@
 
 Without an *armor*, configuration is appended at end of file, specifying `eth0` interface if missing (untouched `dhcpcd.conf`)
 
 ### `ap`
 
 `ap` is itself an `object`.
 
-| Member       | Kind       | Required | Function   |
-|--------------|----------- |----------|------------|
-| `ssid    `   | `string`   | **yes**  | SSID (Network Name)                                                                                        |
-| `passphrase` | `string`   | no | Passphrase/password to connect to the network. Defaults to Open Network                                          |
-| `address`    | `string`   | no | IP address to set on the wireless interface. Defaults to 192.168.2.1                                             |
-| `channel`    | `integer`  | no | WiFi channel to use for the network (1-14). Defaults to `11`.                                                    |
-| `country`    | `string`   | no | Country-code to apply frequencies limitations for. Defaults to `FR`                                              |
-| `hide`       | `boolean`  | no | Hide SSID (Clients must know and enter its name to connect)                                                      |
-| `interface`  | `string`   | no | Interface to configure AP for. Defaults to `wlan0`                                                               |
-| `dhcp-range` | `string`   | no | IP range for AP clients. `start,end,subnet,ttl` format. Default: `.100-.240` from address                        |
-| `network`    | `[string]` | no | Network to advertise DHCP on. Defaults to `.0/24` from address                                                   |
-| `nodhcp-interfaces` | `[string]` | no | Interfaces where the DHCP server will not run |
-| `dns`        | `[string]` | no | DNS to set via DHCP when working as Internet gateway. Defaults to `8.8.8.8`, `1.1.1.1`                           |
-| `as-gateway` | `boolean`  | no | Make this device act as a gateway to Internet (wired) for AP (wireless) clients (when/if `eth0` has connectivity)|
-| `tld`        | `string`   | no | Search (top-level) *domain* to set via DHCP. Defaults to `offspot`                                               |
-| `domain`     | `string`   | no | Domain name to direct to the offspot. Defaults to `generic` (resolved as `generic.{tld}`                         |
-| `welcome`    | `string`   | no | Additional domain to direct to offspot. Defaults to `goto.kiwix` (resolved as `goto.generic.{tld}`               |
-| `spoof`      | `boolean`* | no | Whether to direct all DNS requests to the offspot. Useful for captive-portal without Internet bridge. Special value `auto` triggers it when the hotspot is offline and disables it when it is connected to Internet    |
+| Member              | Kind       | Required | Function                                                                                                         |
+|---------------------|----------- |----------|------------------------------------------------------------------------------------------------------------------|
+| `ssid    `          | `string`   | **yes**  | SSID (Network Name)                                                                                              |
+| `passphrase`        | `string`   | no       | Passphrase/password to connect to the network. Defaults to Open Network                                          |
+| `address`           | `string`   | no       | IP address to set on the wireless interface. Defaults to 192.168.2.1                                             |
+| `channel`           | `integer`  | no       | WiFi channel to use for the network (1-14). Defaults to `11`.                                                    |
+| `country`           | `string`   | no       | Country-code to apply frequencies limitations for. Defaults to `FR`                                              |
+| `hide`              | `boolean`  | no       | Hide SSID (Clients must know and enter its name to connect)                                                      |
+| `interface`         | `string`   | no       | Interface to configure AP for. Defaults to `wlan0`                                                               |
+| `dhcp-range`        | `string`   | no       | IP range for AP clients. `start,end,subnet,ttl` format. Default: `.100-.240` from address                        |
+| `network`           | `[string]` | no       | Network to advertise DHCP on. Defaults to `.0/24` from address                                                   |
+| `nodhcp-interfaces` | `[string]` | no       | Interfaces where the DHCP server will not run                                                                    |
+| `dns`               | `[string]` | no       | DNS to set via DHCP when working as Internet gateway. Defaults to `8.8.8.8`, `1.1.1.1`                           |
+| `captured-address`  | `string`   | no       | IP address to set DNS fallback to when offline (all domains but locals are sent to it). Default:  `198.51.100.1` |
+| `as-gateway`        | `boolean`  | no       | Make this device act as a gateway to Internet (wired) for AP (wireless) clients (when/if `eth0` has connectivity)|
+| `tld`               | `string`   | no       | Search (top-level) *domain* to set via DHCP. Defaults to `offspot`                                               |
+| `domain`            | `string`   | no       | Domain name to direct to the offspot. Defaults to `generic` (resolved as `generic.{tld}`                         |
+| `welcome`           | `string`   | no       | Additional domain to direct to offspot. Defaults to `goto.kiwix` (resolved as `goto.generic.{tld}`               |
+| `spoof`             | `boolean`* | no       | Whether to direct all DNS requests to the offspot. Useful for captive-portal without Internet bridge^1.          |
+
+- ^1: Special value `auto` triggers it when the hotspot is offline and disables it when it is connected to Internet
 
 #### notes
 
 - `iptables` is not persistent. `ap` will write rules to `/etc/iptables/*.rules`. If you don't use `offspot-runtime-config-fromfile` on start, manually reload them via a script or service:
 
 ```sh
 /usr/bin/find /etc/iptables/ -name '*.rules' -exec /sbin/iptables-restore {} \;
```

### Comparing `offspot_config-1.8.2/pyproject.toml` & `offspot_config-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `offspot_config-1.8.2/PKG-INFO` & `offspot_config-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offspot-config
-Version: 1.8.2
+Version: 1.9.0
 Summary: Offspot Config helpers
 Project-URL: Homepage, https://github.com/offspot/offspot-config
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Author-email: Kiwix <dev@kiwix.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offspot
@@ -204,32 +204,35 @@
 
 Without an *armor*, configuration is appended at end of file, specifying `eth0` interface if missing (untouched `dhcpcd.conf`)
 
 ### `ap`
 
 `ap` is itself an `object`.
 
-| Member       | Kind       | Required | Function   |
-|--------------|----------- |----------|------------|
-| `ssid    `   | `string`   | **yes**  | SSID (Network Name)                                                                                        |
-| `passphrase` | `string`   | no | Passphrase/password to connect to the network. Defaults to Open Network                                          |
-| `address`    | `string`   | no | IP address to set on the wireless interface. Defaults to 192.168.2.1                                             |
-| `channel`    | `integer`  | no | WiFi channel to use for the network (1-14). Defaults to `11`.                                                    |
-| `country`    | `string`   | no | Country-code to apply frequencies limitations for. Defaults to `FR`                                              |
-| `hide`       | `boolean`  | no | Hide SSID (Clients must know and enter its name to connect)                                                      |
-| `interface`  | `string`   | no | Interface to configure AP for. Defaults to `wlan0`                                                               |
-| `dhcp-range` | `string`   | no | IP range for AP clients. `start,end,subnet,ttl` format. Default: `.100-.240` from address                        |
-| `network`    | `[string]` | no | Network to advertise DHCP on. Defaults to `.0/24` from address                                                   |
-| `nodhcp-interfaces` | `[string]` | no | Interfaces where the DHCP server will not run |
-| `dns`        | `[string]` | no | DNS to set via DHCP when working as Internet gateway. Defaults to `8.8.8.8`, `1.1.1.1`                           |
-| `as-gateway` | `boolean`  | no | Make this device act as a gateway to Internet (wired) for AP (wireless) clients (when/if `eth0` has connectivity)|
-| `tld`        | `string`   | no | Search (top-level) *domain* to set via DHCP. Defaults to `offspot`                                               |
-| `domain`     | `string`   | no | Domain name to direct to the offspot. Defaults to `generic` (resolved as `generic.{tld}`                         |
-| `welcome`    | `string`   | no | Additional domain to direct to offspot. Defaults to `goto.kiwix` (resolved as `goto.generic.{tld}`               |
-| `spoof`      | `boolean`* | no | Whether to direct all DNS requests to the offspot. Useful for captive-portal without Internet bridge. Special value `auto` triggers it when the hotspot is offline and disables it when it is connected to Internet    |
+| Member              | Kind       | Required | Function                                                                                                         |
+|---------------------|----------- |----------|------------------------------------------------------------------------------------------------------------------|
+| `ssid    `          | `string`   | **yes**  | SSID (Network Name)                                                                                              |
+| `passphrase`        | `string`   | no       | Passphrase/password to connect to the network. Defaults to Open Network                                          |
+| `address`           | `string`   | no       | IP address to set on the wireless interface. Defaults to 192.168.2.1                                             |
+| `channel`           | `integer`  | no       | WiFi channel to use for the network (1-14). Defaults to `11`.                                                    |
+| `country`           | `string`   | no       | Country-code to apply frequencies limitations for. Defaults to `FR`                                              |
+| `hide`              | `boolean`  | no       | Hide SSID (Clients must know and enter its name to connect)                                                      |
+| `interface`         | `string`   | no       | Interface to configure AP for. Defaults to `wlan0`                                                               |
+| `dhcp-range`        | `string`   | no       | IP range for AP clients. `start,end,subnet,ttl` format. Default: `.100-.240` from address                        |
+| `network`           | `[string]` | no       | Network to advertise DHCP on. Defaults to `.0/24` from address                                                   |
+| `nodhcp-interfaces` | `[string]` | no       | Interfaces where the DHCP server will not run                                                                    |
+| `dns`               | `[string]` | no       | DNS to set via DHCP when working as Internet gateway. Defaults to `8.8.8.8`, `1.1.1.1`                           |
+| `captured-address`  | `string`   | no       | IP address to set DNS fallback to when offline (all domains but locals are sent to it). Default:  `198.51.100.1` |
+| `as-gateway`        | `boolean`  | no       | Make this device act as a gateway to Internet (wired) for AP (wireless) clients (when/if `eth0` has connectivity)|
+| `tld`               | `string`   | no       | Search (top-level) *domain* to set via DHCP. Defaults to `offspot`                                               |
+| `domain`            | `string`   | no       | Domain name to direct to the offspot. Defaults to `generic` (resolved as `generic.{tld}`                         |
+| `welcome`           | `string`   | no       | Additional domain to direct to offspot. Defaults to `goto.kiwix` (resolved as `goto.generic.{tld}`               |
+| `spoof`             | `boolean`* | no       | Whether to direct all DNS requests to the offspot. Useful for captive-portal without Internet bridge^1.          |
+
+- ^1: Special value `auto` triggers it when the hotspot is offline and disables it when it is connected to Internet
 
 #### notes
 
 - `iptables` is not persistent. `ap` will write rules to `/etc/iptables/*.rules`. If you don't use `offspot-runtime-config-fromfile` on start, manually reload them via a script or service:
 
 ```sh
 /usr/bin/find /etc/iptables/ -name '*.rules' -exec /sbin/iptables-restore {} \;
```

