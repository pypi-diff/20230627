# Comparing `tmp/plotnine_prism-0.2.0.tar.gz` & `tmp/plotnine_prism-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotnine_prism-0.2.0.tar", max compression
+gzip compressed data, was "plotnine_prism-0.3.0.tar", max compression
```

## Comparing `plotnine_prism-0.2.0.tar` & `plotnine_prism-0.3.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0     1771 2023-02-06 23:43:01.667002 plotnine_prism-0.2.0/README.md
--rw-r--r--   0        0        0     1041 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/__init__.py
--rw-r--r--   0        0        0     5724 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/guide.py
--rw-r--r--   0        0        0     1771 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/pal.py
--rw-r--r--   0        0        0     1215 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/scale.py
--rw-r--r--   0        0        0     5309 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/_color_palettes.toml
--rw-r--r--   0        0        0     5309 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/_fill_palettes.toml
--rw-r--r--   0        0        0     1715 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/_shape_palettes.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/autumn_leaves.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/beer_and_ales.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/black_and_white.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/blueprint.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/candy_bright.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/candy_soft.toml
--rw-r--r--   0        0        0     2350 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/colorblind_safe.toml
--rw-r--r--   0        0        0     6565 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/colors.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/diazo.toml
--rw-r--r--   0        0        0     3535 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/earth_tones.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/evergreen.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/fir.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/flames.toml
--rw-r--r--   0        0        0     4141 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/floral.toml
--rw-r--r--   0        0        0     3535 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/greenwash.toml
--rw-r--r--   0        0        0     2350 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/inferno.toml
--rw-r--r--   0        0        0     2350 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/magma.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/mustard_field.toml
--rw-r--r--   0        0        0     3535 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/muted_rainbow.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/neon.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/ocean.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/office.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/pastels.toml
--rw-r--r--   0        0        0     2350 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/pearl.toml
--rw-r--r--   0        0        0     2350 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/plasma.toml
--rw-r--r--   0        0        0     3535 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/prism_dark.toml
--rw-r--r--   0        0        0     3535 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/prism_light.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/purple_passion.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/quiet.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/shades_of_gray.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/spring.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/stained_glass.toml
--rw-r--r--   0        0        0     2056 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/starry.toml
--rw-r--r--   0        0        0     3535 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/summer.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/sunny_garden.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/the_blues.toml
--rw-r--r--   0        0        0     2350 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/viridis.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/warm_and_sunny.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/warm_pastels.toml
--rw-r--r--   0        0        0     2056 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/waves.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/winter_bright.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/winter_soft.toml
--rw-r--r--   0        0        0     3232 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/schemes/wool_muffler.toml
--rw-r--r--   0        0        0     8837 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/theme.py
--rw-r--r--   0        0        0     2997 2023-02-06 23:43:01.683006 plotnine_prism-0.2.0/plotnine_prism/themeable.py
--rw-r--r--   0        0        0      853 2023-02-06 23:43:01.687007 plotnine_prism-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 plotnine_prism-0.2.0/setup.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 plotnine_prism-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1771 2023-06-27 07:11:30.869574 plotnine_prism-0.3.0/README.md
+-rw-r--r--   0        0        0     1041 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/__init__.py
+-rw-r--r--   0        0        0     5767 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/guide.py
+-rw-r--r--   0        0        0     1771 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/pal.py
+-rw-r--r--   0        0        0     3903 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/scale.py
+-rw-r--r--   0        0        0     5309 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/_color_palettes.toml
+-rw-r--r--   0        0        0     5309 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/_fill_palettes.toml
+-rw-r--r--   0        0        0     1715 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/_shape_palettes.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/autumn_leaves.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/beer_and_ales.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/black_and_white.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/blueprint.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/candy_bright.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/candy_soft.toml
+-rw-r--r--   0        0        0     2350 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/colorblind_safe.toml
+-rw-r--r--   0        0        0     6565 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/colors.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/diazo.toml
+-rw-r--r--   0        0        0     3535 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/earth_tones.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/evergreen.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/fir.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/flames.toml
+-rw-r--r--   0        0        0     4141 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/floral.toml
+-rw-r--r--   0        0        0     3535 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/greenwash.toml
+-rw-r--r--   0        0        0     2350 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/inferno.toml
+-rw-r--r--   0        0        0     2350 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/magma.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/mustard_field.toml
+-rw-r--r--   0        0        0     3535 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/muted_rainbow.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/neon.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/ocean.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/office.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/pastels.toml
+-rw-r--r--   0        0        0     2350 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/pearl.toml
+-rw-r--r--   0        0        0     2350 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/plasma.toml
+-rw-r--r--   0        0        0     3535 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/prism_dark.toml
+-rw-r--r--   0        0        0     3535 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/prism_light.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/purple_passion.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/quiet.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/shades_of_gray.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/spring.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/stained_glass.toml
+-rw-r--r--   0        0        0     2056 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/starry.toml
+-rw-r--r--   0        0        0     3535 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/summer.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/sunny_garden.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/the_blues.toml
+-rw-r--r--   0        0        0     2350 2023-06-27 07:11:30.901574 plotnine_prism-0.3.0/plotnine_prism/schemes/viridis.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/schemes/warm_and_sunny.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/schemes/warm_pastels.toml
+-rw-r--r--   0        0        0     2056 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/schemes/waves.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/schemes/winter_bright.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/schemes/winter_soft.toml
+-rw-r--r--   0        0        0     3232 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/schemes/wool_muffler.toml
+-rw-r--r--   0        0        0     7736 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/theme.py
+-rw-r--r--   0        0        0     3051 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/plotnine_prism/themeable.py
+-rw-r--r--   0        0        0      853 2023-06-27 07:11:30.905574 plotnine_prism-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 plotnine_prism-0.3.0/PKG-INFO
```

### Comparing `plotnine_prism-0.2.0/README.md` & `plotnine_prism-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/__init__.py` & `plotnine_prism-0.3.0/plotnine_prism/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,8 @@
     "guide_prism",
     "guide_prism_minor",
     # "guide_prism_bracket",
     "guide_prism_offset",
     "guide_prism_offset_minor",
 )
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
```

### Comparing `plotnine_prism-0.2.0/plotnine_prism/guide.py` & `plotnine_prism-0.3.0/plotnine_prism/guide.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         """Apply the arguments"""
         xaxis_position = plot.axs[0].xaxis.get_label_position()
         yaxis_position = plot.axs[0].yaxis.get_label_position()
         gca = plot.axs[0].axes
 
         if self.aesthetic == "x":
             major_locs = gca.get_xticks()
