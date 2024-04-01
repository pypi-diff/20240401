# Comparing `tmp/winzig-0.2.7.tar.gz` & `tmp/winzig-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winzig-0.2.7.tar", max compression
+gzip compressed data, was "winzig-0.2.8.tar", max compression
```

## Comparing `winzig-0.2.7.tar` & `winzig-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1051 2024-03-13 16:34:56.468996 winzig-0.2.7/LICENSE
--rw-r--r--   0        0        0     6858 2024-03-24 15:09:36.698910 winzig-0.2.7/README.md
--rw-r--r--   0        0        0      870 2024-03-24 15:37:07.554964 winzig-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-10 23:01:38.883435 winzig-0.2.7/winzig/__init__.py
--rw-r--r--   0        0        0      124 2024-03-23 19:58:14.447350 winzig-0.2.7/winzig/commands/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-23 20:22:28.823153 winzig-0.2.7/winzig/commands/crawl.py
--rw-r--r--   0        0        0     1469 2024-03-23 20:28:31.508519 winzig-0.2.7/winzig/commands/search.py
--rw-r--r--   0        0        0      457 2024-03-23 20:23:25.839389 winzig-0.2.7/winzig/commands/tui.py
--rw-r--r--   0        0        0      585 2024-03-19 16:19:26.741566 winzig-0.2.7/winzig/config.py
--rw-r--r--   0        0        0       54 2024-03-22 17:22:38.871866 winzig-0.2.7/winzig/console.py
--rw-r--r--   0        0        0     6564 2024-03-24 15:35:59.451233 winzig-0.2.7/winzig/crawler.py
--rw-r--r--   0        0        0      487 2024-03-19 16:19:26.741566 winzig-0.2.7/winzig/database.py
--rw-r--r--   0        0        0      508 2024-03-23 20:41:27.782850 winzig-0.2.7/winzig/main.py
--rw-r--r--   0        0        0     1532 2024-03-24 15:36:21.695142 winzig-0.2.7/winzig/models.py
--rw-r--r--   0        0        0     2629 2024-03-23 11:43:24.146280 winzig-0.2.7/winzig/search_engine.py
--rw-r--r--   0        0        0     1454 2024-03-22 18:37:02.319908 winzig-0.2.7/winzig/tf_idf.py
--rw-r--r--   0        0        0     2627 2024-03-24 14:41:48.574090 winzig-0.2.7/winzig/tui.py
--rw-r--r--   0        0        0      137 2024-03-23 10:58:50.710710 winzig-0.2.7/winzig/tui.tcss
--rw-r--r--   0        0        0      835 2024-03-23 11:33:21.553129 winzig-0.2.7/winzig/utils.py
--rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 winzig-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1051 2024-03-13 16:34:56.468996 winzig-0.2.8/LICENSE
+-rw-r--r--   0        0        0     6858 2024-03-24 15:09:36.698910 winzig-0.2.8/README.md
+-rw-r--r--   0        0        0      870 2024-03-25 07:45:22.291470 winzig-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-10 23:01:38.883435 winzig-0.2.8/winzig/__init__.py
+-rw-r--r--   0        0        0      124 2024-03-23 19:58:14.447350 winzig-0.2.8/winzig/commands/__init__.py
+-rw-r--r--   0        0        0     1940 2024-03-25 07:17:53.912980 winzig-0.2.8/winzig/commands/crawl.py
+-rw-r--r--   0        0        0     1469 2024-03-23 20:28:31.508519 winzig-0.2.8/winzig/commands/search.py
+-rw-r--r--   0        0        0      457 2024-03-23 20:23:25.839389 winzig-0.2.8/winzig/commands/tui.py
+-rw-r--r--   0        0        0      585 2024-03-19 16:19:26.741566 winzig-0.2.8/winzig/config.py
+-rw-r--r--   0        0        0       54 2024-03-22 17:22:38.871866 winzig-0.2.8/winzig/console.py
+-rw-r--r--   0        0        0     6857 2024-03-25 07:15:48.525956 winzig-0.2.8/winzig/crawler.py
+-rw-r--r--   0        0        0      487 2024-03-19 16:19:26.741566 winzig-0.2.8/winzig/database.py
+-rw-r--r--   0        0        0      508 2024-03-23 20:41:27.782850 winzig-0.2.8/winzig/main.py
+-rw-r--r--   0        0        0     1532 2024-03-25 07:26:59.406254 winzig-0.2.8/winzig/models.py
+-rw-r--r--   0        0        0     2629 2024-03-23 11:43:24.146280 winzig-0.2.8/winzig/search_engine.py
+-rw-r--r--   0        0        0     1454 2024-03-22 18:37:02.319908 winzig-0.2.8/winzig/tf_idf.py
+-rw-r--r--   0        0        0     2627 2024-03-24 14:41:48.574090 winzig-0.2.8/winzig/tui.py
+-rw-r--r--   0        0        0      137 2024-03-23 10:58:50.710710 winzig-0.2.8/winzig/tui.tcss
+-rw-r--r--   0        0        0      835 2024-03-23 11:33:21.553129 winzig-0.2.8/winzig/utils.py
+-rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 winzig-0.2.8/PKG-INFO
```

### Comparing `winzig-0.2.7/LICENSE` & `winzig-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/README.md` & `winzig-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/pyproject.toml` & `winzig-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "winzig"
-version = "0.2.7"
+version = "0.2.8"
 description = "A tiny search engine for personal use."
 authors = ["dnlzrgz <24715931+dnlzrgz@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dnlzrgz/winzig"
 keywords = ["search", "crawl", "sqlite", "async", "feeds"]
```

### Comparing `winzig-0.2.7/winzig/commands/crawl.py` & `winzig-0.2.8/winzig/commands/crawl.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,47 @@
 @click.group(
     invoke_without_command=True,
     help="Crawl and extract content from feeds and posts. If no subcommand is provided, it automatically crawls previously saved feeds by default.",
 )
 @click.pass_context
 def crawl(ctx):
     if ctx.invoked_subcommand is None:
-        asyncio.run(_crawl_feeds(ctx.obj["engine"], None))
+        asyncio.run(_crawl_feeds(ctx.obj["engine"], None, None))
 
 
 @click.command(
     name="feeds",
     help="Crawl and extract content from the posts of the specified feeds.",
 )
 @click.option(
     "-f",
     "--file",
     type=Path,
     default=None,
     help="Path to the file containing feed sources. If empty, previous feeds added to the database will be used.",
 )
+@click.option(
+    "-m",
+    "--max",
+    type=int,
+    default=None,
+    help="Maximum number of posts to crawl from each feed.",
+)
 @click.pass_context
-def crawl_feeds(ctx, file: Path):
-    asyncio.run(_crawl_feeds(ctx.obj["engine"], file))
+def crawl_feeds(ctx, file: Path, max: int):
+    asyncio.run(_crawl_feeds(ctx.obj["engine"], file, max))
 
 
-async def _crawl_feeds(engine, file: Path | None):
+async def _crawl_feeds(engine, file: Path | None, max: int | None):
     async with AsyncSession(engine) as session:
-        await crawl_from_feeds(session, file)
+        await crawl_from_feeds(
+            session,
+            file,
+            max,
+        )
         await recalculate_tf_idf(session)
 
 
 @click.command(
     name="posts",
     help="Crawl and extract content from the posts specified in a file.",
 )
```

### Comparing `winzig-0.2.7/winzig/commands/search.py` & `winzig-0.2.8/winzig/commands/search.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/winzig/config.py` & `winzig-0.2.8/winzig/config.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/winzig/crawler.py` & `winzig-0.2.8/winzig/crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,23 +56,34 @@
         feed = feedparser.parse(url)
         return True if feed.version else False
     except Exception as e:
         console.log(f"[red bold]Error[/red bold]: Parsing feed '{url}': {e}")
         return False
 
 
-async def get_posts_from_feed(session: AsyncSession, id: int, url: str) -> list[str]:
+async def get_posts_from_feed(
+    session: AsyncSession, feed_id: int, url: str, max: int | None
+) -> list[str]:
     try:
         feed = feedparser.parse(url)
-        statement = select(Post).where(Post.feed_id == id)
+        statement = select(Post).where(Post.feed_id == feed_id)
         results = await session.execute(statement)
         results = results.scalars()
         posts_db_urls = {post.url for post in results}
 
-        return [entry.link for entry in feed.entries if entry.link not in posts_db_urls]
+        if max:
+            return [
+                entry.link
+                for entry in feed.entries[:max]
+                if entry.link not in posts_db_urls
+            ]
+        else:
+            return [
+                entry.link for entry in feed.entries if entry.link not in posts_db_urls
+            ]
     except Exception as e:
         console.log(f"[red bold]Error[/red bold]: Parsing feed '{url}': {e}")
         return []
 
 
 async def process_post(
     session: AsyncSession,
@@ -163,28 +174,30 @@
                 status.update("Fetching posts...")
                 await asyncio.gather(*tasks)
                 await session.commit()
 
         console.log("[green bold]SUCCESS[/green bold]: Posts fetched")
 
 
-async def crawl_from_feeds(session: AsyncSession, file: Path | None = None):
+async def crawl_from_feeds(
+    session: AsyncSession, file: Path | None = None, max: int | None = None
+):
     if file is not None:
         await add_feeds_from_file(session, file)
 
     feeds = await session.execute(select(Feed))
     feeds = feeds.scalars().all()
     if not feeds:
         console.log("[red]Error[/red]: No feeds found!")
         return
 
     async with httpx.AsyncClient(headers=headers, follow_redirects=True) as client:
         with console.status("Fetching posts...", spinner="earth") as status:
             for idx, feed in enumerate(feeds):
-                posts = await get_posts_from_feed(session, feed.id, feed.url)
+                posts = await get_posts_from_feed(session, feed.id, feed.url, max)
                 tasks = [process_post(session, client, feed, post) for post in posts]
 
                 status.update(
                     f"[bold][{idx + 1}/{len(feeds)}][/bold] Fetching posts from '{feed.url}'"
                 )
                 await asyncio.gather(*tasks)
```

### Comparing `winzig-0.2.7/winzig/models.py` & `winzig-0.2.8/winzig/models.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/winzig/search_engine.py` & `winzig-0.2.8/winzig/search_engine.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/winzig/tf_idf.py` & `winzig-0.2.8/winzig/tf_idf.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/winzig/tui.py` & `winzig-0.2.8/winzig/tui.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/winzig/utils.py` & `winzig-0.2.8/winzig/utils.py`

 * *Files identical despite different names*

### Comparing `winzig-0.2.7/PKG-INFO` & `winzig-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winzig
-Version: 0.2.7
+Version: 0.2.8
 Summary: A tiny search engine for personal use.
 Home-page: https://github.com/dnlzrgz/winzig
 License: MIT
 Keywords: search,crawl,sqlite,async,feeds
 Author: dnlzrgz
 Author-email: 24715931+dnlzrgz@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
```

