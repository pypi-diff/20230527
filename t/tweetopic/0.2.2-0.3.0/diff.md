# Comparing `tmp/tweetopic-0.2.2.tar.gz` & `tmp/tweetopic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweetopic-0.2.2.tar", max compression
+gzip compressed data, was "tweetopic-0.3.0.tar", max compression
```

## Comparing `tweetopic-0.2.2.tar` & `tweetopic-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0     1095 2022-09-01 08:37:21.990861 tweetopic-0.2.2/LICENSE
--rw-r--r--   0        0        0     2813 2023-02-23 14:58:53.569131 tweetopic-0.2.2/README.md
--rw-r--r--   0        0        0      471 2023-03-13 12:31:36.838892 tweetopic-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      147 2022-10-02 13:12:37.427033 tweetopic-0.2.2/tweetopic/__init__.py
--rw-r--r--   0        0        0    13299 2022-10-23 14:28:33.145423 tweetopic-0.2.2/tweetopic/_btm.py
--rw-r--r--   0        0        0    14754 2022-10-02 11:33:05.794099 tweetopic-0.2.2/tweetopic/_dmm.py
--rw-r--r--   0        0        0      872 2022-10-02 11:29:35.785488 tweetopic-0.2.2/tweetopic/_doc.py
--rw-r--r--   0        0        0     1236 2022-10-23 14:53:18.462175 tweetopic-0.2.2/tweetopic/_prob.py
--rw-r--r--   0        0        0     1033 2022-09-14 08:47:16.369750 tweetopic-0.2.2/tweetopic/_visualize.py
--rw-r--r--   0        0        0     6413 2022-10-23 14:45:47.606020 tweetopic-0.2.2/tweetopic/btm.py
--rw-r--r--   0        0        0     9686 2022-10-03 09:13:21.654739 tweetopic-0.2.2/tweetopic/dmm.py
--rw-r--r--   0        0        0       46 2022-09-02 08:56:27.846774 tweetopic-0.2.2/tweetopic/exceptions.py
--rw-r--r--   0        0        0     4858 2022-10-03 12:30:04.981046 tweetopic-0.2.2/tweetopic/pipeline.py
--rw-r--r--   0        0        0     3860 2022-09-14 08:47:29.453746 tweetopic-0.2.2/tweetopic/typing.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 tweetopic-0.2.2/setup.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 tweetopic-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2022-08-30 08:48:04.517506 tweetopic-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2838 2023-05-27 14:45:25.993150 tweetopic-0.3.0/README.md
+-rw-r--r--   0        0        0      489 2023-05-27 14:41:52.902359 tweetopic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-05-27 14:48:57.355819 tweetopic-0.3.0/tweetopic/__init__.py
+-rw-r--r--   0        0        0    15966 2023-05-27 12:45:41.313312 tweetopic-0.3.0/tweetopic/_btm.py
+-rw-r--r--   0        0        0    18378 2023-05-27 12:29:35.472442 tweetopic-0.3.0/tweetopic/_dmm.py
+-rw-r--r--   0        0        0      872 2022-11-01 20:04:23.385210 tweetopic-0.3.0/tweetopic/_doc.py
+-rw-r--r--   0        0        0     1236 2022-11-01 20:04:23.385210 tweetopic-0.3.0/tweetopic/_prob.py
+-rw-r--r--   0        0        0     6405 2023-05-27 12:34:29.362474 tweetopic-0.3.0/tweetopic/btm.py
+-rw-r--r--   0        0        0     9676 2023-05-27 12:33:37.178049 tweetopic-0.3.0/tweetopic/dmm.py
+-rw-r--r--   0        0        0       46 2022-08-30 11:16:26.746275 tweetopic-0.3.0/tweetopic/exceptions.py
+-rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 tweetopic-0.3.0/PKG-INFO
```

### Comparing `tweetopic-0.2.2/LICENSE` & `tweetopic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tweetopic-0.2.2/README.md` & `tweetopic-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-![Logo with text](./docs/_static/icon_w_title.png)
+<img align="left" width="82" height="82" src="docs/_static/icon.svg">
 
