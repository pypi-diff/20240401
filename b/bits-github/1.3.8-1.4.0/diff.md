# Comparing `tmp/bits-github-1.3.8.tar.gz` & `tmp/bits_github-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bits-github-1.3.8.tar", last modified: Tue Mar  1 18:39:41 2022, max compression
+gzip compressed data, was "bits_github-1.4.0.tar", max compression
```

## Comparing `bits-github-1.3.8.tar` & `bits_github-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,13 @@
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-03-01 18:39:41.000000 bits-github-1.3.8/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      229 2022-03-01 18:39:41.000000 bits-github-1.3.8/PKG-INFO
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       45 2019-06-03 15:36:26.000000 bits-github-1.3.8/README.md
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-03-01 18:39:41.000000 bits-github-1.3.8/bits/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       89 2019-09-27 03:30:25.000000 bits-github-1.3.8/bits/__init__.py
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-03-01 18:39:41.000000 bits-github-1.3.8/bits/github/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)    25644 2022-03-01 18:37:02.000000 bits-github-1.3.8/bits/github/__init__.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     1885 2019-10-12 18:10:38.000000 bits-github-1.3.8/bits/github/app.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)    13916 2019-11-15 18:05:40.000000 bits-github-1.3.8/bits/github/auditlogs.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)    17160 2022-03-01 15:47:04.000000 bits-github-1.3.8/bits/github/client.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     1931 2020-05-23 16:25:55.000000 bits-github-1.3.8/bits/github/datastore.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)    10167 2022-03-01 15:47:04.000000 bits-github-1.3.8/bits/github/firestore.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     7012 2019-10-31 12:27:32.000000 bits-github-1.3.8/bits/github/helpers.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     2775 2019-10-04 17:32:33.000000 bits-github-1.3.8/bits/github/sync.py
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)    24925 2022-03-01 18:39:29.000000 bits-github-1.3.8/bits/github/update.py
-drwxr-sr-x   0 karlsson  (1001) lukwam    (1001)        0 2022-03-01 18:39:41.000000 bits-github-1.3.8/bits_github.egg-info/
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      229 2022-03-01 18:39:40.000000 bits-github-1.3.8/bits_github.egg-info/PKG-INFO
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      458 2022-03-01 18:39:41.000000 bits-github-1.3.8/bits_github.egg-info/SOURCES.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        1 2022-03-01 18:39:40.000000 bits-github-1.3.8/bits_github.egg-info/dependency_links.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        1 2022-03-01 18:39:40.000000 bits-github-1.3.8/bits_github.egg-info/not-zip-safe
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)       16 2022-03-01 18:39:40.000000 bits-github-1.3.8/bits_github.egg-info/requires.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)        5 2022-03-01 18:39:40.000000 bits-github-1.3.8/bits_github.egg-info/top_level.txt
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)      153 2022-03-01 18:39:41.000000 bits-github-1.3.8/setup.cfg
--rw-r--r--   0 karlsson  (1001) lukwam    (1001)     1043 2022-03-01 17:45:36.000000 bits-github-1.3.8/setup.py
+-rw-r--r--   0        0        0       45 2024-04-01 17:50:32.484241 bits_github-1.4.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/__init__.py
+-rw-r--r--   0        0        0    25745 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/app.py
+-rw-r--r--   0        0        0    13646 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/auditlogs.py
+-rw-r--r--   0        0        0    16434 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/client.py
+-rw-r--r--   0        0        0     1899 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/datastore.py
+-rw-r--r--   0        0        0    10143 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/firestore.py
+-rw-r--r--   0        0        0     6904 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/helpers.py
+-rw-r--r--   0        0        0     2719 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/sync.py
+-rw-r--r--   0        0        0    24647 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/update.py
+-rw-r--r--   0        0        0     1207 2024-04-01 17:50:32.488241 bits_github-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 bits_github-1.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bits-github-1.3.8/bits/github/__init__.py` & `bits_github-1.4.0/bits/github/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# -*- coding: utf-8 -*-
 """GitHub class file."""
 
 import datetime
-import requests
-
 from urllib.parse import urlencode
 
+import requests
 
-class GitHub(object):
+
+class GitHub:
     """GitHub class."""
 
