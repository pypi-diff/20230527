# Comparing `tmp/feynml-0.1.7.tar.gz` & `tmp/feynml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynml-0.1.7.tar", max compression
+gzip compressed data, was "feynml-0.2.0.tar", max compression
```

## Comparing `feynml-0.1.7.tar` & `feynml-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-04-15 21:12:25.141286 feynml-0.1.7/LICENSE
--rw-r--r--   0        0        0     2359 2023-04-15 21:12:25.141286 feynml-0.1.7/README.md
--rw-r--r--   0        0        0      179 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/__init__.py
--rw-r--r--   0        0        0      986 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/connector.py
--rw-r--r--   0        0        0     6932 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/feynmandiagram.py
--rw-r--r--   0        0        0     3096 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/feynml.py
--rw-r--r--   0        0        0      651 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/id.py
--rw-r--r--   0        0        0        0 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/interface/__init__.py
--rw-r--r--   0        0        0     1563 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/interface/hepmc.py
--rw-r--r--   0        0        0     1569 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/interface/qgraf.py
--rw-r--r--   0        0        0      385 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/labeled.py
--rw-r--r--   0        0        0     1035 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/leg.py
--rw-r--r--   0        0        0      303 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/line.py
--rw-r--r--   0        0        0      563 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/momentum.py
--rw-r--r--   0        0        0     1385 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/particles.py
--rw-r--r--   0        0        0     3115 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/pdgid.py
--rw-r--r--   0        0        0      846 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/point.py
--rw-r--r--   0        0        0      207 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/propagator.py
--rw-r--r--   0        0        0      363 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/sourcing.py
--rw-r--r--   0        0        0     2749 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/styled.py
--rw-r--r--   0        0        0      364 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/targeting.py
--rw-r--r--   0        0        0     4182 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/types.py
--rw-r--r--   0        0        0      425 2023-04-15 21:12:25.141286 feynml-0.1.7/feynml/vertex.py
--rw-r--r--   0        0        0     1641 2023-04-15 21:12:26.821293 feynml-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 feynml-0.1.7/setup.py
--rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 feynml-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-27 19:29:52.352554 feynml-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2359 2023-05-27 19:29:52.352554 feynml-0.2.0/README.md
+-rw-r--r--   0        0        0      179 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/connector.py
+-rw-r--r--   0        0        0     4769 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/feynmandiagram.py
+-rw-r--r--   0        0        0     2496 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/feynml.py
+-rw-r--r--   0        0        0     2452 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/head.py
+-rw-r--r--   0        0        0      651 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/id.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/__init__.py
+-rw-r--r--   0        0        0     2636 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/hepmc.py
+-rw-r--r--   0        0        0     4709 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/lhe.py
+-rw-r--r--   0        0        0     1569 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/qgraf.py
+-rw-r--r--   0        0        0     1301 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/interface/util.py
+-rw-r--r--   0        0        0      385 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/labeled.py
+-rw-r--r--   0        0        0     1035 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/leg.py
+-rw-r--r--   0        0        0      303 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/line.py
+-rw-r--r--   0        0        0      396 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/link.py
+-rw-r--r--   0        0        0      400 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/meta.py
+-rw-r--r--   0        0        0      563 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/momentum.py
+-rw-r--r--   0        0        0     1385 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/particles.py
+-rw-r--r--   0        0        0     3115 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/pdgid.py
+-rw-r--r--   0        0        0      846 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/point.py
+-rw-r--r--   0        0        0      207 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/propagator.py
+-rw-r--r--   0        0        0      349 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/shape.py
+-rw-r--r--   0        0        0     7878 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/sheet.py
+-rw-r--r--   0        0        0      363 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/sourcing.py
+-rw-r--r--   0        0        0     2839 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/styled.py
+-rw-r--r--   0        0        0      364 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/targeting.py
+-rw-r--r--   0        0        0      795 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/type.py
+-rw-r--r--   0        0        0      425 2023-05-27 19:29:52.352554 feynml-0.2.0/feynml/vertex.py
+-rw-r--r--   0        0        0      741 2023-05-27 19:29:52.356555 feynml-0.2.0/feynml/xml.py
+-rw-r--r--   0        0        0     1893 2023-05-27 19:29:53.856692 feynml-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 feynml-0.2.0/setup.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 feynml-0.2.0/PKG-INFO
```

### Comparing `feynml-0.1.7/LICENSE` & `feynml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/README.md` & `feynml-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/connector.py` & `feynml-0.2.0/feynml/connector.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/feynml.py` & `feynml-0.2.0/feynml/head.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,87 @@
 import logging
 import warnings
 from dataclasses import dataclass, field
 from importlib.metadata import version
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import cssutils
-from smpl_doc import doc
-from xsdata.formats.dataclass.parsers import XmlParser
-from xsdata.formats.dataclass.serializers import XmlSerializer
-from xsdata.formats.dataclass.serializers.config import SerializerConfig
-
-from feynml.feynmandiagram import FeynmanDiagram
-
-# We don't want to see the cssutils warnings, since we have custom properties
-cssutils.log.setLevel(logging.CRITICAL)
-
-
-feynml_version = version("feynml")
-
-
-@dataclass
-class Tool:
-    class Meta:
-        name = "tool"
-
-    # Deprecated to stay closer to html meta tags
-    @doc.deprecated("0.1.3", "Use feynml.feynml.Meta instead.")
-    def __init__(*args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    name: Optional[str] = field(default="feynml", metadata={"type": "Element"})
-    version: Optional[str] = field(
-        default=version("feynml"), metadata={"type": "Element"}
-    )
+import smpl_io.io as io
+from cssselect import GenericTranslator, SelectorError
+from lxml import etree
+
+from feynml.id import Identifiable
+from feynml.leg import Leg
+from feynml.link import Link
+from feynml.meta import Meta as alias_meta
+from feynml.propagator import Propagator
+from feynml.sheet import SheetHandler
+from feynml.styled import CSSSheet, Styled
+from feynml.type import get_default_sheet
+from feynml.vertex import Vertex
+from feynml.xml import XML
 
 
 @dataclass
-class Meta:
-    class Meta:
-        name = "meta"
-
-    name: Optional[str] = field(default="", metadata={"type": "Attribute"})
-    content: Optional[str] = field(default="", metadata={"type": "Attribute"})
-
-
-alias_meta = Meta
-
-
-@dataclass
-class Head:
+class Head(SheetHandler):
     class Meta:
         name = "head"
 
     metas: List[alias_meta] = field(
         default_factory=list,
         metadata={"name": "meta", "namespace": ""},
     )
-    description: Optional[str] = field(default="", metadata={"type": "Element"})
+    links: List[Link] = field(
+        default_factory=list,
+        metadata={"name": "link", "namespace": ""},
+    )
+    cached_links = {}
+    title: Optional[str] = field(default=None, metadata={"type": "Element"})
 
-    style: Optional[str] = field(default="", metadata={"type": "Element"})
+    # description: Optional[str] = field(default="", metadata={"type": "Element"})
+
+    # style: Optional[str] = field(default="", metadata={"type": "Element"})
+    style: CSSSheet = field(
+        default_factory=lambda: cssutils.parseString(""),
+        metadata={
+            "name": "style",
+            "type": "Element",
+        },
+    )
+
+    def get_link_dict(self, cached=True, cache=True):
+        """
+        Return a dictionary of resolved links.
+
+        If cached is True, then the cached resolved links are returned.
+        """
+        ret = {}
+        for m in self.links:
+            if m.ref in self.cached_links and cached:
+                ret[m.ref] = self.cached_links[m.ref]
+            else:
+                ret[m.ref] = io.read(m.href)
+                if cache:
+                    self.cached_links[m.ref] = ret[m.ref]
+        return ret
 
     def get_meta_dict(self):
         """
         Return a dictionary of meta tags.
         """
         return {m.name: m.content for m in self.metas}
 
-
-@dataclass
-class FeynML:
-    class Meta:
-        name = "feynml"
-
-    version: Optional[str] = field(
-        default=feynml_version, metadata={"name": "version", "type": "Attribute"}
-    )
-
-    # post init to check version
-    def __post_init__(self):
-        if self.version < feynml_version:
-            warnings.warn("FeynML version is older than this parser.")
-        elif self.version > feynml_version:
-            warnings.warn("FeynML version is newer than this parser.")
-
-        self.head.metas.append(Meta("feynml", version("feynml")))
-
-    head: Optional[Head] = field(
-        default=Head(), metadata={"name": "head", "namespace": "", "type": "Element"}
-    )
-
-    diagrams: List[FeynmanDiagram] = field(
-        default_factory=list,
-        metadata={"name": "diagram", "type": "Element", "namespace": ""},
-    )
-
-    def get_diagram(self, idd):
-        for d in self.diagrams:
-            if d.id == idd:
-                return d
-        return None
-
-    def to_xml(self) -> str:
-        """Return self as XML."""
-        config = SerializerConfig(pretty_print=True)
-        serializer = XmlSerializer(config=config)
-        return serializer.render(self)
-
-    @classmethod
-    def from_xml(cls, xml: str):
-        """Load self from XML."""
-        parser = XmlParser()
-        return parser.from_string(xml, cls)
+    def get_sheets(self):
+        sheets = []
+        sheets += super().get_sheets()
+        for k, v in self.get_link_dict().items():
+            if k == "stylesheet":
+                sheets += [v]
+        sheets += [self.style]
+        return sheets
+
+    def get_sheet(self):
+        return self.style
+
+    def with_sheet(self, sheet):
+        self.style = sheet
+        return self
```

### Comparing `feynml-0.1.7/feynml/id.py` & `feynml-0.2.0/feynml/id.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/interface/hepmc.py` & `feynml-0.2.0/feynml/interface/hepmc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,98 @@
+import pyhepmc
 from pyhepmc import GenEvent
 
 from feynml.feynmandiagram import FeynmanDiagram
+from feynml.feynml import FeynML, Head, Meta
 from feynml.leg import Leg
 from feynml.propagator import Propagator
 from feynml.vertex import Vertex
 
+from .util import leg_id_wrap, propagator_id_wrap, vertex_id_wrap
 
-def _vertex_id_wrap(idd):
-    return "Vertex" + str(idd).replace("-", "m")
+# TODO add momenta?
 
 
-def event_to_feynman(event: GenEvent):
+def hepmc_event_to_feynman(event: GenEvent) -> FeynmanDiagram:
+    """
+    Convert a GenEvent to a FeynmanDiagram.
+
+    Args:
+        event: The GenEvent to convert.
+
+    Returns:
+        A FeynmanDiagram object.
+    """
     fd = FeynmanDiagram()
     for v in event.vertices:
-        v = Vertex(id=_vertex_id_wrap(v.id))
+        v = Vertex(id=vertex_id_wrap(v.id))
         fd.add(v)
     for p in event.particles:
         # TODO first create all vertices?
         if p.status == 4:
             # incoming Leg
             fd.add(
                 Leg(
-                    id="Leg" + str(p.id).replace("-", "m"),
+                    id=leg_id_wrap(p.id),
                     pdgid=p.pid,
-                    target=_vertex_id_wrap(p.end_vertex.id),
+                    target=vertex_id_wrap(p.end_vertex.id),
                     sense="incoming",
                 )
             )
         elif p.status == 1:
             # outgoing Leg
             fd.add(
                 Leg(
-                    id="Leg" + str(p.id).replace("-", "m"),
+                    id=leg_id_wrap(p.id),
                     pdgid=p.pid,
-                    target=_vertex_id_wrap(p.production_vertex.id),
+                    target=vertex_id_wrap(p.production_vertex.id),
                     sense="outgoing",
                 )
             )
         else:
             # Propagator
             fd.add(
                 Propagator(
-                    id="Propagator" + str(p.id).replace("-", "m"),
+                    id=propagator_id_wrap(p.id),
                     pdgid=p.pid,
-                    source=_vertex_id_wrap(p.production_vertex.id),
-                    target=_vertex_id_wrap(p.end_vertex.id),
+                    source=vertex_id_wrap(p.production_vertex.id),
+                    target=vertex_id_wrap(p.end_vertex.id),
                 )
             )
     return fd
 
 
-def hepmc_to_feynml(hepmc_file):
-    # TODO: use pyhepmc
-    pass
+def hepmc_to_feynml(
+    hepmc_file: str,
+    creator="pyfeyn2",
+    tool="pyfeyn2.interface.hepmc",
+    title="",
+    description="",
+) -> FeynML:
+    """
+    Convert a HepMC file to a FeynML object.
+
+    Args:
+        hepmc_file: The path to the HepMC file.
+        creator: The creator of the file.
+        tool: The tool used to create the file.
+        title: The title of the file.
+        description: The description of the file.
+
+    Returns:
+        A FeynML object.
+    """
+    fds = []
+    with pyhepmc.open(hepmc_file) as f:
+        for event in f:
+            fds.append(hepmc_event_to_feynman(event))
+    return FeynML(
+        diagrams=fds,
+        head=Head(
+            metas=[
+                Meta(name="creator", content=creator),
+                Meta(name="tool", content=tool),
+                Meta(name="description", content=description),
+                Meta(name="title", content=title),
+            ]
+        ),
+    )
```

### Comparing `feynml-0.1.7/feynml/interface/qgraf.py` & `feynml-0.2.0/feynml/interface/qgraf.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/leg.py` & `feynml-0.2.0/feynml/leg.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/momentum.py` & `feynml-0.2.0/feynml/momentum.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/particles.py` & `feynml-0.2.0/feynml/particles.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/pdgid.py` & `feynml-0.2.0/feynml/pdgid.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/point.py` & `feynml-0.2.0/feynml/point.py`

 * *Files identical despite different names*

### Comparing `feynml-0.1.7/feynml/styled.py` & `feynml-0.2.0/feynml/styled.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,7 +88,10 @@
         if style is not None:
             self.style = cssutils.parseStyle(style)
         return self
 
     def with_class(self, clazz):
         self.clazz = clazz
         return self
+
+    def with_color(self, color):
+        return self.with_style_property("color", color)
```

### Comparing `feynml-0.1.7/pyproject.toml` & `feynml-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynml"
-version = "0.1.7"
+version = "0.2.0"
 description = "Feynman diagram markup language"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynml"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,40 +12,47 @@
 xsdata = {version = "*", extras = ["cli","lxml","soap"]}
 cssutils= "*"
 cssselect ="*"
 #pyqgraf = {path= "../pyqgraf", develop = true }
 #ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
-smpl_io = "*"
-smpl_doc = "*"
+smpl_io = "^1.1.2"
+#smpl_io = {path= "../smpl_io", develop = true}
+smpl_doc = "^1.1.3"
+#smpl_doc = {path= "../smpl_doc", develop = true}
 smpl_util= "*"
 
 pyqgraf = {version = ">=0.0.3", optional = true}
 pyhepmc = {version = "*", optional = true}
+pylhe = {version = "*", optional = true}
 
 [tool.poetry.extras]
-interface = ["pyqgraf", "pyhepmc"]
+interfaces = ["pyqgraf", "pyhepmc", "pylhe"]
 
-
-[tool.poetry.group.dev]
+[tool.poetry.group.test]
 optional = true
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.group.test.dependencies]
 pyhepmc = "*" # for testing
 pyqgraf = ">=0.0.3" # for testing
