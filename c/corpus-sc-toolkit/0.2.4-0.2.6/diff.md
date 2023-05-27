# Comparing `tmp/corpus_sc_toolkit-0.2.4.tar.gz` & `tmp/corpus_sc_toolkit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_sc_toolkit-0.2.4.tar", max compression
+gzip compressed data, was "corpus_sc_toolkit-0.2.6.tar", max compression
```

## Comparing `corpus_sc_toolkit-0.2.4.tar` & `corpus_sc_toolkit-0.2.6.tar`

### file list

```diff
@@ -1,58 +1,57 @@
--rw-r--r--   0        0        0      343 2023-03-05 04:40:55.239419 corpus_sc_toolkit-0.2.4/README.md
--rw-r--r--   0        0        0      679 2023-03-09 07:55:25.398147 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/__init__.py
--rw-r--r--   0        0        0      327 2023-03-08 16:21:12.737171 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/analysis/missing_dockets_in_opinions.sql
--rw-r--r--   0        0        0      248 2023-03-08 16:21:12.737311 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/analysis/missing_phil_in_opinions.sql
--rw-r--r--   0        0        0      248 2023-03-08 16:21:12.737438 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/analysis/missing_scra_in_opinions.sql
--rw-r--r--   0        0        0      420 2023-03-08 16:21:12.737644 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/base/get_author_ids.sql
--rw-r--r--   0        0        0      131 2023-03-08 16:21:12.737766 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/base/get_detail.sql
--rw-r--r--   0        0        0      168 2023-03-08 16:21:12.738017 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/search_unmaterialized.sql
--rw-r--r--   0        0        0     1102 2023-03-08 16:21:12.738154 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/set_decision_id.sql
--rw-r--r--   0        0        0     1316 2023-03-08 16:21:12.738289 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/set_statute_id.sql
--rw-r--r--   0        0        0     1870 2023-03-08 16:21:12.738424 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/set_statute_unit_mp.sql
--rw-r--r--   0        0        0      820 2023-03-08 16:21:12.738573 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/get_base.sql
--rw-r--r--   0        0        0      820 2023-03-08 16:21:12.738686 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/list_event_statutes.sql
--rw-r--r--   0        0        0      215 2023-03-08 16:21:12.738793 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/list_unique_statute_category_idxes_from_events.sql
--rw-r--r--   0        0        0      665 2023-03-08 16:21:12.738908 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/update_statute_id.sql
--rw-r--r--   0        0        0     1381 2023-03-08 16:21:12.739105 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/chief_dates.sql
--rw-r--r--   0        0        0      139 2023-03-08 16:21:12.739213 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/get_base.sql
--rw-r--r--   0        0        0      562 2023-03-08 16:21:12.739407 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/inclusions/popular_citations.sql
--rw-r--r--   0        0        0      219 2023-03-08 16:21:12.739530 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/inclusions/popular_statutes.sql
--rw-r--r--   0        0        0      193 2023-03-08 16:21:12.739637 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/inclusions/read_opinions.sql
--rw-r--r--   0        0        0      989 2023-03-08 16:21:12.739777 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/inclusions/update_decision_id.sql
--rw-r--r--   0        0        0     1616 2023-03-08 16:21:12.739978 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/limit_extract.sql
--rw-r--r--   0        0        0     4751 2023-03-08 16:21:12.740118 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/list_opinions_of_decision.sql
--rw-r--r--   0        0        0     1324 2023-03-08 16:21:12.740306 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/get_base.sql
--rw-r--r--   0        0        0     1009 2023-03-08 16:21:12.740439 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/list_affected_statutes.sql
--rw-r--r--   0        0        0     1455 2023-03-08 16:21:12.740553 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/list_affector_statutes.sql
--rw-r--r--   0        0        0     1364 2023-03-08 16:21:12.740750 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/references/src_ref_mp_list.sql
--rw-r--r--   0        0        0      132 2023-03-08 16:21:12.740864 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/references/unique_statutes_list.sql
--rw-r--r--   0        0        0      578 2023-03-08 16:21:12.740986 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/update_id.sql
--rw-r--r--   0        0        0     7061 2023-03-09 03:19:00.421334 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/config.py
--rw-r--r--   0        0        0      729 2023-03-08 16:21:12.741643 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/__init__.py
--rw-r--r--   0        0        0     1430 2023-03-08 16:21:12.741845 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/_resources.py
--rw-r--r--   0        0        0     4006 2023-03-08 16:21:12.742184 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision.py
--rw-r--r--   0        0        0     6752 2023-03-09 03:45:04.581200 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_fields.py
--rw-r--r--   0        0        0     3376 2023-03-08 16:21:12.742810 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_fields_via_html.py
--rw-r--r--   0        0        0     8083 2023-03-09 07:52:16.209887 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_fields_via_pdf.py
--rw-r--r--   0        0        0     3240 2023-03-08 16:21:12.743348 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_opinion_segments.py
--rw-r--r--   0        0        0     7279 2023-03-09 07:54:20.713434 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_opinions.py
--rw-r--r--   0        0        0      206 2023-03-08 16:21:12.743702 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/__init__.py
--rw-r--r--   0        0        0     2039 2023-03-08 16:21:12.743821 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/category.py
--rw-r--r--   0        0        0      917 2023-03-08 16:21:12.743938 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/composition.py
--rw-r--r--   0        0        0      737 2023-03-08 16:21:12.744038 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/source.py
--rw-r--r--   0        0        0     4213 2023-03-08 16:21:12.744150 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/tags.py
--rw-r--r--   0        0        0     2698 2023-03-08 16:21:12.744278 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/voteline.py
--rw-r--r--   0        0        0      206 2023-03-08 16:21:12.744386 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/__init__.py
--rw-r--r--   0        0        0     1853 2023-03-08 16:21:12.744689 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_list.py
--rw-r--r--   0        0        0     7514 2023-03-08 16:21:12.745031 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_model.py
--rw-r--r--   0        0        0    11465 2023-03-08 16:21:12.745188 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_name.py
--rw-r--r--   0        0        0    10056 2023-03-08 16:21:12.745339 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_select.py
--rw-r--r--   0        0        0    45227 2023-03-08 16:21:12.745614 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/sc.yaml
--rw-r--r--   0        0        0      203 2023-03-09 07:55:15.522666 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/statutes/__init__.py
--rw-r--r--   0        0        0     3604 2023-03-09 03:21:12.660424 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/statutes/_resources.py
--rw-r--r--   0        0        0    11572 2023-03-09 02:19:39.973631 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/statutes/statute.py
--rw-r--r--   0        0        0     1806 2023-03-09 05:56:58.692578 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/store.py
--rw-r--r--   0        0        0     3144 2023-03-09 01:35:01.621153 corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/utils.py
--rw-r--r--   0        0        0     1740 2023-03-09 07:28:35.161732 corpus_sc_toolkit-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 corpus_sc_toolkit-0.2.4/setup.py
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 corpus_sc_toolkit-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-15 17:06:19.095686 corpus_sc_toolkit-0.2.6/LICENSE
+-rw-r--r--   0        0        0      403 2023-03-10 01:10:56.862563 corpus_sc_toolkit-0.2.6/README.md
+-rw-r--r--   0        0        0      858 2023-05-15 17:21:55.305790 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/__init__.py
+-rw-r--r--   0        0        0      327 2023-03-08 16:21:12.737171 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/analysis/missing_dockets_in_opinions.sql
+-rw-r--r--   0        0        0      248 2023-03-08 16:21:12.737311 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/analysis/missing_phil_in_opinions.sql
+-rw-r--r--   0        0        0      248 2023-03-08 16:21:12.737438 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/analysis/missing_scra_in_opinions.sql
+-rw-r--r--   0        0        0      420 2023-03-08 16:21:12.737644 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/base/get_author_ids.sql
+-rw-r--r--   0        0        0      131 2023-03-08 16:21:12.737766 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/base/get_detail.sql
+-rw-r--r--   0        0        0      168 2023-03-08 16:21:12.738017 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/search_unmaterialized.sql
+-rw-r--r--   0        0        0     1102 2023-03-08 16:21:12.738154 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/set_decision_id.sql
+-rw-r--r--   0        0        0     1316 2023-03-08 16:21:12.738289 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/set_statute_id.sql
+-rw-r--r--   0        0        0     1870 2023-03-08 16:21:12.738424 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/set_statute_unit_mp.sql
+-rw-r--r--   0        0        0      820 2023-03-08 16:21:12.738573 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/get_base.sql
+-rw-r--r--   0        0        0      820 2023-03-08 16:21:12.738686 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/list_event_statutes.sql
+-rw-r--r--   0        0        0      215 2023-03-08 16:21:12.738793 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/list_unique_statute_category_idxes_from_events.sql
+-rw-r--r--   0        0        0      665 2023-03-08 16:21:12.738908 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/update_statute_id.sql
+-rw-r--r--   0        0        0     1381 2023-03-08 16:21:12.739105 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/chief_dates.sql
+-rw-r--r--   0        0        0      139 2023-03-08 16:21:12.739213 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/get_base.sql
+-rw-r--r--   0        0        0      562 2023-03-08 16:21:12.739407 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/inclusions/popular_citations.sql
+-rw-r--r--   0        0        0      219 2023-03-08 16:21:12.739530 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/inclusions/popular_statutes.sql
+-rw-r--r--   0        0        0      193 2023-03-08 16:21:12.739637 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/inclusions/read_opinions.sql
+-rw-r--r--   0        0        0      989 2023-03-08 16:21:12.739777 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/inclusions/update_decision_id.sql
+-rw-r--r--   0        0        0     1616 2023-03-08 16:21:12.739978 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/limit_extract.sql
+-rw-r--r--   0        0        0     4751 2023-03-08 16:21:12.740118 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/list_opinions_of_decision.sql
+-rw-r--r--   0        0        0     1324 2023-03-08 16:21:12.740306 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/get_base.sql
+-rw-r--r--   0        0        0     1009 2023-03-08 16:21:12.740439 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/list_affected_statutes.sql
+-rw-r--r--   0        0        0     1455 2023-03-08 16:21:12.740553 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/list_affector_statutes.sql
+-rw-r--r--   0        0        0     1364 2023-03-08 16:21:12.740750 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/references/src_ref_mp_list.sql
+-rw-r--r--   0        0        0      132 2023-03-08 16:21:12.740864 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/references/unique_statutes_list.sql
+-rw-r--r--   0        0        0      578 2023-03-08 16:21:12.740986 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/update_id.sql
+-rw-r--r--   0        0        0      855 2023-05-15 17:18:31.486608 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/__init__.py
+-rw-r--r--   0        0        0     4776 2023-05-15 17:33:27.292610 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/_resources.py
+-rw-r--r--   0        0        0    11211 2023-03-10 02:45:12.912729 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision.py
+-rw-r--r--   0        0        0     5995 2023-03-09 11:58:18.624740 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_fields.py
+-rw-r--r--   0        0        0     4287 2023-03-09 09:57:31.208093 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_fields_via_html.py
+-rw-r--r--   0        0        0     9000 2023-05-15 17:33:27.374719 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_fields_via_pdf.py
+-rw-r--r--   0        0        0     3226 2023-05-15 17:33:27.292851 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_opinion_segments.py
+-rw-r--r--   0        0        0     7364 2023-03-09 11:58:50.124071 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_opinions.py
+-rw-r--r--   0        0        0      206 2023-03-08 16:21:12.743702 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/__init__.py
+-rw-r--r--   0        0        0     2039 2023-03-08 16:21:12.743821 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/category.py
+-rw-r--r--   0        0        0      917 2023-03-08 16:21:12.743938 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/composition.py
+-rw-r--r--   0        0        0      737 2023-03-08 16:21:12.744038 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/source.py
+-rw-r--r--   0        0        0     4213 2023-03-08 16:21:12.744150 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/tags.py
+-rw-r--r--   0        0        0     2698 2023-03-08 16:21:12.744278 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/voteline.py
+-rw-r--r--   0        0        0      206 2023-03-08 16:21:12.744386 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-15 17:11:32.879359 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_list.py
+-rw-r--r--   0        0        0     7482 2023-05-15 17:33:27.384193 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_model.py
+-rw-r--r--   0        0        0    11465 2023-03-08 16:21:12.745188 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_name.py
+-rw-r--r--   0        0        0    10032 2023-05-15 17:08:29.417648 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_select.py
+-rw-r--r--   0        0        0    45227 2023-03-08 16:21:12.745614 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/sc.yaml
+-rw-r--r--   0        0        0     1206 2023-03-09 15:30:56.985399 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/main.py
+-rw-r--r--   0        0        0      188 2023-03-10 02:46:17.963132 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/statutes/__init__.py
+-rw-r--r--   0        0        0    14218 2023-05-15 17:33:27.517311 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/statutes/statute.py
+-rw-r--r--   0        0        0     4408 2023-05-15 17:33:27.347482 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/store.py
+-rw-r--r--   0        0        0     4787 2023-05-15 17:33:27.355911 corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/utils.py
+-rw-r--r--   0        0        0     1525 2023-05-27 10:12:08.327004 corpus_sc_toolkit-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 corpus_sc_toolkit-0.2.6/PKG-INFO
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/__init__.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-__version__ = "0.2.4"
+__version__ = "0.2.6"
 
 
-from .config import ConfigDecisions, ConfigStatutes
 from .decisions import (
     CandidateJustice,
     CitationRow,
+    ConfigDecisions,
     CourtComposition,
     DecisionCategory,
     DecisionHTML,
     DecisionOpinion,
     DecisionPDF,
     DecisionRow,
     DecisionSource,
@@ -16,21 +16,30 @@
     Justice,
     JusticeDetail,
     OpinionRow,
     OpinionWriterName,
     SegmentRow,
     TitleTagRow,
     VoteLine,
+    decision_storage,
     extract_votelines,
     get_justices_file,
     get_justices_from_api,
     tags_from_title,
     voteline_clean,
 )
