# Comparing `tmp/bbot-1.1.7.6rc0.tar.gz` & `tmp/bbot-1.1.7.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.7.6rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.7.7rc0.tar", max compression
```

## Comparing `bbot-1.1.7.6rc0.tar` & `bbot-1.1.7.7rc0.tar`

### file list

```diff
@@ -1,339 +1,339 @@
--rw-r--r--   0        0        0    32473 2024-03-23 12:14:17.703638 bbot-1.1.7.6rc0/LICENSE
--rw-r--r--   0        0        0    37712 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/README.md
--rw-r--r--   0        0        0      208 2024-03-23 12:14:37.435553 bbot-1.1.7.6rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7898 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    17601 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/cli.py
--rw-r--r--   0        0        0       59 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3588 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9843 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5182 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1341 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      617 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/errors.py
--rw-r--r--   0        0        0       91 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    45979 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1656 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1183 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       86 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3583 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     1537 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     4341 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/cloud.py
--rw-r--r--   0        0        0    10930 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14117 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9199 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    47786 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     5639 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     6354 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0    12632 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    82517 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    22071 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0    10041 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0     1990 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     3463 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     5947 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     8781 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    31592 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    19801 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0      191 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8118 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2024-03-23 12:14:17.707638 bbot-1.1.7.6rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4148 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     2328 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/ajaxpro.py
--rw-r--r--   0        0        0     1824 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1372 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     4691 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     4150 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/baddns.py
--rw-r--r--   0        0        0     1245 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/baddns_zone.py
--rw-r--r--   0        0        0     3549 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    59062 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2352 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1299 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0      655 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bucket_amazon.py
--rw-r--r--   0        0        0     1020 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      775 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1915 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bucket_file_enum.py
--rw-r--r--   0        0        0     1352 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2540 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bucket_google.py
--rw-r--r--   0        0        0     4911 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     6553 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1188 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3371 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      798 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     1522 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/chaos.py
--rw-r--r--   0        0        0      735 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     3297 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/credshed.py
--rw-r--r--   0        0        0      376 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1230 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0     5220 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/deadly/dastardly.py
--rw-r--r--   0        0        0    14079 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    17188 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5239 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     3928 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/dehashed.py
--rw-r--r--   0        0        0      930 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/digitorus.py
--rw-r--r--   0        0        0     5324 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     3186 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     3247 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/dockerhub.py
--rw-r--r--   0        0        0     9245 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/dotnetnuke.py
--rw-r--r--   0        0        0      791 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11758 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     7502 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/filedownload.py
--rw-r--r--   0        0        0     2184 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1195 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7794 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1319 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2073 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/git_clone.py
--rw-r--r--   0        0        0     3135 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/github_codesearch.py
--rw-r--r--   0        0        0     8664 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/github_org.py
--rw-r--r--   0        0        0    11415 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      890 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7172 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     6758 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5990 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2098 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0    13124 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2024-03-23 12:14:17.711638 bbot-1.1.7.6rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    18687 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     7448 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     4384 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/internetdb.py
--rw-r--r--   0        0        0     2123 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/ip2location.py
--rw-r--r--   0        0        0     1539 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     1767 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1541 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10816 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    21031 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      857 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     2281 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/newsletters.py
--rw-r--r--   0        0        0     5506 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     4731 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5852 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      774 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    14731 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     3268 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2604 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0      531 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/discord.py
--rw-r--r--   0        0        0      985 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/emails.py
--rw-r--r--   0        0        0     2182 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1907 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1375 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1482 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     1117 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/slack.py
--rw-r--r--   0        0        0     1886 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/splunk.py
--rw-r--r--   0        0        0     1430 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/subdomains.py
--rw-r--r--   0        0        0      723 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/teams.py
--rw-r--r--   0        0        0     3627 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2218 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1689 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     9461 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1619 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1420 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0     5479 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/postman.py
--rw-r--r--   0        0        0      832 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8456 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      828 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2025 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2898 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1201 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0      792 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1993 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/sitedossier.py
--rw-r--r--   0        0        0     1478 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1408 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1769 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7822 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     1327 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/subdomaincenter.py
--rw-r--r--   0        0        0      553 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    17041 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0     5642 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/templates/bucket.py
--rw-r--r--   0        0        0     1308 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/templates/github.py
--rw-r--r--   0        0        0     2436 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/templates/portscanner.py
--rw-r--r--   0        0        0     1182 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/templates/shodan.py
--rw-r--r--   0        0        0     6100 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/templates/subdomain_enum.py
--rw-r--r--   0        0        0     3789 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/templates/webhook.py
--rw-r--r--   0        0        0      678 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     4348 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/trufflehog.py
--rw-r--r--   0        0        0     4102 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2992 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2325 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1591 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     2010 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1272 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2871 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2337 2024-03-23 12:14:17.715638 bbot-1.1.7.6rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    29339 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    41838 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3049 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0    11073 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     5889 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    12418 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     4870 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0       31 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/coverage.cfg
--rwxr-xr-x   0        0        0      652 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1091 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_output.ndjson
--rw-r--r--   0        0        0        0 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5523 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6544 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0     3808 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     5853 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     7572 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    22219 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    31826 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0    16305 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_manager_deduplication.py
--rw-r--r--   0        0        0    77598 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
--rw-r--r--   0        0        0    16717 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     2657 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     7144 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_regexes.py
--rw-r--r--   0        0        0     2884 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0    13141 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     5344 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      664 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      473 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0     2789 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
--rw-r--r--   0        0        0      546 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     3098 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     4805 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     2795 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
--rw-r--r--   0        0        0     2397 2024-03-23 12:14:17.719638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
--rw-r--r--   0        0        0     5599 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3984 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
--rw-r--r--   0        0        0      552 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      907 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0     2282 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
--rw-r--r--   0        0        0      506 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1312 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
--rw-r--r--   0        0        0     5051 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      956 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
--rw-r--r--   0        0        0      564 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0     3362 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
--rw-r--r--   0        0        0      762 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0     2321 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
--rw-r--r--   0        0        0     3432 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
--rw-r--r--   0        0        0     1613 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
--rw-r--r--   0        0        0     1863 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
--rw-r--r--   0        0        0      952 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     3907 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
--rw-r--r--   0        0        0     8232 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
--rw-r--r--   0        0        0      461 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0      944 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
--rw-r--r--   0        0        0    14423 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     2955 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0     2389 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
--rw-r--r--   0        0        0      445 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0    12266 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
--rw-r--r--   0        0        0     3682 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
--rw-r--r--   0        0        0    22783 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
--rw-r--r--   0        0        0     3487 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0     2155 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     3663 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2879 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     2231 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
--rw-r--r--   0        0        0     1123 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
--rw-r--r--   0        0        0      604 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2767 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0     1006 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0     1641 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1711 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      428 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      659 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0     2305 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
--rw-r--r--   0        0        0     3618 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1116 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     5609 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9402 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2142 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10680 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2190 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0    14768 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
--rw-r--r--   0        0        0      184 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2024-03-23 12:14:17.723638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      537 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      713 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     6220 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
--rw-r--r--   0        0        0     2321 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0      415 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
--rw-r--r--   0        0        0     2426 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0     1218 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     3121 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0     1866 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
--rw-r--r--   0        0        0      706 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0      610 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
--rw-r--r--   0        0        0     1116 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
--rw-r--r--   0        0        0      611 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     1222 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
--rw-r--r--   0        0        0     7751 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0    13270 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
--rw-r--r--   0        0        0     1144 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0     1304 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2026 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1103 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     1704 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2024-03-23 12:14:17.727638 bbot-1.1.7.6rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0      764 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/ms_on_prem_subdomains.txt
--rw-r--r--   0        0        0    32226 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2024-03-23 12:14:17.731638 bbot-1.1.7.6rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     2627 2024-03-23 12:14:37.431553 bbot-1.1.7.6rc0/pyproject.toml
--rw-r--r--   0        0        0    39756 1970-01-01 00:00:00.000000 bbot-1.1.7.6rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/LICENSE
+-rw-r--r--   0        0        0    37988 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/README.md
+-rw-r--r--   0        0        0      208 2024-03-22 20:11:21.669284 bbot-1.1.7.7rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7898 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    17601 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/cli.py
+-rw-r--r--   0        0        0       59 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3588 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9843 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5182 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1341 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      617 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0       91 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    45979 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1656 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1183 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       86 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     1537 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     4341 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/cloud.py
+-rw-r--r--   0        0        0    10930 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14117 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9199 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    47786 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     5639 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     6354 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0    12632 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    82517 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    22071 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0    10041 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1990 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     3463 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     5947 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     8781 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    31592 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    19801 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0      191 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8118 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4148 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     2328 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/ajaxpro.py
+-rw-r--r--   0        0        0     1824 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1372 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     4691 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     4150 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/baddns.py
+-rw-r--r--   0        0        0     1245 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/baddns_zone.py
+-rw-r--r--   0        0        0     3549 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    59062 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2352 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1299 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0      655 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_amazon.py
+-rw-r--r--   0        0        0     1020 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      775 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1915 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_file_enum.py
+-rw-r--r--   0        0        0     1352 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2540 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_google.py
+-rw-r--r--   0        0        0     4911 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     6553 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1188 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3371 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      798 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     1522 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/chaos.py
+-rw-r--r--   0        0        0      735 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     3297 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/credshed.py
+-rw-r--r--   0        0        0      376 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1230 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0     5220 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/dastardly.py
+-rw-r--r--   0        0        0    14079 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    17188 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5239 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     3928 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dehashed.py
+-rw-r--r--   0        0        0      930 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     5324 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     3186 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     3247 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dockerhub.py
+-rw-r--r--   0        0        0     9245 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dotnetnuke.py
+-rw-r--r--   0        0        0      791 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11758 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     7502 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/filedownload.py
+-rw-r--r--   0        0        0     2184 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1195 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7794 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1319 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2073 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/git_clone.py
+-rw-r--r--   0        0        0     3135 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/github_codesearch.py
+-rw-r--r--   0        0        0     8664 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/github_org.py
+-rw-r--r--   0        0        0    11415 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      890 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7172 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     6758 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5990 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2098 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0    13124 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    18687 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     7448 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     4384 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internetdb.py
+-rw-r--r--   0        0        0     2123 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ip2location.py
+-rw-r--r--   0        0        0     1539 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     1767 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1541 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10816 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    21031 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      857 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     2281 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/newsletters.py
+-rw-r--r--   0        0        0     5506 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4731 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5852 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      774 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    14731 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     3268 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2604 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0      531 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/discord.py
+-rw-r--r--   0        0        0      985 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/emails.py
+-rw-r--r--   0        0        0     2182 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1907 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1375 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1482 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     1117 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/slack.py
+-rw-r--r--   0        0        0     1886 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/splunk.py
+-rw-r--r--   0        0        0     1430 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/subdomains.py
+-rw-r--r--   0        0        0      723 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/teams.py
+-rw-r--r--   0        0        0     3627 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2218 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1689 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9461 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1619 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1420 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0     5479 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/postman.py
+-rw-r--r--   0        0        0      832 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8456 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      828 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2025 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2898 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1201 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0      792 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1993 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/sitedossier.py
+-rw-r--r--   0        0        0     1478 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1408 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1769 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7822 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     1327 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      553 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    17041 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0     5642 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/bucket.py
+-rw-r--r--   0        0        0     1308 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/github.py
+-rw-r--r--   0        0        0     2436 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/portscanner.py
+-rw-r--r--   0        0        0     1182 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/shodan.py
+-rw-r--r--   0        0        0     6100 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/subdomain_enum.py
+-rw-r--r--   0        0        0     3789 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/webhook.py
+-rw-r--r--   0        0        0      678 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4348 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/trufflehog.py
+-rw-r--r--   0        0        0     4102 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2992 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2325 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1591 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     2010 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1272 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2871 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2337 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    29339 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    41838 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3049 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0    11073 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     5889 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    12418 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     4870 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0       31 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/coverage.cfg
+-rwxr-xr-x   0        0        0      652 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1091 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_output.ndjson
+-rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5523 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6544 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0     3808 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     5853 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     7572 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    22219 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    31826 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0    16305 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_deduplication.py
+-rw-r--r--   0        0        0    77598 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
+-rw-r--r--   0        0        0    16717 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     2657 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     7144 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2884 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0    13141 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     5344 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      664 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      473 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0     2789 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
+-rw-r--r--   0        0        0      546 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     3098 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     4805 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     2795 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
+-rw-r--r--   0        0        0     2397 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
+-rw-r--r--   0        0        0     5599 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3984 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
+-rw-r--r--   0        0        0      552 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      907 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0     2282 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
+-rw-r--r--   0        0        0      506 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1312 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
+-rw-r--r--   0        0        0     5051 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      956 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
+-rw-r--r--   0        0        0      564 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0     3362 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
+-rw-r--r--   0        0        0      762 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     2321 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
+-rw-r--r--   0        0        0     3432 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
+-rw-r--r--   0        0        0     1613 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0     1863 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
+-rw-r--r--   0        0        0      952 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     3907 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
+-rw-r--r--   0        0        0     8232 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
+-rw-r--r--   0        0        0      461 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0      944 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
+-rw-r--r--   0        0        0    14423 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     2955 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0     2389 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
+-rw-r--r--   0        0        0      445 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0    12266 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
+-rw-r--r--   0        0        0     3682 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
+-rw-r--r--   0        0        0    22783 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
+-rw-r--r--   0        0        0     3487 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0     2155 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     3663 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2879 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     2231 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
+-rw-r--r--   0        0        0     1123 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
+-rw-r--r--   0        0        0      604 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2767 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0     1006 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0     1641 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1711 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      428 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      659 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0     2305 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
+-rw-r--r--   0        0        0     3618 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     5609 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9402 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0    14768 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
+-rw-r--r--   0        0        0      184 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      537 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      713 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     6220 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
+-rw-r--r--   0        0        0     2321 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0      415 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
+-rw-r--r--   0        0        0     2426 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0     1218 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     3121 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0     1866 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
+-rw-r--r--   0        0        0      706 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0      610 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0     1116 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
+-rw-r--r--   0        0        0      611 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     1222 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
+-rw-r--r--   0        0        0     7751 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0    13270 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
+-rw-r--r--   0        0        0     1144 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0     1304 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2026 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1103 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     1704 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0      764 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/ms_on_prem_subdomains.txt
+-rw-r--r--   0        0        0    32226 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     2627 2024-03-22 20:11:21.665284 bbot-1.1.7.7rc0/pyproject.toml
+-rw-r--r--   0        0        0    40032 1970-01-01 00:00:00.000000 bbot-1.1.7.7rc0/PKG-INFO
```

### Comparing `bbot-1.1.7.6rc0/LICENSE` & `bbot-1.1.7.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/README.md` & `bbot-1.1.7.7rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -260,37 +260,37 @@
 
 ![subdomain-stats-ebay](https://github.com/blacklanternsecurity/bbot/assets/20261699/53e07e9f-50b6-4b70-9e83-297dbfbcb436)
 
 ## BBOT Modules By Flag
 For a full list of modules, including the data types consumed and emitted by each one, see [List of Modules](https://www.blacklanternsecurity.com/bbot/modules/list_of_modules/).
 
 <!-- BBOT MODULE FLAGS -->
-| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-|------------------|-------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| safe             | 77          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
-| passive          | 57          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                         |
-| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                          |
-| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dockerhub, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                        |
-| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| slow             | 9           | May take a long time to complete                   | bucket_digitalocean, dastardly, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+|------------------|-------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| safe             | 78          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
+| passive          | 58          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                         |
+| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                                      |
+| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dockerhub, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                                    |
+| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| slow             | 9           | May take a long time to complete                   | bucket_digitalocean, dastardly, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 <!-- END BBOT MODULE FLAGS -->
 
 ## BBOT Output Modules
 BBOT can save its data to TXT, CSV, JSON, and tons of other destinations including [Neo4j](https://www.blacklanternsecurity.com/bbot/scanning/output/#neo4j), [Splunk](https://www.blacklanternsecurity.com/bbot/scanning/output/#splunk), and [Discord](https://www.blacklanternsecurity.com/bbot/scanning/output/#discord-slack-teams). For instructions on how to use these, see [Output Modules](https://www.blacklanternsecurity.com/bbot/scanning/output). 
 
 <!-- BBOT OUTPUT MODULES -->
 | Module          | Type   | Needs API Key   | Description                                                                             | Flags          | Consumed Events                                                                                  | Produced Events           |
```

### Comparing `bbot-1.1.7.6rc0/bbot/agent/agent.py` & `bbot-1.1.7.7rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/cli.py` & `bbot-1.1.7.7rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.7.7rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/configurator/args.py` & `bbot-1.1.7.7rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/configurator/environ.py` & `bbot-1.1.7.7rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/configurator/files.py` & `bbot-1.1.7.7rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/errors.py` & `bbot-1.1.7.7rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/event/base.py` & `bbot-1.1.7.7rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/event/helpers.py` & `bbot-1.1.7.7rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/flags.py` & `bbot-1.1.7.7rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/cache.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/cloud.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/command.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/diff.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/dns.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/files.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/helper.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/logger.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/misc.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/modules.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/url.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/validators.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/web.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.7.7rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/core/logger/logger.py` & `bbot-1.1.7.7rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/db/neo4j.py` & `bbot-1.1.7.7rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/defaults.yml` & `bbot-1.1.7.7rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/ajaxpro.py` & `bbot-1.1.7.7rc0/bbot/modules/ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/anubisdb.py` & `bbot-1.1.7.7rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/azure_realm.py` & `bbot-1.1.7.7rc0/bbot/modules/azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.7.7rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/baddns.py` & `bbot-1.1.7.7rc0/bbot/modules/baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/baddns_zone.py` & `bbot-1.1.7.7rc0/bbot/modules/baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/badsecrets.py` & `bbot-1.1.7.7rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/base.py` & `bbot-1.1.7.7rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bevigil.py` & `bbot-1.1.7.7rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/binaryedge.py` & `bbot-1.1.7.7rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bucket_amazon.py` & `bbot-1.1.7.7rc0/bbot/modules/bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.7.7rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.7.7rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bucket_file_enum.py` & `bbot-1.1.7.7rc0/bbot/modules/bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.7.7rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bucket_google.py` & `bbot-1.1.7.7rc0/bbot/modules/bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/builtwith.py` & `bbot-1.1.7.7rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/bypass403.py` & `bbot-1.1.7.7rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/c99.py` & `bbot-1.1.7.7rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/censys.py` & `bbot-1.1.7.7rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/certspotter.py` & `bbot-1.1.7.7rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/chaos.py` & `bbot-1.1.7.7rc0/bbot/modules/chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/columbus.py` & `bbot-1.1.7.7rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/credshed.py` & `bbot-1.1.7.7rc0/bbot/modules/credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/crt.py` & `bbot-1.1.7.7rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/deadly/dastardly.py` & `bbot-1.1.7.7rc0/bbot/modules/deadly/dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.7.7rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.7.7rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.7.7rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/dehashed.py` & `bbot-1.1.7.7rc0/bbot/modules/dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/digitorus.py` & `bbot-1.1.7.7rc0/bbot/modules/digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.7.7rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.7.7rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/dockerhub.py` & `bbot-1.1.7.7rc0/bbot/modules/dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/dotnetnuke.py` & `bbot-1.1.7.7rc0/bbot/modules/dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/emailformat.py` & `bbot-1.1.7.7rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.7.7rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/filedownload.py` & `bbot-1.1.7.7rc0/bbot/modules/filedownload.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.7.7rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/fullhunt.py` & `bbot-1.1.7.7rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.7.7rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/git.py` & `bbot-1.1.7.7rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/git_clone.py` & `bbot-1.1.7.7rc0/bbot/modules/git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/github_codesearch.py` & `bbot-1.1.7.7rc0/bbot/modules/github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/github_org.py` & `bbot-1.1.7.7rc0/bbot/modules/github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/gowitness.py` & `bbot-1.1.7.7rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/hackertarget.py` & `bbot-1.1.7.7rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/host_header.py` & `bbot-1.1.7.7rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/httpx.py` & `bbot-1.1.7.7rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/hunt.py` & `bbot-1.1.7.7rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/hunterio.py` & `bbot-1.1.7.7rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.7.7rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/internal/base.py` & `bbot-1.1.7.7rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.7.7rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.7.7rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/internetdb.py` & `bbot-1.1.7.7rc0/bbot/modules/internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/ip2location.py` & `bbot-1.1.7.7rc0/bbot/modules/ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.7.7rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/ipstack.py` & `bbot-1.1.7.7rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/leakix.py` & `bbot-1.1.7.7rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/masscan.py` & `bbot-1.1.7.7rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/massdns.py` & `bbot-1.1.7.7rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/myssl.py` & `bbot-1.1.7.7rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/newsletters.py` & `bbot-1.1.7.7rc0/bbot/modules/newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/nmap.py` & `bbot-1.1.7.7rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/ntlm.py` & `bbot-1.1.7.7rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/oauth.py` & `bbot-1.1.7.7rc0/bbot/modules/oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/otx.py` & `bbot-1.1.7.7rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.7.7rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/base.py` & `bbot-1.1.7.7rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/csv.py` & `bbot-1.1.7.7rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/discord.py` & `bbot-1.1.7.7rc0/bbot/modules/output/discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/emails.py` & `bbot-1.1.7.7rc0/bbot/modules/output/emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/http.py` & `bbot-1.1.7.7rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/human.py` & `bbot-1.1.7.7rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/json.py` & `bbot-1.1.7.7rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.7.7rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/slack.py` & `bbot-1.1.7.7rc0/bbot/modules/output/slack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/splunk.py` & `bbot-1.1.7.7rc0/bbot/modules/output/splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/subdomains.py` & `bbot-1.1.7.7rc0/bbot/modules/output/subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/teams.py` & `bbot-1.1.7.7rc0/bbot/modules/output/teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/web_report.py` & `bbot-1.1.7.7rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/output/websocket.py` & `bbot-1.1.7.7rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.7.7rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.7.7rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.7.7rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/passivetotal.py` & `bbot-1.1.7.7rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/pgp.py` & `bbot-1.1.7.7rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/postman.py` & `bbot-1.1.7.7rc0/bbot/modules/postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/rapiddns.py` & `bbot-1.1.7.7rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.7.7rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/report/asn.py` & `bbot-1.1.7.7rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/riddler.py` & `bbot-1.1.7.7rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/robots.py` & `bbot-1.1.7.7rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/secretsdb.py` & `bbot-1.1.7.7rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/securitytrails.py` & `bbot-1.1.7.7rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.7.7rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/sitedossier.py` & `bbot-1.1.7.7rc0/bbot/modules/sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/skymem.py` & `bbot-1.1.7.7rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/smuggler.py` & `bbot-1.1.7.7rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/social.py` & `bbot-1.1.7.7rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/sslcert.py` & `bbot-1.1.7.7rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/subdomaincenter.py` & `bbot-1.1.7.7rc0/bbot/modules/subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/sublist3r.py` & `bbot-1.1.7.7rc0/bbot/modules/sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/telerik.py` & `bbot-1.1.7.7rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/templates/bucket.py` & `bbot-1.1.7.7rc0/bbot/modules/templates/bucket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/templates/github.py` & `bbot-1.1.7.7rc0/bbot/modules/templates/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/templates/portscanner.py` & `bbot-1.1.7.7rc0/bbot/modules/templates/portscanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/templates/shodan.py` & `bbot-1.1.7.7rc0/bbot/modules/templates/shodan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/templates/subdomain_enum.py` & `bbot-1.1.7.7rc0/bbot/modules/templates/subdomain_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/templates/webhook.py` & `bbot-1.1.7.7rc0/bbot/modules/templates/webhook.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/threatminer.py` & `bbot-1.1.7.7rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/trufflehog.py` & `bbot-1.1.7.7rc0/bbot/modules/trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.7.7rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/urlscan.py` & `bbot-1.1.7.7rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/viewdns.py` & `bbot-1.1.7.7rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/virustotal.py` & `bbot-1.1.7.7rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/wafw00f.py` & `bbot-1.1.7.7rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.7.7rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/wayback.py` & `bbot-1.1.7.7rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/modules/zoomeye.py` & `bbot-1.1.7.7rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.7.7rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/scanner/manager.py` & `bbot-1.1.7.7rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/scanner/scanner.py` & `bbot-1.1.7.7rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/scanner/stats.py` & `bbot-1.1.7.7rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/scanner/target.py` & `bbot-1.1.7.7rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/scripts/docs.py` & `bbot-1.1.7.7rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.7.7rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/conftest.py` & `bbot-1.1.7.7rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/run_tests.sh` & `bbot-1.1.7.7rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test.conf` & `bbot-1.1.7.7rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_manager_deduplication.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_deduplication.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_regexes.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_discord.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_emails.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_json.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_postman.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_teams.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/testsslcert.pem` & `bbot-1.1.7.7rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/test/testsslkey.pem` & `bbot-1.1.7.7rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.7.7rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/ms_on_prem_subdomains.txt` & `bbot-1.1.7.7rc0/bbot/wordlists/ms_on_prem_subdomains.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.7.7rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.7.7rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.7.7rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.7.7rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.7.7rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.6rc0/pyproject.toml` & `bbot-1.1.7.7rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.7.6rc"
+version = "v1.1.7.7rc"
 description = "OSINT automation for hackers."
 authors = [
     "TheTechromancer",
     "Paul Mueller",
 ]
 license = "GPL-3.0"
 readme = "README.md"
```

### Comparing `bbot-1.1.7.6rc0/PKG-INFO` & `bbot-1.1.7.7rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.7.6rc0
+Version: 1.1.7.7rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Keywords: python,cli,automation,osint,neo4j,scanner,python-library,hacking,recursion,pentesting,recon,command-line-tool,bugbounty,subdomains,security-tools,subdomain-scanner,osint-framework,attack-surface,subdomain-enumeration,osint-tool
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -304,37 +304,37 @@
 
 ![subdomain-stats-ebay](https://github.com/blacklanternsecurity/bbot/assets/20261699/53e07e9f-50b6-4b70-9e83-297dbfbcb436)
 
 ## BBOT Modules By Flag
 For a full list of modules, including the data types consumed and emitted by each one, see [List of Modules](https://www.blacklanternsecurity.com/bbot/modules/list_of_modules/).
 
 <!-- BBOT MODULE FLAGS -->
-| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-|------------------|-------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| safe             | 77          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
-| passive          | 57          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                         |
-| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                          |
-| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dockerhub, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                        |
-| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| slow             | 9           | May take a long time to complete                   | bucket_digitalocean, dastardly, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+|------------------|-------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| safe             | 78          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
+| passive          | 58          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                         |
+| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                                      |
+| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dockerhub, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                                    |
+| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| slow             | 9           | May take a long time to complete                   | bucket_digitalocean, dastardly, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 <!-- END BBOT MODULE FLAGS -->
 
 ## BBOT Output Modules
 BBOT can save its data to TXT, CSV, JSON, and tons of other destinations including [Neo4j](https://www.blacklanternsecurity.com/bbot/scanning/output/#neo4j), [Splunk](https://www.blacklanternsecurity.com/bbot/scanning/output/#splunk), and [Discord](https://www.blacklanternsecurity.com/bbot/scanning/output/#discord-slack-teams). For instructions on how to use these, see [Output Modules](https://www.blacklanternsecurity.com/bbot/scanning/output). 
 
 <!-- BBOT OUTPUT MODULES -->
 | Module          | Type   | Needs API Key   | Description                                                                             | Flags          | Consumed Events                                                                                  | Produced Events           |
```

