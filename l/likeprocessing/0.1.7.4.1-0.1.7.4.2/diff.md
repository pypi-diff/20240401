# Comparing `tmp/likeprocessing-0.1.7.4.1.tar.gz` & `tmp/likeprocessing-0.1.7.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likeprocessing-0.1.7.4.1.tar", max compression
+gzip compressed data, was "likeprocessing-0.1.7.4.2.tar", max compression
```

## Comparing `likeprocessing-0.1.7.4.1.tar` & `likeprocessing-0.1.7.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6665 2023-11-23 12:26:13.177138 likeprocessing-0.1.7.4.1/likeprocessing/affichage.py
--rw-r--r--   0        0        0    28492 2023-04-21 06:47:40.260173 likeprocessing-0.1.7.4.1/likeprocessing/bloc2D.py
--rw-r--r--   0        0        0     1322 2022-12-28 17:02:23.280566 likeprocessing-0.1.7.4.1/likeprocessing/error.png
--rw-r--r--   0        0        0       38 2022-12-28 17:02:23.281566 likeprocessing-0.1.7.4.1/likeprocessing/exceptions.py
--rw-r--r--   0        0        0    28385 2023-11-24 18:08:35.080786 likeprocessing-0.1.7.4.1/likeprocessing/formes.py
--rw-r--r--   0        0        0    14488 2023-04-21 06:47:40.263169 likeprocessing-0.1.7.4.1/likeprocessing/images/image1.png
--rw-r--r--   0        0        0     6467 2023-04-21 06:47:40.264159 likeprocessing-0.1.7.4.1/likeprocessing/images/image10.png
--rw-r--r--   0        0        0     4165 2023-04-21 06:47:40.264159 likeprocessing-0.1.7.4.1/likeprocessing/images/image2.png
--rw-r--r--   0        0        0     8127 2023-04-21 06:47:40.265157 likeprocessing-0.1.7.4.1/likeprocessing/images/image3.png
--rw-r--r--   0        0        0     7330 2023-04-21 06:47:40.265157 likeprocessing-0.1.7.4.1/likeprocessing/images/image4.png
--rw-r--r--   0        0        0     7973 2023-04-21 06:47:40.266157 likeprocessing-0.1.7.4.1/likeprocessing/images/image5.png
--rw-r--r--   0        0        0     4547 2023-04-21 06:47:40.266157 likeprocessing-0.1.7.4.1/likeprocessing/images/image6.png
--rw-r--r--   0        0        0     4446 2023-04-21 06:47:40.267159 likeprocessing-0.1.7.4.1/likeprocessing/images/image7.png
--rw-r--r--   0        0        0     5664 2023-04-21 06:47:40.267159 likeprocessing-0.1.7.4.1/likeprocessing/images/image8.png
--rw-r--r--   0        0        0     6670 2023-04-21 06:47:40.268156 likeprocessing-0.1.7.4.1/likeprocessing/images/image9.png
--rw-r--r--   0        0        0     3164 2023-11-23 12:22:26.133821 likeprocessing-0.1.7.4.1/likeprocessing/images.py
--rw-r--r--   0        0        0     1407 2022-12-28 17:02:23.289572 likeprocessing-0.1.7.4.1/likeprocessing/info.png
--rw-r--r--   0        0        0     1553 2023-04-21 06:47:40.268156 likeprocessing-0.1.7.4.1/likeprocessing/jauge.py
--rw-r--r--   0        0        0      617 2022-12-28 17:02:23.291567 likeprocessing-0.1.7.4.1/likeprocessing/list_tools.py
--rw-r--r--   0        0        0     2972 2022-12-28 17:02:23.292567 likeprocessing-0.1.7.4.1/likeprocessing/print_vars.py
--rw-r--r--   0        0        0    20446 2023-05-08 11:55:47.663644 likeprocessing-0.1.7.4.1/likeprocessing/processing.py
--rw-r--r--   0        0        0   117367 2023-10-13 17:47:28.144774 likeprocessing-0.1.7.4.1/likeprocessing/pyDialog.py
--rw-r--r--   0        0        0    12642 2023-04-21 06:47:40.273407 likeprocessing-0.1.7.4.1/likeprocessing/pygame_textinput.py
--rw-r--r--   0        0        0     1399 2022-12-28 17:02:23.296567 likeprocessing-0.1.7.4.1/likeprocessing/question.png
--rw-r--r--   0        0        0    34097 2023-11-24 19:18:11.221504 likeprocessing-0.1.7.4.1/likeprocessing/README.md
--rw-r--r--   0        0        0     4005 2023-04-21 06:47:40.273407 likeprocessing-0.1.7.4.1/likeprocessing/tempos.py
--rw-r--r--   0        0        0     5983 2023-11-24 19:19:49.194921 likeprocessing-0.1.7.4.1/likeprocessing/texte.py
--rw-r--r--   0        0        0     1768 2023-04-21 06:47:40.274429 likeprocessing-0.1.7.4.1/likeprocessing/tor.py
--rw-r--r--   0        0        0     4351 2023-04-21 06:47:40.275419 likeprocessing-0.1.7.4.1/likeprocessing/transformation.py
--rw-r--r--   0        0        0     4065 2022-12-28 17:02:23.303567 likeprocessing-0.1.7.4.1/likeprocessing/trigo.py
--rw-r--r--   0        0        0      720 2022-12-28 17:02:23.304568 likeprocessing-0.1.7.4.1/likeprocessing/warning.png
--rw-r--r--   0        0        0      429 2023-11-24 19:26:51.351676 likeprocessing-0.1.7.4.1/pyproject.toml
--rw-r--r--   0        0        0    34942 2023-11-24 19:27:08.691648 likeprocessing-0.1.7.4.1/setup.py
--rw-r--r--   0        0        0    33249 2023-11-24 19:27:08.692646 likeprocessing-0.1.7.4.1/PKG-INFO
+-rw-r--r--   0        0        0     6665 2023-11-23 12:26:13.177138 likeprocessing-0.1.7.4.2/likeprocessing/affichage.py
+-rw-r--r--   0        0        0    28492 2023-04-21 06:47:40.260173 likeprocessing-0.1.7.4.2/likeprocessing/bloc2D.py
+-rw-r--r--   0        0        0     1322 2022-12-28 17:02:23.280566 likeprocessing-0.1.7.4.2/likeprocessing/error.png
+-rw-r--r--   0        0        0       38 2022-12-28 17:02:23.281566 likeprocessing-0.1.7.4.2/likeprocessing/exceptions.py
+-rw-r--r--   0        0        0    28433 2023-11-25 08:20:28.471722 likeprocessing-0.1.7.4.2/likeprocessing/formes.py
+-rw-r--r--   0        0        0    14488 2023-04-21 06:47:40.263169 likeprocessing-0.1.7.4.2/likeprocessing/images/image1.png
+-rw-r--r--   0        0        0     6467 2023-04-21 06:47:40.264159 likeprocessing-0.1.7.4.2/likeprocessing/images/image10.png
+-rw-r--r--   0        0        0     4165 2023-04-21 06:47:40.264159 likeprocessing-0.1.7.4.2/likeprocessing/images/image2.png
+-rw-r--r--   0        0        0     8127 2023-04-21 06:47:40.265157 likeprocessing-0.1.7.4.2/likeprocessing/images/image3.png
+-rw-r--r--   0        0        0     7330 2023-04-21 06:47:40.265157 likeprocessing-0.1.7.4.2/likeprocessing/images/image4.png
+-rw-r--r--   0        0        0     7973 2023-04-21 06:47:40.266157 likeprocessing-0.1.7.4.2/likeprocessing/images/image5.png
+-rw-r--r--   0        0        0     4547 2023-04-21 06:47:40.266157 likeprocessing-0.1.7.4.2/likeprocessing/images/image6.png
+-rw-r--r--   0        0        0     4446 2023-04-21 06:47:40.267159 likeprocessing-0.1.7.4.2/likeprocessing/images/image7.png
+-rw-r--r--   0        0        0     5664 2023-04-21 06:47:40.267159 likeprocessing-0.1.7.4.2/likeprocessing/images/image8.png
+-rw-r--r--   0        0        0     6670 2023-04-21 06:47:40.268156 likeprocessing-0.1.7.4.2/likeprocessing/images/image9.png
+-rw-r--r--   0        0        0     3164 2023-11-23 12:22:26.133821 likeprocessing-0.1.7.4.2/likeprocessing/images.py
+-rw-r--r--   0        0        0     1407 2022-12-28 17:02:23.289572 likeprocessing-0.1.7.4.2/likeprocessing/info.png
+-rw-r--r--   0        0        0     1553 2023-04-21 06:47:40.268156 likeprocessing-0.1.7.4.2/likeprocessing/jauge.py
+-rw-r--r--   0        0        0      617 2022-12-28 17:02:23.291567 likeprocessing-0.1.7.4.2/likeprocessing/list_tools.py
+-rw-r--r--   0        0        0     2972 2022-12-28 17:02:23.292567 likeprocessing-0.1.7.4.2/likeprocessing/print_vars.py
+-rw-r--r--   0        0        0    20616 2023-11-25 16:46:30.759621 likeprocessing-0.1.7.4.2/likeprocessing/processing.py
+-rw-r--r--   0        0        0   118031 2023-11-27 10:01:26.781865 likeprocessing-0.1.7.4.2/likeprocessing/pyDialog.py
+-rw-r--r--   0        0        0    12642 2023-04-21 06:47:40.273407 likeprocessing-0.1.7.4.2/likeprocessing/pygame_textinput.py
+-rw-r--r--   0        0        0     1399 2022-12-28 17:02:23.296567 likeprocessing-0.1.7.4.2/likeprocessing/question.png
+-rw-r--r--   0        0        0    34097 2023-11-24 19:18:11.221504 likeprocessing-0.1.7.4.2/likeprocessing/README.md
+-rw-r--r--   0        0        0     4659 2024-04-01 16:00:54.316205 likeprocessing-0.1.7.4.2/likeprocessing/tempos.py
+-rw-r--r--   0        0        0     5983 2023-11-24 19:19:49.194921 likeprocessing-0.1.7.4.2/likeprocessing/texte.py
+-rw-r--r--   0        0        0     1768 2023-04-21 06:47:40.274429 likeprocessing-0.1.7.4.2/likeprocessing/tor.py
+-rw-r--r--   0        0        0     4351 2023-04-21 06:47:40.275419 likeprocessing-0.1.7.4.2/likeprocessing/transformation.py
+-rw-r--r--   0        0        0     4065 2022-12-28 17:02:23.303567 likeprocessing-0.1.7.4.2/likeprocessing/trigo.py
+-rw-r--r--   0        0        0      720 2022-12-28 17:02:23.304568 likeprocessing-0.1.7.4.2/likeprocessing/warning.png
+-rw-r--r--   0        0        0      429 2024-04-01 16:30:11.871072 likeprocessing-0.1.7.4.2/pyproject.toml
+-rw-r--r--   0        0        0    34942 2024-04-01 16:30:21.066370 likeprocessing-0.1.7.4.2/setup.py
+-rw-r--r--   0        0        0    33249 2024-04-01 16:30:21.068370 likeprocessing-0.1.7.4.2/PKG-INFO
```

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/affichage.py` & `likeprocessing-0.1.7.4.2/likeprocessing/affichage.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/bloc2D.py` & `likeprocessing-0.1.7.4.2/likeprocessing/bloc2D.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/error.png` & `likeprocessing-0.1.7.4.2/likeprocessing/error.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/formes.py` & `likeprocessing-0.1.7.4.2/likeprocessing/formes.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,16 @@
     arrow_start : si True pointe de fléche au début
     arrow_end : si True point de flèche à la fin
     command : nom de la fonction à appeler si les trait est cliqué
     name : valeur passée à la fonction désignée par command"""
     stroke = kwargs.get("stroke", processing.__border_color)
     points = [(x1, y1), (x2, y2)]
     points = processing.transformation(points)
+    x1, y1 = points[0]
+    x2, y2 = points[1]
     stroke_weight = kwargs.get("stroke_weight", processing.__border_width)
     fill_mouse_on = kwargs.get("fill_mouse_on", processing.__fill_color_mouse_on)
     arrow_start = kwargs.get("arrow_start", False)
     arrow_end = kwargs.get("arrow_end", False)
     command = kwargs.get("command", None)
     command_mouse_over = kwargs.get("command_mouse_over", None)
     name = kwargs.get("name", None)
```

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image1.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image1.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image10.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image10.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image2.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image2.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image3.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image3.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image4.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image4.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image5.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image5.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image6.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image6.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image7.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image7.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image8.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image8.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images/image9.png` & `likeprocessing-0.1.7.4.2/likeprocessing/images/image9.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/images.py` & `likeprocessing-0.1.7.4.2/likeprocessing/images.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/info.png` & `likeprocessing-0.1.7.4.2/likeprocessing/info.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/jauge.py` & `likeprocessing-0.1.7.4.2/likeprocessing/jauge.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/list_tools.py` & `likeprocessing-0.1.7.4.2/likeprocessing/list_tools.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/print_vars.py` & `likeprocessing-0.1.7.4.2/likeprocessing/print_vars.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/processing.py` & `likeprocessing-0.1.7.4.2/likeprocessing/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,18 +194,20 @@
     elif valeur == 0:
         processing.__score = 0
     else:
         processing.__score += valeur
 
 
 def random(mini, maxi=None):
