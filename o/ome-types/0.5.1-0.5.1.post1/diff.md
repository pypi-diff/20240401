# Comparing `tmp/ome_types-0.5.1.tar.gz` & `tmp/ome_types-0.5.1.post1.tar.gz`

## Comparing `ome_types-0.5.1.tar` & `ome_types-0.5.1.post1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    29354 2020-02-02 00:00:00.000000 ome_types-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/generator.py
--rw-r--r--   0        0        0     8621 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/main.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/overrides.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/transformer.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/templates/class.jinja2
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/templates/docstrings.numpy.jinja2
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_autogen/templates/enum.jinja2
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/__init__.py
--rw-r--r--   0        0        0    20049 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_conversion.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_pydantic_compat.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/etree_fixes.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/napari.yaml
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/py.typed
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/units.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_collections.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_kinded.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_map_mixin.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_mixins/_validators.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_vendor/__init__.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_vendor/_pydantic_color_v1.py
--rw-r--r--   0        0        0    24647 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/_vendor/_pydantic_color_v2.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/model/_converters.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2003-FC-to-2008-09.xsl
--rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2007-06-to-2008-09.xsl
--rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2008-02-to-2008-09.xsl
--rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2008-09-to-2009-09.xsl
--rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2009-09-to-2010-04.xsl
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2010-04-to-2010-06.xsl
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2010-06-to-2011-06.xsl
--rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2011-06-to-2012-06.xsl
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2012-06-to-2013-06.xsl
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2013-06-to-2015-01.xsl
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/ome_types/transforms/2015-01-to-2016-06.xsl
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/config.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/pydantic_compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.5.1/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.5.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.5.1/LICENSE
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 ome_types-0.5.1/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.5.1/hatch_build.py
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 ome_types-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 ome_types-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    29354 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/generator.py
+-rw-r--r--   0        0        0     8621 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/main.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/overrides.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/transformer.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/templates/class.jinja2
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/templates/docstrings.numpy.jinja2
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_autogen/templates/enum.jinja2
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/__init__.py
+-rw-r--r--   0        0        0    20049 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_pydantic_compat.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/etree_fixes.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/napari.yaml
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/py.typed
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/units.py
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_collections.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_kinded.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_map_mixin.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_mixins/_validators.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_vendor/__init__.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_vendor/_pydantic_color_v1.py
+-rw-r--r--   0        0        0    24647 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/_vendor/_pydantic_color_v2.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2003-FC-to-2008-09.xsl
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2007-06-to-2008-09.xsl
+-rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2008-02-to-2008-09.xsl
+-rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2008-09-to-2009-09.xsl
+-rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2009-09-to-2010-04.xsl
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2010-04-to-2010-06.xsl
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2010-06-to-2011-06.xsl
+-rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2011-06-to-2012-06.xsl
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2012-06-to-2013-06.xsl
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2013-06-to-2015-01.xsl
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/ome_types/transforms/2015-01-to-2016-06.xsl
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/config.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/LICENSE
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/hatch_build.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/pyproject.toml
+-rw-r--r--   0        0        0    10406 2020-02-02 00:00:00.000000 ome_types-0.5.1.post1/PKG-INFO
```

### Comparing `ome_types-0.5.1/CHANGELOG.md` & `ome_types-0.5.1.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/_util.py` & `ome_types-0.5.1.post1/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/generator.py` & `ome_types-0.5.1.post1/src/ome_autogen/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/main.py` & `ome_types-0.5.1.post1/src/ome_autogen/main.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/overrides.py` & `ome_types-0.5.1.post1/src/ome_autogen/overrides.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/transformer.py` & `ome_types-0.5.1.post1/src/ome_autogen/transformer.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/templates/class.jinja2` & `ome_types-0.5.1.post1/src/ome_autogen/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_autogen/templates/enum.jinja2` & `ome_types-0.5.1.post1/src/ome_autogen/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/__init__.py` & `ome_types-0.5.1.post1/src/ome_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_conversion.py` & `ome_types-0.5.1.post1/src/ome_types/_conversion.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_pydantic_compat.py` & `ome_types-0.5.1.post1/src/ome_types/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/etree_fixes.py` & `ome_types-0.5.1.post1/src/ome_types/etree_fixes.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/ome-2016-06.xsd` & `ome_types-0.5.1.post1/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/units.py` & `ome_types-0.5.1.post1/src/ome_types/units.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/widget.py` & `ome_types-0.5.1.post1/src/ome_types/widget.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_base_type.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_base_type.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_collections.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_collections.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_ids.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_ids.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_instrument.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_kinded.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_kinded.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_map_mixin.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_map_mixin.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_ome.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_ome.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_reference.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_mixins/_validators.py` & `ome_types-0.5.1.post1/src/ome_types/_mixins/_validators.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_vendor/__init__.py` & `ome_types-0.5.1.post1/src/ome_types/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_vendor/_pydantic_color_v1.py` & `ome_types-0.5.1.post1/src/ome_types/_vendor/_pydantic_color_v1.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/_vendor/_pydantic_color_v2.py` & `ome_types-0.5.1.post1/src/ome_types/_vendor/_pydantic_color_v2.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/model/__init__.py` & `ome_types-0.5.1.post1/src/ome_types/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/model/_color.py` & `ome_types-0.5.1.post1/src/ome_types/model/_color.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/model/_converters.py` & `ome_types-0.5.1.post1/src/ome_types/model/_converters.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/model/simple_types.py` & `ome_types-0.5.1.post1/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2003-FC-to-2008-09.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2003-FC-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2007-06-to-2008-09.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2007-06-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2008-02-to-2008-09.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2008-02-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2008-09-to-2009-09.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2008-09-to-2009-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2009-09-to-2010-04.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2009-09-to-2010-04.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2010-04-to-2010-06.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2010-04-to-2010-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2010-06-to-2011-06.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2010-06-to-2011-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2011-06-to-2012-06.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2011-06-to-2012-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2012-06-to-2013-06.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2012-06-to-2013-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2013-06-to-2015-01.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2013-06-to-2015-01.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/ome_types/transforms/2015-01-to-2016-06.xsl` & `ome_types-0.5.1.post1/src/ome_types/transforms/2015-01-to-2016-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/xsdata_pydantic_basemodel/config.py` & `ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/config.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/src/xsdata_pydantic_basemodel/pydantic_compat.py` & `ome_types-0.5.1.post1/src/xsdata_pydantic_basemodel/pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/.gitignore` & `ome_types-0.5.1.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/LICENSE` & `ome_types-0.5.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/README.md` & `ome_types-0.5.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.5.1/pyproject.toml` & `ome_types-0.5.1.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic >=1.9.0", "pydantic-compat >=0.1.0", "xsdata >=23.6"]
+dependencies = ["pydantic >=1.9.0", "pydantic-compat >=0.1.0", "xsdata >=23.6,<24.4"]
 
 [project.urls]
 Source = "https://github.com/tlambert03/ome-types"
 Tracker = "https://github.com/tlambert03/ome-types/issues"
 Documentation = "https://ome-types.readthedocs.io/en/latest/"
 
 [project.entry-points."napari.manifest"]
```

### Comparing `ome_types-0.5.1/PKG-INFO` & `ome_types-0.5.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ome-types
-Version: 0.5.1
+Version: 0.5.1.post1
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: pydantic-compat>=0.1.0
 Requires-Dist: pydantic>=1.9.0
-Requires-Dist: xsdata>=23.6
+Requires-Dist: xsdata<24.4,>=23.6
 Provides-Extra: build
 Requires-Dist: ruff==0.3.0; extra == 'build'
 Requires-Dist: xsdata[cli]==24.2.1; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == 'docs'
```

