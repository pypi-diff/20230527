# Comparing `tmp/corpus_unpdf-0.0.8.tar.gz` & `tmp/corpus_unpdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_unpdf-0.0.8.tar", max compression
+gzip compressed data, was "corpus_unpdf-0.0.9.tar", max compression
```

## Comparing `corpus_unpdf-0.0.8.tar` & `corpus_unpdf-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      558 2023-01-29 10:58:37.331283 corpus_unpdf-0.0.8/README.md
--rw-r--r--   0        0        0       96 2023-02-07 03:34:32.487763 corpus_unpdf-0.0.8/corpus_unpdf/__init__.py
--rw-r--r--   0        0        0     6282 2023-02-07 03:58:52.996559 corpus_unpdf-0.0.8/corpus_unpdf/decision.py
--rw-r--r--   0        0        0      626 2023-02-05 05:24:00.060212 corpus_unpdf-0.0.8/corpus_unpdf/src/__init__.py
--rw-r--r--   0        0        0      227 2023-02-05 05:03:52.096928 corpus_unpdf-0.0.8/corpus_unpdf/src/common/__init__.py
--rw-r--r--   0        0        0     3289 2023-02-05 03:14:11.840252 corpus_unpdf-0.0.8/corpus_unpdf/src/common/fetch.py
--rw-r--r--   0        0        0     6893 2023-02-05 03:14:11.840404 corpus_unpdf-0.0.8/corpus_unpdf/src/common/slice.py
--rw-r--r--   0        0        0     2374 2023-02-05 03:14:11.840515 corpus_unpdf-0.0.8/corpus_unpdf/src/content_ender.py
--rw-r--r--   0        0        0     4954 2023-02-05 05:24:00.355426 corpus_unpdf-0.0.8/corpus_unpdf/src/content_markers.py
--rw-r--r--   0        0        0     2348 2023-02-05 03:14:11.840730 corpus_unpdf-0.0.8/corpus_unpdf/src/content_starter.py
--rw-r--r--   0        0        0     9096 2023-02-07 03:44:27.815804 corpus_unpdf-0.0.8/corpus_unpdf/src/decision_objects.py
--rw-r--r--   0        0        0     2641 2023-02-05 03:14:11.840800 corpus_unpdf-0.0.8/corpus_unpdf/src/page_footer.py
--rw-r--r--   0        0        0     4116 2023-02-07 03:40:55.897530 corpus_unpdf-0.0.8/corpus_unpdf/src/page_header.py
--rw-r--r--   0        0        0     1764 2023-02-07 03:34:24.257598 corpus_unpdf-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 corpus_unpdf-0.0.8/setup.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 corpus_unpdf-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-01-29 10:58:37.331283 corpus_unpdf-0.0.9/README.md
+-rw-r--r--   0        0        0      147 2023-02-08 10:35:44.239354 corpus_unpdf-0.0.9/corpus_unpdf/__init__.py
+-rw-r--r--   0        0        0     8248 2023-02-08 10:38:58.744061 corpus_unpdf-0.0.9/corpus_unpdf/decision.py
+-rw-r--r--   0        0        0      692 2023-02-08 10:35:44.240275 corpus_unpdf-0.0.9/corpus_unpdf/src/__init__.py
+-rw-r--r--   0        0        0      238 2023-02-08 10:35:44.246425 corpus_unpdf-0.0.9/corpus_unpdf/src/common/__init__.py
+-rw-r--r--   0        0        0     3289 2023-02-05 03:14:11.840252 corpus_unpdf-0.0.9/corpus_unpdf/src/common/fetch.py
+-rw-r--r--   0        0        0     6926 2023-02-08 09:39:22.727966 corpus_unpdf-0.0.9/corpus_unpdf/src/common/slice.py
+-rw-r--r--   0        0        0     2374 2023-02-05 03:14:11.840515 corpus_unpdf-0.0.9/corpus_unpdf/src/content_ender.py
+-rw-r--r--   0        0        0     7355 2023-02-08 10:35:44.248195 corpus_unpdf-0.0.9/corpus_unpdf/src/content_markers.py
+-rw-r--r--   0        0        0     2348 2023-02-05 03:14:11.840730 corpus_unpdf-0.0.9/corpus_unpdf/src/content_starter.py
+-rw-r--r--   0        0        0    10050 2023-02-08 10:37:26.329567 corpus_unpdf-0.0.9/corpus_unpdf/src/decision_objects.py
+-rw-r--r--   0        0        0     2641 2023-02-05 03:14:11.840800 corpus_unpdf-0.0.9/corpus_unpdf/src/page_footer.py
+-rw-r--r--   0        0        0     4116 2023-02-07 03:40:55.897530 corpus_unpdf-0.0.9/corpus_unpdf/src/page_header.py
+-rw-r--r--   0        0        0     1764 2023-02-08 10:11:01.339293 corpus_unpdf-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 corpus_unpdf-0.0.9/setup.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 corpus_unpdf-0.0.9/PKG-INFO
```

### Comparing `corpus_unpdf-0.0.8/README.md` & `corpus_unpdf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/decision.py` & `corpus_unpdf-0.0.9/corpus_unpdf/decision.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 from loguru import logger
 from pdfplumber.page import Page
 from pdfplumber.pdf import PDF
 
 from .src import (
     Decision,
     DecisionPage,
+    Opinion,
     PositionCourtComposition,
     PositionDecisionCategoryWriter,
     PositionNotice,
+    PositionOpinion,
     get_end_page_pos,
     get_start_page_pos,
 )
 
 
 class DecisionMeta(NamedTuple):
     """Metadata required to create a [decision][decision-document].
@@ -113,14 +115,24 @@
                 logger.debug(f"Initialize {nxt.page_number=}.")
                 if page_valid := DecisionPage.set(page=nxt):
                     yield page_valid
                 else:
                     logger.warning("Detected blank page.")
 
 
+def construct(obj: Decision | Opinion):
+    for page in obj.pages:
+        obj.body += f"\n\n\n\n{page.body_text}"
+        obj.segments.extend(page.segments)
+        if page.annex_text:
+            obj.annex += f"\n\n\n\n{page.annex_text}"
+            obj.footnotes.extend(page.footnotes)
+    return obj
+
+
 def get_decision(path: Path) -> Decision:
     """From a _*.pdf_ file found in `path`, extract relevant [metadata][decisionmeta]
     to generate a [decision][decision-document] having [pages][decision-pages].
     Each of which will contain a body and, likely, an annex for footnotes.
 
     Examples:
         >>> from pathlib import Path