+from .main import config_db
 from .statutes import (
+    ConfigStatutes,
     Statute,
     StatuteFoundInUnit,
     StatuteMaterialPath,
     StatuteRow,
     StatuteTitleRow,
     StatuteUnitSearch,
+    statute_storage,
+)
+from .store import (
+    store_local_decisions_in_r2,
+    store_local_statutes_in_r2,
+    store_pdf_decisions_in_r2,
 )
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/set_decision_id.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/set_decision_id.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/set_statute_id.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/set_statute_id.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/events/set_statute_unit_mp.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/events/set_statute_unit_mp.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/get_base.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/get_base.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/list_event_statutes.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/list_event_statutes.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/codes/update_statute_id.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/codes/update_statute_id.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/chief_dates.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/chief_dates.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/inclusions/popular_citations.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/inclusions/popular_citations.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/inclusions/update_decision_id.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/inclusions/update_decision_id.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/limit_extract.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/limit_extract.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/decisions/list_opinions_of_decision.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/decisions/list_opinions_of_decision.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/get_base.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/get_base.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/list_affected_statutes.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/list_affected_statutes.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/list_affector_statutes.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/list_affector_statutes.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/references/src_ref_mp_list.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/references/src_ref_mp_list.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/_sql/statutes/update_id.sql` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/_sql/statutes/update_id.sql`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_fields.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_fields.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from typing import Self
 
 from citation_utils import Citation
 from loguru import logger
 from pydantic import BaseModel, Field, root_validator
 