-            minor_locs = gca.xaxis.get_minorticklocs()
+            minor_locs = gca.get_xticks(minor=True)
             if yaxis_position == "left":
                 offset = (
                     self.offset
                     if major_locs[0] > minor_locs[0]
                     else self.offset / 2
                 )
             else:
@@ -57,27 +57,28 @@
                     else self.offset / 2
                 )
             gca.spines[yaxis_position].set_position(("outward", offset))
             gca.set_xlim(min(major_locs), max(major_locs))
             gca.xaxis.set_minor_locator(NullLocator())
         else:
             major_locs = gca.get_yticks()
-            minor_locs = gca.yaxis.get_minorticklocs()
+            minor_locs = gca.get_yticks(minor=True)
             if xaxis_position == "bottom":
                 offset = (
                     self.offset
-                    if major_locs[0] > minor_locs[0]
+                    if len(minor_locs) > 0 and major_locs[0] > minor_locs[0]
                     else self.offset / 2
                 )
             else:
                 offset = (
                     self.offset
-                    if major_locs[-1] < minor_locs[-1]
+                    if len(minor_locs) > 0 and major_locs[-1] < minor_locs[-1]
                     else self.offset / 2
                 )
+
             gca.spines[xaxis_position].set_position(("outward", offset))
             gca.set_ylim(min(major_locs), max(major_locs))
             gca.yaxis.set_minor_locator(NullLocator())
 
     def merge(self, other):
         """Simply discards the other guide"""
         return self
```

### Comparing `plotnine_prism-0.2.0/plotnine_prism/pal.py` & `plotnine_prism-0.3.0/plotnine_prism/pal.py`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/_color_palettes.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/_color_palettes.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/_fill_palettes.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/_fill_palettes.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/_shape_palettes.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/_shape_palettes.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/autumn_leaves.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/autumn_leaves.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/beer_and_ales.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/beer_and_ales.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/black_and_white.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/black_and_white.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/blueprint.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/blueprint.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/candy_bright.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/candy_bright.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/candy_soft.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/candy_soft.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/colorblind_safe.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/colorblind_safe.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/colors.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/colors.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/diazo.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/diazo.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/earth_tones.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/earth_tones.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/evergreen.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/evergreen.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/fir.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/fir.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/flames.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/flames.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/floral.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/floral.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/greenwash.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/greenwash.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/inferno.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/inferno.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/magma.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/magma.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/mustard_field.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/mustard_field.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/muted_rainbow.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/muted_rainbow.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/neon.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/neon.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/ocean.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/ocean.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/office.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/office.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/pastels.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/pastels.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/pearl.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/pearl.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/plasma.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/plasma.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/prism_dark.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/prism_dark.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/prism_light.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/prism_light.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/purple_passion.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/purple_passion.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/quiet.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/quiet.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/shades_of_gray.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/shades_of_gray.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/spring.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/spring.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/stained_glass.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/stained_glass.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/starry.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/starry.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/summer.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/summer.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/sunny_garden.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/sunny_garden.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/the_blues.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/the_blues.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/viridis.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/viridis.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/warm_and_sunny.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/warm_and_sunny.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/warm_pastels.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/warm_pastels.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/waves.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/waves.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/winter_bright.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/winter_bright.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/winter_soft.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/winter_soft.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/schemes/wool_muffler.toml` & `plotnine_prism-0.3.0/plotnine_prism/schemes/wool_muffler.toml`

 * *Files identical despite different names*