-    def __init__(
+    CODE_OK = 204
+    CODE_NOT_CHANGED = 304
+    CODE_NOT_FOUND = 404
+
+    def __init__(  # noqa: PLR0913
             self,
             token,
             org=None,
             org_id=None,
             owner_team=None,
             role_team=None,
             role_team_name=None,
@@ -52,66 +55,66 @@
         self.app_project = app_project
 
     #
     # Sub Classes
     #
     def app(self, auth=None):
         """Return an App instance."""
-        from bits.github.app import App
+        from .app import App
         return App(auth=auth, github=self)
 
     def auditlogs(self, auth=None, args=None):
         """Return an AuditLogs instance."""
-        from bits.github.auditlogs import AuditLogs
+        from .auditlogs import AuditLogs
         return AuditLogs(auth=auth, github=self, args=args)
 
     def client(self, auth=None, app_project=None):
         """Return a Client instance."""
-        from bits.github.client import Client
+        from .client import Client
         if not app_project:
             app_project = self.app_project
         return Client(auth=auth, github=self, app_project=app_project)
 
     def datastore(self, auth=None):
         """Return a Datastore instance."""
-        from bits.github.datastore import Datastore
+        from .datastore import Datastore
         return Datastore(auth=auth, github=self)
 
     def firestore(
         self,
         auth=None,
         project="broad-bitsdb-firestore",
         app_project=None,
         bitsdb_project="broad-bitsdb-prod",
     ):
         """Return a Firestore instance."""
-        from bits.github.firestore import Firestore
+        from .firestore import Firestore
         if not app_project:
             app_project = self.app_project
         return Firestore(
             auth=auth,
             github=self,
             project=project,
             app_project=app_project,
             bitsdb_project=bitsdb_project,
         )
 
     def helpers(self, auth=None):
         """Return a Firestore instance."""
-        from bits.github.helpers import Helpers
+        from .helpers import Helpers
         return Helpers(auth=auth, github=self)
 
     def sync(self, auth=None):
         """Return an Update instance."""
-        from bits.github.sync import Sync
+        from .sync import Sync
         return Sync(auth=auth, github=self)
 
     def update(self, auth=None):
         """Return an Update instance."""
-        from bits.github.update import Update
+        from .update import Update
         return Update(auth=auth, github=self)
 
     #
     # Helpers
     #
     def get(self, url, headers={}, params={}, raise_for_status=True):
         """Return a response from a GET call."""
@@ -132,15 +135,15 @@
         """Return a list as a dict with the given key."""
         data = {}
         for item in items:
             k = item[key]
             data[k] = item
         return data
 
-    def get_modified(self, url, headers={}, params={}, etag=None, last_modified=None):
+    def get_modified(self, url, headers={}, params={}, etag=None, last_modified=None):  # noqa: PLR0913
         """Return a response from a GET call if modified, otherwise return False."""
         # reset the headers from any previous requests
         headers["If-None-Match"] = None
         headers["If-Modified-Since"] = None
 
         # add etag and last-modified request headers
         if etag:
@@ -148,15 +151,15 @@
         elif last_modified:
             headers["If-Modified-Since"] = last_modified
 
         # get response
         response = self.get(url, headers=headers, params=params)
 
         # check if not changed
-        if response.status_code == 304:
+        if response.status_code == self.CODE_NOT_CHANGED:
             return False
 
         return response.json()
 
     def get_list(self, base_url, url, headers={}, params={}):
         """Return a paginated list from a GET call."""
         items_list = []
@@ -195,15 +198,15 @@
             "client_id": client_id,
             "redirect_uri": redirect_uri,
             "scopes": scopes,
             "state": state,
         }
         return f"{base_url}?{urlencode(params)}"
 
-    def get_oauth_access_token(self, client_id, client_secret, redirect_uri, code, state):
+    def get_oauth_access_token(self, client_id, client_secret, redirect_uri, code, state):  # noqa: PLR0913
         """Return an access token for a user."""
         # POST /login/oauth/access_token
         url = "https://github.com/login/oauth/access_token"
         headers = {"Accept": "application/json"}
         params = {
             "client_id": client_id,
             "client_secret": client_secret,
@@ -276,39 +279,39 @@
     def check_org_membership(self, member):
         """Return a user"s organization membership."""
         # GET /orgs/:org/members/:username
         url = f"{self.base_url}/orgs/{self.org}/members/{member}"
         response = self.get(url, raise_for_status=False).json()
 
         # requester is an organization member and user is a member
-        if response.status_code == 204:
+        if response.status_code == self.CODE_OK:
             return True
 
         # requester is an organization member and user is not a member
-        if response.status_code == 404:
+        if response.status_code == self.CODE_NOT_FOUND:
             return False
 
         # raise for status
         response.raise_for_status
 
         return False
 
-    def get_org_members(self, filterString=None, role=None, insecure=False):
+    def get_org_members(self, filterString=None, role=None, insecure=False):  # noqa: N803
         """Return a list of organization members."""
         # GET /orgs/:org/members
         params = {
             "filter": filterString,
             "role": role,
         }
         # add 2fa_disabled tag if insecure is true
         if insecure:
             params["filter"] = "2fa_disabled"
         return self.get_list(self.org_base_url, "members", params=params)
 
-    def get_org_members_dict(self, filterString=None, role=None, insecure=False, key="id"):
+    def get_org_members_dict(self, filterString=None, role=None, insecure=False, key="id"):  # noqa: N803
         """Return a dict of organization teams."""
         return self.get_dict(self.get_org_members(filterString, role, insecure), key)
 
     #
     # Org Memberships
     #
     def get_org_membership(self, member):
@@ -330,23 +333,23 @@
         # DELETE /orgs/:org/memberships/:username
         url = f"{self.org_base_url}/memberships/{member}"
         return requests.delete(url, headers=self.headers)
 
     #
     # Org Outside Collaborators
     #
-    def get_org_outside_collaborators(self, filterString=None, insecure=False):
+    def get_org_outside_collaborators(self, filterString=None, insecure=False):  # noqa: N803
         """Return a list of organization outside collaborators."""
         # GET /orgs/:org/outside_collaborators
         params = {"filter": filterString}
         if insecure:
             params["filter"] = "2fa_disabled"
         return self.get_list(self.org_base_url, "outside_collaborators", params=params)
 
-    def get_org_outside_collaborators_dict(self, filterString=None, insecure=False, key="id"):
+    def get_org_outside_collaborators_dict(self, filterString=None, insecure=False, key="id"):  # noqa: N803
         """Return a dict of organization outside collaborators."""
         return self.get_dict(self.get_org_outside_collaborators(filterString, insecure), key)
 
     #
     # Org Public Members
     #
     def get_org_public_member(self, member):
```

### Comparing `bits-github-1.3.8/bits/github/app.py` & `bits_github-1.4.0/bits/github/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
 """GitHub App class file."""
 
 import datetime
 import logging
 
 
-class App(object):
+class App:
     """GitHub App class."""
 
     def __init__(self, auth=None, github=None):
         """Initialize a class instance."""
         self.auth = auth
         self.github = github
 
@@ -35,18 +34,15 @@
             'google_email': google_email,
             'google_id': google_id,
             'token': token,
             'updated': datetime.datetime.now().isoformat(),
         }
 
         if not github_id or not github_login or not token:
-            logging.error('Invalid GitHub token info for user: %s [%s]' % (
-                google_email,
-                google_id,
-            ))
+            logging.error(f'Invalid GitHub token info for user: {google_email} [{google_id}]')
             logging.error('GitHub User Data: %s' % (github_user))
             return
 
         # save user in firestore
         return self.github.firestore().app.collection('tokens').document(google_id).set(data)
 
     #
```

### Comparing `bits-github-1.3.8/bits/github/auditlogs.py` & `bits_github-1.4.0/bits/github/auditlogs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# -*- coding: utf-8 -*-
 """Audit Logs class file."""
 
 import argparse
 import datetime
 import json
 import logging
-import pytz
 import re
 import sys
 
+import pytz
+
 from bits.google import Google
 
 
-class AuditLogs(object):
+class AuditLogs:
     """Audit Logs class."""
 
     def __init__(self, auth, github, args):
         """Initialize a class instance."""
         self.auth = auth
         self.github = github
 
@@ -57,32 +57,32 @@
         """Return the type of file being imported."""
         # determine the type of file being passed
         filetype = None
         if re.match('gs://', self.filename):
             filetype = 'gcs'
         elif not re.search(':', self.filename):
             filetype = 'local'
-        logging.info('Filename: {} [{}]'.format(self.filename, filetype))
+        logging.info(f'Filename: {self.filename} [{filetype}]')
         return filetype
 
     def _import_gcs_file(self):
         """Import audit logs from a gcs object."""
         g = Google()
         path = self.filename.replace('gs://', '')
         bucket = path.split('/')[0]
         filename = '/'.join(path.split('/')[1:])
         return g.storage().download_blob_as_string(bucket, filename)
 
     def _import_local_file(self):
         """Import audit logs from a local file."""
         # read file off disk
         try:
-            f = open(self.filename, 'r')
+            f = open(self.filename)
         except FileNotFoundError as e:
-            logging.error('Failed to open audit logs file: {}'.format(self.filename))
+            logging.error(f'Failed to open audit logs file: {self.filename}')
             sys.exit(e)
 
         return f.read()
 
     #
     # Parse arguments
     #
@@ -182,15 +182,15 @@
 
         # import file contents
         if location == 'gcs':
             filestring = self._import_gcs_file()
         elif location == 'local':
             filestring = self._import_local_file()
         else:
-            logging.error('Unsupported file path: "{}"'.format(self.filename))
+            logging.error(f'Unsupported file path: "{self.filename}"')
             sys.exit(1)
 
         # import json to a dictionary
         try:
             logs = sorted(json.loads(filestring), key=lambda x: x['created_at'])
         except json.decoder.JSONDecodeError as e:
             logging.error('Failed to import audit logs JSON.')
@@ -199,37 +199,36 @@
         return self.filter_logs(logs)
 
     def _get_repo_collaborators(self, repo):
         """Return a list of logins that are current repo collaborators."""
         try:
             collaborators = self.github.get_repo_collaborators(repo)
         except Exception as e:
-            logging.error('Failed to get collaborators for repo: {}'.format(repo))
+            logging.error(f'Failed to get collaborators for repo: {repo}')
             print(e)
             return []
         logins = []
         for m in collaborators:
             logins.append(m['login'].lower())
         return logins
 
     def _restore_repo_collaborators(self, repo, actions):
         """Restore collaborators for a single repo."""
         collaborators = self._get_repo_collaborators(repo)
-        print('\nRepo: {} [{}]'.format(repo, len(actions)))
+        print(f'\nRepo: {repo} [{len(actions)}]')
         for login in sorted(actions):
             if login in collaborators:
                 if self.verbose:
-                    print('   o Already added {}'.format(login))
+                    print(f'   o Already added {login}')
             elif login in self.org_members:
-                print('   + Inviting {}...'.format(login))
+                print(f'   + Inviting {login}...')
                 if not self.flags.noop:
                     self.github.add_repo_collaborator(repo, login)
-            else:
-                if self.verbose:
-                    print('   o Skipping {} [not org member]'.format(login))
+            elif self.verbose:
+                print(f'   o Skipping {login} [not org member]')
 
     def restore_repos_collaborators(self, logs):
         """Restore repo collaborators from audit logs."""
         self.org_members = self._get_org_members()
         repos = {}
         for row in logs:
             login = row['user'].lower()
@@ -238,44 +237,43 @@
                 repos[repo] = []
             if login not in repos[repo]:
                 repos[repo].append(login)
         if repos:
             resource = 'repo'
             if len(repos) > 1:
                 resource += 's'
-            print('\nRestoring collaborators to {} {}...'.format(len(repos), resource))
+            print(f'\nRestoring collaborators to {len(repos)} {resource}...')
             for repo in sorted(repos):
                 self._restore_repo_collaborators(repo, repos[repo])
 
     def _get_team_members(self, team_id):
         """Return a list of logins that are current team members."""
         logins = []
         for m in self.github.get_team_members(team_id):
             logins.append(m['login'].lower())
         return logins
 
     def _restore_team_members(self, slug, actions):
         """Restore members for a single team."""
         team = slug.replace('broadinstitute/', '')
         if team not in self.org_teams:
-            logging.error('Team not found in org: {}'.format(team))
+            logging.error(f'Team not found in org: {team}')
             return []
         team_id = self.org_teams[team]['id']
         members = self._get_team_members(team_id)
-        print('\nTeam: {} [{}]'.format(team, len(actions)))
+        print(f'\nTeam: {team} [{len(actions)}]')
         for login in sorted(actions):
             if login in members:
                 if self.verbose:
-                    print('   o Already added {}'.format(login))
+                    print(f'   o Already added {login}')
             elif login in self.org_members:
-                print('   + Inviting {}...'.format(login))
+                print(f'   + Inviting {login}...')
                 self.github.invite_team_member(team_id, login)
-            else:
-                if self.verbose:
-                    print('   o Skipping {} [not org member]'.format(login))
+            elif self.verbose:
+                print(f'   o Skipping {login} [not org member]')
 
     def restore_teams_members(self, logs):
         """Restore team members from audit logs."""
         self.org_members = self._get_org_members()
         self.org_teams = self._get_org_teams()
         teams = {}
         for row in logs:
@@ -289,66 +287,66 @@
                 teams[team] = []
             if login not in teams[team]:
                 teams[team].append(login)
         if teams:
             resource = 'team'
             if len(teams) > 1:
                 resource += 's'
-            print('\nRestoring members to {} {}...'.format(len(teams), resource))
+            print(f'\nRestoring members to {len(teams)} {resource}...')
             for team in sorted(teams):
                 self._restore_team_members(team, teams[team])
 
     #
     # Stats
     #
     def display_stats(self, stats):
         """Display stats about the logs."""
         start_date = stats['min_created_at']
         end_date = stats['max_created_at']
 
-        print('Audit Logs Start Date: {}'.format(start_date))
-        print('Audit Logs End Date: {}'.format(end_date))
+        print(f'Audit Logs Start Date: {start_date}')
+        print(f'Audit Logs End Date: {end_date}')
 
         # actions
         actions = stats['actions']
-        print('\nActions: [{}]'.format(len(actions)))
+        print(f'\nActions: [{len(actions)}]')
         print('{}{}'.format(
             '   * ',
             '\n   * '.join(sorted(actions)),
         ))
 
         # actors
         actors = stats['actors']
-        print('\nActors: [{}]'.format(len(actors)))
+        print(f'\nActors: [{len(actors)}]')
         print('{}{}'.format(
             '   * ',
             '\n   * '.join(sorted(actors)),
         ))
 
         # repos
         repos = stats['repos']
         if repos:
-            print('\nRepos: [{}]'.format(len(repos)))
+            print(f'\nRepos: [{len(repos)}]')
         print('{}{}'.format(
             '   * ',
             '\n   * '.join(sorted(repos)),
         ))
 
         # teams
         teams = stats['teams']
         if teams:
-            print('\nTeams: [{}]'.format(len(teams)))
+            print(f'\nTeams: [{len(teams)}]')
         print('{}{}'.format(
             '   * ',
             '\n   * '.join(sorted(teams)),
         ))
 
         # users
         users = stats['users']
-        print('\nUsers: [{}]'.format(len(users)))
+        print(f'\nUsers: [{len(users)}]')
         print('{}{}'.format(
             '   * ',
             '\n   * '.join(sorted(users)),
         ))
 
     def get_stats(self, logs):
         """Return status about the logs."""
```

### Comparing `bits-github-1.3.8/bits/github/client.py` & `bits_github-1.4.0/bits/github/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
 """GitHub Client class file."""
 
 import re
 import sys
 
 
-class Client(object):
+class Client:
     """GitHub Client class."""
 
     def __init__(self, auth, github, app_project=None):
         """Initialize a class instance."""
         self.auth = auth
         self.github = github
 
@@ -19,28 +18,25 @@
     def auditlogs_restore(self, args=None):
         """Restore users to repos or teams from audit logs."""
         auditlogs = self.github.auditlogs(auth=self.auth, args=args)
         logs = list(auditlogs.import_logs())
         if not logs:
             return
         auditlogs.display_logs(logs)
-        print('Your filters matched {} audit log entries.'.format(len(logs)))
+        print(f'Your filters matched {len(logs)} audit log entries.')
         if auditlogs.flags.action == 'repo.remove_member':
             resource = 'repo collaborator'
         elif auditlogs.flags.action == 'team.remove_member':
             resource = 'team member'
         else:
-            error = 'Unsupported action: {}'.format(auditlogs.flags.action)
+            error = f'Unsupported action: {auditlogs.flags.action}'
             sys.exit(error)
         if len(logs) > 1:
             resource += 's'
-        response = input('\nRestore {} {} from the log entries above? [y/N]: '.format(
-            len(logs),
-            resource,
-        ))
+        response = input(f'\nRestore {len(logs)} {resource} from the log entries above? [y/N]: ')
         if not re.match('(y|Y)', response):
             sys.exit('Exiting.')
 
         if auditlogs.flags.action == 'repo.remove_member':
             auditlogs.restore_repos_collaborators(logs)
         elif auditlogs.flags.action == 'team.remove_member':
             auditlogs.restore_teams_members(logs)
@@ -62,150 +58,132 @@
                 continue
             print('{} -> {} [{}]'.format(
                 person['email_username'],
                 person['github_login'],
                 person['github_id'],
             ))
             users.append(person)
-        print('Total Linked GitHub Users: {}'.format(len(users)))
+        print(f'Total Linked GitHub Users: {len(users)}')
 
     def collaborators_list(self):
         """List GitHub Collaborators."""
         print('Getting GitHub collaborators...')
         github_collaborators = self.github.get_org_outside_collaborators()
-        print('Found {} collaborators in organization: {}.'.format(
-            len(github_collaborators),
-            self.github.org,
-        ))
+        print(f'Found {len(github_collaborators)} collaborators in organization: {self.github.org}.')
         for c in sorted(github_collaborators, key=lambda x: x['login'].lower()):
             print('{} [{}]'.format(c['login'].lower(), c['id']))
 
     def invitations_list(self):
         """List GitHub Invitations."""
         print('Getting GitHub invitations...')
         github_invitations = self.github.get_org_invitations()
-        print('Found {} invitations in organization: {}.'.format(
-            len(github_invitations),
-            self.github.org,
-        ))
+        print(f'Found {len(github_invitations)} invitations in organization: {self.github.org}.')
         for i in sorted(github_invitations, key=lambda x: x['login'].lower()):
             print('{}: {} ({}) [{}]'.format(
                 i['login'].lower(),
                 i['created_at'],
                 i['role'],
                 i['id'],
             ))
 
     def members_list(self, insecure=False):
         """List GitHub Members."""
         print('Getting GitHub members...')
         github_members = self.github.get_org_members(insecure=insecure)
-        print('Found {} members in organization: {}.'.format(
-            len(github_members),
-            self.github.org,
-        ))
+        print(f'Found {len(github_members)} members in organization: {self.github.org}.')
         for m in sorted(github_members, key=lambda x: x['login'].lower()):
             admin = ''
             if m['site_admin']:
                 admin = ' (admin)'
             print('{} [{}]{}'.format(
                 m['login'].lower(),
                 m['id'],
                 admin
             ))
 
     def organization_audit(self):
         """Audit the github organiztaion."""
-        print('Organization Name: {}'.format(self.github.org))
+        print(f'Organization Name: {self.github.org}')
 
         print('\nGetting organization members...')
         members = self.github.get_org_members()
-        print('Found {} organization members.'.format(len(members)))
+        print(f'Found {len(members)} organization members.')
 
         print('\nGetting organization collaborators...')
         collaborators = self.github.get_org_outside_collaborators()
-        print('Found {} organization collaborators.'.format(len(collaborators)))
+        print(f'Found {len(collaborators)} organization collaborators.')
 
         print('\nGetting owner account members...')
         owners = self.github.get_org_members(role='admin')
         for user in sorted(owners, key=lambda x: x['login'].lower()):
             print('   * {} [{}]'.format(user['login'].lower(), user['id']))
-        print('Found {} owner account members.'.format(len(owners)))
+        print(f'Found {len(owners)} owner account members.')
 
         print('\nGetting role account members...')
         role_members = self.github.get_team_members(self.github.role_team)
         for user in sorted(role_members, key=lambda x: x['login'].lower()):
             print('   * {} [{}]'.format(user['login'].lower(), user['id']))
-        print('Found {} role account members.'.format(len(role_members)))
+        print(f'Found {len(role_members)} role account members.')
 
         print('\nGetting open organization invitations...')
         invitations = self.github.get_org_invitations()
         for i in sorted(invitations, key=lambda x: x['login'].lower()):
             print('   * {} [{}]'.format(i['login'].lower(), i['id']))
-        print('Found {} open organization invitations.'.format(len(invitations)))
+        print(f'Found {len(invitations)} open organization invitations.')
 
         print('\nGetting organization repos...')
         repos = self.github.get_org_repos()
         private_repos = []
         public_repos = []
         for r in sorted(repos, key=lambda x: x['name']):
             if r['private']:
                 private_repos.append(r)
             else:
                 public_repos.append(r)
-        print('   * private repos: {}'.format(len(private_repos)))
-        print('   * public repos: {}'.format(len(public_repos)))
-        print('Found {} organization repos.'.format(len(repos)))
+        print(f'   * private repos: {len(private_repos)}')
+        print(f'   * public repos: {len(public_repos)}')
+        print(f'Found {len(repos)} organization repos.')
 
         print('\nGetting organization teams...')
         teams = self.github.get_org_teams()
-        print('Found {} organization teams.'.format(len(teams)))
+        print(f'Found {len(teams)} organization teams.')
 
     def public_members_list(self):
         """List GitHub Public Mmebers."""
         print('Getting GitHub public_members...')
         github_members = self.github.get_org_public_members()
-        print('Found {} public_members in organization: {}.'.format(
-            len(github_members),
-            self.github.org,
-        ))
+        print(f'Found {len(github_members)} public_members in organization: {self.github.org}.')
         for m in sorted(github_members, key=lambda x: x['login'].lower()):
             print('{} [{}]'.format(m['login'].lower(), m['id']))
 
     def repo_hooks_list(self):
         """List GitHub Repo Hooks."""
         print('Getting GitHub repos...')
         github_repos = self.github.get_org_repos()
-        print('Found {} repos in organization: {}.'.format(
-            len(github_repos),
-            self.github.org,
-        ))
+        print(f'Found {len(github_repos)} repos in organization: {self.github.org}.')
         for r in sorted(github_repos, key=lambda x: x['name']):
             hooks = self.github.get_repo_hooks(r['name'])
             if hooks:
                 print('{}/{}:'.format(self.github.org, r['name']))
                 for h in hooks:
                     # get repo hook name
                     name = h['name']
                     if name == 'web':
                         name = h['config'].get('url')
                     # get repo hook status
                     status = 'inactive'
                     if h['active']:
                         status = 'active'
-                    print('  - {}: ({})'.format(name, status))
+                    print(f'  - {name}: ({status})')
 
     def repo_hooks_search(self, query):
         """List GitHub Repo Hooks."""
         print('Getting GitHub repos...')
         github_repos = self.github.get_org_repos()
-        print('Found {} repos in organization: {}.'.format(
-            len(github_repos),
-            self.github.org,
-        ))
+        print(f'Found {len(github_repos)} repos in organization: {self.github.org}.')
         for r in sorted(github_repos, key=lambda x: x['name']):
             hooks = self.github.get_repo_hooks(r['name'])
             if hooks:
                 matches = []
                 for h in hooks:
                     name = h['name']
                     if name == 'web':
@@ -226,18 +204,15 @@
                         status,
                     ))
 
     def repos_list(self):
         """List GitHub Repos."""
         print('Getting GitHub repos...')
         github_repos = self.github.get_org_repos()