-from ._resources import DECISION_BUCKET_NAME, DECISION_CLIENT, decision_storage
+from ._resources import decision_storage
 from .decision_opinions import DecisionOpinion
 from .fields import CourtComposition, DecisionCategory
 
 
 class DecisionFields(BaseModel):
     """
     Field | Type | Description
@@ -100,34 +100,14 @@
             "docket_date": self.date.isoformat(),
             "report_phil": self.citation.phil,
             "report_scra": self.citation.scra,
             "report_off_gaz": self.citation.offg,
             "has_pdf": self.is_pdf,
         }
 
-    @classmethod
-    def key_raw(cls, dated_prefix: str) -> str | None:
-        """Is suffix `details.yaml` present in result of `cls.iter_dockets()`?"""
-        key = f"{dated_prefix}/details.yaml"
-        try:
-            DECISION_CLIENT.get_object(Bucket=DECISION_BUCKET_NAME, Key=key)
-            return key
-        except Exception:
-            return None
-
-    @classmethod
-    def key_pdf(cls, dated_prefix: str) -> str | None:
-        """Is suffix `pdf.yaml` present in result of `cls.iter_dockets()`?"""
-        key = f"{dated_prefix}/pdf.yaml"
-        try:
-            DECISION_CLIENT.get_object(Bucket=DECISION_BUCKET_NAME, Key=key)
-            return key
-        except Exception:
-            return None
-
     def put_in_storage(self, suffix: str):
         """Puts Pydantic exported data dict to `details.yaml` or `pdf.yaml` in
         R2, depending on the value of `suffix`."""
 
         # Set guard on suffix only
         if suffix not in ("details.yaml", "pdf.yaml"):
             raise Exception("Invalid upload path.")
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_fields_via_html.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_fields_via_html.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,56 @@
+from collections.abc import Iterator
 from pathlib import Path
 
 import yaml
 from citation_utils import Citation
 from loguru import logger
 from markdownify import markdownify
 from pydantic import Field
 from sqlite_utils import Database
 
-from ._resources import decision_storage
+from ._resources import DECISION_BUCKET_NAME, DECISION_CLIENT, decision_storage
 from .decision_fields import DecisionFields
 from .decision_opinions import DecisionOpinion
 from .fields import (
     CourtComposition,
     DecisionCategory,
     voteline_clean,
 )
 from .justice import CandidateJustice
 
+DETAILS_KEY = "details.yaml"
+"""This suffix is uploaded / retrieved from R2 storage based on `DecisionHTML`."""
+
 
 class DecisionHTML(DecisionFields):
     home_html: Path | None = Field(default=None, exclude=True)
 
+    @classmethod
+    def get_key(cls, dated_prefix: str) -> str | None:
+        """Is suffix `details.yaml` present in result of `cls.iter_dockets()`?"""
+        key = f"{dated_prefix}/{DETAILS_KEY}"
+        try:
+            DECISION_CLIENT.get_object(Bucket=DECISION_BUCKET_NAME, Key=key)
+            return key
+        except Exception:
+            return None
+
+    @classmethod
+    def get_existing_prefixes(cls) -> Iterator[str]:
+        if object_list := decision_storage.all_items():
+            if filtered_list := decision_storage.filter_content(
+                filter_suffix="/{DETAILS_KEY}", objects_list=object_list
+            ):
+                for item in filtered_list:
+                    yield item["Key"]
+
     def to_storage(self):
         # Uses `details.yaml` to upload decision fields represented by instance.
-        self.put_in_storage("details.yaml")
+        self.put_in_storage(DETAILS_KEY)
 
         # Upload legacy html files
         if self.home_html and self.home_html.exists():
             loc = f"{self.prefix}/body.html"
             decision_storage.upload(file_like=self.home_html, loc=loc)
 
         # Upload markdown-based opinion files
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_fields_via_pdf.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_fields_via_pdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 from pebble import concurrent
 from pydantic import BaseModel, Field
 from sqlite_utils import Database
 from statute_trees import MentionedStatute
 
 from corpus_sc_toolkit.utils import sqlenv
 
+from ._resources import DECISION_BUCKET_NAME, DECISION_CLIENT, decision_storage
 from .decision_fields import DecisionFields
 from .decision_opinion_segments import OpinionSegment
 from .decision_opinions import DecisionOpinion, OpinionTag
 from .fields import CourtComposition, DecisionCategory
 from .justice import CandidateJustice
 
+PDF_KEY = "pdf.yaml"
+"""This suffix is uploaded / retrieved from R2 storage based on `DecisionPDF`."""
+
 
 @concurrent.process(timeout=5)
 def list_statutes(body_text: str, annex_text: str | None = None):
     items = []
     items.extend(list(MentionedStatute.set_counted_statute(text=body_text)))
     if annex_text:
-        items.extend(
-            list(MentionedStatute.set_counted_statute(text=annex_text))
-        )
+        items.extend(list(MentionedStatute.set_counted_statute(text=annex_text)))
     return items
 
 
 @concurrent.process(timeout=5)
 def list_citations(body_text: str, annex_text: str | None = None):
     items = []
     items.extend(list(Citation.extract_citations(text=body_text)))
@@ -162,34 +164,53 @@
             opinions.append(opinion)
         return {"opinions": opinions} | match_ponencia
 
 
 class DecisionPDF(DecisionFields):
     ...
 
+    @classmethod
+    def get_key(cls, dated_prefix: str) -> str | None:
+        """Is suffix `pdf.yaml` present in result of `cls.iter_dockets()`?"""
+        key = f"{dated_prefix}/{PDF_KEY}"
+        try:
+            DECISION_CLIENT.get_object(Bucket=DECISION_BUCKET_NAME, Key=key)
+            return key
+        except Exception:
+            return None
+
+    @classmethod
+    def get_existing_prefixes(cls) -> Iterator[str]:
+        if object_list := decision_storage.all_items():
+            if filtered_list := decision_storage.filter_content(
+                filter_suffix="/{PDF_KEY}", objects_list=object_list
+            ):
+                for item in filtered_list:
+                    yield item["Key"]
+
     def to_storage(self):
         # Uses `pdf.yaml` to upload decision fields represented by instance.
         logger.debug(f"Uploading: {self.id=}")
-        self.put_in_storage("pdf.yaml")
+        self.put_in_storage(PDF_KEY)
 
         # Upload txt-based opinion files
         for opinion in self.opinions:
             opinion.to_storage(self.prefix, "txt")
 
     @classmethod
     def originate(cls, db: Database) -> Iterator[Self]:
         """Extract sql query (`/sql/limit_extract.sql`) from `db` to instantiate
         a list of rows to process.
 
         Args:
