# Comparing `tmp/newscleaner-0.1.5.tar.gz` & `tmp/newscleaner-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscleaner-0.1.5.tar", last modified: Tue Mar 19 11:23:34 2024, max compression
+gzip compressed data, was "newscleaner-0.1.6.tar", last modified: Mon Apr  1 10:44:33 2024, max compression
```

## Comparing `newscleaner-0.1.5.tar` & `newscleaner-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 11:23:34.697114 newscleaner-0.1.5/
--rw-rw-rw-   0        0        0     1073 2023-05-10 10:09:49.000000 newscleaner-0.1.5/LICENCE.txt
--rw-rw-rw-   0        0        0       34 2023-05-10 10:10:08.000000 newscleaner-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2024-03-19 11:23:34.695975 newscleaner-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-29 11:40:52.000000 newscleaner-0.1.5/README.md
--rw-rw-rw-   0        0        0       84 2023-05-10 10:10:18.000000 newscleaner-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 11:23:34.697975 newscleaner-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      882 2024-03-19 11:22:04.000000 newscleaner-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:23:34.677951 newscleaner-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-19 11:23:34.688013 newscleaner-0.1.5/src/newscleaner/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:44.000000 newscleaner-0.1.5/src/newscleaner/__init__.py
--rw-rw-rw-   0        0        0    88392 2024-03-19 11:22:46.000000 newscleaner-0.1.5/src/newscleaner/cleaner.py
--rw-rw-rw-   0        0        0      885 2024-03-19 11:22:29.000000 newscleaner-0.1.5/src/newscleaner/setup.py
--rw-rw-rw-   0        0        0      841 2023-12-05 12:10:24.000000 newscleaner-0.1.5/src/newscleaner/strip_clean.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:23:34.695975 newscleaner-0.1.5/src/newscleaner.egg-info/
--rw-rw-rw-   0        0        0      559 2024-03-19 11:23:34.000000 newscleaner-0.1.5/src/newscleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-10 10:01:43.000000 newscleaner-0.1.5/src/newscleaner.egg-info/PKG-INFO.txt
--rw-rw-rw-   0        0        0      362 2024-03-19 11:23:34.000000 newscleaner-0.1.5/src/newscleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 11:23:34.000000 newscleaner-0.1.5/src/newscleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-19 11:23:34.000000 newscleaner-0.1.5/src/newscleaner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.874589 newscleaner-0.1.6/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 10:09:49.000000 newscleaner-0.1.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       34 2023-05-10 10:10:08.000000 newscleaner-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2024-04-01 10:44:33.873571 newscleaner-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-29 11:40:52.000000 newscleaner-0.1.6/README.md
+-rw-rw-rw-   0        0        0       84 2023-05-10 10:10:18.000000 newscleaner-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 10:44:33.874589 newscleaner-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      882 2024-04-01 10:41:36.000000 newscleaner-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.863584 newscleaner-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.869574 newscleaner-0.1.6/src/newscleaner/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:44.000000 newscleaner-0.1.6/src/newscleaner/__init__.py
+-rw-rw-rw-   0        0        0   110920 2024-04-01 10:30:06.000000 newscleaner-0.1.6/src/newscleaner/cleaner.py
+-rw-rw-rw-   0        0        0      885 2024-04-01 10:42:20.000000 newscleaner-0.1.6/src/newscleaner/setup.py
+-rw-rw-rw-   0        0        0      841 2023-12-05 12:10:24.000000 newscleaner-0.1.6/src/newscleaner/strip_clean.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.873571 newscleaner-0.1.6/src/newscleaner.egg-info/
+-rw-rw-rw-   0        0        0      559 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-10 10:01:43.000000 newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO.txt
+-rw-rw-rw-   0        0        0      362 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/top_level.txt
```

### Comparing `newscleaner-0.1.5/LICENCE.txt` & `newscleaner-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `newscleaner-0.1.5/PKG-INFO` & `newscleaner-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newscleaner
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package to clean up noise from news articles
 Home-page: https://github.com/pankajjha/newscleaner
 Author: Lakshita Kain
 Author-email: mail@pankajjha.me
 Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newscleaner-0.1.5/setup.py` & `newscleaner-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="newscleaner",
-    version="0.1.5",
+    version="0.1.6",
     author="Lakshita Kain",
     author_email="mail@pankajjha.me",
     description="Package to clean up noise from news articles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pankajjha/newscleaner",
     project_urls={
```