-        print('Found {} repos in organization: {}.'.format(
-            len(github_repos),
-            self.github.org,
-        ))
+        print(f'Found {len(github_repos)} repos in organization: {self.github.org}.')
         for r in sorted(github_repos, key=lambda x: x['name']):
             print('{} [{}]'.format(r['name'], r['id']))
 
     def role_accounts_list(self):
         """List GitHub Role Accounts."""
         print('Getting GitHub Role Accounts...')
         team = self.github.get_team(self.github.role_team)
@@ -245,60 +220,54 @@
         for m in sorted(role_accounts, key=lambda x: x['login'].lower()):
             print('{} [{}]'.format(m['login'].lower(), m['id']))
 
     def services_list(self):
         """List GitHub Services."""
         print('Getting GitHub repos...')
         github_repos = self.github.get_org_repos()
-        print('Found {} repos in organization: {}.'.format(
-            len(github_repos),
-            self.github.org,
-        ))
+        print(f'Found {len(github_repos)} repos in organization: {self.github.org}.')
         for r in sorted(github_repos, key=lambda x: x['name']):
             hooks = self.github.get_repo_hooks(r['name'])
             if hooks:
                 output = ''
                 for h in hooks:
                     name = h['name']
                     if name == 'web':
                         continue
                     # get hook status
                     status = 'inactive'
                     if h['active']:
                         status = 'active'
                     # set output