@@ -152,17 +164,64 @@
     """  # noqa: E501
     meta = DecisionMeta.prep(path)
     with pdfplumber.open(path) as pdf:
         # create all the pages of the decision
         caso = meta.init(pdf=pdf)
         content_pages = meta.add(pages=pdf.pages)
         caso.pages.extend(content_pages)
-
         # construct full decision
-        page_break = "\n\n\n\n"
-        for page in caso.pages:
-            caso.body += f"{page_break}{page.body_text}"
-            caso.segments.extend(page.segments)
-            if page.annex_text:
-                caso.annex += f"{page_break}{page.annex_text}"
-                caso.footnotes.extend(page.footnotes)
-        return caso
+        obj = construct(caso)
+        if isinstance(obj, Decision):
+            return obj
+        raise Exception("Bad construction of Decision.")
+
+
+def get_opinion(path: Path) -> Opinion:
+    """From a _*.pdf_ file found in `path`, extract relevant opinion metadata
+    to generate an [opinion][opinion-document] having [pages][decision-pages].
+    Each of which will contain a body and, likely, an annex for footnotes.
+
+    Examples:
+        >>> from pathlib import Path
+        >>> x = Path().cwd() / "tests" / "data" / "opinion.pdf"
+        >>> opinion = get_opinion(x)
+        >>> opinion.writer
+        'HERNANDO, J.:'
+        >>> opinion.label
+        'DISSENTING OPINION'
+        >>> len(opinion.pages) # total page count
+        28
+        >>> isinstance(opinion.pages[0], DecisionPage) # first page
+        True
+        >>> from corpus_unpdf.src import Footnote, Bodyline
+        >>> isinstance(opinion.segments[0], Bodyline)
+        True
+        >>> isinstance(opinion.footnotes[0], Footnote)
+        True
+        >>> len(opinion.footnotes)
+        49
+
+    Args:
+        path (Path): Path to the pdf file.
+
+    Returns:
+        Self: Instance of an Opinion with pages populated
+    """  # noqa: E501
+    with pdfplumber.open(path) as pdf:
+        meta = PositionOpinion.from_pdf(pdf)
+        # initialize the opinion
+        start_page = pdf.pages[0]
+        start_y = meta.writer_pct_height * start_page.height
+        opinion = Opinion(
+            label=meta.label,
+            writer=meta.writer,
+            pages=[DecisionPage.set(page=start_page, start_y=start_y)],
+        )
+        # create all the pages of the opinion
+        for page in pdf.pages[1:]:
+            if page_valid := DecisionPage.set(page=page):
+                opinion.pages.append(page_valid)
+        # construct full opinion
+        obj = construct(opinion)
+        if isinstance(obj, Opinion):
+            return obj
+        raise Exception("Bad construction of Opinion.")
```

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/__init__.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from .common import (
     PageCut,
-    get_centered_coordinates,
     get_contours,
     get_img_from_page,
+    get_likelihood_centered_coordinates,
     get_page_and_img,
     get_reverse_pages_and_imgs,
 )
 from .content_ender import get_end_page_pos
 from .content_markers import (
     CourtCompositionChoices,
     DecisionCategoryChoices,
     PositionCourtComposition,
     PositionDecisionCategoryWriter,
     PositionNotice,
+    PositionOpinion,
 )
 from .content_starter import get_start_page_pos
-from .decision_objects import Bodyline, Decision, DecisionPage, Footnote
+from .decision_objects import (
+    Bodyline,
+    Decision,
+    DecisionPage,
+    Footnote,
+    Opinion,
+)
 from .page_footer import get_footer_line_coordinates, get_page_end
 from .page_header import get_header_line, get_page_num
```

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/common/fetch.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/common/fetch.py`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/common/slice.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/common/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
     dilate = cv2.dilate(thresh, kernel, iterations=1)
     cv2.imwrite("temp/sample_dilated.png", dilate)
     cnts = cv2.findContours(dilate, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     cnts = cnts[0] if len(cnts) == 2 else cnts[1]
     return sorted(cnts, key=lambda x: cv2.boundingRect(x)[1])
 
 
-def get_centered_coordinates(
+def get_likelihood_centered_coordinates(
     im: numpy.ndarray, text_to_match: str
 ) -> tuple[int, int, int, int] | None:
     """With a image `im`, get all contours found in the center
     of the image and then for each of these matches, if they
     are text resembling `text_to_match`, extract the coordinates of
     such contours.
 
     Examples:
         >>> from corpus_unpdf.src.common.fetch import get_page_and_img
         >>> from pathlib import Path
         >>> x = Path().cwd() / "tests" / "data" / "decision.pdf"
         >>> page, im = get_page_and_img(x, 0)
