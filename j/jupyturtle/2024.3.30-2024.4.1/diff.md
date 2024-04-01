# Comparing `tmp/jupyturtle-2024.3.30.tar.gz` & `tmp/jupyturtle-2024.4.1.tar.gz`

## Comparing `jupyturtle-2024.3.30.tar` & `jupyturtle-2024.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0   125505 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/notebooks/ThinkPythonChap04.ipynb
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/notebooks/arc-lab.ipynb
--rw-r--r--   0        0        0    83528 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/notebooks/command-ref.ipynb
--rw-r--r--   0        0        0   184849 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/notebooks/gallery.ipynb
--rw-r--r--   0        0        0    29763 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/notebooks/lab.ipynb
--rw-r--r--   0        0        0    22570 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/notebooks/magic-lab.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/src/jupyturtle/__init__.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/src/jupyturtle/jupyturtle.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/tests/jupyturtle_test.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/LICENSE
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/README.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/pyproject.toml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 jupyturtle-2024.3.30/PKG-INFO
+-rw-r--r--   0        0        0   125484 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/notebooks/ThinkPythonChap04.ipynb
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/notebooks/arc-lab.ipynb
+-rw-r--r--   0        0        0    88658 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/notebooks/command-ref.ipynb
+-rw-r--r--   0        0        0   233665 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/notebooks/gallery.ipynb
+-rw-r--r--   0        0        0    31334 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/notebooks/lab.ipynb
+-rw-r--r--   0        0        0    22733 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/notebooks/magic-lab.ipynb
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/src/jupyturtle/__init__.py
+-rw-r--r--   0        0        0    13791 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/src/jupyturtle/jupyturtle.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/tests/jupyturtle_test.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/README.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 jupyturtle-2024.4.1/PKG-INFO
```

### Comparing `jupyturtle-2024.3.30/notebooks/ThinkPythonChap04.ipynb` & `jupyturtle-2024.4.1/notebooks/ThinkPythonChap04.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971050870147256%*

 * *Differences: {"'cells'": "{51: {'execution_count': 33}, 53: {'execution_count': 34}, 54: {'execution_count': "*

 * *            "35}, 56: {'execution_count': 36}, 57: {'execution_count': 37}, 59: "*

 * *            "{'execution_count': 38}, 60: {'execution_count': 39}, 61: {'execution_count': 40}, "*

 * *            "62: {'execution_count': 41}, 64: {'execution_count': 42}, 66: {'execution_count': "*

 * *            "43}, 67: {'execution_count': 44}, 68: {'execution_count': 45}, 69: "*

 * *            "{'execution_count': 46}, 71: {'execution_c […]*

```diff
@@ -929,15 +929,15 @@
                 "## Exercises\n",
                 "\n",
                 "`penup` and `pendown`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 33,
             "id": "6f9a0106",
             "metadata": {
                 "id": "6f9a0106"
             },
             "outputs": [],
             "source": [
                 "from jupyturtle import forward, penup, pendown\n",
@@ -962,15 +962,15 @@
                 "### Exercise\n",
                 "\n",
                 "Draw a rectangle:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 34,
             "id": "c54ba660",
             "metadata": {
                 "id": "c54ba660"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -986,15 +986,15 @@
                 "        left(90)\n",
                 "        forward(length2)\n",
                 "        left(90)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 35,
             "id": "1311ee08",
             "metadata": {
                 "id": "1311ee08",
                 "outputId": "f73e1eaf-e057-4099-8d25-45fc326b491a"
             },
             "outputs": [
                 {
@@ -1036,15 +1036,15 @@
                 "### Exercise\n",
                 "\n",
                 "Draw a rhombus:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 36,
             "id": "3db6f106",
             "metadata": {
                 "id": "3db6f106"
             },
             "outputs": [],
             "source": [
                 "def rhombus(length, angle):\n",
@@ -1053,15 +1053,15 @@
                 "        left(angle)\n",
                 "        forward(length)\n",
                 "        left(180-angle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 37,
             "id": "1d845de9",
             "metadata": {
                 "id": "1d845de9",
                 "outputId": "66e0bd71-a207-482a-c855-184f9603b6b5"
             },
             "outputs": [
                 {
@@ -1103,15 +1103,15 @@
                 "### Exercise\n",
                 "\n",
                 "Write `parallelogram`, then rewrite `rectangle` and `rhombus` to use it:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 38,
             "id": "895005cb",
             "metadata": {
                 "id": "895005cb"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -1122,15 +1122,15 @@
                 "        left(angle)\n",
                 "        forward(length2)\n",
                 "        left(180-angle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 39,
             "id": "7e7d34b0",
             "metadata": {
                 "id": "7e7d34b0"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -1142,30 +1142,30 @@
                 "    length2: length of the second size\n",
                 "    \"\"\"\n",
                 "    parallelogram(length1, length2, 90)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 40,
             "id": "481396f9",
             "metadata": {
                 "id": "481396f9"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
                 "\n",
                 "def rhombus(length, angle):\n",
                 "    parallelogram(length, length, angle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 41,
             "id": "c8dfebc9",
             "metadata": {
                 "id": "c8dfebc9",
                 "outputId": "a6b35bd8-69c7-44ed-cb5f-c540b8abacd8"
             },
             "outputs": [
                 {
@@ -1217,15 +1217,15 @@
                 "### Exercise\n",
                 "\n",
                 "A `triangle` function:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 42,
             "id": "8be6442e",
             "metadata": {
                 "id": "8be6442e"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -1258,15 +1258,15 @@
             "metadata": {},
             "source": [
                 "(a little demonstration)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 43,
             "id": "2666dcde",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -1293,15 +1293,15 @@
                 "for i in range(12):\n",
                 "    triangle(50, 10)\n",
                 "    left(30)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 44,
             "id": "be1b7ed8",
             "metadata": {
                 "id": "be1b7ed8"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -1316,15 +1316,15 @@
                 "    for i in range(n):\n",
                 "        triangle(radius,  angle/2)\n",
                 "        left(angle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 45,
             "id": "9b1f5a1e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -1351,15 +1351,15 @@
             "source": [
                 "make_turtle(delay=0.01)\n",
                 "draw_pie(5, 40)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 46,
             "id": "89ce198a",
             "metadata": {
                 "id": "89ce198a",
                 "outputId": "252a28de-d853-4851-abb0-525ea33c0998"
             },
             "outputs": [
                 {
@@ -1418,15 +1418,15 @@
                 "### Exercise\n",
                 "\n",
                 "Draw flowers with `petal`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 47,
             "id": "0f0e7498",
             "metadata": {
                 "id": "0f0e7498"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -1441,15 +1441,15 @@
                 "    for i in range(2):\n",
                 "        arc(radius,  angle)\n",
                 "        left(180-angle)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": 48,
             "id": "6c0d0bff",
             "metadata": {
                 "id": "6c0d0bff"
             },
             "outputs": [],
             "source": [
                 "# Solution\n",
@@ -1464,15 +1464,15 @@
                 "    for i in range(n):\n",
                 "        petal(radius,  angle)\n",
                 "        left(360/n)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 49,
             "id": "2f4b4c22-198d-4e30-8d38-68d04023309a",
             "metadata": {
                 "id": "4cfea3b0",
                 "outputId": "cb03438b-e82a-4c35-97dc-884bfde25056"
             },
             "outputs": [
                 {
@@ -1525,15 +1525,15 @@
             "source": [
                 "For faster results, set `animate` to `False`.\n",
                 "The drawing will only be rendered when you call `draw()`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 50,
             "id": "c9a31629-d57b-4b1a-b146-4766a799d119",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -1578,15 +1578,15 @@
                 "In this case, the `animate` setting is preserved but\n",
                 "set to `False` within the block.\n",
                 "The `delay` has no effect within the block."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 51,
             "id": "442e5e7d-c00f-441a-b9e5-67774a8c9d13",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -1626,15 +1626,15 @@
                 "### Ask an assistant\n",
                 "\n",
                 "Draw a spiral:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 52,
             "id": "46d3151c",
             "metadata": {
                 "id": "46d3151c",
                 "outputId": "47731432-91f7-4efc-d6da-077dd95234f8"
             },
             "outputs": [
                 {
@@ -1675,15 +1675,15 @@
                 "        length += 2  # Increase the length for each segment\n",
                 "\n",
                 "spiral(5, 90)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": 53,
             "id": "186c7fbc",
             "metadata": {
                 "id": "186c7fbc",
                 "outputId": "45628c53-a3b4-482e-dbf0-32a4ac0edaf9"
             },
             "outputs": [
                 {
@@ -1738,15 +1738,15 @@
                 "\n",
                 "circular_spiral(50, 1)\n",
                 "print('done')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 54,
             "id": "0cd5b7e3-ccaf-4954-bca0-ccebd10bfbc7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"550\" height=\"550\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -1777,27 +1777,26 @@
                 "\n",
                 "# quick version\n",
                 "from jupyturtle import no_pen\n",
                 "\n",
                 "make_turtle(animate=False, width=550, height=550)\n",
                 "\n",
                 "with no_pen():\n",
-                "    penup()\n",
                 "    rt(90)\n",
                 "    fd(150)\n",
                 "    lt(90)\n",
                 "\n",
                 "circular_spiral(500, 3)\n",
                 "draw()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3350ce5a-82e0-4ec0-94a5-37373a1f0156",
+            "id": "bdd0745c-df4b-4593-be3b-da0a6633c0db",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "celltoolbar": "Tags",
```

### Comparing `jupyturtle-2024.3.30/notebooks/arc-lab.ipynb` & `jupyturtle-2024.4.1/notebooks/arc-lab.ipynb`

 * *Files identical despite different names*

### Comparing `jupyturtle-2024.3.30/notebooks/command-ref.ipynb` & `jupyturtle-2024.4.1/notebooks/command-ref.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835706794282375%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '#### [`back`](#forward(n);-back(n)-—-aliases-fd;-bk) "*

 * *            '[`bk`](#forward(n);-back(n)-—-aliases-fd;-bk) [`draw`](#draw()) '*

 * *            '[`forward`](#forward(n);-back(n)-—-aliases-fd;-bk) '*

 * *            '[`fd`](#forward(n);-back(n)-—-aliases-fd;-bk) [`get_turtle`](#get_turtle()) '*

 * *            '[`hide`](#hide()) [`jump_to`](#jump_to()) '*

 * *            '[`left`](#left(n);-right(n)-—-aliases-lt;-rt) '*

 * *            '[`lt`](#left(n);-right(n)-—-aliases-lt;-rt) [`m […]*

```diff
@@ -3,16 +3,16 @@
         {
             "cell_type": "markdown",
             "id": "9ab72fcd-c8ec-4338-b492-1b13f6a6f7f9",
             "metadata": {},
             "source": [
                 "# Turtle command reference\n",
                 "\n",
-                "#### [`back`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`bk`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`forward`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`fd`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`get_turtle`](#get_turtle()) [`hide`](#hide()) [`jumpto`](#jumpto()) [`left`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`lt`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`make_turtle`](#get_turtle())\n",
-                "#### [`moveto`](#moveto()) [`no_pen`](#no_pen()) [`pendown`](#pendown()) [`penup`](#penup()) [`render`](#draw()) [`right`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`rt`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`set_color`](#set_color(color)) [`set_width`](#set_width(n))  [`show`](#show()) [`toggle_pen`](#toggle_pen())"
+                "#### [`back`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`bk`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`draw`](#draw()) [`forward`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`fd`](#forward(n);-back(n)-\u2014-aliases-fd;-bk) [`get_turtle`](#get_turtle()) [`hide`](#hide()) [`jump_to`](#jump_to()) [`left`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`lt`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`make_turtle`](#make_turtle()) [`move_to`](#move_to()) \n",
+                "#### [`no_pen`](#no_pen()) [`pen_down`](#pen_down()) [`pen_up`](#pen_up()) [`right`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`rt`](#left(n);-right(n)-\u2014-aliases-lt;-rt) [`set_color`](#set_color(color)) [`set_width`](#set_width(n))  [`show`](#show()) [`toggle_pen`](#toggle_pen()) [`%%turtle`](#%25%25turtle)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5009dbfb-670b-4807-81cb-45d03fb384c7",
             "metadata": {},
             "source": [
@@ -184,25 +184,71 @@
                 "fd(50)\n",
                 "bk(75)\n",
                 "fd(25)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "829724e9-593c-45c3-b0b7-b8d6fde7d7a3",
+            "metadata": {},
+            "source": [
+                "If two numbers `a`, `b` are given, move forward `a` units then turn left `b` degrees. Use negative degrees to turn right."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "d99fbc7d-b8c9-4b7c-b1d6-90975e446190",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
+                            "    <rect width=\"100%\" height=\"100%\" fill=\"#F3F3F7\" />\n",
+                            "\n",
+                            "\n",
+                            "<path stroke=\"#663399\" stroke-width=\"2\" d=\"M 150,75 220,75 185,14.4 150,75\" />'\n",
+                            "\n",
+                            "<g transform=\"rotate(-90.0,150.0,75.0) translate(150.0, 75.0)\">\n",
+                            "    <circle stroke=\"#63A375\" stroke-width=\"2\" fill=\"transparent\" r=\"5.5\" cx=\"0\" cy=\"0\"/>\n",
+                            "    <polygon points=\"0,12 2,9 -2,9\" style=\"fill:#63A375;stroke:#63A375;stroke-width:2\"/>\n",
+                            "</g>\n",
+                            "\n",
+                            "</svg>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "make_turtle()\n",
+                "\n",
+                "fd(70, 120)\n",
+                "fd(70, 120)\n",
+                "fd(70, 120)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "0c4c2dc0-5d63-4b2b-b95b-6a948e1fc5cc",
             "metadata": {},
             "source": [
                 "### `left(n)`; `right(n)` \u2014 aliases `lt`; `rt`\n",
                 "\n",
                 "Turn turtle left or right `n` degrees, remaining in place."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "c373365e-ce43-4bdf-bb4a-5755344e586d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -233,22 +279,22 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "39f11122-d702-497a-a4c1-2abdb813ce4a",
             "metadata": {},
             "source": [
-                "### `penup()`; `pendown()`\n",
+                "### `pen_up()`; `pen_down()`\n",
                 "\n",
                 "Raise or lower the turtle's pen. The turtle leaves a trail only when the pen is down (the default)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "id": "119f7479-3829-40bb-b5ce-c0bb99523dc4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -281,17 +327,17 @@
                 }
             ],
             "source": [
                 "make_turtle()\n",
                 "\n",
                 "for _ in range(4):\n",
                 "    fd(10)\n",
-                "    penup()\n",
+                "    pen_up()\n",
                 "    fd(20)\n",
-                "    pendown()"
+                "    pen_down()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7fdfb5fb-f766-40ba-9531-55af0faed716",
             "metadata": {},
             "source": [
@@ -299,23 +345,23 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "82a5c39c-7b96-4c08-a7e1-5170666b8d48",
             "metadata": {},
             "source": [
-                "Returs a context manager that calls `penup()` at the top of the `with` block\n",
+                "Returs a context manager that calls `pen_up()` at the top of the `with` block\n",
                 "and resets the pen to its previous state at the end of the block.\n",
                 "\n",
                 "This is useful to move the turtle without drawing for a few steps."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "id": "cd28cd07-9373-466a-8030-dbb06b938c2d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -359,22 +405,22 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "20fd626d-b6d1-4e69-9362-ee5fc04469c2",
             "metadata": {},
             "source": [
-                "### toggle_pen()\n",
+                "### `toggle_pen()`\n",
                 "\n",
                 "Lower the pen if it's up; raises it if it's down."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "id": "a349cc89-b669-4801-b26f-5a0c2b0df24e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -440,15 +486,15 @@
             "metadata": {},
             "source": [
                 "Make the turtle invisible or visible. The turtle is visible by default. Making it invisible speeds up drawing."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "b674e05e-fe12-458d-912b-d50f9a74f29a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -495,15 +541,15 @@
                 "\n",
                 "The `delay` is ignored when `animate` is `False`, \n",
                 "because the drawing will only be updated once, after a call to `draw()`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "11cf07ae-f313-43ca-a617-1879b6c46f52",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -535,16 +581,15 @@
                 }
             ],
             "source": [
                 "make_turtle(delay=5, animate=False, height=240, width=240)\n",
                 "\n",
                 "def circle():\n",
                 "    for _ in range(180):\n",
-                "        fd(2)\n",
-                "        lt(2)\n",
+                "        fd(2, 2)\n",
                 "\n",
                 "for _ in range(24):\n",
                 "    circle()\n",
                 "    lt(15)\n",
                 "\n",
                 "draw()"
             ]
@@ -558,15 +603,15 @@
                 "The drawing below will be updated at 361 times: 180 updates per circle, plus the update of `lt(15)`.\n",
                 "\n",
                 "> **Note**: The `jupyturtle` Python code generates the drawing as SVG code, which is then rendered by the browser's graphic engine. For each update, automatic or not, a complete new drawing is generated and rendered."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "id": "2206c253-c5ba-4b74-a7da-c0fcf1a5a72d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"240\" height=\"240\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -591,31 +636,103 @@
                 }
             ],
             "source": [
                 "make_turtle(delay=0, height=240, width=240)\n",
                 "\n",
                 "def circle():\n",
                 "    for _ in range(180):\n",
-                "        fd(2)\n",
-                "        lt(2)\n",
+                "        fd(2, 2)\n",
                 "        \n",
                 "circle()\n",
                 "lt(15)\n",
                 "circle()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "f99595a4-3432-4ae2-b772-f3e7f72a5266",
+            "metadata": {},
+            "source": [
+                "### `%%turtle`\n",
+                "\n",
+                "A shortcut for `make_turtle()` written as a magic command at the top of a cell.\n",
+                "\n",
+                "    %%turtle arg1 arg2 arg3\n",
+                "\n",
+                "All arguments are optional.\n",
+                "\n",
+                "If one of them is the word `fast`, animation is turned off.\n",
+                "\n",
+                "If two of them are numbers, they set the drawing `width` and `height` in that order.\n",
+                "\n",
+                "If only one is a number, it sets both `width` and `height`.\n",
+                "\n",
+                "**Note**: the `%%turtle` magic is available only after you import `jupyturtle`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "7f70ee92-802c-4744-8b43-8ce0ab8772e2",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<svg width=\"75\" height=\"75\" style=\"fill:none; stroke-linecap:round;\">\n",
+                            "    <rect width=\"100%\" height=\"100%\" fill=\"#F3F3F7\" />\n",
+                            "\n",
+                            "\n",
+                            "<path stroke=\"#663399\" stroke-width=\"2\" d=\"M 37,37\" />'\n",
+                            "\n",
+                            "<path stroke=\"#663399\" stroke-width=\"2\" d=\"M 37,67 37.5,67 38,67 38.5,67 39,66.9 39.5,66.9 40,66.9 40.5,66.8 41,66.8 41.5,66.7 42,66.6 42.5,66.5 43,66.4 43.5,66.3 43.9,66.2 44.4,66.1 44.9,66 45.4,65.8 45.9,65.7 46.3,65.5 46.8,65.4 47.3,65.2 47.7,65 48.2,64.8 48.7,64.6 49.1,64.4 49.6,64.2 50,64 50.5,63.8 50.9,63.5 51.4,63.3 51.8,63 52.2,62.8 52.6,62.5 53.1,62.2 53.5,62 53.9,61.7 54.3,61.4 54.7,61.1 55.1,60.8 55.5,60.5 55.9,60.1 56.2,59.8 56.6,59.5 57,59.1 57.3,58.8 57.7,58.4 58,58.1 58.4,57.7 58.7,57.3 59,57 59.4,56.6 59.7,56.2 60,55.8 60.3,55.4 60.6,55 60.9,54.6 61.1,54.2 61.4,53.7 61.7,53.3 61.9,52.9 62.2,52.5 62.4,52 62.7,51.6 62.9,51.1 63.1,50.7 63.3,50.2 63.5,49.8 63.7,49.3 63.9,48.9 64.1,48.4 64.3,47.9 64.4,47.4 64.6,47 64.7,46.5 64.9,46 65,45.5 65.1,45 65.2,44.6 65.3,44.1 65.4,43.6 65.5,43.1 65.6,42.6 65.7,42.1 65.7,41.6 65.8,41.1 65.8,40.6 65.8,40.1 65.9,39.6 65.9,39.1 65.9,38.6 65.9,38.1 65.9,37.6 65.9,37.1 65.8,36.6 65.8,36.1 65.8,35.6 65.7,35.1 65.7,34.6 65.6,34.1 65.5,33.6 65.4,33.1 65.3,32.6 65.2,32.2 65.1,31.7 65,31.2 64.9,30.7 64.7,30.2 64.6,29.7 64.4,29.3 64.3,28.8 64.1,28.3 63.9,27.9 63.7,27.4 63.5,26.9 63.3,26.5 63.1,26 62.9,25.6 62.7,25.1 62.4,24.7 62.2,24.2 61.9,23.8 61.7,23.4 61.4,23 61.1,22.5 60.9,22.1 60.6,21.7 60.3,21.3 60,20.9 59.7,20.5 59.4,20.1 59,19.7 58.7,19.4 58.4,19 58,18.6 57.7,18.3 57.3,17.9 57,17.6 56.6,17.2 56.2,16.9 55.9,16.6 55.5,16.2 55.1,15.9 54.7,15.6 54.3,15.3 53.9,15 53.5,14.7 53.1,14.5 52.6,14.2 52.2,13.9 51.8,13.7 51.4,13.4 50.9,13.2 50.5,12.9 50,12.7 49.6,12.5 49.1,12.3 48.7,12.1 48.2,11.9 47.7,11.7 47.3,11.5 46.8,11.3 46.3,11.2 45.9,11 45.4,10.9 44.9,10.7 44.4,10.6 43.9,10.5 43.5,10.4 43,10.3 42.5,10.2 42,10.1 41.5,10 41,9.9 40.5,9.9 40,9.8 39.5,9.8 39,9.8 38.5,9.7 38,9.7 37.5,9.7\" />'\n",
+                            "\n",
+                            "<g transform=\"rotate(90.0,37.5,9.7) translate(37.5, 9.7)\">\n",
+                            "    <circle stroke=\"#63A375\" stroke-width=\"2\" fill=\"transparent\" r=\"5.5\" cx=\"0\" cy=\"0\"/>\n",
+                            "    <polygon points=\"0,12 2,9 -2,9\" style=\"fill:#63A375;stroke:#63A375;stroke-width:2\"/>\n",
+                            "</g>\n",
+                            "\n",
+                            "</svg>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "%%turtle 75 fast\n",
+                "\n",
+                "def arc(degrees):\n",
+                "    if degrees == 0: return\n",
+                "    fd(.5)\n",
+                "    lt(1)\n",
+                "    arc(degrees-1)\n",
+                "\n",
+                "with no_pen():\n",
+                "    rt(90)\n",
+                "    fd(30)\n",
+                "    lt(90)\n",
+                "\n",
+                "arc(180)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "e6f6249d-fbed-44bc-95fa-c880c83489c3",
             "metadata": {},
             "source": [
                 "### `get_turtle()`\n",
                 "\n",
                 "Returns existing `_main_turtle`, or creates and sets it if it was `None`.\n",
+                "\n",
                 "Useful when you need to change some turtle attribute, like `animate` or `delay` after `make_turtle()`.\n",
+                "\n",
                 "See example in `draw()`."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "46e41738-27ba-436c-99b0-2801d71dac51",
             "metadata": {},
@@ -626,21 +743,21 @@
                 "Use `draw()` to render the drawing after setting `animate=False` and\n",
                 "issuing turtle commands like `fd()`, `lt()` etc.\n",
                 "\n",
                 "When `animate=True`, `draw()` is automatically called after each turtle command.\n",
                 "\n",
                 "The next example draws two circles.\n",
                 "We can see the turtle drawing the first circle because `animate=True`.\n",
-                "We then set `animate=False`, and the second circle is rendered all at once\n",
-                "when we call `draw()`."
+                "When we set `animate=False`, \n",
+                "the second circle is rendered all at once when we call `draw()`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 14,
             "id": "ee2dccee-8416-4b13-afd6-0cf1815e670e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"240\" height=\"240\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -682,22 +799,22 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "eb84f112-7bc9-4e73-bcaa-11bc3e0d4e11",
             "metadata": {},
             "source": [
-                "### `jumpto(x, y)`\n",
+                "### `jump_to(x, y)`\n",
                 "\n",
-                "Teleport the turtle to coordinates (x, y) without drawing. Contrast with `moveto(x, y)`."
+                "Teleport the turtle to coordinates (x, y) without drawing. Contrast with `move_to(x, y)`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
             "id": "b4d789d3-bb36-485b-945f-fec3b5743734",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -732,31 +849,31 @@
                 "\n",
                 "def square():\n",
                 "    for _ in range(4):\n",
                 "        fd(30)\n",
                 "        rt(90)\n",
                 "\n",
                 "for i in range(3):\n",
-                "    jumpto(i*60 + 5, i*40 + 5)\n",
+                "    jump_to(i*60 + 5, i*40 + 5)\n",
                 "    square()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2ec30936-aae6-4fb5-889c-a5774481155a",
             "metadata": {},
             "source": [
-                "### `moveto(x, y)`\n",
+                "### `move_to(x, y)`\n",
                 "\n",
-                "Move the turtle to coordinates (x, y), drawing if the pen is down. Contrast with `jumpto(x, y)`."
+                "Move the turtle to coordinates (x, y), drawing if the pen is down. Contrast with `jump_to(x, y)`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 16,
             "id": "b5ac5f58-2734-4808-ab1e-78eaa2b64787",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -780,15 +897,15 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "make_turtle(delay=0.01)\n",
                 "\n",
                 "for i in range(3):\n",
-                "    moveto(i*60 + 5, i*40 + 5)\n",
+                "    move_to(i*60 + 5, i*40 + 5)\n",
                 "    square()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6a623799",
             "metadata": {},
@@ -796,15 +913,15 @@
                 "### `set_color(color)`\n",
                 "\n",
                 "Set the `turtle.pen_color` attribute to `color`, which should be a string the `'#RRGGBB'` format or one of the many [Web color names](https://en.wikipedia.org/wiki/Web_colors) supported by modern browsers. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 17,
             "id": "a01a6020",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
@@ -852,15 +969,15 @@
                 "### `set_width(n)`\n",
                 "\n",
                 "Set the `turtle.pen_width` attribute to the integer `n`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 18,
             "id": "78d65084-f35e-4c16-b452-5466c074af07",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<svg width=\"300\" height=\"150\" style=\"fill:none; stroke-linecap:round;\">\n",
```

### Comparing `jupyturtle-2024.3.30/notebooks/lab.ipynb` & `jupyturtle-2024.4.1/notebooks/lab.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856977513227514%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'text': {insert: [(0, 'Help on function forward in module "*

 * *            "jupyturtle.jupyturtle:\\n'), (4, '    If `degrees` is given, turn left after "*

 * *            "moving.\\n')], delete: [0]}}}}, 26: {'id': 'bd8416f5-d17d-41d2-b06d-e7feda399411'}, "*

 * *            "insert: [(23, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'4467f27d-fc39-4657-a1cf-35948a37bfb8'), ('metadata', OrderedDict()), ('source', ['## "*

 * *            "The great renaming\\n', '\\n', 'Curre […]*

```diff
@@ -66,18 +66,19 @@
             "id": "5d7f9eee",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Help on function forward in module jupyturtle:\n",
+                        "Help on function forward in module jupyturtle.jupyturtle:\n",
                         "\n",
                         "forward(*args)\n",
                         "    Move turtle forward by units; draw path if pen is down.\n",
+                        "    If `degrees` is given, turn left after moving.\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "lt(120)\n",
                 "fd(50)\n",
@@ -498,17 +499,89 @@
                 }
             ],
             "source": [
                 "print(get_turtle().get_SVG())"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "4467f27d-fc39-4657-a1cf-35948a37bfb8",
+            "metadata": {},
+            "source": [
+                "## The great renaming\n",
+                "\n",
+                "Current command names:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "id": "2c4f6b84-881a-4067-ac59-f693dae1596d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "bk\n",
+                        "fd\n",
+                        "jp\n",
+                        "lt\n",
+                        "mv\n",
+                        "pd\n",
+                        "pu\n",
+                        "rt\n"
+                    ]
+                }
+            ],
+            "source": [
+                "import jupyturtle\n",
+                "\n",
+                "for name in sorted(dir(jupyturtle), key=str.upper):\n",
+                "    if len(name) == 2:\n",
+                "        print(name)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "6428422c-a736-4afe-9455-12a1ee204238",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'draw': [],\n",
+                            " 'hide': [],\n",
+                            " 'show': [],\n",
+                            " 'move_to': ['moveto', 'mv'],\n",
+                            " 'forward': ['fd'],\n",
+                            " 'back': ['bk'],\n",
+                            " 'jump_to': ['jumpto', 'jp'],\n",
+                            " 'left': ['lt'],\n",
+                            " 'right': ['rt'],\n",
+                            " 'pen_up': ['penup', 'pu'],\n",
+                            " 'pen_down': ['pendown', 'pd'],\n",
+                            " 'toggle_pen': []}"
+                        ]
+                    },
+                    "execution_count": 15,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from jupyturtle.jupyturtle import _commands\n",
+                "_commands"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9f6229de-6923-4399-a7b4-fff42f1e21df",
+            "id": "bd8416f5-d17d-41d2-b06d-e7feda399411",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `jupyturtle-2024.3.30/notebooks/magic-lab.ipynb` & `jupyturtle-2024.4.1/notebooks/magic-lab.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{insert: [(7, OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'35c97a28-61b2-4749-86c4-7b29ecdadca2'), ('metadata', OrderedDict()), ('outputs', "*

 * *            "[]), ('source', [])]))]}"}*

```diff
@@ -218,14 +218,22 @@
                     ]
                 }
             ],
             "source": [
                 "%%turtle 100 200 banana fast 300\n",
                 "pass"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "35c97a28-61b2-4749-86c4-7b29ecdadca2",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `jupyturtle-2024.3.30/src/jupyturtle/jupyturtle.py` & `jupyturtle-2024.4.1/src/jupyturtle/jupyturtle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """
 🐢 jupyturtle.py
+version 2024.04.01
 """
 
 import math
 import sys
 import time
 from contextlib import contextmanager
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import NamedTuple
 
 from IPython.core.error import UsageError
-from IPython.core.magic import register_cell_magic
 from IPython.core.getipython import get_ipython
 from IPython.display import display, HTML, DisplayHandle
 
+if get_ipython() is None:
+    register_cell_magic = lambda f: f  # no-op
+else:
+    from IPython.core.magic import register_cell_magic
+
 
 # defaults
 DEFAULT_DRAW_WIDTH = 300
 DEFAULT_DRAW_HEIGHT = 150
 DRAW_BGCOLOR = '#F3F3F7'  # "anti-flash white" (non-standard name)
 
 
@@ -86,21 +91,21 @@
 
 # mapping of method names to global aliases
 _commands = {}
 
 
 # decorators to build procedural API with turtle commands
 def command(method):
-    """register method for use as a top level function in procedural API"""
+    """Register method for use as a top level function in procedural API."""
     _commands[method.__name__] = []  # no alias
     return method
 
 
 def command_alias(*names):
-    """same as @command, but assigning aliases to the top level function"""
+    """Same as @command, but assigning aliases to the top level function."""
 
     def decorator(method):
         _commands[method.__name__] = list(names)
         return method
 
     return decorator
 
@@ -245,44 +250,47 @@
     @command
     def show(self):
         """Show turtle."""
         self.visible = True
         if self.animate:
             self.draw()
 
-    @command
-    def moveto(self, x: float, y: float):
+    @command_alias('moveto', 'mv')
+    def move_to(self, x: float, y: float):
         """Move the turtle to coordinates (x, y), drawing if the pen is down."""
         new_pos = Point(x, y)
         if self.active_pen:
             self.paths[-1].append(Point(*new_pos))
         else:
             self.paths.append(
                 Path(points=[new_pos], color=self.pen_color, width=self.pen_width)
             )
         self.position = new_pos
         if self.animate:
             self.draw()
 
     @command_alias('fd')
-    def forward(self, units: float):
-        """Move turtle forward by units; draw path if pen is down."""
+    def forward(self, units: float, degrees: float = 0):
+        """Move turtle forward by units; draw path if pen is down.
+        If `degrees` is given, turn left after moving."""
         angle = math.radians(self.heading)
         dx = units * math.cos(angle)
         dy = units * math.sin(angle)
         new_pos = self.position.translated(dx, dy)
-        self.moveto(*new_pos)
+        self.move_to(*new_pos)
+        if degrees:
+            self.left(degrees)
 
     @command_alias('bk')
     def back(self, units: float):
         """Move the turtle backward by units, drawing if the pen is down."""
         self.forward(-units)
 
-    @command
-    def jumpto(self, x: float, y: float):
+    @command_alias('jumpto', 'jp')
+    def jump_to(self, x: float, y: float):
         """Teleport the turtle to coordinates (x, y) without drawing."""
         self.position = Point(x, y)
         self.paths.append(
             Path(points=[self.position], color=self.pen_color, width=self.pen_width)
         )
         if self.animate:
             self.draw()
@@ -297,21 +305,21 @@
     @command_alias('rt')
     def right(self, degrees: float):
         """Turn turtle right by degrees."""
         self.heading += degrees
         if self.animate:
             self.draw()
 
-    @command
-    def penup(self):
+    @command_alias('penup', 'pu')
+    def pen_up(self):
         """Lift the pen, so turtle stops drawing."""
         self.active_pen = False
 
-    @command
-    def pendown(self):
+    @command_alias('pendown', 'pd')
+    def pen_down(self):
         """Lower the pen, so turtle starts drawing."""
         self.active_pen = True
 
     @command
     def toggle_pen(self):
         """Lower the pen if it's up; raises if it's down."""
         self.active_pen = not self.active_pen
@@ -328,23 +336,29 @@
 
 
 ################################################## procedural API
 
 # _install_command() will append more names when the module loads
 __all__ = [
     'Turtle',
+    'Point',
+    'Path',
     'make_turtle',
     'get_turtle',
     'no_pen',
     'set_color',
     'set_width',
     'no_update',
     'set_default',
     'set_heading',
     'show_SVG',
+    'DEFAULT_DRAW_WIDTH',
+    'DEFAULT_DRAW_HEIGHT',
+    'PEN_COLOR',
+    'PEN_WIDTH',
 ]
 
 
 def __dir__():
     return sorted(__all__)
 
 
@@ -387,18 +401,18 @@
     turtle.heading = angle
 
 
 @contextmanager
 def no_pen():
     turtle = get_turtle()
     pen_state = turtle.active_pen
-    turtle.penup()
+    turtle.pen_up()
     yield
     if pen_state:
-        turtle.pendown()
+        turtle.pen_down()
 
 
 @contextmanager
 def no_update():
     with get_turtle() as t:
         yield
 
@@ -413,14 +427,15 @@
 
 def show_SVG():
     print(get_turtle().get_SVG())
 
 
 ######################################## install commands as top-level functions
 
+
 def _make_command(name):
     method = getattr(Turtle, name)  # get unbound method
 
     def command(*args):
         turtle = get_turtle()
         method(turtle, *args)
 
@@ -445,14 +460,15 @@
 
 
 _install_commands()
 
 
 ######################################## install %%turtle cell magic
 
+
 def pop_int_args(args: list[str], expected_at_most: int) -> list[int]:
     int_like_args = []
     for arg in args:
         try:
             int(arg)
         except ValueError:
             continue
@@ -471,15 +487,15 @@
         return True
     return False
 
 
 @register_cell_magic
 def turtle(line, cell):
     """create a new turtle before running this cell
-    
+
     usage: %%turtle arg1 arg2 arg3
 
     All arguments are optional.
     If one of them is the word "fast" (no quotes), animation is turned off.
     If two of them are numbers, they set the drawing width and height in that order.
     If only one is a number, it sets both width and height of the drawing.
     """
```

### Comparing `jupyturtle-2024.3.30/tests/jupyturtle_test.py` & `jupyturtle-2024.4.1/tests/jupyturtle_test.py`

 * *Files identical despite different names*

### Comparing `jupyturtle-2024.3.30/.gitignore` & `jupyturtle-2024.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyturtle-2024.3.30/LICENSE` & `jupyturtle-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyturtle-2024.3.30/README.md` & `jupyturtle-2024.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # jupyturtle
 
 Python Turtle graphics for Jupyter notebooks
 
-For a quick demo, open [the lab notebook](lab.ipynb).
+For a quick demo, open
+[the lab notebook](https://github.com/ramalho/jupyturtle/blob/main/notebooks/lab.ipynb).
 
-No installation required, just download the `jupyter.py`
-module to the same folder where your notebook is saved,
+To use on a live Jupyter Notebook, 
+just download the `jupyter.py` file to the same folder where your notebook is saved,
 and import it.
 
 
 ## Credits
 
 The idea and some of the code for this module came from
 [Tolga Atam](https://github.com/tolgaatam)'s
```

### Comparing `jupyturtle-2024.3.30/pyproject.toml` & `jupyturtle-2024.4.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "jupyturtle"
 description = "Turtle graphics for Jupyter Notebooks"
-version = "2024.03.30"
+version = "2024.04.01"
 authors = [
   { name="Luciano Ramalho", email="luciano@ramalho.org" },
 ]
 dependencies = [
-  "pytest",
+  "jupyter",
   "ipython>=8",
+  "pytest",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
@@ -24,7 +25,12 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.ruff.format]
 # Like Python's `repr()`, use single quotes for strings.
 quote-style = 'single'
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
```

### Comparing `jupyturtle-2024.3.30/PKG-INFO` & `jupyturtle-2024.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.3
 Name: jupyturtle
-Version: 2024.3.30
+Version: 2024.4.1
 Summary: Turtle graphics for Jupyter Notebooks
 Project-URL: Homepage, https://github.com/ramalho/jupyturtle
 Project-URL: Issues, https://github.com/ramalho/jupyturtle/issues
 Author-email: Luciano Ramalho <luciano@ramalho.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: ipython>=8
+Requires-Dist: jupyter
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # jupyturtle
 
 Python Turtle graphics for Jupyter notebooks
 
-For a quick demo, open [the lab notebook](lab.ipynb).
+For a quick demo, open
+[the lab notebook](https://github.com/ramalho/jupyturtle/blob/main/notebooks/lab.ipynb).
 
-No installation required, just download the `jupyter.py`
-module to the same folder where your notebook is saved,
+To use on a live Jupyter Notebook, 
+just download the `jupyter.py` file to the same folder where your notebook is saved,
 and import it.
 
 
 ## Credits
 
 The idea and some of the code for this module came from
 [Tolga Atam](https://github.com/tolgaatam)'s
```