+    """retourne un nombre aléatoire entre mini et maxi inclus
+    si maxi n'est pas précisé, retourne un nombre aléatoire entre 0 et la valeur entrée en paramètre"""
     if maxi is None:
         maxi = mini
         mini = 0
-    return randint(mini, maxi - 1)
+    return randint(mini, maxi)
 
 
 def mouseX():
     """retourne la position en X de la souris"""
     return pygame.mouse.get_pos()[0]
```

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/pyDialog.py` & `likeprocessing-0.1.7.4.2/likeprocessing/pyDialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,25 +239,33 @@
                 couleur_fond = self.fill
 
             if self.image_rect is None:
                 if self.fill is not None:
                     # modifications pour arrondir les rectangles
                     # r = pygame.Surface((self.width, self.height))
                     # r.fill(couleur_fond)
-                    r = pygame.Rect(self.parent.left + self.left, self.parent.top + self.top, self.width, self.height)
+                    if isinstance(self.parent, Dialog):
+                        r = pygame.Rect(self.parent.left + self.left, self.parent.top + self.top, self.width,
+                                        self.height)
+                    else:
+                        r = pygame.Rect(self.left, self.top, self.width, self.height)
                     pygame.draw.rect(Boite.ecran, couleur_fond, r, 0, self.border_rounded)
                 else:
                     r = pygame.Surface((self.width, self.height), pygame.SRCALPHA, 32)
                     r = r.convert_alpha()
                     Boite.ecran.blit(r, [self.parent.left + self.left, self.parent.top + self.top])
             else:
                 Boite.ecran.blit(self.image_rect, (self.parent.left + self.left, self.parent.top + self.top),
                                  (0, 0, self.image_rect.get_width(), self.image_rect.get_height()))
             if self.stroke_weight > 0:
-                r = pygame.Rect(self.parent.left + self.left, self.parent.top + self.top, self.width, self.height)
+                if isinstance(self.parent, Dialog):
+                    r = pygame.Rect(self.parent.left + self.left, self.parent.top + self.top, self.width,
+                                    self.height)
+                else:
+                    r = pygame.Rect(self.left, self.top, self.width, self.height)
                 pygame.draw.rect(Boite.ecran, couleur_bord, r, self.stroke_weight, self.border_rounded)
 
     def draw_infobulle(self):
         if self.affiche_tool_tips and self.tick < 100:
             processing.triangle(self.x_bulle, self.y_bulle, self.x_bulle + 5, self.y_bulle - 20,
                                 self.x_bulle + 10, self.y_bulle - 10, fill="#EFF67B", no_stroke=True)
             tool_tips = MultiLineText(None, (self.x_bulle, self.y_bulle), self.infobulle,
@@ -707,15 +715,15 @@
         kwargs["stroke_weight"] = kwargs.get("stroke_weight", 1)
         kwargs["fill"] = kwargs.get("fill", affichage.rgb_color("white"))
         kwargs["font"] = kwargs.get("font", "arial")
         kwargs["font_size"] = kwargs.get("font_size", 12)
         nb_ligne = kwargs.get('nb_ligne', 10)
         ps = pygame.font.SysFont(kwargs["font"], kwargs["font_size"])
         h = ps.size("bg")[0]
-        rectangle: tuple[int,int,int,int] = tuple(list(rect[:3]) + [(4 + h) * nb_ligne + 4])
+        rectangle: tuple[int, int, int, int] = tuple(list(rect[:3]) + [(4 + h) * nb_ligne + 4])
         if parent is None:
             processing.ihm.append(self)
         super().__init__(parent, rectangle, **kwargs)
         self.police = kwargs["font"]
         self.texte = texte.split("\n")
         self.nb_ligne = nb_ligne
         self.ligne_actuelle = 0
@@ -1281,16 +1289,20 @@
 
     def positionne(self):
         if self.pos == "center":
             self.center_me()
 
     def center_me(self):
         """center la boite sur l'écran"""
-        self.x = (self.parent.width - self.width) // 2
-        self.y = (self.parent.height - self.height) // 2
+        if isinstance(self.parent, Dialog):
+            self.x = (self.parent.width - self.width) // 2
+            self.y = (self.parent.height - self.height) // 2
+        else:
+            self.x = (processing.width() - self.width) // 2
+            self.y = (processing.height() - self.height) // 2
 
     def quitter(self):
         """methode appelée lors du clic sur la croix
         de la boite de dialogue"""
         self._visible = False
         self.focus = False
         self.destroy = True
@@ -2786,15 +2798,16 @@
     def response(self) -> int:
         x, y = 0, 0
         self.focus = True
         fond = processing.get_background_image()
         processing.save_background()
         while self.value == -1:
             processing.draw_background()
-            self.parent.draw()
+            if isinstance(self.parent, Dialog):
+                self.parent.draw()
             self.draw()
             processing.redraw()
             __events = pygame.event.get()
             for event in __events:
                 if event.type == 1024:
                     x, y = pygame.mouse.get_pos()
                 elif event.type == pygame.MOUSEBUTTONDOWN:
```

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/pygame_textinput.py` & `likeprocessing-0.1.7.4.2/likeprocessing/pygame_textinput.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/question.png` & `likeprocessing-0.1.7.4.2/likeprocessing/question.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/README.md` & `likeprocessing-0.1.7.4.2/likeprocessing/README.md`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/tempos.py` & `likeprocessing-0.1.7.4.2/likeprocessing/tempos.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 import likeprocessing.processing as processing
 
 
 class Tempo:
-
     def __init__(self, duree_ms: int, work=True):
         """t=Tempo(500) créer un objet de temporisation t de durée 500 ms qui se relance indéfiniment"""
         self.depart = processing.frameCount()
         self.duree_ms = duree_ms
         self.work = work
         if self.work:
             self.on = True
         else:
             self.on = False
 
+    def stop(self):
+        """arrête le fonctionnement de la temporisation """
+        self.work = False
+
+    def start(self,value=None):
+        """démarre le fonctionnement de la temporisation """
+        self.work = True
+        if value is not None:
+            self.set_tempo(value)
+        else:
+            self.reset()
+
     def flip(self):
         self.on = not self.on
 
     def set_tempo(self, duree_ms: int):
         """permet de réinitialiser la temporisation avec une nouvelle valeur."""
-        self.depart = processing.frameCount()
         self.duree_ms = duree_ms
+        self.reset()
 
     def reset(self):
         """force le redémarrage de la temporisation."""
         self.on = self.work
-        self.depart = processing.frameCount()
+        if self.work:
+            self.depart = processing.frameCount()
 
     def fin(self) -> bool:
         """renvoie True lorsque la temporisation est terminée. Pour notre exemple au bout de 500 ms."""
-        if ((processing.frameCount() - self.depart) / processing.getFrameRate()) * 1000 >= self.duree_ms:
-            self.depart = processing.frameCount()
-            self.flip()
-            return True
-        else:
-            return False
+        if self.work:
+            if ((processing.frameCount() - self.depart) / processing.getFrameRate()) * 1000 >= self.duree_ms:
+                self.depart = processing.frameCount()
+                self.flip()
+                return True
+            else:
+                return False
+        return False
 
     def is_on(self):
         """renvoie True si la temporisation est à on."""
         self.fin()
         return self.on
 
     def is_off(self):
         """renvoie True si la temporisation est à off."""
         return not self.is_on()
 
+    def is_stop(self):
+        """retourne True si la temporistion est à l'arrêt"""
+        return not self.work
+
+    def is_start(self):
+        """retourne True si la temporisation est en fonctionnement"""
+        return self.work
 
 class Monostable(Tempo):
     def __init__(self, duree_ms: int, work=True):
         """t=Monostable(500) créer un objet de temporisation t de durée 500 ms qui ne relance pas indéfiniment"""
         super().__init__(duree_ms, work)
         self.__stop = True
         self.trigger_value = False
```

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/texte.py` & `likeprocessing-0.1.7.4.2/likeprocessing/texte.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/tor.py` & `likeprocessing-0.1.7.4.2/likeprocessing/tor.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/transformation.py` & `likeprocessing-0.1.7.4.2/likeprocessing/transformation.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/trigo.py` & `likeprocessing-0.1.7.4.2/likeprocessing/trigo.py`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/likeprocessing/warning.png` & `likeprocessing-0.1.7.4.2/likeprocessing/warning.png`

 * *Files identical despite different names*

