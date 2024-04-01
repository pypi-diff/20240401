# Comparing `tmp/uwsgitop-0.8.tar.gz` & `tmp/uwsgitop-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uwsgitop-0.8.tar", last modified: Fri Feb 28 05:56:49 2014, max compression
+gzip compressed data, was "dist/uwsgitop-0.9.tar", last modified: Fri Oct  9 15:49:45 2015, max compression
```

## Comparing `uwsgitop-0.8.tar` & `uwsgitop-0.9.tar`

### file list

```diff
@@ -1,5 +1,13 @@
-drwxr-xr-x   0 roberta    (501) staff       (20)        0 2014-02-28 05:56:49.000000 uwsgitop-0.8/
--rw-r--r--   0 roberta    (501) staff       (20)      197 2014-02-28 05:56:49.000000 uwsgitop-0.8/PKG-INFO
--rw-r--r--   0 roberta    (501) staff       (20)      397 2014-02-28 05:51:57.000000 uwsgitop-0.8/README
--rw-r--r--   0 roberta    (501) staff       (20)      210 2014-02-28 05:51:57.000000 uwsgitop-0.8/setup.py
--rw-r--r--   0 roberta    (501) staff       (20)     8252 2014-02-28 05:51:57.000000 uwsgitop-0.8/uwsgitop
+drwxr-xr-x   0 rm        (1000) rm        (1000)        0 2015-10-09 15:49:45.000000 uwsgitop-0.9/
+-rw-r--r--   0 rm        (1000) rm        (1000)     3628 2015-10-09 15:49:45.000000 uwsgitop-0.9/PKG-INFO
+-rw-r--r--   0 rm        (1000) rm        (1000)     9401 2015-10-09 15:39:06.000000 uwsgitop-0.9/uwsgitop
+-rw-r--r--   0 rm        (1000) rm        (1000)      422 2015-10-09 15:46:55.000000 uwsgitop-0.9/setup.py
+-rw-r--r--   0 rm        (1000) rm        (1000)       59 2015-10-09 15:49:45.000000 uwsgitop-0.9/setup.cfg
+drwxr-xr-x   0 rm        (1000) rm        (1000)        0 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/
+-rw-r--r--   0 rm        (1000) rm        (1000)       11 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/requires.txt
+-rw-r--r--   0 rm        (1000) rm        (1000)       47 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/pbr.json
+-rw-r--r--   0 rm        (1000) rm        (1000)     3628 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/PKG-INFO
+-rw-r--r--   0 rm        (1000) rm        (1000)      214 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/SOURCES.txt
+-rw-r--r--   0 rm        (1000) rm        (1000)        1 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/top_level.txt
+-rw-r--r--   0 rm        (1000) rm        (1000)        1 2015-10-09 15:49:45.000000 uwsgitop-0.9/uwsgitop.egg-info/dependency_links.txt
+-rw-r--r--   0 rm        (1000) rm        (1000)     2906 2015-10-06 18:59:44.000000 uwsgitop-0.9/README.rst
```

### Comparing `uwsgitop-0.8/uwsgitop` & `uwsgitop-0.9/uwsgitop`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#!python
+#!/usr/bin/env python
 
 import socket
 try:
     import simplejson as json
 except ImportError:
     import json
 import curses
 import time
 import atexit
 import sys
 import traceback
 from collections import defaultdict
+import errno
 
 need_reset = True
 screen = None
 
 def human_size(n):
     # G
     if n >= (1024*1024*1024): 
@@ -26,61 +27,81 @@
     if n >= 1024:
         return "%.1fK" % (n/1024)
     return "%d" % n
 
 def game_over():
     global need_reset
     if need_reset:
+        curses.echo()
         curses.endwin()
 
 def exc_hook(type, value, tb):
     global need_reset, screen
     need_reset = False
     if screen:
+        curses.echo()
         curses.endwin()
     traceback.print_exception(type, value, tb)
 
 sys.excepthook = exc_hook
 
 argc = len(sys.argv)
 
 if argc < 2:
     raise Exception("You have to specify the uWSGI stats socket")
 
+def inet_addr(arg):
+    sfamily = socket.AF_INET
+    host, port = arg.rsplit(':', 1)
+    addr = (host, int(port))
+    return sfamily, addr, host
+
+def unix_addr(arg):
+    sfamily = socket.AF_UNIX
+    addr = arg
+    return sfamily, addr, socket.gethostname()
+
+def abstract_unix_addr(arg):
+    sfamily = socket.AF_UNIX
+    addr = '\0' + arg[1:]
+    return sfamily, addr, socket.gethostname()
+
 addr = sys.argv[1]
-sfamily = socket.AF_UNIX
-addr_tuple = addr
 if ':' in addr:
-    sfamily = socket.AF_INET
-    addr_parts = addr.split(':')
-    addr_tuple = (addr_parts[0], int(addr_parts[1]))
+    sfamily, addr, host = inet_addr(addr)
+elif addr.startswith('@'):
+    sfamily, addr, host = abstract_unix_addr(addr)
+else:
+    sfamily, addr, host = unix_addr(addr)
 
-freq = 3
 try:
     freq = int(sys.argv[2])
-except:
-    pass
+except IndexError:
+    freq = 1
 
 screen = curses.initscr()
+curses.noecho()
 curses.start_color()
+curses.use_default_colors()
 
 try:
     # busy
-    curses.init_pair(1, curses.COLOR_GREEN, curses.COLOR_BLACK)
+    curses.init_pair(1, curses.COLOR_GREEN, -1)
     # cheap
-    curses.init_pair(2, curses.COLOR_MAGENTA, curses.COLOR_BLACK)
-    # pause
-    curses.init_pair(3, curses.COLOR_RED, curses.COLOR_BLACK)
+    curses.init_pair(2, curses.COLOR_MAGENTA, -1)
+    # respawn
+    curses.init_pair(3, curses.COLOR_RED, -1)
     # sig
-    curses.init_pair(4, curses.COLOR_YELLOW, curses.COLOR_BLACK)
+    curses.init_pair(4, curses.COLOR_YELLOW, -1)
+    # pause
+    curses.init_pair(5, curses.COLOR_BLUE, -1)
 except curses.error:
     # the terminal doesn't support colors
     pass
 
-screen.timeout(freq*1000)
 atexit.register(game_over)
 
 try:
     curses.curs_set(0)
 except:
     pass
 screen.clear()
@@ -114,30 +135,40 @@
 last_reqnumber_per_worker = defaultdict(int)
 last_reqnumber_per_core = defaultdict(int)
 
 # 0 - do not show async core
 # 1 - merge core statistics with worker statistics
 # 2 - display active cores under workers
 async_mode = 0
+fast_screen = 0
 
 while True:
 
+    if fast_screen == 1:
+        screen.timeout(100)
+    else:
+        screen.timeout(freq*1000)
+
     screen.clear()
 
     js = ''
 
     try:
         s = socket.socket(sfamily, socket.SOCK_STREAM)
-        s.connect( addr_tuple )
+        s.connect( addr )
 
         while True:
             data = s.recv(4096)
             if len(data) < 1:
                 break
             js += data.decode('utf8')
+    except IOError as e:
+        if e.errno != errno.EINTR:
+            raise
+        continue
     except:
         raise Exception("unable to get uWSGI statistics")
 
     dd = json.loads(js)
 
 
     
@@ -160,25 +191,26 @@
     if 'gid' in dd:
         gid = "- gid: %d" % dd['gid'] 
 
     masterpid = ""
     if 'pid' in dd:
         masterpid = "- masterpid: %d" % dd['pid'] 
 
-    screen.addstr(1, 0, "node: %s %s %s %s %s" % (socket.gethostname(), cwd, uid, gid, masterpid))
+    screen.addstr(1, 0, "node: %s %s %s %s %s" % (host, cwd, uid, gid, masterpid))
 
     if 'vassals' in dd:
         screen.addstr(0, 0, "uwsgi%s - %s - emperor: %s - tyrant: %d" % (uversion, time.ctime(), dd['emperor'], dd['emperor_tyrant']))
-        vassal_spaces = max([len(v['id']) for v in dd['vassals']])
-        screen.addstr(2, 0, " VASSAL%s\tPID\t" % (' ' * (vassal_spaces-6)), curses.A_REVERSE)
-        pos = 3
-        for vassal in dd['vassals']:
-            screen.addstr(pos, 0, " %s\t%d" % (vassal['id'].ljust(vassal_spaces), vassal['pid']))
-            pos += 1
-    
+        if dd['vassals']:
+            vassal_spaces = max([len(v['id']) for v in dd['vassals']])
+            screen.addstr(2, 0, " VASSAL%s\tPID\t" % (' ' * (vassal_spaces-6)), curses.A_REVERSE)
+            pos = 3
+            for vassal in dd['vassals']:
+                screen.addstr(pos, 0, " %s\t%d" % (vassal['id'].ljust(vassal_spaces), vassal['pid']))
+                pos += 1
+
     elif 'workers' in dd:
         tot = sum( [worker['requests'] for worker in dd['workers']] )
 
         rps_per_worker = {}
         rps_per_core = {}
         cores = defaultdict(list)
         dt = time.time() - last_tot_time
@@ -208,49 +240,55 @@
 
         if async_mode == 1:
             merge_worker_with_cores(dd['workers'], rps_per_worker,
                                     cores, rps_per_core)
 
         tx = human_size(sum( [worker['tx'] for worker in dd['workers']] ))
         screen.addstr(0, 0, "uwsgi%s - %s - req: %d - RPS: %d - lq: %d - tx: %s" % (uversion, time.ctime(), tot, int(round(total_rps)), dd['listen_queue'], tx))
-        screen.addstr(2, 0, " WID\t%\tPID\tREQ\tRPS\tEXC\tSIG\tSTATUS\tAVG\tRSS\tVSZ\tTX\tRunT\t", curses.A_REVERSE)
+        screen.addstr(2, 0, " WID\t%\tPID\tREQ\tRPS\tEXC\tSIG\tSTATUS\tAVG\tRSS\tVSZ\tTX\tReSpwn\tHC\tRunT\tLastSpwn", curses.A_REVERSE)
         pos = 3
 
-        dd['workers'].sort(key=reqcount)
+        dd['workers'].sort(key=reqcount, reverse=True)
         for worker in dd['workers']:
             sigs = 0
             wtx = human_size(worker['tx'])
+            wlastspawn = "--:--:--"
 
             wrunt = worker['running_time']/1000
             if wrunt > 9999999:
                 wrunt = "%sm" % str(wrunt / (1000*60))
             else:
                 wrunt = str(wrunt)
+
+            if worker['last_spawn']:
+                wlastspawn = time.strftime("%H:%M:%S", time.localtime(worker['last_spawn']))
                 
             color = curses.color_pair(0)
             if 'signals' in worker:
                 sigs = worker['signals']
             if worker['status'] == 'busy':
                 color = curses.color_pair(1)
             if worker['status'] == 'cheap':
                 color = curses.color_pair(2)
-            if worker['status'] == 'pause':
+            if worker['rss'] == 0:
                 color = curses.color_pair(3)
             if worker['status'].startswith('sig'):
                 color = curses.color_pair(4)
+            if worker['status'] == 'pause':
+                color = curses.color_pair(5)
 
             wid = worker['id']
 
             rps = int(round(rps_per_worker[wid]))
 
             try:
-                screen.addstr(pos, 0, " %s\t%.1f\t%d\t%d\t%d\t%d\t%d\t%s\t%dms\t%s\t%s\t%s\t%s" % (
+                screen.addstr(pos, 0, " %s\t%.1f\t%d\t%d\t%d\t%d\t%d\t%s\t%dms\t%s\t%s\t%s\t%s\t%s\t%s\t%s" % (
                     wid, calc_percent(tot, worker['requests']),  worker['pid'], worker['requests'], rps, worker['exceptions'], sigs, worker['status'],
                     worker['avg_rt']/1000, human_size(worker['rss']), human_size(worker['vsz']),
-                    wtx, wrunt
+                    wtx, worker['respawn_count'], worker['harakiri_count'], wrunt, wlastspawn
                 ), color)
             except:
                 pass
             pos += 1
             if async_mode != 2:
                 continue
             for core in cores[wid]:
@@ -276,9 +314,11 @@
     s.close()
     ch = screen.getch()
     if ch == ord('q'):
         game_over()
         break
     elif ch == ord('a'):
         async_mode = (async_mode + 1) % 3
+    elif ch == ord('f'):
+        fast_screen = (fast_screen + 1) % 2
```