-            db (Database): Contains previously created pdf-based / justice tables.
+            db (Database): result of a [corpus-extractor](https://github.com/justmars/corpus-extractor/) process.
 
         Yields:
             Iterator[Self]: Instances of the Interim Decision.
-        """
+        """  # noqa: E501
         q = sqlenv.get_template("decisions/limit_extract.sql").render()
         for row in db.execute_returning_dicts(q):
             result = extract_citation_ids(row)
             if not result:
                 logger.error(
                     f"No citation from {row.get('docket_category')=} {row.get('serial')=} {row.get('date')=}"  # noqa: E501
                 )
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_opinion_segments.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_opinion_segments.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,15 @@
         title="Body Segment",
         description="Partial fragment of opinion.",
         col=str,
         fts=True,
     )
 
     @classmethod
-    def segmentize(
-        cls, full_text: str, min_num_chars: int = 10
-    ) -> Iterator[dict]:
+    def segmentize(cls, full_text: str, min_num_chars: int = 10) -> Iterator[dict]:
         """Split first by double-spaced breaks `\\n\\n` and then by
         single spaced breaks `\\n` to get the position of the segment.
 
         Will exclude footnotes and segments with less than 10 characters.
 
         Args:
             full_text (str): The opinion to segment
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/decision_opinions.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/decision_opinions.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     concurs: list[dict] | None = Field(default=None)
     text: str = Field(
         ...,
         description="Text proper of opinion (ideally in markdown)",
         col=str,
         fts=True,
     )
+    # TODO: The lists below need to be extracted to separate db table, see relations
     statutes: list[MentionedStatute]
     segments: list[OpinionSegment]
     citations: list[Citation]
 
     class Config:
         use_enum_values = True
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/category.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/category.py`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/composition.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/composition.py`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/source.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/source.py`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/tags.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/tags.py`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/fields/voteline.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/fields/voteline.py`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_list.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     calling [get_justices_from_api()][source-list-from-api].
 
     Args:
         local_file (Path, optional): Path to justice list. See default folder /"sc.yaml"
 
     Examples:
         >>> from pathlib import Path
-        >>> p = Path().cwd() / "justice" / "sc.yaml" # the test file
+        >>> p = Path(__file__).parent / "sc.yaml" # the test file
         >>> f = get_justices_file(p)
         >>> f.exists()
         True
 
     Returns:
         Path: Yaml file containing list of justices
     """
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_model.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         >>> c = Connection(DatabasePath="test.db")
         >>> c.path_to_db.unlink(missing_ok=True) # tear down
         >>> table = c.create_table(Justice)
         >>> isinstance(table, Table)
         True
         >>> # See local file
         >>> from pathlib import Path