-                    output += '  - {}: ({})\n'.format(
-                        name,
-                        status
-                    )
+                    output += f'  - {name}: ({status})\n'
                 if output:
                     print('{}/{}:'.format(self.github.org, r['name']))
                     print(output)
 
-    def teams_audit(self):
+    def teams_audit(self):  # noqa: PLR0912,PLR0915
         """Audit github teams."""
         print('\nGetting organization teams...')
         teams = self.github.get_org_teams()
-        print('Found {} organization teams.'.format(len(teams)))
+        print(f'Found {len(teams)} organization teams.')
 
         print('\nGetting cached teams members...')
         teams_members = self.firestore.get_teams_members_dict()
-        print('Found {} teams members.'.format(len(teams_members)))
+        print(f'Found {len(teams_members)} teams members.')
 
         print('\nGetting cached teams repos...')
         teams_repos = self.firestore.get_teams_repos_dict()
-        print('Found {} teams repos.'.format(len(teams_repos)))
+        print(f'Found {len(teams_repos)} teams repos.')
 
         print('\nGetting org admins...')
         owners = self.github.get_org_members(role="admin")
-        print('Found {} org admins.'.format(len(owners)))
+        print(f'Found {len(owners)} org admins.')
 
         print('\nGetting team syncs...')
         team_syncs = self.firestore.get_team_syncs_dict()