### Comparing `newscleaner-0.1.5/src/newscleaner/cleaner.py` & `newscleaner-0.1.6/src/newscleaner/cleaner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # coding: utf-8
-#cleaner function 0.1.5
+#cleaner function 0.1.6
 
 
 # importing all the important libraries
 import re
 import json
 import html
 import unicodedata
@@ -674,19 +674,14 @@
     clean_text =re.sub('{p}The FOX 5 Storm Team will continue to keep you up to date on the latest changes. Watch the most current forecast on FOX 5 Atlanta, streaming on FOX5Atlanta.com and on FOX Local for your Smart TV.&#160;{/p}','',clean_text, flags=re.DOTALL)
     clean_text =re.sub('{strong}&#160;AND FOLLOWING&#160;{/strong}','', clean_text, flags=re.DOTALL)
     clean_text =re.sub('{p}{strong}We will continue to follow the latest on this breaking news story. Stay tuned to FOX 26 and FOX26Houston.com for the very latest.{/strong}{/p}','', clean_text, flags=re.DOTALL)
     clean_text =re.sub('{p}Image 1 of 7{/p}','', clean_text, flags=re.DOTALL)
     clean_text =re.sub('{p}Image 1 of 25{/p}','', clean_text, flags=re.DOTALL)
 
 
-
-    # display(clean_text)
-#########################################################
-
-
     # For fox5sandiego.com
     clean_text = re.sub(r'The Associated Press contributed to this report.', '', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'\{p\}\(ProVideo contributed to this report.\)\{/p\}', '', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'{p}Updated.*?(?:[aApP]\.?[mM]\.?|AM|PM)\s*ET{/p}', '', clean_text, flags=re.DOTALL)
 
     # For fox7austin.com (continues.....)
     clean_text = re.sub(r'{p}Image \d+ of \d+{/p}  &#9660;{/p}{p}[^{]*{/p}', '', clean_text, flags=re.DOTALL)
@@ -916,15 +911,251 @@
     clean_text = re.sub(r'{p} making a tax-deductible gift {/p}','', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'{p} making a tax-deductible gift today. {/p}','', clean_text, flags=re.DOTALL)
 
     # For click2houston (continue.....)
     clean_text = re.sub(r'} Recommended Videos{','}{', clean_text, flags=re.DOTALL)
 
 