### Comparing `plotnine_prism-0.2.0/plotnine_prism/themeable.py` & `plotnine_prism-0.3.0/plotnine_prism/themeable.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,94 +10,94 @@
     axis_ticks_minor_y,
 )
 
 
 class axis_ticks_x(axis_ticks_major_x, axis_ticks_minor_x):
     """Themeable for ticks on x axis that is missing in plotnine"""
 
-    def apply(self, ax):
+    def apply_ax(self, ax):
         """Apply themeable to the axis"""
-        axis_ticks_major_x.apply(self, ax)
-        axis_ticks_minor_x.apply(self, ax)
+        axis_ticks_major_x.apply_ax(self, ax)
+        axis_ticks_minor_x.apply_ax(self, ax)
 
-    def blank(self, ax):
+    def blank_ax(self, ax):
         """When it's set blank"""
         axis_ticks_major_x.blank(self, ax)
         axis_ticks_minor_x.blank(self, ax)
 
 
 class axis_ticks_y(axis_ticks_major_y, axis_ticks_minor_y):
     """Themeable for ticks on y axis that is missing in plotnine"""
 
-    def apply(self, ax):
+    def apply_ax(self, ax):
         """Apply themeable to the axis"""
-        axis_ticks_major_y.apply(self, ax)
-        axis_ticks_minor_y.apply(self, ax)
+        axis_ticks_major_y.apply_ax(self, ax)
+        axis_ticks_minor_y.apply_ax(self, ax)
 
-    def blank(self, ax):
+    def blank_ax(self, ax):
         """When it's set blank"""
         axis_ticks_major_y.blank(self, ax)
         axis_ticks_minor_y.blank(self, ax)
 
 
 class prism_ticks_length_x(themeable_abc):
     """Themeable for ticks length on x axis"""
 
-    def apply(self, ax):
+    def apply_ax(self, ax):
         """Apply themeable to the axis"""
-        themeable_abc.apply(self, ax)
+        themeable_abc.apply_ax(self, ax)
 
         d = deepcopy(self.properties)
         with suppress(KeyError):
             length = d.pop("value")
             ax.xaxis.set_tick_params(
                 which="minor",
                 length=abs(length),
                 direction="in" if length < 0 else "out",
             )
 
         for tick in ax.xaxis.get_minor_ticks():
             tick.tick1line.set(**d)
 
-    def blank(self, ax):
+    def blank_ax(self, ax):
         """When it's set blank"""
         themeable_abc.blank(self, ax)
         ax.xaxis.set_tick_params(which="minor", bottom=False)
 
 
 class prism_ticks_length_y(themeable_abc):
     """Themeable for ticks length on y axis"""
 
-    def apply(self, ax):
+    def apply_ax(self, ax):
         """Apply themeable to the axis"""
-        themeable_abc.apply(self, ax)
+        themeable_abc.apply_ax(self, ax)
 
         d = deepcopy(self.properties)
         with suppress(KeyError):
             length = d.pop("value")
             ax.yaxis.set_tick_params(
                 which="minor",
                 length=abs(length),
                 direction="in" if length < 0 else "out",
             )
 
         for tick in ax.yaxis.get_minor_ticks():
             tick.tick1line.set(**d)
 
-    def blank(self, ax):
+    def blank_ax(self, ax):
         """When it's set blank"""
         themeable_abc.blank(self, ax)
         ax.yaxis.set_tick_params(which="minor", bottom=False)
 
 
 class prism_ticks_length(prism_ticks_length_x, prism_ticks_length_y):
     """Themeable for ticks length"""
 
-    def apply(self, ax):
+    def apply_ax(self, ax):
         """Apply themeable to the axis"""
-        prism_ticks_length_x.apply(self, ax)
-        prism_ticks_length_y.apply(self, ax)
+        prism_ticks_length_x.apply_ax(self, ax)
+        prism_ticks_length_y.apply_ax(self, ax)
 
-    def blank(self, ax):
+    def blank_ax(self, ax):
         """When it's set blank"""
         prism_ticks_length_x.blank(self, ax)
         prism_ticks_length_y.blank(self, ax)
```

### Comparing `plotnine_prism-0.2.0/PKG-INFO` & `plotnine_prism-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: plotnine-prism
-Version: 0.2.0
+Version: 0.3.0
 Summary: Prism themes for plotnine, inspired by ggprism
 License: GNU General Public License v2.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: diot (>=0.1,<0.2)
-Requires-Dist: plotnine (>=0.10,<0.11)
+Requires-Dist: diot (>=0.2,<0.3)
+Requires-Dist: plotnine (>=0.12,<0.13)
 Requires-Dist: rtoml (>=0.8,<0.9)
 Description-Content-Type: text/markdown
 
 # plotnine-prism
 
 Prism themes for [plotnine][1], inspired by [ggprism][2].
```