-        print('Found {} team syncs.'.format(len(team_syncs)))
+        print(f'Found {len(team_syncs)} team syncs.')
 
         print('\nChecking for teams with no members or no repos:')
 
         nomembers = []
         norepos = []
         onemember = []
         for t in sorted(teams, key=lambda x: x['slug']):
@@ -308,17 +277,17 @@
             if not tmembers.get('members', []):
                 nomembers.append(t)
             if len(tmembers.get('members', [])) == 1:
                 onemember.append(t)
             if not trepos.get('repos', []):
                 norepos.append(t)
 
-        print('Found {} teams with no members.'.format(len(nomembers)))
-        print('Found {} teams with one member.'.format(len(onemember)))
-        print('Found {} teams with no repos.'.format(len(norepos)))
+        print(f'Found {len(nomembers)} teams with no members.')
+        print(f'Found {len(onemember)} teams with one member.')
+        print(f'Found {len(norepos)} teams with no repos.')
 
         if nomembers:
             print('\nTeams with no members:')
             for team in sorted(nomembers, key=lambda x: x['slug']):
                 slug = team['slug']
                 team_url = 'https://github.com/orgs/broadinstitute/teams'
                 note = ''
@@ -366,15 +335,15 @@
                     slug,
                     t['id'],
                     team_url,
                     slug,
                     note
                 ))
 
-        print('\nTeams with Google Group Syncs [{}]:'.format(len(team_syncs)))
+        print(f'\nTeams with Google Group Syncs [{len(team_syncs)}]:')
         for slug in sorted(team_syncs):
             sync = team_syncs[slug]
             tid = sync['team_id']
 
             maintainers = self.github.get_team_members(tid, role='maintainer')
             logins = []
             for user in maintainers:
@@ -388,17 +357,15 @@
                 slug,
                 sync['group_email'],
                 ', '.join(sorted(logins))
             ))
 
         nomaintainer = []
 
-        print('\nTeams without Google Group Syncs [{}]:'.format(
-            len(teams) - len(team_syncs)
-        ))
+        print(f'\nTeams without Google Group Syncs [{len(teams) - len(team_syncs)}]:')
 
         print('\n  With a Maintainer:')
         for team in sorted(teams, key=lambda x: x['slug']):
             tid = team['id']
             slug = team['slug']
             if slug in team_syncs:
                 continue
@@ -424,23 +391,23 @@
             slug = team['slug']
             print('     * {} [{}]'.format(slug, team['id']))
 
     def team_syncs_list(self):
         """List GitHub Team Syncs."""
         print('Getting GitHub team syncs...')
         team_syncs = self.firestore.get_team_syncs_dict()
-        print('Found {} syncs.'.format(len(team_syncs)))
+        print(f'Found {len(team_syncs)} syncs.')
         for oid in sorted(team_syncs, key=lambda x: team_syncs[x]['google_group']):
             s = team_syncs[oid]
             print('{} --> {} [{}]'.format(
                 s['google_group'],
                 s['github_team_slug'],
                 s['github_team']
             ))
 
     def teams_list(self):
         """List Github teams."""
         print('Getting GitHub teams...')
         teams = self.github.get_org_teams()
-        print('Found {} teams in organization: {}.'.format(len(teams), self.github.org))
+        print(f'Found {len(teams)} teams in organization: {self.github.org}.')
         for r in sorted(teams, key=lambda x: x['slug']):
             print('{} [{}]'.format(r['slug'], r['id']))
```

### Comparing `bits-github-1.3.8/bits/github/datastore.py` & `bits_github-1.4.0/bits/github/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 """Datastore Class file."""
 
 from google.cloud import datastore
 
 