+    ########################################################################################
+    # For everythinglubbock.com (continues.....) 
+    clean_text = re.sub(r"{p}Note: The video above reflects top headlines from the morning of (January|February|March|April|May|June|July|August|September|October|November|December) \d+, \d+.{/p}",'', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}If you or someone you know would like to give to the Hill family during this time, click  here.  {/p}','', clean_text, flags=re.DOTALL)
+
+    # For kcbd.com
+    clean_text = re.sub(r'{i}{b}PREVIOUS COVERAGE: {/b}{/i}{i}{b}.*?{/b}{/i}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Specific information about the closures can be received through LBKAlert. The public can sign up for LBKAlert at  www.lbkalert.com  and register for the &#8216;Road Closure&#8217; alerts.{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}For more information{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Full story here:  {b}.*?{/b}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Read more here:  {b}.*?{/b}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'For more news, local and national, stick with KCBD on its free app and website; just look in the&#160; News &#160;section.', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} As always, be sure to join&#160; (\w+) (\w+) ,&#160; (\w+) (\w+) &#160;and&#160; (\w+) (\w+) &#160;for your top headlines. Download the free KCBD NewsChannel 11 app, like us on Facebook and follow us on Twitter.{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{b}Read the latest details on the wildfires here. {/b}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{b}PREVIOUS STORY: {/b}{b}.*?{/b}', '', clean_text, flags=re.DOTALL)
+
+    # For fox56.com
+    clean_text = re.sub(r'{strong}RELATED \| {/strong}', '', clean_text, flags = re.DOTALL)
+    clean_text = re.sub(r'{li}{strong}RELATED I {/strong}{/li}', '', clean_text, flags = re.DOTALL)
+
+    # For pagesix.com (continue.....)
+    clean_text = re.sub(r'}\n \n\t\t\t\t\tWant more celebrity and pop culture news\?\t\t\t\t{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\n\n\n\n\n\n \n\s*\n \n\nEnter your email address\n\n\n \n \n\n\t\t\t\t\t\t\tPlease provide a valid email address.\t\t\t\t\t\t\n{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n\t\t\t\t\tWant celebrity news as it breaks\? Hooked on Housewives\?\t\t\t\t{', '}{', clean_text, flags=re.DOTALL)
+
+    # For foxnews.com (continue.....)
+    clean_text = re.sub(r'Plus special access to select articles and other premium content with your account - free of charge.', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Join Fox News for access to this content', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Please enter a valid email address.', '', clean_text, flags=re.DOTALL)
+
+    # For keranews.org
+    clean_text = re.sub(r'{p}This  article  first appeared on  Fort Worth Report  and is republished here under a Creative Commons license.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}The News{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p} making a tax-deductible gift {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p} making a tax-deductible gift today. {/p}','', clean_text, flags=re.DOTALL)
+
+    # For click2houston (continue.....)
+    clean_text = re.sub(r'} Recommended Videos{','}{', clean_text, flags=re.DOTALL)
+
+    # For clearwatertimes.com
+    clean_text = re.sub(r'{p}{strong}READ ALSO:.*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p} VIDEO:.*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}&#8226; RELATED:.*? {/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}TO WATCH {/strong} .*?{/p}','', clean_text, flags=re.DOTALL)
+
+    # For digitaltrends.com
+    clean_text = re.sub(r'}\s*Recommended Videos\s*{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*Editors\' Recommendations{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*Get your weekly teardown of the tech behind PC gaming{/strong}\s*ReSpec\s*{/p}\s*Check your inbox!\t{','}{', clean_text, flags=re.DOTALL)
+
+    # For dailyfetched.com
+    clean_text = re.sub(r'{p}{strong}READ:.*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong} READ MORE:.*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For sfist.com
+    clean_text = re.sub(r'{p}{strong}RELATED:{/strong} .*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Related:{/strong} .*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Related: {/strong} .*? {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Previously:{/strong} .*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Previously: {/strong} .*?{/p}','', clean_text, flags=re.DOTALL)
+
+    # For tampafp.com
+    clean_text = re.sub(r'{p}{strong}Read: .*? {/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}{strong}Help&#160; support &#160;the Tampa Free Press by making&#160; any small donation by clicking here .{/strong}{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Android Users,&#160;Click&#160;To&#160; Download The Tampa Free Press App &#160;And Never Miss A Story. Follow Us On&#160; Facebook &#160;and&#160; Twitter .&#160;&#160; free newsletter .{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Share This:{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Read:.*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For thebaltimorebanner.com
+    clean_text = re.sub(r'{p}The Baltimore Banner thanks its sponsors. Become one.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} The Baltimore Banner thanks its sponsors.   Become one. {','}{', clean_text, flags=re.DOTALL)
+
+    # For slaynews.com
+    clean_text = re.sub(r'{strong} READ MORE:.*?{/strong}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong} READ MORE.*?{/strong}','', clean_text, flags=re.DOTALL)
+
+    # For news5cleveland.com
+    clean_text = re.sub(r'{p}News 5 will follow through on this developing story.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*We Follow Through{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Want us to continue to follow through on a story\? Let us know.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\s*\n\s*\n\s*\n\s*\n\s*First Name\n\s*\n{/p}\n\n\s*Last Name\n\s*\n{/p}\n\n\s*Email\n\s*\n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\n\s*What story do you want us to follow through on\? What questions do you have\?\n\s*\n{/p}\n\n\s*Please include the headline and/or URL of the story you want us to follow through on.\n\s*\n{/p}\n\n\s* Provide any other information that may help us to follow through on the story\n\s*\n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*Captcha\s*{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{b}RELATED:{/b}.*? {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{b}RELATED: {/b}.*? {/p}','', clean_text, flags=re.DOTALL)
+
+    # For lancasteronline.com
+    clean_text = re.sub(r'{h3}\s*Newsletter\s*{/h3}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}\s*{strong}Success!{/strong} An email has been sent to {strong}{/strong} with a link to confirm list signup.\s*{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*{strong}Error!{/strong} There was an error processing your request.\s*{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h4}\s*What to Read Next\s*{/h4}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*{{hammer}}{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*{{kicker}}{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*{{title}}\s*{/span}{{subhead}}{','}{', clean_text, flags=re.DOTALL)
+
+    # For newsantaana.com
+    clean_text = re.sub(r'} Share this:{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s* Post navigation{','}{', clean_text, flags=re.DOTALL)
+
+    # For variety.com
+    clean_text = re.sub(r'}\s*See a teaser video for the new studio below.{/','}{', clean_text, flags=re.DOTALL)
+
+    # For ew.com
+    clean_text = re.sub(r'Sign up for&#160; Entertainment Weekly  \'s&#160;free daily newsletter &#160;to get breaking TV news, exclusive first looks, recaps, reviews, interviews with your favorite stars, and more.','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Related content:','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\'s free daily newsletter  to get breaking TV news, exclusive first looks, recaps, reviews, interviews with your favorite stars, and more.','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Sign up for&#160; Entertainment Weekly\'s&#160;free daily newsletter &#160;to get breaking TV news, exclusive first looks, recaps, reviews, interviews with your favorite stars, and more.','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} \n \n{strong}Related content: {/strong}\n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}Want more movie news? Sign up for&#160; Entertainment Weekly\'s  &#160;free newsletter &#160;to get the latest trailers, celebrity interviews, film reviews, and more.{/strong}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}\'s free daily newsletter  to get breaking TV news, exclusive first looks, recaps, reviews, interviews with your favorite stars, and more.{/strong}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}Related content{/strong}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}Check out more from EW\'s&#160; The Awardist , featuring exclusive interviews, analysis, and&#160; our podcast &#160;diving into all the highlights from the year\'s best films, TV, and music.{/strong}','', clean_text, flags=re.DOTALL)
+
+    # For fredericksburg.com
+    clean_text = re.sub(r'}\s*Your notification has been saved.\s*There was a problem saving your notification.\s*{{description}}{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Followed notifications{','}{', clean_text, flags=re.DOTALL)
+
+    # For cumberlink.com
+    clean_text = re.sub(r'\n alert','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}  top story{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Email him at   and follow him on Twitter at:','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Love{/span}\n\n\n \n0\n\n\n\n Funny{/span}\n\n\n \n0\n\n\n\n Wow{/span}\n\n\n \n0\n\n\n\n Sad{/span}\n\n\n \n0\n\n\n\n Angry{/span}\n\n\n \n0','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Get in the game with our Prep Sports Newsletter','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'You can contact him at   and follow him on Twitter at:','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Sports Reporter{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Sports Editor{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*Catch the latest in Opinion{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\n 0{/p}\n Funny{/p}\n {/p}\n 0{/p}\n Wow{/p}\n {/p}\n 0{/p}\n Sad{/p}\n {/p}\n 0{/p}\n Angry{/p}\n {/p}\n 0','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Love{/span}\n\n\n \n0\n\n\n\n Funny{/span}\n\n\n \n0\n\n\n\n Wow{/span}\n\n\n \n0\n\n\n\n Sad{/span}\n\n\n \n0\n\n\n\n Angry','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'You can contact her at   and follow her on Twitter at:','', clean_text, flags=re.DOTALL)
+
+    # For csmonitor.com
+    clean_text = re.sub(r'}\n Get stories that  {strong}empower and uplift{/strong} daily.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}By signing up, you agree to our  Privacy Policy  {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\n Already a subscriber\?  Log in to hide ads .','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{span}Subscribe to insightful journalism{/span}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For buckrail.com
+    clean_text = re.sub(r'}\n \n Related Posts{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\n Related Posts','', clean_text, flags=re.DOTALL)
+
+    # For greensboro.com
+    clean_text = re.sub(r'Be the first to know','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}  editor\'s pick{','}{', clean_text, flags=re.DOTALL)
+
+
+    # For whdh.com
+    clean_text = re.sub(r'{p}\(Copyright \(c\) \d+ Sunbeam Television. All Rights Reserved. This material may not be published, broadcast, rewritten, or redistributed.\){/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Join our Newsletter for the latest news right to your inbox{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}\(Copyright \(c\) \d+ The Associated Press. All Rights Reserved. This material may not be published, broadcast, rewritten, or redistributed.\){/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}This is a developing news story; stay with 7NEWS on-air and online for the latest details.{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Join our Newsletter for the latest news right to your inbox{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}\(Copyright \(c\) \d+ CNN. All Rights Reserved. This material may not be published, broadcast, rewritten, or redistributed.\){/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Email address','', clean_text, flags=re.DOTALL)
+
+
+    # For eater.com
+    clean_text = re.sub(r'Filed under:','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{span}Eater at Home{/span}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Share this story{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n{li}\n \n Share{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n All sharing options{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n All sharing options for:{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n The freshest news from the food world every day{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"}\n      's newsletter\n    {",'}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Check your inbox for a welcome email.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Oops. Something went wrong. Please enter a valid email and try again.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Email  \(required\){/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}Update: \d{1,2}/\d{1,2}/\d{4}:\{/strong}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n      Dining In With Eater at Home\n    {/h3}\n Highlighting the people, products, and trends inspiring how we cook now{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*newsletter\s*{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Read More \n  {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Eater maps are curated by editors and aim to reflect a diversity of neighborhoods, cuisines, and prices.  Learn more about our editorial process.  {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n    \n       The freshest news from the food world every day{','}{', clean_text, flags=re.DOTALL)
+
+    # For kfoxtv.com
+    clean_text = re.sub(r'{p}{strong}Get reports like this and all the news of the day in Middle Tennessee delivered to your inbox each morning with the {/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p} to receive the topmost interesting stories from in and around our community once a day in your inbox.{/p}','', clean_text, flags=re.DOTALL)
+
+    # For vox.com
+    clean_text = re.sub(r'}\n \n \n \n Share this on Reddit{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n Share{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\s*Next Up In\s*{span}{/span} \n{/h2}\n \n\nvox-mark\n \n \n\n{/span}{/span}\n      Today, Explained\n    {/h2}\n Understand the world with a daily explainer plus the most compelling stories of the day.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{span}Email  \(required\){/strong}{/span}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'By submitting your email, you agree to our  Terms  and  Privacy Notice . You can opt out at any time. This site is protected by reCAPTCHA and the Google  Privacy Policy  and  Terms of Service  apply.\n      For more newsletters, check out our  newsletters page .','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Next Up In\n    \n         {span}.*?{/span}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n A version of this story was published in the Vox Technology newsletter.  {strong}Sign up here{/strong}  so you don’t miss the next one!{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n This story appeared originally in  {strong}Today, Explained{/strong} , Vox’s flagship daily newsletter.  {strong}Sign up here for future editions{/strong}{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n\nvox-mark\n \n \n\n{/span}{/span}\n      Today, Explained\n    {/h2}\n Understand the world with a daily explainer plus the most compelling stories of the day.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n {strong}Further reading:{/strong}  .*?{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n {strong}Further reading: {/strong} .*?{','}{', clean_text, flags=re.DOTALL)
+
+
+    # For northcentralpa.com
+    clean_text = re.sub(r'}\n Get Our Free Newsletters {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Never miss a headline with NorthcentralPa.com newsletters.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p} Sign Up Today!{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Morning Headlines:\xa0Would you like to receive our daily morning newsletter\?\xa0{strong}{/strong}{/h4}\n Afternoon Update:\xa0What\'s happening today\? Here\'s your update!{/h4}\n Daily Obits:\xa0Get a daily list straight to your email inbox.\n\xa0{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Keep your news local{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Access to independent, local news is important, do you agree\? {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}We work hard to deliver timely, relevant news, for free. 100% of your contribution to NorthcentralPa.com goes directly to helping us cover news and events in the region.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Thank you for saying that local news matters!{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Keep your news local{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}This article is republished from    under a Creative Commons license. Read the  original article .{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}\n{strong}Success!{/strong} An email has been sent to   with a link to confirm list signup.\n            {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"}\n Morning Headlines:\xa0Would you like to receive our daily morning newsletter\?\xa0{/h4}\n Afternoon Update:\xa0What's happening today\? Here's your update!{/h4}\n Daily Obits:\xa0Get a daily list straight to your email inbox.\n\xa0{",'', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Afternoon Update{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"{p}What's happening today\? Here's your update!{/p}",'', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Get a daily list straight to your email inbox.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Get the latest Job listings in your email! {strong}Sign up today!{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Get a weekly list of events happening in North Central Pa.!{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Sign Up to be eligible for our weekly Giveaways!{/p}','', clean_text, flags=re.DOTALL)
+
+    # For krocnews.com
+    clean_text = re.sub(r'Get our free mobile app','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}Google loading...{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}Minnesota News{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h2}See Also:  .*?{/h2}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h3}More  Minnesota News :{/h3}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}For the latest forecast, weather-related announcements and real-time road conditions download the free  KROC News App .{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} More  Minnesota News :{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}See Also:  .*?{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}See Also:.*?{','}{', clean_text, flags=re.DOTALL)
+
+    # For fox17online.com
+    clean_text = re.sub(r'}For more scores, highlights, and the latest news on high school sports in West Michigan, go to the   FOX 17 Blitz page{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{b}READ MORE: {/b} .*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}  Facebook  -  X \(formerly Twitter\)  -  Instagram  -  YouTube {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{b}READ MORE:{/b}  .*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}MORE:.*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For cinemablend.com
+    clean_text = re.sub('} Your Daily Blend of Entertainment News{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub('Contact me with news and offers from other Future brands Receive email from us on behalf of our trusted partners or sponsors','', clean_text, flags=re.DOTALL)
+
 
+    
     # display(clean_text)
 
 
     clean_text = re.sub('(\\n)','',clean_text) #removing new line character
     clean_text = re.sub('(\\t)','',clean_text) #removing tabular character
     clean_text = re.sub('(\\r)','',clean_text) #removing carriage return character
     clean_text = re.sub('({p}{br}{/p})','',clean_text) # removing line break
```

### Comparing `newscleaner-0.1.5/src/newscleaner/setup.py` & `newscleaner-0.1.6/src/newscleaner/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="newscleaner",
-    version="0.1.5",
+    version="0.1.6",
     author="Lakshita Kain",
     author_email="mail@pankajjha.me",
     description="Package to clean up waste postfix from articles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pankajjha/newscleaner",
     project_urls={
```

### Comparing `newscleaner-0.1.5/src/newscleaner/strip_clean.py` & `newscleaner-0.1.6/src/newscleaner/strip_clean.py`

 * *Files identical despite different names*

### Comparing `newscleaner-0.1.5/src/newscleaner.egg-info/PKG-INFO` & `newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newscleaner
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package to clean up noise from news articles
 Home-page: https://github.com/pankajjha/newscleaner
 Author: Lakshita Kain
 Author-email: mail@pankajjha.me
 Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newscleaner-0.1.5/src/newscleaner.egg-info/PKG-INFO.txt` & `newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO.txt`

 * *Files identical despite different names*