-        >>> from corpus_sc_toolkit.justice import get_justices_file
+        >>> from corpus_sc_toolkit import get_justices_file
         >>> p = Path().cwd() / "tests" / "sc.yaml" # the test file
         >>> f = get_justices_file(p)
         >>> f.exists()
         True
         >>> # Can add all pydantic validated records from the local copy of justices to the database.
         >>> import yaml
         >>> res = c.add_records(Justice, yaml.safe_load(f.read_bytes()))
@@ -93,17 +93,15 @@
         ge=1,
         lt=1000,
         col=int,
     )
     alias: str | None = Field(
         None,
         title="Alias",
-        description=(
-            "Means of matching ponente and voting strings to the justice id."
-        ),
+        description="Means of matching ponente and voting strings to the justice id.",
         col=str,
         index=True,
     )
     start_term: datetime.date | None = Field(
         None,
         title="Start Term",
         description="Date of appointment.",
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_name.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_name.py`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/justice_select.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/justice_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def rows(self) -> list[dict]:
         """When selecting a ponente or voting members, create a candidate list of
         justices based on the `valid_date`.
 
         Examples:
             >>> import yaml
             >>> from pathlib import Path
-            >>> from corpus_sc_toolkit.justice import Justice, get_justices_file
+            >>> from corpus_sc_toolkit import Justice, get_justices_file
             >>> from sqlpyd import Connection
             >>> p = Path().cwd() / "tests" / "sc.yaml" # the test file
             >>> c = Connection(DatabasePath="test.db")
             >>> c.path_to_db.unlink(missing_ok=True) # tear down
             >>> tbl = c.create_table(Justice)
             >>> res = c.add_records(Justice, yaml.safe_load(get_justices_file(p).read_bytes()))
             >>> search = CandidateJustice(db=c.db, date_str='Dec. 1, 1995')
@@ -88,15 +88,15 @@
         """Based on `get_active_on_date()`, match the cleaned_name to either the alias
         of the justice or the justice's last name; on match, determine whether the
         designation should be 'C.J.' or 'J.'
 
         Examples:
             >>> import yaml
             >>> from pathlib import Path
-            >>> from corpus_sc_toolkit.justice import Justice, get_justices_file
+            >>> from corpus_sc_toolkit import Justice, get_justices_file
             >>> from sqlpyd import Connection
             >>> p = Path().cwd() / "tests" / "sc.yaml" # the test file
             >>> c = Connection(DatabasePath="test.db")
             >>> c.path_to_db.unlink(missing_ok=True) # tear down
             >>> tbl = c.create_table(Justice)
             >>> res = c.add_records(Justice, yaml.safe_load(get_justices_file(p).read_bytes()))
             >>> search = CandidateJustice(db=c.db, text='Panganiban, Acting Cj', date_str='Dec. 1, 1995')
@@ -143,15 +143,15 @@
     @property
     def detail(self) -> JusticeDetail | None:
         """Get object to match fields directly
 
         Examples:
             >>> import yaml
             >>> from pathlib import Path
-            >>> from corpus_sc_toolkit.justice import Justice, get_justices_file
+            >>> from corpus_sc_toolkit import Justice, get_justices_file
             >>> from sqlpyd import Connection
             >>> p = Path().cwd() / "tests" / "sc.yaml" # the test file
             >>> c = Connection(DatabasePath="test.db")
             >>> c.path_to_db.unlink(missing_ok=True) # tear down
             >>> tbl = c.create_table(Justice)
             >>> res = c.add_records(Justice, yaml.safe_load(get_justices_file(p).read_bytes()))
             >>> search = CandidateJustice(db=c.db, text='Panganiban, Acting Cj', date_str='Dec. 1, 1995')
```

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/decisions/justice/sc.yaml` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/decisions/justice/sc.yaml`

 * *Files identical despite different names*

### Comparing `corpus_sc_toolkit-0.2.4/corpus_sc_toolkit/statutes/statute.py` & `corpus_sc_toolkit-0.2.6/corpus_sc_toolkit/statutes/statute.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import sqlite3
 from collections.abc import Iterator
 from pathlib import Path
 from typing import Self
 
+from corpus_pax import Individual
 from loguru import logger
-from pydantic import EmailStr, Field, ValidationError
+from pydantic import BaseModel, EmailStr, Field, ValidationError
 from sqlpyd import Connection, TableConfig
-from statute_patterns import (
-    StatuteTitleCategory,
-    extract_rules,
-)
+from statute_patterns import StatuteTitleCategory, extract_rules
 from statute_trees import (
     Node,
     Page,
     StatuteBase,
     StatutePage,
     StatuteUnit,
     generic_content,
     generic_mp,
 )
 
+from corpus_sc_toolkit.store import StorageToDatabaseConfiguration
 from corpus_sc_toolkit.utils import sqlenv
 
-from ._resources import Integrator, statute_storage
+from ..decisions import StorageUtils
 
+DETAILS_FILE = "details.yaml"
+STATUTE_TEMP_FOLDER = Path(__file__).parent / "_tmp"
+STATUTE_TEMP_FOLDER.mkdir(exist_ok=True)
+statute_storage = StorageUtils(name="ph-statutes", temp_folder=STATUTE_TEMP_FOLDER)
 
-class StatuteRow(Page, StatuteBase, TableConfig):
-    """This corresponds to statute_trees.StatutePage but is adjusted
-    for the purpose of table creation."""
 
+class StatuteRow(Page, StatuteBase, TableConfig):
     __prefix__ = "lex"
     __tablename__ = "statutes"
     __indexes__ = [
         ["statute_category", "statute_serial_id", "date", "variant"],
         ["statute_category", "statute_serial_id", "date"],
         ["statute_category", "statute_serial_id", "variant"],
         ["statute_category", "statute_serial_id"],
@@ -52,17 +53,14 @@
         q = "id = ?"
         rows = list(tbl.rows_where(where=q, where_args=(pk,), select="id"))
         idx = rows[0]["id"] if rows else None
         return idx
 
 
 class StatuteTitleRow(TableConfig):
-    """This corresponds to statute_patterns.StatuteTitle but
-    is adjusted for the purpose of table creation."""
-
     __prefix__ = "lex"
     __tablename__ = "statute_titles"
     __indexes__ = [["category", "text"], ["category", "statute_id"]]
     statute_id: str = Field(..., col=str, fk=(StatuteRow.__tablename__, "id"))
     category: StatuteTitleCategory = Field(
         ...,
         col=str,
@@ -122,103 +120,88 @@
         col=str,
         fk=(StatuteRow.__tablename__, "id"),
     )
 
     @classmethod
     def list_affected_statutes(cls, c: Connection, pk: str) -> dict:
         sql_file = "statutes/list_affected_statutes.sql"
-        results = c.db.execute_returning_dicts(
-            sqlenv.get_template(sql_file).render(
-                ref_tbl=cls.__tablename__,
-                statute_tbl=StatuteRow.__tablename__,
-                affecting_statute_id=pk,
-            )
+        template = sqlenv.get_template(sql_file)
+        query = template.render(
+            ref_tbl=cls.__tablename__,
+            statute_tbl=StatuteRow.__tablename__,
+            affecting_statute_id=pk,
         )
-        if results:
-            return results[0]
+        if rows := c.db.execute_returning_dicts(query):
+            return rows[0]
         return {}
 
     @classmethod
     def list_affector_statutes(cls, c: Connection, pk: str) -> dict:
-        sql_file = "statutes/list_affector_statutes.sql"
-        results = c.db.execute_returning_dicts(
-            sqlenv.get_template(sql_file).render(
-                ref_tbl=cls.__tablename__,
-                statute_tbl=StatuteRow.__tablename__,
-                affected_statute_id=pk,
-            )
+        sql = "statutes/list_affector_statutes.sql"
+        template = sqlenv.get_template(sql)
+        query = template.render(
+            ref_tbl=cls.__tablename__,
+            statute_tbl=StatuteRow.__tablename__,
+            affected_statute_id=pk,
         )
-        if results:
-            return results[0]
+        if rows := c.db.execute_returning_dicts(query):
+            return rows[0]
         return {}
 
     @classmethod
     def find_statute_in_unit(
-        cls,
-        text: str,
-        mp: str,
-        statute_id: str,
-    ) -> Iterator["StatuteFoundInUnit"]:
-        """Given text of a particular `material_path`, determine if there are
-        statutes found by `get_statute_labels`; if they're found, determine
-        the proper `StatuteFoundInUnit` to yield.
-        """
+        cls, text: str, mp: str, statute_id: str
+    ) -> Iterator[Self]:
+        """Yield statutes in `text` of material_path `mp`."""
         for rule in extract_rules(text):
             yield cls(
                 material_path=mp,
                 statute_id=statute_id,
                 statute_category=rule.cat,
                 statute_serial_id=rule.id,
                 matching_statute_id=None,
             )
 
     @classmethod
-    def extract_units(
-        cls,
-        pk: str,
-        units: list["StatuteUnit"],
-    ) -> Iterator["StatuteFoundInUnit"]:
-        """Traverse the tree and search the caption and content of each unit
-        for possible Statutes.
-        """
+    def extract_units(cls, pk: str, units: list[StatuteUnit]) -> Iterator[Self]:
+        """Traverse tree and search unit caption /content for possible Statutes."""
         for u in units:
             if u.caption and u.content:
                 text = f"{u.caption}. {u.content}"
                 yield from cls.find_statute_in_unit(text, u.id, pk)
             elif u.content:
                 yield from cls.find_statute_in_unit(u.content, u.id, pk)
             if u.units:
                 yield from cls.extract_units(pk, u.units)
 
     @classmethod
     def get_statutes_from_references(cls, c: Connection) -> Iterator[dict]:
-        """Extract relevant statute category and identifier pairs
-        from the cls.__tablename__."""
-        for row in c.db.execute_returning_dicts(
-            sqlenv.get_template(
-                "statutes/references/unique_statutes_list.sql"
-            ).render(statute_references_tbl=cls.__tablename__)
-        ):
+        """Extract statute category and identifier pairs from the cls.__tablename__."""
+        sql = "statutes/references/unique_statutes_list.sql"
+        template = sqlenv.get_template(sql)
+        query = template.render(statute_references_tbl=cls.__tablename__)
+        rows = c.db.execute_returning_dicts(query)
+        for row in rows:
             yield StatuteBase(**row).dict()
 
     @classmethod
     def update_statute_ids(cls, c: Connection) -> sqlite3.Cursor:
-        """Since all statutes present in `db`, supply `matching_statute_id` in
-        the references table."""
+        """Since statutes present in `db`, supply `matching_statute_id` in
+        references table."""
         with c.session as cur:
             return cur.execute(
                 sqlenv.get_template("statutes/update_id.sql").render(
                     statute_tbl=StatuteRow.__tablename__,
                     target_tbl=cls.__tablename__,
                     target_col=cls.__fields__["matching_statute_id"].name,
                 )
             )
 
 
-class Statute(Integrator):
+class Statute(BaseModel):
     id: str
     prefix: str
     emails: list[EmailStr]
     meta: StatuteRow
     titles: list[StatuteTitleRow]
     tree: list[StatuteUnit]
     unit_fts: list[StatuteUnitSearch]
@@ -269,16 +252,15 @@
         # assign row for creation
         page.id = page.prefix_db_key  # mutate the page prior to export as dict
         meta = StatuteRow(**page.dict(exclude={"emails", "tree", "titles"}))
         statute_id = page.prefix_db_key  # use same id for related entities
 
         # setup associated titles
         titles = [
-            StatuteTitleRow(**statute_title.dict())
-            for statute_title in page.titles
+            StatuteTitleRow(**statute_title.dict()) for statute_title in page.titles
         ]
 
         # enable full text searches of contents of the tree; starts with `1.1.`
         fts = [
             StatuteUnitSearch(**unit)
             for unit in StatuteUnit.searchables(statute_id, page.tree)
         ]
@@ -301,31 +283,27 @@
             emails=page.emails,
             meta=meta,
             tree=page.tree,
             titles=titles,
             unit_fts=root_fts + fts,
             material_paths=[
                 StatuteMaterialPath(**unit)
-                for unit in StatuteUnit.granularize(
-                    pk=statute_id, nodes=page.tree
-                )
+                for unit in StatuteUnit.granularize(pk=statute_id, nodes=page.tree)
             ],
             statutes_found=list(
-                StatuteFoundInUnit.extract_units(
-                    pk=statute_id, units=page.tree
-                )
+                StatuteFoundInUnit.extract_units(pk=statute_id, units=page.tree)
             ),
         )
 
     def to_storage(self):
-        loc = f"{self.prefix}/details.yaml"
+        loc = f"{self.prefix}/{DETAILS_FILE}"
         data = self.dict(exclude_none=True)
         temp_file = statute_storage.make_temp_yaml_path_from_data(data)
         args = statute_storage.set_extra_meta(self.storage_meta)
-        statute_storage.upload(file_like=temp_file, loc=loc, args=args)
+        statute_storage.upload(file_like=temp_file, key=loc, args=args)
         temp_file.unlink()
 
     @classmethod
     def get(cls, prefix: str) -> Self:
         """Retrieve data represented by the `prefix` from R2 (implies previous
         `upload()`) and instantiate the Statute based on such retrieved data.
 
@@ -334,7 +312,88 @@
 
         Returns:
             Self: Integrated Statute instance from R2 prefix.
         """
         if not (data := statute_storage.restore_temp_yaml(yaml_suffix=prefix)):
             raise Exception(f"Could not originate {prefix=}")
         return cls(**data)
+
+
+class ConfigStatutes(StorageToDatabaseConfiguration):
+    def set_tables(self):
+        self.conn.create_table(StatuteRow)
+        self.conn.create_table(StatuteTitleRow)
+        self.conn.create_table(StatuteUnitSearch)
+        self.conn.create_table(StatuteMaterialPath)
+        self.conn.create_table(StatuteFoundInUnit)
+        self.conn.db.index_foreign_keys()
+        logger.info("Statute-based tables ready.")
+        return self.conn.db
+
+    def add_row(self, statute: Statute):
+        # id should be modified prior to adding to db
+        record = statute.meta.dict(exclude={"emails"})
+        record["id"] = statute.id  # see TODO in Statute
+        self.conn.add_record(StatuteRow, record)
+        for email in statute.emails:
+            self.conn.table(StatuteRow).update(statute.id).m2m(
+                other_table=self.conn.table(Individual),
+                lookup={"email": email},
+                pk="id",
+            )
+
+        for statute_title in statute.titles:
+            statute_title.statute_id = statute.id  # see TODO in Statute
+            self.conn.add_record(
+                kls=StatuteTitleRow,
+                item=statute_title.dict(),
+            )
+
+        self.conn.add_cleaned_records(
+            kls=StatuteMaterialPath,
+            items=statute.material_paths,
+        )
+
+        self.conn.add_cleaned_records(
+            kls=StatuteUnitSearch,
+            items=statute.unit_fts,
+        )
+
+        self.conn.add_cleaned_records(
+            kls=StatuteFoundInUnit,
+            items=statute.statutes_found,
+        )
+        return statute.id
+
+    def add_rows(self):
+        self.set_tables()
+        if statute_prefixes := self.storage.all_items():
+            for prefix in statute_prefixes:
+                if prefix["Key"].endswith(DETAILS_FILE):
+                    try:
+                        row = self.add_row(Statute.get(prefix["Key"]))
+                        logger.success(f"Added: {row=}")
+                    except Exception as e:
+                        logger.error(f"Bad {prefix['key']}; {e=}")
+
+    def get_db_ids(self) -> Iterator[str]:
+        table = self.conn.db[StatuteRow.__tablename__]
+        for row in table.rows_where(select="id"):
+            yield row["id"]
+
+    def get_r2_ids(self) -> Iterator[str]:
+        if objs := self.storage.all_items():
+            for item in self.storage.filter_content(DETAILS_FILE, objs):
+                key = item["Key"].removesuffix(f"/{DETAILS_FILE}")
+                yield key.replace("/", ".")
+
+    def add_missing_r2_ids(self):
+        r2_ids = set(self.get_r2_ids())
+        db_ids = set(self.get_db_ids())
+        for id in r2_ids.difference(db_ids):
+            key = id.replace(".", "/")
+            prefix = f"{key}/{DETAILS_FILE}"
+            try:
+                self.add_row(Statute.get(prefix))
+                logger.success(f"Added: {prefix=}")
+            except Exception as e:
+                logger.error(f"Bad {prefix}; {e=}")
```

### Comparing `corpus_sc_toolkit-0.2.4/pyproject.toml` & `corpus_sc_toolkit-0.2.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "corpus-sc-toolkit"
 description = "Toolkit to process component elements of a Philippine Supreme Court decision."
-version = "0.2.4"
+version = "0.2.6"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
-license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/corpus-sc-toolkit"
 documentation = "https://mv3.dev/corpus-sc-toolkit"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
@@ -16,60 +15,41 @@
   "Framework :: Pydantic",
   "Intended Audience :: Legal Industry",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 # custom
-pylts = "^0.0.8" # litestream, sqlite database, loguru
-corpus-pax = "^0.1.24" # start-sdk, cloudflare, github api
-statute-trees = "^0.1.4"
-citation-utils = "^0.2.8"
+cloudflare-r2 = "^0.0.2"
+corpus-pax = "^0.1.27" # cloudflare-images, start-github, sqlpyd
+statute-trees = "^0.1.5"
+citation-utils = "^0.2.11"
 # helpers
 markdownify = "^0.11.6"
 unidecode = "^1.3.6"
-pebble = "^5.0.3"
+pebble = "^5.0.3" # needed to handle function timeouts
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
-black = "^23.1.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
-ipython = "^8.11.0"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 filterwarnings = ['ignore::DeprecationWarning']
 addopts = "-ra -q --doctest-modules --cov tests/"
-testpaths = ["tests"]
+testpaths = ["tests", "corpus_sc_toolkit"]
 
 [tool.ruff]
 ignore = ["F401"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
-[tool.black]
-target-version = ['py311']
-line-length = 79
-include = '.pyi?$'
-exclude = '''
-/(
-    .git
-    | .hg
-    | .mypy_cache
-    | .tox
-    | .venv
-    | _build
-    | buck-out
-    | build
-    | dist
-)/
-'''
-
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `corpus_sc_toolkit-0.2.4/PKG-INFO` & `corpus_sc_toolkit-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: corpus-sc-toolkit
-Version: 0.2.4
+Version: 0.2.6
 Summary: Toolkit to process component elements of a Philippine Supreme Court decision.
 Home-page: https://mv3.dev
-License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: citation-utils (>=0.2.8,<0.3.0)
-Requires-Dist: corpus-pax (>=0.1.24,<0.2.0)
+Requires-Dist: citation-utils (>=0.2.11,<0.3.0)
+Requires-Dist: cloudflare-r2 (>=0.0.2,<0.0.3)
+Requires-Dist: corpus-pax (>=0.1.27,<0.2.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: pebble (>=5.0.3,<6.0.0)
-Requires-Dist: pylts (>=0.0.8,<0.0.9)
-Requires-Dist: statute-trees (>=0.1.4,<0.2.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: statute-trees (>=0.1.5,<0.2.0)
 Requires-Dist: unidecode (>=1.3.6,<2.0.0)
 Project-URL: Documentation, https://mv3.dev/corpus-sc-toolkit
 Project-URL: Repository, https://github.com/justmars/corpus-sc-toolkit
 Description-Content-Type: text/markdown
 
 # corpus-sc-toolkit
 
@@ -37,7 +35,9 @@
 
 See [documentation](https://justmars.github.io/corpus-sc-toolkit).
 
 1. Run `poetry shell`
 2. Run `poetry update`
 3. Run `pytest`
 
+Could not originate prefix='gr/1290/1905/1/5/details.yaml'
+
```