### Comparing `likeprocessing-0.1.7.4.1/setup.py` & `likeprocessing-0.1.7.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'likeprocessing': ['images/*']}
 
 install_requires = \
 ['pygame>=2.1.2,<3.0.0', 'pygame_textinput>=1.0.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'likeprocessing',
-    'version': '0.1.7.4.1',
+    'version': '0.1.7.4.2',
     'description': 'Like processing library with pygame',
     'long_description': '\n## Structure du programme \n\n\n### Installation:\n\n**Dans pycharm :** \\\nCTRL+ALT+s, puis choisir project -> python interpreter et + puis likeprocessing\n\n**dans le terminal :** \\\npip install likeprocessing\n\n\n### Les fonctions setup(), draw() et run(globals())\n\nLe programme doit contenir deux fonctions, setup() et draw(), et l\'exécution est lancée à l\'aide de l\'instruction run(globals()).\n\nLorsque l\'on exécute l\'instruction run(globals()), la fonction setup() est exécutée une fois :\n\n\n```\nfrom likeprocessing.processing import *\ndef setup():\n    createCanvas(800,600)\n    # instructions de paramétrage de l\'affichage\n```\n\n\nCette fonction permet de définir les dimensions de la fenêtre de tracé, et quelques paramètres initiaux. Les valeurs données aux paramètres de la fonction **createCanvas() ** sont affectées automatiquement à deux variables systèmes : **width** pour le premier paramètre et **height** pour le second. Un troisième paramètre **resizable** optionnel permet d\'offrir la possibilité de redimensionner la fenêtre avec la souris  On peut récupérer les valeurs de **width** et **height** grâce au fonction **width()** et **height()**\n\nPuis la fonction **draw()** est ensuite exécutée en boucle, après l\'exécution de **setup()**:\n\n\n```\ndef draw():\n    # instructions de dessin\n```\n\n\nElle contient des instructions qui seront exécutées avec une fréquence réglable, permettant de modifier le contenu de la fenêtre et de créer des contenus statiques ou des animations.\n\nL\'instruction **stop()** met fin à l\'exécution de la boucle :\n\n\n```\ndef compute():\n    # instructions de calcul\n```\n\n\nCette fonction n\'est pas obligatoire. Elle permet d\'éviter de trop surcharger la fonction **draw()** en réservant celle-ci aux instructions de dessins. La fonction **compute()** si elle existe est insérée dans la boucle et est exécutée avant la fonction **draw()** \n\n\n## Structure de base :\n\n\n```\nfrom likeprocessing.processing import *\n\ndef setup():\n   createCanvas(400,200)\n   background("grey")\n\ndef draw():\n   pass\n\nrun(globals())\n```\n\n\n\n## Fonctions système\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>width(), height()\n   </td>\n   <td>Dimensions de la zone de dessin. Les valeurs de width et height sont définies par les paramètres de la fonction createCanvas().\n   </td>\n  </tr>\n  <tr>\n   <td>createCanvas()\n   </td>\n   <td> La fonction createCanvas(largeur,hauteur) permet de dimensionner la fenêtre de l\'application. En plus de la largeur et de la hauteur on peut ajouter un troisieme paramètre à True pour que la fenêtre puisse être redimensionnée. (ex createCanvas(400,300,True).\n     <BR>On peut aussi changer l\'icone de la fenêtre avec le paramètre facultatif icone :<br>\n     createCanvas(400,300,True,icone="image.png")  \n   </td>\n  </tr>\n  <tr>\n   <td>title("mon titre")\n   </td>\n   <td> La fonction title("mon titre") permet de changer le titre de la fenêtre par mon titre\n   </td>\n  </tr>\n  <tr>\n   <td>set_icone("icone.jpg")\n   </td>\n   <td> La fonction set_icone() permet de changer l\'icône de la fenêtre\n   </td>\n  </tr>\n</table>\n\n\n\n## Rafraîchissement\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>frameCount()\n   </td>\n   <td>Nombre d\'images affichées depuis le démarrage du programme.\n   </td>\n  </tr>\n  <tr>\n   <td>frameRate() \\\ngetFrameRate()\n   </td>\n   <td>Renvoie le nombre d\'images affichées chaque seconde.\n   </td>\n  </tr>\n  <tr>\n   <td>frameRate(valeur) \\\nsetFrameRate(valeur)\n   </td>\n   <td>Spécifie le nombre d\'images à afficher chaque seconde.\n   </td>\n  </tr>\n  <tr>\n   <td>noLoop()\n   </td>\n   <td>Si cette instruction est présente dans la fonction setup la fonction draw sera exécutée une seule fois. Si cette instruction est présente dans la fonction draw, les instructions de la fonction draw en cours sont exécutées (il n\'y a pas d\'interruption) mais celle-ci ne sera pas appelée à nouveau.\n   </td>\n  </tr>\n  <tr>\n   <td>loop()\n   </td>\n   <td>Relance l\'exécution en boucle de draw().\n   </td>\n  </tr>\n</table>\n\n\n\n## Couleurs\n\n\n## Désigner une couleur\n\n\n<table>\n  <tr>\n   <td><strong>syntaxe</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>\'red\'\n   </td>\n   <td>nom de couleur\n   </td>\n  </tr>\n  <tr>\n   <td>120\n   </td>\n   <td>niveau de gris : 0 - 255\n   </td>\n  </tr>\n  <tr>\n   <td>(100, 125, 255)\n   </td>\n   <td>couleur r, v, b (décimal) : 0 - 255\n   </td>\n  </tr>\n  <tr>\n   <td>\'#2aff95\'\n   </td>\n   <td>couleur r, v, b (hexadécimal) : 00 - ff\n   </td>\n  </tr>\n</table>\n\n\n\n## Dessiner en couleur\n\n\n<table>\n  <tr>\n   <td><strong>Fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>background(couleur)\n   </td>\n   <td>Définit la couleur d\'arrière-plan de la zone de dessin (255 par défaut).\n   </td>\n  </tr>\n  <tr>\n   <td>set_background_image(image: Image)\n   </td>\n   <td>Définit l\'image d\'arrière-plan de la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>get_background_image()\n   </td>\n   <td>Récupère l\'image d\'arrière-plan de la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>save_background():\n   </td>\n   <td>fait une copie du contenu de la fenêtre et le sauvegarde dans l\'image d\'arrière plan.\n   </td>\n  </tr>\n  <tr>\n   <td>fill(couleur=None)\n   </td>\n   <td>Définit la couleur de remplissage des formes (255 par défaut) et réactive le remplissage des formes. Sans paramètre seul le remplissage est activé (utile après un noFill()). Retourne la valeur précédente du remplissage.\n   </td>\n  </tr>\n  <tr>\n   <td>fill_mouse_on(couleur: any):\n   </td>\n   <td>initialise la couleur de fond des figures qui affichera quand la souris est dessus.\n   </td>\n  </tr>\n  <tr>\n   <td>get_fill()\n   </td>\n   <td>Retourne la couleur de fond actuelle\n   </td>\n  </tr>\n  <tr>\n   <td>noFill()\n   </td>\n   <td>Désactive la couleur de remplissage.\n   </td>\n  </tr>\n  <tr>\n   <td>stroke(couleur)\n   </td>\n   <td>Définit la couleur du tracé des bords des formes et des lignes("black" par défaut). Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n  <tr>\n   <td>get_stroke()\n   </td>\n   <td>retourne la couleur des bords actuelle\n   </td>\n  </tr>\n  <tr>\n   <td>noStroke()\n   </td>\n   <td>Désactive le tracé du contour des figures. Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n  <tr>\n   <td>save_fill_stroke()\n   </td>\n   <td>Sauvegarde les paramètres fill et stroke\n   </td>\n  </tr>\n  <tr>\n   <td>restore_fill_stroke()\n   </td>\n   <td>recharge les paramètres fill et stroke précédemment sauvegardé avec <strong>save_fill_stroke</strong>\n   </td>\n  </tr>\n</table>\n\n\nSi **noFill()** et **noStroke() **sont exécutées en même temps, rien n\'est tracé dans la zone de dessin.\n\n\n## Formes\n\n\n### Primitives 2d\n\nL\'origine du repère est située en haut à gauche. Les abscisses augmentent de gauche à droite, les ordonnées augmentent de haut en bas.\n\n\n\n![](./images/image1.png)\n\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>point(x, y)\n   </td>\n   <td>Trace un point de coordonnées (x, y). carré de 2x2 pixels\n   </td>\n  </tr>\n  <tr>\n   <td>line(x1, y1, x2, y2)\n   </td>\n   <td>Trace un segment reliant les deux points de coordonnées (x1, y1) et (x2, y2).\n   </td>\n  </tr>\n  <tr>\n   <td>ellipse(x, y, largeur, hauteur)\n   </td>\n   <td>Tracer une ellipse dont le centre a pour coordonnées (x, y) et dont la largeur et la hauteur prennent les valeurs fixées.\n   </td>\n  </tr>\n  <tr>\n   <td>circle(x, y, diametre)\n   </td>\n   <td>Trace un cercle dont le centre a pour coordonnées (x, y) et dont le diamètre prend la valeur fixée. Idem ellipse((x, y, diametre, diametre)\n   </td>\n  </tr>\n  <tr>\n   <td>arc(x,y,largeur,hauteur,,angleDebut, angleFin)\n   </td>\n   <td>Créer une portion d\'ellipse type part de tarte qui pourra être rempli entre les points repérés par les angles angleDébut et angleFin (unité courante). x et y sont les coordonnées du centre du cercle.  \n   </td>\n  </tr>\n  <tr>\n   <td>circle_arc(x,y,rayon,angleDebut, angleFin)\n   </td>\n   <td>idem arc mais à partir d\'un disque\n   </td>\n  </tr>\n  <tr>\n   <td>ellipseMode(corners_center: str)\n   </td>\n   <td>Définie la position des points x et y des fonctions basées sur ellipse. par défaut : "corners" x et y sont les coordonnées du point en haut à gauche du rectangle dans lequel est inscrit l\'ellipse. si les paramètre est "center" x et y représente le centre du rectangle. Retourne la valeur précédente du mode.\n   </td>\n  </tr>\n  <tr>\n   <td>rect(x, y, largeur, hauteur)\n   </td>\n   <td>Créer un rectangle aux coordonnées x,y de largeur largeur et de hauteur. Si rectMode(\'center\') x et y sont les coordonnées du centre du rectangle. Si rectMode(\'corners\') x,y sont les coordonnées du coin haut gauche. Le rectangle est rempli par la couleur définie par fill(couleur). Si le paramètre image est renseigné (image= ...) le fond du rectangle sera occupé pas l\'image retaillée aux dimensions du rectangle sauf si largeur et/ou hauteur sont nulles (ou non renseignées). largeur et/ou hauteur seront alors celles de l\'image. Les paramètres <strong>allign_h </strong>(left, center et right) et  <strong>allign_v</strong> (top,center et bottom) permettent d\'aligner l\'image dans un cadre plus grand qu\'elle.\n   </td>\n  </tr>\n  <tr>\n   <td>square(x, y, cote)\n   </td>\n   <td>Trace un carré dont le sommet en haut à gauche a pour coordonnées (x, y) et dont le côté prend la valeur fixée. fonctionnement idem rectangle\n   </td>\n  </tr>\n  <tr>\n   <td>rectMode(corners_center: str)\n   </td>\n   <td>Définie la position des points x et y des fonctions basées sur rect. par défaut : "corners" x et y sont les coordonnées du point en haut à gauche du rectangle. si les paramètre est "center" x et y représente le centre du rectangle. Retourne la valeur précédente du mode.\n   </td>\n  </tr>\n  <tr>\n   <td>triangle(x1, y1, x2, y2, x3, y3)\n   </td>\n   <td>Trace un triangle dont les trois sommets ont pour coordonnées (x1, y1), (x2, y2), et (x3, y3).\n   </td>\n  </tr>\n  <tr>\n   <td>quad(x1, y1, x2, y2, x3, y3, x4, y4)\n   </td>\n   <td>Trace un quadrilatère dont les quatre sommets ont pour coordonnées (x1, y1), (x2, y2), (x3, y3) et (x4, y4).\n   </td>\n  </tr>\n  <tr>\n   <td>k_line(points)\n   </td>\n   <td>trace un ligne brisée à partir d\'une liste de points [[1,2],[5,6],[8,3],.....]. (nb_point = nb_segments + 1)\n   </td>\n  </tr>\n</table>\n\n\n\n### Tracés\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>strokeWeight(epaisseur)\n   </td>\n   <td>Définit l\'épaisseur du tracé en pixels (par défaut : 1 pixel). Retourne la valeur précédente de la largeur du trait\n   </td>\n  </tr>\n  <tr>\n   <td>noStroke()\n   </td>\n   <td>Désactive le tracé du contour des figures en mettant la largeur du bord à 0. Retourne la valeur précédente de la largeur.\n   </td>\n  </tr>\n  <tr>\n   <td>stroke(couleur)\n   </td>\n   <td>Définit la couleur du tracé des bords des formes et des lignes ("black" par défaut). Si aucune valeur n\'est passée, celle-ci retourne la couleur actuelle. Retourne la valeur précédente de la couleur.\n   </td>\n  </tr>\n</table>\n\n\n\n## Paramètres optionnels:\n\nLes paramètres optionnels sont passés directement dans la fonction et ne concernent que celle-ci: \n\nfill, no_fill, fill_mouse_on, stroke, stroke_weight, command, fill_mousse_on, name. Pour les rectangles nous avons en plus image et border_rounded \n\nexemple :\n\n\n```\ntriangle(20, 10, 50, 15, 40, 70, fill = "green", fill_mouse_on="yellow", stroke_weight=3)\nrect(10,100,100,50,fill = "red", image=loadImage("image.jpg")) # rectangle avec une image\nrect(150,100,100,60,fill= "blue",border_rounded = 10) # rectangle au coins arrondis avec un rayon de 10px \n```\n\n\nl\'ajout de **command = ma_fonction** ou **command_mouse_over = ma_fonction** au paramètre **fill_mouse_on="couleur"** permet d\'exécuter la fonction **ma_fonction()**. Si l\'on veut attribuer **ma_fonction** à plusieurs formes il est possible d\'ajouter le paramètre **name = valeur**. Dans ce cas, la fonction **ma_fonction(name)** sera exécutée . Il faudra créer impérativement soit : \n\ndef ma_fonction():\n\n    pass\n\nou\n\ndef ma_fonction(nom):\n\n    pass\n\nRemarque:<br>\navec le paramètre command exécute la fonction si la forme est cliquée alors qu\'avec command_mous_over elle sera exécutée simplement si la souris est sur la forme.<br>\nSi les deux paramètres sont présents les deux fonctions sont exécutées.\n\n## Textes\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>text(chaine, x, y)\n   </td>\n   <td>Affiche la chaîne à la position (x, y) dans une boite ajustée. couleur, largeur bord et couleur bord de la boite idem formes. Accepte les paramètres optionnels\n   </td>\n  </tr>\n  <tr>\n   <td>text(chaine, x, y, largeur, hauteur)\n   </td>\n   <td>Affiche la chaîne à la position (x, y) dans une boite de dimensions largeur x hauteur. couleur, largeur bord et couleur bord de la boite idem formes. largeur et hauteur sont optionnels\n   </td>\n  </tr>\n  <tr>\n   <td>text_button(texte_bouton, x, y, largeur, hauteur,command=ma_fonction, name="nom")\n   </td>\n   <td>Affiche un bouton à la position (x, y) dans une boite de dimensions largeur x hauteur. couleur, largeur bord et couleur bord de la boite idem formes. largeur et hauteur sont optionnels.command est une fonction qui sera exécutée si le bouton est cliqué. name est optionnel et permet d\'attribuer un nom au bouton. Si name est présent, la fonction command sera exécutée avec le paramètre name (optionnel). \n   </td>\n  </tr>\n  <tr>\n   <td>textAlign(alignement_horizontal)\n<p>\ntextAlign(alignement_horizontal, alignement_vertical)\n   </td>\n   <td>Spécifie l\'alignement horizontal parmi LEFT, CENTER, et RIGHT et l\'alignement vertical parmi TOP, BOTTOM, CENTER, et BASELINE\n   </td>\n  </tr>\n  <tr>\n   <td>textFont(police)\n<p>\ntextFont(police, taille)\n   </td>\n   <td>Spécifie la police de caractères et éventuellement sa taille. Retourne la police et la taille précédente \n   </td>\n  </tr>\n  <tr>\n   <td>textSize(taille)\n   </td>\n   <td>Spécifie la taille de la police de caractères. Retourne la taille précédente de la police\n   </td>\n  </tr>\n  <tr>\n   <td>textStyle(style)\n   </td>\n   <td>Spécifie le style parmi NORMAL, ITALIC, BOLD et BOLDITALIC\n   </td>\n  </tr>\n  <tr>\n   <td>textWidth(chaine)\n   </td>\n   <td>Largeur en pixels de l\'affichage de chaîne, dans la police et taille actuelles\n   </td>\n  </tr>\n</table>\n\n\n\n## Paramètres optionnels spécifique à text:\n\nLes paramètres optionnels sont passés directement dans la fonction et ne concernent que celle-ci: \n\nla fonction text possèdes elle aussi des paramètres optionnels qui ne concernent que la fonction en cours : \\\n**font, font_size, font_color** qui permettent  de définir la police, la taille des caractères ainsi que la couleur de ceux-ci. \n\n**allign_h et allign_v** permettent de positionner le texte dans la boîte de texte comme **textAllign()**.\n\n**padx et pady** permettent de créer une marge autour du texte (valeur en pixels)\n\n**margin_left, margin_right, margin_top, margin_bottom** permettent de créer de décaler le texte (valeur en pixels) \\\n**margin_left** décale le texte vers la droite si align_h="left" \\\n**margin_right** décale le texte vers la gauche si align_h="right" \\\n**margin_top** décale le texte vers le bas si align_v="top" \\\n**margin_bottom** décale le texte vers le haut si align_v="bottom" \n\nexemple : \n\n\n```\ntext("salut les amis",20,30,300,allign_h="center",font="arial",font_size=48,fontTools="green",pady=10)\n```\n\n\n\nCe code va afficher "salut les amis" dans un cadre de longueur 300 à la position x=20 et y=30. La hauteur du cadre est calculée en fonction de la hauteur du texte (font_size). **pady=10** ajoute 10 pixels au dessus et en dessous du texte. **Si la hauteur du cadre est donnée, si celle-ci est trop petite le texte sortira du cadre.** \n\n\n## Événements\n\n\n### Touches du clavier\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>key()\n   </td>\n   <td>état des touches du clavier (list)\n   </td>\n  </tr>\n  <tr>\n   <td>keyCode()\n   </td>\n   <td>Code de la dernière touche appuyée.\n   </td>\n  </tr>\n  <tr>\n   <td>keyIsPressed()\n<p>\nisKeyPressed()\n   </td>\n   <td>Vaut True lorsqu\'une touche du clavier est appuyée et False sinon.\n   </td>\n  </tr>\n  <tr>\n   <td>keyIsDown(code)\n<p>\nkeyIsDown(touche)\n   </td>\n   <td>Vaut True si la touche concernée est appuyée et False sinon.\n   </td>\n  </tr>\n</table>\n\n\n\n### Souris\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>mouseX(), mouseY()\n   </td>\n   <td>Coordonnées du pointeur de la souris\n   </td>\n  </tr>\n  <tr>\n   <td>mouseXY()\n   </td>\n   <td>Coordonnées du pointeur de la souris sous forme de tuple\n   </td>\n  </tr>\n  <tr>\n   <td>mouseIsPressed()\n   </td>\n   <td>Vaut True si la souris est cliquée, et False sinon.\n   </td>\n  </tr>\n  <tr>\n   <td>fill_mouse_on(couleur:str)\n   </td>\n   <td>Change la couleur des formes quand on passe la souris dessus. Non actif par défaut.\n   </td>\n  </tr>\n  <tr>\n   <td>noFill_mouse_on()\n   </td>\n   <td>annule l\'effet de fill_mouse_on()\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click_down()\n   </td>\n   <td>renvoie True lors du passage de relâché à appuyé du bouton de la souris.\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click_up()\n   </td>\n   <td>renvoie True lors du passage de appuyé à relâché du bouton de la souris.\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_click()\n   </td>\n   <td>idem mouseIsPressed()\n   </td>\n  </tr>\n  <tr>\n   <td>mouse_wheel_state()\n   </td>\n   <td>retourne 1 si la roulette de la souris est tournée vers l\'avant, -1 vers l\'arrière et 0 si elle est immobile.\n   </td>\n  </tr>\n</table>\n\n\n\n## Mathématiques\n\n\n### Angles\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>angleMode(mode_angle:str)\n   </td>\n   <td>Définit l\'unité de mesure des angles. \\\n \'rad\' les angles des fonctions trigonométriques seront pris comme des radians (défaut) \\\n \'deg\' les angles des fonctions trigonométriques seront pris comme des degrés \\\n\'grd\' les angles des fonctions trigonométriques seront pris comme des grades \\\nUne exception est levée en cas d\'erreur de paramètre\n<p>\nsi mode_angle == "" la valeur de mode est retournée (str)\n   </td>\n  </tr>\n  <tr>\n   <td>cos(), sin(), tan(), acos(),asin(),atan(),atan2()\n   </td>\n   <td>Fonctions trigonométriques usuelles l\'unité considérée sera celle choisie avec angleMode(). atan2 : même fonctionnement que la fonction math.atan2 mais l\'unité de l\'angle retourné dépend  de angleMode()  \n   </td>\n  </tr>\n  <tr>\n   <td>degrees(mesure) \\\nradians(mesure) \\\ngrades(mesure)\n   </td>\n   <td>Convertit une mesure d\'angle en degrés, en radians ou en grades. l\'unité de mesure dépend de angleMode(). \n   </td>\n  </tr>\n  <tr>\n   <td>HALF_PI, PI, QUARTER_PI, TWO_PI\n   </td>\n   <td>Constantes permettant respectivement d\'approcher les valeurs de π/2, π, π/4, 2π\n   </td>\n  </tr>\n</table>\n\n\n\n### Géométrie\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>dist(x1,y1,x2,y2)\n   </td>\n   <td>retourne la distance entre deux points\n   </td>\n  </tr>\n  <tr>\n   <td>midPoint(x1, y1, x2, y2)\n   </td>\n   <td>retourne le milieu d\'un segment défini par deux points\n   </td>\n  </tr>\n</table>\n\n\n\n## Images\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>loadImage(chemin)\n   </td>\n   <td>Charge une image à partir d\'un chemin et crée un objet Image. Si nécessaire, l\'image peut être préchargée en plaçant l\'appel à la fonction loadImage en debut de programme.\n   </td>\n  </tr>\n  <tr>\n   <td>loadImages((liste_images:list[str],sens=0) ->Image:\n   </td>\n   <td>Retourne une surface qui est l\'assemblage de toutes les images\n    de la liste. Si sens = 1 les images sont assemblées verticalement\n    et horizontalement si sens =0. Ex: loadImages(["image1.png","image2.jpg"])\n   </td>\n  </tr>\n  <tr>\n   <td>background(Image)\n   </td>\n   <td>Affiche une Image en fond d\'écran\n   </td>\n  </tr>\n  <tr>\n   <td>image(image, x, y)\n   </td>\n   <td>Affiche une Image en plaçant le pixel en haut à gauche au point de coordonnées (x, y) dans la zone de dessin.\n   </td>\n  </tr>\n  <tr>\n   <td>copy_image(picture: Image, rect=None) -> Image\n   </td>\n   <td>retourne une copie de picture ou une partie de picture au dimensions de rect\n   </td>\n  </tr>\n  <tr>\n   <td>get_pixel_color(picture: Image, pos: tuple) -> tuple\n   </td>\n   <td>retourne la valeur de la couleur d\'un pixel d\'une image (picture)\n<p>\nsous la forme d\'un tuple\n   </td>\n  </tr>\n  <tr>\n   <td>resize_image(picture:Image,size : tuple\n   </td>\n   <td>retourne une image redimensionné en fonction de size : (largeur,hauteur) \n   </td>\n  </tr>\n</table>\n\n\n\n## Transformations\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>translate(x,y)\n   </td>\n   <td>applique une translation à toutes les fonctions de dessin et d\'image. x et y sont des valeurs relatives qui s\'ajoutent aux translations précédentes.\n<p>\nLa translation est remise à zéro avant chaque exécution de la fonction draw().\n   </td>\n  </tr>\n  <tr>\n   <td>get_translate()\n   </td>\n   <td>retourne la valeur de la translation sous la forme d\'un tuple (x,y)\n   </td>\n  </tr>\n  <tr>\n   <td>init_translate()\n   </td>\n   <td>Force la remise à zéro de la translation. (A utiliser dans la fonction draw() en cas de besoin \n   </td>\n  </tr>\n  <tr>\n   <td>rotate(angle,axis)\n   </td>\n   <td>applique une rotation &lt;angle> par rapport à &lt;axis>. à toutes les fonctions de dessin et d\'image. angle est une valeur absolue. Par défaut axis vaut (0,0). Cette fonction retourne la valeur précédente prise par la fonction sous la forme d\'un tuple.\n   </td>\n  </tr>\n  <tr>\n   <td>flip_h(axe_h)\n   </td>\n   <td>entraîne une symétrie horizontale par rapport à la droite y = axe_h\n   </td>\n  </tr>\n  <tr>\n   <td>flip_v(axe_v)\n   </td>\n   <td>entraîne une symétrie verticale par rapport à la droite x = axe_v\n   </td>\n  </tr>\n</table>\n\n\n\n## Temporisations\n\n\n\n<table>\n  <tr>\n   <td><strong>fonctions</strong>\n   </td>\n   <td><strong>description</strong>\n   </td>\n  </tr>\n  <tr>\n   <td>t=Tempo(duree_ms)\n   </td>\n   <td>t=Tempo(1000) créer un objet de temporisation t de durée 1000 ms qui se relance indéfiniment. \n    <img src="./images/image2.png">\n   </td>\n  </tr>\n  <tr>\n   <td>t.fin()\n   </td>\n   <td>renvoie True lorsque la temporisation est terminée. Pour notre exemple au bout de 500 ms.\n   </td>\n  </tr>\n  <tr>\n   <td>t.is_on()\n   </td>\n   <td>renvoie True si la temporisation est à on.\n   </td>\n  </tr>\n  <tr>\n   <td>t.is_off()\n   </td>\n   <td>renvoie True si la temporisation est à off.\n   </td>\n  </tr>\n  <tr>\n   <td>t.set_tempo(duree_ms)\n   </td>\n   <td>permet de réinitialiser la temporisation avec une nouvelle valeur.\n   </td>\n  </tr>\n  <tr>\n   <td>t.reset()\n   </td>\n   <td>force le redémarrage de la temporisation.\n   </td>\n  </tr>\n   <td>t=Monostable(duree_ms)\n   </td>\n   <td>t=Monostable(500) créer un objet de temporisation t de durée 500 ms qui ne se relance qu\'après execution de la methode reset() \n   </td>\n<tr>\n   <td>t=Pwm(500,25) \n    </td>\n    <td>\n    créer un objet générateur de signaux carré de période 500 ms et de rapport cyclique 25% \n   </td>\n  </tr>\n</table>\n\nComme les objets Monostable et Pwm héritent de Tempo ils en possèdent les méthodes.\n\n# Tutoriel Interface homme Machine\n\n\nl’IHM d’un programme permet à l’utilisateur d’interagir avec celui-ci.\n\nEn mode console les instructions print et input permettent de réaliser une interaction sommaire entre le programme et l’utilisateur.\n\nEn mode graphique l’interaction sera plus poussée.\n\n\n## IHM en python avec LikeProcessing\n\n\n### à faire vous même 1\n\nTaper le code suivant dans un nouveau fichier dans votre ide préféré :\n\n\n```\nfrom likeprocessing.processing import *\n\nihm = IhmScreen()\n\ndef setup():\n   createCanvas(400, 200)\n   ihm.init()\n   background("grey")\ndef compute():\nihm.scan_events()\n\n\ndef draw():\nihm.draw()\n\n\nrun(globals())\n```\n\n\nQuand vous exécutez ce code une fenêtre fonctionnelle vide apparaît.\n\n\n## Ajouter des Widgets à l’intérieur de la fenêtre.\n\nNous allons ajouter du texte dans la fenêtre.\n\n\n### à faire vous même 2\n\nAjouter le code suivant :\n\n\n```\netiquette1 = Label(ihm, (10, 10, 0, 0), "notre premier texte")\n```\n\n\n et lancer le programme. Que se passe-t-il ?\n\nMaintenant ajouter\n\n\n```\nihm.addObjet(etiquette1)\n```\n\n\n et lancer le programme. Que se passe-t-il ?\n\nAjouter : \n\n\n```\nihm.pack(["obj_1"])\n\n```\n\n\nQue se passe-t-il ?\n\nEssayer pack(margin_left=10) , pack(margin_right=10)\n\nAjouter une étiquette2 à la fenêtre.\n\n\n```\netiquette2 = Label(ihm, (10, 10, 0, 0), "etiquette2")\nihm.addObjet(etiquette2)\n```\n\n\nOù se place-t-elle sans utiliser **pack** ?\n\nEssayer avec la méthode pack et conclure.\n\nRemarque :\n\non peut utiliser la méthode addObjet en lui passant une liste d\'objet  \n\n\n```\nihm.addObjet([texte,entry, bouton])\n```\n\n\n\n## Interaction des éléments (widget) avec l’utilisateur.\n\nOn souhaite réaliser interface suivante qui contient :\n\n\n\n![](./images/image3.png)\n\nune étiquette (Label) donnant une explication à l’utilisateur, une zone de texte modifiable (LineEdit) et un bouton (Bouton) qui permettra de changer le titre de la fenêtre par le texte entré par l’utilisateur.\n\n\n```\netiquette = Label(ihm, (10, 10, 0, 0), "Modifier le texte et appuyer sur le bouton")\ntexte = LineEdit(ihm,(10,30,100,30),"")\nbouton = Bouton(ihm, (10, 60, 100, 30), "Changer le titre")\nihm.addObjet([etiquette,texte, bouton])\nihm.pack(["obj_1","obj_2","obj_3"])\n```\n\n\nn’oubliez pas d’utiliser les méthode addObjet() et pack()\n\nLorsque vous lancez le programme, que se passe-t-il ?\n\nModifier votre programme en complétant la création du bouton avec :\n\n\n```\ncommand=lambda : title(texte.text())\n```\n\n\ntexte.text() permet de récupérer le texte écrit par l’utilisateur.\n\nlambda permet de définir une fonction sur une ligne (le paramètre **command** à besoin d’une fonction comme valeur). On peut aussi donner le nom d\'une fonction que l\'on aura déjà créé.\n\nTester votre programme et modifier les paramètres de pack() en utilisant expand="x",pady=10,padx=10 pour obtenir la fenêtre ci-dessus (vous pouvez changer la hauteur de la fenêtre).\n\n\n## Précision sur l\'objet IhmScreen\n\nL\'objet IhmScreen possède plusieurs méthodes pour gérer l\'interface graphique:\n\naddObjet permet d\'ajouter des widgets à l\'interface. Si les objets n\'ont pas de nom (paramètre nom non renseigné) la méthode les nomme "obj_1", "obj_2",... \n\nobjet_by_name(nom_objet) permet de récupérer l\'objet de l\'interface pour par exemple changer sa couleur, récupérer la valeur du texte d\'un LineEdit ou changer le **text()** d\'un Label...\n\nEx : \n\n\n```\nihm.addObjet(LineEdit(ihm,(10,30,100,30),""),"texte")\n```\n\n\nCette commande ajoute à l\'interface un champ modifiable qui sera appelé "texte" \n\nprint(ihm.objet_by_name("texte").text()) affichera sur le console la valeur du champ.\n\nOn peut si on le souhaite supprimer un objet : ihm.delObjet(nom_objet) ou simplement le rendre invisible avec ihm.objet_by_name(nom_objet).visible = False\n\n\n## Création d’une calculatrice\n\nOn désire réaliser l’interface suivante :\n\nIl faut créer des boutons pour chaque touche ainsi qu’une étiquette pour simuler l’écran de la calculatrice.\n\n\n```\ntouche = [["1","2","3","*"],\n         ["4","5","6","/"],\n         ["7","8","9","+"],\n         ["0",".","²","-"],\n         ["(",")","=","AC"]]\n\nfor i in range(5):\n   for j in range(4):\n       ihm.addObjet(Bouton(None, (10+.....*40, 50+.....*40, 40, 40), touche[i][j], command=lambda v=touche[i][j]: calcule(v)))\n```\n\n\nla dernière ligne peut être remplacer par :\n\n\n```\nihm.addObjet(Bouton(None, (10+.....*40, 50+.....*40, 40, 40), touche[i][j], command=calcule, name = touche[i][j])) \n```\n\n\nce qui évite d\'utiliser la fonction lambda.\n\nLe paramètre **name** sera envoyé à la fonction **calcule**.\n\n\n### à faire vous même 3\n\ncréer l’IHM de la calculatrice.\n\n\n\n\n\n![](./images/image4.png)\n\n\n### à faire vous même 4\n\nRéalisation de l’interface graphique d\'un logiciel de dessin\n\nOn veut créer l’IHM du logiciel de dessin my_paint dont le code est le suivant:\n\n\n```\nfrom likeprocessing.processing import *\n\nforme = "cercle"\ncouleur = "blue"\npoint1 = None\nfigure = []\n\n\ndef draw_figure():\n   for f in figure:\n       largeur = abs(f[1][0] - f[2][0])\n       hauteur = abs(f[1][1] - f[2][1])\n       if f[0] == "rectangle":\n           rect(*f[1],largeur,hauteur,fill=f[3])\n       elif f[0] == "ligne":\n           line(*f[1],*f[2],stroke=f[3])\n       elif f[0] == "cercle":\n           circle(*f[1],dist(*f[1],*f[2]),fill=f[3],center_mode="center")\n\n\ndef setup():\n   createCanvas(400, 200,True)\n   background("grey")\n   title("my_paint")\n\n\ndef compute():\n   global point1\n   if mouse_click_down():\n       if point1 is None:\n           point1 = mouseXY()\n           figure.append([forme, point1, point1, couleur])\n   if len(figure)>0 and mouseIsPressed():\n       figure[-1][2] = mouseXY()\n   if mouse_click_up():\n       figure[-1][2] = mouseXY()\n       point1 = None\n\n\n\ndef draw():\n   draw_figure()\n\n\nrun(globals())\n```\n\n\nforme peut prendre les valeurs suivantes : "rectangle","cercle","ligne" et couleur les couleurs acceptés par likeprocessing.\n\nl\'interface doit permettre :\n\n- afficher le type de forme en cours\n\n- de changer le type de forme,\n\n- couleur des figures,\n\n- la couleur du fond,\n\n- effacer la dernière forme,\n\n- effacer le dessin,\n\n\n## Utilisation des boîtes de dialogues d\'information (Show)  et des boîtes de dialogues de questionnement (Ask…)\n\nCes boîtes ont un comportement bloquant c\'est à dire que seule l\'interaction avec avec la boite est prise en compte : les fonctions compute(), draw(), exit() ne sont plus appelées.\n\n\n```\nShowInfo(ihm, "Ceci est une \\ninformation").response()\n```\n\n\n\n![](./images/image5.png)\n\n\n```\nShowWarning(ihm, "Ceci est un \\navertissement").response()\n```\n\n\n![](./images/image6.png)\n\n\n\n```\nShowError(ihm, "Ceci est une \\nerreur").response()\n```\n\n\n![](./images/image7.png)\n\n\n\n```\nAskYesNo(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response()\n```\n\n\n\n![](./images/image8.png)\n\n\n\n```\nAskOkCancel(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response()\n```\n\n\n\n![](images/image9.png)\n\n\n\n```\nAskRetriyCancel(ihm, "Voulez-vous tenter\\nà nouveau\\nvotre chance").response()\n```\n\n\n![](./images/image10.png)\n\n\n\n### Utilisation: \n\nles bouton sont numéroté de la gauche vers la droite (0,1) .Le clique sur croix de la boîte retourne la valeur 4 \n\n\n```\nif AskYesNo(ihm, "Voulez-vous tenter\\nà nouveau\\nvotre chance").response() == 0:\n```\n\n\nAvec le code ci-dessus, la condition sera vraie si le bouton de gauche est cliqué. \n\nExemple d\'utilisation d\'une boîte et de la fonction exit().\n\nLa fonction exit() est une fonction facultative (comme compute) destinée à simplifier la sortie du programme que ce soit par l\'intermédiaire d\'un bouton dédié ou par l\'utilisation de la croix de fermeture de la fenêtre.\n\nSans cette fonction lorsque que l\'on appuie sur la croix la fonction **set_quit(True)** est exécutée ce qui à pour effet de fermer immédiatement l\'application.\n\n le code suivant qui utilise la fonction exit() permet de faire les choses avec plus d\'élégance : \n\n\n```\ndef exit():\n   set_quit(False)\n   if AskYesNo(ihm, "Voulez-vous Vraiment\\nquitter le jeu").response() == 0:\n       set_quit(True)\n```\n\n\najout d\'un bouton dédié à la fermeture du programme : \n\n\n```\nihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",\n                   font_size=20, command=lambda : set_quit(True) ), bp_quitter")\n```\n\n\nOn peut aussi passer par une fonction intermédiaire:\n\n\n```\ndef bp_quitter():\n   set_quit(True)\n\nihm.addObjet(Bouton(ihm, (0, 0, 100, 0), "Quitter",\n                   font_size=20, command=bp_quitter), "bp_quitter")\n```\n\n\n \n\n**Remarque**: on peut rendre si nécessaire la croix de la fenêtre likeprocessing inactive avec la fonction  **disabled_quit_cross(). **La fonction** enabled_quit_cross()** permet de la réactivée.\n\n \n',
     'author': 'Pierre Lemaitre',
     'author_email': 'oultetman@sfr.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `likeprocessing-0.1.7.4.1/PKG-INFO` & `likeprocessing-0.1.7.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: likeprocessing
-Version: 0.1.7.4.1
+Version: 0.1.7.4.2
 Summary: Like processing library with pygame
 Author: Pierre Lemaitre
 Author-email: oultetman@sfr.fr
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

