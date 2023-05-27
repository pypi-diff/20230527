# Comparing `tmp/crowsetta-5.0.0rc2.tar.gz` & `tmp/crowsetta-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowsetta-5.0.0rc2.tar", last modified: Mon Mar  6 16:54:23 2023, max compression
+gzip compressed data, was "crowsetta-5.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `crowsetta-5.0.0rc2.tar` & `crowsetta-5.0.1.tar`

### file list

```diff
@@ -1,170 +1,172 @@
--rw-r--r--   0        0        0      815 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.all-contributorsrc
--rw-r--r--   0        0        0     1311 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      749 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      823 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      356 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.gitignore
--rw-r--r--   0        0        0     1089 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      366 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.readthedocs.yaml
--rw-r--r--   0        0        0      746 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/CITATION.cff
--rw-r--r--   0        0        0     5556 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1879 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1515 2020-11-08 19:17:24.773706 crowsetta-5.0.0rc2/LICENSE
--rw-r--r--   0        0        0     8972 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/README.md
--rw-r--r--   0        0        0    21762 2023-03-06 15:41:14.149711 crowsetta-5.0.0rc2/doc/CHANGELOG.md
--rw-r--r--   0        0        0      580 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc2/doc/Makefile
--rw-r--r--   0        0        0    26325 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/doc/_static/crowsetta-logomark.png
--rw-r--r--   0        0        0   250992 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/doc/_static/crowsetta-primary-logo.png
--rw-r--r--   0        0        0    83463 2023-03-06 13:01:07.254070 crowsetta-5.0.0rc2/doc/_static/crowsetta-secondary-logo.png
--rw-r--r--   0        0        0  1638145 2023-03-06 13:01:07.258070 crowsetta-5.0.0rc2/doc/_static/example-raven-for-index.png
--rw-r--r--   0        0        0   640083 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/_static/example-textgrid-for-index.png
--rw-r--r--   0        0        0      612 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/_templates/class.rst
--rw-r--r--   0        0        0     1177 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/_templates/module.rst
--rw-r--r--   0        0        0     1857 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/core.md
--rw-r--r--   0        0        0      409 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/formats.md
--rw-r--r--   0        0        0      581 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/index.md
--rw-r--r--   0        0        0      565 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/interface.md
--rw-r--r--   0        0        0     6936 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/conf.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/data/.gitkeep
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/data/giraudon-et-al-2021/.gitkeep
--rw-r--r--   0        0        0      446 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/development/commit-abbreviations.rst
--rw-r--r--   0        0        0     8631 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/development/contributors.md
--rw-r--r--   0        0        0     1024 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/development/index.md
--rw-r--r--   0        0        0      741 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/bbox/raven.md
--rw-r--r--   0        0        0     1556 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/index.md
--rw-r--r--   0        0        0     1092 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/aud-seq.md
--rw-r--r--   0        0        0     1179 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/birdsongrec.md
--rw-r--r--   0        0        0     1268 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/generic-seq.md
--rw-r--r--   0        0        0      783 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/notmat.md
--rw-r--r--   0        0        0     1294 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/simple-seq.md
--rw-r--r--   0        0        0      717 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/textgrid.md
--rw-r--r--   0        0        0      739 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/timit.md
--rw-r--r--   0        0        0      231 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto.md
--rw-r--r--   0        0        0     7488 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/bat1_annotation.mat
--rw-r--r--   0        0        0     4503 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/batlab.py
--rw-r--r--   0        0        0     7256 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/convert-generic-seq.md
--rw-r--r--   0        0        0     9563 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/convert-simple-seq.md
--rw-r--r--   0        0        0    26382 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/howto-user-format.md
--rw-r--r--   0        0        0     2265 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/parsebat.py
--rw-r--r--   0        0        0    29107 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/remove-silent-labels-textgrid.md
--rw-r--r--   0        0        0    12885 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/index.md
--rw-r--r--   0        0        0      752 2020-11-08 19:17:24.773706 crowsetta-5.0.0rc2/doc/make.bat
--rw-r--r--   0        0        0      881 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/nitpick-ignore.txt
--rw-r--r--   0        0        0    19417 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt
--rw-r--r--   0        0        0  2942427 2023-03-06 13:01:07.270070 crowsetta-5.0.0rc2/doc/scripts/annot/b06_concat_dtw.TextGrid
--rw-r--r--   0        0        0   640046 2023-03-06 13:01:07.274070 crowsetta-5.0.0rc2/doc/scripts/audio/Recording_1_Segment_07-snippet.wav
--rw-r--r--   0        0        0   150046 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/scripts/audio/b06_concat-snippet.wav
--rw-r--r--   0        0        0     3885 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/scripts/raven-chronister-et-al-2021.md
--rw-r--r--   0        0        0     5966 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/scripts/textgrid-BF-dataset.md
--rw-r--r--   0        0        0    10627 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/tutorial.md
--rw-r--r--   0        0        0     2927 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/noxfile.py
--rw-r--r--   0        0        0     1969 2023-03-06 16:53:57.406967 crowsetta-5.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      846 2023-03-06 16:53:57.394967 crowsetta-5.0.0rc2/src/crowsetta/__about__.py
--rw-r--r--   0        0        0      882 2023-03-06 16:27:50.541769 crowsetta-5.0.0rc2/src/crowsetta/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/__init__.py
--rw-r--r--   0        0        0      379 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/AUTHORS
--rw-r--r--   0        0        0     1090 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/LICENSE
--rw-r--r--   0        0        0      723 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/README.md
--rw-r--r--   0        0        0       78 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/__init__.py
--rw-r--r--   0        0        0       41 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/exceptions.py
--rw-r--r--   0        0        0    32141 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/textgrid.py
--rw-r--r--   0        0        0     4559 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/annotation.py
--rw-r--r--   0        0        0     2406 2023-03-06 16:50:53.755772 crowsetta-5.0.0rc2/src/crowsetta/bbox.py
--rw-r--r--   0        0        0      469 2023-03-06 16:27:50.537769 crowsetta-5.0.0rc2/src/crowsetta/data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/__init__.py
--rw-r--r--   0        0        0      153 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/citation.txt
--rw-r--r--   0        0        0      887 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/spinetail.txt
--rw-r--r--   0        0        0     1828 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audseq/__init__.py
--rw-r--r--   0        0        0      238 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audseq/citation.txt
--rw-r--r--   0        0        0   651901 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/Annotation.xml
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/__init__.py
--rw-r--r--   0        0        0      172 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/citation.txt
--rw-r--r--   0        0        0    10424 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/data.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/generic/__init__.py
--rw-r--r--   0        0        0        5 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/generic/citation.txt
--rw-r--r--   0        0        0    19451 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/generic/example_custom_format.csv
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/notmat/__init__.py
--rw-r--r--   0        0        0      161 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/notmat/citation.txt
--rw-r--r--   0        0        0     2154 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat
--rw-r--r--   0        0        0      482 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/raven/Recording_1_Segment_02.Table.1.selections.txt
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/raven/__init__.py
--rw-r--r--   0        0        0      257 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/raven/citation.txt
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/simple/__init__.py
--rw-r--r--   0        0        0     2341 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv
--rw-r--r--   0        0        0      194 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/simple/citation.txt
--rw-r--r--   0        0        0    18463 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/1179.TextGrid
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/__init__.py
--rw-r--r--   0        0        0      233 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/citation.txt
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/timit/__init__.py
--rw-r--r--   0        0        0      173 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/timit/citation.txt
--rwxr-xr-x   0        0        0      542 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/timit/sa1.phn
--rw-r--r--   0        0        0     2631 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/__init__.py
--rw-r--r--   0        0        0       97 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/__init__.py
--rw-r--r--   0        0        0     8045 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/audbbox.py
--rw-r--r--   0        0        0     5935 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/raven.py
--rw-r--r--   0        0        0      398 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/__init__.py
--rw-r--r--   0        0        0     7753 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/audseq.py
--rw-r--r--   0        0        0    12711 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/birdsongrec.py
--rw-r--r--   0        0        0    14505 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/generic.py
--rw-r--r--   0        0        0     9478 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/notmat.py
--rw-r--r--   0        0        0    11167 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/simple.py
--rw-r--r--   0        0        0     7262 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/textgrid.py
--rw-r--r--   0        0        0     9960 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/timit.py
--rw-r--r--   0        0        0     7749 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/yarden.py
--rw-r--r--   0        0        0      286 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/__init__.py
--rw-r--r--   0        0        0      935 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/base.py
--rw-r--r--   0        0        0       58 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/bbox/__init__.py
--rw-r--r--   0        0        0     1636 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/bbox/base.py
--rw-r--r--   0        0        0       56 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/seq/__init__.py
--rw-r--r--   0        0        0     1800 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/interface/seq/base.py
--rw-r--r--   0        0        0     4123 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/segment.py
--rw-r--r--   0        0        0    18671 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/sequence.py
--rw-r--r--   0        0        0     7288 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/transcriber.py
--rw-r--r--   0        0        0      167 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/typing.py
--rw-r--r--   0        0        0     3508 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/validation.py
--rw-r--r--   0        0        0       24 2021-12-01 22:40:47.771260 crowsetta-5.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      174 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/tests/conftest.py
--rw-r--r--   0        0        0      345 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      270 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/audbbox.py
--rw-r--r--   0        0        0      314 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/audseq.py
--rw-r--r--   0        0        0      556 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/bbox.py
--rw-r--r--   0        0        0      579 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/birdsongrec.py
--rw-r--r--   0        0        0     1953 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/csv.py
--rw-r--r--   0        0        0      254 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/data.py
--rw-r--r--   0        0        0      406 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/example_user_format.py
--rw-r--r--   0        0        0      490 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/notmat.py
--rw-r--r--   0        0        0      884 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/raven.py
--rw-r--r--   0        0        0      912 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/tests/fixtures/segment.py
--rw-r--r--   0        0        0     1324 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/sequence.py
--rw-r--r--   0        0        0      530 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/simple.py
--rw-r--r--   0        0        0      283 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/textgrid.py
--rw-r--r--   0        0        0     1491 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/timit.py
--rw-r--r--   0        0        0      167 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/yarden.py
--rw-r--r--   0        0        0       23 2021-12-01 22:40:49.867233 crowsetta-5.0.0rc2/tests/helpers/__init__.py
--rw-r--r--   0        0        0      603 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/helpers/keywords.py
--rw-r--r--   0        0        0     4806 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/scripts/remake_test_csv.py
--rw-r--r--   0        0        0     2194 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_annotation.py
--rw-r--r--   0        0        0     1798 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_bbox.py
--rw-r--r--   0        0        0     9566 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_data.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_bbox/__init__.py
--rw-r--r--   0        0        0     4160 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_audbbox.py
--rw-r--r--   0        0        0     2744 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_raven.py
--rw-r--r--   0        0        0     1793 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_formats.py
--rw-r--r--   0        0        0        0 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/__init__.py
--rw-r--r--   0        0        0      200 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/asserts.py
--rw-r--r--   0        0        0     3579 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_audseq.py
--rw-r--r--   0        0        0     7271 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_birdsongrec.py
--rw-r--r--   0        0        0    24465 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_generic.py
--rw-r--r--   0        0        0     3897 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_notmat.py
--rw-r--r--   0        0        0     3940 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_simple.py
--rw-r--r--   0        0        0     3065 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_textgrid.py
--rw-r--r--   0        0        0     1937 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_timit.py
--rw-r--r--   0        0        0     3485 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_yarden.py
--rw-r--r--   0        0        0     1250 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/tests/test_segment.py
--rw-r--r--   0        0        0     7325 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_sequence.py
--rw-r--r--   0        0        0     3180 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_transcriber.py
--rw-r--r--   0        0        0      931 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_validation.py
--rw-r--r--   0        0        0    11470 1970-01-01 00:00:00.000000 crowsetta-5.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1185 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.all-contributorsrc
+-rw-r--r--   0        0        0     1311 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      750 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      826 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      356 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.gitignore
+-rw-r--r--   0        0        0     1089 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      367 2023-05-27 17:43:15.009356 crowsetta-5.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1345 2023-05-27 17:43:15.009356 crowsetta-5.0.1/CITATION.cff
+-rw-r--r--   0        0        0     5556 2023-05-27 17:43:15.009356 crowsetta-5.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1879 2023-05-27 17:43:15.009356 crowsetta-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1515 2020-11-08 19:17:24.773706 crowsetta-5.0.1/LICENSE
+-rw-r--r--   0        0        0     9985 2023-05-27 17:43:15.009356 crowsetta-5.0.1/README.md
+-rw-r--r--   0        0        0    23099 2023-05-27 18:10:38.342024 crowsetta-5.0.1/doc/CHANGELOG.md
+-rw-r--r--   0        0        0      580 2023-02-28 02:25:58.381961 crowsetta-5.0.1/doc/Makefile
+-rw-r--r--   0        0        0    26325 2023-05-27 17:43:15.013356 crowsetta-5.0.1/doc/_static/crowsetta-logomark.png
+-rw-r--r--   0        0        0   250992 2023-05-27 17:43:15.013356 crowsetta-5.0.1/doc/_static/crowsetta-primary-logo.png
+-rw-r--r--   0        0        0    83463 2023-05-27 17:43:15.013356 crowsetta-5.0.1/doc/_static/crowsetta-secondary-logo.png
+-rw-r--r--   0        0        0  1638145 2023-05-27 17:43:15.025356 crowsetta-5.0.1/doc/_static/example-raven-for-index.png
+-rw-r--r--   0        0        0   640083 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/_static/example-textgrid-for-index.png
+-rw-r--r--   0        0        0      612 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/_templates/class.rst
+-rw-r--r--   0        0        0     1177 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/_templates/module.rst
+-rw-r--r--   0        0        0     1857 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/api/core.md
+-rw-r--r--   0        0        0      409 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/api/formats.md
+-rw-r--r--   0        0        0      581 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/api/index.md
+-rw-r--r--   0        0        0      565 2023-05-27 17:43:15.029356 crowsetta-5.0.1/doc/api/interface.md
+-rw-r--r--   0        0        0     6936 2023-05-27 17:43:15.033356 crowsetta-5.0.1/doc/conf.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.033356 crowsetta-5.0.1/doc/data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.033356 crowsetta-5.0.1/doc/data/giraudon-et-al-2021/.gitkeep
+-rw-r--r--   0        0        0  2942427 2023-05-27 17:43:15.041355 crowsetta-5.0.1/doc/data/r6paq/b06_concat_dtw.TextGrid
+-rw-r--r--   0        0        0  2703945 2023-05-27 17:43:15.053355 crowsetta-5.0.1/doc/data/r6paq/b11_concat_dtw.TextGrid
+-rw-r--r--   0        0        0  6488878 2023-05-27 17:43:15.077355 crowsetta-5.0.1/doc/data/r6paq/b35_concat_dtw.TextGrid
+-rw-r--r--   0        0        0      446 2023-05-27 17:43:15.077355 crowsetta-5.0.1/doc/development/commit-abbreviations.rst
+-rw-r--r--   0        0        0     8631 2023-05-27 17:43:15.077355 crowsetta-5.0.1/doc/development/contributors.md
+-rw-r--r--   0        0        0     1024 2023-05-27 17:43:15.077355 crowsetta-5.0.1/doc/development/index.md
+-rw-r--r--   0        0        0      741 2023-05-27 17:43:15.077355 crowsetta-5.0.1/doc/formats/bbox/raven.md
+-rw-r--r--   0        0        0     1556 2023-05-27 17:43:15.077355 crowsetta-5.0.1/doc/formats/index.md
+-rw-r--r--   0        0        0     1092 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/aud-seq.md
+-rw-r--r--   0        0        0     1179 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/birdsongrec.md
+-rw-r--r--   0        0        0     1268 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/generic-seq.md
+-rw-r--r--   0        0        0      783 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/notmat.md
+-rw-r--r--   0        0        0     1294 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/simple-seq.md
+-rw-r--r--   0        0        0      756 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/textgrid.md
+-rw-r--r--   0        0        0      739 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/formats/seq/timit.md
+-rw-r--r--   0        0        0      230 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto.md
+-rw-r--r--   0        0        0     7488 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/bat1_annotation.mat
+-rw-r--r--   0        0        0     4503 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/batlab.py
+-rw-r--r--   0        0        0     7256 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/convert-generic-seq.md
+-rw-r--r--   0        0        0     9553 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/convert-simple-seq.md
+-rw-r--r--   0        0        0    26382 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/howto-user-format.md
+-rw-r--r--   0        0        0    24070 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/munging-annotations-textgrid.md
+-rw-r--r--   0        0        0     2265 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/howto/parsebat.py
+-rw-r--r--   0        0        0    12868 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/index.md
+-rw-r--r--   0        0        0      752 2020-11-08 19:17:24.773706 crowsetta-5.0.1/doc/make.bat
+-rw-r--r--   0        0        0      881 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/nitpick-ignore.txt
+-rw-r--r--   0        0        0    19417 2023-05-27 17:43:15.081355 crowsetta-5.0.1/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt
+-rw-r--r--   0        0        0  2942427 2023-05-27 17:43:15.093355 crowsetta-5.0.1/doc/scripts/annot/b06_concat_dtw.TextGrid
+-rw-r--r--   0        0        0   640046 2023-05-27 17:43:15.097355 crowsetta-5.0.1/doc/scripts/audio/Recording_1_Segment_07-snippet.wav
+-rw-r--r--   0        0        0   150046 2023-05-27 17:43:15.101355 crowsetta-5.0.1/doc/scripts/audio/b06_concat-snippet.wav
+-rw-r--r--   0        0        0     3885 2023-05-27 17:43:15.101355 crowsetta-5.0.1/doc/scripts/raven-chronister-et-al-2021.md
+-rw-r--r--   0        0        0     5966 2023-05-27 17:43:15.101355 crowsetta-5.0.1/doc/scripts/textgrid-BF-dataset.md
+-rw-r--r--   0        0        0    10627 2023-05-27 17:43:15.101355 crowsetta-5.0.1/doc/tutorial.md
+-rw-r--r--   0        0        0     3213 2023-05-27 17:43:15.101355 crowsetta-5.0.1/noxfile.py
+-rw-r--r--   0        0        0     1861 2023-05-27 18:10:38.362024 crowsetta-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0      843 2023-05-27 18:10:38.358024 crowsetta-5.0.1/src/crowsetta/__about__.py
+-rw-r--r--   0        0        0      882 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/__init__.py
+-rw-r--r--   0        0        0     5130 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/annotation.py
+-rw-r--r--   0        0        0     2406 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/bbox.py
+-rw-r--r--   0        0        0      469 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/audbbox/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/audbbox/citation.txt
+-rw-r--r--   0        0        0      887 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/audbbox/spinetail.txt
+-rw-r--r--   0        0        0     1828 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/audseq/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-27 17:43:15.101355 crowsetta-5.0.1/src/crowsetta/data/audseq/citation.txt
+-rw-r--r--   0        0        0   651901 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/birdsongrec/Annotation.xml
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/birdsongrec/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/birdsongrec/citation.txt
+-rw-r--r--   0        0        0    10434 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/data.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/generic/__init__.py
+-rw-r--r--   0        0        0        5 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/generic/citation.txt
+-rw-r--r--   0        0        0    19451 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/generic/example_custom_format.csv
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/notmat/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/notmat/citation.txt
+-rw-r--r--   0        0        0     2154 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat
+-rw-r--r--   0        0        0      482 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/raven/Recording_1_Segment_02.Table.1.selections.txt
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/raven/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/raven/citation.txt
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/simple/__init__.py
+-rw-r--r--   0        0        0     2341 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv
+-rw-r--r--   0        0        0      194 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/simple/citation.txt
+-rw-r--r--   0        0        0     2774 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/textgrid/AVO-maea-basic.TextGrid
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/textgrid/__init__.py
+-rw-r--r--   0        0        0      332 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/textgrid/citation.txt
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/timit/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/timit/citation.txt
+-rwxr-xr-x   0        0        0      542 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/data/timit/sa1.phn
+-rw-r--r--   0        0        0     2753 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/formats/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/formats/bbox/__init__.py
+-rw-r--r--   0        0        0     8234 2023-05-27 17:43:15.105355 crowsetta-5.0.1/src/crowsetta/formats/bbox/audbbox.py
+-rw-r--r--   0        0        0     6010 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/bbox/raven.py
+-rw-r--r--   0        0        0      398 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/__init__.py
+-rw-r--r--   0        0        0     7863 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/audseq.py
+-rw-r--r--   0        0        0    13028 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/birdsongrec.py
+-rw-r--r--   0        0        0    15100 2023-05-27 18:06:29.659695 crowsetta-5.0.1/src/crowsetta/formats/seq/generic.py
+-rw-r--r--   0        0        0     9525 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/notmat.py
+-rw-r--r--   0        0        0    11311 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/simple.py
+-rw-r--r--   0        0        0       55 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/textgrid/__init__.py
+-rw-r--r--   0        0        0     5311 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/textgrid/classes.py
+-rw-r--r--   0        0        0     7345 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/textgrid/parse.py
+-rw-r--r--   0        0        0    16675 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/textgrid/textgrid.py
+-rw-r--r--   0        0        0    10783 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/timit.py
+-rw-r--r--   0        0        0     7983 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/formats/seq/yarden.py
+-rw-r--r--   0        0        0      286 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/interface/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/interface/base.py
+-rw-r--r--   0        0        0       58 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/interface/bbox/__init__.py
+-rw-r--r--   0        0        0     1671 2023-05-27 17:43:15.109355 crowsetta-5.0.1/src/crowsetta/interface/bbox/base.py
+-rw-r--r--   0        0        0       56 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/interface/seq/__init__.py
+-rw-r--r--   0        0        0     1822 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/interface/seq/base.py
+-rw-r--r--   0        0        0     4160 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/segment.py
+-rw-r--r--   0        0        0    19292 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/sequence.py
+-rw-r--r--   0        0        0    10636 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/transcriber.py
+-rw-r--r--   0        0        0      167 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/typing.py
+-rw-r--r--   0        0        0     3609 2023-05-27 17:43:15.113355 crowsetta-5.0.1/src/crowsetta/validation.py
+-rw-r--r--   0        0        0       24 2021-12-01 22:40:47.771260 crowsetta-5.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-27 17:43:15.113355 crowsetta-5.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      345 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/audbbox.py
+-rw-r--r--   0        0        0      314 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/audseq.py
+-rw-r--r--   0        0        0      556 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/bbox.py
+-rw-r--r--   0        0        0      579 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/birdsongrec.py
+-rw-r--r--   0        0        0     1953 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/csv.py
+-rw-r--r--   0        0        0      254 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/data.py
+-rw-r--r--   0        0        0      406 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/example_user_format.py
+-rw-r--r--   0        0        0      490 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/notmat.py
+-rw-r--r--   0        0        0      884 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/raven.py
+-rw-r--r--   0        0        0      912 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/segment.py
+-rw-r--r--   0        0        0     1324 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/sequence.py
+-rw-r--r--   0        0        0      530 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/simple.py
+-rw-r--r--   0        0        0      973 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/textgrid.py
+-rw-r--r--   0        0        0     1491 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/timit.py
+-rw-r--r--   0        0        0      167 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/fixtures/yarden.py
+-rw-r--r--   0        0        0       23 2021-12-01 22:40:49.867233 crowsetta-5.0.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/helpers/keywords.py
+-rw-r--r--   0        0        0     4806 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/scripts/remake_test_csv.py
+-rw-r--r--   0        0        0     2194 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_annotation.py
+-rw-r--r--   0        0        0     1798 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_bbox.py
+-rw-r--r--   0        0        0     9566 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_data.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/test_bbox/__init__.py
+-rw-r--r--   0        0        0     4160 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/test_bbox/test_audbbox.py
+-rw-r--r--   0        0        0     2744 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/test_bbox/test_raven.py
+-rw-r--r--   0        0        0     1793 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/test_formats.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/test_seq/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-27 17:43:15.865350 crowsetta-5.0.1/tests/test_formats/test_seq/asserts.py
+-rw-r--r--   0        0        0     3579 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_audseq.py
+-rw-r--r--   0        0        0     7271 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_birdsongrec.py
+-rw-r--r--   0        0        0    24465 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_generic.py
+-rw-r--r--   0        0        0     3897 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_notmat.py
+-rw-r--r--   0        0        0     3940 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_simple.py
+-rw-r--r--   0        0        0        0 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_textgrid/__init__.py
+-rw-r--r--   0        0        0     3894 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_textgrid/test_classes.py
+-rw-r--r--   0        0        0     5193 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_textgrid/test_parse.py
+-rw-r--r--   0        0        0     4507 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_textgrid/test_textgrid.py
+-rw-r--r--   0        0        0     1937 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_timit.py
+-rw-r--r--   0        0        0     3485 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_formats/test_seq/test_yarden.py
+-rw-r--r--   0        0        0     1250 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_segment.py
+-rw-r--r--   0        0        0     7334 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_sequence.py
+-rw-r--r--   0        0        0     3180 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_transcriber.py
+-rw-r--r--   0        0        0      931 2023-05-27 17:43:15.869350 crowsetta-5.0.1/tests/test_validation.py
+-rw-r--r--   0        0        0    12337 1970-01-01 00:00:00.000000 crowsetta-5.0.1/PKG-INFO
```