-# tweetopic: Blazing Fast Topic modelling for Short Texts
+# tweetopic
+
+<br>
+
+Blazing Fast Topic modelling for Short Texts
 
 [![PyPI version](https://badge.fury.io/py/tweetopic.svg)](https://pypi.org/project/tweetopic/)
 [![pip downloads](https://img.shields.io/pypi/dm/tweetopic.svg)](https://pypi.org/project/tweetopic/)
 [![python version](https://img.shields.io/badge/Python-%3E=3.7-blue)](https://github.com/centre-for-humanities-computing/tweetopic)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
```

### Comparing `tweetopic-0.2.2/tweetopic/_btm.py` & `tweetopic-0.3.0/tweetopic/_btm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Module for utility functions for fitting BTMs"""
 
 import random
 from typing import Dict, Tuple, TypeVar
 
-import numba
 import numpy as np
 from numba import njit
+from tqdm import tqdm
+
 from tweetopic._prob import norm_prob, sample_categorical
 
 
 @njit
 def doc_unique_biterms(
     doc_unique_words: np.ndarray, doc_unique_word_counts: np.ndarray
 ) -> Dict[Tuple[int, int], int]:
@@ -224,14 +225,57 @@
             topic_word_distribution[i_topic, i_term] = (
                 topic_word_count[i_topic, i_term] + beta
             ) / (n_topic_terms + n_vocab * beta)
     return topic_distribution, topic_word_distribution
 
 
 @njit(fastmath=True)
+def _sampling_step(
+    alpha: float,
+    beta: float,
+    n_components: int,
+    n_vocab: int,
+    biterms: np.ndarray,
+    n_biterms: int,
+    biterm_topic_assignments: np.ndarray,
+    topic_word_count: np.ndarray,
+    topic_biterm_count: np.ndarray,
+    prediction: np.ndarray,
+):
+    for i_biterm in range(n_biterms):
+        prev_topic = biterm_topic_assignments[i_biterm]
+        remove_biterm(
+            i_biterm=i_biterm,
+            i_topic=prev_topic,
+            biterms=biterms,
+            topic_word_count=topic_word_count,
+            topic_biterm_count=topic_biterm_count,
+        )
+        propose_topic_biterm(
+            prediction=prediction,
+            i_biterm=i_biterm,
+            n_components=n_components,
+            alpha=alpha,
+            beta=beta,
+            n_vocab=n_vocab,
+            biterms=biterms,
+            topic_word_count=topic_word_count,
+            topic_biterm_count=topic_biterm_count,
+        )
+        next_topic = sample_categorical(prediction)
+        add_biterm(
+            i_biterm=i_biterm,
+            i_topic=next_topic,
+            biterms=biterms,
+            topic_word_count=topic_word_count,
+            topic_biterm_count=topic_biterm_count,
+        )
+        biterm_topic_assignments[i_biterm] = next_topic
+
+
 def fit_model(
     n_iter: int,
     alpha: float,
     beta: float,
     n_components: int,
     n_vocab: int,
     biterms: np.ndarray,
@@ -239,62 +283,106 @@
     (
         biterm_topic_assignments,
         topic_word_count,
         topic_biterm_count,
     ) = init_components(n_components, n_vocab, biterms)
     n_biterms, _ = biterms.shape
     prediction = np.zeros(n_components)
-    for i_iter in range(n_iter):
-        n_transferred = 0
-        for i_biterm in range(n_biterms):
-            prev_topic = biterm_topic_assignments[i_biterm]
-            remove_biterm(
-                i_biterm=i_biterm,
-                i_topic=prev_topic,
-                biterms=biterms,
-                topic_word_count=topic_word_count,
-                topic_biterm_count=topic_biterm_count,
-            )
-            propose_topic_biterm(
-                prediction=prediction,
-                i_biterm=i_biterm,
-                n_components=n_components,
-                alpha=alpha,
-                beta=beta,
-                n_vocab=n_vocab,
-                biterms=biterms,
-                topic_word_count=topic_word_count,
-                topic_biterm_count=topic_biterm_count,
-            )
-            next_topic = sample_categorical(prediction)
-            add_biterm(
-                i_biterm=i_biterm,
-                i_topic=next_topic,
-                biterms=biterms,
-                topic_word_count=topic_word_count,
-                topic_biterm_count=topic_biterm_count,
-            )
-            biterm_topic_assignments[i_biterm] = next_topic
-            # NOTE: Consider branchless, if it affects performance
-            # n_tranferred += int(next_topic != prev_topic)
-            if next_topic != prev_topic:
-                n_transferred += 1
-        print(f" Iteration {i_iter}: transferred {n_transferred} biterms.")
+    iterator = tqdm(range(n_iter), desc="Sampling")
+    for _ in iterator:
+        _sampling_step(
+            alpha=alpha,
+            beta=beta,
+            n_components=n_components,
+            n_vocab=n_vocab,
+            biterms=biterms,
+            n_biterms=n_biterms,
+            biterm_topic_assignments=biterm_topic_assignments,
+            topic_word_count=topic_word_count,
+            topic_biterm_count=topic_biterm_count,
+            prediction=prediction,
+        )
     topic_distribution, topic_word_distribution = estimate_parameters(
         alpha=alpha,
         beta=beta,
         n_components=n_components,
         n_vocab=n_vocab,
         n_biterms=n_biterms,
         topic_word_count=topic_word_count,
         topic_biterm_count=topic_biterm_count,
     )
     return topic_distribution, topic_word_distribution
 
 
+#
+# @njit(fastmath=True)
+# def fit_model(
+#     n_iter: int,
+#     alpha: float,
+#     beta: float,
+#     n_components: int,
+#     n_vocab: int,
+#     biterms: np.ndarray,
+# ) -> Tuple[np.ndarray, np.ndarray]:
+#     (
+#         biterm_topic_assignments,
+#         topic_word_count,
+#         topic_biterm_count,
+#     ) = init_components(n_components, n_vocab, biterms)
+#     n_biterms, _ = biterms.shape
+#     prediction = np.zeros(n_components)
+#     for i_iter in range(n_iter):
+#         n_transferred = 0
+#         for i_biterm in range(n_biterms):
+#             prev_topic = biterm_topic_assignments[i_biterm]
+#             remove_biterm(
+#                 i_biterm=i_biterm,
+#                 i_topic=prev_topic,
+#                 biterms=biterms,
+#                 topic_word_count=topic_word_count,
+#                 topic_biterm_count=topic_biterm_count,
+#             )
+#             propose_topic_biterm(
+#                 prediction=prediction,
+#                 i_biterm=i_biterm,
+#                 n_components=n_components,
+#                 alpha=alpha,
+#                 beta=beta,
+#                 n_vocab=n_vocab,
+#                 biterms=biterms,
+#                 topic_word_count=topic_word_count,
+#                 topic_biterm_count=topic_biterm_count,
+#             )
+#             next_topic = sample_categorical(prediction)
+#             add_biterm(
+#                 i_biterm=i_biterm,
+#                 i_topic=next_topic,
+#                 biterms=biterms,
+#                 topic_word_count=topic_word_count,
+#                 topic_biterm_count=topic_biterm_count,
+#             )
+#             biterm_topic_assignments[i_biterm] = next_topic
+#             # NOTE: Consider branchless, if it affects performance
+#             # n_tranferred += int(next_topic != prev_topic)
+#             if next_topic != prev_topic:
+#                 n_transferred += 1
+#         print(f" Iteration {i_iter}: transferred {n_transferred} biterms.")
+#     topic_distribution, topic_word_distribution = estimate_parameters(
+#         alpha=alpha,
+#         beta=beta,
+#         n_components=n_components,
+#         n_vocab=n_vocab,
+#         n_biterms=n_biterms,
+#         topic_word_count=topic_word_count,
+#         topic_biterm_count=topic_biterm_count,
+#     )
+#     return topic_distribution, topic_word_distribution
+#
+
+
 @njit(fastmath=True)
 def prob_topic_given_biterm(
     w_i: int,
     w_j: int,
     prediction: np.ndarray,
     topic_distribution: np.ndarray,
     topic_word_distribution: np.ndarray,
```

### Comparing `tweetopic-0.2.2/tweetopic/_dmm.py` & `tweetopic-0.3.0/tweetopic/_dmm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Module containing tools for fitting a Dirichlet Multinomial Mixture Model."""
 from __future__ import annotations
 
 from math import exp, log
 
 import numpy as np
 from numba import njit
+from tqdm import tqdm
 
-from tweetopic._prob import sample_categorical, norm_prob
+from tweetopic._prob import norm_prob, sample_categorical
 
 
 @njit
 def _remove_add_doc(
     i_doc: int,
     i_cluster: int,
     remove: bool,
@@ -297,14 +298,76 @@
             max_unique_words=max_unique_words,
         )
     # Normalize probability vector
     norm_prob(probabilities)
 
 
 @njit(parallel=False)
+def _sampling_step(
+    alpha: float,
+    beta: float,
+    n_clusters: int,
+    n_vocab: int,
+    n_docs: int,
+    doc_unique_words: np.ndarray,
+    doc_unique_word_counts: np.ndarray,
+    doc_clusters: np.ndarray,
+    cluster_doc_count: np.ndarray,
+    cluster_word_count: np.ndarray,
+    cluster_word_distribution: np.ndarray,
+    max_unique_words: int,
+    prediction: np.ndarray,
+    doc_word_count: np.ndarray,
+) -> None:
+    for i_doc in range(n_docs):
+        # Removing document from previous cluster
+        prev_cluster = doc_clusters[i_doc]
+        # Removing document from the previous cluster
+        remove_doc(
+            i_doc,
+            prev_cluster,
+            cluster_word_distribution=cluster_word_distribution,
+            cluster_word_count=cluster_word_count,
+            cluster_doc_count=cluster_doc_count,
+            doc_unique_words=doc_unique_words,
+            doc_unique_word_counts=doc_unique_word_counts,
+            max_unique_words=max_unique_words,
+        )
+        # Getting new prediction for the document at hand
+        predict_doc(
+            probabilities=prediction,
+            i_document=i_doc,
+            doc_unique_words=doc_unique_words,
+            doc_unique_word_counts=doc_unique_word_counts,
+            n_words=doc_word_count[i_doc],
+            alpha=alpha,
+            beta=beta,
+            n_clusters=n_clusters,
+            n_vocab=n_vocab,
+            n_docs=n_docs,
+            cluster_doc_count=cluster_doc_count,
+            cluster_word_count=cluster_word_count,
+            cluster_word_distribution=cluster_word_distribution,
+            max_unique_words=max_unique_words,
+        )
+        new_cluster = sample_categorical(prediction)
+        # Adding document back to the newly chosen cluster
+        doc_clusters[i_doc] = new_cluster
+        add_doc(
+            i_doc,
+            new_cluster,
+            cluster_word_distribution=cluster_word_distribution,
+            cluster_word_count=cluster_word_count,
+            cluster_doc_count=cluster_doc_count,
+            doc_unique_words=doc_unique_words,
+            doc_unique_word_counts=doc_unique_word_counts,
+            max_unique_words=max_unique_words,
+        )
+
+
 def fit_model(
     n_iter: int,
     alpha: float,
     beta: float,
     n_clusters: int,
     n_vocab: int,
     n_docs: int,
@@ -312,99 +375,138 @@
     doc_unique_word_counts: np.ndarray,
     doc_clusters: np.ndarray,
     cluster_doc_count: np.ndarray,
     cluster_word_count: np.ndarray,
     cluster_word_distribution: np.ndarray,
     max_unique_words: int,
 ) -> None:
-    """Fits the Dirichlet Mixture Model with Gibbs Sampling. Implements
-    algorithm described in Yin & Wang (2014)
-
-    Parameters
-    ----------
-    n_iter: int
-        Number of iterations to conduct.
-    alpha: float
-        Alpha parameter of the model.
-    beta: float
-        Beta parameter of the model.
-    n_clusters: int
-        Number of mixture components in the model.
-    n_vocab: int
-        Number of total vocabulary items.
-    n_docs: int
-        Total number of documents.
-    doc_term_matrix: matrix of shape (n_documents, n_vocab)
-        Contains how many times a term occurs in each document.
-        (Bag of words matrix)
-    doc_unique_words: array of shape (MAX_UNIQUE_WORDS, )
-        Array containing all the ids of unique words in a document.
-    doc_clusters: array of shape (n_docs, )
-        Contains a cluster label for each document, that has
-        to be assigned.
-    doc_unique_words_count: array of shape (n_documents, )
-        Vector containing the number of unique terms in each document.
-    cluster_doc_count(OUT): array of shape (n_clusters,)
-        Array containing how many documents there are in each cluster.
-    cluster_word_count(OUT): array of shape (n_clusters,)
-        Contains the amount of words there are in each cluster.
-    cluster_word_distribution(OUT): matrix of shape (n_clusters, n_vocab)
-        Contains the amount a word occurs in a certain cluster.
-    max_unique_words: int
-        Maximum count of unique words in a document seen in the corpus.
-    """
     doc_word_count = np.sum(doc_unique_word_counts, axis=1)
     prediction = np.empty(n_clusters)
-    for iteration in range(n_iter):
-        total_transfers = 0
-        for i_doc in range(n_docs):
-            # Removing document from previous cluster
-            prev_cluster = doc_clusters[i_doc]
-            # Removing document from the previous cluster
-            remove_doc(
-                i_doc,
-                prev_cluster,
-                cluster_word_distribution=cluster_word_distribution,
-                cluster_word_count=cluster_word_count,
-                cluster_doc_count=cluster_doc_count,
-                doc_unique_words=doc_unique_words,
-                doc_unique_word_counts=doc_unique_word_counts,
-                max_unique_words=max_unique_words,
-            )
-            # Getting new prediction for the document at hand
-            predict_doc(
-                probabilities=prediction,
-                i_document=i_doc,
-                doc_unique_words=doc_unique_words,
-                doc_unique_word_counts=doc_unique_word_counts,
-                n_words=doc_word_count[i_doc],
-                alpha=alpha,
-                beta=beta,
-                n_clusters=n_clusters,
-                n_vocab=n_vocab,
-                n_docs=n_docs,
-                cluster_doc_count=cluster_doc_count,
-                cluster_word_count=cluster_word_count,
-                cluster_word_distribution=cluster_word_distribution,
-                max_unique_words=max_unique_words,
-            )
-            new_cluster = sample_categorical(prediction)
-            if prev_cluster != new_cluster:
-                total_transfers += 1
-            # Adding document back to the newly chosen cluster
-            doc_clusters[i_doc] = new_cluster
-            add_doc(
-                i_doc,
-                new_cluster,
-                cluster_word_distribution=cluster_word_distribution,
-                cluster_word_count=cluster_word_count,
-                cluster_doc_count=cluster_doc_count,
-                doc_unique_words=doc_unique_words,
-                doc_unique_word_counts=doc_unique_word_counts,
-                max_unique_words=max_unique_words,
-            )
-        n_populated = np.count_nonzero(cluster_doc_count)
-        print(
-            f" Iteration {iteration}/{n_iter}: transferred"
-            f" {total_transfers} documents,"
-            f"{n_populated} clusters remain populated.",
+    iterator = tqdm(range(n_iter), desc="Sampling")
+    for _ in iterator:
+        _sampling_step(
+            alpha=alpha,
+            beta=beta,
+            n_clusters=n_clusters,
+            n_vocab=n_vocab,
+            n_docs=n_docs,
+            doc_unique_words=doc_unique_words,
+            doc_unique_word_counts=doc_unique_word_counts,
+            doc_clusters=doc_clusters,
+            cluster_doc_count=cluster_doc_count,
+            cluster_word_count=cluster_word_count,
+            cluster_word_distribution=cluster_word_distribution,
+            max_unique_words=max_unique_words,
+            doc_word_count=doc_word_count,
+            prediction=prediction,
         )
+
+
+#
+# @njit(parallel=False)
+# def fit_model(
+#     n_iter: int,
+#     alpha: float,
+#     beta: float,
+#     n_clusters: int,
+#     n_vocab: int,
+#     n_docs: int,
+#     doc_unique_words: np.ndarray,
+#     doc_unique_word_counts: np.ndarray,
+#     doc_clusters: np.ndarray,
+#     cluster_doc_count: np.ndarray,
+#     cluster_word_count: np.ndarray,
+#     cluster_word_distribution: np.ndarray,
+#     max_unique_words: int,
+# ) -> None:
+#     """Fits the Dirichlet Mixture Model with Gibbs Sampling. Implements
+#     algorithm described in Yin & Wang (2014)
+#
+#     Parameters
+#     ----------
+#     n_iter: int
+#         Number of iterations to conduct.
+#     alpha: float
+#         Alpha parameter of the model.
+#     beta: float
+#         Beta parameter of the model.
+#     n_clusters: int
+#         Number of mixture components in the model.
+#     n_vocab: int
+#         Number of total vocabulary items.
+#     n_docs: int
+#         Total number of documents.
+#     doc_term_matrix: matrix of shape (n_documents, n_vocab)
+#         Contains how many times a term occurs in each document.
+#         (Bag of words matrix)
+#     doc_unique_words: array of shape (MAX_UNIQUE_WORDS, )
+#         Array containing all the ids of unique words in a document.
+#     doc_clusters: array of shape (n_docs, )
+#         Contains a cluster label for each document, that has
+#         to be assigned.
+#     doc_unique_words_count: array of shape (n_documents, )
+#         Vector containing the number of unique terms in each document.
+#     cluster_doc_count(OUT): array of shape (n_clusters,)
+#         Array containing how many documents there are in each cluster.
+#     cluster_word_count(OUT): array of shape (n_clusters,)
+#         Contains the amount of words there are in each cluster.
+#     cluster_word_distribution(OUT): matrix of shape (n_clusters, n_vocab)
+#         Contains the amount a word occurs in a certain cluster.
+#     max_unique_words: int
+#         Maximum count of unique words in a document seen in the corpus.
+#     """
+#     doc_word_count = np.sum(doc_unique_word_counts, axis=1)
+#     prediction = np.empty(n_clusters)
+#     for iteration in range(n_iter):
+#         total_transfers = 0
+#         for i_doc in range(n_docs):
+#             # Removing document from previous cluster
+#             prev_cluster = doc_clusters[i_doc]
+#             # Removing document from the previous cluster
+#             remove_doc(
+#                 i_doc,
+#                 prev_cluster,
+#                 cluster_word_distribution=cluster_word_distribution,
+#                 cluster_word_count=cluster_word_count,
+#                 cluster_doc_count=cluster_doc_count,
+#                 doc_unique_words=doc_unique_words,
+#                 doc_unique_word_counts=doc_unique_word_counts,
+#                 max_unique_words=max_unique_words,
+#             )
+#             # Getting new prediction for the document at hand
+#             predict_doc(
+#                 probabilities=prediction,
+#                 i_document=i_doc,
+#                 doc_unique_words=doc_unique_words,
+#                 doc_unique_word_counts=doc_unique_word_counts,
+#                 n_words=doc_word_count[i_doc],
+#                 alpha=alpha,
+#                 beta=beta,
+#                 n_clusters=n_clusters,
+#                 n_vocab=n_vocab,
+#                 n_docs=n_docs,
+#                 cluster_doc_count=cluster_doc_count,
+#                 cluster_word_count=cluster_word_count,
+#                 cluster_word_distribution=cluster_word_distribution,
+#                 max_unique_words=max_unique_words,
+#             )
+#             new_cluster = sample_categorical(prediction)
+#             if prev_cluster != new_cluster:
+#                 total_transfers += 1
+#             # Adding document back to the newly chosen cluster
+#             doc_clusters[i_doc] = new_cluster
+#             add_doc(
+#                 i_doc,
+#                 new_cluster,
+#                 cluster_word_distribution=cluster_word_distribution,
+#                 cluster_word_count=cluster_word_count,
+#                 cluster_doc_count=cluster_doc_count,
+#                 doc_unique_words=doc_unique_words,
+#                 doc_unique_word_counts=doc_unique_word_counts,
+#                 max_unique_words=max_unique_words,
+#             )
+#         n_populated = np.count_nonzero(cluster_doc_count)
+#         print(
+#             f" Iteration {iteration}/{n_iter}: transferred"
+#             f" {total_transfers} documents,"
+#             f"{n_populated} clusters remain populated.",
+#         )
```

### Comparing `tweetopic-0.2.2/tweetopic/_doc.py` & `tweetopic-0.3.0/tweetopic/_doc.py`

 * *Files identical despite different names*

### Comparing `tweetopic-0.2.2/tweetopic/_prob.py` & `tweetopic-0.3.0/tweetopic/_prob.py`

 * *Files identical despite different names*

### Comparing `tweetopic-0.2.2/tweetopic/btm.py` & `tweetopic-0.3.0/tweetopic/btm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 
 from typing import Union
 
 import numpy as np
 import scipy.sparse as spr
 import sklearn
 from numpy.typing import ArrayLike
-from tweetopic._btm import (compute_biterm_set, corpus_unique_biterms,
-                            fit_model, predict_docs)
+
+from tweetopic._btm import (
+    compute_biterm_set,
+    corpus_unique_biterms,
+    fit_model,
+    predict_docs,
+)
 from tweetopic._doc import init_doc_words
 from tweetopic.exceptions import NotFittedException
 
 
 class BTM(sklearn.base.TransformerMixin, sklearn.base.BaseEstimator):
     """Implementation of the Biterm Topic Model with Gibbs Sampling
     solver.
@@ -89,15 +94,15 @@
         }
 
     def set_params(self, **params) -> BTM:
         """Set parameters for this estimator.
 
         Returns
         -------
-        DMM
+        BTM
             Estimator instance
 
         Note
         ----
         Exists for sklearn compatibility.
         """
         for param, value in params.items():
```

### Comparing `tweetopic-0.2.2/tweetopic/dmm.py` & `tweetopic-0.3.0/tweetopic/dmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     """Implementation of the Dirichlet Mixture Model with Gibbs Sampling
     solver. The class aims to achieve full compatibility with sklearn.
 
     Parameters
     ----------
     n_components: int
         Number of mixture components in the model.
-    n_iterations: int, default 30
+    n_iterations: int, default 50
         Number of iterations during fitting.
+        If you find your results are unsatisfactory, increase this number.
     alpha: float, default 0.1
         Willingness of a document joining an empty cluster.
     beta: float, default 0.1
         Willingness to join clusters, where the terms in the document
         are not present.
 
     Attributes
@@ -44,16 +45,16 @@
         Total number of documents seen during fitting.
     max_unique_words: int
         Maximum number of unique words in a document seen during fitting.
     """
 
     def __init__(
         self,
-        n_components: int = 8,
-        n_iterations: int = 30,
+        n_components: int,
+        n_iterations: int = 50,
         alpha: float = 0.1,
         beta: float = 0.1,
     ):
         self.n_components = n_components
         self.n_iterations = n_iterations
         self.alpha = alpha
         self.beta = beta
@@ -138,21 +139,20 @@
         fit() works in-place too, the fitted model is returned for convenience.
         """
         # Converting X into sparse array if it isn't one already.
         X = spr.csr_matrix(X)
         self.n_documents, self.n_features_in_ = X.shape
         # Calculating the number of nonzero elements for each row
         # using the internal properties of CSR matrices.
+        print("Initializing components.")
         self.max_unique_words = np.max(np.diff(X.indptr))
-        print("Calculating unique words.")
         doc_unique_words, doc_unique_word_counts = init_doc_words(
             X.tolil(),
             max_unique_words=self.max_unique_words,
         )
-        print("Initialising mixture components")
         initial_clusters = np.random.multinomial(
             1,
             np.ones(self.n_components) / self.n_components,
             size=self.n_documents,
         )
         doc_clusters = np.argmax(initial_clusters, axis=1)
         self.cluster_doc_count = np.zeros(self.n_components)
@@ -163,15 +163,14 @@
             cluster_word_count=self.cluster_word_count,
             cluster_doc_count=self.cluster_doc_count,
             doc_clusters=doc_clusters,
             doc_unique_words=doc_unique_words,
             doc_unique_word_counts=doc_unique_word_counts,
             max_unique_words=self.max_unique_words,
         )
-        print("Fitting model")
         fit_model(
             n_iter=self.n_iterations,
             alpha=self.alpha,
             beta=self.beta,
             n_clusters=self.n_components,
             n_vocab=self.n_features_in_,
             n_docs=self.n_documents,
```

### Comparing `tweetopic-0.2.2/PKG-INFO` & `tweetopic-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweetopic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Topic modelling over short texts
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,19 +13,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: deprecated (>=1.2.0)
 Requires-Dist: joblib (>=1.1.0)
 Requires-Dist: numba (>=0.56.0)
 Requires-Dist: numpy (>=1.19,<1.24.0)
 Requires-Dist: scikit-learn (>=1.1.1,<1.3.0)
+Requires-Dist: tqdm (>=4.64.0)
 Description-Content-Type: text/markdown
 
-![Logo with text](./docs/_static/icon_w_title.png)
+<img align="left" width="82" height="82" src="docs/_static/icon.svg">
 
-# tweetopic: Blazing Fast Topic modelling for Short Texts
+# tweetopic
+
+<br>
+
+Blazing Fast Topic modelling for Short Texts
 
 [![PyPI version](https://badge.fury.io/py/tweetopic.svg)](https://pypi.org/project/tweetopic/)
 [![pip downloads](https://img.shields.io/pypi/dm/tweetopic.svg)](https://pypi.org/project/tweetopic/)
 [![python version](https://img.shields.io/badge/Python-%3E=3.7-blue)](https://github.com/centre-for-humanities-computing/tweetopic)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
```