-        >>> get_centered_coordinates(im, 'Decision') # None found
-        >>> get_centered_coordinates(im, 'Resolution')
+        >>> get_likelihood_centered_coordinates(im, 'Decision') # None found
+        >>> get_likelihood_centered_coordinates(im, 'Resolution')
         (1068, 2108, 564, 92)
         >>> page.pdf.close()
 
     Args:
         im (numpy.ndarray): The base image to look for text
         text_to_match (str): The words that should match
```

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/content_ender.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/content_ender.py`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/content_starter.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/content_starter.py`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/decision_objects.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/decision_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,27 +223,57 @@
                 numpy.array(crop.to_image(resolution=300).original),
                 cv2.COLOR_RGB2BGR,
             )
         ).strip()
 
 
 @dataclass
+class Opinion:
+    """Metadata of a pdf file parsed via `get_opinion()`
+
+    Field | Description
+    --:|:--
+    `label` | How the opinion is labelled
+    `writer` | When available, the writer of the case
+    `pages` | A list of [Decision Pages][decision-pages]
+    `body` | The compiled string consisting of each page's `body_text`
+    `annex` | The compiled string consisting of each page's `annex_text`, if existing
+    `segments` | Each [bodyline][bodyline] of the body's text
+    `footnotes` | Each [footnote][footnote] in the annex's text
+    """
+
+    label: str
+    writer: str
+    pages: list[DecisionPage] = field(default_factory=list)
+    segments: list[Bodyline] = field(default_factory=list)
+    footnotes: list[Footnote] = field(default_factory=list)
+    body: str = ""
+    annex: str = ""
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.writer.title()} | {self.label.title()}: pages"
+            f" {len(self.pages)}"
+        )
+
+
+@dataclass
 class Decision:
     """Metadata of a pdf file parsed via `get_decision()`
 
     Field | Description
     --:|:--
     `composition` | The composition of the Supreme Court that decided the case
     `category` | When available, whether the case is a "Decision" or a "Resolution"
     `header` | The top portion of the page, usually excluded from metadata
     `writer` | When available, the writer of the case
     `notice` | When True, means that there is no `category` available
-    `pages` | A list of [Decision Pages with bodies/annexes][decision-pages]
-    `body` | The compiled string consisting of all the page's body_text
-    `annex` | The compiled string consisting of all the page's annex_text, if existing
+    `pages` | A list of [Decision Pages][decision-pages]
+    `body` | The compiled string consisting of each page's `body_text`
+    `annex` | The compiled string consisting of each page's `annex_text`, if existing
     `segments` | Each [bodyline][bodyline] of the body's text
     `footnotes` | Each [footnote][footnote] in the annex's text
     """
 
     composition: CourtCompositionChoices
     category: DecisionCategoryChoices | None = None
     header: CroppedPage | None = None
```

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/page_footer.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/page_footer.py`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.8/corpus_unpdf/src/page_header.py` & `corpus_unpdf-0.0.9/corpus_unpdf/src/page_header.py`

 * *Files identical despite different names*