### Comparing `crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `crowsetta-5.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `crowsetta-5.0.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/.github/workflows/ci.yml` & `crowsetta-5.0.1/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   pull_request:
 
 jobs:
   ci:
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: [3.9, "3.10", 3.11]
         os: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `crowsetta-5.0.0rc2/.github/workflows/lint.yml` & `crowsetta-5.0.1/.github/workflows/lint.yml`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       - uses: actions/checkout@v2
       - uses: psf/black@stable
         with:
           options: "--line-length=120"
           src: "./src"
       - uses: actions/setup-python@v2
         with:
-          python-version: 3.8
+          python-version: "3.10"
       - name: install libsndfile1 on ubuntu
         if: matrix.os == 'ubuntu-latest'
         run: sudo apt install libsndfile1
       - name: install
         run: |
           pip install nox
           pip install '.[dev]'
```

### Comparing `crowsetta-5.0.0rc2/.pre-commit-config.yaml` & `crowsetta-5.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/CODE_OF_CONDUCT.md` & `crowsetta-5.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/CONTRIBUTING.md` & `crowsetta-5.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/LICENSE` & `crowsetta-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/README.md` & `crowsetta-5.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 <img src="https://github.com/vocalpy/crowsetta/blob/main/doc/_static/crowsetta-primary-logo.png?raw=True" width="400">
 </div>
 <hr>
 
 ## A Python tool to work with any format for annotating animal vocalizations and bioacoustics data
 
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-review/issues/68)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05338/status.svg)](https://doi.org/10.21105/joss.05338)
 [![Build Status](https://github.com/vocalpy/crowsetta/actions/workflows/ci.yml/badge.svg)](https://github.com/vocalpy/crowsetta/actions)
 [![Documentation Status](https://readthedocs.org/projects/crowsetta/badge/?version=latest)](https://crowsetta.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/159904494.svg)](https://zenodo.org/badge/latestdoi/159904494)
 [![PyPI version](https://badge.fury.io/py/crowsetta.svg)](https://badge.fury.io/py/crowsetta)
 [![PyPI Python versions](https://img.shields.io/pypi/pyversions/crowsetta)](https://img.shields.io/pypi/pyversions/crowsetta)
 [![codecov](https://codecov.io/gh/vocalpy/crowsetta/branch/main/graph/badge.svg?token=TXtNTxXKmb)](https://codecov.io/gh/vocalpy/crowsetta)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 crowsetta provides a Pythonic way to work with annotation formats 
 for animal vocalizations and bioacoustics data. 
 These formats are used, for example, by 
 applications that enable users to annotate audio and/or spectrograms. 
 Such annotations typically include the times when sound events start and stop, 
@@ -188,16 +190,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="http://tessarhinehart.com"><img src="https://avatars.githubusercontent.com/u/27306428?v=4?s=100" width="100px;" alt="Tessa Rhinehart"/><br /><sub><b>Tessa Rhinehart</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=rhine3" title="Documentation">📖</a> <a href="https://github.com/vocalpy/crowsetta/issues?q=author%3Arhine3" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/shaupert"><img src="https://avatars.githubusercontent.com/u/43136040?v=4?s=100" width="100px;" alt="Sylvain HAUPERT"/><br /><sub><b>Sylvain HAUPERT</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=shaupert" title="Code">💻</a> <a href="#ideas-shaupert" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://tessarhinehart.com"><img src="https://avatars.githubusercontent.com/u/27306428?v=4?s=100" width="100px;" alt="Tessa Rhinehart"/><br /><sub><b>Tessa Rhinehart</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=rhine3" title="Documentation">📖</a> <a href="https://github.com/vocalpy/crowsetta/issues?q=author%3Arhine3" title="Bug reports">🐛</a> <a href="#userTesting-rhine3" title="User Testing">📓</a> <a href="#ideas-rhine3" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/shaupert"><img src="https://avatars.githubusercontent.com/u/43136040?v=4?s=100" width="100px;" alt="Sylvain HAUPERT"/><br /><sub><b>Sylvain HAUPERT</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=shaupert" title="Code">💻</a> <a href="#ideas-shaupert" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-shaupert" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/YannickJadoul"><img src="https://avatars.githubusercontent.com/u/8025744?v=4?s=100" width="100px;" alt="Yannick Jadoul"/><br /><sub><b>Yannick Jadoul</b></sub></a><br /><a href="#ideas-YannickJadoul" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/vocalpy/crowsetta/issues?q=author%3AYannickJadoul" title="Bug reports">🐛</a> <a href="https://github.com/vocalpy/crowsetta/commits?author=YannickJadoul" title="Documentation">📖</a> <a href="#userTesting-YannickJadoul" title="User Testing">📓</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `crowsetta-5.0.0rc2/doc/CHANGELOG.md` & `crowsetta-5.0.1/doc/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## Unreleased
+## 5.0.1 -- 2023-05-27
+### Fixed
+- Fix bug in "generic-seq" format; use validated dataframe 
+  returned by pandera schema, so that "label" column is 
+  coerced to strings
+  [#258](https://github.com/NickleDave/crowsetta/pull/258).
+  Fixes [#257](https://github.com/NickleDave/crowsetta/issues/257).
+
+## 5.0.0 -- 2023-03-29
 ### Added
 - Add information on contributing and setting up a development environment
   [#212](https://github.com/NickleDave/crowsetta/pull/212).
   Fixes [#30](https://github.com/NickleDave/crowsetta/issues/30).
 - Add method to convert generic sequence format to a pandas DataFrame
   [#216](https://github.com/NickleDave/crowsetta/pull/216).
 - Add additional vignettes to docs:
@@ -17,24 +25,41 @@
   [#216](https://github.com/NickleDave/crowsetta/pull/216).
   Fixes [#152](https://github.com/NickleDave/crowsetta/issues/152)
   and [#197](https://github.com/NickleDave/crowsetta/issues/197).
 - Add format class for Audacity extended label track format
   [#226](https://github.com/NickleDave/crowsetta/pull/226).
   Fixes [#222](https://github.com/NickleDave/crowsetta/issues/222)
   and [#213](https://github.com/NickleDave/crowsetta/issues/213).
+- Add the ability for a crowsetta.Annotation to have multiple sequences
+  [#243](https://github.com/NickleDave/crowsetta/pull/243).
+  Fixes [#42](https://github.com/NickleDave/crowsetta/issues/42).
+- Rewrite TextGrid class to better handle file formats:
+  parse both "short" and default format in either UTF-8 or UTF-16
+  encoding; remove empty intervals from interval tiers by default;
+  can convert multiple interval tiers to a single crowsetta.Annotation 
+  with multiple crowsetta.Sequences
+  [#243](https://github.com/NickleDave/crowsetta/pull/243).
+  Fixes [#241](https://github.com/NickleDave/crowsetta/issues/241)
 
 ### Removed
 - Remove `Segment.from_row` method, no longer used
   [#232](https://github.com/NickleDave/crowsetta/pull/232).
   Fixes [#231](https://github.com/NickleDave/crowsetta/issues/231)
 
 ### Fixed
 - Revise landing page of docs, and some vignettes. 
   Make other changes to clean up the docs build process 
   [#216](https://github.com/NickleDave/crowsetta/pull/216).
+- Coerce path-like attributes of `GenericSeq` dataframe schema to be strings.
+  This helps ensure these columns are always native Pandas types
+  [#237](https://github.com/NickleDave/crowsetta/pull/237).
+- Fix how the `crowsetta.Segment` class converts 
+  onset sample and offset sample to int; correctly handle 
+  multiple numpy integer subtypes
+  [#238](https://github.com/NickleDave/crowsetta/pull/238).
 
 ## 4.0.0.post2 -- 2022-06-25
 ### Changed
 - [c6ba100](https://github.com/vocalpy/crowsetta/commit/c6ba100d7335a880f2e1dbf66f5673ef562f3cc5)
   Fix description and uri in pyproject.toml and crowsetta/__about__.py
 - [f70828f](https://github.com/vocalpy/crowsetta/commit/f70828fc09102215ae9d8076f66a79d515db3388)
   Make README images link to raw GitHub files so they render on PyPI
```

### Comparing `crowsetta-5.0.0rc2/doc/Makefile` & `crowsetta-5.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_static/crowsetta-logomark.png` & `crowsetta-5.0.1/doc/_static/crowsetta-logomark.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_static/crowsetta-primary-logo.png` & `crowsetta-5.0.1/doc/_static/crowsetta-primary-logo.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_static/crowsetta-secondary-logo.png` & `crowsetta-5.0.1/doc/_static/crowsetta-secondary-logo.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_static/example-raven-for-index.png` & `crowsetta-5.0.1/doc/_static/example-raven-for-index.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_static/example-textgrid-for-index.png` & `crowsetta-5.0.1/doc/_static/example-textgrid-for-index.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_templates/class.rst` & `crowsetta-5.0.1/doc/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/_templates/module.rst` & `crowsetta-5.0.1/doc/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/api/core.md` & `crowsetta-5.0.1/doc/api/core.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/api/index.md` & `crowsetta-5.0.1/doc/api/index.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/api/interface.md` & `crowsetta-5.0.1/doc/api/interface.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/conf.py` & `crowsetta-5.0.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/development/contributors.md` & `crowsetta-5.0.1/doc/development/contributors.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/development/index.md` & `crowsetta-5.0.1/doc/development/index.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/bbox/raven.md` & `crowsetta-5.0.1/doc/formats/bbox/raven.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/index.md` & `crowsetta-5.0.1/doc/formats/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 that assigns it to a specific class.
 
 ### widely-used
 
 These are sequence-like formats for widely-used applications:
 
 - {ref}`Praat .TextGrid files <textgrid>`
-- {ref}`Audacity label tracks <aud-txt>`
+- {ref}`Audacity label tracks <aud-seq>`
 
 ### general
 
 These are formats that can represent a wide variety of sequence-like 
 annotation formats.
 
 - {ref}`simple-seq`
```

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/aud-seq.md` & `crowsetta-5.0.1/doc/formats/seq/aud-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/birdsongrec.md` & `crowsetta-5.0.1/doc/formats/seq/birdsongrec.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/generic-seq.md` & `crowsetta-5.0.1/doc/formats/seq/generic-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/notmat.md` & `crowsetta-5.0.1/doc/formats/seq/notmat.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/simple-seq.md` & `crowsetta-5.0.1/doc/formats/seq/simple-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/textgrid.md` & `crowsetta-5.0.1/doc/formats/seq/textgrid.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 (textgrid)=
 
-# Praat .TextGrid files
+# Praat TextGrid files
 
-Annotation format saved by the [Praat](https://www.fon.hum.uva.nl/praat/) application. 
-More details about annotating with Praat can be found here:
+Annotation file format saved by the [Praat](https://www.fon.hum.uva.nl/praat/) application. 
+
+More details about annotating with Praat can be found here:  
 <https://www.fon.hum.uva.nl/praat/manual/Intro_7__Annotation.html>
-The specification for TextGrid objects is here: 
-<https://www.fon.hum.uva.nl/praat/manual/TextGrid.html>
 
-Internally, crowsetta uses the Python tool `textgrid`
-(<https://github.com/kylebgorman/textgrid>) to load .TextGrid files. 
-A version is distributed with crowsetta 
-under [MIT license](https://github.com/kylebgorman/textgrid/blob/master/LICENSE).
+The specification for TextGrid files is here:  
+<https://www.fon.hum.uva.nl/praat/manual/TextGrid_file_formats.html>
 
 The annotations can be loaded with the following class: 
 {py:class}`crowsetta.formats.seq.textgrid.TextGrid`.
+Please see that documentation for more details 
+and examples of which TextGrid files 
+crowsetta can parse, and how crowsetta can convert 
+interval tiers from TextGrid files to 
+{py:class}`crowsetta.Sequence` instances 
+and {py:class}`crowsetta.Annotation` instances.
```

### Comparing `crowsetta-5.0.0rc2/doc/formats/seq/timit.md` & `crowsetta-5.0.1/doc/formats/seq/timit.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/howto/bat1_annotation.mat` & `crowsetta-5.0.1/doc/howto/bat1_annotation.mat`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/howto/batlab.py` & `crowsetta-5.0.1/doc/howto/batlab.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/howto/convert-generic-seq.md` & `crowsetta-5.0.1/doc/howto/convert-generic-seq.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 where we have multiple annotation files, 
 we use a loop to load each one and convert it to a 
 {class}`crowsetta.Annotation` instance.
  
 We use the same dataset we used in the {ref}`tutorial` for this example, 
 ["Labeled songs of domestic canary M1-2016-spring (Serinus canaria)"](https://zenodo.org/record/6521932)
 by Giraudon et al., 2021, 
-annotated with {ref}`Audacity Labeltrack <aud-txt>` files.
+annotated with {ref}`Audacity Labeltrack <aud-seq>` files.
 
 ```{code-cell} ipython3
 cd ..
 ```
 
 First we download and extract the dataset, if we haven't already.
```

### Comparing `crowsetta-5.0.0rc2/doc/howto/convert-simple-seq.md` & `crowsetta-5.0.1/doc/howto/convert-simple-seq.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 that retains only the information required to train 
 machine learning models to perform the task.
 crowsetta provides simplified representations 
 of annotation formats that map directly to machine learning tasks, 
 and makes it easy to convert your annotations 
 in widely used formats to these simplified representations.
 
-This vignette shows how to convert {ref}`sequence-like <sequence-like-formats>` annotations 
+This vignette shows how to convert {ref}`sequence-like <formats-seq-like>` annotations 
 to a simplified format that is useful for tasks 
 such as building data sets for machine learning.
 In this vignette, we write an example small Python script
 to convert a set of annotations 
 to the `'simple-seq'` format using the pandas library.
 We then show that we are able to load the annotations 
 with crowsetta after converting them.
@@ -76,15 +76,15 @@
 and the vak library similarly allows for 
 [building datasets with a simple csv format](https://vak.readthedocs.io/en/latest/howto/howto_user_annot.html#method-1-converting-your-annotations-to-the-simple-seq-format)
 (this vignette is adapted from that section of the vak docs).
 
 ### What types of annotation formats will this work with
 
 The approach shown here will work for a wide array of annotation formats 
-that crowsetta calls {ref}`sequence-like <sequence-like-formats>`,
+that crowsetta calls {ref}`sequence-like <formats-seq-like>`,
 because they can all be represented as a sequence of segments, 
 with each segment having an onset time, offset time, and label.
 
 **The one assumption the `'simple-seq'` format makes is that you have one annotation file 
 per file that is annotated, that is, 
 one annotation file per audio file or per array file containing a spectrogram.**
 This is likely to be the case if you are using apps like Praat or Audacity.
@@ -93,15 +93,15 @@
 exported to .txt files, that you would get if you were to annotate with  
 [region labels](https://manual.audacityteam.org/man/label_tracks.html#type).
 We use the Audacity format in this vignette.
 
 ### Downloading the example dataset
 
 We download some examples of annotation files in the 
-{ref}`Audacity LabelTrack format <aud-txt>`, 
+{ref}`Audacity LabelTrack format <aud-seq>`, 
 from the dataset 
 ["Labeled songs of domestic canary M1-2016-spring (Serinus canaria)"](https://zenodo.org/record/6521932)
 by Giraudon et al., 2021.
 
 ```{code-cell} ipython3
 cd ..
 ```
```

### Comparing `crowsetta-5.0.0rc2/doc/howto/howto-user-format.md` & `crowsetta-5.0.1/doc/howto/howto-user-format.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/howto/parsebat.py` & `crowsetta-5.0.1/doc/howto/parsebat.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/howto/remove-silent-labels-textgrid.md` & `crowsetta-5.0.1/doc/howto/munging-annotations-textgrid.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,110 +5,84 @@
     format_name: myst
     format_version: 0.13
     jupytext_version: 1.14.5
 kernelspec:
   display_name: Python 3 (ipykernel)
   language: python
   name: python3
+mystnb:
+  execution_timeout: 300
 ---
 
-(howto-remove-silent-labels-textgrid)=
+(munging-annotations-textgrid)=
 
-# How to use crowsetta to remove unlabeled intervals from TextGrid annotations
+# Munging annotations from Praat TextGrid files with crowsetta to fit a first-order Markov model of birdsong syntax
 
 A common need when working with annotations 
 for animal vocalizations 
 is to transform them to perform a certain analysis.
 This is a sort of [data munging](https://en.wikipedia.org/wiki/Data_wrangling).
 In this vignette, we provide a simple example of munging annotations to build a model of birdsong syntax.
 
-We will work with a dataset 
-of Bengalese finch song annotated with the 
-[Praat .TextGrid format](https://www.fon.hum.uva.nl/praat/manual/TextGrid_file_formats.html).
+We will work with a 
+[dataset of Bengalese finch song](https://nickledave.github.io/bfsongrepo/)
+annotated in a format used by ["evsonganaly"](https://github.com/NickleDave/evfuncs),
+a MATLAB GUI for annotating song.
 We want to build a matrix of the transition probabilities between syllables in the song, 
 that is, a first-order [Markov model](https://en.wikipedia.org/wiki/Markov_chain).
-But before we can do that, 
-we need to clean the data.
-
-Specifically, we need to remove the labels that Praat gives 
-to all of the silent periods between syllables when it saves a TextGrid file.
-In the terminology of Praat, 
-we need to remove the *intervals* 
-that have empty labels.
-[Praat allows annotators to create multiple *tiers*](https://www.fon.hum.uva.nl/praat/manual/Intro_7__Annotation.html), or
-or levels, of labeling 
-E.g., if we were annotating speech, 
-we could have a tier each for phonemes, syllables, 
-words, and sentences.
-In this example we will work with interval tiers, 
-that consists of a set of *intervals* as the name suggests.
-(There are also point tiers where annotators label single time points.)
-Each interval has a start time, stop time, and label,
-all created by an annotator working with the Praat GUI.
-When the annotator does not assign a label to some interval, 
-then the corresponding TextGrid file will contain an interval with an empty label. 
-Commonly this happens for silent periods between intervals of interest.
-In our case, it happens for every brief (50-100ms) silent gap 
-between the syllables in a Bengalese finch's song.
-These lables become `None` when we load them into crowsetta.
-We don't want to include these intervals as states in our Markov model, 
-because we are only interested in transitions between syllables.
-So, to compute our transition matrix, 
-we need to remove all these intervals with `None` labels.
 
 +++
 
 ```{admonition} Download this page as a Jupyter notebook!
 To work with this tutorial interactively, 
 we suggest downloading this notebook!
 Click on the download icon in the upper right 
 to download a Markdown file (with '.md' extension) 
 that you can run as a Jupyter notebook 
 after installing Jupyter lab and jupytext.
 ```
 
 +++
 
-
-
-
 ## Workflow
 
 Here's the steps we'll follow:  
 
 0. Write code for analysis
-1. Download data from Open Science Framework
-2. Load data with crowsetta
-3. Remove `None` labels
-4. Compute transition matrix
+1. Load .not.mat files saved by evsonganaly with crowsetta, and convert to crowsetta Annotations with Sequences
+2. Munge data
+3. Compute transition matrices
 
 For this vignette, we use annotations from the 
-[Bengalese finch song dataset](https://osf.io/r6paq/), 
-by Tachibana and Morita 2021, adapted under 
+[Bengalese finch song repository](https://nickledave.github.io/bfsongrepo), 
+by Nicholson, Queen, Sober 2017 [^1], adapted under 
 [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).
 
+[^1]: Nicholson, D., Queen, J. E., & J. Sober, S. (2017). Bengalese Finch song repository (Version 7).
+figshare. https://doi.org/10.6084/m9.figshare.4805749.v7
+
 +++
 
 ## 0. Write code for analysis
 
 Before we can analyze our data, we need to know what analysis we're doing.
 It can save you a lot of time to write a rough draft of this analysis code first, 
 and test it with some toy data that you generate.
 
 We also do this first to help understand what format we're going to need to get our data into below.
 
 Our goal here is to fit a first-order Markov model of the transition probabilities in the song of Bengalese finches. 
-This model has been used in several previous studies[^1][^2], 
-although it was later shown[^3] that such a model does not completely describe the statistics of the song. 
+This model has been used in several previous studies[^2][^3], 
+although it was later shown[^4] that such a model does not completely describe the statistics of the song. 
 In spite of that, a first-order Markov model is very convenient to fit, 
 and can give us a useful first-order approximation (literally!) of singing behavior.
 
-[^1]: Woolley SM, Rubel EW (1997) Bengalese finches lonchura striata domestica depend upon auditory feedback for the maintenance of adult song. J Neurosci 17: 6380–90.
-[^2]: Honda E, Okanoya K (1999) Acoustical and syntactical comparisons between songs of the white-backed munia (lonchura striata) and its domesticated strain, the bengalese finch (lonchura striata var. domestica). Zool Sci 16: 319–326.
-[^3]: Jin DZ, Kozhevnikov AA (2011) A Compact Statistical Model of the Song Syntax in Bengalese Finch. PLOS Computational Biology 7(3): e1001108. https://doi.org/10.1371/journal.pcbi.1001108
+[^2]: Woolley SM, Rubel EW (1997) Bengalese finches lonchura striata domestica depend upon auditory feedback for the maintenance of adult song. J Neurosci 17: 6380–90.
+[^3]: Honda E, Okanoya K (1999) Acoustical and syntactical comparisons between songs of the white-backed munia (lonchura striata) and its domesticated strain, the bengalese finch (lonchura striata var. domestica). Zool Sci 16: 319–326.
+[^4]: Jin DZ, Kozhevnikov AA (2011) A Compact Statistical Model of the Song Syntax in Bengalese Finch. PLOS Computational Biology 7(3): e1001108. https://doi.org/10.1371/journal.pcbi.1001108
 
 To build such a model for Bengalese finch song, 
 we consider the song syllables to be states. 
 We construct a transition matrix $P$ where the rows 
 are the state we're transitioning from, 
 the columns are the state we're transitioning to, 
 and thus the value in each cell $p_{i, j}$ is 
@@ -136,15 +110,15 @@
 The functions are written in such a way that, 
 after cleaning and transforming our loaded annotations, 
 we pass them into the second function, and it will call the first one for us 
 when it computes the transition matrix.
 
 ```{note}
 This code is adapted from
-https://github.com/yardencsGitHub/tweetynet/blob/master/article/src/article/bfbehav/sequence.py
+<https://github.com/yardencsGitHub/tweetynet/blob/master/article/src/article/bfbehav/sequence.py>
 under [BSD license](https://github.com/yardencsGitHub/tweetynet/blob/master/LICENSE).
 
 As used for the paper
 Cohen, Y., Nicholson, D., Sanchioni, A., Mallaber, E., Skidanova, V., & Gardner, T. (2022). 
 Automated annotation of birdsong with a neural network that segments spectrograms. eLife. <https://doi.org/10.7554/eLife.63853>
 ```
 
@@ -303,209 +277,87 @@
     if thresh is not None:
         trans_mat[trans_mat < thresh] = 0.0
         trans_mat = row_norm(trans_mat)
 
     return TransitionMatrix(counts=counts, matrix=trans_mat, states=states)
 ```
 
-## 1. Download data from Open Science Framework
+## 1. Load data with crowsetta
 
 +++
 
-The annotations we want to use are in a public project on the [Open Science Framework](osf.io).
-To download the files, we use the Python package [`osfclient`](https://github.com/osfclient/osfclient). First we make sure it is installed.
-
-```{code-cell} ipython3
-!pip install osfclient
-```
-
-Then we import the package.
-
-```{code-cell} ipython3
-import osfclient
-```
-
-We change directories to download into the `./data` directory we have set up for our project, following [good practices](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510#sec009).
+We change directories so we can access the `./data` directory we have set up for our project, following [good practices](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510#sec009).
 
 ```{code-cell} ipython3
 cd ..
 ```
 
-We write a helper function to list the files in a project.
-This function is adapted 
-from the command-line interface of `osfclient`, 
-specifically 
-[the `list` function found in the `osfclient.cli` module]((https://github.com/osfclient/osfclient/blob/411497f67aae457a238f0b91ef864d38d6879918/osfclient/cli.py#L255)).
-(Code is adapted under [BSD license](https://github.com/osfclient/osfclient/blob/master/LICENSE).)
-
-```{code-cell} ipython3
-import os
-
-
-def get_files_list(project):
-    """Get a list all files from all storages for project."""
-    files = []
-
-    for store in project.storages:
-        prefix = store.name
-        for file_ in store.files:
-            path = file_.path
-            if path.startswith('/'):
-                path = path[1:]
-            files.append(
-                os.path.join(prefix, path)
-            )
-    
-    return files
-```
-
-We also write a helper function to download a list of files.
-This function is adapted from the `clone` function of the `osfclient.cli` module,
-found 
-[here](https://github.com/osfclient/osfclient/blob/411497f67aae457a238f0b91ef864d38d6879918/osfclient/cli.py#L147).
-
-```{code-cell} ipython3
-def fetch_files(project, file_paths, output_dir=None, update=True):
-    """Fetch a list of files from an OSF project"""
-    if output_dir is None:
-        output_dir = project.id
-    else:
-        output_dir = os.path.join(output_dir, project.id)
-
-    for store in project.storages:
-        for file_ in store.files:
-            file_path = file_.path
-            if file_path.startswith('/'):
-                file_path = file_path[1:]
-            file_path = os.path.join(store.name, file_path)
-
-            dst_path = os.path.join(output_dir, file_path)
-            if os.path.exists(dst_path) and update:
-                if osfclient.utils.checksum(dst_path) == file_.hashes.get('md5'):
-                    continue
-
-            # do not download if this file is not in the list that we passed in
-            if file_path not in file_paths:
-                print(
-                    f'Not in file_paths, skipping: {file_path}'
-                )
-                continue
-            directory, _ = os.path.split(dst_path)
-            osfclient.utils.makedirs(directory, exist_ok=True)
-
-            with open(dst_path, "wb") as f:
-                print(
-                    f'Downloading: {file_}'
-                )
-                file_.write_to(f)
-```
-
-Now we can use our functions to download *just* the TextGrid files from the project.
-
-To do so, we need the project's ID number. 
-Conveniently, this is the last part of the url for any project, 
-so we can copy the project's url by hand and then get the project ID from it 
-using the Python `String` method `split`.
-
-```{code-cell} ipython3
-project_url = 'https://osf.io/r6paq/'
-project_id = project_url.split('/')[-2]  # -2 because -1 is an empty string from trailing slash
-```
-
-We make an instance of the `osfclient` class `OSF` that represents the API, 
-and then use that instance's `project` method to make a `Project` instance 
-that represents the project we want to access programmatically.
-
-```{code-cell} ipython3
-osf = osfclient.OSF()
-project = osf.project(project_id)
-```
-
-Now we can get the list of files from the project's public storage, using our first helper function from above.
-
-```{code-cell} ipython3
-project_files = get_files_list(project)
-```
-
-We only want to keep the annotation files, so we filter the list using a 
-[list comprehension](https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions).
-
-```{code-cell} ipython3
-project_files = [file for file in project_files if file.endswith('TextGrid')]
-```
-
-The last step before we can clean our data is to fetch the files from the storage.
-
-```{code-cell} ipython3
-fetch_files(project, project_files, output_dir='./data')
-```
-
-## 2. Load data with crowsetta
-
-+++
-
-Our TextGrid files are in the output directory we specified when calling our helper function (`'./data`), 
-which made new subdirectories inside of that directory with our project's ID and the file paths from that project: 
-`./data/r6pqa/osfstorage/TextGrid`.
+Our TextGrid files are in a sub-directory, `./data/r6pqa` (the unique ID associated with the OSF project for the dataset).
 
 We get a list of the TextGrid files from that subdirectory using `pathlib`.
 
+To download these files and work with them locally, click the following links:
+{download}`b06_concat_dtw.TextGrid<../data/r6paq/b06_concat_dtw.TextGrid>`  
+{download}`b11_concat_dtw.TextGrid<../data/r6paq/b11_concat_dtw.TextGrid>`
+{download}`b35_concat_dtw.TextGrid<../data/r6paq/b35_concat_dtw.TextGrid>`  
+
 ```{code-cell} ipython3
 import pathlib
 
-downloaded_dir = pathlib.Path('./data/r6paq/osfstorage/TextGrid/')
+downloaded_dir = pathlib.Path('./data/r6paq/')
 ```
 
 We make sure that our paths are `sorted` just in case 
 [it matters](https://www.vice.com/en/article/zmjwda/a-code-glitch-may-have-caused-errors-in-more-than-100-published-studies) 
 for our analysis.
 
 ```{code-cell} ipython3
 textgrid_paths = sorted(downloaded_dir.glob('*.TextGrid'))
 ```
 
 We inspect the first four paths just to check that we got what we expect.
 
 ```{code-cell} ipython3
-textgrid_paths[:4]
+textgrid_paths
 ```
 
 Looks like it. 
 
-Each of the files corresponds to all the song from one individual bird. E.g., the file `b01_concat_dtw.TextGrid` contains annotations from the bird with ID "b01" and the file `b03_concat_dtw.TextGrid` contains annotations from the bird with ID "b03".
+Each of the files corresponds to all the song from one individual bird. E.g., the file `b06_concat_dtw.TextGrid` contains annotations from the bird with ID "b06" and the file `b011_concat_dtw.TextGrid` contains annotations from the bird with ID "b11".
 
 We will need to do some book-keeping as we transform our data so we that we're able to fit a model for each bird. Mainly this will involve using Python dictionaries where the bird's ID is the key, and pandas DataFrames where we have the ID in a column.
 
 But first let's load all those annotations with crowsetta to get a sense of them.
 
 ```{code-cell} ipython3
 import crowsetta
 
 scribe = crowsetta.Transcriber(format='textgrid')
 ```
 
-Some of the files won't load because of overlapping IntervalTiers.  
-We skip those and just load the ones that will.
+Notice below the argument `keep_empty=True`. The parameter `keep_empty` defaults to `False`, but we actually want to keep the unlabeled intervals between syllables, because they will help us divide the song up into bouts, as we will see below.
+
+These are large files (that concatenate annotations across a day of song for each bird) so they take a while to load.
 
 ```{code-cell} ipython3
 textgrids = {}
 
 for textgrid_path in textgrid_paths:
-    try:
-        bird_id = textgrid_path.name.split('_')[0]  # bird ID will be first element from list after split
-        annot = scribe.from_file(textgrid_path)
-        textgrids[bird_id] = annot
-    except ValueError:
-            continue
+    bird_id = textgrid_path.name.split('_')[0]  # bird ID will be first element from list after split
+    annot = scribe.from_file(textgrid_path, keep_empty=True)
+    textgrids[bird_id] = annot
 ```
 
-## 3. Remove `None` labels
+## 2. Munge data
+
+Now we want to munge the data into the format we want to carry out our analysis.
+
+#### Looking at descriptive statistics
 
-Now we can look at the counts of the different classes of labels.  
-This helps us get an overview of our data before we do anything to it.
+A good first thing to do with any new dataset is plot some descriptive statistics to get an overview of the data before we do anything with it. As an example of this, let's look at the counts of the different classes of labels.  
 
 First we convert the TextGrid annotations to `crowsetta.Annotation`s to make them easier to work with.  
 Here we use a dictionary comprehension to transform our `textgrids` dictionary to a dictionary of `crowsetta.Annotation`s.
 
 ```{code-cell} ipython3
 annots = {bird_id: textgrid.to_annot() 
           for bird_id, textgrid in textgrids.items()}
@@ -519,51 +371,39 @@
 counts = Counter(
     [lbl for annot in annots.values() for lbl in annot.seq.labels]
 )
 
 print(counts)
 ```
 
-We can see that we have many segments in our sequences that have no labels, 
-these are the ones that give us an empty string, `''`.  
+We can see that we have many segments in our sequences that have the label `'x'`. 
+These are squawky "intro" notes that are sometimes ommitted from models of song syntax.  
 
 In fact this is the most frequent label! 
 (The `collection.Counter` prints its key-value pairs in descending order of value by default.)
 
-These empty string labels in the `crowsetta.Annotation`s are the `IntervalTier`s that have `None` labels, that we want to remove.
-
-To demonstrate this we show the very first interval from the interval tier, and the corresponding label from the first segment of the `crowsetta.Sequence` from the first `crowsetta.Annotation`.
-
-```{code-cell} ipython3
-textgrids['b06'].textgrid[0][0]
-```
-
-```{code-cell} ipython3
-annots['b06'].seq.segments[0].label
-```
-
-We also saw above that the second most common label is `'x'`. 
-These are squawky "intro" notes that are sometimes ommitted from models of song syntax.  
-We will remove those as well when cleaning our data.
+We will remove the squawky "intro" notes for this analysis (this is sometimes called "cleaning" data, although [maybe you shouldn't make your data feel like it's dirty](https://www.jstor.org/stable/10.5749/j.ctvg251hk.26)).
 
 +++
 
+#### Dividing the annotations into song bouts
+
 We want to add states to our model for the beginning and ending of each song bout. 
 To do that with the data we're using here, we need to find the bouts within the annotations somehow, 
 since each annotation file contains entire days of song. 
 
 One way to do this is to set a threshold on the duration of silent intervals, 
 e.g. greater than 500 seconds, and use that threshold to break up annotations into bouts.
 
 Before we do that, let's eyeball the distribution of the silent intervals with empty string labels, 
 to see what kind of threshold might make sense.
 
 We start by converting the annotations to a `pandas.DataFrame` so we can easily munge and tidy the data. This is one advantage of moving from the Praat TextGrid format to the `'generic-seq'` format built into crowsetta.
 
-One approach would be to put all the annotations in a single DataFrame, adding a column named `'bird ID'` that we'd use to split the DataFrame back up below. But we'll stick with a dictionary to hopefully make it easier to follow. Our new dictionary `dfs` will map each bird ID to a `pandas.DataFrame` made from its annotations.
+One approach would be to put all the annotations in a single DataFrame, adding a column named `'bird ID'` that we'd use to split the DataFrame back up below (a sort of ["long form"](https://en.wikipedia.org/wiki/Tidy_data) DataFrame). But we'll stick with a dictionary to hopefully make the loops a bit easier to follow without inspecting the contents of DataFrames. Our new dictionary `dfs` will map each bird ID to a `pandas.DataFrame` made from its annotations.
 
 ```{code-cell} ipython3
 dfs = {
     bird_id: crowsetta.formats.seq.GenericSeq(annots=annot).to_df()
     for bird_id, annot in annots.items()
 }
 ```
```

### Comparing `crowsetta-5.0.0rc2/doc/index.md` & `crowsetta-5.0.1/doc/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 ---
-title: crowsetta
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.13.8
+    jupytext_version: 1.14.5
 kernelspec:
   display_name: Python 3 (ipykernel)
   language: python
   name: python3
-execution:
-  timeout: 120
 ---
 
 ::::{grid}
 :reverse:
 :gutter: 2 1 1 1
 :margin: 4 4 1 1
 
@@ -41,15 +38,15 @@
 for animal vocalizations and bioacoustics data. 
 Files in these formats are created by
 applications that enable users to annotate audio and/or spectrograms. 
 Such annotations typically include the times when sound events start and stop, 
 and labels that assign each sound to some set of classes 
 chosen by the annotator.
 crowsetta has built-in support for many widely used {ref}`formats <formats-index>` 
-such as {ref}`Audacity label tracks <aud-txt>`, 
+such as {ref}`Audacity label tracks <aud-seq>`, 
 {ref}`Praat .TextGrid files <textgrid>`, 
 and {ref}`Raven .txt files <raven>`.
 The images below show examples of the two families of annotation formats 
 built into crowsetta, sequence-like formats and bounding box-like formats.
 
 :::{figure} _static/example-textgrid-for-index.png
 ---
@@ -133,15 +130,15 @@
 
 # Features
 
 With crowsetta, you can:
 * work with your annotations in Python,
   taking advantage of built-in support 
   for many widely used {ref}`formats <formats-index>`
-  such as {ref}`Audacity label tracks <aud-txt>`, 
+  such as {ref}`Audacity label tracks <aud-seq>`, 
   {ref}`Praat .TextGrid files <textgrid>`,
   and {ref}`Raven .txt files <raven>`.
 * work with any format by remembering just one class:  
   `annot = crowsetta.Transcriber(format='format').from_file('annotations.ext')`
   - no need to remember different functions for different formats
   - great for interactive analysis and scripts
 * when needed, use classes that represent the formats 
@@ -152,15 +149,15 @@
 * work with custom annotation formats that are not built in 
   by writing simple classes, leveraging abstractions in crowsetta 
   that can represent a wide array of annotation formats
 
 <h3>Built-in support for many widely-used formats</h3>
 
 crowsetta has built-in support for many widely used {ref}`formats <formats-index>` 
-such as {ref}`Audacity label tracks <aud-txt>`, 
+such as {ref}`Audacity label tracks <aud-seq>`, 
 {ref}`Praat .TextGrid files <textgrid>`, 
 and {ref}`Raven .txt files <raven>`.
 
 Here is an example of loading an example {ref}`Praat .TextGrid <textgrid>` file:
 
 ```{code-cell} ipython3
 :tags: [remove-cell]
@@ -172,16 +169,21 @@
 crowsetta.data.extract_data_files()
 ```
 
 ```{code-cell} ipython3
 import crowsetta
 example = crowsetta.data.get('textgrid')
 a_textgrid = crowsetta.formats.seq.TextGrid.from_file(example.annot_path)
-print(f"`a_textgrid` is a {type(a_textgrid)}")
-print(f"The first five intervals from the interval tier in `a_textgrid`:\n{a_textgrid.textgrid[0][:5]}")
+print(
+    f"`a_textgrid` is a {type(a_textgrid)}"
+)
+print(
+    "The first five intervals from the interval tier in `a_textgrid`:\n"
+    f"{a_textgrid.tiers[1].intervals[:5]}"
+)
 ```
 
 Instead of writing out the class name, 
 each format can also be referred to by a shorthand string name:
 
 ```{code-cell} ipython3
 import crowsetta
```

### Comparing `crowsetta-5.0.0rc2/doc/make.bat` & `crowsetta-5.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/nitpick-ignore.txt` & `crowsetta-5.0.1/doc/nitpick-ignore.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt` & `crowsetta-5.0.1/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/scripts/annot/b06_concat_dtw.TextGrid` & `crowsetta-5.0.1/doc/data/r6paq/b06_concat_dtw.TextGrid`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/scripts/audio/Recording_1_Segment_07-snippet.wav` & `crowsetta-5.0.1/doc/scripts/audio/Recording_1_Segment_07-snippet.wav`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/scripts/audio/b06_concat-snippet.wav` & `crowsetta-5.0.1/doc/scripts/audio/b06_concat-snippet.wav`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/scripts/raven-chronister-et-al-2021.md` & `crowsetta-5.0.1/doc/scripts/raven-chronister-et-al-2021.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/scripts/textgrid-BF-dataset.md` & `crowsetta-5.0.1/doc/scripts/textgrid-BF-dataset.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/doc/tutorial.md` & `crowsetta-5.0.1/doc/tutorial.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ## Getting some example data to work with
 
 Since crowsetta is a tool to working with annotations of
 vocalizations, we need some audio files containing vocalizations that
 are annotated.
 
 We download some examples of annotation files in the 
-{ref}`Audacity LabelTrack format <aud-txt>`, 
+{ref}`Audacity LabelTrack format <aud-seq>`, 
 from the dataset 
 ["Labeled songs of domestic canary M1-2016-spring (Serinus canaria)"](https://zenodo.org/record/6521932)
 by Giraudon et al., 2021.
 
 ```{code-cell} ipython3
 !curl --no-progress-meter -L 'https://zenodo.org/record/6521932/files/M1-2016-spring_audacity_annotations.zip?download=1' -o './data/M1-2016-spring_audacity_annotations.zip'
 ```
@@ -79,15 +79,15 @@
 The `Transcriber` is a Python `class`, and we want to create a new
 instance of that class. You don’t have to understand what that
 means, but you do have to know that before you can do anything with a
 `Transcriber`, you have to call the class, as if it were a function,
 and assign it to some variable, like this:
 
 ```{code-cell} ipython3
-scribe = crowsetta.Transcriber(format='aud-txt')
+scribe = crowsetta.Transcriber(format='aud-seq')
 print("scribe is an instance of a", type(scribe))
 ```
 
 Now we have a `scribe` with methods that we can use on our
 annotation files (methods are functions that “belong” to a class). 
 We use the `from_file` method of the `Transcriber` to load the annotations.
 
@@ -124,15 +124,15 @@
 ```
 
 Depending on the format type, sequence-like 
 or bounding box-lie, 
 the `Annotation` will either have a `seq` attribute, 
 short for "Sequence", or a `bbox` attribute, 
 short for "Bounding box".
-Since `'aud-txt'` is a sequence-like format, 
+Since `'aud-seq'` is a sequence-like format, 
 the `Annotation`s have a `seq` attribute:
 
 ```{code-cell} ipython3
 print(
     f'seq for first Annotation: {annots[0].seq}'
 )
 ```
@@ -171,20 +171,20 @@
 ### Working with `Sequence`s
 
 As we said, 
 what we really want is some data types 
 that make it easier to work with our annotations, 
 and that help us write clean, readable code.
 
-The {ref}`Audacity .txt <aud-txt>` format 
+The {ref}`Audacity .txt <aud-seq>` format 
 we are using in this tutorial above is one of what 
 crowsetta calls a "sequence-like" format, 
 as stated above.
 What this means is that we can convert our 
-each one of our `'aud-txt'` annotations to 
+each one of our `'aud-seq'` annotations to 
 a `Sequence`. 
 Each `Sequence` consists of some number of `Segment`s, i.e., a
 part of the sequence defined by an `onset` and `offset` that has a
 `label` associated with it.
 These `Sequence`s and `Segment`s are what specifically helps  
 us write clean code, as we'll see below.
 (Bounding box-like annotation formats similarly give us generic
```

### Comparing `crowsetta-5.0.0rc2/noxfile.py` & `crowsetta-5.0.1/noxfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import pathlib
 import shutil
+import sys
 
 import nox
 
 DIR = pathlib.Path(__file__).parent.resolve()
 VENV_DIR = pathlib.Path('./.venv').resolve()
 
 
@@ -39,34 +40,44 @@
     """
 
     session.install("virtualenv")
     # VENV_DIR here is a pathlib.Path location of the project virtualenv
     # e.g. .venv
     session.run("virtualenv", os.fsdecode(VENV_DIR), silent=True)
 
-    python = os.fsdecode(VENV_DIR.joinpath("bin/python"))
+    if sys.platform.startswith("linux") or sys.platform == "darwin":
+        python = os.fsdecode(VENV_DIR.joinpath("bin/python"))
+    elif sys.platform.startswith("win"):
+        python = os.fsdecode(VENV_DIR.joinpath("Scripts/python.exe"))
 
     # Use the venv's interpreter to install the project along with
     # all it's dev dependencies, this ensures it's installed in the right way
     session.run(python, "-m", "pip", "install", "-e", ".[dev,test,doc]", external=True)
 
 
-@nox.session
+@nox.session(python="3.10")
 def lint(session):
     """
     Run the linter.
     """
     session.install(".[dev]")
     # run isort first since black disagrees with it
     session.run("isort", "./src")
     session.run("black", "./src", "--line-length=120")
     session.run("flake8", "./src", "--max-line-length", "120", "--exclude", "./src/crowsetta/_vendor")
 
 
-@nox.session
+TEST_PYTHONS = [
+    "3.9",
+    "3.10",
+    "3.11"
+]
+
+
+@nox.session(python=TEST_PYTHONS)
 def test(session) -> None:
     """
     Run the unit and regular tests.
     """
     session.install(".[test]")
     session.run("pytest", "-n", "auto", *session.posargs)
```

### Comparing `crowsetta-5.0.0rc2/pyproject.toml` & `crowsetta-5.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,36 +4,34 @@
 
 [project]
 name = "crowsetta"
 description = "A Python tool to work with any format for annotating animal vocalizations and bioacoustics data"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "appdirs >=1.4.4",
     "attrs >=19.3.0",
     "evfuncs >=0.3.5",
     "birdsong-recognition-dataset >=0.3.2",
-    "importlib-resources >=5.7.1",
-    "numpy >=1.18.1",
+    "numpy >=1.21.0",
     "pandas >= 1.3.5",
     "pandera >= 0.9.0",
-    "scipy >=1.4.1",
-    "SoundFile >=0.10.3",
+    "scipy >=1.7.0",
+    "SoundFile >=0.12.1",
 ]
-version = "5.0.0rc2"
+version = "5.0.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     'License :: OSI Approved :: BSD License',
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: Implementation :: CPython',
 ]
 
 [project.optional-dependencies]
 test = [
@@ -43,15 +41,14 @@
 ]
 doc = [
     "ipython != 8.7.0",
     "jupyterlab >=3.0.3",
     "jupytext >=1.13.8",
     "librosa >=0.9.1",
     "myst-nb >=0.15.0",
-    "osfclient >=0.0.5",
     "pyprojroot >=0.2.0",
     "seaborn >=0.11.2",
     "Sphinx >=3.4.3",
     "sphinx-autobuild >= 2021.3.14",
     "sphinx-book-theme >=0.3.2",
     "sphinx-copybutton >=0.4.0",
     "sphinx-design >=0.2.0",
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/__about__.py` & `crowsetta-5.0.1/src/crowsetta/__about__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     base_dir = None
 
 
 __title__ = "crowsetta"
 __summary__ = "A Python tool to work with any format for annotating animal vocalizations and bioacoustics data"
 __uri__ = "https://github.com/vocalpy/crowsetta"
 
-__version__ = "5.0.0rc2"
+__version__ = "5.0.1"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/__init__.py` & `crowsetta-5.0.1/src/crowsetta/__init__.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/annotation.py` & `crowsetta-5.0.1/src/crowsetta/annotation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """A class to represent annotations for a single file."""
+from __future__ import annotations
+
 from pathlib import Path
-from typing import List, Optional
+import reprlib
+from typing import Optional
 
 import crowsetta
 
 from .bbox import BBox
 from .sequence import Sequence
 from .typing import PathLike
 
@@ -14,35 +17,39 @@
 
     The annotations can be one of two types:
     a single sequence, or a list of bounding boxes.
 
     Attributes
     ----------
     annot_path : str, pathlib.Path
-        path to file from which annotations were loaded
+        Path to file from which annotations were loaded.
     notated_path : str, pathlib.Path
-        path to file that ``annot_path`` annotates.
+        Path to file that ``annot_path`` annotates.
         E.g., an audio file, or an array file
         that contains a spectrogram generated from audio.
         Optional, default is None.
-    seq : crowsetta.Sequence
-        a sequence of annotated segments,
-        each having an onset time, offset time,
+    seq : crowsetta.Sequence, list
+        A :class:`crowsetta.Sequence` instance,
+        or a list of :class:`crowsetta.Sequence` instances.
+        Each :class:`crowsetta.Sequence` instance
+        represents a sequence of annotated segments,
+        with a segment having an onset time, offset time,
         and label.
     bboxes : list
-        of ``crowsetta.BBox``,
-        annotated bounding boxes,
+        List of annotated bounding boxes,
         each having an onset time, offset time,
         lowest frequency, highest frequency,
         and label.
+        Each item in the list will be a
+        :class:`crowsetta.BBox` instance.
 
     Notes
     -----
-    A ``crowsetta.Annotation`` can have a ``seq``
-    or ``bboxes``, but not both.
+    A :class:`crowsetta.Annotation` can have either a ``seq``
+    attribute or a ``bboxes`` attribute, but not both.
 
     Examples
     --------
 
     A toy example of a sequence-like annotation.
 
     >>> import numpy as np
@@ -67,26 +74,31 @@
     BBox(onset=3.0, offset=4.0, low_freq=3250.0, high_freq=12500.0, label='Pinacosaurus grangeri')])
     """
 
     def __init__(
         self,
         annot_path: PathLike,
         notated_path: Optional[PathLike] = None,
-        seq: Optional[Sequence] = None,
-        bboxes: Optional[List[BBox]] = None,
+        seq: Optional[Sequence | list[Sequence]] = None,
+        bboxes: Optional[list[BBox]] = None,
     ):
         if seq is None and bboxes is None:
             raise ValueError("an Annotation must have either a ``seq`` or ``bboxes``")
 
         if seq is not None and bboxes is not None:
             raise ValueError("an Annotation can have either a ``seq``" "or ``bboxes``, but not both.")
 
         if seq:
-            if not isinstance(seq, crowsetta.Sequence):
-                raise TypeError(f"``seq`` should be a ``crowsetta.Sequence`` but was: {type(seq)}")
+            if not (
+                    isinstance(seq, crowsetta.Sequence) or
+                    (isinstance(seq, list) and all([isinstance(seq_, crowsetta.Sequence) for seq_ in seq]))
+            ):
+                raise TypeError(
+                    f"``seq`` should be a crowsetta.Sequence or list of Sequences but was: {type(seq)}"
+                )
             self.seq = seq
 
         if bboxes:
             if not isinstance(bboxes, list):
                 raise ValueError("``bboxes`` should be a list")
             if not all([isinstance(bbox, BBox) for bbox in bboxes]):
                 raise ValueError("``bboxes`` should be a list of ``crowsetta.BBox`` instances")
@@ -97,17 +109,17 @@
             self.notated_path = Path(notated_path)
         else:
             self.notated_path = notated_path
 
     def __repr__(self):
         repr_ = f"Annotation(annot_path={repr(self.annot_path)}, notated_path={repr(self.notated_path)}, "
         if hasattr(self, "seq"):
-            repr_ += f"seq={self.seq})"
+            repr_ += f"seq={reprlib.repr(self.seq)})"
         elif hasattr(self, "bboxes"):
-            repr_ += f"bboxes={self.bboxes})"
+            repr_ += f"bboxes={reprlib.repr(self.bboxes)})"
         return repr_
 
     def __eq__(self, other):
         is_annot_and_audio_eq = self.annot_path == other.annot_path and self.notated_path == other.notated_path
         if hasattr(self, "seq") and hasattr(other, "seq"):
             return is_annot_and_audio_eq and self.seq == other.seq
         elif hasattr(self, "bboxes") and hasattr(other, "bboxes"):
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/bbox.py` & `crowsetta-5.0.1/src/crowsetta/bbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/spinetail.txt` & `crowsetta-5.0.1/src/crowsetta/data/audbbox/spinetail.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt` & `crowsetta-5.0.1/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/Annotation.xml` & `crowsetta-5.0.1/src/crowsetta/data/birdsongrec/Annotation.xml`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/data.py` & `crowsetta-5.0.1/src/crowsetta/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     "birdsong-recognition-dataset": FormatPathArgs(package="crowsetta.data.birdsongrec", resource="Annotation.xml"),
     "generic-seq": FormatPathArgs(package="crowsetta.data.generic", resource="example_custom_format.csv"),
     "notmat": FormatPathArgs(package="crowsetta.data.notmat", resource="gy6or6_baseline_230312_0808.138.cbin.not.mat"),
     "raven": FormatPathArgs(package="crowsetta.data.raven", resource="Recording_1_Segment_02.Table.1.selections.txt"),
     "simple-seq": FormatPathArgs(
         package="crowsetta.data.simple", resource="bl26lb16_190412_0721.20144_annotations.csv"
     ),
-    "textgrid": FormatPathArgs(package="crowsetta.data.textgrid", resource="1179.TextGrid"),
+    "textgrid": FormatPathArgs(package="crowsetta.data.textgrid", resource="AVO-maea-basic.TextGrid"),
     "timit": FormatPathArgs(package="crowsetta.data.timit", resource="sa1.phn"),
 }
 
 
 def extract_data_files(user_data_dir: PathLike | None = None):
     """Extract example annotation files from ``crowsetta.data``
     to a local directory on the file system.
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/generic/example_custom_format.csv` & `crowsetta-5.0.1/src/crowsetta/data/generic/example_custom_format.csv`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat` & `crowsetta-5.0.1/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv` & `crowsetta-5.0.1/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/data/timit/sa1.phn` & `crowsetta-5.0.1/src/crowsetta/data/timit/sa1.phn`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/__init__.py` & `crowsetta-5.0.1/src/crowsetta/formats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,17 @@
         attr = getattr(module, attr_name)
         if inspect.isclass(attr):
             if issubclass(attr, interface.seq.SeqLike) or issubclass(attr, interface.bbox.BBoxLike):
                 # note we use the class-level ``name`` attribute, a string, as keys in the dictionary
                 FORMATS[attr.name] = attr
 
 
+__all__ = ["bbox", "FORMATS", "seq"]
+
+
 def by_name(name: str) -> Type:
     """Get an annotation class by its string name
 
     Parameters
     ----------
     name : str
         Shorthand name for an annotation format, e.g. 'timit'
@@ -59,32 +62,33 @@
     """
     return sorted(FORMATS.keys())
 
 
 def register_format(format_class: Type) -> Type:
     """Decorator to register annotation formats.
 
-    Adds class to ``crowsetta.formats``.
+    Adds class to :mod:`crowsetta.formats`.
     The decorator maps the class variable ``name``,
     a string, to the class itself, so that calling
-    ``crowsetta.formats.by_name`` with that string
+    :func:`crowsetta.formats.by_name` with that string
     will return the class.
 
     Parameters
     ----------
     format_class : class
         A class that has the required class variables
         and adheres to one of the interfaces
-        defined in ``crowsetta.interface``,
-        either ``SeqLike`` or ``BBoxLike``.
+        defined in :mod:`crowsetta.interface`,
+        either :class:`~crowsetta.interface.seq.SeqLike`
+        or :class:`~crowsetta.interface.bbox.BBoxLike`.
 
     Returns
     -------
     format_class : class
         The same class, unchanged.
         This decorator only adds the class
-        to ``crowsetta.formats.FORMATS``.
+        to :data:`crowsetta.formats.FORMATS`.
     """
     if not issubclass(format_class, interface.seq.SeqLike) and not issubclass(format_class, interface.bbox.BBoxLike):
         raise TypeError(f"format class must be subclass of SeqLike or BBoxLike, but was not: {format_class}")
     FORMATS[format_class.name] = format_class
     return format_class
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/audbbox.py` & `crowsetta-5.0.1/src/crowsetta/formats/bbox/audbbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for Audacity label tracks
-in extended format, exported to .txt files
+in extended format, exported to txt files
 https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Extended_format_with_frequency_ranges
 """
 from __future__ import annotations
 
 import pathlib
 from typing import ClassVar, List, Optional
 
@@ -14,33 +14,33 @@
 
 import crowsetta
 from crowsetta.typing import PathLike
 
 
 def txt_to_records(aud_txt_path: PathLike) -> list[dict]:
     """Load a txt file in Audacity extended label track format
-    into records for a `pandas.DataFrame``.
+    into records for a :type:`pandas.DataFrame`.
 
-    Returns a ``list`` of ``dict`` that can be made into a
-    ``DataFrame`` by calling ``pandas.DataFrame.from_records``.
+    Returns a :class:`list` of :class:`dict` that can be made into a
+    :class:`~pandas.DataFrame` by calling :meth:`pandas.DataFrame.from_records`.
 
     Parameters
     ----------
     aud_txt_path : str, pathlib.Path
 
     Returns
     -------
     records : list
-        Of ``dict``, each ``dict`` a row
-        in the ``DataFrame``.
+        Of :class:`dict`, each :class:`dict` will become
+        a row in the :class:`~pandas.DataFrame`.
 
     Notes
     -----
     We work with Audacity txt files this way, instead of
-    loading with ``pandas.read_csv`` then munging, so that we can
+    loading with :func:`pandas.read_csv` then munging, so that we can
     be sure that we can round-trip data without corrupting it.
     """
     with pathlib.Path(aud_txt_path).open("r") as fp:
         lines = fp.read().splitlines()
     lines = [line.split("\t") for line in lines]
 
     records = []
@@ -54,37 +54,38 @@
             "high_freq_hz": float(row2[2]),
         }
         records.append(record)
     return records
 
 
 def df_to_lines(df: pd.DataFrame) -> list[str]:
-    """Convert a pandas DataFrame to a list of strings
-    that can be saved as a txt file in Audacity extended
+    """Convert a :type:`pandas.DataFrame` to a
+    :class:`list` of :class:`str` that can be saved
+    as a txt file in Audacity extended
     label track format.
 
     This function is (roughly) the inverse of
-    ``crowsetta.formats.bbox.audbbox.txt_to_records``.
+    :func:`crowsetta.formats.bbox.audbbox.txt_to_records`.
 
     Parameters
     ----------
     df : pandas.DataFrame
-        With contents of a .txt file in Audacity extended label track format,
-        after being loaded and parsed by ``crowsetta.formats.bbox.audbbox.audbbox_txt_to_df``
+        With contents of a txt file in Audacity extended label track format,
+        after being loaded and parsed by :func:`crowsetta.formats.bbox.audbbox.audbbox_txt_to_df`
 
     Returns
     -------
     lines : list
         List of strings that can be saved to a text file
-        by calling ``writelines``.
+        by calling :func:`writelines`.
 
     Notes
     -----
     We work with Audacity txt files this way, instead of
-    munging and then calling ``pandas.DataFrame.to_csv``,
+    munging and then calling :meth:`pandas.DataFrame.to_csv`,
     so that we can be sure that we can round-trip data
     without corrupting it.
     """
     df = AudBBoxSchema.validate(df)
 
     lines = []
     for record in df.itertuples():
@@ -92,17 +93,18 @@
         row2 = f"\\\t{float(record.low_freq_hz)}\t{float(record.high_freq_hz)}\n"
         lines.extend((row1, row2))
 
     return lines
 
 
 class AudBBoxSchema(pandera.SchemaModel):
-    """A ``pandera.SchemaModel`` that validates ``pandas`` dataframes
+    """A :class:`pandera.SchemaModel` that
+    validates :mod:`pandas` dataframes
     loaded from Audacity label tracks
-    in extended format, exported to .txt files
+    in extended format, exported to txt files
     https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Extended_format_with_frequency_ranges
     """
 
     begin_time_s: Series[float] = pandera.Field(coerce=True)
     end_time_s: Series[float] = pandera.Field(coerce=True)
     label: Series[pd.StringDtype] = pandera.Field(coerce=True)
     low_freq_hz: Series[float] = pandera.Field(coerce=True)
@@ -113,29 +115,29 @@
         strict = True
 
 
 @crowsetta.interface.BBoxLike.register
 @attr.define
 class AudBBox:
     """Class that represents Audacity label tracks
-    in extended format, exported to .txt files
+    in extended format, exported to txt files
     https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Extended_format_with_frequency_ranges
 
     Attributes
     ----------
     name: str
         Shorthand name for annotation format: 'aud-bbox'.
     ext: str
         Extension of files in annotation format: '.txt'
     df : pandas.DataFrame
         with annotations loaded into it
     annot_path : str, pathlib.Path
-        Path to Audacity .txt file from which annotations were loaded.
+        Path to Audacity txt file from which annotations were loaded.
     audio_path : str. pathlib.Path
-        Path to audio file that the Audacity .txt file annotates.
+        Path to audio file that the Audacity txt file annotates.
     """
 
     COLUMNS_MAP: ClassVar[dict] = {
         0: "begin_time_s",
         1: "end_time_s",
         2: "label",
         3: "low_freq_hz",
@@ -147,51 +149,52 @@
 
     df: pd.DataFrame
     annot_path: pathlib.Path
     audio_path: Optional[pathlib.Path] = attr.field(default=None, converter=attr.converters.optional(pathlib.Path))
 
     @classmethod
     def from_file(cls, annot_path: PathLike, audio_path: Optional[PathLike] = None) -> "Self":  # noqa: F821
-        """Load annotations from a Audacity annotation file with bbox,
+        """Load annotations from an Audacity annotation file with bounding boxes,
         created by exporting a Selection Table.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            Path to a .txt file exported from Audacity bbox.
+            Path to a txt file exported from Audacity bbox.
         audio_path : str, pathlib.Path
-            Path to audio file that the Audacity bbox .txt file annotates.
+            Path to audio file that the Audacity bbox txt file annotates.
             Optional, defaults to None.
 
         Examples
         --------
         >>> example = crowsetta.data.get('aud-bbox')
         >>> audbbox = crowsetta.formats.bbox.AudBBox.from_file(example.annot_path)
         """
         annot_path = pathlib.Path(annot_path)
         crowsetta.validation.validate_ext(annot_path, extension=cls.ext)
         records = crowsetta.formats.bbox.audbbox.txt_to_records(annot_path)
         df = pd.DataFrame.from_records(records)
         if len(df) < 1:
-            raise ValueError(f"Cannot load annotations, " f"there are no rows in Audacity .txt file:\n{df}")
+            raise ValueError(f"Cannot load annotations, " f"there are no rows in Audacity txt file:\n{df}")
         df = crowsetta.formats.bbox.audbbox.AudBBoxSchema.validate(df)
 
         return cls(
             df=df,
             annot_path=annot_path,
             audio_path=audio_path,
         )
 
     def to_bbox(self) -> List[crowsetta.BBox]:
-        """Convert this Audacity extended label track annotation to a ``list`` of ``crowsetta.Bbox``.
+        """Convert this Audacity extended label track annotation
+        to a :class:`list` of :class:`crowsetta.Bbox`.
 
         Returns
         -------
         bboxes : list
-            of ``crowsetta.BBox``
+            A :class:`list` of :class:`crowsetta.BBox` instances.
 
         Examples
         --------
         >>> example = crowsetta.data.get('aud-bbox')
         >>> audbbox = crowsetta.formats.bbox.AudBBox.from_file(example.annot_path)
         >>> bboxes = audbbox.to_bbox()
         """
@@ -205,15 +208,16 @@
         ):
             bboxes.append(
                 crowsetta.BBox(onset=begin_time, offset=end_time, low_freq=low_freq, high_freq=high_freq, label=label)
             )
         return bboxes
 
     def to_annot(self) -> crowsetta.Annotation:
-        """Convert this Audacity bbox annotation to a ``crowsetta.Annotation``.
+        """Convert this Audacity bbox annotation
+        to a :class:`crowsetta.Annotation`.
 
         Returns
         -------
         annot : crowsetta.Annotation
 
         Examples
         --------
@@ -221,15 +225,15 @@
         >>> audacitybbox = crowsetta.formats.bbox.AudBBox.from_file(example.annot_path)
         >>> annot = audacitybbox.to_annot()
         """
         bboxes = self.to_bbox()
         return crowsetta.Annotation(annot_path=self.annot_path, notated_path=self.audio_path, bboxes=bboxes)
 
     def to_file(self, annot_path: PathLike) -> None:
-        """Make a .txt file from this annotation
+        """Make a txt file from this annotation
         in extended label track format that can be read by Audacity.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
              Path including filename where file should be saved.
              Must have extension '.txt'
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/raven.py` & `crowsetta-5.0.1/src/crowsetta/formats/bbox/raven.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from pandera.typing import Series
 
 import crowsetta
 from crowsetta.typing import PathLike
 
 
 class RavenSchema(pandera.SchemaModel):
-    """A ``pandera.SchemaModel`` that validates ``pandas`` dataframes
-    loaded from a .txt file, created by exporting a Selection Table
+    """A :class:`pandera.SchemaModel` that validates :type:`pandas.DataFrame`s
+    loaded from a txt file, created by exporting a Selection Table
     from Raven.
     """
 
     begin_time_s: Series[float] = pandera.Field()
     end_time_s: Series[float] = pandera.Field()
     low_freq_hz: Series[float] = pandera.Field()
     high_freq_hz: Series[float] = pandera.Field()
@@ -36,30 +36,30 @@
         # and we don't want to throw an error because of it
         strict = False
 
 
 @crowsetta.interface.BBoxLike.register
 @attr.define
 class Raven:
-    """Class that represents .txt annotation files
+    """Class that represents txt annotation files
     from Raven (https://ravensoundsoftware.com/software/),
     created by exporting a Selection Table.
 
     Attributes
     ----------
     name: str
         Shorthand name for annotation format: 'raven'.
     ext: str
         Extension of files in annotation format: '.txt'
     df : pandas.DataFrame
         with annotations loaded into it
     annot_path : str, pathlib.Path
-        Path to Raven .txt file from which annotations were loaded.
+        Path to Raven txt file from which annotations were loaded.
     audio_path : str. pathlib.Path
-        Path to audio file that the Raven .txt file annotates.
+        Path to audio file that the Raven txt file annotates.
     """
 
     name: ClassVar[str] = "raven"
     ext: ClassVar[str] = (".txt",)
     COLUMNS_MAP: ClassVar[dict] = {
         "Begin Time (s)": "begin_time_s",
         "End Time (s)": "end_time_s",
@@ -78,52 +78,53 @@
     ) -> "Self":  # noqa: F821
         """Load annotations from a Raven annotation file,
         created by exporting a Selection Table.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            Path to a .txt file exported from Raven.
+            Path to a txt file exported from Raven.
         annot_col : str
-            name of column that contains annotations
+            Name of column that contains annotations.
         audio_path : str, pathlib.Path
-            Path to audio file that the Raven .txt file annotates.
+            Path to audio file that the Raven txt file annotates.
             Optional, defaults to None.
 
         Examples
         --------
         >>> example = crowsetta.data.get('raven')
         >>> raven = crowsetta.formats.bbox.Raven.from_file(example.annot_path)
         """
         annot_path = pathlib.Path(annot_path)
         crowsetta.validation.validate_ext(annot_path, extension=cls.ext)
 
         #  assume file is space-separated with no header
         df = pd.read_csv(annot_path, sep="\t")
         if len(df) < 1:
-            raise ValueError(f"Cannot load annotations, " f"there are no rows in Raven .txt file:\n{df}")
+            raise ValueError(f"Cannot load annotations, " f"there are no rows in Raven txt file:\n{df}")
         columns_map = dict(cls.COLUMNS_MAP)  # copy
         columns_map.update({annot_col: "annotation"})
         df.rename(columns=columns_map, inplace=True)
         df = RavenSchema.validate(df)
 
         return cls(
             df=df,
             annot_path=annot_path,
             annot_col=annot_col,
             audio_path=audio_path,
         )
 
     def to_bbox(self) -> List[crowsetta.BBox]:
-        """Convert this Raven annotation to a ``list`` of ``crowsetta.Bbox``.
+        """Convert this Raven annotation to a
+        :class:`list` of :class:`crowsetta.Bbox` instances.
 
         Returns
         -------
         bboxes : list
-            of ``crowsetta.BBox``
+            A :class:`list` of :class:`crowsetta.BBox` instances.
 
         Examples
         --------
         >>> example = crowsetta.data.get('raven')
         >>> raven = crowsetta.formats.bbox.Raven.from_file(example.annot_path)
         >>> bboxes = raven.to_bbox()
         """
@@ -137,15 +138,16 @@
         ):
             bboxes.append(
                 crowsetta.BBox(onset=begin_time, offset=end_time, low_freq=low_freq, high_freq=high_freq, label=label)
             )
         return bboxes
 
     def to_annot(self) -> crowsetta.Annotation:
-        """Convert this Raven annotation to a ``crowsetta.Annotation``.
+        """Convert this Raven annotation to a
+        :class:`crowsetta.Annotation`.
 
         Returns
         -------
         annot : crowsetta.Annotation
 
         Examples
         --------
@@ -153,21 +155,21 @@
         >>> raven = crowsetta.formats.bbox.Raven.from_file(example.annot_path)
         >>> annot = raven.to_annot()
         """
         bboxes = self.to_bbox()
         return crowsetta.Annotation(annot_path=self.annot_path, notated_path=self.audio_path, bboxes=bboxes)
 
     def to_file(self, annot_path: PathLike) -> None:
-        """make a .txt file that can be read by Raven
+        """Make a txt file that can be read by Raven
         from this annotation
 
         Parameters
         ----------
         annot_path : str, pahtlib.Path
-             path including filename where file should be saved.
+             Path including filename where file should be saved.
              Must have extension '.txt'
         """
         crowsetta.validation.validate_ext(annot_path, extension=self.ext)
 
         columns_map = {v: k for k, v in self.COLUMNS_MAP.items()}  # copy
         columns_map.update({"annotation": self.annot_col})
         df_out = self.df.rename(columns=columns_map)
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/audseq.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/audseq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """module for Audacity LabelTrack
-in standard/default format exported to .txt files
+in standard/default format exported to txt files
 https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Standard_.28default.29_format
 """
 import pathlib
 from typing import ClassVar, Optional
 
 import attr
 import numpy as np
@@ -12,17 +12,20 @@
 from pandera.typing import Series
 
 import crowsetta
 from crowsetta.typing import PathLike
 
 
 class AudSeqSchema(pandera.SchemaModel):
-    """A ``pandera.SchemaModel`` that validates ``pandas`` dataframes
+    """A :class:`pandera.SchemaModel`
+    that validates :type:`pandas.DataFrame`s
     loaded from Audacity Labeltrack annotations
-    exported to .txt files in the standard format
+    exported to txt files in the standard format.
+
+    The standard format is described here:
     https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Standard_.28default.29_format
     """
 
     start_time: Optional[Series[float]] = pandera.Field()
     end_time: Optional[Series[float]] = pandera.Field()
     label: Series[pd.StringDtype] = pandera.Field(coerce=True)
 
@@ -32,45 +35,47 @@
 
 
 @crowsetta.interface.SeqLike.register
 @attr.define
 class AudSeq:
     """Class meant to represent
     Audacity Labeltrack annotations
-    exported to .txt files in the standard format
-    https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Standard_.28default.29_format
+    exported to txt files in the standard format[1]_.
 
-    The .txt file will have 3 tab-separated columns
+    The txt file will have 3 tab-separated columns
     that represent the start time, end time, and labels
     of annotated regions.
 
     Attributes
     ----------
     name: str
         Shorthand name for annotation format: ``'aud-seq'``.
     ext: str
-        Extension of files in annotation format:
-        ``'.txt'``
+        Extension of files in annotation format, ``'.txt'``.
     start_times : numpy.ndarray
         Vector of integer sample numbers corresponding
-        to beginning of segments, i.e. onsets
+        to beginning of segments, i.e. onsets.
     end_times : numpy.ndarray
         Vector of integer sample numbers corresponding
-        to ends of segments, i.e. offsets
+        to ends of segments, i.e. offsets.
     labels : numpy.ndarray
         Vector of string labels for segments;
         each element is either a single word,
         or a single phonetic transcription code.
     annot_path : str, pathlib.Path
         Path to file from which annotations were loaded.
-    notated_path : str. pathlib.Path
-        path to file that ``annot_path`` annotates.
+    notated_path : str, pathlib.Path
+        Path to file that ``annot_path`` annotates.
         E.g., an audio file, or an array file
         that contains a spectrogram generated from audio.
         Optional, default is None.
+
+    References
+    ----------
+    .. [1^] https://manual.audacityteam.org/man/importing_and_exporting_labels.html#Standard_.28default.29_format
     """
 
     name: ClassVar[str] = "aud-seq"
     ext: ClassVar[str] = ".txt"
 
     start_times: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
     end_times: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
@@ -80,23 +85,23 @@
 
     @classmethod
     def from_file(
         cls,
         annot_path: PathLike,
         notated_path: Optional[PathLike] = None,
     ) -> "Self":  # noqa: F821
-        """Load annotations from a file
+        """Load annotations from a file.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
             Path to an annotation file,
             with '.txt' extension.
         notated_path : str, pathlib.Path
-            path to file that ``annot_path`` annotates.
+            Path to file that ``annot_path`` annotates.
             E.g., an audio file, or an array file
             that contains a spectrogram generated from audio.
             Optional, default is None.
 
         Examples
         --------
         >>> example = crowsetta.data.get('aud-seq')
@@ -113,20 +118,20 @@
             end_times=df["end_time"].values,
             labels=df["label"].values,
             annot_path=annot_path,
             notated_path=notated_path,
         )
 
     def to_seq(self, round_times: bool = True, decimals: int = 3) -> crowsetta.Sequence:
-        """Convert this annotation to a ``crowsetta.Sequence``.
+        """Convert this annotation to a :class:`crowsetta.Sequence`.
 
         Parameters
         ----------
         round_times : bool
-            If True, round onsets_s and offsets_s.
+            If True, round ``onsets_s`` and ``offsets_s``.
             Default is True.
         decimals : int
             Number of decimals places to round floating point numbers to.
             Only meaningful if round_times is True.
             Default is 3, so that times are rounded to milliseconds.
 
         Returns
@@ -154,15 +159,15 @@
             onsets_s = self.start_times
             offsets_s = self.end_times
 
         seq = crowsetta.Sequence.from_keyword(labels=self.labels, onsets_s=onsets_s, offsets_s=offsets_s)
         return seq
 
     def to_annot(self, round_times: bool = True, decimals: int = 3) -> crowsetta.Annotation:
-        """Convert this annotation to a ``crowsetta.Annotation``.
+        """Convert this annotation to a :class:`crowsetta.Annotation`.
 
         Parameters
         ----------
         round_times : bool
             If True, round onsets_s and offsets_s.
             Default is True.
         decimals : int
@@ -188,26 +193,26 @@
         and then sending them to a csv file,
         the result should be the same on Windows and Linux.
         """
         seq = self.to_seq(round_times, decimals)
         return crowsetta.Annotation(annot_path=self.annot_path, notated_path=self.notated_path, seq=seq)
 
     def to_file(self, annot_path: PathLike) -> None:
-        """save this 'aud-seq' annotation to a .txt file
-        in the standard/default Audacity LabelTrack format
+        """Save this 'aud-seq' annotation to a txt file
+        in the standard/default Audacity LabelTrack format.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            Path with filename of .csv file that should be saved.
+            Path with filename of txt file that should be saved.
         """
         df = pd.DataFrame.from_records(
             {"start_time": self.start_times, "end_time": self.end_times, "label": self.labels}
         )
         df = df[["start_time", "end_time", "label"]]  # put in correct order
         try:
             df = AudSeqSchema.validate(df)
         except pandera.errors.SchemaError as e:
             raise ValueError(
-                f"Annotations produced an invalid dataframe, " f"cannot convert to Audacity LabelTrack .txt file:\n{df}"
+                f"Annotations produced an invalid dataframe, " f"cannot convert to Audacity LabelTrack txt file:\n{df}"
             ) from e
         df.to_csv(annot_path, sep="\t", header=False, index=False)
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/birdsongrec.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/birdsongrec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""module with functions that handle the following dataset:
+"""Module with functions that handle the following dataset:
 Koumura, T. (2016). BirdsongRecognition (Version 1). figshare.
 https://doi.org/10.6084/m9.figshare.3470165.v1
 https://figshare.com/articles/BirdsongRecognition/3470165
 
 as used in this paper:
 Koumura T, Okanoya K (2016) Automatic Recognition of Element Classes and
 Boundaries in the Birdsong with Variable Sequences. PLoS ONE 11(7): e0159188.
@@ -31,15 +31,15 @@
     Attributes
     ----------
     name: str
         Shorthand name for annotation format: ``'birdsong-recognition-dataset'``.
     ext: str
         Extension of files in annotation format: ``'.xml'``.
     sequences: list
-        List of ``birdsongrec.Sequence`` instances.
+        List of :class:`birdsongrec.Sequence` instances.
     annot_path: pathlib.Path
         Path to file from which annotations were loaded.
         Typically with filename 'Annotation.xml'.
     wav_path: pathlib.Path
         Path to directory containing .wav files annotated by the .xml file.
         If not specified, defaults to directory "Wave", relative to the parent
         of ``xml_path``. E.g., if ``xml_path`` is 'Bird0/Annotation.xml'
@@ -66,22 +66,24 @@
     https://github.com/NickleDave/birdsong-recognition-dataset
     That package creates Python objects from .xml files that obey
     this XML schema document:
     https://github.com/NickleDave/birdsong-recognition-dataset/blob/main/doc/xsd/AnnotationSchema.xsd
 
     References
     ----------
-    [1] Koumura, T. (2016). BirdsongRecognition (Version 1). figshare.
-    https://doi.org/10.6084/m9.figshare.3470165.v1
-    https://figshare.com/articles/BirdsongRecognition/3470165
-
-    [2] Koumura T., Okanoya K. (2016) Automatic Recognition of Element Classes and
-    Boundaries in the Birdsong with Variable Sequences. PLoS ONE 11(7): e0159188.
-    https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0159188
-    doi:10.1371/journal.pone.0159188
+
+    .. [1] Koumura, T. (2016). BirdsongRecognition (Version 1). figshare.
+       https://doi.org/10.6084/m9.figshare.3470165.v1
+       https://figshare.com/articles/BirdsongRecognition/3470165
+
+
+    .. [2] Koumura T., Okanoya K. (2016) Automatic Recognition of Element Classes and
+       Boundaries in the Birdsong with Variable Sequences. PLoS ONE 11(7): e0159188.
+       https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0159188
+       doi:10.1371/journal.pone.0159188
     """
 
     name: ClassVar[str] = "birdsong-recognition-dataset"
     ext: ClassVar[str] = ".xml"
 
     sequences: List[birdsongrec.Sequence]
     annot_path: pathlib.Path = attr.field(converter=pathlib.Path)
@@ -92,39 +94,43 @@
         cls, annot_path: PathLike, wav_path: Optional[PathLike] = None, concat_seqs_into_songs: bool = True
     ) -> "Self":  # noqa: F821
         """Load BirdsongRecognition annotations from an .xml file.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            Path to .xml file from BirdsongRecognition dataset
+            Path to xml file from BirdsongRecognition dataset
             that contains annotations.
         wav_path : str, pathlib.Path
-            Path in which .wav files listed in Annotation.xml file are found.
-            Defaults to a directory `Wave` that is located in the parent directory of
+            Path in which wav files listed in Annotation.xml file are found.
+            Defaults to a directory ``Wave`` that is located in the parent directory of
             the Annotation.xml file, which matches the structure of the dataset from [1]_.
 
             .. code-block:: console
 
                 ├── Bird0
                 │   ├── Annotation.xml
                 │   └── Wave
                 │       ├── 0.wav
                 │       ├── 100.wav
                 │       ├── 101.wav
                 ...
 
         concat_seqs_into_songs : bool
-            If True, concatenate sequences from xml_file, so that
+            If True, concatenate sequences from ``annot_path``, so that
             one sequence = one song / .wav file. Default is True.
 
         Examples
         --------
         >>> example = crowsetta.data.get('birdsong-recognition-dataset')
         >>> birdsongrec = crowsetta.formats.seq.BirdsongRec.from_file(example.annot_path)
+
+        .. [1] Koumura, T. (2016). BirdsongRecognition (Version 1). figshare.
+           https://doi.org/10.6084/m9.figshare.3470165.v1
+           https://figshare.com/articles/BirdsongRecognition/3470165
         """
         annot_path = pathlib.Path(annot_path)
         crowsetta.validation.validate_ext(annot_path, extension=cls.ext)
         if not annot_path.exists():
             raise FileNotFoundError(f"annot_path not found: {annot_path}")
 
         if wav_path is None:
@@ -137,15 +143,15 @@
         birdsongrec_seqs = birdsongrec.parse_xml(annot_path, concat_seqs_into_songs=concat_seqs_into_songs)
         return cls(sequences=birdsongrec_seqs, annot_path=annot_path, wav_path=wav_path)
 
     def to_seq(
         self, round_times: bool = True, decimals: int = 3, samplerate: Optional[int] = None
     ) -> List[crowsetta.Sequence]:
         """Convert this set of ``'birdsong-recognition-dataset'``
-        annotations to a list of ``crowsetta.Sequence`` instances.
+        annotations to a list of :class:`crowsetta.Sequence` instances.
 
         Parameters
         ----------
         round_times : bool
             If True, round times of onsets and offsets.
             Default is True.
         decimals : int
@@ -156,20 +162,20 @@
             Sampling rate for wave files. Used to convert
             ``position`` and ``length`` attributes of
             ``birdsongrec.Syllable`` from sample number
             to seconds. Default is None, in which ths function
             tries to open each .wav file and determine
             the actual sampling rate. If this does not work,
             then the ``onsets_s`` and ``offsets_s`` attributes
-            of the ``crowsetta.Sequence`` are left as None.
+            of the :class:`crowsetta.Sequence` are left as None.
 
         Returns
         -------
         seqs : list
-            List of ``crowsetta.Sequence``s.
+            A :class:`list` of :class:`crowsetta.Sequence` instances.
 
         Examples
         --------
         >>> example = crowsetta.data.get('birdsong-recognition-dataset')
         >>> birdsongrec = crowsetta.formats.seq.BirdsongRec.from_file(example.annot_path)
         >>> seqs = birdsongrec.to_seq()
 
@@ -238,15 +244,15 @@
             seqs.append(seq)
         return seqs
 
     def to_annot(
         self, round_times: bool = True, decimals: int = 3, samplerate: Optional[int] = None
     ) -> List[crowsetta.Annotation]:
         """Convert this set of ``'birdsong-recognition-dataset'``
-        annotations to a list of ``crowsetta.Annotation`` instances
+        annotations to a :class:`list` of :class:`crowsetta.Annotation` instances.
 
         Parameters
         ----------
         round_times : bool
             If True, round times of onsets and offsets.
             Default is True.
         decimals : int
@@ -257,20 +263,20 @@
             Sampling rate for wave files. Used to convert
             ``position`` and ``length`` attributes of
             ``birdsongrec.Syllable`` from sample number
             to seconds. Default is None, in which ths function
             tries to open each .wav file and determine
             the actual sampling rate. If this does not work,
             then the ``onsets_s`` and ``offsets_s`` attributes
-            of the ``crowsetta.Sequence`` are left as None.
+            of the :class:`crowsetta.Sequence` are left as None.
 
         Returns
         -------
         annots : list
-            Of ``crowsetta.Annotation``.
+            A list of :class:`crowsetta.Annotation` instances.
 
         Examples
         --------
         >>> example = crowsetta.data.get('birdsong-recognition-dataset')
         >>> birdsongrec = crowsetta.formats.seq.BirdsongRec.from_file(example.annot_path)
         >>> annots = birdsongrec.to_annot()
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/generic.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
-generic format,
+Generic sequence format,
 meant to be an abstraction of
 any sequence-like format.
 
-Consists of ``Annotation``s,
-each with a ``Sequence`` made up
-of ``Segment``s.
+Consists of :class:`crowsetta.Annotation`
+instances, each with a :class:`crowsetta.Sequence`
+made up of :class:`crowsetta.Segment`s.
 
 Functions in this module
-load the format from a .csv,
-or write a .csv in the generic format.
-Other formats that convert to ``Annotation``s
-with ``Sequence``s can be converted
+load the format from a csv file,
+or write a csv file in the generic format.
+Other formats that convert to
+:class:`~crowsetta.Annotation`s
+with :class:`~crowsetta.Sequence`s can be converted
 to this format.
 """
 import os
 from collections import OrderedDict
 from typing import ClassVar, List, Optional, Union
 
 import attr
@@ -31,27 +32,28 @@
 seconds (float), or sample number (integer). All rows must be non-null for either
 'onset_s' and 'offset_s' or 'onset_sample' and 'offset_sample'.
 Both units can also be specified. Conversion between units is not validated.
 """
 
 
 class GenericSeqSchema(pandera.SchemaModel):
-    """``pandera.SchemaModel`` that validates ``pandas`` dataframes
-    loaded from a .csv file  in the ``'generic-seq'`` annotation
+    """A :class: `pandera.SchemaModel` that validates
+    :type:`pandas.DataFrame`s
+    loaded from a csv file  in the ``'generic-seq'`` annotation
     format.
     """
 
     label: Series[pd.StringDtype] = pandera.Field(coerce=True)
     onset_s: Optional[Series[float]] = pandera.Field()
     offset_s: Optional[Series[float]] = pandera.Field()
     onset_sample: Optional[Series[int]] = pandera.Field()
     offset_sample: Optional[Series[int]] = pandera.Field()
 
-    notated_path: Series[str] = pandera.Field()
-    annot_path: Series[str] = pandera.Field()
+    notated_path: Series[str] = pandera.Field(coerce=True)
+    annot_path: Series[str] = pandera.Field(coerce=True)
     sequence: Series[int] = pandera.Field()
     annotation: Series[int] = pandera.Field()
 
     @pandera.dataframe_check(error=ONSET_OFFSET_COLS_ERR)
     def both_onset_s_and_offset_s_if_either(cls, df: pd.DataFrame) -> bool:
         """check that, if one of {'onset_s', 'offset_s'} column is present,
         then both are present"""
@@ -85,37 +87,37 @@
         ordered = True
         strict = True
 
 
 def annot2df(
     annot: Union[crowsetta.Annotation, List[crowsetta.Annotation]], abspath: bool = False, basename: bool = False
 ) -> pd.DataFrame:
-    """Convert sequence-like ``crowsetta.Annotation``
-    to a ``pandas.DataFrame`` in the ``'generic-seq'`` format.
+    """Convert sequence-like :class:`crowsetta.Annotation`
+    to a :type:`pandas.DataFrame` in the ``'generic-seq'`` format.
 
     Parameters
     ----------
     annot : crowsetta.Annotation, or list of Annotations
     csv_path : str, pathlib.Path
-        Path including filename of .csv to write to,
+        Path including filename of csv file to write to,
         will be created (or overwritten if it exists already)
     abspath : bool
-        if True, converts filename for each audio file into absolute path.
+        If True, converts filename for each audio file into absolute path.
         Default is False.
     basename : bool
-        if True, discard any information about path and just use file name.
+        If True, discard any information about path and just use file name.
         Default is False.
 
     Notes
     -----
     The abspath and basename parameters specify how file names for audio files are saved.
     These options are useful when working with multiple copies of files, and for
     reproducibility (so you know which copy of a file you were working with).
     Default for both is False, in which case the filename is saved just as it is passed to
-    this function in a Sequence object.
+    this function in a :class:`crowsetta.Sequence` object.
     """
     if not (isinstance(annot, crowsetta.Annotation) or isinstance(annot, list)):
         raise TypeError("annot must be Annotation or list of Annotations, " f"not type {type(annot)})")
 
     if isinstance(annot, crowsetta.Annotation):
         # put in a list so we can iterate over it
         annot = [annot]
@@ -128,15 +130,18 @@
             "abspath and basename arguments cannot both be set to True, "
             "unclear whether absolute path should be saved or if no path "
             "information (just base filename) should be saved."
         )
 
     records = []
     for annot_num, annot_ in enumerate(annot):
-        seq_list = [annot_.seq]
+        if isinstance(annot_.seq, crowsetta.Sequence):
+            seq_list = [annot_.seq]
+        elif isinstance(annot_.seq, list):
+            seq_list = annot_.seq
         for seq_num, seq in enumerate(seq_list):
             for segment in seq.segments:
                 row = OrderedDict(
                     {
                         key: val
                         for key, val in segment.asdict().items()
                         # don't keep onset or offset if they are None
@@ -173,28 +178,28 @@
 
 def annot2csv(
     annot: Union[crowsetta.Annotation, List[crowsetta.Annotation]],
     csv_path: PathLike,
     abspath: bool = False,
     basename: bool = False,
 ) -> None:
-    """write sequence-like ``crowsetta.Annotation``
-    to a .csv file in the ``'generic-seq'`` format
+    """Write sequence-like :class:`crowsetta.Annotation`
+    to a csv file in the ``'generic-seq'`` format
 
     Parameters
     ----------
     annot : crowsetta.Annotation, or list of Annotations
     csv_path : str, pathlib.Path
-        path including filename of .csv to write to,
+        Path including filename of csv file to write to,
         will be created (or overwritten if it exists already)
     abspath : bool
-        if True, converts filename for each audio file into absolute path.
+        If True, converts filename for each audio file into absolute path.
         Default is False.
     basename : bool
-        if True, discard any information about path and just use file name.
+        If True, discard any information about path and just use file name.
         Default is False.
 
     Notes
     -----
     The abspath and basename parameters specify how file names for audio files are saved.
     These options are useful when working with multiple copies of files, and for
     reproducibility (so you know which copy of a file you were working with).
@@ -202,30 +207,31 @@
     this function in a Sequence object.
     """
     df = annot2df(annot, abspath, basename)
     df.to_csv(csv_path, index=False)
 
 
 def csv2annot(csv_path: PathLike) -> List[crowsetta.Annotation]:
-    """loads a comma-separated values (csv) file containing annotations
-    for song files, returns contents as a list of Annotation objects
+    """Loads a comma-separated values (csv) file containing annotations
+    for song files, returns contents as a
+    :class:`list` of :class:`crowsetta.Annotation` instances.
 
     Parameters
     ----------
     csv_path : str, pathlib.Path
-        Path to .csv file containing annotations
+        Path to csv file containing annotations
         saved in the ``'generic-seq'`` format.
 
     Returns
     -------
     annot_list : list
-        list of Annotations
+        A :class:`list` of :class:`crowsetta.Annotation` instances.
     """
     df = pd.read_csv(csv_path)
-    GenericSeqSchema.validate(df)
+    df = GenericSeqSchema.validate(df)
 
     annot_list = []
     # tried doing this various ways with `pandas.DataFrame.groupby('annotation')`
     # but they are all less readable +
     # required more work to convert -> `crowsetta.Annotation` instances
     for annotation_ind in df.annotation.unique():
         df_annot = df[df.annotation == annotation_ind]
@@ -274,108 +280,106 @@
 
     return annot_list
 
 
 @crowsetta.interface.SeqLike.register
 @attr.define
 class GenericSeq:
-    """
-    class that represents annotations from a generic format,
+    """Class that represents annotations from a generic format,
     meant to be an abstraction of
     any sequence-like format.
 
-    Consists of ``Annotation``s,
-    each with a ``Sequence`` made up
-    of ``Segment``s.
+    Consists of :class:`crowsetta.Annotation`s,
+    each with a :class:`crowsetta.Sequence` made up
+    of :class:`crowsetta.Segment`s.
 
-    Other formats that convert to ``Annotation``s
-    with ``Sequence``s can be converted
+    Other formats that convert to :class:`~crowsetta.Annotation`s
+    with :class:`~crowsetta.Sequence`s can be converted
     to this format.
 
     Attributes
     ----------
     name: str
-        shorthand name for annotation format: ``'generic-seq'``
+        Shorthand name for annotation format: ``'generic-seq'``
     ext: str
-        extension of files in annotation format: ``'.csv'``
+        Extension of files in annotation format: ``'.csv'``
     annots : list
-        of ``crowsetta.Annotation`` instances
+        A :class:`list` of :class:`crowsetta.Annotation` instances.
     """
 
     name: ClassVar[str] = "generic-seq"
     ext: ClassVar[str] = ".csv"
 
     annots: List[crowsetta.Annotation]
 
     @classmethod
     def from_file(cls, annot_path: PathLike) -> "Self":  # noqa: F821
-        """load annotations in 'generic-seq' format from a .csv file
+        """Load annotations in 'generic-seq' format from a csv file.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            Path to .csv file containing annotations
+            Path to csv file containing annotations
             saved in the ``'generic-seq'`` format.
 
         Examples
         --------
         >>> example = crowsetta.data.get('generic-seq')
         >>> generic = crowsetta.formats.seq.GenericSeq.from_file(example.annot_path)"""
         annots = csv2annot(csv_path=annot_path)
         return cls(annots=annots)
 
     def to_seq(self) -> List[crowsetta.Sequence]:
-        """return a list of ``crowsetta.Sequence``,
-        one for every annotation
+        """Return a :class:`list` of :class:`crowsetta.Sequence` instances,
+        one for every annotation.
 
         Examples
         --------
         >>> example = crowsetta.data.get('generic-seq')
         >>> generic = crowsetta.formats.seq.GenericSeq.from_file(example.annot_path)
         >>> seqs = generic.to_seq()
         """
         return [annot.seq for annot in self.annots]
 
     def to_annot(self) -> List[crowsetta.Annotation]:
-        """returns these ``crowsetta.Annotation`` instances
-        as a list
+        """Returns this set of :class:`crowsetta.Annotation` instances
+        as a :class:`list`.
 
-        This is the same as accessing the list of ``Annotation``
-        instances directly. It is implemented so that this class
-        conforms with the ``SeqLike`` interface.
+        This is the same as accessing the :class:`list` of :class:`crowsetta.Annotation`
+        instances directly. The method is implemented so that this class
+        conforms with the :class:`crowsetta.interface.seq.SeqLike` interface.
 
         Examples
         --------
         >>> example = crowsetta.data.get('generic-seq')
         >>> generic = crowsetta.formats.seq.GenericSeq.from_file(example.annot_path)
         >>> annots = generic.to_annot()
         """
         return self.annots
 
     def to_df(self, abspath: bool = False, basename: bool = False) -> pd.DataFrame:
-        """Convert these annotations to a
-        ``pandas.DataFrame``
+        """Convert these annotations to a :type:`pandas.DataFrame`.
 
         abspath : bool
             If True, converts filename for each audio file into absolute path.
             Default is False.
         basename : bool
             If True, discard any information about path and just use file name.
             Default is False.
         """
         return annot2df(self.annots, abspath, basename)
 
     def to_file(self, annot_path: PathLike, abspath: bool = False, basename: bool = False) -> None:
-        """Write these annotations to a .csv file
+        """Write these annotations to a csv file
         in ``'generic-seq'`` format.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            Path including filename of .csv to write to,
+            Path including filename of csv file to write to,
             will be created (or overwritten if it exists already)
         abspath : bool
             If True, converts filename for each audio file into absolute path.
             Default is False.
         basename : bool
             If True, discard any information about path and just use file name.
             Default is False.
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/notmat.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/notmat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""module with functions that handle .not.mat annotation files
-produced by evsonganaly GUI
+"""Module with functions that handle .not.mat annotation files
+produced by evsonganaly GUI.
 """
 import pathlib
 from typing import ClassVar, Dict, Optional
 
 import attr
 import evfuncs
 import numpy as np
@@ -77,15 +77,15 @@
         offsets = notmat_dict["offsets"] / 1000
         labels = np.asarray(list(notmat_dict["labels"]))
 
         audio_path = annot_path.parent / annot_path.name.replace(".not.mat", "")
         return cls(annot_path=annot_path, onsets=onsets, offsets=offsets, labels=labels, audio_path=audio_path)
 
     def to_seq(self, round_times: bool = True, decimals: int = 3) -> crowsetta.Sequence:
-        """Convert this .not.mat annotation to a ``crowsetta.Sequence``.
+        """Convert this .not.mat annotation to a :class:`crowsetta.Sequence`.
 
         Parameters
         ----------
         round_times : bool
             If True, round times of onsets and offsets.
             Default is True.
         decimals : int
@@ -118,15 +118,15 @@
             onsets = self.onsets
             offsets = self.offsets
 
         seq = crowsetta.Sequence.from_keyword(labels=self.labels, onsets_s=onsets, offsets_s=offsets)
         return seq
 
     def to_annot(self, round_times: bool = True, decimals: int = 3) -> crowsetta.Annotation:
-        """Convert this .not.mat annotation to a ``crowsetta.Annotation``.
+        """Convert this .not.mat annotation to a :class:`crowsetta.Annotation`.
 
         Parameters
         ----------
         round_times : bool
             If True, round times of onsets and offsets.
             Default is True.
         decimals : int
@@ -171,19 +171,22 @@
         (MATLAB GUI for annotating vocalizations).
 
         Parameters
         ----------
         samp_freq : int
             Sampling frequency of audio file.
         threshold : int
-            Value above which amplitude is considered part of a segment. default is 5000.
+            Value above which amplitude is considered part of a segment.
+            Default is 5000.
         min_syl_dur : float
-            Minimum duration of a segment. default is 0.02, i.e. 20 ms.
+            Minimum duration of a segment.
+            Default is 0.02, i.e. 20 ms.
         min_silent_dur : float
-            Minimum duration of silent gap between segment. default is 0.002, i.e. 2 ms.
+            Minimum duration of silent gap between segment.
+            Default is 0.002, i.e. 2 ms.
         fname : str, pathlib.Path
             Name of audio file associated with .not.mat,
             will be used as base of name for .not.mat file.
             e.g., if filename is
             'bl26lb16\041912\bl26lb16_190412_0721.20144.cbin'
             then the .not.mat file will be
             'bl26lb16\041912\bl26lb16_190412_0721.20144.cbin.not.mat'
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/simple.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""module with functions meant to handle
+"""Module with functions meant to handle
 any simple sequence-like annotation format.
 
-Can be a .csv or .txt file,
-should have 3 columns that represent
+The annotations can be a csv or txt file;
+the format should have 3 columns that represent
 the onset and offset times in seconds
 and the labels of the segments
 in the annotated sequences.
 
 The default is to assume
 a comma-separated values file
 with a header 'onset_s, offset_s, label',
@@ -27,18 +27,19 @@
 from pandera.typing import Series
 
 import crowsetta
 from crowsetta.typing import PathLike
 
 
 class SimpleSeqSchema(pandera.SchemaModel):
-    """A ``pandera.SchemaModel`` that validates ``pandas`` dataframes
-    loaded from a .csv or .txt file in a 'simple-seq' format.
+    """A :class:`pandera.SchemaModel`
+    that validates :type:`pandas.DataFrame`s
+    loaded from a csv or txt file in a 'simple-seq' format.
 
-    The ``SimpleSeq.from_file`` loads the ``pandas.DataFrame``
+    The :meth:`SimpleSeq.from_file` loads the :type:`pandas.DataFrame`
     and makes any changes needed to get it to this format
     before validation, e.g., changing column names.
     """
 
     onset_s: Optional[Series[float]] = pandera.Field()
     offset_s: Optional[Series[float]] = pandera.Field()
     label: Series[pd.StringDtype] = pandera.Field(coerce=True)
@@ -49,18 +50,18 @@
 
 
 @crowsetta.interface.SeqLike.register
 @attr.define
 class SimpleSeq:
     """Class meant to represent any simple sequence-like annotation format.
 
-    Can be a .csv or .txt file;
-    should have 3 columns that represent
-    the onset time, offset time,
-    and labels of the segments
+    The annotations can be a csv or txt file;
+    the format should have 3 columns that represent
+    the onset and offset times in seconds
+    and the labels of the segments
     in the annotated sequences.
 
     The default is to assume
     a comma-separated values file
     with a header 'onset_s, offset_s, label',
     but this can be modified
     with keyword arguments.
@@ -109,18 +110,18 @@
         notated_path: Optional[PathLike] = None,
         columns_map: Optional[Mapping] = None,
         read_csv_kwargs: Optional[Mapping] = None,
     ) -> "Self":  # noqa: F821
         """Load annotations from a file
         in the 'simple-seq' format.
 
-        Can be a .csv or .txt file;
-        should have 3 columns that represent
-        the onset time, offset time,
-        and labels of the segments
+        The annotations can be a csv or txt file;
+        the format should have 3 columns that represent
+        the onset and offset times in seconds
+        and the labels of the segments
         in the annotated sequences.
 
         The default is to assume
         a comma-separated values file
         with a header 'onset_s, offset_s, label',
         but this can be modified
         with keyword arguments.
@@ -131,30 +132,30 @@
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
             Path to an annotation file,
             with one of the extensions {'.csv', '.txt'}.
         notated_path : str, pathlib.Path
-            path to file that ``annot_path`` annotates.
+            Path to file that ``annot_path`` annotates.
             E.g., an audio file, or an array file
             that contains a spectrogram generated from audio.
             Optional, default is None.
         columns_map : dict-like
             Maps column names in header of ``annot_path``
             to the standardized names
             used by this format.
             E.g., ``{'begin_time': 'onset_s', 'end_time': 'offset_s', 'text': 'label'}``.
             Optional, default is None--assumes that
             columns have the standardized names.
         read_csv_kwargs : dict
-            keyword arguments passed to
-            ``pandas.read_csv``. Default is None,
+            Keyword arguments passed to
+            :func:`pandas.read_csv`. Default is None,
             in which case all defaults for
-            ``pandas.read_csv`` will be used.
+            :func:`pandas.read_csv` will be used.
 
         Examples
         --------
         >>> example = crowsetta.data.get('simple-seq')
         >>> simple = crowsetta.formats.seq.SimpleSeq.from_file(example.annot_path,
         >>>                                                    columns_map={'start_seconds': 'onset_s',
         >>>                                                                 'stop_seconds': 'offset_s',
@@ -179,15 +180,15 @@
             offsets_s=df["offset_s"].values,
             labels=df["label"].values,
             annot_path=annot_path,
             notated_path=notated_path,
         )
 
     def to_seq(self, round_times: bool = True, decimals: int = 3) -> crowsetta.Sequence:
-        """Convert this annotation to a ``crowsetta.Sequence``.
+        """Convert this annotation to a :class:`crowsetta.Sequence`.
 
         Parameters
         ----------
         round_times : bool
             If True, round onsets_s and offsets_s.
             Default is True.
         decimals : int
@@ -224,15 +225,15 @@
             onsets_s = self.onsets_s
             offsets_s = self.offsets_s
 
         seq = crowsetta.Sequence.from_keyword(labels=self.labels, onsets_s=onsets_s, offsets_s=offsets_s)
         return seq
 
     def to_annot(self, round_times: bool = True, decimals: int = 3) -> crowsetta.Annotation:
-        """Convert this annotation to a ``crowsetta.Annotation``.
+        """Convert this annotation to a :class:`crowsetta.Annotation`.
 
         Parameters
         ----------
         round_times : bool
             If True, round onsets_s and offsets_s.
             Default is True.
         decimals : int
@@ -262,25 +263,25 @@
         and then sending them to a csv file,
         the result should be the same on Windows and Linux.
         """
         seq = self.to_seq(round_times, decimals)
         return crowsetta.Annotation(annot_path=self.annot_path, notated_path=self.notated_path, seq=seq)
 
     def to_file(self, annot_path: PathLike, to_csv_kwargs: Optional[Mapping] = None) -> None:
-        """Save this 'simple-seq' annotation to a .csv file.
+        """Save this 'simple-seq' annotation to a csv file.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
-            path with filename of .csv file that should be saved
+            Path with filename of csv file that should be saved
         to_csv_kwargs : dict-like
             keyword arguments passed to
-            ``pandas.DataFrame.to_csv``.
+            :meth:`pandas.DataFrame.to_csv`.
             Default is None, in which case
-            defaults for ``pandas.to_csv``
+            defaults for :func:`pandas.to_csv`
             will be used, except ``index``
             is set to False.
         """
         df = pd.DataFrame.from_records({"onset_s": self.onsets_s, "offset_s": self.offsets_s, "label": self.labels})
         df = df[["onset_s", "offset_s", "label"]]  # put in correct order
         try:
             df = SimpleSeqSchema.validate(df)
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/timit.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/timit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""module with functions that handle .phn annotation files from the TIMIT dataset
+"""Module with functions that handle phn annotation files
+from the TIMIT[1]_ dataset.
+
+.. [1] Garofolo, John S., et al. TIMIT Acoustic-Phonetic Continuous Speech Corpus LDC93S1.
+   Web Download. Philadelphia: Linguistic Data Consortium, 1993.
 """
 import pathlib
 import warnings
 from typing import ClassVar, Optional
 
 import attr
 import numpy as np
@@ -12,16 +16,21 @@
 from pandera.typing import Series
 
 import crowsetta
 from crowsetta.typing import PathLike
 
 
 class TimitTranscriptSchema(pandera.SchemaModel):
-    """A ``pandera.SchemaModel`` that validates ``pandas`` dataframes
-    loaded from a .phn or .wrd file in the TIMIT transcription format.
+    """A :class:`pandera.SchemaModel` that validates :type:`pandas.DataFrame`s
+    loaded from a phn or wrd file in the TIMIT[1]_ transcription format.
+
+    References
+    ----------
+    .. [1] Garofolo, John S., et al. TIMIT Acoustic-Phonetic Continuous Speech Corpus LDC93S1.
+       Web Download. Philadelphia: Linguistic Data Consortium, 1993.
     """
 
     begin_sample: Optional[Series[int]] = pandera.Field()
     end_sample: Optional[Series[int]] = pandera.Field()
     text: Series[pd.StringDtype] = pandera.Field(coerce=True)
 
     class Config:
@@ -29,15 +38,15 @@
         strict = True
 
 
 @crowsetta.interface.SeqLike.register
 @attr.define
 class Timit:
     """Class that represents annotations from transcription files in the
-    DARPA TIMIT Acoustic-Phonetic Continuous Speech Corpus (TIMIT)
+    DARPA TIMIT Acoustic-Phonetic Continuous Speech Corpus[1]_.
 
     Attributes
     ----------
     name: str
         Shorthand name for annotation format: ``'timit'``.
     ext: str
         Extension of files in annotation format:
@@ -52,28 +61,33 @@
         Vector of string labels for segments;
         each element is either a single word,
         or a single phonetic transcription code.
     annot_path : str, pathlib.Path
         Path to TIMIT transcription file from which annotations were loaded.
     audio_path : str. pathlib.Path
         Path to audio file that the TIMIT transcription file annotates.
+
+    References
+    ----------
+    .. [1] Garofolo, John S., et al. TIMIT Acoustic-Phonetic Continuous Speech Corpus LDC93S1.
+       Web Download. Philadelphia: Linguistic Data Consortium, 1993.
     """
 
     name: ClassVar[str] = "timit"
     ext: ClassVar[str] = (".phn", ".PHN", ".wrd", ".WRD")
 
     begin_samples: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
     end_samples: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
     text: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
     annot_path: pathlib.Path
     audio_path: Optional[pathlib.Path] = attr.field(default=None, converter=attr.converters.optional(pathlib.Path))
 
     @classmethod
     def from_file(cls, annot_path: PathLike, audio_path: Optional[PathLike] = None) -> "Self":  # noqa: F821
-        """Load annotations from a TIMIT transcription file
+        """Load annotations from a TIMIT[1]_ transcription file.
 
         Parameters
         ----------
         annot_path : str, pathlib.Path
             Path to a TIMIT transcription file,
             with one of the extensions {'.phn', '.PHN', '.wrd', '.WRD'}.
         audio_path : str, pathlib.Path
@@ -87,14 +101,19 @@
         >>> example = crowsetta.data.get('timit')
         >>> timit = crowsetta.formats.seq.Timit.from_file(example.annot_path)
 
         Notes
         -----
         Versions of the dataset exist with the extensions
         in capital letters. Some platforms may not have case-sensitive paths.
+
+        References
+        ----------
+        .. [1] Garofolo, John S., et al. TIMIT Acoustic-Phonetic Continuous Speech Corpus LDC93S1.
+           Web Download. Philadelphia: Linguistic Data Consortium, 1993.
         """
         annot_path = pathlib.Path(annot_path)
         # note multiple extensions, both all-uppercase and all-lowercase `.phn` exist,
         # depending on which version of TIMIT dataset you have
         crowsetta.validation.validate_ext(annot_path, extension=cls.ext)
 
         #  assume file is space-separated with no header
@@ -118,15 +137,15 @@
             text=df["text"].values,
             audio_path=audio_path,
         )
 
     def to_seq(
         self, round_times: bool = True, decimals: int = 3, samplerate: Optional[int] = None
     ) -> crowsetta.Sequence:
-        """Convert this TIMIT annotation to a ``crowsetta.Sequence``.
+        """Convert this TIMIT annotation to a :class:`crowsetta.Sequence`.
 
         Parameters
         ----------
         round_times : bool
             if True, round onsets_s and offsets_s.
             Default is True.
         decimals : int
@@ -137,15 +156,15 @@
             Sampling rate for wave files. Used to convert
             ``begin_samples`` and ``end_samples``
             from sample number to seconds.
             Default is None, in which ths function
             tries to open ``audio_path`` and determine
             the actual sampling rate. If this does not work,
             then the ``onsets_s`` and ``offsets_s`` attributes
-            of the ``crowsetta.Sequence`` are left as None.
+            of the :class:`crowsetta.Sequence` are left as None.
 
         Examples
         --------
         >>> example = crowsetta.data.get('timit')
         >>> timit = crowsetta.formats.seq.Timit.from_file(example.annot_path)
         >>> seq = timit.to_seq()
 
@@ -194,34 +213,34 @@
             offsets_s=offsets_s,
         )
         return phn_seq
 
     def to_annot(
         self, round_times: bool = True, decimals: int = 3, samplerate: Optional[int] = None
     ) -> crowsetta.Annotation:
-        """Convert this TIMIT annotation to a ``crowsetta.Annotation``.
+        """Convert this TIMIT annotation to a :class:`crowsetta.Annotation`.
 
         Parameters
         ----------
         round_times : bool
-            if True, round onsets_s and offsets_s.
+            If True, round onsets_s and offsets_s.
             Default is True.
         decimals : int
-            number of decimals places to round floating point numbers to.
+            Number of decimals places to round floating point numbers to.
             Only meaningful if round_times is True.
             Default is 3, so that times are rounded to milliseconds.
         samplerate : int
             Sampling rate for wave files. Used to convert
             ``begin_samples`` and ``end_samples``
             from sample number to seconds.
             Default is None, in which ths function
             tries to open ``audio_path`` and determine
             the actual sampling rate. If this does not work,
             then the ``onsets_s`` and ``offsets_s`` attributes
-            of the ``crowsetta.Sequence`` are left as None.
+            of the :class:`crowsetta.Sequence` are left as None.
 
         Examples
         --------
         >>> example = crowsetta.data.get('timit')
         >>> timit = crowsetta.formats.seq.Timit.from_file(example.annot_path)
         >>> annot = timit.to_annot()
 
@@ -237,20 +256,21 @@
         and then sending them to a csv file,
         the result should be the same on Windows and Linux.
         """
         phn_seq = self.to_seq(round_times, decimals, samplerate)
         return crowsetta.Annotation(annot_path=self.annot_path, notated_path=self.audio_path, seq=phn_seq)
 
     def to_file(self, annot_path: PathLike) -> None:
-        """make a .phn file from an annotation
+        """Make a phn file in the TIMIT format
+        from this instance.
 
         Parameters
         ----------
         annot_path : str, pahtlib.Path
-             path including filename where file should be saved.
+             Path including filename where file should be saved.
              Must have a valid extension for TIMIT transcription files,
              one of {'.phn', '.PHN', '.wrd', '.WRD'}.
         """
         crowsetta.validation.validate_ext(annot_path, extension=self.ext)
 
         lines = []
         for begin_sample, end_sample, text in zip(
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/yarden.py` & `crowsetta-5.0.1/src/crowsetta/formats/seq/yarden.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""module for loading annotations from .mat files
+"""Module for loading annotations from .mat files
 created by SongAnnotationGUI:
 https://github.com/yardencsGitHub/BirdSongBout/tree/master/helpers/GUI
 """
 import os
 import pathlib
 from typing import ClassVar, List
 
@@ -28,15 +28,15 @@
         raise TypeError(f"Type {type(val)} not recognized when converting annotations to arrays.")
 
 
 VALID_AUDIO_FORMATS = ["wav"]
 
 
 def _recursive_stem(path_str):
-    """helper function that 'recursively' removes file extensions
+    """Helper function that 'recursively' removes file extensions
     to recover name of an audio file from the name of an array file
 
     i.e. bird1_122213_1534.wav.mat -> i.e. bird1_122213_1534.wav
     and i.e. bird1_122213_1534.cbin.not.mat -> i.e. bird1_122213_1534.cbin
 
     adapted from ``vak`` library
     """
@@ -64,33 +64,33 @@
     Attributes
     ----------
     name: str
         Shorthand name for annotation format: ``'yarden'``.
     ext: str
         Extension of files in annotation format: ``'.mat'``.
     annotations : numpy.ndarray
-        ``numpy`` record array where each record is an annotation.
+        A :mod:`numpy` record array where each record is an annotation.
     audio_paths : numpy.ndarray
-        ``numpy`` array where each element is a path to an audio file.
+        A :mod:`numpy` array where each element is a path to an audio file.
         Same length as ``annotations``. Each element in ``annotations``
         is the annotation for the corresponding path in ``audio_paths``.
     annot_path : str, pathlib.Path
-        Path to .mat file from which annotations were loaded.
+        Path to mat file from which annotations were loaded.
     """
 
     name: ClassVar[str] = "yarden"
     ext: ClassVar[str] = ".mat"
 
     annotations: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
     audio_paths: np.ndarray = attr.field(eq=attr.cmp_using(eq=np.array_equal))
     annot_path: pathlib.Path = attr.field(converter=pathlib.Path)
 
     @classmethod
     def from_file(cls, annot_path: PathLike) -> "Self":  # noqa: F821
-        """load annotations from .mat files
+        """Load annotations from mat files
         created by SongAnnotationGUI:
         https://github.com/yardencsGitHub/BirdSongBout/tree/master/helpers/GUI
 
         Parameters
         ----------
         annot_path: str, pathlib.Path
             Path to .mat file with annotations.
@@ -108,30 +108,35 @@
         annotations = annot_mat["elements"]
         if len(audio_paths) != len(annotations):
             raise ValueError(f"list of filenames and list of annotations in {annot_path} do not have the same length")
 
         return cls(annotations=annotations, audio_paths=audio_paths, annot_path=annot_path)
 
     def to_seq(self, round_times: bool = True, decimals: int = 3) -> List[crowsetta.Sequence]:
-        """Convert this .not.mat annotation to a ``crowsetta.Sequence``.
+        """Convert this set of annotations to a :class:`list` of
+        :class:`crowsetta.Sequence` instances.
+
+        We assume there is one :class:`~crowsetta.Sequence`
+        per annotated song in the source annotations.
 
         Parameters
         ----------
         round_times : bool
             If True, round times of onsets and offsets.
             Default is True.
         decimals : int
             Number of decimals places to round floating point numbers to.
             Only meaningful if round_times is True.
             Default is 3, so that times are rounded to milliseconds.
 
         Returns
         -------
         seqs : list
-            of ``crowsetta.Sequence``, one for each element in ``annotations``.
+            A :class:`list` of :class:`~crowsetta.Sequence` instances,
+            one for each element in ``annotations``.
 
         Notes
         -----
         The ``round_times`` and ``decimals`` arguments are provided
         to reduce differences across platforms
         due to floating point error, e.g. when loading annotation files
         and then sending them to a csv file,
@@ -162,30 +167,30 @@
 
             seq = crowsetta.Sequence.from_dict(seq_dict)
             seqs.append(seq)
 
         return seqs
 
     def to_annot(self, round_times: bool = True, decimals: int = 3) -> List[crowsetta.Annotation]:
-        """Convert this .not.mat annotation to a ``crowsetta.Annotation``.
+        """Convert this annotation to a :class:`crowsetta.Annotation`.
 
         Parameters
         ----------
         round_times : bool
             If True, round times of onsets and offsets.
             Default is True.
         decimals : int
             Number of decimals places to round floating point numbers to.
             Only meaningful if round_times is True.
             Default is 3, so that times are rounded to milliseconds.
 
         Returns
         -------
         annots : list
-            of ``crowsetta.Annotation``
+            A :class:`list` of :class:`crowsetta.Annotation` instances.
 
         Notes
         -----
         The ``round_times`` and ``decimals`` arguments are provided
         to reduce differences across platforms
         due to floating point error, e.g. when loading annotation files
         and then sending them to a csv file,
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/interface/base.py` & `crowsetta-5.0.1/src/crowsetta/interface/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,12 +21,12 @@
         ...
 
     # type hints here would cause circular imports if not strings
     # TODO: fix type hinting here (use stubs?)
     @abc.abstractmethod
     def to_annot(self) -> "Union[crowsetta.Annotation,List[crowsetta.Annotation]]":  # noqa: F821
         """Converts the instance representing annotations
-        loaded from a file into a `crowsetta.Annotation`
-        or a list of `crowsetta.Annotation`s,
-        that can be used to convert to other formats
+        loaded from a file into a :class:`crowsetta.Annotation`
+        or a :class:`list` of :class:`~crowsetta.Annotation` instances,
+        that can be used to convert to other formats.
         """
         ...
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/interface/seq/base.py` & `crowsetta-5.0.1/src/crowsetta/interface/seq/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 class SeqLike(BaseFormat, abc.ABC):
     """An abstract base class defining the interface
     for any annotation format
     that can be represented as a sequence of segments,
     with each segment having an onset time,
     offset time, and a label.
 
-    In terms of code in ``crowsetta``,
+    In terms of code in :mod:`crowsetta`,
     a sequence-like format is any format
     that can be represented as a
-    ``crowsetta.Sequence`` made up of ``crowsetta.Segment``s.
+    :class:`crowsetta.Sequence` made up of :class:`crowsetta.Segment` instances.
     The code block below shows some of the features of these data types.
 
     .. code-block:: python
 
        >>> from crowsetta import Segment, Sequence
        >>> a_segment = Segment(
        ...     label='a',
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/segment.py` & `crowsetta-5.0.1/src/crowsetta/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """A class that represents a segment of a time series,
 used to annotate animal communication."""
 import attr
 import numpy as np
 from attr.validators import instance_of
 
 
-def int64_to_int(val):
-    """Converter that converts ``numpy.int64`` to ``int``,
-    returns ``int`` as is, and errors for other values.
+def convert_int(val):
+    """Converter that converts :class:`numpy.integer` to :class:`int`,
+    returns native Python :class:`int` as is, and
+    raises an error for any other type.
     """
-    if hasattr(val, "dtype"):
-        if val.dtype == np.int64:
-            return int(val)
+    if hasattr(val, "dtype") and isinstance(val, np.integer):
+        return int(val)
     elif isinstance(val, int):
         return val
     else:
         raise TypeError(f"Invalid type {type(val)} for onset or offset sample: {val}. Must be an integer.")
 
 
 @attr.s(frozen=True)
@@ -77,20 +77,20 @@
     _FIELDS = ("label", "onset_s", "offset_s", "onset_sample", "offset_sample")
 
     label = attr.ib(converter=str)
     onset_s = attr.ib(validator=attr.validators.optional(instance_of(float)), default=None)
     offset_s = attr.ib(validator=attr.validators.optional(instance_of(float)), default=None)
     onset_sample = attr.ib(
         validator=attr.validators.optional(instance_of(int)),
-        converter=attr.converters.optional(int64_to_int),
+        converter=attr.converters.optional(convert_int),
         default=None,
     )
     offset_sample = attr.ib(
         validator=attr.validators.optional(instance_of(int)),
-        converter=attr.converters.optional(int64_to_int),
+        converter=attr.converters.optional(convert_int),
         default=None,
     )
     asdict = attr.asdict
 
     def __attrs_post_init__(self):
         if (self.onset_sample is None and self.offset_sample is None) and (
             self.onset_s is None and self.offset_s is None
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/sequence.py` & `crowsetta-5.0.1/src/crowsetta/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,72 +14,76 @@
 
     E.g., a human sentence made up of syllables,
     or a bout of birdsong made up of "syllables".
 
     Attributes
     ----------
     segments : tuple
-        of Segment objects.
+        A :class:`tuple` of :class:`crowsetta.Segment` instances.
     onset_samples : numpy.ndarray or None
-        of type int, onset of each annotated segment in samples/second
+        Numpy array of type int, onset of each annotated segment in sample number.
     offset_samples : numpy.ndarray or None
-        of type int, offset of each annotated segment in samples/second
+        Numpy array of type int, offset of each annotated segment in sample number.
     onsets_s : numpy.ndarray or None
-        of type float, onset of each annotated segment in seconds
+        Numpy array of type float, onset of each annotated segment in seconds.
     offsets_s : numpy.ndarray or None
-        of type float, offset of each annotated segment in seconds
+        Numpy array of type float, offset of each annotated segment in seconds.
     labels : str, list, or numpy.ndarray
-        of type str, label for each annotated segment
+        Numpy array of type char, label for each annotated segment.
 
     Methods
     -------
-    from_segments : make a Sequence from a list of segments
-    from_keyword : make a Sequence by passing keywords (all arguments except segments)
-    from_dict : like from_keyword, but pass a Python dictionary where keys are keywords
-        and values are arguments for those keywords
-    to_dict : convert to a dict. The inverse of from_dict.
+    from_segments : method
+        Make a :class:`~crowsetta.Sequence` from a :class:`list` of :class:`~crowsetta.Segment`s.
+    from_keyword : method
+        Make a :class:`~crowsetta.Sequence` by passing keywords (all arguments except segments)
+    from_dict : method
+        Like from_keyword, but pass a Python dictionary where keys are keywords
+        and values are arguments for those keywords.
+    to_dict : method
+        Convert to a :class:`dict`. The inverse of :meth:`~crowsetta.Sequence.from_dict`.
 
     Examples
     --------
 
     A sequence with onsets and offsets given in seconds.
 
     >>> import numpy as np
     >>> import crowsetta
     >>> onsets_s = np.array([1.0, 3.0, 5.0])
     >>> offsets_s = np.array(2.0, 4.0, 6.0])
     >>> labels = np.array(['a', 'a', 'b'])
     >>> seq = crowsetta.Sequence.from_keyword(labels=labels, onsets_s=onsets_s, offsets_s=offsets_s)
 
-    The same sequence could also be made with ``crowsetta.Segment`` instances,
-    by calling the ``from_segments`` class method.
+    The same sequence could also be made
+    by calling the :meth:`~crowsetta.Sequence.from_segments` class method.
 
     >>> segments = []
     >>> for onset, offset, label in zip(onsets_s, offsets_s, labels):
     ...     segments.append(crowsetta.Segment(onset_s=onset, offset_s=offset, label=label))
     >>> seq2 = crowsetta.Sequence.from_segments(segments)
     """
 
     def __init__(self, segments, labels, onsets_s=None, offsets_s=None, onset_samples=None, offset_samples=None):
-        """Initialize a new ``Sequence`` instance.
+        """Initialize a new :class:`~crowsetta.Sequence` instance.
 
         Parameters
         ----------
-        segments : list or tuple
-            of Segment objects.
+        segments : tuple
+            A :class:`tuple` of :class:`crowsetta.Segment` instances.
         onset_samples : numpy.ndarray or None
-            of type int, onset of each annotated segment in samples/second
+            Numpy array of type int, onset of each annotated segment in sample number.
         offset_samples : numpy.ndarray or None
-            of type int, offset of each annotated segment in samples/second
+            Numpy array of type int, offset of each annotated segment in sample number.
         onsets_s : numpy.ndarray or None
-            of type float, onset of each annotated segment in seconds
+            Numpy array of type float, onset of each annotated segment in seconds.
         offsets_s : numpy.ndarray or None
-            of type float, offset of each annotated segment in seconds
+            Numpy array of type float, offset of each annotated segment in seconds.
         labels : str, list, or numpy.ndarray
-            of type str, label for each annotated segment
+            Numpy array of type char, label for each annotated segment.
         """
         if segments is not None:
             if type(segments) == Segment:
                 segments = (segments,)
             elif type(segments) in (list, tuple):
                 segments = tuple(segments)
             else:
@@ -185,23 +189,23 @@
             except ValueError:
                 raise ValueError("unable to convert all elements in labels to characters")
             labels = np.asarray(labels)
         return labels
 
     @staticmethod
     def _validate_segments_type(segments):
-        """validate that all items in list of segments are Segment"""
+        """Validate that all items in list of segments are Segment"""
         if not all([type(seg) == Segment for seg in segments]):
             raise TypeError(
                 "A Sequence must be made from a list of Segments but not all " "items in the list passed were Segments."
             )
 
     @staticmethod
     def _validate_onsets_offsets_labels(onsets_s, offsets_s, onset_samples, offset_samples, labels):
-        """validate onsets, offsets, and labels passed to __init__ or class methods
+        """Validate onsets, offsets, and labels passed to __init__ or class methods
 
         Parameters
         ----------
         onsets_s : numpy.ndarray or None
         offsets_s : numpy.ndarray or None
         onset_samples : numpy.ndarray or None
         offset_samples : numpy.ndarray or None
@@ -309,25 +313,27 @@
             onsets_s = np.asarray([None] * num_samples)
             offsets_s = np.asarray([None] * num_samples)
 
         return onsets_s, offsets_s, onset_samples, offset_samples, labels
 
     @classmethod
     def from_segments(cls, segments):
-        """construct a Sequence from a list of Segment objects
+        """Construct a :class:`crowsetta.Sequence`
+        from a :class:`list` of :class:`crowsetta.Segment` objects.
 
         Parameters
         ----------
         segments : list
-            Of crowsetta.Segment instances.
+            A :class:`list` of :class:`crowsetta.Segment` instances.
 
         Returns
         -------
-        seq : Sequence
-            instance of Sequence generated using list of segments
+        seq : crowsetta.Sequence
+            A :class:`~crowsetta.Sequence` instance
+            generated using the :class:`list` of :class:`~crowsetta.Segment`s.
         """
         cls._validate_segments_type(segments)
 
         onsets_s = []
         offsets_s = []
         onset_samples = []
         offset_samples = []
@@ -352,30 +358,31 @@
             onsets_s, offsets_s, onset_samples, offset_samples, labels
         )
 
         return cls(segments, labels, onsets_s, offsets_s, onset_samples, offset_samples)
 
     @classmethod
     def from_keyword(cls, labels, onset_samples=None, offset_samples=None, onsets_s=None, offsets_s=None):
-        """construct a Sequence from keyword arguments
+        """Construct a :class:`crowsetta.Sequence` from keyword arguments
 
         Parameters
         ----------
         onset_samples : numpy.ndarray or None
             of type int, onset of each annotated segment in samples/second
         offset_samples : numpy.ndarray or None
             of type int, offset of each annotated segment in samples/second
         onsets_s : numpy.ndarray or None
             of type float, onset of each annotated segment in seconds
         offsets_s : numpy.ndarray or None
             of type float, offset of each annotated segment in seconds
         labels : str, list, or numpy.ndarray
             of type str, label for each annotated segment
 
-        Must specify both onsets and offsets, either in units of Hz or seconds (or both).
+        Must specify both onsets and offsets,
+        either in units of Hz or seconds (or both).
         """
         labels = cls._convert_labels(labels)
 
         (onsets_s, offsets_s, onset_samples, offset_samples, labels) = cls._validate_onsets_offsets_labels(
             onsets_s, offsets_s, onset_samples, offset_samples, labels
         )
 
@@ -392,16 +399,17 @@
                 )
             )
 
         return cls(segments, labels, onsets_s, offsets_s, onset_samples, offset_samples)
 
     @classmethod
     def from_dict(cls, seq_dict):
-        """Returns a Sequence, given a Python dictionary
-        where keys of dictionary are arguments to Sequence.from_keyword()
+        """Construct a :class:`crowsetta.Sequence`
+        from a :class:`dict` where keys
+        are arguments to :meth:`~crowsetta.Sequence.from_keyword`.
 
         Parameters
         ----------
         seq_dict : dict
             with following key, value pairs
             onset_samples : numpy.ndarray or None
                 of type int, onset of each annotated segment in samples/second
@@ -410,16 +418,16 @@
             onsets_s : numpy.ndarray or None
                 of type float, onset of each annotated segment in seconds
             offsets_s : numpy.ndarray or None
                 of type float, offset of each annotated segment in seconds
             labels : str, list, or numpy.ndarray
                 of type str, label for each annotated segment
 
-        seq_dict must specify both onsets and offsets, either in units of Hz or seconds
-        (or both).
+        ``seq_dict`` must specify both onsets and offsets,
+        either in units of samples or seconds (or both).
 
         Examples
         --------
         >>> seq_dict = {
         ...     'labels': 'abc',
         ...     'onset_samples': np.asarray([16005, 17925, 19837]),
         ...     'offset_samples': np.asarray([17602, 19520, 21435]),
@@ -428,15 +436,16 @@
         >>> seq = Sequence.from_dict(seq_dict)
         """
         # basically a convenience method
         # so user doesn't have to grok the concept of 'dictionary unpacking operator'
         return cls.from_keyword(**seq_dict)
 
     def as_dict(self) -> dict:
-        """Returns sequence as a dictionary
+        """Convert this :class:`crowsetta.Sequence`
+        to a :class:`dict`.
 
         Returns
         -------
         seq_dict : dict
             with the following key, value pairs:
                 onset_samples : numpy.ndarray or None
                     of type int, onset of each annotated segment in samples/second
```

### Comparing `crowsetta-5.0.0rc2/src/crowsetta/validation.py` & `crowsetta-5.0.1/src/crowsetta/validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Module with functions for data validation.
 
 Some utilities adapted from scikit-learn under BSD 3 License
 https://github.com/scikit-learn/scikit-learn/blob/master/sklearn/utils/validation.py
 """
 import numbers
 from pathlib import PurePath
-from typing import Union
+from typing import Sequence, Union
 
 import numpy as np
+import numpy.typing as npt
 
 from .typing import PathLike
 
 
-def _num_samples(x):
+def _num_samples(x: npt.ArrayLike) -> int:
     """Return number of samples in array-like x."""
     if not hasattr(x, "__len__") and not hasattr(x, "shape"):
         if hasattr(x, "__array__"):
             x = np.asarray(x)
         else:
             raise TypeError("Expected sequence or array-like, got %s" % type(x))
     if hasattr(x, "shape"):
@@ -28,32 +29,34 @@
             return x.shape[0]
         else:
             return len(x)
     else:
         return len(x)
 
 
-def check_consistent_length(arrays):
+def check_consistent_length(arrays: Sequence[npt.ArrayLike]) -> None:
     """Check that all arrays have consistent first dimensions.
     Checks whether all objects in arrays have the same shape or length.
+
     Parameters
     ----------
     arrays : list or tuple of input objects.
         Objects that will be checked for consistent length.
     """
     lengths = [_num_samples(X) for X in arrays if X is not None]
     uniques = np.unique(lengths)
     if len(uniques) > 1:
         raise ValueError(
             "Found input variables with inconsistent numbers of" " samples: %r" % [int(length) for length in lengths]
         )
 
 
-def column_or_row_or_1d(y):
-    """Ravel column or row vector or 1d numpy array, else raises an error
+def column_or_row_or_1d(y: npt.NDArray) -> npt.NDArray:
+    """Ravel column or row vector or 1d numpy array,
+    else raises an error
 
     Parameters
     ----------
     y : array-like
 
     Returns
     -------
@@ -63,22 +66,22 @@
     if (len(shape) == 1) or (len(shape) == 2 and (shape[1] == 1 or shape[0] == 1)):
         return np.ravel(y)
     else:
         raise ValueError("bad input shape {0}".format(shape))
 
 
 def validate_ext(file: PathLike, extension: Union[str, tuple]) -> None:
-    """ "check that a file has a valid extension
+    """Check that a file has a valid extension.
 
     Parameters
     ----------
     file : str, pathlib.Path
-        path to a file; string or pathlib.Path
+        Path to a file.
     extension : str, tuple
-        valid file extension(s). tuple must be tuple of strings.
+        Valid file extension(s). Tuple must be tuple of strings.
         Function expects that extensions will be specified with a period,
         e.g. {'.phn', '.PHN'}
     """
     if isinstance(extension, str):
         extension = (extension,)
     elif isinstance(extension, tuple):
         if not all([isinstance(element, str) for element in extension]):
```

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/bbox.py` & `crowsetta-5.0.1/tests/fixtures/bbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/birdsongrec.py` & `crowsetta-5.0.1/tests/fixtures/birdsongrec.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/csv.py` & `crowsetta-5.0.1/tests/fixtures/csv.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/raven.py` & `crowsetta-5.0.1/tests/fixtures/raven.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/segment.py` & `crowsetta-5.0.1/tests/fixtures/segment.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/sequence.py` & `crowsetta-5.0.1/tests/fixtures/sequence.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/simple.py` & `crowsetta-5.0.1/tests/fixtures/simple.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/fixtures/timit.py` & `crowsetta-5.0.1/tests/fixtures/timit.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/helpers/keywords.py` & `crowsetta-5.0.1/tests/helpers/keywords.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/scripts/remake_test_csv.py` & `crowsetta-5.0.1/tests/scripts/remake_test_csv.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_annotation.py` & `crowsetta-5.0.1/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_bbox.py` & `crowsetta-5.0.1/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_data.py` & `crowsetta-5.0.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_audbbox.py` & `crowsetta-5.0.1/tests/test_formats/test_bbox/test_audbbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_raven.py` & `crowsetta-5.0.1/tests/test_formats/test_bbox/test_raven.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_formats.py` & `crowsetta-5.0.1/tests/test_formats/test_formats.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_audseq.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_audseq.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_birdsongrec.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_birdsongrec.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_generic.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_generic.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_notmat.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_notmat.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_simple.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_simple.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_timit.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_timit.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_yarden.py` & `crowsetta-5.0.1/tests/test_formats/test_seq/test_yarden.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_segment.py` & `crowsetta-5.0.1/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_sequence.py` & `crowsetta-5.0.1/tests/test_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,24 @@
     labels = 12345
     onset_samples = np.asarray([0, 2, 4, 6, 8])
     offset_samples = np.asarray([1, 3, 5, 7, 9])
     with pytest.raises(TypeError):
         Sequence.from_keyword(labels=labels, onset_samples=onset_samples, offset_samples=offset_samples)
 
 
-def test_from_keyword__onset_offset_in_seconds():
+def test_from_keyword_onset_offset_in_seconds():
     labels = "abcde"
     onsets_s = np.asarray([0.0, 0.2, 0.4, 0.6, 0.8])
     offsets_s = np.asarray([0.1, 0.3, 0.5, 0.7, 0.9])
     seq = Sequence.from_keyword(labels=labels, onsets_s=onsets_s, offsets_s=offsets_s)
     assert hasattr(seq, "segments")
     assert type(seq.segments) == tuple
 
 
-def test_from_keyword_onset_offset_in_Hertz():
+def test_from_keyword_onset_offset_in_samples():
     labels = "abcde"
     onset_samples = np.asarray([0, 2, 4, 6, 8])
     offset_samples = np.asarray([1, 3, 5, 7, 9])
     seq = Sequence.from_keyword(labels=labels, onset_samples=onset_samples, offset_samples=offset_samples)
     assert hasattr(seq, "segments")
     assert type(seq.segments) == tuple
 
@@ -78,15 +78,15 @@
         "offsets_s": np.asarray([0.1, 0.3, 0.5, 0.7, 0.9]),
     }
     seq = Sequence.from_dict(seq_dict=seq_dict)
     assert hasattr(seq, "segments")
     assert type(seq.segments) == tuple
 
 
-def test_from_dict_onset_offset_in_Hertz():
+def test_from_dict_onset_offset_in_samples():
     seq_dict = {
         "labels": "abcde",
         "onset_samples": np.asarray([0, 2, 4, 6, 8]),
         "offset_samples": np.asarray([1, 3, 5, 7, 9]),
     }
     seq = Sequence.from_dict(seq_dict=seq_dict)
     assert hasattr(seq, "segments")
@@ -104,25 +104,25 @@
 
 
 def test_missing_onset_seconds_raises():
     with pytest.raises(ValueError):
         Sequence.from_keyword(labels="abcde", offsets_s=np.asarray([0.0, 0.2, 0.4, 0.6, 0.8]))
 
 
-def test_missing_offset_Hertz_raises():
+def test_missing_offset_samples_raises():
     with pytest.raises(ValueError):
         Sequence.from_keyword(labels="abcde", onset_samples=np.asarray([0, 2, 4, 6, 8]))
 
 
-def test_missing_onset_Hertz_raises():
+def test_missing_onset_samples_raises():
     with pytest.raises(ValueError):
         Sequence.from_keyword(labels="abcde", offset_samples=np.asarray([0, 2, 4, 6, 8]))
 
 
-def test_as_dict_onset_offset_in_Hertz():
+def test_as_dict_onset_offset_in_samples():
     labels = "abcde"
     onset_samples = np.asarray([0, 2, 4, 6, 8])
     offset_samples = np.asarray([1, 3, 5, 7, 9])
     seq = Sequence.from_keyword(labels=labels, onset_samples=onset_samples, offset_samples=offset_samples)
     seq_dict = seq.as_dict()
 
     assert np.all(seq_dict["labels"] == np.asarray(list(labels)))
```

### Comparing `crowsetta-5.0.0rc2/tests/test_transcriber.py` & `crowsetta-5.0.1/tests/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/tests/test_validation.py` & `crowsetta-5.0.1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc2/PKG-INFO` & `crowsetta-5.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 Metadata-Version: 2.1
 Name: crowsetta
-Version: 5.0.0rc2
+Version: 5.0.1
 Summary: A Python tool to work with any format for annotating animal vocalizations and bioacoustics data
 Author-email: David Nicholson <nickledave@users.noreply.github.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: appdirs >=1.4.4
 Requires-Dist: attrs >=19.3.0
 Requires-Dist: evfuncs >=0.3.5
 Requires-Dist: birdsong-recognition-dataset >=0.3.2
-Requires-Dist: importlib-resources >=5.7.1
-Requires-Dist: numpy >=1.18.1
+Requires-Dist: numpy >=1.21.0
 Requires-Dist: pandas >= 1.3.5
 Requires-Dist: pandera >= 0.9.0
-Requires-Dist: scipy >=1.4.1
-Requires-Dist: SoundFile >=0.10.3
+Requires-Dist: scipy >=1.7.0
+Requires-Dist: SoundFile >=0.12.1
 Requires-Dist: black >=23.1.0 ; extra == "dev"
 Requires-Dist: crowsetta[doc, test] ; extra == "dev"
 Requires-Dist: flake8 >=6.0.0 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: isort >=5.12.0 ; extra == "dev"
 Requires-Dist: pycln >=2.1.3 ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: ipython != 8.7.0 ; extra == "doc"
 Requires-Dist: jupyterlab >=3.0.3 ; extra == "doc"
 Requires-Dist: jupytext >=1.13.8 ; extra == "doc"
 Requires-Dist: librosa >=0.9.1 ; extra == "doc"
 Requires-Dist: myst-nb >=0.15.0 ; extra == "doc"
-Requires-Dist: osfclient >=0.0.5 ; extra == "doc"
 Requires-Dist: pyprojroot >=0.2.0 ; extra == "doc"
 Requires-Dist: seaborn >=0.11.2 ; extra == "doc"
 Requires-Dist: Sphinx >=3.4.3 ; extra == "doc"
 Requires-Dist: sphinx-autobuild >= 2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-book-theme >=0.3.2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton >=0.4.0 ; extra == "doc"
 Requires-Dist: sphinx-design >=0.2.0 ; extra == "doc"
@@ -59,22 +56,24 @@
 <img src="https://github.com/vocalpy/crowsetta/blob/main/doc/_static/crowsetta-primary-logo.png?raw=True" width="400">
 </div>
 <hr>
 
 ## A Python tool to work with any format for annotating animal vocalizations and bioacoustics data
 
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-review/issues/68)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05338/status.svg)](https://doi.org/10.21105/joss.05338)
 [![Build Status](https://github.com/vocalpy/crowsetta/actions/workflows/ci.yml/badge.svg)](https://github.com/vocalpy/crowsetta/actions)
 [![Documentation Status](https://readthedocs.org/projects/crowsetta/badge/?version=latest)](https://crowsetta.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/159904494.svg)](https://zenodo.org/badge/latestdoi/159904494)
 [![PyPI version](https://badge.fury.io/py/crowsetta.svg)](https://badge.fury.io/py/crowsetta)
 [![PyPI Python versions](https://img.shields.io/pypi/pyversions/crowsetta)](https://img.shields.io/pypi/pyversions/crowsetta)
 [![codecov](https://codecov.io/gh/vocalpy/crowsetta/branch/main/graph/badge.svg?token=TXtNTxXKmb)](https://codecov.io/gh/vocalpy/crowsetta)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 crowsetta provides a Pythonic way to work with annotation formats 
 for animal vocalizations and bioacoustics data. 
 These formats are used, for example, by 
 applications that enable users to annotate audio and/or spectrograms. 
 Such annotations typically include the times when sound events start and stop, 
@@ -244,16 +243,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="http://tessarhinehart.com"><img src="https://avatars.githubusercontent.com/u/27306428?v=4?s=100" width="100px;" alt="Tessa Rhinehart"/><br /><sub><b>Tessa Rhinehart</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=rhine3" title="Documentation">📖</a> <a href="https://github.com/vocalpy/crowsetta/issues?q=author%3Arhine3" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/shaupert"><img src="https://avatars.githubusercontent.com/u/43136040?v=4?s=100" width="100px;" alt="Sylvain HAUPERT"/><br /><sub><b>Sylvain HAUPERT</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=shaupert" title="Code">💻</a> <a href="#ideas-shaupert" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://tessarhinehart.com"><img src="https://avatars.githubusercontent.com/u/27306428?v=4?s=100" width="100px;" alt="Tessa Rhinehart"/><br /><sub><b>Tessa Rhinehart</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=rhine3" title="Documentation">📖</a> <a href="https://github.com/vocalpy/crowsetta/issues?q=author%3Arhine3" title="Bug reports">🐛</a> <a href="#userTesting-rhine3" title="User Testing">📓</a> <a href="#ideas-rhine3" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/shaupert"><img src="https://avatars.githubusercontent.com/u/43136040?v=4?s=100" width="100px;" alt="Sylvain HAUPERT"/><br /><sub><b>Sylvain HAUPERT</b></sub></a><br /><a href="https://github.com/vocalpy/crowsetta/commits?author=shaupert" title="Code">💻</a> <a href="#ideas-shaupert" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-shaupert" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/YannickJadoul"><img src="https://avatars.githubusercontent.com/u/8025744?v=4?s=100" width="100px;" alt="Yannick Jadoul"/><br /><sub><b>Yannick Jadoul</b></sub></a><br /><a href="#ideas-YannickJadoul" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/vocalpy/crowsetta/issues?q=author%3AYannickJadoul" title="Bug reports">🐛</a> <a href="https://github.com/vocalpy/crowsetta/commits?author=YannickJadoul" title="Documentation">📖</a> <a href="#userTesting-YannickJadoul" title="User Testing">📓</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