-class Datastore(object):
+class Datastore:
     """Datastore class."""
 
     def __init__(
         self,
         auth=None,
         github=None,
         project='broad-github-app'
```

### Comparing `bits-github-1.3.8/bits/github/firestore.py` & `bits_github-1.4.0/bits/github/firestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
 """Firestore Class file."""
 
 import re
+
 from google.cloud import firestore
 
 
-class Firestore(object):
+class Firestore:
     """Firestore class."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         auth=None,
         github=None,
         project='broad-bitsdb-firestore',
         app_project=None,
         bitsdb_project='broad-bitsdb-prod',
     ):
@@ -126,15 +126,15 @@
         fields = [
             'team_id',
             'team_slug',
             'group_email',
             'group_id',
         ]
         groups_ref = self.app.collection('team_syncs')
-        query = groups_ref.where(u'group_members', u'array_contains', google_id).select(fields)
+        query = groups_ref.where('group_members', 'array_contains', google_id).select(fields)
         team_syncs = []
         for doc in query.stream():
             sync = doc.to_dict()
             team_syncs.append(sync)
         return team_syncs
 
     #
@@ -232,15 +232,15 @@
             path = doc.reference.path
             if not re.match(r'github_teams\/[0-9]+\/repos\/[0-9]+', path):
                 continue
             _, team_id, _, _ = path.split('/')
 
             team_id = int(team_id)
             if team_id not in teams:
-                print('ERROR: Team not found: {}'.format(team_id))
+                print(f'ERROR: Team not found: {team_id}')
                 continue
 
             team = teams[team_id]
             if 'repos' not in team:
                 team['repos'] = []
 
             team['repos'].append(doc.to_dict())
```

### Comparing `bits-github-1.3.8/bits/github/helpers.py` & `bits_github-1.4.0/bits/github/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 """GitHub Helpers class file."""
 
 import dateutil.parser as dateparser
 
 
-class Helpers(object):
+class Helpers:
     """GitHub Helpers class."""
 
     def __init__(self, auth=None, github=None):
         """Initialize a class instance."""
         self.auth = auth
         self.github = github
 
@@ -42,20 +41,20 @@
             else:
                 user = self.github.get_user(login)
 
             # check if record was updated
             if user is False:
                 members.append(cached)
                 if self.verbose:
-                    print('Skipped user: {}'.format(login))
+                    print(f'Skipped user: {login}')
             else:
                 members.append(user)
                 # firestore.db.collection('github_members').document(str(mid)).set(user)
                 if self.verbose:
-                    print('Updated user: {}'.format(login))
+                    print(f'Updated user: {login}')
 
         return members
 
     def get_org_repos_full(self):
         """Return a list of org repos with full details."""
         firestore = self.github.firestore(app_project='broad-github-app')
         firestore_repos = firestore.get_repos_dict()
@@ -78,20 +77,20 @@
             else:
                 repo = self.github.get_repo(name)
 
             # check if record was updated
             if repo is False:
                 repos.append(cached)
                 if self.verbose:
-                    print('Skipped repo: {}'.format(name))
+                    print(f'Skipped repo: {name}')
             else:
                 repos.append(repo)
                 # firestore.db.collection('github_repos').document(str(rid)).set(repo)
                 if self.verbose:
-                    print('Updated repo: {}'.format(name))
+                    print(f'Updated repo: {name}')
 
         return repos
 
     def get_org_teams_full(self):
         """Return a list of org teams with full details."""
         firestore = self.github.firestore(app_project='broad-github-app')
         firestore_teams = firestore.get_teams_dict()
@@ -114,20 +113,20 @@
             else:
                 team = self.github.get_team(tid)
 
             # check if record was updated
             if team is False:
                 teams.append(cached)
                 if self.verbose:
-                    print('Skipped team: {}'.format(name))
+                    print(f'Skipped team: {name}')
             else:
                 teams.append(team)
                 # firestore.db.collection('github_teams').document(str(tid)).set(team)
                 if self.verbose:
-                    print('Updated team: {}'.format(name))
+                    print(f'Updated team: {name}')
 
         return teams
 
     def get_org_repos_collaborators(self):
         """Return a list of org repos collaborators."""
         repos_collaborators = []
         for r in sorted(self.github.get_org_repos(), key=lambda x: x['name'].lower()):
@@ -143,15 +142,15 @@
                 'id': rid,
                 'name': name,
                 'collaborators': collaborators,
             }
             repos_collaborators.append(repo)
             # firestore.db.collection('github_repos_collaborators').document(str(rid)).set(repo)
             if self.verbose:
-                print('Updated repo collaborators: {}'.format(name))
+                print(f'Updated repo collaborators: {name}')
 
         return repos_collaborators
 
     def get_org_teams_members(self):
         """Return an iterator of org teams and their members."""
         for t in sorted(self.github.get_org_teams(), key=lambda x: x['slug'].lower()):
             tid = t['id']
@@ -164,15 +163,15 @@
 
             team = {
                 'id': tid,
                 'slug': slug,
                 'members': members,
             }
             if self.verbose:
-                print('Retrieved {} members from team: {}'.format(len(members), slug))
+                print(f'Retrieved {len(members)} members from team: {slug}')
 
             yield team
 
     def get_org_teams_repos(self):
         """Return an iterator of org teams and their repos."""
         for t in sorted(self.github.get_org_teams(), key=lambda x: x['slug'].lower()):
             tid = t['id']
@@ -185,10 +184,10 @@
 
             team = {
                 'id': tid,
                 'slug': slug,
                 'repos': repos,
             }
             if self.verbose:
-                print('Retrieved {} repos from team: {}'.format(len(repos), slug))
+                print(f'Retrieved {len(repos)} repos from team: {slug}')
 
             yield team
```

### Comparing `bits-github-1.3.8/bits/github/sync.py` & `bits_github-1.4.0/bits/github/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 """GitHub Sync Class."""
 
 
-class Sync(object):
+class Sync:
     """Sync Class."""
 
     def __init__(self, auth=None, github=None):
         """Initialize a class instance."""
         self.auth = auth
         self.github = github
         self.mongo = auth.mongo_prod()
@@ -46,19 +45,19 @@
         firestore = self.github.firestore()
         return firestore.get_people_dict()
 
     def prepare_data(self):
         """Prepare data for syncing."""
         print('Getting source data...')
         github_team_syncs = self.get_mongo_github_team_syncs()
-        print('  Found {} github_team_sync records in BITSdb Mongo.'.format(len(github_team_syncs)))
+        print(f'  Found {len(github_team_syncs)} github_team_sync records in BITSdb Mongo.')
         github_users = self.get_datastore_users()
-        print('  Found {} GitHubUser records in broad-github Datastore.'.format(len(github_users)))
+        print(f'  Found {len(github_users)} GitHubUser records in broad-github Datastore.')
         people = self.get_people()
-        print('  Found {} people records in bits-bitsdb-firestore Firestore.'.format(len(people)))
+        print(f'  Found {len(people)} people records in bits-bitsdb-firestore Firestore.')
 
     def update_all(self):
         """Sync all GitHub data."""
         # prepare data for syncing
         self.prepare_data()
         self.update_team_syncs()
         self.update_users()
```

### Comparing `bits-github-1.3.8/bits/github/update.py` & `bits_github-1.4.0/bits/github/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# -*- coding: utf-8 -*-
 """Update Class file."""
 
 import datetime
-import dateutil.parser
 import logging
-import pytz
 import sys
 
-from bits.github import GitHub
+import dateutil.parser
+import pytz
 from requests import HTTPError
 
+from . import GitHub
+
 
-class Update(object):
+class Update:
     """Update class."""
 
+    MAX_REMOVE = 50
+    CODE_UNAUTHORIZED = 401
+
     def __init__(self, auth=None, github=None):
         """Initialize a class instance."""
         self.auth = auth
         self.github = github
 
         self.verbose = False
         if self.auth:
@@ -78,15 +81,15 @@
             invitations[login] = i
         return invitations
 
     def _get_members(self):
         """Return a dict of members by GitHub ID."""
         members = {}
         for m in self.github.get_org_members():
-            gid = u'{}'.format(m['id'])
+            gid = '{}'.format(m['id'])
             members[gid] = m
         return members
 
     def _get_new_logins(self, new):
         """Return a list of logins in the new users data."""
         logins = []
         for gid in new:
@@ -190,25 +193,25 @@
         return uninvite
 
     def _prepare_members(self):
         """Prepare a list of org members for GitHub."""
         # get users that have linked their github account
         if not self.users:
             self.users = self._get_users()
-        print('Found {} Tokens in GitHub App.'.format(len(self.users)))
+        print(f'Found {len(self.users)} Tokens in GitHub App.')
 
         # get people
         if not self.people:
             self.people = self._get_people()
-        print('Found {} People in BITSdb.'.format(len(self.people)))
+        print(f'Found {len(self.people)} People in BITSdb.')
 
         # get role_accounts
         if not self.role_accounts:
             role_accounts = self._get_github_role_accounts()
-        print('Found {} GitHub Role Accounts.'.format(len(role_accounts)))
+        print(f'Found {len(role_accounts)} GitHub Role Accounts.')
 
         members = {}
 
         # add github users who have linked their account and have a valid token
         for email in self.users:
             user = self.users[email]
             github_id = str(user['github_id'])
@@ -241,75 +244,74 @@
 
             # check if google id is in people
             if google_id not in self.people:
                 print('Person not found: {} [{}]'.format(m['email'], google_id))
                 continue
 
             # check if google id is terminated
-            else:
-                if self.people[google_id]['terminated']:
-                    continue
+            elif self.people[google_id]['terminated']:
+                continue
 
             user = self.google_ids[google_id]
             github_id = user['github_id']
             team_members[github_id] = user
 
         return team_members
 
     #
     # Update Org Members
     #
     def update_members(self):
         """Update members in GitHub."""
         current = self._get_members()
-        print('Found {} current GitHub Members.'.format(len(current)))
+        print(f'Found {len(current)} current GitHub Members.')
 
         new = self._prepare_members()
-        print('Found {} suitable GitHub Members.'.format(len(new)))
+        print(f'Found {len(new)} suitable GitHub Members.')
 
         invitations = self._get_invitations()
-        print('Found {} open GitHub Invitations.'.format(len(invitations)))
+        print(f'Found {len(invitations)} open GitHub Invitations.')
 
         # get users to invite and remove from the org
         invite = self._get_users_to_invite(current, new, invitations)
         remove = self._get_users_to_remove(current, new)
 
         # check to make sure we do not remove too many members
         current_count = len(current) + len(invitations)
         new_count = len(new)
 
-        # check for more than 50 members being removed
-        if (current_count - new_count) > 50 or len(remove) > 50:
-            logging.error('More than 50 members to remove! Exiting.')
+        # check for more than MAX_REMOVE members being removed
+        if (current_count - new_count) > self.MAX_REMOVE or len(remove) > self.MAX_REMOVE:
+            logging.error(f"More than {self.MAX_REMOVE} members to remove! Exiting.")
             sys.exit(1)
 
         # check for invitations to cancel
         logins = self._get_new_logins(new)
         uninvite = self._get_users_to_uninvite(invitations, logins)
 
         if invite:
-            print('\nMembers to invite: {}'.format(len(invite)))
+            print(f'\nMembers to invite: {len(invite)}')
             for login in sorted(invite):
-                print('   + {}'.format(login))
+                print(f'   + {login}')
                 try:
                     self.github.invite_org_member(login)
                 except Exception as e:
-                    print('ERROR: Failed to invite org member: {}'.format(login))
+                    print(f'ERROR: Failed to invite org member: {login}')
                     print(e)
 
         if remove:
-            print('\nMembers to remove: {}'.format(len(remove)))
+            print(f'\nMembers to remove: {len(remove)}')
             for login in sorted(remove):
-                print('   - {}'.format(login))
+                print(f'   - {login}')
                 self.github.remove_org_member(login)
 
         if uninvite:
-            print('\nInvitations to cancel: {}'.format(len(uninvite)))
+            print(f'\nInvitations to cancel: {len(uninvite)}')
             for login in sorted(uninvite):
-                print('   - {}'.format(login))
+                print(f'   - {login}')
                 self.github.remove_org_member(login)
 
         if self.verbose:
             print('Done updating GitHub members.')
 
     #
     # Update Org Teams
@@ -331,70 +333,62 @@
         # get team members to add
         add = self._get_team_members_to_add(current, new, invitations)
 
         # get team members to remove
         remove = self._get_team_members_to_remove(current, new, invitations)
 
         if self.verbose or add or remove:
-            print('\n{} [{}] <-- {}:'.format(
-                slug,
-                team_id,
-                email,
-            ))
+            print(f'\n{slug} [{team_id}] <-- {email}:')
 
         # display stats
         if self.verbose:
-            print('   current: {}, group: {}, new: {}, invitations: {}'.format(
-                len(current),
-                len(group_members),
-                len(new),
-                len(invitations),
-            ))
+            print(f"   current: {len(current)}, group: {len(group_members)}, "
+                   "new: {len(new)}, invitations: {len(invitations)}")
 
         # display any users to add
         if add:
-            print('   members to add: {}'.format(len(add)))
+            print(f'   members to add: {len(add)}')
             for github_id in sorted(add, key=lambda x: add[x]['login'].lower()):
                 user = add[github_id]
                 login = user['login'].lower()
-                print('     + {} [{}]'.format(login, github_id))
+                print(f'     + {login} [{github_id}]')
                 # add the github user to the team
                 self.github.invite_team_member(team_id, login)
 
         # display any users to remove
         if remove:
-            print('   members to remove: {}'.format(len(remove)))
+            print(f'   members to remove: {len(remove)}')
             for github_id in sorted(remove, key=lambda x: remove[x]['login'].lower()):
                 user = remove[github_id]
                 login = user['login'].lower()
-                print('     - {} [{}]'.format(login, github_id))
+                print(f'     - {login} [{github_id}]')
                 # remove the github user from the team
                 self.github.remove_team_member(team_id, login)
 
     def update_teams(self):
         """Update team membership in GitHub from Google Groups."""
         # get Broadies that have linked their GitHub accounts.
         if not self.users:
             self.users = self._get_users()
-        print('Found {} Tokens in GitHub App.'.format(len(self.users)))
+        print(f'Found {len(self.users)} Tokens in GitHub App.')
 
         # get role accounts
         if not self.role_accounts:
             self.role_accounts = self._get_github_role_accounts()
-        print('Found {} Role Accounts in GitHub.'.format(len(self.role_accounts)))
+        print(f'Found {len(self.role_accounts)} Role Accounts in GitHub.')
 
         # firestore - get people
         if not self.people:
             self.people = self._get_people()
-        print('Found {} People in BITSdb.'.format(len(self.people)))
+        print(f'Found {len(self.people)} People in BITSdb.')
 
         # firestore - get team syncs
         firestore = self.github.firestore(app_project='broad-github-app')
         team_syncs = firestore.get_team_syncs_dict()
-        print('Found {} GitHub Team Syncs in BITSdb.'.format(len(team_syncs)))
+        print(f'Found {len(team_syncs)} GitHub Team Syncs in BITSdb.')
 
         for slug in sorted(team_syncs):
             s = team_syncs[slug]
             team_id = s['team_id']
             email = s['group_email']
             self.update_team(slug, team_id, email)
 
@@ -428,24 +422,24 @@
             if isinstance(created, str):
                 sync['created'] = datetime.datetime.strptime(created, '%Y-%b-%d %H:%M:%S').astimezone(tz)
             if isinstance(modified, str):
                 sync['modified'] = datetime.datetime.strptime(modified, '%Y-%b-%d %H:%M:%S').astimezone(tz)
             mongo_team_syncs.append(sync)
             syncs_dict[sync['_id']] = sync
         m.update_collection('github_team_sync', syncs_dict)
-        print('Found {} GitHub Team Syncs in BITSdb Mongo.'.format(len(mongo_team_syncs)))
+        print(f'Found {len(mongo_team_syncs)} GitHub Team Syncs in BITSdb Mongo.')
 
         # create new dict of team syncs ready for datastore and firestore
         datastore_syncs = {}
         firestore_syncs = {}
         for sync in sorted(mongo_team_syncs, key=lambda x: x['google_group']):
             del sync['_id']
             email = sync['google_group']
 
-            print('Getting group and members: {}'.format(email))
+            print(f'Getting group and members: {email}')
             # get group
             group = g.directory().get_group(email)
             # get members
             members = []
             for m in g.directory().get_members_recursively(email):
                 members.append(m['id'])
 
@@ -476,20 +470,20 @@
                 'team_name': sync['github_team_name'],
                 'team_slug': sync['github_team_slug'],
             }
             team_id = str(sync['github_team'])
 
             # add to datastore syncs
             if team_id in datastore_syncs:
-                print('Duplicate Datastore Sync: {} -> {}'.format(email, team_id))
+                print(f'Duplicate Datastore Sync: {email} -> {team_id}')
             datastore_syncs[team_id] = datastore_sync
 
             # add to firestore syncs
             if team_id in firestore_syncs:
-                print('Duplicate Firestore Sync: {} -> {}'.format(email, team_id))
+                print(f'Duplicate Firestore Sync: {email} -> {team_id}')
             firestore_syncs[team_id] = firestore_sync
 
         # update the data in the bitsdb api
         b.update(
             cls=g,
             collection='github/teams/syncs',
             data=datastore_syncs,
@@ -537,20 +531,20 @@
             google_email = t['google_email']
 
             remove = False
             update = False
 
             # check google_id
             if google_id not in people:
-                print('Google User not found: {} [{}]'.format(google_id, google_email))
+                print(f'Google User not found: {google_id} [{google_email}]')
                 remove = True
 
             # check github_id
             elif github_id not in users:
-                print('GitHub User not found: {} [{}]'.format(github_id, github_login))
+                print(f'GitHub User not found: {github_id} [{github_login}]')
                 remove = True
 
             # check google email
             elif google_email != people[google_id]['email_username']:
                 print('Google Email needs update: {}: {} -> {}'.format(
                     google_id,
                     google_email,
@@ -572,29 +566,29 @@
             if remove:
                 remove_tokens.append(t)
             elif update:
                 update_tokens.append(t)
 
         # update tokens that need updating
         if update_tokens:
-            print('\nUpdating tokens for {} users...'.format(len(update_tokens)))
+            print(f'\nUpdating tokens for {len(update_tokens)} users...')
             for t in sorted(update_tokens, key=lambda x: x['github_login']):
                 current = firestore.get_stored_token(t['google_id'])
                 print('   * {} [{}]'.format(
                     current['github_login'],
                     current['github_id'],
                 ))
                 current = firestore.get_stored_token(t['google_id'])
                 current['github_login'] = t['github_login']
                 current['google_email'] = t['google_email']
                 firestore.store_token(current)
 
         # remove tokens that need updating
         if remove_tokens:
-            print('\nRemoving tokens for {} users...'.format(len(remove_tokens)))
+            print(f'\nRemoving tokens for {len(remove_tokens)} users...')
             for t in sorted(remove_tokens, key=lambda x: x['github_login']):
                 print('   - {} [{}]'.format(
                     t['github_login'],
                     t['github_id'],
                 ))
                 firestore.delete_stored_token(t['google_id'])
 
@@ -612,75 +606,78 @@
         # authenticate with user's token
         github = GitHub(token)
 
         # get user from github api
         try:
             new = github.get_self(last_modified=last_modified)
         except HTTPError as e:
-            if e.response.status_code == 401:
-                logging.warning('Invalid token for user: {} [{}]'.format(login, github_id))
-                print('Deleting user with invalid token: {} [{}]'.format(login, github_id))
+            if e.response.status_code == self.CODE_UNAUTHORIZED:
+                logging.warning(f"Invalid token for user: {login} [{github_id}]")
+                print(f"Deleting user with invalid token: {login} [{github_id}]")
                 # delete user with invalid token from user token store
                 self.github.firestore().delete_stored_github_user(github_id)
             else:
-                logging.error('Failed to get user: {} [{}]'.format(login, github_id))
+                logging.error(f'Failed to get user: {login} [{github_id}]')
                 logging.error(e)
             return user
 
         # don't update users that haven't changed
         if new is False:
             # User record has not been updated since the last time we checked.
             if self.verbose:
-                print('Skipping {} [{}]'.format(login, github_id))
+                print(f'Skipping {login} [{github_id}]')
             return user
 
         # print(json.dumps(user, indent=2, sort_keys=True))
         if user:
             print('Updated user: {}'.format(new['login'].lower()))
         else:
             print('Added user: {}'.format(new['login'].lower()))
 
         # check user_id
         user_id = str(new['id'])
         if github_id != user_id:
-            logging.error('User ID Mismatch: {} != {}'.format(github_id, user_id))
+            logging.error(f'User ID Mismatch: {github_id} != {user_id}')
 
         return new
 
     def update_users(self):
         """Update cached data about linked users in Firestore."""
         # get Broadies that have linked their GitHub accounts.
         if not self.users:
             self.users = self._get_users()
         if self.verbose:
-            print('Found {} Tokens in GitHub App.'.format(len(self.users)))
+            print(f"Found {len(self.users)} Tokens in GitHub App.")
 
         if not self.github_users:
             self.github_users = self._get_firestore_github_users()
         if self.verbose:
-            print('Found {} GitHub Users in Firestore.'.format(len(self.github_users)))
+            print(f"Found {len(self.github_users)} GitHub Users in Firestore.")
 
         # update users
         github_users = []
         updates = []
         for email in sorted(self.users, key=lambda x: self.users[x]['login'].lower()):
             # get user from github app with stored token
             linked_user = self.users[email]
             github_id = linked_user['github_id']
             login = linked_user['login']
             token = linked_user['token']
 
             # get cached user from firestore
             user = self.github_users.get(github_id, {})
             new = self.update_user(github_id, login, token, user)
+            if not new:
+                # If nothing is returned from update_user, don't add to github_users
+                continue
 
             # add updated user to list
             github_users.append(new)
 
             # if updated, add to updates
             if new != user:
                 updates.append(new)
 
         if self.verbose:
-            print('Updated {} GitHub Users.'.format(len(updates)))
+            print(f"Updated {len(updates)} GitHub Users.")
 
         return github_users
```