### Comparing `corpus_unpdf-0.0.8/pyproject.toml` & `corpus_unpdf-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corpus-unpdf"
-version = "0.0.8"
+version = "0.0.9"
 description = "Parse Philippine Supreme Court decisions issued in PDF format as text."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/corpus-unpdf"
 documentation = "https://justmars.github.io/corpus-unpdf"
```

### Comparing `corpus_unpdf-0.0.8/setup.py` & `corpus_unpdf-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pdfplumber>=0.7.6,<0.8.0',
  'pillow>=9.4.0,<10.0.0',
  'pytesseract>=0.3.10,<0.4.0',
  'python-dotenv>=0.21,<0.22']
 
 setup_kwargs = {
     'name': 'corpus-unpdf',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Parse Philippine Supreme Court decisions issued in PDF format as text.',
     'long_description': '# corpus-unpdf\n\n![Github CI](https://github.com/justmars/corpus-unpdf/actions/workflows/main.yml/badge.svg)\n\nParse Philippine Supreme Court decisions issued in PDF format as text; _hopefully_, this can be utilized in the [LawSQL dataset](https://lawsql.com).\n\n## Documentation\n\nSee [documentation](https://justmars.github.io/corpus-unpdf).\n\n## Development\n\nCheckout code, create a new virtual environment:\n\n```sh\npoetry add corpus-unpdf # python -m pip install corpus-unpdf\npoetry update # install dependencies\npoetry shell\n```\n\nRun tests:\n\n```sh\npytest\n```\n',
     'author': 'Marcelino G. Veloso III',
     'author_email': 'mars@veloso.one',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://lawsql.com',
```

### Comparing `corpus_unpdf-0.0.8/PKG-INFO` & `corpus_unpdf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus-unpdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parse Philippine Supreme Court decisions issued in PDF format as text.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