-pre-commit = "^2.20.0"
+pre-commit = ">=2.20,<4.0"
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 pytest-line-profiler-apn = ">=0.1.3"
+
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.1"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.23.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `feynml-0.1.7/setup.py` & `feynml-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 install_requires = \
 ['cssselect',
  'cssutils',
  'deprecated',
  'deprecation',
  'particle',
- 'smpl_doc',
- 'smpl_io',
+ 'smpl_doc>=1.1.3,<2.0.0',
+ 'smpl_io>=1.1.2,<2.0.0',
  'smpl_util',
  'xsdata[cli,lxml,soap]']
 
 extras_require = \
-{'interface': ['pyqgraf>=0.0.3', 'pyhepmc']}
+{'interfaces': ['pyqgraf>=0.0.3', 'pyhepmc', 'pylhe']}
 
 setup_kwargs = {
     'name': 'feynml',
-    'version': '0.1.7',
+    'version': '0.2.0',
     'description': 'Feynman diagram markup language',
     'long_description': '# FeynML\n\nFeynML from <https://feynml.hepforge.org/>\n\nFeynML is a project to develop an XML dialect for describing Feynman diagrams as used in quantum field theory calculations. The primary aim is to unambiguously describe the structure of a diagram in XML, giving a de facto representation for diagram structure which can be easily translated into another representation.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynml.svg)\n\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] [![Codacy Badge][cc c i]][cc c l]  [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Installation\n```sh\npip install [--user] feynml\n```\n\nor from cloned source:\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/feynml/>\n*   <https://apn-pucky.github.io/pyfeyn2/feynml/index.html>\n\n## Related:\n\n*   <https://github.com/APN-Pucky/pyfeyn2>\n\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n\n[pypi image]: https://badge.fury.io/py/feynml.svg\n[pypi link]: https://pypi.org/project/feynml/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynml.svg\n\n[a t link]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynml/actions/workflows/test.yml/badge.svg\n\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/feynml&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/feynml/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/feynml&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynml?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynml/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynml',
```

### Comparing `feynml-0.1.7/PKG-INFO` & `feynml-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: feynml
-Version: 0.1.7
+Version: 0.2.0
 Summary: Feynman diagram markup language
 Home-page: https://github.com/APN-Pucky/feynml
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: interface
+Provides-Extra: interfaces
 Requires-Dist: cssselect
 Requires-Dist: cssutils
 Requires-Dist: deprecated
 Requires-Dist: deprecation
 Requires-Dist: particle
-Requires-Dist: pyhepmc; extra == "interface"
-Requires-Dist: pyqgraf (>=0.0.3); extra == "interface"
-Requires-Dist: smpl_doc
-Requires-Dist: smpl_io
+Requires-Dist: pyhepmc; extra == "interfaces"
+Requires-Dist: pylhe; extra == "interfaces"
+Requires-Dist: pyqgraf (>=0.0.3); extra == "interfaces"
+Requires-Dist: smpl_doc (>=1.1.3,<2.0.0)
+Requires-Dist: smpl_io (>=1.1.2,<2.0.0)
 Requires-Dist: smpl_util
 Requires-Dist: xsdata[cli,lxml,soap]
 Project-URL: Repository, https://github.com/APN-Pucky/feynml
 Description-Content-Type: text/markdown
 
 # FeynML
```

