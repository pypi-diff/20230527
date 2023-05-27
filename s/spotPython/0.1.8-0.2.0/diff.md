# Comparing `tmp/spotPython-0.1.8.tar.gz` & `tmp/spotPython-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.1.8.tar", last modified: Fri May 26 12:49:37 2023, max compression
+gzip compressed data, was "spotPython-0.2.0.tar", last modified: Sat May 27 21:02:35 2023, max compression
```

## Comparing `spotPython-0.1.8.tar` & `spotPython-0.2.0.tar`

### file list

```diff
@@ -1,215 +1,213 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.429461 spotPython-0.1.8/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.376621 spotPython-0.1.8/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.381266 spotPython-0.1.8/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    12811 2023-05-20 21:56:15.000000 spotPython-0.1.8/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.1.8/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.393733 spotPython-0.1.8/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.1.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.1.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.1.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.1.8/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.1.8/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.1.8/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-26 12:49:37.429284 spotPython-0.1.8/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.1.8/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.396460 spotPython-0.1.8/docs/
--rw-r--r--   0 bartz      (501) staff       (20)   137970 2023-05-20 04:16:59.000000 spotPython-0.1.8/docs/bart23e.html
--rw-r--r--   0 bartz      (501) staff       (20)   335911 2023-05-20 04:17:05.000000 spotPython-0.1.8/docs/bart23e.pdf
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.398763 spotPython-0.1.8/docs/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.1.8/docs/figures/parallel.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.399079 spotPython-0.1.8/docs/img/
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-19 13:48:01.000000 spotPython-0.1.8/docs/img/spotLogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-20 04:17:06.000000 spotPython-0.1.8/docs/index.html
--rw-r--r--   0 bartz      (501) staff       (20)    48220 2023-05-20 04:17:05.000000 spotPython-0.1.8/docs/search.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.377326 spotPython-0.1.8/docs/site_libs/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.401728 spotPython-0.1.8/docs/site_libs/bootstrap/
--rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap-icons.css
--rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap-icons.woff
--rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-20 04:16:58.000000 spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap.min.css
--rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.402247 spotPython-0.1.8/docs/site_libs/clipboard/
--rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/clipboard/clipboard.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.403325 spotPython-0.1.8/docs/site_libs/quarto-html/
--rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-html/anchor.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-html/popper.min.js
--rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-19 12:56:10.000000 spotPython-0.1.8/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
--rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-html/quarto.js
--rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-html/tippy.css
--rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-html/tippy.umd.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.403560 spotPython-0.1.8/docs/site_libs/quarto-nav/
--rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-nav/quarto-nav.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.404174 spotPython-0.1.8/docs/site_libs/quarto-search/
--rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-search/autocomplete.umd.js
--rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-search/fuse.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.1.8/docs/site_libs/quarto-search/quarto-search.js
--rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.1.8/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.1.8/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.418145 spotPython-0.1.8/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.1.8/notebooks/00_spot_doc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.1.8/notebooks/01_spot_intro.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.1.8/notebooks/02_spot_multidim.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.1.8/notebooks/03_spot_anisotropic.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.1.8/notebooks/04_spot_sklearn_surrogate.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.1.8/notebooks/05_spot_sklearn_optimizers.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.1.8/notebooks/06_spot_gaussian.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.1.8/notebooks/07_spot_ei.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.1.8/notebooks/08_spot_noisy.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.1.8/notebooks/09_spot_ocba.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.1.8/notebooks/10_spot_hpt_sklearn_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    23215 2023-05-20 08:35:48.000000 spotPython-0.1.8/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    28105 2023-05-20 08:36:30.000000 spotPython-0.1.8/notebooks/12_spot_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.1.8/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   754486 2023-05-26 06:53:37.000000 spotPython-0.1.8/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.1.8/notebooks/15_spot_hpt_sklearn_regression.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)  2496232 2023-05-26 12:47:53.000000 spotPython-0.1.8/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.377548 spotPython-0.1.8/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.418634 spotPython-0.1.8/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.1.8/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.1.8/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.420112 spotPython-0.1.8/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.1.8/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.1.8/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.1.8/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.1.8/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.1.8/notebooks/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-26 12:49:00.000000 spotPython-0.1.8/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-26 12:49:37.429501 spotPython-0.1.8/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.377812 spotPython-0.1.8/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.420367 spotPython-0.1.8/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-26 12:49:37.000000 spotPython-0.1.8/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.421172 spotPython-0.1.8/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.1.8/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.421436 spotPython-0.1.8/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.1.8/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.1.8/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.422594 spotPython-0.1.8/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.1.8/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.1.8/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-20 18:34:33.000000 spotPython-0.1.8/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.1.8/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     6154 2023-05-20 09:08:40.000000 spotPython-0.1.8/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.1.8/src/spotPython/data/torch_hyper_dict.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.422943 spotPython-0.1.8/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.1.8/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.1.8/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.1.8/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.423312 spotPython-0.1.8/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     6273 2023-05-26 12:49:30.000000 spotPython-0.1.8/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     4769 2023-05-20 09:28:12.000000 spotPython-0.1.8/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.1.8/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.423725 spotPython-0.1.8/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.1.8/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     3849 2023-05-19 14:05:20.000000 spotPython-0.1.8/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    26028 2023-05-07 10:48:32.000000 spotPython-0.1.8/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.424042 spotPython-0.1.8/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-02-02 22:52:12.000000 spotPython-0.1.8/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.1.8/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.424190 spotPython-0.1.8/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    32443 2023-05-12 15:27:01.000000 spotPython-0.1.8/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.424866 spotPython-0.1.8/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1000 2023-05-20 08:56:22.000000 spotPython-0.1.8/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      413 2023-05-20 08:56:34.000000 spotPython-0.1.8/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      791 2023-05-20 08:56:44.000000 spotPython-0.1.8/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)    16118 2023-05-26 12:49:31.000000 spotPython-0.1.8/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.426643 spotPython-0.1.8/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.1.8/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.1.8/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.1.8/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.1.8/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.1.8/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.1.8/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.1.8/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     1080 2023-05-20 08:23:54.000000 spotPython-0.1.8/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-20 20:12:12.000000 spotPython-0.1.8/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.1.8/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.1.8/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.1.8/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.421056 spotPython-0.1.8/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-26 12:49:37.000000 spotPython-0.1.8/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     9141 2023-05-26 12:49:37.000000 spotPython-0.1.8/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-26 12:49:37.000000 spotPython-0.1.8/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-26 12:49:37.000000 spotPython-0.1.8/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-26 12:49:37.000000 spotPython-0.1.8/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-26 12:49:37.429028 spotPython-0.1.8/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.1.8/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.1.8/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.1.8/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.1.8/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.1.8/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.297261 spotPython-0.2.0/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.265755 spotPython-0.2.0/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.269266 spotPython-0.2.0/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    12811 2023-05-20 21:56:15.000000 spotPython-0.2.0/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.2.0/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.275080 spotPython-0.2.0/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.2.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.2.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.2.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.2.0/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.2.0/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.2.0/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-27 21:02:35.297086 spotPython-0.2.0/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.2.0/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.276290 spotPython-0.2.0/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)   189050 2023-05-27 21:00:53.000000 spotPython-0.2.0/docs/bart23e.html
+-rw-r--r--   0 bartz      (501) staff       (20)   707240 2023-05-27 21:01:00.000000 spotPython-0.2.0/docs/bart23e.pdf
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.276543 spotPython-0.2.0/docs/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.2.0/docs/figures/parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-27 21:01:00.000000 spotPython-0.2.0/docs/index.html
+-rw-r--r--   0 bartz      (501) staff       (20)    63930 2023-05-27 21:01:00.000000 spotPython-0.2.0/docs/search.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.266374 spotPython-0.2.0/docs/site_libs/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.277480 spotPython-0.2.0/docs/site_libs/bootstrap/
+-rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-27 21:00:51.000000 spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.277655 spotPython-0.2.0/docs/site_libs/clipboard/
+-rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.278497 spotPython-0.2.0/docs/site_libs/quarto-html/
+-rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-23 19:54:10.000000 spotPython-0.2.0/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.278641 spotPython-0.2.0/docs/site_libs/quarto-nav/
+-rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.279073 spotPython-0.2.0/docs/site_libs/quarto-search/
+-rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.2.0/docs/site_libs/quarto-search/quarto-search.js
+-rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.2.0/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.2.0/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.287417 spotPython-0.2.0/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.2.0/notebooks/00_spot_doc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.2.0/notebooks/01_spot_intro.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.2.0/notebooks/02_spot_multidim.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.2.0/notebooks/03_spot_anisotropic.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.2.0/notebooks/04_spot_sklearn_surrogate.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.2.0/notebooks/05_spot_sklearn_optimizers.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.2.0/notebooks/06_spot_gaussian.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.2.0/notebooks/07_spot_ei.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.2.0/notebooks/08_spot_noisy.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.2.0/notebooks/09_spot_ocba.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.2.0/notebooks/10_spot_hpt_sklearn_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-27 07:00:04.000000 spotPython-0.2.0/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-27 07:00:42.000000 spotPython-0.2.0/notebooks/12_spot_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.2.0/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   100996 2023-05-27 21:00:00.000000 spotPython-0.2.0/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.2.0/notebooks/15_spot_hpt_sklearn_regression.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  2496232 2023-05-26 12:47:53.000000 spotPython-0.2.0/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.266562 spotPython-0.2.0/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.287565 spotPython-0.2.0/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.2.0/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.2.0/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.289390 spotPython-0.2.0/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.0/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.2.0/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.2.0/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.2.0/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.2.0/notebooks/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-27 06:20:37.000000 spotPython-0.2.0/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-27 21:02:35.297356 spotPython-0.2.0/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.266831 spotPython-0.2.0/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.289552 spotPython-0.2.0/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-27 21:02:35.000000 spotPython-0.2.0/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.290315 spotPython-0.2.0/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.2.0/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.290581 spotPython-0.2.0/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.2.0/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.2.0/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.291364 spotPython-0.2.0/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.2.0/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.2.0/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-20 18:34:33.000000 spotPython-0.2.0/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.2.0/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5171 2023-05-27 19:39:42.000000 spotPython-0.2.0/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.2.0/src/spotPython/data/torch_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.291769 spotPython-0.2.0/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.2.0/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.2.0/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.2.0/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.292128 spotPython-0.2.0/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     6273 2023-05-26 12:49:30.000000 spotPython-0.2.0/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4911 2023-05-27 18:18:59.000000 spotPython-0.2.0/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.2.0/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.292513 spotPython-0.2.0/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.2.0/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-27 19:48:36.000000 spotPython-0.2.0/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26028 2023-05-07 10:48:32.000000 spotPython-0.2.0/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.292763 spotPython-0.2.0/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-02-02 22:52:12.000000 spotPython-0.2.0/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.2.0/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.292879 spotPython-0.2.0/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    32443 2023-05-12 15:27:01.000000 spotPython-0.2.0/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.293399 spotPython-0.2.0/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.2.0/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.2.0/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.2.0/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13380 2023-05-27 19:18:58.000000 spotPython-0.2.0/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.294801 spotPython-0.2.0/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.2.0/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.2.0/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.2.0/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.2.0/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.2.0/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.2.0/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.2.0/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1421 2023-05-27 07:35:33.000000 spotPython-0.2.0/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-20 20:12:12.000000 spotPython-0.2.0/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.2.0/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.2.0/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.2.0/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.290183 spotPython-0.2.0/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-27 21:02:35.000000 spotPython-0.2.0/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     9159 2023-05-27 21:02:35.000000 spotPython-0.2.0/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-27 21:02:35.000000 spotPython-0.2.0/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-27 21:02:35.000000 spotPython-0.2.0/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-27 21:02:35.000000 spotPython-0.2.0/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-27 21:02:35.296861 spotPython-0.2.0/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.2.0/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.2.0/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.2.0/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.2.0/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.2.0/tox.ini
```

### Comparing `spotPython-0.1.8/.github/workflows/test.yml` & `spotPython-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/.gitignore` & `spotPython-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.2.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.2.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.2.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.2.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.2.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.2.0/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/LICENSE.txt` & `spotPython-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/PKG-INFO` & `spotPython-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.1.8
+Version: 0.2.0
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.1.8/README.md` & `spotPython-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/bart23e.html` & `spotPython-0.2.0/docs/bart23e.html`

 * *Files 17% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     <div class="quarto-alternate-formats"><h2>Other Formats</h2><ul><li><a href="bart23e.pdf"><i class="bi bi-file-pdf"></i>PDF</a></li></ul></div></div>
 <!-- main -->
 <main class="content" id="quarto-document-content">
 
 <header id="title-block-header" class="quarto-title-block default">
 <div class="quarto-title">
 <h1 class="title">PyTorch Hyperparameter Tuning — A Tutorial for spotPython</h1>
-<p class="subtitle lead">Version 0.1.3</p>
+<p class="subtitle lead">Version 0.2.0</p>
 </div>
 
 
 <div class="quarto-title-meta-author">
   <div class="quarto-title-meta-heading">Author</div>
   <div class="quarto-title-meta-heading">Affiliations</div>
   
@@ -214,25 +214,25 @@
 <h1>Hyperparameter Tuning for PyTorch With <code>spotPython</code></h1>
 <p>In this tutorial, we will show how <code>spotPython</code> can be integrated into the <code>PyTorch</code> training workflow. It is based on the tutorial “Hyperparameter Tuning with Ray Tune” from the <code>PyTorch</code> documentation <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span>, which is an extension of the tutorial “Training a Classifier” <span class="citation" data-cites="pyto23b">(<a href="#ref-pyto23b" role="doc-biblioref">PyTorch 2023b</a>)</span> for training a CIFAR10 image classifier.</p>
 <p>This document refers to the following software versions:</p>
 <ul>
 <li><code>python</code>: 3.10.10</li>
 <li><code>torch</code>: 2.0.1</li>
 <li><code>torchvision</code>: 0.15.0</li>
-<li><code>spotPython</code>: 0.1.3</li>
+<li><code>spotPython</code>: 0.2.0</li>
 </ul>
 <p><code>spotPython</code> can be installed via pip<a href="#fn2" class="footnote-ref" id="fnref2" role="doc-noteref"><sup>2</sup></a>.</p>
 <pre class="{raw}"><code>!pip install spotPython</code></pre>
 <p>Results that refer to the <code>Ray Tune</code> package are taken from <a href="https://PyTorch.org/tutorials/beginner/hyperparameter_tuning_tutorial.html">https://PyTorch.org/tutorials/beginner/hyperparameter_tuning_tutorial.html</a><a href="#fn3" class="footnote-ref" id="fnref3" role="doc-noteref"><sup>3</sup></a>.</p>
 <section id="sec-setup" class="level2">
 <h2 class="anchored" data-anchor-id="sec-setup">Setup</h2>
 <p>Before we consider the detailed experimental setup, we select the parameters that affect run time, initial design size and the device that is used.</p>
 <div class="cell" data-execution_count="1">
 <div class="sourceCode cell-code" id="cb2"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb2-1"><a href="#cb2-1" aria-hidden="true" tabindex="-1"></a>MAX_TIME <span class="op">=</span> <span class="dv">60</span></span>
-<span id="cb2-2"><a href="#cb2-2" aria-hidden="true" tabindex="-1"></a>INIT_SIZE <span class="op">=</span> <span class="dv">10</span></span>
+<span id="cb2-2"><a href="#cb2-2" aria-hidden="true" tabindex="-1"></a>INIT_SIZE <span class="op">=</span> <span class="dv">20</span></span>
 <span id="cb2-3"><a href="#cb2-3" aria-hidden="true" tabindex="-1"></a>DEVICE <span class="op">=</span> <span class="st">"cpu"</span> <span class="co"># "cuda:0"</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="initialization-of-the-fun_control-dictionary" class="level2">
 <h2 class="anchored" data-anchor-id="initialization-of-the-fun_control-dictionary">Initialization of the <code>fun_control</code> Dictionary</h2>
 <p><code>spotPython</code> uses a Python dictionary for storing the information required for the hyperparameter tuning process. This dictionary is called <code>fun_control</code> and is initialized with the function <code>fun_control_init</code>. The function <code>fun_control_init</code> returns a skeleton dictionary. The dictionary is filled with the required information for the hyperparameter tuning process. It stores the hyperparameter tuning settings, e.g., the deep learning network architecture that should be tuned, the classification (or regression) problem, and the data that is used for the tuning. The dictionary is used as an input for the SPOT function.</p>
 <div class="cell" data-execution_count="4">
@@ -315,17 +315,17 @@
 <pre class="{raw}"><code>optimizer = optim.SGD(net.parameters(), lr=config["lr"], momentum=0.9)</code></pre>
 </section>
 <section id="sec-implementation-with-spotpython" class="level3">
 <h3 class="anchored" data-anchor-id="sec-implementation-with-spotpython">Implementing a Configurable Neural Network With spotPython</h3>
 <p><code>spotPython</code> implements a class which is similar to the class described in the <code>PyTorch</code> tutorial. The class is called <code>Net_CIFAR10</code> and is implemented in the file <code>netcifar10.py</code>.</p>
 <pre class="{raw}"><code>import spotPython.torch.netcore as netcore
 class Net_CIFAR10(netcore.Net_Core):
-    def __init__(self, l1, l2, lr, batch_size, epochs, k_folds, patience):
+    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):
         super(Net_CIFAR10, self).__init__(
-            lr=lr, batch_size=batch_size, epochs=epochs, k_folds=k_folds,
+            lr_mult=lr_mult, batch_size=batch_size, epochs=epochs, k_folds=k_folds,
             patience=patience
         )
         self.conv1 = nn.Conv2d(3, 6, 5)
         self.pool = nn.MaxPool2d(2, 2)
         self.conv2 = nn.Conv2d(6, 16, 5)
         self.fc1 = nn.Linear(16 * 5 * 5, l1)
         self.fc2 = nn.Linear(l1, l2)
@@ -335,30 +335,30 @@
         x = self.pool(F.relu(self.conv1(x)))
         x = self.pool(F.relu(self.conv2(x)))
         x = x.view(-1, 16 * 5 * 5)
         x = F.relu(self.fc1(x))
         x = F.relu(self.fc2(x))
         x = self.fc3(x)
         return x</code></pre>
-<p><code>Net_CIFAR10</code> inherits from the class <code>Net_Core</code> which is implemented in the file <code>netcore.py</code>. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate <code>lr</code>, the batch size <code>batch_size</code>, the number of epochs <code>epochs</code>, the number of folds <code>k_folds</code> for the cross validation, and the patience <code>patience</code> for the early stopping. The class <code>Net_Core</code> is shown below.</p>
+<p><code>Net_CIFAR10</code> inherits from the class <code>Net_Core</code> which is implemented in the file <code>netcore.py</code>. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate multiplier <code>lr_mult</code>, the batch size <code>batch_size</code>, the number of epochs <code>epochs</code>, the number of folds <code>k_folds</code> for the cross validation, and the patience <code>patience</code> for the early stopping. The class <code>Net_Core</code> is shown below.</p>
 <pre class="{raw}"><code>from torch import nn
 
 
 class Net_Core(nn.Module):
-    def __init__(self, lr, batch_size, epochs, k_folds, patience):
+    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):
         super(Net_Core, self).__init__()
-        self.lr = lr
+        self.lr_mult = lr_mult
         self.batch_size = batch_size
         self.epochs = epochs
         self.k_folds = k_folds
         self.patience = patience</code></pre>
 </section>
 <section id="sec-comparison" class="level3">
 <h3 class="anchored" data-anchor-id="sec-comparison">Comparison of the Approach Described in the PyTorch Tutorial With spotPython</h3>
-<p>Comparing the class <code>Net</code> from the <code>PyTorch</code> tutorial and the class <code>Net_CIFAR10</code> from <code>spotPython</code>, we see that the class <code>Net_CIFAR10</code> has additional attributes and does not inherit from <code>nn</code> directly. It adds an additional class, <code>Net_core</code>, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate <code>lr</code> or the batch size <code>batch_size</code>.</p>
+<p>Comparing the class <code>Net</code> from the <code>PyTorch</code> tutorial and the class <code>Net_CIFAR10</code> from <code>spotPython</code>, we see that the class <code>Net_CIFAR10</code> has additional attributes and does not inherit from <code>nn</code> directly. It adds an additional class, <code>Net_core</code>, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate multiplier <code>lr_mult</code> or the batch size <code>batch_size</code>.</p>
 <p><code>spotPython</code>’s <code>core_model</code> implements an instance of the <code>Net_CIFAR10</code> class. In addition to the basic neural network model, the <code>core_model</code> can use these additional attributes. <code>spotPython</code> provides methods for handling these additional attributes to guarantee 100% compatibility with the <code>PyTorch</code> classes. The method <code>add_core_model_to_fun_control</code> adds the hyperparameters and additional attributes to the <code>fun_control</code> dictionary. The method is shown below.</p>
 <div class="cell" data-execution_count="8">
 <div class="sourceCode cell-code" id="cb12"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb12-1"><a href="#cb12-1" aria-hidden="true" tabindex="-1"></a>core_model <span class="op">=</span> Net_CIFAR10</span>
 <span id="cb12-2"><a href="#cb12-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> add_core_model_to_fun_control(core_model<span class="op">=</span>core_model,</span>
 <span id="cb12-3"><a href="#cb12-3" aria-hidden="true" tabindex="-1"></a>                              fun_control<span class="op">=</span>fun_control,</span>
 <span id="cb12-4"><a href="#cb12-4" aria-hidden="true" tabindex="-1"></a>                              hyper_dict<span class="op">=</span>TorchHyperDict,</span>
 <span id="cb12-5"><a href="#cb12-5" aria-hidden="true" tabindex="-1"></a>                              filename<span class="op">=</span><span class="va">None</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
@@ -377,15 +377,15 @@
 <ul>
 <li>learning rate (<code>lr</code>),</li>
 <li>batch size (<code>batch_size</code>),</li>
 <li>epochs (<code>epochs</code>),</li>
 <li>k_folds (<code>k_folds</code>), and</li>
 <li>early stopping criterion “patience” (<code>patience</code>)</li>
 </ul>
-<p>Further attributes can be easily added to the class, e.g., <code>optimizer</code> or <code>loss_function</code>.</p>
+<p>Further attributes can be easily added to the class, e.g., <code>optimizer</code>.</p>
 </div>
 </div>
 </section>
 </section>
 <section id="sec-search-space" class="level2">
 <h2 class="anchored" data-anchor-id="sec-search-space">The Search Space</h2>
 <p>In <a href="#sec-configuring-the-search-space-with-ray-tune">Section&nbsp;3.6.1</a>, we first describe how to configure the search space with <code>ray[tune]</code> (as shown in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>) and then how to configure the search space with <code>spotPython</code> in <a href="#sec-configuring-the-search-space-with-spotpython">Section&nbsp;3.6.2</a>.</p>
@@ -426,20 +426,20 @@
 <span id="cb15-8"><a href="#cb15-8" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">9</span><span class="fu">},</span></span>
 <span id="cb15-9"><a href="#cb15-9" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"l2"</span><span class="fu">:</span> <span class="fu">{</span></span>
 <span id="cb15-10"><a href="#cb15-10" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
 <span id="cb15-11"><a href="#cb15-11" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
 <span id="cb15-12"><a href="#cb15-12" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
 <span id="cb15-13"><a href="#cb15-13" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
 <span id="cb15-14"><a href="#cb15-14" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">9</span><span class="fu">},</span></span>
-<span id="cb15-15"><a href="#cb15-15" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"lr"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb15-15"><a href="#cb15-15" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"lr_mult"</span><span class="fu">:</span> <span class="fu">{</span></span>
 <span id="cb15-16"><a href="#cb15-16" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"float"</span><span class="fu">,</span></span>
-<span id="cb15-17"><a href="#cb15-17" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">1e-03</span><span class="fu">,</span></span>
+<span id="cb15-17"><a href="#cb15-17" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="fl">1.0</span><span class="fu">,</span></span>
 <span id="cb15-18"><a href="#cb15-18" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-19"><a href="#cb15-19" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">1e-05</span><span class="fu">,</span></span>
-<span id="cb15-20"><a href="#cb15-20" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">1e-02</span><span class="fu">},</span></span>
+<span id="cb15-19"><a href="#cb15-19" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="fl">0.1</span><span class="fu">,</span></span>
+<span id="cb15-20"><a href="#cb15-20" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">10</span><span class="fu">},</span></span>
 <span id="cb15-21"><a href="#cb15-21" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"batch_size"</span><span class="fu">:</span> <span class="fu">{</span></span>
 <span id="cb15-22"><a href="#cb15-22" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
 <span id="cb15-23"><a href="#cb15-23" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">,</span></span>
 <span id="cb15-24"><a href="#cb15-24" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
 <span id="cb15-25"><a href="#cb15-25" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">1</span><span class="fu">,</span></span>
 <span id="cb15-26"><a href="#cb15-26" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">},</span></span>
 <span id="cb15-27"><a href="#cb15-27" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"epochs"</span><span class="fu">:</span> <span class="fu">{</span></span>
@@ -477,45 +477,22 @@
 <span id="cb15-59"><a href="#cb15-59" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"factor"</span><span class="fu">,</span></span>
 <span id="cb15-60"><a href="#cb15-60" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="st">"SGD"</span><span class="fu">,</span></span>
 <span id="cb15-61"><a href="#cb15-61" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
 <span id="cb15-62"><a href="#cb15-62" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"class_name"</span><span class="fu">:</span> <span class="st">"torch.optim"</span><span class="fu">,</span></span>
 <span id="cb15-63"><a href="#cb15-63" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"core_model_parameter_type"</span><span class="fu">:</span> <span class="st">"str"</span><span class="fu">,</span></span>
 <span id="cb15-64"><a href="#cb15-64" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">0</span><span class="fu">,</span></span>
 <span id="cb15-65"><a href="#cb15-65" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">12</span><span class="fu">},</span></span>
-<span id="cb15-66"><a href="#cb15-66" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"criterion"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-67"><a href="#cb15-67" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"levels"</span><span class="fu">:</span> <span class="ot">[</span><span class="st">"L1Loss"</span><span class="ot">,</span></span>
-<span id="cb15-68"><a href="#cb15-68" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"MSELoss"</span><span class="ot">,</span></span>
-<span id="cb15-69"><a href="#cb15-69" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"CrossEntropyLoss"</span><span class="ot">,</span></span>
-<span id="cb15-70"><a href="#cb15-70" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"CTCLoss"</span><span class="ot">,</span></span>
-<span id="cb15-71"><a href="#cb15-71" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"NLLLoss"</span><span class="ot">,</span></span>
-<span id="cb15-72"><a href="#cb15-72" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"PoissonNLLLoss"</span><span class="ot">,</span></span>
-<span id="cb15-73"><a href="#cb15-73" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"GaussianNLLLoss"</span><span class="ot">,</span></span>
-<span id="cb15-74"><a href="#cb15-74" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"KLDivLoss"</span><span class="ot">,</span></span>
-<span id="cb15-75"><a href="#cb15-75" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"BCELoss"</span><span class="ot">,</span></span>
-<span id="cb15-76"><a href="#cb15-76" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"BCEWithLogitsLoss"</span><span class="ot">,</span></span>
-<span id="cb15-77"><a href="#cb15-77" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"MarginRankingLoss"</span><span class="ot">,</span></span>
-<span id="cb15-78"><a href="#cb15-78" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"HingeEmbeddingLoss"</span><span class="ot">,</span></span>
-<span id="cb15-79"><a href="#cb15-79" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"MultiLabelMarginLoss"</span><span class="ot">,</span></span>
-<span id="cb15-80"><a href="#cb15-80" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"HuberLoss"</span><span class="ot">,</span></span>
-<span id="cb15-81"><a href="#cb15-81" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"SmoothL1Loss"</span><span class="ot">,</span></span>
-<span id="cb15-82"><a href="#cb15-82" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"SoftMarginLoss"</span><span class="ot">,</span></span>
-<span id="cb15-83"><a href="#cb15-83" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"MultiLabelSoftMarginLoss"</span><span class="ot">,</span></span>
-<span id="cb15-84"><a href="#cb15-84" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"CosineEmbeddingLoss"</span><span class="ot">,</span></span>
-<span id="cb15-85"><a href="#cb15-85" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"MultiMarginLoss"</span><span class="ot">,</span></span>
-<span id="cb15-86"><a href="#cb15-86" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"TripletMarginLoss"</span><span class="ot">,</span></span>
-<span id="cb15-87"><a href="#cb15-87" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"TripletMarginWithDistanceLoss"</span><span class="ot">]</span><span class="fu">,</span></span>
-<span id="cb15-88"><a href="#cb15-88" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"factor"</span><span class="fu">,</span></span>
-<span id="cb15-89"><a href="#cb15-89" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="st">"CrossEntropyLoss"</span><span class="fu">,</span></span>
-<span id="cb15-90"><a href="#cb15-90" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-91"><a href="#cb15-91" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"class_name"</span><span class="fu">:</span> <span class="st">"torch.nn"</span><span class="fu">,</span></span>
-<span id="cb15-92"><a href="#cb15-92" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"core_model_parameter_type"</span><span class="fu">:</span> <span class="st">"instance()"</span><span class="fu">,</span></span>
-<span id="cb15-93"><a href="#cb15-93" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">0</span><span class="fu">,</span></span>
-<span id="cb15-94"><a href="#cb15-94" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">20</span><span class="fu">}</span></span>
-<span id="cb15-95"><a href="#cb15-95" aria-hidden="true" tabindex="-1"></a>    <span class="fu">}</span></span>
-<span id="cb15-96"><a href="#cb15-96" aria-hidden="true" tabindex="-1"></a><span class="fu">}</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<span id="cb15-66"><a href="#cb15-66" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"sgd_momentum"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb15-67"><a href="#cb15-67" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"float"</span><span class="fu">,</span></span>
+<span id="cb15-68"><a href="#cb15-68" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="fl">0.0</span><span class="fu">,</span></span>
+<span id="cb15-69"><a href="#cb15-69" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb15-70"><a href="#cb15-70" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="fl">0.0</span><span class="fu">,</span></span>
+<span id="cb15-71"><a href="#cb15-71" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="fl">1.0</span><span class="fu">}</span></span>
+<span id="cb15-72"><a href="#cb15-72" aria-hidden="true" tabindex="-1"></a>    <span class="fu">}</span></span>
+<span id="cb15-73"><a href="#cb15-73" aria-hidden="true" tabindex="-1"></a><span class="fu">}</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </section>
 </section>
 </section>
 <section id="sec-modification-of-hyperparameters" class="level2">
 <h2 class="anchored" data-anchor-id="sec-modification-of-hyperparameters">Modifying the Hyperparameters</h2>
 <p>Ray tune <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span> does not provide a way to change the specified hyperparameters without re-compilation. However, <code>spotPython</code> provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters without re-compilation of the Python source code. These functions are described in the following.</p>
 <section id="sec-modification-of-default-values" class="level3">
@@ -539,125 +516,284 @@
 <div class="cell" data-execution_count="10">
 <div class="sourceCode cell-code" id="cb17"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb17-1"><a href="#cb17-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>, [<span class="st">"SGD"</span>, <span class="st">"Adam"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The hyperparameter <code>optimizer</code> can be de-activated by choosing only one value (level), here: <code>"SGD"</code>.</p>
 <div class="cell" data-execution_count="11">
 <div class="sourceCode cell-code" id="cb18"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb18-1"><a href="#cb18-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>, [<span class="st">"SGD"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<p>As discussed in <a href="#sec-optimizers">Section&nbsp;3.7.4</a>, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in <code>spotPython</code> by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. <code>Rprop</code> was remmoved, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since <code>SparseAdam</code> does not support dense gradients, <code>Adam</code> was used instead. Therefore, there are 10 default optimizers:</p>
+<p>As discussed in <a href="#sec-optimizers">Section&nbsp;3.7.4</a>, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in <code>spotPython</code> by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. <code>Rprop</code> was removed, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since <code>SparseAdam</code> does not support dense gradients, <code>Adam</code> was used instead. Therefore, there are 10 default optimizers:</p>
 <div class="cell" data-execution_count="12">
 <div class="sourceCode cell-code" id="cb19"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb19-1"><a href="#cb19-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>,[<span class="st">"Adadelta"</span>,</span>
 <span id="cb19-2"><a href="#cb19-2" aria-hidden="true" tabindex="-1"></a>     <span class="st">"Adagrad"</span>, <span class="st">"Adam"</span>, <span class="st">"AdamW"</span>, <span class="st">"Adamax"</span>, <span class="st">"ASGD"</span>, <span class="st">"NAdam"</span>, <span class="st">"RAdam"</span>,</span>
 <span id="cb19-3"><a href="#cb19-3" aria-hidden="true" tabindex="-1"></a>      <span class="st">"RMSprop"</span>, <span class="st">"SGD"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="sec-optimizers" class="level3">
 <h3 class="anchored" data-anchor-id="sec-optimizers">Optimizers</h3>
 <p><a href="#tbl-optimizers">Table&nbsp;1</a> shows some of the optimizers available in <code>PyTorch</code>:</p>
 <div id="tbl-optimizers" class="anchored">
 <table class="table">
-<caption>Table&nbsp;1: Optimizers available in PyTorch (selection). “mom” denotes <code>momentum</code>, “weight” <code>weight_decay</code>, “damp” <code>dampening</code>, “nest” <code>nesterov</code>, and “lr_sc” <code>learning rate for scaling delta</code>. The default values are shown in the table.</caption>
+<caption>Table&nbsp;1: Optimizers available in PyTorch (selection). “mom” denotes <code>momentum</code>, “weight” <code>weight_decay</code>, “damp” <code>dampening</code>, “nest” <code>nesterov</code>, “lr_sc” <code>learning rate for scaling delta</code>, “mom_dec” for <code>momentum_decay</code>, and “step_s” for <code>step_sizes</code>. The default values are shown in the table.</caption>
 <colgroup>
-<col style="width: 13%">
-<col style="width: 9%">
-<col style="width: 9%">
-<col style="width: 9%">
-<col style="width: 9%">
-<col style="width: 9%">
-<col style="width: 9%">
-<col style="width: 9%">
 <col style="width: 9%">
-<col style="width: 11%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 6%">
+<col style="width: 7%">
+<col style="width: 7%">
+<col style="width: 7%">
+<col style="width: 7%">
+<col style="width: 6%">
+<col style="width: 6%">
 </colgroup>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Optimizer</th>
 <th style="text-align: left;">lr</th>
 <th style="text-align: left;">mom</th>
 <th style="text-align: left;">weight</th>
 <th style="text-align: left;">damp</th>
 <th style="text-align: left;">nest</th>
 <th style="text-align: left;">rho</th>
 <th style="text-align: left;">lr_sc</th>
 <th style="text-align: left;">lr_decay</th>
 <th style="text-align: left;">betas</th>
+<th style="text-align: left;">lambd</th>
+<th style="text-align: left;">alpha</th>
+<th style="text-align: left;">mom_decay</th>
+<th style="text-align: left;">etas</th>
+<th style="text-align: left;">step_s</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
-<td style="text-align: left;">SGD</td>
-<td style="text-align: left;">required</td>
-<td style="text-align: left;">float: 0</td>
-<td style="text-align: left;">float: 0</td>
-<td style="text-align: left;">float: 0</td>
-<td style="text-align: left;">bool: False</td>
+<td style="text-align: left;">Adadelta</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.9</td>
+<td style="text-align: left;">1.0</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 </tr>
 <tr class="even">
-<td style="text-align: left;">Adadelta</td>
+<td style="text-align: left;">Adagrad</td>
+<td style="text-align: left;">1e-2</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">float: 0</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">float: 0.9</td>
-<td style="text-align: left;">float: 1.0</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 </tr>
 <tr class="odd">
-<td style="text-align: left;">Adagrad</td>
-<td style="text-align: left;">float: 1e-2</td>
+<td style="text-align: left;">Adam</td>
+<td style="text-align: left;">1e-3</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">float: 0</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9,0.999)</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">float: 0</td>
 <td style="text-align: left;">-</td>
 </tr>
 <tr class="even">
-<td style="text-align: left;">Adam</td>
-<td style="text-align: left;">float: 1e-3</td>
+<td style="text-align: left;">AdamW</td>
+<td style="text-align: left;">1e-3</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">1e-2</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">float: 0</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9,0.999)</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">Tuple[float, float]: (0.9, 0.999)</td>
 </tr>
 <tr class="odd">
-<td style="text-align: left;">AdamW</td>
-<td style="text-align: left;">float: 1e-3</td>
+<td style="text-align: left;">SparseAdam</td>
+<td style="text-align: left;">1e-3</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">float: 1e-2</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9,0.999)</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">Tuple[float, float]: (0.9, 0.999)</td>
 </tr>
 <tr class="even">
-<td style="text-align: left;">SparseAdam</td>
-<td style="text-align: left;">float: 1e-3</td>
+<td style="text-align: left;">Adamax</td>
+<td style="text-align: left;">2e-3</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9, 0.999)</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">ASGD</td>
+<td style="text-align: left;">1e-2</td>
+<td style="text-align: left;">0.9</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">False</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">1e-4</td>
+<td style="text-align: left;">0.75</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">LBFGS</td>
+<td style="text-align: left;">1.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">NAdam</td>
+<td style="text-align: left;">2e-3</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9,0.999)</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">RAdam</td>
+<td style="text-align: left;">1e-3</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9,0.999)</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">RMSprop</td>
+<td style="text-align: left;">1e-2</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.9,0.999)</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">Rprop</td>
+<td style="text-align: left;">1e-2</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">(0.5,1.2)</td>
+<td style="text-align: left;">(1e-6, 50)</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">SGD</td>
+<td style="text-align: left;">required</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">0.</td>
+<td style="text-align: left;">False</td>
+<td style="text-align: left;">-</td>
+<td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
 <td style="text-align: left;">-</td>
-<td style="text-align: left;">Tuple[float, float]: (0.9, 0.999)</td>
 </tr>
 </tbody>
 </table>
 </div>
 <p><code>spotPython</code> implements an <code>optimization</code> handler that maps the optimizer names to the corresponding <code>PyTorch</code> optimizers.</p>
 <div class="callout callout-style-default callout-note callout-titled">
 <div class="callout-header d-flex align-content-center">
@@ -665,24 +801,40 @@
 <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container flex-fill">
 A note on LBFGS
 </div>
 </div>
 <div class="callout-body-container callout-body">
-<p><code>PyTorch</code>’s LBFGS optimizer is deactivated in <code>spotPython</code> by default, because it does not perform very well. The <code>PyTorch</code> documentation, see <a href="https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS">https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS</a>, states:</p>
+<p>We recommend deactivating <code>PyTorch</code>’s LBFGS optimizer, because it does not perform very well. The <code>PyTorch</code> documentation, see <a href="https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS">https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS</a>, states:</p>
 <blockquote class="blockquote">
 <p>This is a very memory intensive optimizer (it requires additional <code>param_bytes * (history_size + 1)</code> bytes). If it doesn’t fit in memory try reducing the history size, or use a different algorithm.</p>
 </blockquote>
 <p>Furthermore, the LBFGS optimizer is not compatible with the <code>PyTorch</code> tutorial. The reason is that the LBFGS optimizer requires the <code>closure</code> function, which is not implemented in the <code>PyTorch</code> tutorial. Therefore, the <code>LBFGS</code> optimizer is recommended here.</p>
 </div>
 </div>
-<p>Since there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only. Thus, the learning rate, which affects the <code>SGD</code> optimizer, will be set to a fixed value. We choose the default value of <code>1e-3</code> for the learning rate, because it is used in other <code>PyTorch</code> examples. We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.</p>
+<p>Since there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only.</p>
+<div class="callout callout-style-default callout-note callout-titled">
+<div class="callout-header d-flex align-content-center">
+<div class="callout-icon-container">
+<i class="callout-icon"></i>
+</div>
+<div class="callout-title-container flex-fill">
+A note on the learning rate
+</div>
+</div>
+<div class="callout-body-container callout-body">
+<p><code>spotPython</code> provides a multiplier for the default learning rates, because optimizers use different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore, we recommend fixing the learning rate for all optimizers if multiple optimizers are used. This can be done by setting the lower and upper bounds of the learning rate multiplier to the same value as shown below.</p>
+</div>
+</div>
+<p>Thus, the learning rate, which affects the <code>SGD</code> optimizer, will be set to a fixed value. We choose the default value of <code>1e-3</code> for the learning rate, because it is used in other <code>PyTorch</code> examples (it is also the default value used by <code>spotPython</code> as defined in the <code>optimizer_handler()</code> method). We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.</p>
+<p>For the same reason, we will fix the <code>sgd_momentum</code> to <code>0.9</code>.</p>
 <div class="cell" data-execution_count="13">
-<div class="sourceCode cell-code" id="cb20"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb20-1"><a href="#cb20-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"lr"</span>, bounds<span class="op">=</span>[<span class="fl">1e-3</span>, <span class="fl">1e-3</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb20"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb20-1"><a href="#cb20-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"lr_mult"</span>, bounds<span class="op">=</span>[<span class="fl">1.0</span>, <span class="fl">1.0</span>])</span>
+<span id="cb20-2"><a href="#cb20-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"sgd_momentum"</span>, bounds<span class="op">=</span>[<span class="fl">0.9</span>, <span class="fl">0.9</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 </section>
 <section id="sec-selection-of-target-function" class="level2">
 <h2 class="anchored" data-anchor-id="sec-selection-of-target-function">Evaluation</h2>
 <p>The evaluation procedure requires the specification of two elements:</p>
 <ol type="1">
@@ -707,19 +859,19 @@
 <div class="callout-body-container callout-body">
 <p><code>spotPython</code> returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.</p>
 <p>Summarizing, the following splits are performed in the hold-out setting:</p>
 <ol type="1">
 <li>Run <code>spotPython</code> with <code>eval</code> set to <code>train_hold_out</code> to determine the best hyperparameter configuration.</li>
 <li>Train the model with the best hyperparameter configuration on the training data set:
 <ul>
-<li><code>train_save(model_spot, train, "model_spot.pt")</code>.</li>
+<li><code>train_tuned(model_spot, train, "model_spot.pt")</code>.</li>
 </ul></li>
 <li>Test the model on the test data:
 <ul>
-<li><code>test_saved(model_spot, test, "model_spot.pt")</code></li>
+<li><code>test_tuned(model_spot, test, "model_spot.pt")</code></li>
 </ul></li>
 </ol>
 <p>These steps will be exemplified in the following sections.</p>
 </div>
 </div>
 <p>In addition to this <code>hold-out</code> setting, <code>spotPython</code> provides another hold-out setting, where an explicit test data is specified by the user that will be used as the validation set. To choose this option, the <code>eval</code> parameter is set to <code>test_hold_out</code>. In this case, the training data set is used for the model training. Then, the explicitly defined test data set is used for the evaluation of the hyperparameter configuration (the validation).</p>
 </section>
@@ -732,68 +884,425 @@
 <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container flex-fill">
 Note
 </div>
 </div>
 <div class="callout-body-container callout-body">
-<p>Combinations of the above settings are possible, e.g., cross validation can be used for training and hold-out for evaluation or . Also, cross validation can be used for training and testing. Because cross validation is not used in the <code>PyTorch</code> tutorial <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span>, it is not considered further here.</p>
+<p>Combinations of the above settings are possible, e.g., cross validation can be used for training and hold-out for evaluation or <em>vice versa</em>. Also, cross validation can be used for training and testing. Because cross validation is not used in the <code>PyTorch</code> tutorial <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span>, it is not considered further here.</p>
 </div>
 </div>
 </section>
+<section id="overview-of-the-evaluation-settings" class="level4">
+<h4 class="anchored" data-anchor-id="overview-of-the-evaluation-settings">Overview of the Evaluation Settings</h4>
+<section id="settings-for-the-hyperparameter-tuning" class="level5">
+<h5 class="anchored" data-anchor-id="settings-for-the-hyperparameter-tuning">Settings for the Hyperparameter Tuning</h5>
+<p><a href="#tbl-eval-settings">Table&nbsp;2</a> provides an overview of the training evaluations.</p>
+<div id="tbl-eval-settings" class="anchored">
+<table class="table">
+<caption>Table&nbsp;2: Overview of the evaluation settings.</caption>
+<colgroup>
+<col style="width: 15%">
+<col style="width: 26%">
+<col style="width: 26%">
+<col style="width: 15%">
+<col style="width: 15%">
+</colgroup>
+<thead>
+<tr class="header">
+<th><code>eval</code></th>
+<th style="text-align: center;"><code>train</code></th>
+<th style="text-align: center;"><code>test</code></th>
+<th>function</th>
+<th>comment</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td><code>"train_hold_out"</code></td>
+<td style="text-align: center;"><span class="math inline">\(\checkmark\)</span></td>
+<td style="text-align: center;"></td>
+<td><code>train_hold_out()</code>, <code>validate_fold_or_hold_out()</code> for early stopping</td>
+<td>splits the <code>train</code> data set internally</td>
+</tr>
+<tr class="even">
+<td><code>"test_hold_out"</code></td>
+<td style="text-align: center;"><span class="math inline">\(\checkmark\)</span></td>
+<td style="text-align: center;"><span class="math inline">\(\checkmark\)</span></td>
+<td><code>train_hold_out()</code>, <code>validate_fold_or_hold_out()</code> for early stopping</td>
+<td>use the <code>test data set</code> for <code>validate_fold_or_hold_out()</code></td>
+</tr>
+<tr class="odd">
+<td><code>"train_cv"</code></td>
+<td style="text-align: center;"><span class="math inline">\(\checkmark\)</span></td>
+<td style="text-align: center;"></td>
+<td><code>evaluate_cv(net, train)</code></td>
+<td>CV using the <code>train</code> data set</td>
+</tr>
+<tr class="even">
+<td><code>"test_cv"</code></td>
+<td style="text-align: center;"></td>
+<td style="text-align: center;"><span class="math inline">\(\checkmark\)</span></td>
+<td><code>evaluate_cv(net, test)</code></td>
+<td>CV using the <code>test</code> data set . Identical to <code>"train_cv"</code>, uses only test data.</td>
+</tr>
+</tbody>
+</table>
+</div>
+<ul>
+<li><code>"train_cv"</code> and <code>"test_cv"</code> use <code>sklearn.model_selection.KFold()</code> internally.</li>
+</ul>
 </section>
-<section id="loss-functions-and-metrics" class="level3">
-<h3 class="anchored" data-anchor-id="loss-functions-and-metrics">Loss Functions and Metrics</h3>
-<p>The key <code>"criterion"</code> specifies the loss function which is used during the optimization. There are several different loss functions under <code>PyTorch</code>’s <code>nn</code> package. For example, a simple loss is <code>MSELoss</code>, which computes the mean-squared error between the output and the target. In this tutorial we will use <code>CrossEntropyLoss</code>, because it is also used in the <code>PyTorch</code> tutorial.</p>
+</section>
+<section id="detailed-description-of-the-train_hold_out-setting" class="level4">
+<h4 class="anchored" data-anchor-id="detailed-description-of-the-train_hold_out-setting">Detailed Description of the <code>"train_hold_out"</code> Setting</h4>
+<p>The <code>"train_hold_out"</code> setting is used by default. It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_hold_out()</code> as follows:</li>
+</ol>
 <div class="cell" data-execution_count="14">
-<div class="sourceCode cell-code" id="cb21"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb21-1"><a href="#cb21-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"criterion"</span>, [<span class="st">"CrossEntropyLoss"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb21"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb21-1"><a href="#cb21-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_hold_out(</span>
+<span id="cb21-2"><a href="#cb21-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
+<span id="cb21-3"><a href="#cb21-3" aria-hidden="true" tabindex="-1"></a>    train_dataset<span class="op">=</span>fun_control[<span class="st">"train"</span>],</span>
+<span id="cb21-4"><a href="#cb21-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
+<span id="cb21-5"><a href="#cb21-5" aria-hidden="true" tabindex="-1"></a>    loss_function<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb21-6"><a href="#cb21-6" aria-hidden="true" tabindex="-1"></a>    metric<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb21-7"><a href="#cb21-7" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
+<span id="cb21-8"><a href="#cb21-8" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
+<span id="cb21-9"><a href="#cb21-9" aria-hidden="true" tabindex="-1"></a>    path<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"path"</span>],</span>
+<span id="cb21-10"><a href="#cb21-10" aria-hidden="true" tabindex="-1"></a>) </span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<p>In addition to the loss functions, <code>spotPython</code> provides access to a large number of metrics. The key <code>"metric_sklearn"</code> is used for metrics that follow the <code>scikit-learn</code> conventions<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>. Because the <code>PyTorch</code> tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial’s example code. Therefore, we will use the same implementation here and set the key <code>"metric_sklearn"</code> to <code>None</code>.</p>
+<p>Note: Only the data set <code>fun_control["train"]</code> is used for training and validation. It is used as follows:</p>
 <div class="cell" data-execution_count="15">
-<div class="sourceCode cell-code" id="cb22"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb22-1"><a href="#cb22-1" aria-hidden="true" tabindex="-1"></a>weights <span class="op">=</span> <span class="fl">1.0</span></span>
-<span id="cb22-2"><a href="#cb22-2" aria-hidden="true" tabindex="-1"></a>criterion <span class="op">=</span> CrossEntropyLoss</span>
-<span id="cb22-3"><a href="#cb22-3" aria-hidden="true" tabindex="-1"></a>shuffle <span class="op">=</span> <span class="va">True</span></span>
-<span id="cb22-4"><a href="#cb22-4" aria-hidden="true" tabindex="-1"></a><span class="bu">eval</span> <span class="op">=</span> <span class="st">"train_hold_out"</span></span>
-<span id="cb22-5"><a href="#cb22-5" aria-hidden="true" tabindex="-1"></a>device <span class="op">=</span> DEVICE</span>
-<span id="cb22-6"><a href="#cb22-6" aria-hidden="true" tabindex="-1"></a>show_batch_interval <span class="op">=</span> <span class="dv">100_000</span></span>
-<span id="cb22-7"><a href="#cb22-7" aria-hidden="true" tabindex="-1"></a>save_model <span class="op">=</span> <span class="va">True</span></span>
-<span id="cb22-8"><a href="#cb22-8" aria-hidden="true" tabindex="-1"></a>path<span class="op">=</span><span class="st">"torch_model.pt"</span></span>
-<span id="cb22-9"><a href="#cb22-9" aria-hidden="true" tabindex="-1"></a></span>
-<span id="cb22-10"><a href="#cb22-10" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
-<span id="cb22-11"><a href="#cb22-11" aria-hidden="true" tabindex="-1"></a>               <span class="st">"data_dir"</span>: <span class="va">None</span>,</span>
-<span id="cb22-12"><a href="#cb22-12" aria-hidden="true" tabindex="-1"></a>               <span class="st">"checkpoint_dir"</span>: <span class="va">None</span>,</span>
-<span id="cb22-13"><a href="#cb22-13" aria-hidden="true" tabindex="-1"></a>               <span class="st">"horizon"</span>: <span class="va">None</span>,</span>
-<span id="cb22-14"><a href="#cb22-14" aria-hidden="true" tabindex="-1"></a>               <span class="st">"oml_grace_period"</span>: <span class="va">None</span>,</span>
-<span id="cb22-15"><a href="#cb22-15" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weights"</span>: weights,</span>
-<span id="cb22-16"><a href="#cb22-16" aria-hidden="true" tabindex="-1"></a>               <span class="st">"step"</span>: <span class="va">None</span>,</span>
-<span id="cb22-17"><a href="#cb22-17" aria-hidden="true" tabindex="-1"></a>               <span class="st">"log_level"</span>: <span class="dv">50</span>,</span>
-<span id="cb22-18"><a href="#cb22-18" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weight_coeff"</span>: <span class="va">None</span>,</span>
-<span id="cb22-19"><a href="#cb22-19" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric"</span>: <span class="va">None</span>,</span>
-<span id="cb22-20"><a href="#cb22-20" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_sklearn"</span>: <span class="va">None</span>,</span>
-<span id="cb22-21"><a href="#cb22-21" aria-hidden="true" tabindex="-1"></a>               <span class="st">"criterion"</span>: criterion,</span>
-<span id="cb22-22"><a href="#cb22-22" aria-hidden="true" tabindex="-1"></a>               <span class="st">"shuffle"</span>: shuffle,</span>
-<span id="cb22-23"><a href="#cb22-23" aria-hidden="true" tabindex="-1"></a>               <span class="st">"eval"</span>: <span class="bu">eval</span>,</span>
-<span id="cb22-24"><a href="#cb22-24" aria-hidden="true" tabindex="-1"></a>               <span class="st">"device"</span>: device,</span>
-<span id="cb22-25"><a href="#cb22-25" aria-hidden="true" tabindex="-1"></a>               <span class="st">"show_batch_interval"</span>: show_batch_interval,</span>
-<span id="cb22-26"><a href="#cb22-26" aria-hidden="true" tabindex="-1"></a>               <span class="st">"save_model"</span>: save_model,</span>
-<span id="cb22-27"><a href="#cb22-27" aria-hidden="true" tabindex="-1"></a>               <span class="st">"path"</span>: path,</span>
-<span id="cb22-28"><a href="#cb22-28" aria-hidden="true" tabindex="-1"></a>               })</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb22"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb22-1"><a href="#cb22-1" aria-hidden="true" tabindex="-1"></a>trainloader, valloader <span class="op">=</span> create_train_val_data_loaders(</span>
+<span id="cb22-2"><a href="#cb22-2" aria-hidden="true" tabindex="-1"></a>                dataset<span class="op">=</span>train_dataset, batch_size<span class="op">=</span>batch_size_instance, shuffle<span class="op">=</span>shuffle</span>
+<span id="cb22-3"><a href="#cb22-3" aria-hidden="true" tabindex="-1"></a>            )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p><code>create_train_val_data_loaders()</code> splits the <code>train_dataset</code> into <code>trainloader</code> and <code>valloader</code> using <code>torch.utils.data.random_split()</code> as follows:</p>
+<div class="cell" data-execution_count="16">
+<div class="sourceCode cell-code" id="cb23"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb23-1"><a href="#cb23-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers<span class="op">=</span><span class="dv">0</span>):</span>
+<span id="cb23-2"><a href="#cb23-2" aria-hidden="true" tabindex="-1"></a>    test_abs <span class="op">=</span> <span class="bu">int</span>(<span class="bu">len</span>(dataset) <span class="op">*</span> <span class="fl">0.6</span>)</span>
+<span id="cb23-3"><a href="#cb23-3" aria-hidden="true" tabindex="-1"></a>    train_subset, val_subset <span class="op">=</span> random_split(dataset, [test_abs, <span class="bu">len</span>(dataset) <span class="op">-</span> test_abs])</span>
+<span id="cb23-4"><a href="#cb23-4" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb23-5"><a href="#cb23-5" aria-hidden="true" tabindex="-1"></a>        train_subset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb23-6"><a href="#cb23-6" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb23-7"><a href="#cb23-7" aria-hidden="true" tabindex="-1"></a>    valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb23-8"><a href="#cb23-8" aria-hidden="true" tabindex="-1"></a>        val_subset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb23-9"><a href="#cb23-9" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb23-10"><a href="#cb23-10" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainloader, valloader</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>The optimizer is set up as follows:</p>
+<div class="cell" data-execution_count="17">
+<div class="sourceCode cell-code" id="cb24"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb24-1"><a href="#cb24-1" aria-hidden="true" tabindex="-1"></a>lr_mult_instance <span class="op">=</span> net.lr_mult</span>
+<span id="cb24-2"><a href="#cb24-2" aria-hidden="true" tabindex="-1"></a>optimizer <span class="op">=</span> optimizer_handler(optimizer_name<span class="op">=</span>optimizer_instance, params<span class="op">=</span>net.parameters(), lr_mult<span class="op">=</span>lr_mult_instance)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="3" type="1">
+<li><code>evaluate_hold_out()</code> sets the <code>net</code> attributes such as <code>epochs</code>, <code>batch_size</code>, <code>optimizer</code>, and <code>patience</code>. For each epoch, the methods <code>train_hold_out()</code> and <code>validate_fold_or_hold_out()</code> are called, the former for training and the latter for validation and early stopping. The validation loss from the last epoch (not the best validation loss) is returned from <code>evaluate_hold_out</code>.</li>
+<li>The method <code>train_hold_out()</code> is implemented as follows:</li>
+</ol>
+<div class="cell" data-execution_count="18">
+<div class="sourceCode cell-code" id="cb25"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb25-1"><a href="#cb25-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>):</span>
+<span id="cb25-2"><a href="#cb25-2" aria-hidden="true" tabindex="-1"></a>    running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb25-3"><a href="#cb25-3" aria-hidden="true" tabindex="-1"></a>    epoch_steps <span class="op">=</span> <span class="dv">0</span></span>
+<span id="cb25-4"><a href="#cb25-4" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(trainloader, <span class="dv">0</span>):</span>
+<span id="cb25-5"><a href="#cb25-5" aria-hidden="true" tabindex="-1"></a>        inputs, labels <span class="op">=</span> data</span>
+<span id="cb25-6"><a href="#cb25-6" aria-hidden="true" tabindex="-1"></a>        inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
+<span id="cb25-7"><a href="#cb25-7" aria-hidden="true" tabindex="-1"></a>        optimizer.zero_grad()</span>
+<span id="cb25-8"><a href="#cb25-8" aria-hidden="true" tabindex="-1"></a>        outputs <span class="op">=</span> net(inputs)</span>
+<span id="cb25-9"><a href="#cb25-9" aria-hidden="true" tabindex="-1"></a>        loss <span class="op">=</span> loss_function(outputs, labels)</span>
+<span id="cb25-10"><a href="#cb25-10" aria-hidden="true" tabindex="-1"></a>        loss.backward()</span>
+<span id="cb25-11"><a href="#cb25-11" aria-hidden="true" tabindex="-1"></a>        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm<span class="op">=</span><span class="fl">1.0</span>)</span>
+<span id="cb25-12"><a href="#cb25-12" aria-hidden="true" tabindex="-1"></a>        optimizer.step()</span>
+<span id="cb25-13"><a href="#cb25-13" aria-hidden="true" tabindex="-1"></a>        running_loss <span class="op">+=</span> loss.item()</span>
+<span id="cb25-14"><a href="#cb25-14" aria-hidden="true" tabindex="-1"></a>        epoch_steps <span class="op">+=</span> <span class="dv">1</span></span>
+<span id="cb25-15"><a href="#cb25-15" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> i <span class="op">%</span> show_batch_interval <span class="op">==</span> (show_batch_interval <span class="op">-</span> <span class="dv">1</span>):  <span class="co"># print every show_batch_interval mini-batches</span></span>
+<span id="cb25-16"><a href="#cb25-16" aria-hidden="true" tabindex="-1"></a>            <span class="bu">print</span>(</span>
+<span id="cb25-17"><a href="#cb25-17" aria-hidden="true" tabindex="-1"></a>                <span class="st">"Batch: </span><span class="sc">%5d</span><span class="st">. Batch Size: </span><span class="sc">%d</span><span class="st">. Training Loss (running): </span><span class="sc">%.3f</span><span class="st">"</span></span>
+<span id="cb25-18"><a href="#cb25-18" aria-hidden="true" tabindex="-1"></a>                <span class="op">%</span> (i <span class="op">+</span> <span class="dv">1</span>, <span class="bu">int</span>(batch_size), running_loss <span class="op">/</span> epoch_steps)</span>
+<span id="cb25-19"><a href="#cb25-19" aria-hidden="true" tabindex="-1"></a>            )</span>
+<span id="cb25-20"><a href="#cb25-20" aria-hidden="true" tabindex="-1"></a>            running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb25-21"><a href="#cb25-21" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> loss.item()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="5" type="1">
+<li>The method <code>validate_fold_or_hold_out()</code> is implemented as follows:</li>
+</ol>
+<div class="cell" data-execution_count="19">
+<div class="sourceCode cell-code" id="cb26"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb26-1"><a href="#cb26-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> validate_fold_or_hold_out(net, valloader, loss_function, metric, device):</span>
+<span id="cb26-2"><a href="#cb26-2" aria-hidden="true" tabindex="-1"></a>    val_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb26-3"><a href="#cb26-3" aria-hidden="true" tabindex="-1"></a>    val_steps <span class="op">=</span> <span class="dv">0</span></span>
+<span id="cb26-4"><a href="#cb26-4" aria-hidden="true" tabindex="-1"></a>    metric.reset()</span>
+<span id="cb26-5"><a href="#cb26-5" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(valloader, <span class="dv">0</span>):</span>
+<span id="cb26-6"><a href="#cb26-6" aria-hidden="true" tabindex="-1"></a>        <span class="cf">with</span> torch.no_grad():</span>
+<span id="cb26-7"><a href="#cb26-7" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> data</span>
+<span id="cb26-8"><a href="#cb26-8" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
+<span id="cb26-9"><a href="#cb26-9" aria-hidden="true" tabindex="-1"></a>            outputs <span class="op">=</span> net(inputs)</span>
+<span id="cb26-10"><a href="#cb26-10" aria-hidden="true" tabindex="-1"></a>            _, predicted <span class="op">=</span> torch.<span class="bu">max</span>(outputs.data, <span class="dv">1</span>)</span>
+<span id="cb26-11"><a href="#cb26-11" aria-hidden="true" tabindex="-1"></a>            metric_value <span class="op">=</span> metric(predicted, labels).to(device)</span>
+<span id="cb26-12"><a href="#cb26-12" aria-hidden="true" tabindex="-1"></a>            loss <span class="op">=</span> loss_function(outputs, labels)</span>
+<span id="cb26-13"><a href="#cb26-13" aria-hidden="true" tabindex="-1"></a>            val_loss <span class="op">+=</span> loss.cpu().numpy()</span>
+<span id="cb26-14"><a href="#cb26-14" aria-hidden="true" tabindex="-1"></a>            val_steps <span class="op">+=</span> <span class="dv">1</span></span>
+<span id="cb26-15"><a href="#cb26-15" aria-hidden="true" tabindex="-1"></a>    loss <span class="op">=</span> val_loss <span class="op">/</span> val_steps</span>
+<span id="cb26-16"><a href="#cb26-16" aria-hidden="true" tabindex="-1"></a>    metric_value <span class="op">=</span> metric.compute()</span>
+<span id="cb26-17"><a href="#cb26-17" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> metric_value, loss</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+</section>
+<section id="detailed-description-of-the-test_hold_out-setting" class="level4">
+<h4 class="anchored" data-anchor-id="detailed-description-of-the-test_hold_out-setting">Detailed Description of the <code>"test_hold_out"</code> Setting</h4>
+<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_hold_out()</code> similar to the <code>"train_hold_out"</code> setting with one exception: It passes an additional <code>test</code> data set to <code>evaluate_hold_out()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="20">
+<div class="sourceCode cell-code" id="cb27"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb27-1"><a href="#cb27-1" aria-hidden="true" tabindex="-1"></a>test_dataset<span class="op">=</span>fun_control[<span class="st">"test"</span>]</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p><code>evaluate_hold_out()</code> calls <code>create_train_test_data_loaders</code> instead of <code>create_train_val_data_loaders</code> as follows: The two data sets are used in <code>create_train_test_data_loaders</code> as follows:</p>
+<div class="cell" data-execution_count="21">
+<div class="sourceCode cell-code" id="cb28"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb28-1"><a href="#cb28-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers<span class="op">=</span><span class="dv">0</span>):</span>
+<span id="cb28-2"><a href="#cb28-2" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb28-3"><a href="#cb28-3" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb28-4"><a href="#cb28-4" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb28-5"><a href="#cb28-5" aria-hidden="true" tabindex="-1"></a>    testloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb28-6"><a href="#cb28-6" aria-hidden="true" tabindex="-1"></a>        test_dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb28-7"><a href="#cb28-7" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb28-8"><a href="#cb28-8" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainloader, testloader</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="3" type="1">
+<li>The following steps are identical to the <code>"train_hold_out"</code> setting. Only a different data loader is used for testing.</li>
+</ol>
+</section>
+<section id="detailed-description-of-the-train_cv-setting" class="level4">
+<h4 class="anchored" data-anchor-id="detailed-description-of-the-train_cv-setting">Detailed Description of the <code>"train_cv"</code> Setting</h4>
+<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_cv()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="22">
+<div class="sourceCode cell-code" id="cb29"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb29-1"><a href="#cb29-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_cv(</span>
+<span id="cb29-2"><a href="#cb29-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
+<span id="cb29-3"><a href="#cb29-3" aria-hidden="true" tabindex="-1"></a>    dataset<span class="op">=</span>fun_control[<span class="st">"train"</span>],</span>
+<span id="cb29-4"><a href="#cb29-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
+<span id="cb29-5"><a href="#cb29-5" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
+<span id="cb29-6"><a href="#cb29-6" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
+<span id="cb29-7"><a href="#cb29-7" aria-hidden="true" tabindex="-1"></a>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>Note: Only the data set <code>fun_control["train"]</code> is used for CV. 3. In `evaluate_cv(), the following steps are performed: The optimizer is set up as follows:</p>
+<div class="cell" data-execution_count="23">
+<div class="sourceCode cell-code" id="cb30"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb30-1"><a href="#cb30-1" aria-hidden="true" tabindex="-1"></a>lr_instance <span class="op">=</span> net.lr</span>
+<span id="cb30-2"><a href="#cb30-2" aria-hidden="true" tabindex="-1"></a>optimizer <span class="op">=</span> optimizer_handler(optimizer_name<span class="op">=</span>optimizer_instance, params<span class="op">=</span>net.parameters(), lr_mult<span class="op">=</span>lr_mult_instance)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p><code>evaluate_cv()</code> sets the <code>net</code> attributes such as <code>epochs</code>, <code>batch_size</code>, <code>optimizer</code>, and <code>patience</code>. CV is implemented as follows:</p>
+<div class="cell" data-execution_count="24">
+<div class="sourceCode cell-code" id="cb31"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb31-1"><a href="#cb31-1" aria-hidden="true" tabindex="-1"></a>kfold <span class="op">=</span> KFold(n_splits<span class="op">=</span>k_folds_instance, shuffle<span class="op">=</span>shuffle)</span>
+<span id="cb31-2"><a href="#cb31-2" aria-hidden="true" tabindex="-1"></a><span class="cf">for</span> fold, (train_ids, val_ids) <span class="kw">in</span> <span class="bu">enumerate</span>(kfold.split(dataset)):</span>
+<span id="cb31-3"><a href="#cb31-3" aria-hidden="true" tabindex="-1"></a>    train_subsampler <span class="op">=</span> torch.utils.data.SubsetRandomSampler(train_ids)</span>
+<span id="cb31-4"><a href="#cb31-4" aria-hidden="true" tabindex="-1"></a>    val_subsampler <span class="op">=</span> torch.utils.data.SubsetRandomSampler(val_ids)</span>
+<span id="cb31-5"><a href="#cb31-5" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb31-6"><a href="#cb31-6" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span>batch_size_instance, sampler<span class="op">=</span>train_subsampler, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb31-7"><a href="#cb31-7" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb31-8"><a href="#cb31-8" aria-hidden="true" tabindex="-1"></a>    valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb31-9"><a href="#cb31-9" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span>batch_size_instance, sampler<span class="op">=</span>val_subsampler, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb31-10"><a href="#cb31-10" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb31-11"><a href="#cb31-11" aria-hidden="true" tabindex="-1"></a>    reset_weights(net)</span>
+<span id="cb31-12"><a href="#cb31-12" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Train fold for several epochs:</span></span>
+<span id="cb31-13"><a href="#cb31-13" aria-hidden="true" tabindex="-1"></a>    train_fold(</span>
+<span id="cb31-14"><a href="#cb31-14" aria-hidden="true" tabindex="-1"></a>        net,</span>
+<span id="cb31-15"><a href="#cb31-15" aria-hidden="true" tabindex="-1"></a>        trainloader,</span>
+<span id="cb31-16"><a href="#cb31-16" aria-hidden="true" tabindex="-1"></a>        epochs_instance,</span>
+<span id="cb31-17"><a href="#cb31-17" aria-hidden="true" tabindex="-1"></a>        loss_function,</span>
+<span id="cb31-18"><a href="#cb31-18" aria-hidden="true" tabindex="-1"></a>        optimizer,</span>
+<span id="cb31-19"><a href="#cb31-19" aria-hidden="true" tabindex="-1"></a>        device,</span>
+<span id="cb31-20"><a href="#cb31-20" aria-hidden="true" tabindex="-1"></a>        show_batch_interval<span class="op">=</span>show_batch_interval,</span>
+<span id="cb31-21"><a href="#cb31-21" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb31-22"><a href="#cb31-22" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Validate fold: use only loss for tuning</span></span>
+<span id="cb31-23"><a href="#cb31-23" aria-hidden="true" tabindex="-1"></a>    metric_values[fold], loss_values[fold] <span class="op">=</span> validate_fold_or_hold_out(net, valloader, loss_function, device)</span>
+<span id="cb31-24"><a href="#cb31-24" aria-hidden="true" tabindex="-1"></a>df_eval <span class="op">=</span> <span class="bu">sum</span>(loss_values.values()) <span class="op">/</span> <span class="bu">len</span>(loss_values.values())</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="4" type="1">
+<li>The method <code>train_fold()</code> is implemented as follows:</li>
+</ol>
+<div class="cell" data-execution_count="25">
+<div class="sourceCode cell-code" id="cb32"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb32-1"><a href="#cb32-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>):</span>
+<span id="cb32-2"><a href="#cb32-2" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> epoch <span class="kw">in</span> <span class="bu">range</span>(epochs):</span>
+<span id="cb32-3"><a href="#cb32-3" aria-hidden="true" tabindex="-1"></a>        <span class="bu">print</span>(<span class="ss">f"Epoch: </span><span class="sc">{</span>epoch <span class="op">+</span> <span class="dv">1</span><span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb32-4"><a href="#cb32-4" aria-hidden="true" tabindex="-1"></a>        running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb32-5"><a href="#cb32-5" aria-hidden="true" tabindex="-1"></a>        epoch_steps <span class="op">=</span> <span class="dv">0</span></span>
+<span id="cb32-6"><a href="#cb32-6" aria-hidden="true" tabindex="-1"></a>        <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(trainloader, <span class="dv">0</span>):</span>
+<span id="cb32-7"><a href="#cb32-7" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> data</span>
+<span id="cb32-8"><a href="#cb32-8" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
+<span id="cb32-9"><a href="#cb32-9" aria-hidden="true" tabindex="-1"></a>            optimizer.zero_grad()</span>
+<span id="cb32-10"><a href="#cb32-10" aria-hidden="true" tabindex="-1"></a>            outputs <span class="op">=</span> net(inputs)</span>
+<span id="cb32-11"><a href="#cb32-11" aria-hidden="true" tabindex="-1"></a>            loss <span class="op">=</span> loss_function(outputs, labels)</span>
+<span id="cb32-12"><a href="#cb32-12" aria-hidden="true" tabindex="-1"></a>            loss.backward()</span>
+<span id="cb32-13"><a href="#cb32-13" aria-hidden="true" tabindex="-1"></a>            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm<span class="op">=</span><span class="fl">1.0</span>)</span>
+<span id="cb32-14"><a href="#cb32-14" aria-hidden="true" tabindex="-1"></a>            optimizer.step()</span>
+<span id="cb32-15"><a href="#cb32-15" aria-hidden="true" tabindex="-1"></a>            <span class="co"># the following is for printing the statistic only</span></span>
+<span id="cb32-16"><a href="#cb32-16" aria-hidden="true" tabindex="-1"></a>            running_loss <span class="op">+=</span> loss.item()</span>
+<span id="cb32-17"><a href="#cb32-17" aria-hidden="true" tabindex="-1"></a>            epoch_steps <span class="op">+=</span> <span class="dv">1</span></span>
+<span id="cb32-18"><a href="#cb32-18" aria-hidden="true" tabindex="-1"></a>            <span class="cf">if</span> i <span class="op">%</span> show_batch_interval <span class="op">==</span> (show_batch_interval <span class="op">-</span> <span class="dv">1</span>):  <span class="co"># print every show_batch_interval mini-batches</span></span>
+<span id="cb32-19"><a href="#cb32-19" aria-hidden="true" tabindex="-1"></a>                <span class="bu">print</span>(<span class="st">"Batch: </span><span class="sc">%5d</span><span class="st">. Training Loss (running): </span><span class="sc">%.3f</span><span class="st">"</span> <span class="op">%</span> (i <span class="op">+</span> <span class="dv">1</span>, running_loss <span class="op">/</span> epoch_steps))</span>
+<span id="cb32-20"><a href="#cb32-20" aria-hidden="true" tabindex="-1"></a>                running_loss <span class="op">=</span> <span class="fl">0.0</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="5" type="1">
+<li>The method <code>validate_fold_or_hold_out()</code> is implemented as shown above. In contrast to the hold-out setting, it is called for each of the <span class="math inline">\(k\)</span> folds. The results are stored in a dictionaries <code>metric_values</code> and <code>loss_values</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="26">
+<div class="sourceCode cell-code" id="cb33"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb33-1"><a href="#cb33-1" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Validate fold: use only loss for tuning</span></span>
+<span id="cb33-2"><a href="#cb33-2" aria-hidden="true" tabindex="-1"></a>    metric_values[fold], loss_values[fold] <span class="op">=</span> validate_fold_or_hold_out(net, valloader, loss_function, device)</span>
+<span id="cb33-3"><a href="#cb33-3" aria-hidden="true" tabindex="-1"></a>df_eval <span class="op">=</span> <span class="bu">sum</span>(loss_values.values()) <span class="op">/</span> <span class="bu">len</span>(loss_values.values())</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>The results are averaged over the <span class="math inline">\(k\)</span> folds and returned as <code>df_eval</code>.</p>
+</section>
+<section id="detailed-description-of-the-test_cv-setting" class="level4">
+<h4 class="anchored" data-anchor-id="detailed-description-of-the-test_cv-setting">Detailed Description of the <code>"test_cv"</code> Setting</h4>
+<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_cv()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="27">
+<div class="sourceCode cell-code" id="cb34"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb34-1"><a href="#cb34-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_cv(</span>
+<span id="cb34-2"><a href="#cb34-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
+<span id="cb34-3"><a href="#cb34-3" aria-hidden="true" tabindex="-1"></a>    dataset<span class="op">=</span>fun_control[<span class="st">"test"</span>],</span>
+<span id="cb34-4"><a href="#cb34-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
+<span id="cb34-5"><a href="#cb34-5" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
+<span id="cb34-6"><a href="#cb34-6" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
+<span id="cb34-7"><a href="#cb34-7" aria-hidden="true" tabindex="-1"></a>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>Note: The data set <code>fun_control["test"]</code> is used for CV. The rest is the same as for the <code>"train_cv"</code> setting.</p>
+</section>
+<section id="settings-for-the-final-evaluation-of-the-tuned-architecture" class="level4">
+<h4 class="anchored" data-anchor-id="settings-for-the-final-evaluation-of-the-tuned-architecture">Settings for the Final Evaluation of the Tuned Architecture</h4>
+<section id="training-of-the-tuned-architecture" class="level5">
+<h5 class="anchored" data-anchor-id="training-of-the-tuned-architecture">Training of the Tuned Architecture</h5>
+<p><code>train_tuned(model, train)</code>: train the model with the best hyperparameter configuration (or simply the default) on the training data set. It splits the <code>train</code>data into new <code>train</code> and <code>validation</code> sets using <code>create_train_val_data_loaders()</code>, which calls <code>torch.utils.data.random_split()</code> internally. Currently, 60% of the data is used for training and 40% for validation. The <code>train</code> data is used for training the model with <code>train_hold_out()</code>. The <code>validation</code> data is used for early stopping using <code>validate_fold_or_hold_out()</code> on the <code>validation</code> data set.</p>
+<p><code>train_tuned()</code> is just a wrapper to <code>evaluate_hold_out</code> using the <code>train</code> data set. It is implemented as follows:</p>
+<div class="cell" data-execution_count="28">
+<div class="sourceCode cell-code" id="cb35"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb35-1"><a href="#cb35-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_tuned(net, train_dataset, shuffle, loss_function, metric, device<span class="op">=</span><span class="va">None</span>, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>, path<span class="op">=</span><span class="va">None</span>):</span>
+<span id="cb35-2"><a href="#cb35-2" aria-hidden="true" tabindex="-1"></a>    evaluate_hold_out(</span>
+<span id="cb35-3"><a href="#cb35-3" aria-hidden="true" tabindex="-1"></a>        net<span class="op">=</span>net,</span>
+<span id="cb35-4"><a href="#cb35-4" aria-hidden="true" tabindex="-1"></a>        train_dataset<span class="op">=</span>train_dataset,</span>
+<span id="cb35-5"><a href="#cb35-5" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span>shuffle,</span>
+<span id="cb35-6"><a href="#cb35-6" aria-hidden="true" tabindex="-1"></a>        test_dataset<span class="op">=</span><span class="va">None</span>,</span>
+<span id="cb35-7"><a href="#cb35-7" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>loss_function,</span>
+<span id="cb35-8"><a href="#cb35-8" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>metric,</span>
+<span id="cb35-9"><a href="#cb35-9" aria-hidden="true" tabindex="-1"></a>        device<span class="op">=</span>device,</span>
+<span id="cb35-10"><a href="#cb35-10" aria-hidden="true" tabindex="-1"></a>        show_batch_interval<span class="op">=</span>show_batch_interval,</span>
+<span id="cb35-11"><a href="#cb35-11" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span>path,</span>
+<span id="cb35-12"><a href="#cb35-12" aria-hidden="true" tabindex="-1"></a>    )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>Note: During training, <code>shuffle</code> is set to <code>True</code>, whereas during testing, <code>shuffle</code> is set to <code>False</code>.</p>
+</section>
+<section id="testing-of-the-tuned-architecture" class="level5">
+<h5 class="anchored" data-anchor-id="testing-of-the-tuned-architecture">Testing of the Tuned Architecture</h5>
+<p><code>test_tuned(model, test)</code>: test the model on the test data set. No data splitting is performed. The (trained) model is evaluated using the <code>validate_fold_or_hold_out()</code> function.</p>
+<p>Note: During training, <code>shuffle</code> is set to <code>True</code>, whereas during testing, <code>shuffle</code> is set to <code>False</code>.</p>
+<div class="cell" data-execution_count="29">
+<div class="sourceCode cell-code" id="cb36"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb36-1"><a href="#cb36-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> test_tuned(net, shuffle, test_dataset<span class="op">=</span><span class="va">None</span>, loss_function<span class="op">=</span><span class="va">None</span>, metric<span class="op">=</span><span class="va">None</span>, device<span class="op">=</span><span class="va">None</span>, path<span class="op">=</span><span class="va">None</span>):</span>
+<span id="cb36-2"><a href="#cb36-2" aria-hidden="true" tabindex="-1"></a>    batch_size_instance <span class="op">=</span> net.batch_size</span>
+<span id="cb36-3"><a href="#cb36-3" aria-hidden="true" tabindex="-1"></a>    removed_attributes, net <span class="op">=</span> get_removed_attributes_and_base_net(net)</span>
+<span id="cb36-4"><a href="#cb36-4" aria-hidden="true" tabindex="-1"></a>    <span class="cf">if</span> path <span class="kw">is</span> <span class="kw">not</span> <span class="va">None</span>:</span>
+<span id="cb36-5"><a href="#cb36-5" aria-hidden="true" tabindex="-1"></a>        net.load_state_dict(torch.load(path))</span>
+<span id="cb36-6"><a href="#cb36-6" aria-hidden="true" tabindex="-1"></a>        net.<span class="bu">eval</span>()</span>
+<span id="cb36-7"><a href="#cb36-7" aria-hidden="true" tabindex="-1"></a>    <span class="cf">try</span>:</span>
+<span id="cb36-8"><a href="#cb36-8" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> getDevice(device<span class="op">=</span>device)</span>
+<span id="cb36-9"><a href="#cb36-9" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> torch.cuda.is_available():</span>
+<span id="cb36-10"><a href="#cb36-10" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> <span class="st">"cuda:0"</span></span>
+<span id="cb36-11"><a href="#cb36-11" aria-hidden="true" tabindex="-1"></a>            <span class="cf">if</span> torch.cuda.device_count() <span class="op">&gt;</span> <span class="dv">1</span>:</span>
+<span id="cb36-12"><a href="#cb36-12" aria-hidden="true" tabindex="-1"></a>                <span class="bu">print</span>(<span class="st">"We will use"</span>, torch.cuda.device_count(), <span class="st">"GPUs!"</span>)</span>
+<span id="cb36-13"><a href="#cb36-13" aria-hidden="true" tabindex="-1"></a>                net <span class="op">=</span> nn.DataParallel(net)</span>
+<span id="cb36-14"><a href="#cb36-14" aria-hidden="true" tabindex="-1"></a>        net.to(device)</span>
+<span id="cb36-15"><a href="#cb36-15" aria-hidden="true" tabindex="-1"></a>        valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb36-16"><a href="#cb36-16" aria-hidden="true" tabindex="-1"></a>            test_dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size_instance), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span><span class="dv">0</span></span>
+<span id="cb36-17"><a href="#cb36-17" aria-hidden="true" tabindex="-1"></a>        )</span>
+<span id="cb36-18"><a href="#cb36-18" aria-hidden="true" tabindex="-1"></a>        metric_value, loss <span class="op">=</span> validate_fold_or_hold_out(</span>
+<span id="cb36-19"><a href="#cb36-19" aria-hidden="true" tabindex="-1"></a>            net, valloader<span class="op">=</span>valloader, loss_function<span class="op">=</span>loss_function, metric<span class="op">=</span>metric, device<span class="op">=</span>device</span>
+<span id="cb36-20"><a href="#cb36-20" aria-hidden="true" tabindex="-1"></a>        )</span>
+<span id="cb36-21"><a href="#cb36-21" aria-hidden="true" tabindex="-1"></a>        df_eval <span class="op">=</span> loss</span>
+<span id="cb36-22"><a href="#cb36-22" aria-hidden="true" tabindex="-1"></a>        df_metric <span class="op">=</span> metric_value</span>
+<span id="cb36-23"><a href="#cb36-23" aria-hidden="true" tabindex="-1"></a>        df_preds <span class="op">=</span> np.nan</span>
+<span id="cb36-24"><a href="#cb36-24" aria-hidden="true" tabindex="-1"></a>    <span class="cf">except</span> <span class="pp">Exception</span> <span class="im">as</span> err:</span>
+<span id="cb36-25"><a href="#cb36-25" aria-hidden="true" tabindex="-1"></a>        <span class="bu">print</span>(<span class="ss">f"Error in Net_Core. Call to test_tuned() failed. </span><span class="sc">{</span>err<span class="op">=</span><span class="sc">}</span><span class="ss">, </span><span class="sc">{</span><span class="bu">type</span>(err)<span class="op">=</span><span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb36-26"><a href="#cb36-26" aria-hidden="true" tabindex="-1"></a>        df_eval <span class="op">=</span> np.nan</span>
+<span id="cb36-27"><a href="#cb36-27" aria-hidden="true" tabindex="-1"></a>        df_metric <span class="op">=</span> np.nan</span>
+<span id="cb36-28"><a href="#cb36-28" aria-hidden="true" tabindex="-1"></a>        df_preds <span class="op">=</span> np.nan</span>
+<span id="cb36-29"><a href="#cb36-29" aria-hidden="true" tabindex="-1"></a>    add_attributes(net, removed_attributes)</span>
+<span id="cb36-30"><a href="#cb36-30" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="ss">f"Final evaluation: Validation loss: </span><span class="sc">{</span>df_eval<span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb36-31"><a href="#cb36-31" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="ss">f"Final evaluation: Validation metric: </span><span class="sc">{</span>df_metric<span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb36-32"><a href="#cb36-32" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="st">"----------------------------------------------"</span>)</span>
+<span id="cb36-33"><a href="#cb36-33" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> df_eval, df_preds, df_metric</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+</section>
+</section>
+</section>
+<section id="loss-functions-and-metrics" class="level3">
+<h3 class="anchored" data-anchor-id="loss-functions-and-metrics">Loss Functions and Metrics</h3>
+<p>The key <code>"loss_function"</code> specifies the loss function which is used during the optimization. There are several different loss functions under <code>PyTorch</code>’s <code>nn</code> package. For example, a simple loss is <code>MSELoss</code>, which computes the mean-squared error between the output and the target. In this tutorial we will use <code>CrossEntropyLoss</code>, because it is also used in the <code>PyTorch</code> tutorial.</p>
+<div class="cell" data-execution_count="30">
+<div class="sourceCode cell-code" id="cb37"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb37-1"><a href="#cb37-1" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> torch.nn <span class="im">import</span> CrossEntropyLoss</span>
+<span id="cb37-2"><a href="#cb37-2" aria-hidden="true" tabindex="-1"></a>loss_function <span class="op">=</span> CrossEntropyLoss()</span>
+<span id="cb37-3"><a href="#cb37-3" aria-hidden="true" tabindex="-1"></a>fun_control.update({<span class="st">"loss_function"</span>: loss_function})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>In addition to the loss functions, <code>spotPython</code> provides access to a large number of metrics. The key <code>"metric_sklearn"</code> is used for metrics that follow the <code>scikit-learn</code> conventions. The key <code>"river_metric"</code> is used for the river based evaluation <span class="citation" data-cites="mont20a">(<a href="#ref-mont20a" role="doc-biblioref">Montiel et al. 2021</a>)</span> via <code>eval_oml_iter_progressive</code>, and the key <code>"metric_torch"</code> is used for the metrics from <code>TorchMetrics</code>. <code>TorchMetrics</code> is a collection of more than 90 PyTorch metrics<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>. Because the <code>PyTorch</code> tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial’s example code. We will use <code>TorchMetrics</code> instead, because it offers:</p>
+<ul>
+<li>A standardized interface to increase reproducibility</li>
+<li>Reduces Boilerplate</li>
+<li>Distributed-training compatible</li>
+<li>Rigorously tested</li>
+<li>Automatic accumulation over batches</li>
+<li>Automatic synchronization between multiple devices</li>
+</ul>
+<p>Therefore, we set</p>
+<div class="cell" data-execution_count="31">
+<div class="sourceCode cell-code" id="cb38"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb38-1"><a href="#cb38-1" aria-hidden="true" tabindex="-1"></a>metric_torch <span class="op">=</span> torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="32">
+<div class="sourceCode cell-code" id="cb39"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb39-1"><a href="#cb39-1" aria-hidden="true" tabindex="-1"></a>loss_function <span class="op">=</span> CrossEntropyLoss()</span>
+<span id="cb39-2"><a href="#cb39-2" aria-hidden="true" tabindex="-1"></a>weights <span class="op">=</span> <span class="fl">1.0</span></span>
+<span id="cb39-3"><a href="#cb39-3" aria-hidden="true" tabindex="-1"></a>metric_torch <span class="op">=</span> torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>)</span>
+<span id="cb39-4"><a href="#cb39-4" aria-hidden="true" tabindex="-1"></a>shuffle <span class="op">=</span> <span class="va">True</span></span>
+<span id="cb39-5"><a href="#cb39-5" aria-hidden="true" tabindex="-1"></a><span class="bu">eval</span> <span class="op">=</span> <span class="st">"train_hold_out"</span></span>
+<span id="cb39-6"><a href="#cb39-6" aria-hidden="true" tabindex="-1"></a>device <span class="op">=</span> DEVICE</span>
+<span id="cb39-7"><a href="#cb39-7" aria-hidden="true" tabindex="-1"></a>show_batch_interval <span class="op">=</span> <span class="dv">100_000</span></span>
+<span id="cb39-8"><a href="#cb39-8" aria-hidden="true" tabindex="-1"></a>path<span class="op">=</span><span class="st">"torch_model.pt"</span></span>
+<span id="cb39-9"><a href="#cb39-9" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb39-10"><a href="#cb39-10" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
+<span id="cb39-11"><a href="#cb39-11" aria-hidden="true" tabindex="-1"></a>               <span class="st">"data_dir"</span>: <span class="va">None</span>,</span>
+<span id="cb39-12"><a href="#cb39-12" aria-hidden="true" tabindex="-1"></a>               <span class="st">"checkpoint_dir"</span>: <span class="va">None</span>,</span>
+<span id="cb39-13"><a href="#cb39-13" aria-hidden="true" tabindex="-1"></a>               <span class="st">"horizon"</span>: <span class="va">None</span>,</span>
+<span id="cb39-14"><a href="#cb39-14" aria-hidden="true" tabindex="-1"></a>               <span class="st">"oml_grace_period"</span>: <span class="va">None</span>,</span>
+<span id="cb39-15"><a href="#cb39-15" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weights"</span>: weights,</span>
+<span id="cb39-16"><a href="#cb39-16" aria-hidden="true" tabindex="-1"></a>               <span class="st">"step"</span>: <span class="va">None</span>,</span>
+<span id="cb39-17"><a href="#cb39-17" aria-hidden="true" tabindex="-1"></a>               <span class="st">"log_level"</span>: <span class="dv">50</span>,</span>
+<span id="cb39-18"><a href="#cb39-18" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weight_coeff"</span>: <span class="va">None</span>,</span>
+<span id="cb39-19"><a href="#cb39-19" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_torch"</span>: metric_torch,</span>
+<span id="cb39-20"><a href="#cb39-20" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_river"</span>: <span class="va">None</span>,</span>
+<span id="cb39-21"><a href="#cb39-21" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_sklearn"</span>: <span class="va">None</span>,</span>
+<span id="cb39-22"><a href="#cb39-22" aria-hidden="true" tabindex="-1"></a>               <span class="st">"loss_function"</span>: loss_function,</span>
+<span id="cb39-23"><a href="#cb39-23" aria-hidden="true" tabindex="-1"></a>               <span class="st">"shuffle"</span>: shuffle,</span>
+<span id="cb39-24"><a href="#cb39-24" aria-hidden="true" tabindex="-1"></a>               <span class="st">"eval"</span>: <span class="bu">eval</span>,</span>
+<span id="cb39-25"><a href="#cb39-25" aria-hidden="true" tabindex="-1"></a>               <span class="st">"device"</span>: device,</span>
+<span id="cb39-26"><a href="#cb39-26" aria-hidden="true" tabindex="-1"></a>               <span class="st">"show_batch_interval"</span>: show_batch_interval,</span>
+<span id="cb39-27"><a href="#cb39-27" aria-hidden="true" tabindex="-1"></a>               <span class="st">"path"</span>: path,</span>
+<span id="cb39-28"><a href="#cb39-28" aria-hidden="true" tabindex="-1"></a>               })</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 </section>
 <section id="sec-call-the-hyperparameter-tuner" class="level2">
 <h2 class="anchored" data-anchor-id="sec-call-the-hyperparameter-tuner">Calling the SPOT Function</h2>
 <p>Now, the dictionary <code>fun_control</code> contains all information needed for the hyperparameter tuning. Before the hyperparameter tuning is started, it is recommended to take a look at the experimental design. The method <code>gen_design_table</code> generates a design table as follows:</p>
-<div class="cell" data-execution_count="17">
-<div class="sourceCode cell-code" id="cb23"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb23-1"><a href="#cb23-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="34">
+<div class="sourceCode cell-code" id="cb40"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb40-1"><a href="#cb40-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<p>This allows to check if all information is available and if the information is correct. <a href="#tbl-design">Table&nbsp;2</a> shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column “transform”, e.g., the <code>l1</code> default is <code>5</code>, which results in the value <span class="math inline">\(2^5 = 32\)</span> for the network, because the transformation <code>transform_power_2_int</code> was selected in the <code>JSON</code> file. The default value of the <code>batch_size</code> is set to <code>4</code>, which results in a batch size of <span class="math inline">\(2^4 = 16\)</span>.</p>
+<p>This allows to check if all information is available and if the information is correct. <a href="#tbl-design">Table&nbsp;3</a> shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column “transform”, e.g., the <code>l1</code> default is <code>5</code>, which results in the value <span class="math inline">\(2^5 = 32\)</span> for the network, because the transformation <code>transform_power_2_int</code> was selected in the <code>JSON</code> file. The default value of the <code>batch_size</code> is set to <code>4</code>, which results in a batch size of <span class="math inline">\(2^4 = 16\)</span>.</p>
 <div id="tbl-design" class="anchored">
 <table class="table">
-<caption>Table&nbsp;2: Experimental design for the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The transformation function is used to transform the hyperparameter values from the unit hypercube to the original domain. The transformation function is applied to the hyperparameter values before the evaluation of the objective function.</caption>
+<caption>Table&nbsp;3: Experimental design for the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The transformation function is used to transform the hyperparameter values from the unit hypercube to the original domain. The transformation function is applied to the hyperparameter values before the evaluation of the objective function.</caption>
 <colgroup>
 <col style="width: 15%">
 <col style="width: 10%">
 <col style="width: 22%">
 <col style="width: 11%">
 <col style="width: 11%">
 <col style="width: 29%">
@@ -869,118 +1378,130 @@
 <td>optimizer</td>
 <td>factor</td>
 <td>SGD</td>
 <td>0</td>
 <td>9</td>
 <td>None</td>
 </tr>
-<tr class="odd">
-<td>criterion</td>
-<td>factor</td>
-<td>CrossEntropyLoss</td>
-<td>0</td>
-<td>0</td>
-<td>None</td>
-</tr>
 </tbody>
 </table>
 </div>
 <p>The objective function <code>fun_torch</code> is selected next. It implements an interface from <code>PyTorch</code>’s training, validation, and testing methods to <code>spotPython</code>.</p>
-<div class="cell" data-execution_count="18">
-<div class="sourceCode cell-code" id="cb24"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb24-1"><a href="#cb24-1" aria-hidden="true" tabindex="-1"></a>fun <span class="op">=</span> HyperTorch().fun_torch</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="35">
+<div class="sourceCode cell-code" id="cb41"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb41-1"><a href="#cb41-1" aria-hidden="true" tabindex="-1"></a>fun <span class="op">=</span> HyperTorch().fun_torch</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The <code>spotPython</code> hyperparameter tuning is started by calling the <code>Spot</code> function. Here, we will run the tuner for approximately 30 minutes (<code>max_time</code>). Note: the initial design is always evaluated in the <code>spotPython</code> run. As a consequence, the run may take longer than specified by <code>max_time</code>, because the evaluation time of initial design (here: <code>init_size</code>, 10 points) is performed independently of <code>max_time</code>.</p>
-<div class="cell" data-execution_count="20">
-<div class="sourceCode cell-code" id="cb25"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb25-1"><a href="#cb25-1" aria-hidden="true" tabindex="-1"></a>spot_tuner <span class="op">=</span> spot.Spot(fun<span class="op">=</span>fun,</span>
-<span id="cb25-2"><a href="#cb25-2" aria-hidden="true" tabindex="-1"></a>                   lower <span class="op">=</span> lower,</span>
-<span id="cb25-3"><a href="#cb25-3" aria-hidden="true" tabindex="-1"></a>                   upper <span class="op">=</span> upper,</span>
-<span id="cb25-4"><a href="#cb25-4" aria-hidden="true" tabindex="-1"></a>                   fun_evals <span class="op">=</span> inf,</span>
-<span id="cb25-5"><a href="#cb25-5" aria-hidden="true" tabindex="-1"></a>                   fun_repeats <span class="op">=</span> <span class="dv">1</span>,</span>
-<span id="cb25-6"><a href="#cb25-6" aria-hidden="true" tabindex="-1"></a>                   max_time <span class="op">=</span> MAX_TIME,</span>
-<span id="cb25-7"><a href="#cb25-7" aria-hidden="true" tabindex="-1"></a>                   noise <span class="op">=</span> <span class="va">False</span>,</span>
-<span id="cb25-8"><a href="#cb25-8" aria-hidden="true" tabindex="-1"></a>                   tolerance_x <span class="op">=</span> np.sqrt(np.spacing(<span class="dv">1</span>)),</span>
-<span id="cb25-9"><a href="#cb25-9" aria-hidden="true" tabindex="-1"></a>                   var_type <span class="op">=</span> var_type,</span>
-<span id="cb25-10"><a href="#cb25-10" aria-hidden="true" tabindex="-1"></a>                   var_name <span class="op">=</span> var_name,</span>
-<span id="cb25-11"><a href="#cb25-11" aria-hidden="true" tabindex="-1"></a>                   infill_criterion <span class="op">=</span> <span class="st">"y"</span>,</span>
-<span id="cb25-12"><a href="#cb25-12" aria-hidden="true" tabindex="-1"></a>                   n_points <span class="op">=</span> <span class="dv">1</span>,</span>
-<span id="cb25-13"><a href="#cb25-13" aria-hidden="true" tabindex="-1"></a>                   seed<span class="op">=</span><span class="dv">123</span>,</span>
-<span id="cb25-14"><a href="#cb25-14" aria-hidden="true" tabindex="-1"></a>                   log_level <span class="op">=</span> <span class="dv">50</span>,</span>
-<span id="cb25-15"><a href="#cb25-15" aria-hidden="true" tabindex="-1"></a>                   show_models<span class="op">=</span> <span class="va">False</span>,</span>
-<span id="cb25-16"><a href="#cb25-16" aria-hidden="true" tabindex="-1"></a>                   show_progress<span class="op">=</span> <span class="va">True</span>,</span>
-<span id="cb25-17"><a href="#cb25-17" aria-hidden="true" tabindex="-1"></a>                   fun_control <span class="op">=</span> fun_control,</span>
-<span id="cb25-18"><a href="#cb25-18" aria-hidden="true" tabindex="-1"></a>                   design_control<span class="op">=</span>{<span class="st">"init_size"</span>: INIT_SIZE,</span>
-<span id="cb25-19"><a href="#cb25-19" aria-hidden="true" tabindex="-1"></a>                                   <span class="st">"repeats"</span>: <span class="dv">1</span>},</span>
-<span id="cb25-20"><a href="#cb25-20" aria-hidden="true" tabindex="-1"></a>                   surrogate_control<span class="op">=</span>{<span class="st">"noise"</span>: <span class="va">True</span>,</span>
-<span id="cb25-21"><a href="#cb25-21" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"cod_type"</span>: <span class="st">"norm"</span>,</span>
-<span id="cb25-22"><a href="#cb25-22" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"min_theta"</span>: <span class="op">-</span><span class="dv">4</span>,</span>
-<span id="cb25-23"><a href="#cb25-23" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"max_theta"</span>: <span class="dv">3</span>,</span>
-<span id="cb25-24"><a href="#cb25-24" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"n_theta"</span>: <span class="bu">len</span>(var_name),</span>
-<span id="cb25-25"><a href="#cb25-25" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_optimizer"</span>: differential_evolution,</span>
-<span id="cb25-26"><a href="#cb25-26" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_fun_evals"</span>: <span class="dv">10_000</span>,</span>
-<span id="cb25-27"><a href="#cb25-27" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"log_level"</span>: <span class="dv">50</span></span>
-<span id="cb25-28"><a href="#cb25-28" aria-hidden="true" tabindex="-1"></a>                                      })</span>
-<span id="cb25-29"><a href="#cb25-29" aria-hidden="true" tabindex="-1"></a>spot_tuner.run(X_start<span class="op">=</span>X_start)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="37">
+<div class="sourceCode cell-code" id="cb42"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb42-1"><a href="#cb42-1" aria-hidden="true" tabindex="-1"></a>spot_tuner <span class="op">=</span> spot.Spot(fun<span class="op">=</span>fun,</span>
+<span id="cb42-2"><a href="#cb42-2" aria-hidden="true" tabindex="-1"></a>                   lower <span class="op">=</span> lower,</span>
+<span id="cb42-3"><a href="#cb42-3" aria-hidden="true" tabindex="-1"></a>                   upper <span class="op">=</span> upper,</span>
+<span id="cb42-4"><a href="#cb42-4" aria-hidden="true" tabindex="-1"></a>                   fun_evals <span class="op">=</span> inf,</span>
+<span id="cb42-5"><a href="#cb42-5" aria-hidden="true" tabindex="-1"></a>                   fun_repeats <span class="op">=</span> <span class="dv">1</span>,</span>
+<span id="cb42-6"><a href="#cb42-6" aria-hidden="true" tabindex="-1"></a>                   max_time <span class="op">=</span> MAX_TIME,</span>
+<span id="cb42-7"><a href="#cb42-7" aria-hidden="true" tabindex="-1"></a>                   noise <span class="op">=</span> <span class="va">False</span>,</span>
+<span id="cb42-8"><a href="#cb42-8" aria-hidden="true" tabindex="-1"></a>                   tolerance_x <span class="op">=</span> np.sqrt(np.spacing(<span class="dv">1</span>)),</span>
+<span id="cb42-9"><a href="#cb42-9" aria-hidden="true" tabindex="-1"></a>                   var_type <span class="op">=</span> var_type,</span>
+<span id="cb42-10"><a href="#cb42-10" aria-hidden="true" tabindex="-1"></a>                   var_name <span class="op">=</span> var_name,</span>
+<span id="cb42-11"><a href="#cb42-11" aria-hidden="true" tabindex="-1"></a>                   infill_criterion <span class="op">=</span> <span class="st">"y"</span>,</span>
+<span id="cb42-12"><a href="#cb42-12" aria-hidden="true" tabindex="-1"></a>                   n_points <span class="op">=</span> <span class="dv">1</span>,</span>
+<span id="cb42-13"><a href="#cb42-13" aria-hidden="true" tabindex="-1"></a>                   seed<span class="op">=</span><span class="dv">123</span>,</span>
+<span id="cb42-14"><a href="#cb42-14" aria-hidden="true" tabindex="-1"></a>                   log_level <span class="op">=</span> <span class="dv">50</span>,</span>
+<span id="cb42-15"><a href="#cb42-15" aria-hidden="true" tabindex="-1"></a>                   show_models<span class="op">=</span> <span class="va">False</span>,</span>
+<span id="cb42-16"><a href="#cb42-16" aria-hidden="true" tabindex="-1"></a>                   show_progress<span class="op">=</span> <span class="va">True</span>,</span>
+<span id="cb42-17"><a href="#cb42-17" aria-hidden="true" tabindex="-1"></a>                   fun_control <span class="op">=</span> fun_control,</span>
+<span id="cb42-18"><a href="#cb42-18" aria-hidden="true" tabindex="-1"></a>                   design_control<span class="op">=</span>{<span class="st">"init_size"</span>: INIT_SIZE,</span>
+<span id="cb42-19"><a href="#cb42-19" aria-hidden="true" tabindex="-1"></a>                                   <span class="st">"repeats"</span>: <span class="dv">1</span>},</span>
+<span id="cb42-20"><a href="#cb42-20" aria-hidden="true" tabindex="-1"></a>                   surrogate_control<span class="op">=</span>{<span class="st">"noise"</span>: <span class="va">True</span>,</span>
+<span id="cb42-21"><a href="#cb42-21" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"cod_type"</span>: <span class="st">"norm"</span>,</span>
+<span id="cb42-22"><a href="#cb42-22" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"min_theta"</span>: <span class="op">-</span><span class="dv">4</span>,</span>
+<span id="cb42-23"><a href="#cb42-23" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"max_theta"</span>: <span class="dv">3</span>,</span>
+<span id="cb42-24"><a href="#cb42-24" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"n_theta"</span>: <span class="bu">len</span>(var_name),</span>
+<span id="cb42-25"><a href="#cb42-25" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_optimizer"</span>: differential_evolution,</span>
+<span id="cb42-26"><a href="#cb42-26" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_fun_evals"</span>: <span class="dv">10_000</span>,</span>
+<span id="cb42-27"><a href="#cb42-27" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"log_level"</span>: <span class="dv">50</span></span>
+<span id="cb42-28"><a href="#cb42-28" aria-hidden="true" tabindex="-1"></a>                                      })</span>
+<span id="cb42-29"><a href="#cb42-29" aria-hidden="true" tabindex="-1"></a>spot_tuner.run(X_start<span class="op">=</span>X_start)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>During the run, the following output is shown:</p>
-<pre class="{raw}"><code>config: {'l1': 8, 'l2': 16, 'lr': 0.001, 'batch_size': 2, 
-'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'NAdam', 
-'criterion': CrossEntropyLoss()}
+<pre class="{raw}"><code>config: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'Adadelta', 'sgd_momentum': 0.9}
 Epoch: 1
-Loss on hold-out set: 1.798599960240349
-Accuracy on hold-out set: 0.38035
+Loss on hold-out set: 1.602842689704895
+Accuracy on hold-out set: 0.4006
+Metric value on hold-out data: 0.40059998631477356
 Epoch: 2
-Loss on hold-out set: 1.681505929086823
-Accuracy on hold-out set: 0.4163
+Loss on hold-out set: 1.4648857820034027
+Accuracy on hold-out set: 0.47685
+Metric value on hold-out data: 0.4768500030040741
 Epoch: 3
-Loss on hold-out set: 1.6875325478885324
-Accuracy on hold-out set: 0.42245
+Loss on hold-out set: 1.403354868555069
+Accuracy on hold-out set: 0.482
+Metric value on hold-out data: 0.4819999933242798
 Epoch: 4
-Loss on hold-out set: 1.6695034023197601
-Accuracy on hold-out set: 0.45265
+Loss on hold-out set: 1.384560032081604
+Accuracy on hold-out set: 0.49065
+Metric value on hold-out data: 0.4906499981880188
 Epoch: 5
-Loss on hold-out set: 1.6984369342865335
-Accuracy on hold-out set: 0.45085
+Loss on hold-out set: 1.4326466094970702
+Accuracy on hold-out set: 0.4809
+Metric value on hold-out data: 0.48089998960494995
 Epoch: 6
-Loss on hold-out set: 1.6061365829033545
-Accuracy on hold-out set: 0.4527
+Loss on hold-out set: 1.3759961807250976
+Accuracy on hold-out set: 0.4995
+Metric value on hold-out data: 0.49950000643730164
 Epoch: 7
-Loss on hold-out set: 1.7061124059396433
-Accuracy on hold-out set: 0.4566
+Loss on hold-out set: 1.3684927892208099
+Accuracy on hold-out set: 0.50695
+Metric value on hold-out data: 0.5069500207901001
 Epoch: 8
-Loss on hold-out set: 1.7162298802530742
-Accuracy on hold-out set: 0.4504
+Loss on hold-out set: 1.3642385012149811
+Accuracy on hold-out set: 0.506
+Metric value on hold-out data: 0.5059999823570251
 Epoch: 9
-Loss on hold-out set: 1.6683832777252945
-Accuracy on hold-out set: 0.47205
-Early stopping at epoch 8
-Returned to Spot: Validation loss: 1.6683832777252945</code></pre>
+Loss on hold-out set: 1.3157437609672546
+Accuracy on hold-out set: 0.5304
+Metric value on hold-out data: 0.5303999781608582
+Epoch: 10
+Loss on hold-out set: 1.3481314319610596
+Accuracy on hold-out set: 0.5268
+Metric value on hold-out data: 0.5267999768257141
+Epoch: 11
+Loss on hold-out set: 1.3608774542331696
+Accuracy on hold-out set: 0.51525
+Metric value on hold-out data: 0.515250027179718
+Epoch: 12
+Loss on hold-out set: 1.359324642753601
+Accuracy on hold-out set: 0.52355
+Metric value on hold-out data: 0.5235499739646912
+Early stopping at epoch 11
+Returned to Spot: Validation loss: 1.359324642753601
+----------------------------------------------</code></pre>
 </section>
 <section id="sec-results-tuning" class="level2">
 <h2 class="anchored" data-anchor-id="sec-results-tuning">Results</h2>
 <p>After the hyperparameter tuning run is finished, the progress of the hyperparameter tuning can be visualized. The following code generates the progress plot from <a href="#fig-progress">Figure&nbsp;2</a>.</p>
 <div id="fig-progress" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<div class="sourceCode cell-code" id="cb27"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb27-1"><a href="#cb27-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_progress(log_y<span class="op">=</span><span class="va">False</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_progress.pdf"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb44"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb44-1"><a href="#cb44-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_progress(log_y<span class="op">=</span><span class="va">False</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_progress.png"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 <figcaption class="figure-caption">Figure&nbsp;1: <strong>?(caption)</strong></figcaption>
 </figure>
 </div>
 <div id="fig-progress" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;2: Progress plot. <code>Black</code> dots denote results from the initial design. <code>Red</code> dots illustrate the improvement found by the surrogate model based optimization (surrogate model based optimization).</figcaption>
 </figure>
 </div>
 <p><a href="#fig-progress">Figure&nbsp;2</a> shows a typical behaviour that can be observed in many hyperparameter studies <span class="citation" data-cites="bart21i">(<a href="#ref-bart21i" role="doc-biblioref">Bartz et al. 2022</a>)</span>: the largest improvement is obtained during the evaluation of the initial design. The surrogate model based optimization-optimization with the surrogate refines the results. <a href="#fig-progress">Figure&nbsp;2</a> also illustrates one major difference between <code>ray[tune]</code> as used in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span> and <code>spotPython</code>: the <code>ray[tune]</code> uses a random search and will generate results similar to the <em>black</em> dots, whereas <code>spotPython</code> uses a surrogate model based optimization and presents results represented by <em>red</em> dots in <a href="#fig-progress">Figure&nbsp;2</a>. The surrogate model based optimization is considered to be more efficient than a random search, because the surrogate model guides the search towards promising regions in the hyperparameter space.</p>
-<p>In addition to the improved (“optimized”) hyperparameter values, <code>spotPython</code> allows a statistical analysis, e.g., a sensitivity analysis, of the results. We can print the results of the hyperparameter tuning, see <a href="#tbl-results">Table&nbsp;3</a>.</p>
-<div class="cell" data-execution_count="23">
-<div class="sourceCode cell-code" id="cb28"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb28-1"><a href="#cb28-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control<span class="op">=</span>fun_control, spot<span class="op">=</span>spot_tuner))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>In addition to the improved (“optimized”) hyperparameter values, <code>spotPython</code> allows a statistical analysis, e.g., a sensitivity analysis, of the results. We can print the results of the hyperparameter tuning, see <a href="#tbl-results">Table&nbsp;4</a>.</p>
+<div class="cell" data-execution_count="40">
+<div class="sourceCode cell-code" id="cb45"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb45-1"><a href="#cb45-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control<span class="op">=</span>fun_control, spot<span class="op">=</span>spot_tuner))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <div id="tbl-results" class="anchored">
 <table class="table">
-<caption>Table&nbsp;3: Results of the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The column “tuned” shows the tuned values. The column “importance” shows the importance of the hyperparameters. The column “stars” shows the importance of the hyperparameters in stars. The importance is computed by the SPOT software.</caption>
+<caption>Table&nbsp;4: Results of the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The column “tuned” shows the tuned values. The column “importance” shows the importance of the hyperparameters. The column “stars” shows the importance of the hyperparameters in stars. The importance is computed by the SPOT software.</caption>
 <colgroup>
 <col style="width: 10%">
 <col style="width: 7%">
 <col style="width: 16%">
 <col style="width: 8%">
 <col style="width: 8%">
 <col style="width: 8%">
@@ -1021,20 +1542,20 @@
 <td style="text-align: right;">9.0</td>
 <td style="text-align: right;">3.0</td>
 <td>pow_2_int</td>
 <td style="text-align: right;">96.29</td>
 <td>***</td>
 </tr>
 <tr class="odd">
-<td>lr</td>
+<td>lr_mult</td>
 <td>float</td>
-<td>0.001</td>
-<td style="text-align: right;">0.001</td>
-<td style="text-align: right;">0.001</td>
-<td style="text-align: right;">0.001</td>
+<td>1.0</td>
+<td style="text-align: right;">0.1</td>
+<td style="text-align: right;">10.0</td>
+<td style="text-align: right;">0.1</td>
 <td>None</td>
 <td style="text-align: right;">0.00</td>
 <td></td>
 </tr>
 <tr class="even">
 <td>batchsize</td>
 <td>int</td>
@@ -1086,108 +1607,109 @@
 <td style="text-align: right;">0.0</td>
 <td style="text-align: right;">9.0</td>
 <td style="text-align: right;">3.0</td>
 <td>None</td>
 <td style="text-align: right;">0.16</td>
 <td>.</td>
 </tr>
-<tr class="odd">
-<td>criterion</td>
-<td>factor</td>
-<td>CrossEntLoss</td>
-<td style="text-align: right;">0.0</td>
-<td style="text-align: right;">0.0</td>
-<td style="text-align: right;">0.0</td>
-<td>None</td>
-<td style="text-align: right;">0.00</td>
-<td></td>
-</tr>
 </tbody>
 </table>
 </div>
 <p>To visualize the most important hyperparameters, <code>spotPython</code> provides the function <code>plot_importance</code>. The following code generates the importance plot from <a href="#fig-importance">Figure&nbsp;3</a>.</p>
-<div class="cell" data-execution_count="24">
-<div class="sourceCode cell-code" id="cb29"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb29-1"><a href="#cb29-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_importance(threshold<span class="op">=</span><span class="fl">0.025</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_importance.pdf"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="41">
+<div class="sourceCode cell-code" id="cb46"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb46-1"><a href="#cb46-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_importance(threshold<span class="op">=</span><span class="fl">0.025</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_importance.png"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <div id="fig-importance" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf" class="img-fluid" style="width:50.0%"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png" class="img-fluid figure-img" style="width:50.0%"></p>
 <figcaption class="figure-caption">Figure&nbsp;3: Variable importance</figcaption>
 </figure>
 </div>
 </section>
 <section id="sec-get-spot-results" class="level2">
 <h2 class="anchored" data-anchor-id="sec-get-spot-results">Get SPOT Results</h2>
 <p>The architecture of the <code>spotPython</code> model can be obtained by the following code:</p>
-<div class="cell" data-execution_count="25">
-<div class="sourceCode cell-code" id="cb30"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb30-1"><a href="#cb30-1" aria-hidden="true" tabindex="-1"></a>X <span class="op">=</span> spot_tuner.to_all_dim(spot_tuner.min_X.reshape(<span class="dv">1</span>,<span class="op">-</span><span class="dv">1</span>))</span>
-<span id="cb30-2"><a href="#cb30-2" aria-hidden="true" tabindex="-1"></a>model_spot <span class="op">=</span> get_one_core_model_from_X(X, fun_control)</span>
-<span id="cb30-3"><a href="#cb30-3" aria-hidden="true" tabindex="-1"></a>model_spot</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="42">
+<div class="sourceCode cell-code" id="cb47"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb47-1"><a href="#cb47-1" aria-hidden="true" tabindex="-1"></a>X <span class="op">=</span> spot_tuner.to_all_dim(spot_tuner.min_X.reshape(<span class="dv">1</span>,<span class="op">-</span><span class="dv">1</span>))</span>
+<span id="cb47-2"><a href="#cb47-2" aria-hidden="true" tabindex="-1"></a>model_spot <span class="op">=</span> get_one_core_model_from_X(X, fun_control)</span>
+<span id="cb47-3"><a href="#cb47-3" aria-hidden="true" tabindex="-1"></a>model_spot</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>First, the numerical representation of the hyperparameters are obtained, i.e., the numpy array <code>X</code> is generated. This array is then used to generate the model <code>model_spot</code> by the function <code>get_one_core_model_from_X</code>. The model <code>model_spot</code> has the following architecture:</p>
 <pre class="{raw}"><code>Net_CIFAR10(
   (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))
   (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
   (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
   (fc1): Linear(in_features=400, out_features=64, bias=True)
   (fc2): Linear(in_features=64, out_features=32, bias=True)
   (fc3): Linear(in_features=32, out_features=10, bias=True)
 )</code></pre>
 </section>
 <section id="get-default-hyperparameters" class="level2">
 <h2 class="anchored" data-anchor-id="get-default-hyperparameters">Get Default Hyperparameters</h2>
 <p>In a similar manner as in <a href="#sec-get-spot-results">Section&nbsp;3.11</a>, the default hyperparameters can be obtained.</p>
-<div class="cell" data-execution_count="26">
-<div class="sourceCode cell-code" id="cb32"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb32-1"><a href="#cb32-1" aria-hidden="true" tabindex="-1"></a><span class="co"># fun_control was modified, we generate a new one with the original default hyperparameters</span></span>
-<span id="cb32-2"><a href="#cb32-2" aria-hidden="true" tabindex="-1"></a>fc <span class="op">=</span> copy.deepcopy(fun_control)</span>
-<span id="cb32-3"><a href="#cb32-3" aria-hidden="true" tabindex="-1"></a>fc.update({<span class="st">"core_model_hyper_dict"</span>: hyper_dict[fun_control[<span class="st">"core_model"</span>].<span class="va">__name__</span>]})</span>
-<span id="cb32-4"><a href="#cb32-4" aria-hidden="true" tabindex="-1"></a>model_default <span class="op">=</span> get_one_core_model_from_X(X_start, fun_control<span class="op">=</span>fc)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="43">
+<div class="sourceCode cell-code" id="cb49"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb49-1"><a href="#cb49-1" aria-hidden="true" tabindex="-1"></a><span class="co"># fun_control was modified, we generate a new one with the original default hyperparameters</span></span>
+<span id="cb49-2"><a href="#cb49-2" aria-hidden="true" tabindex="-1"></a>fc <span class="op">=</span> copy.deepcopy(fun_control)</span>
+<span id="cb49-3"><a href="#cb49-3" aria-hidden="true" tabindex="-1"></a>fc.update({<span class="st">"core_model_hyper_dict"</span>: hyper_dict[fun_control[<span class="st">"core_model"</span>].<span class="va">__name__</span>]})</span>
+<span id="cb49-4"><a href="#cb49-4" aria-hidden="true" tabindex="-1"></a>model_default <span class="op">=</span> get_one_core_model_from_X(X_start, fun_control<span class="op">=</span>fc)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The corresponding default model has the following architecture:</p>
 <pre class="{raw}"><code>Net_CIFAR10(
   (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))
   (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
   (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
   (fc1): Linear(in_features=400, out_features=32, bias=True)
   (fc2): Linear(in_features=32, out_features=32, bias=True)
   (fc3): Linear(in_features=32, out_features=10, bias=True)
 )</code></pre>
 </section>
 <section id="evaluation-of-the-tuned-architecture" class="level2">
 <h2 class="anchored" data-anchor-id="evaluation-of-the-tuned-architecture">Evaluation of the Tuned Architecture</h2>
-<p>The method <code>train_save</code> takes a model architecture without trained weights and trains this model with the train data. The train data is split into train and validation data. The validation data is used for early stopping. The trained model weights are saved as a dictionary.</p>
+<p>The method <code>train_tuned</code> takes a model architecture without trained weights and trains this model with the train data. The train data is split into train and validation data. The validation data is used for early stopping. The trained model weights are saved as a dictionary.</p>
 <p>This evaluation is similar to the final evaluation in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>.</p>
-<div class="cell" data-execution_count="27">
-<div class="sourceCode cell-code" id="cb34"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb34-1"><a href="#cb34-1" aria-hidden="true" tabindex="-1"></a>train_save(net<span class="op">=</span>model_default, train_dataset<span class="op">=</span>train, shuffle<span class="op">=</span><span class="va">True</span>,</span>
-<span id="cb34-2"><a href="#cb34-2" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> <span class="st">"cpu"</span>, show_batch_interval<span class="op">=</span><span class="dv">1_000</span>, </span>
-<span id="cb34-3"><a href="#cb34-3" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span><span class="st">"model_default_trained.pt"</span>, save_model<span class="op">=</span><span class="va">True</span>)</span>
-<span id="cb34-4"><a href="#cb34-4" aria-hidden="true" tabindex="-1"></a>test_saved(net<span class="op">=</span>model_default, test_dataset<span class="op">=</span>test, shuffle<span class="op">=</span><span class="va">False</span>, </span>
-<span id="cb34-5"><a href="#cb34-5" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> <span class="st">"cpu"</span>, path<span class="op">=</span><span class="st">"model_default_trained.pt"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>The following code trains the model <code>model_spot</code> and saves the weights of the trained model to the file <code>model_spot_trained.pt</code>.</p>
-<div class="cell" data-execution_count="28">
-<div class="sourceCode cell-code" id="cb35"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb35-1"><a href="#cb35-1" aria-hidden="true" tabindex="-1"></a>train_save(net<span class="op">=</span>model_spot, train_dataset<span class="op">=</span>train,</span>
-<span id="cb35-2"><a href="#cb35-2" aria-hidden="true" tabindex="-1"></a>                shuffle<span class="op">=</span><span class="va">True</span>, path<span class="op">=</span><span class="st">"model_spot_trained.pt"</span>, save_model<span class="op">=</span><span class="va">True</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="44">
+<div class="sourceCode cell-code" id="cb51"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb51-1"><a href="#cb51-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_default, train_dataset<span class="op">=</span>train, shuffle<span class="op">=</span><span class="va">True</span>,</span>
+<span id="cb51-2"><a href="#cb51-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb51-3"><a href="#cb51-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb51-4"><a href="#cb51-4" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE, show_batch_interval<span class="op">=</span><span class="dv">1_000</span>,)</span>
+<span id="cb51-5"><a href="#cb51-5" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_default, test_dataset<span class="op">=</span>test, </span>
+<span id="cb51-6"><a href="#cb51-6" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb51-7"><a href="#cb51-7" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb51-8"><a href="#cb51-8" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">False</span>, </span>
+<span id="cb51-9"><a href="#cb51-9" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>The following code trains the model <code>model_spot</code>. If <code>path</code> is set to a filename, e.g., <code>path = "model_spot_trained.pt"</code>, the weights of the trained model will be saved to this file.</p>
+<div class="cell" data-execution_count="45">
+<div class="sourceCode cell-code" id="cb52"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb52-1"><a href="#cb52-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_spot, train_dataset<span class="op">=</span>train,</span>
+<span id="cb52-2"><a href="#cb52-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb52-3"><a href="#cb52-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb52-4"><a href="#cb52-4" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">True</span>,</span>
+<span id="cb52-5"><a href="#cb52-5" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE,</span>
+<span id="cb52-6"><a href="#cb52-6" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span><span class="va">None</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <pre class="{raw}"><code>Loss on hold-out set: 1.2267619131326675
 Accuracy on hold-out set: 0.58955
 Early stopping at epoch 13</code></pre>
-<div class="cell" data-execution_count="29">
-<div class="sourceCode cell-code" id="cb37"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb37-1"><a href="#cb37-1" aria-hidden="true" tabindex="-1"></a>test_saved(net<span class="op">=</span>model_spot, test_dataset<span class="op">=</span>test,</span>
-<span id="cb37-2"><a href="#cb37-2" aria-hidden="true" tabindex="-1"></a>            shuffle<span class="op">=</span><span class="va">False</span>, path<span class="op">=</span><span class="st">"model_spot_trained.pt"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>If <code>path</code> is set to a filename, e.g., <code>path = "model_spot_trained.pt"</code>, the weights of the trained model will be loaded from this file.</p>
+<div class="cell" data-execution_count="46">
+<div class="sourceCode cell-code" id="cb54"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb54-1"><a href="#cb54-1" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_spot, test_dataset<span class="op">=</span>test,</span>
+<span id="cb54-2"><a href="#cb54-2" aria-hidden="true" tabindex="-1"></a>            shuffle<span class="op">=</span><span class="va">False</span>,</span>
+<span id="cb54-3"><a href="#cb54-3" aria-hidden="true" tabindex="-1"></a>            loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb54-4"><a href="#cb54-4" aria-hidden="true" tabindex="-1"></a>            metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb54-5"><a href="#cb54-5" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> DEVICE)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <pre class="{raw}"><code>Loss on hold-out set: 1.242568492603302
 Accuracy on hold-out set: 0.5957</code></pre>
 </section>
 <section id="comparison-with-default-hyperparameters-and-ray-tune" class="level2">
 <h2 class="anchored" data-anchor-id="comparison-with-default-hyperparameters-and-ray-tune">Comparison with Default Hyperparameters and Ray Tune</h2>
-<p><a href="#tbl-comparison">Table&nbsp;4</a> shows the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from <code>ray[tune]</code>.</p>
+<p><a href="#tbl-comparison">Table&nbsp;5</a> shows the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from <code>ray[tune]</code>.</p>
 <div id="tbl-comparison" class="anchored">
 <table class="table">
-<caption>Table&nbsp;4: Comparison of the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from <code>ray[tune]</code>. <code>ray[tune]</code> only shows the validation loss, because training loss is not reported by <code>ray[tune]</code>.</caption>
+<caption>Table&nbsp;5: Comparison of the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from <code>ray[tune]</code>. <code>ray[tune]</code> only shows the validation loss, because training loss is not reported by <code>ray[tune]</code>.</caption>
 <colgroup>
 <col style="width: 16%">
 <col style="width: 25%">
 <col style="width: 30%">
 <col style="width: 13%">
 <col style="width: 14%">
 </colgroup>
@@ -1227,68 +1749,68 @@
 </div>
 </section>
 <section id="detailed-hyperparameter-plots" class="level2">
 <h2 class="anchored" data-anchor-id="detailed-hyperparameter-plots">Detailed Hyperparameter Plots</h2>
 <p>The contour plots in this section visualize the interactions of the three most important hyperparameters, <code>l1</code>, <code>l2</code>, and <code>epochs</code>, and <code>optimizer</code> of the surrogate model used to optimize the hyperparameters. Since some of these hyperparameters take fatorial or integer values, sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook <span class="citation" data-cites="bart23e">(<a href="#ref-bart23e" role="doc-biblioref">Bartz-Beielstein 2023</a>)</span>.</p>
 <div id="fig-contour" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<div class="sourceCode cell-code" id="cb39"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb39-1"><a href="#cb39-1" aria-hidden="true" tabindex="-1"></a>threshold <span class="op">=</span> <span class="fl">0.025</span></span>
-<span id="cb39-2"><a href="#cb39-2" aria-hidden="true" tabindex="-1"></a>impo <span class="op">=</span> spot_tuner.print_importance(threshold<span class="op">=</span>threshold, print_screen<span class="op">=</span><span class="va">True</span>)</span>
-<span id="cb39-3"><a href="#cb39-3" aria-hidden="true" tabindex="-1"></a>var_plots <span class="op">=</span> [i <span class="cf">for</span> i, x <span class="kw">in</span> <span class="bu">enumerate</span>(impo) <span class="cf">if</span> x[<span class="dv">1</span>] <span class="op">&gt;</span> threshold]</span>
-<span id="cb39-4"><a href="#cb39-4" aria-hidden="true" tabindex="-1"></a>min_z <span class="op">=</span> <span class="bu">min</span>(spot_tuner.y)</span>
-<span id="cb39-5"><a href="#cb39-5" aria-hidden="true" tabindex="-1"></a>max_z <span class="op">=</span> <span class="bu">max</span>(spot_tuner.y)</span>
-<span id="cb39-6"><a href="#cb39-6" aria-hidden="true" tabindex="-1"></a>n <span class="op">=</span> spot_tuner.k</span>
-<span id="cb39-7"><a href="#cb39-7" aria-hidden="true" tabindex="-1"></a><span class="cf">for</span> i <span class="kw">in</span> var_plots:</span>
-<span id="cb39-8"><a href="#cb39-8" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> j <span class="kw">in</span> var_plots:</span>
-<span id="cb39-9"><a href="#cb39-9" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> j <span class="op">&gt;</span> i:</span>
-<span id="cb39-10"><a href="#cb39-10" aria-hidden="true" tabindex="-1"></a>            filename <span class="op">=</span> <span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_contour_"</span><span class="op">+</span><span class="bu">str</span>(i)<span class="op">+</span><span class="st">"_"</span><span class="op">+</span><span class="bu">str</span>(j)<span class="op">+</span><span class="st">".pdf"</span></span>
-<span id="cb39-11"><a href="#cb39-11" aria-hidden="true" tabindex="-1"></a>            spot_tuner.plot_contour(i<span class="op">=</span>i, j<span class="op">=</span>j, min_z<span class="op">=</span>min_z, max_z <span class="op">=</span> max_z, filename<span class="op">=</span>filename)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb56"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb56-1"><a href="#cb56-1" aria-hidden="true" tabindex="-1"></a>threshold <span class="op">=</span> <span class="fl">0.025</span></span>
+<span id="cb56-2"><a href="#cb56-2" aria-hidden="true" tabindex="-1"></a>impo <span class="op">=</span> spot_tuner.print_importance(threshold<span class="op">=</span>threshold, print_screen<span class="op">=</span><span class="va">True</span>)</span>
+<span id="cb56-3"><a href="#cb56-3" aria-hidden="true" tabindex="-1"></a>var_plots <span class="op">=</span> [i <span class="cf">for</span> i, x <span class="kw">in</span> <span class="bu">enumerate</span>(impo) <span class="cf">if</span> x[<span class="dv">1</span>] <span class="op">&gt;</span> threshold]</span>
+<span id="cb56-4"><a href="#cb56-4" aria-hidden="true" tabindex="-1"></a>min_z <span class="op">=</span> <span class="bu">min</span>(spot_tuner.y)</span>
+<span id="cb56-5"><a href="#cb56-5" aria-hidden="true" tabindex="-1"></a>max_z <span class="op">=</span> <span class="bu">max</span>(spot_tuner.y)</span>
+<span id="cb56-6"><a href="#cb56-6" aria-hidden="true" tabindex="-1"></a>n <span class="op">=</span> spot_tuner.k</span>
+<span id="cb56-7"><a href="#cb56-7" aria-hidden="true" tabindex="-1"></a><span class="cf">for</span> i <span class="kw">in</span> var_plots:</span>
+<span id="cb56-8"><a href="#cb56-8" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> j <span class="kw">in</span> var_plots:</span>
+<span id="cb56-9"><a href="#cb56-9" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> j <span class="op">&gt;</span> i:</span>
+<span id="cb56-10"><a href="#cb56-10" aria-hidden="true" tabindex="-1"></a>            filename <span class="op">=</span> <span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_contour_"</span><span class="op">+</span><span class="bu">str</span>(i)<span class="op">+</span><span class="st">"_"</span><span class="op">+</span><span class="bu">str</span>(j)<span class="op">+</span><span class="st">".png"</span></span>
+<span id="cb56-11"><a href="#cb56-11" aria-hidden="true" tabindex="-1"></a>            spot_tuner.plot_contour(i<span class="op">=</span>i, j<span class="op">=</span>j, min_z<span class="op">=</span>min_z, max_z <span class="op">=</span> max_z, filename<span class="op">=</span>filename)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 <figcaption class="figure-caption">Figure&nbsp;4: <strong>?(caption)</strong></figcaption>
 </figure>
 </div>
 <div id="fig-contour-0-1" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;5: Contour plot of the loss as a function of <code>l1</code> and <code>l2</code>, i.e., the number of neurons in the layers.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-0-3" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;6: Contour plot of the loss as a function of the number of epochs and the neurons in layer <code>l1</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-0-4" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;7: Contour plot of the loss as a function of the optimizer and the neurons in layer <code>l1</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-1-3" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;8: Contour plot of the loss as a function of the number of epochs and the neurons in layer <code>l2</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-1-3" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;9: Contour plot of the loss as a function of the optimizer and the neurons in layer <code>l2</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-3-4" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<p><embed src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf" class="img-fluid"></p>
+<p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;10: Contour plot of the loss as a function of the optimizer and the number of epochs.</figcaption>
 </figure>
 </div>
 <p><a href="#fig-contour-0-1">Figure&nbsp;5</a> to <a href="#fig-contour-3-4">Figure&nbsp;10</a> show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. <code>spotPython</code> provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, <a href="#fig-parallel">Figure&nbsp;12</a> shows the parallel plot of the hyperparameters.</p>
 <div id="fig-parallel" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<div class="sourceCode cell-code" id="cb40"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb40-1"><a href="#cb40-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.parallel_plot()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb57"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb57-1"><a href="#cb57-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.parallel_plot()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 <figcaption class="figure-caption">Figure&nbsp;11: <strong>?(caption)</strong></figcaption>
 </figure>
 </div>
 <div id="fig-parallel" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/parallel.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;12: Parallel plot</figcaption>
@@ -1393,15 +1915,15 @@
 
 <div id="quarto-appendix" class="default"><section id="footnotes" class="footnotes footnotes-end-of-document" role="doc-endnotes"><h2 class="anchored quarto-appendix-heading">Footnotes</h2>
 
 <ol>
 <li id="fn1"><p><a href="https://github.com/sequential-parameter-optimization">https://github.com/sequential-parameter-optimization</a><a href="#fnref1" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 <li id="fn2"><p>Alternatively, the source code can be downloaded from gitHub: <a href="https://github.com/sequential-parameter-optimization/spotPython">https://github.com/sequential-parameter-optimization/spotPython</a>.<a href="#fnref2" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 <li id="fn3"><p>We were not able to install <code>Ray Tune</code> on our system. Therefore, we used the results from the <code>PyTorch</code> tutorial.<a href="#fnref3" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn4"><p>The key <code>"metric"</code> is used for the river based evaluation <span class="citation" data-cites="mont20a">(<a href="#ref-mont20a" role="doc-biblioref">Montiel et al. 2021</a>)</span> via <code>eval_oml_iter_progressive</code>.<a href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn4"><p><a href="https://torchmetrics.readthedocs.io/en/latest/">https://torchmetrics.readthedocs.io/en/latest/.</a><a href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 </ol>
 </section></div></main> <!-- /main -->
 <script id="quarto-html-after-body" type="application/javascript">
 window.document.addEventListener("DOMContentLoaded", function (event) {
   const toggleBodyColorMode = (bsSheetEl) => {
     const mode = bsSheetEl.getAttribute("data-mode");
     const bodyEl = window.document.querySelector("body");
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 
 
 
 ***** Other Formats *****
     * PDF
 
 ****** PyTorch Hyperparameter Tuning â A Tutorial for spotPython ******
-Version 0.1.3
+Version 0.2.0
 Author
 Affiliations
 Thomas_Bartz-Beielstein [data:image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/
 9hAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA2ZpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/
 eHBhY2tldCBiZWdpbj0i77u/
 IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuMC1jMDYwIDYxLjEzNDc3NywgMjAxMC8wMi8xMi0xNzozMjowMCAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDo1N0NEMjA4MDI1MjA2ODExOTk0QzkzNTEzRjZEQTg1NyIgeG1wTU06RG9jdW1lbnRJRD0ieG1wLmRpZDozM0NDOEJGNEZGNTcxMUUxODdBOEVCODg2RjdCQ0QwOSIgeG1wTU06SW5zdGFuY2VJRD0ieG1wLmlpZDozM0NDOEJGM0ZGNTcxMUUxODdBOEVCODg2RjdCQ0QwOSIgeG1wOkNyZWF0b3JUb29sPSJBZG9iZSBQaG90b3Nob3AgQ1M1IE1hY2ludG9zaCI+IDx4bXBNTTpEZXJpdmVkRnJvbSBzdFJlZjppbnN0YW5jZUlEPSJ4bXAuaWlkOkZDN0YxMTc0MDcyMDY4MTE5NUZFRDc5MUM2MUUwNEREIiBzdFJlZjpkb2N1bWVudElEPSJ4bXAuZGlkOjU3Q0QyMDgwMjUyMDY4MTE5OTRDOTM1MTNGNkRBODU3Ii8+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+84NovQAAAR1JREFUeNpiZEADy85ZJgCpeCB2QJM6AMQLo4yOL0AWZETSqACk1gOxAQN+cAGIA4EGPQBxmJA0nwdpjjQ8xqArmczw5tMHXAaALDgP1QMxAGqzAAPxQACqh4ER6uf5MBlkm0X4EGayMfMw/
@@ -143,24 +143,24 @@
 with Ray Tuneâ from the PyTorch documentation (PyTorch_2023a), which is an
 extension of the tutorial âTraining a Classifierâ (PyTorch_2023b) for
 training a CIFAR10 image classifier.
 This document refers to the following software versions:
     * python: 3.10.10
     * torch: 2.0.1
     * torchvision: 0.15.0
-    * spotPython: 0.1.3
+    * spotPython: 0.2.0
 spotPython can be installed via pip2.
 !pip install spotPython
 Results that refer to the Ray Tune package are taken from https://PyTorch.org/
 tutorials/beginner/hyperparameter_tuning_tutorial.html3.
 ***** Setup *****
 Before we consider the detailed experimental setup, we select the parameters
 that affect run time, initial design size and the device that is used.
 MAX_TIME = 60
-INIT_SIZE = 10
+INIT_SIZE = 20
 DEVICE = "cpu" # "cuda:0"
 
 ***** Initialization of the fun_control Dictionary *****
 spotPython uses a Python dictionary for storing the information required for
 the hyperparameter tuning process. This dictionary is called fun_control and is
 initialized with the function fun_control_init. The function fun_control_init
 returns a skeleton dictionary. The dictionary is filled with the required
@@ -253,17 +253,18 @@
 
 **** Implementing a Configurable Neural Network With spotPython ****
 spotPython implements a class which is similar to the class described in the
 PyTorch tutorial. The class is called Net_CIFAR10 and is implemented in the
 file netcifar10.py.
 import spotPython.torch.netcore as netcore
 class Net_CIFAR10(netcore.Net_Core):
-    def __init__(self, l1, l2, lr, batch_size, epochs, k_folds, patience):
+    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):
         super(Net_CIFAR10, self).__init__(
-            lr=lr, batch_size=batch_size, epochs=epochs, k_folds=k_folds,
+            lr_mult=lr_mult, batch_size=batch_size, epochs=epochs,
+k_folds=k_folds,
             patience=patience
         )
         self.conv1 = nn.Conv2d(3, 6, 5)
         self.pool = nn.MaxPool2d(2, 2)
         self.conv2 = nn.Conv2d(6, 16, 5)
         self.fc1 = nn.Linear(16 * 5 * 5, l1)
         self.fc2 = nn.Linear(l1, l2)
@@ -275,37 +276,38 @@
         x = x.view(-1, 16 * 5 * 5)
         x = F.relu(self.fc1(x))
         x = F.relu(self.fc2(x))
         x = self.fc3(x)
         return x
 Net_CIFAR10 inherits from the class Net_Core which is implemented in the file
 netcore.py. It implements the additional attributes that are common to all
-neural network models. The attributes are the learning rate lr, the batch size
-batch_size, the number of epochs epochs, the number of folds k_folds for the
-cross validation, and the patience patience for the early stopping. The class
-Net_Core is shown below.
+neural network models. The attributes are the learning rate multiplier lr_mult,
+the batch size batch_size, the number of epochs epochs, the number of folds
+k_folds for the cross validation, and the patience patience for the early
+stopping. The class Net_Core is shown below.
 from torch import nn
 
 
 class Net_Core(nn.Module):
-    def __init__(self, lr, batch_size, epochs, k_folds, patience):
+    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):
         super(Net_Core, self).__init__()
-        self.lr = lr
+        self.lr_mult = lr_mult
         self.batch_size = batch_size
         self.epochs = epochs
         self.k_folds = k_folds
         self.patience = patience
 
 **** Comparison of the Approach Described in the PyTorch Tutorial With
 spotPython ****
 Comparing the class Net from the PyTorch tutorial and the class Net_CIFAR10
 from spotPython, we see that the class Net_CIFAR10 has additional attributes
 and does not inherit from nn directly. It adds an additional class, Net_core,
 that takes care of additional attributes that are common to all neural network
-models, e.g., the learning rate lr or the batch size batch_size.
+models, e.g., the learning rate multiplier lr_mult or the batch size
+batch_size.
 spotPythonâs core_model implements an instance of the Net_CIFAR10 class. In
 addition to the basic neural network model, the core_model can use these
 additional attributes. spotPython provides methods for handling these
 additional attributes to guarantee 100% compatibility with the PyTorch classes.
 The method add_core_model_to_fun_control adds the hyperparameters and
 additional attributes to the fun_control dictionary. The method is shown below.
 core_model = Net_CIFAR10
@@ -317,16 +319,15 @@
 In addition to the class Net from the PyTorch tutorial, the class Net_CIFAR10
 has additional attributes, e.g.:
     * learning rate (lr),
     * batch size (batch_size),
     * epochs (epochs),
     * k_folds (k_folds), and
     * early stopping criterion âpatienceâ (patience)
-Further attributes can be easily added to the class, e.g., optimizer or
-loss_function.
+Further attributes can be easily added to the class, e.g., optimizer.
 
 ***** The Search Space *****
 In Section 3.6.1, we first describe how to configure the search space with ray
 [tune] (as shown in PyTorch (2023a)) and then how to configure the search space
 with spotPython in Section 3.6.2.
 **** Configuring the Search Space With Ray Tune ****
 Ray Tuneâs search space can be configured as follows (PyTorch_2023a):
@@ -376,20 +377,20 @@
             "upper": 9},
         "l2": {
             "type": "int",
             "default": 5,
             "transform": "transform_power_2_int",
             "lower": 2,
             "upper": 9},
-        "lr": {
+        "lr_mult": {
             "type": "float",
-            "default": 1e-03,
+            "default": 1.0,
             "transform": "None",
-            "lower": 1e-05,
-            "upper": 1e-02},
+            "lower": 0.1,
+            "upper": 10},
         "batch_size": {
             "type": "int",
             "default": 4,
             "transform": "transform_power_2_int",
             "lower": 1,
             "upper": 4},
         "epochs": {
@@ -427,43 +428,20 @@
             "type": "factor",
             "default": "SGD",
             "transform": "None",
             "class_name": "torch.optim",
             "core_model_parameter_type": "str",
             "lower": 0,
             "upper": 12},
-        "criterion": {
-            "levels": ["L1Loss",
-                       "MSELoss",
-                       "CrossEntropyLoss",
-                       "CTCLoss",
-                       "NLLLoss",
-                       "PoissonNLLLoss",
-                       "GaussianNLLLoss",
-                       "KLDivLoss",
-                       "BCELoss",
-                       "BCEWithLogitsLoss",
-                       "MarginRankingLoss",
-                       "HingeEmbeddingLoss",
-                       "MultiLabelMarginLoss",
-                       "HuberLoss",
-                       "SmoothL1Loss",
-                       "SoftMarginLoss",
-                       "MultiLabelSoftMarginLoss",
-                       "CosineEmbeddingLoss",
-                       "MultiMarginLoss",
-                       "TripletMarginLoss",
-                       "TripletMarginWithDistanceLoss"],
-            "type": "factor",
-            "default": "CrossEntropyLoss",
+        "sgd_momentum": {
+            "type": "float",
+            "default": 0.0,
             "transform": "None",
-            "class_name": "torch.nn",
-            "core_model_parameter_type": "instance()",
-            "lower": 0,
-            "upper": 20}
+            "lower": 0.0,
+            "upper": 1.0}
     }
 }
 
 ***** Modifying the Hyperparameters *****
 Ray tune (PyTorch_2023a) does not provide a way to change the specified
 hyperparameters without re-compilation. However, spotPython provides functions
 for modifying the hyperparameters, their bounds and factors as well as for
@@ -504,74 +482,80 @@
 "Adam"])
 The hyperparameter optimizer can be de-activated by choosing only one value
 (level), here: "SGD".
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
 As discussed in Section 3.7.4, there are some issues with the LBFGS optimizer.
 Therefore, the usage of the LBFGS optimizer is not deactivated in spotPython by
 default. However, the LBFGS optimizer can be activated by adding it to the list
-of optimizers. Rprop was remmoved, because it does perform very poorly (as some
+of optimizers. Rprop was removed, because it does perform very poorly (as some
 pre-tests have shown). However, it can also be activated by adding it to the
 list of optimizers. Since SparseAdam does not support dense gradients, Adam was
 used instead. Therefore, there are 10 default optimizers:
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer",
 ["Adadelta",
      "Adagrad", "Adam", "AdamW", "Adamax", "ASGD", "NAdam", "RAdam",
       "RMSprop", "SGD"])
 
 **** Optimizers ****
 Table 1 shows some of the optimizers available in PyTorch:
-   Table 1: Optimizers available in PyTorch (selection). âmomâ denotes
-    momentum, âweightâ weight_decay, âdampâ dampening, ânestâ
-nesterov, and âlr_scâ learning rate for scaling delta. The default values
-                           are shown in the table.
-Optimizer  lr       mom    weight damp   nest  rho    lr_sc  lr_decay betas
-SGD        required float: float: float: bool: -      -      -        -
-                    0      0      0      False
-Adadelta   -        -      float: -      -     float: float: -        -
-                           0                   0.9    1.0
-Adagrad    float:   -      float: -      -     -      -      float: 0 -
-           1e-2            0
-                                                                      Tuple
-           float:          float:                                     [float,
-Adam       1e-3     -      0      -      -     -      -      -        float]:
-                                                                      (0.9,
-                                                                      0.999)
-                                                                      Tuple
-           float:          float:                                     [float,
-AdamW      1e-3     -      1e-2   -      -     -      -      -        float]:
-                                                                      (0.9,
-                                                                      0.999)
-                                                                      Tuple
-           float:                                                     [float,
-SparseAdam 1e-3     -      -      -      -     -      -      -        float]:
-                                                                      (0.9,
-                                                                      0.999)
+ Table 1: Optimizers available in PyTorch (selection). âmomâ denotes momentum, âweightâ weight_decay,
+  âdampâ dampening, ânestâ nesterov, âlr_scâ learning rate for scaling delta, âmom_decâ for
+         momentum_decay, and âstep_sâ for step_sizes. The default values are shown in the table.
+Optimizer  lr       mom weight damp nest  rho lr_sc lr_decay betas       lambd alpha     mom_decay etas step_s
+Adadelta   -        -   0.     -    -     0.9 1.0   -        -           -     -         -         -    -
+Adagrad    1e-2     -   0.     -    -     -   -     0.       -           -     -         -         -    -
+Adam       1e-3     -   0.     -    -     -   -     -        (0.9,0.999) -     -         -         -    -
+AdamW      1e-3     -   1e-2   -    -     -   -     -        (0.9,0.999) -     -         -         -    -
+SparseAdam 1e-3     -   -      -    -     -   -     -        (0.9,0.999) -     -         -         -    -
+Adamax     2e-3     -   0.     -    -     -   -     -        (0.9,       -     -         -         -    -
+                                                             0.999)
+ASGD       1e-2     0.9 0.     -    False -   -     -        -           1e-4  0.75      -         -    -
+LBFGS      1.       -   -      -    -     -   -     -        -           -     -         -         -    -
+NAdam      2e-3     -   0.     -    -     -   -     -        (0.9,0.999) -     -         0         -    -
+RAdam      1e-3     -   0.     -    -     -   -     -        (0.9,0.999) -     -         -         -    -
+RMSprop    1e-2     0.  0.     -    -     -   -     -        (0.9,0.999) -     -         -         -    -
+Rprop      1e-2     -   -      -    -     -   -     -        -           -     (0.5,1.2) (1e-6,    -    -
+                                                                                         50)
+SGD        required 0.  0.     0.   False -   -     -        -           -     -         -         -    -
 spotPython implements an optimization handler that maps the optimizer names to
 the corresponding PyTorch optimizers.
 A note on LBFGS
-PyTorchâs LBFGS optimizer is deactivated in spotPython by default, because it
-does not perform very well. The PyTorch documentation, see https://pytorch.org/
-docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS, states:
+We recommend deactivating PyTorchâs LBFGS optimizer, because it does not
+perform very well. The PyTorch documentation, see https://pytorch.org/docs/
+stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS, states:
      This is a very memory intensive optimizer (it requires additional
      param_bytes * (history_size + 1) bytes). If it doesnât fit in
      memory try reducing the history size, or use a different algorithm.
 Furthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial.
 The reason is that the LBFGS optimizer requires the closure function, which is
 not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is
 recommended here.
 Since there are 10 optimizers in the portfolio, it is not recommended tuning
-the hyperparameters that effect one single optimizer only. Thus, the learning
-rate, which affects the SGD optimizer, will be set to a fixed value. We choose
-the default value of 1e-3 for the learning rate, because it is used in other
-PyTorch examples. We recommend tuning the learning rate later, when a reduced
-set of optimizers is fixed. Here, we will demonstrate how to select in a
-screening phase the optimizers that should be used for the hyperparameter
-tuning.
-fun_control = modify_hyper_parameter_bounds(fun_control, "lr", bounds=[1e-3,
-1e-3])
+the hyperparameters that effect one single optimizer only.
+A note on the learning rate
+spotPython provides a multiplier for the default learning rates, because
+optimizers use different learning rates. Using a multiplier for the learning
+rates might enable a simultaneous tuning of the learning rates for all
+optimizers. However, this is not recommended, because the learning rates are
+not comparable across optimizers. Therefore, we recommend fixing the learning
+rate for all optimizers if multiple optimizers are used. This can be done by
+setting the lower and upper bounds of the learning rate multiplier to the same
+value as shown below.
+Thus, the learning rate, which affects the SGD optimizer, will be set to a
+fixed value. We choose the default value of 1e-3 for the learning rate, because
+it is used in other PyTorch examples (it is also the default value used by
+spotPython as defined in the optimizer_handler() method). We recommend tuning
+the learning rate later, when a reduced set of optimizers is fixed. Here, we
+will demonstrate how to select in a screening phase the optimizers that should
+be used for the hyperparameter tuning.
+For the same reason, we will fix the sgd_momentum to 0.9.
+fun_control = modify_hyper_parameter_bounds(fun_control, "lr_mult", bounds=
+[1.0, 1.0])
+fun_control = modify_hyper_parameter_bounds(fun_control, "sgd_momentum",
+bounds=[0.9, 0.9])
 
 ***** Evaluation *****
 The evaluation procedure requires the specification of two elements:
    1. the way how the data is split into a train and a test set and
    2. the loss function (and a metric).
 **** Hold-out Data Split and Cross-Validation ****
 As a default, spotPython provides a standard hold-out data split and cross
@@ -595,17 +579,17 @@
 training is performed on the training data set. The test data set is used for
 the final evaluation of the model.
 Summarizing, the following splits are performed in the hold-out setting:
    1. Run spotPython with eval set to train_hold_out to determine the best
       hyperparameter configuration.
    2. Train the model with the best hyperparameter configuration on the
       training data set:
-          o train_save(model_spot, train, "model_spot.pt").
+          o train_tuned(model_spot, train, "model_spot.pt").
    3. Test the model on the test data:
-          o test_saved(model_spot, test, "model_spot.pt")
+          o test_tuned(model_spot, test, "model_spot.pt")
 These steps will be exemplified in the following sections.
 In addition to this hold-out setting, spotPython provides another hold-out
 setting, where an explicit test data is specified by the user that will be used
 as the validation set. To choose this option, the eval parameter is set to
 test_hold_out. In this case, the training data set is used for the model
 training. Then, the explicitly defined test data set is used for the evaluation
 of the hyperparameter configuration (the validation).
@@ -617,91 +601,405 @@
 \(k\) times, so that each fold is used exactly once for evaluation. The final
 evaluation is performed on the test data set. The cross validation setting is
 useful for small data sets, because it allows to use all data for training and
 evaluation. However, it is computationally expensive, because the model has to
 be trained \(k\) times.
 Note
 Combinations of the above settings are possible, e.g., cross validation can be
-used for training and hold-out for evaluation or . Also, cross validation can
-be used for training and testing. Because cross validation is not used in the
-PyTorch tutorial (PyTorch_2023a), it is not considered further here.
+used for training and hold-out for evaluation or vice versa. Also, cross
+validation can be used for training and testing. Because cross validation is
+not used in the PyTorch tutorial (PyTorch_2023a), it is not considered further
+here.
+
+*** Overview of the Evaluation Settings ***
+** Settings for the Hyperparameter Tuning **
+Table 2 provides an overview of the training evaluations.
+                         Table 2: Overview of the evaluation settings.
+eval             train         test          function                  comment
+                 \                           train_hold_out(),         splits the train data set
+"train_hold_out" (\checkmark\)               validate_fold_or_hold_out internally
+                                             () for early stopping
+                 \             \             train_hold_out(),         use the test data set for
+"test_hold_out"  (\checkmark\) (\checkmark\) validate_fold_or_hold_out validate_fold_or_hold_out
+                                             () for early stopping     ()
+"train_cv"       \                           evaluate_cv(net, train)   CV using the train data
+                 (\checkmark\)                                         set
+                                                                       CV using the test data
+"test_cv"                      \             evaluate_cv(net, test)    set . Identical to
+                               (\checkmark\)                           "train_cv", uses only
+                                                                       test data.
+    * "train_cv" and "test_cv" use sklearn.model_selection.KFold() internally.
+
+*** Detailed Description of the "train_hold_out" Setting ***
+The "train_hold_out" setting is used by default. It uses the loss function
+specfied in fun_control and the metric specified in fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as
+      follows:
+df_eval, _ = evaluate_hold_out(
+    model,
+    train_dataset=fun_control["train"],
+    shuffle=self.fun_control["shuffle"],
+    loss_function=self.fun_control["loss_function"],
+    metric=self.fun_control["metric_torch"],
+    device=self.fun_control["device"],
+    show_batch_interval=self.fun_control["show_batch_interval"],
+    path=self.fun_control["path"],
+)
+Note: Only the data set fun_control["train"] is used for training and
+validation. It is used as follows:
+trainloader, valloader = create_train_val_data_loaders(
+                dataset=train_dataset, batch_size=batch_size_instance,
+shuffle=shuffle
+            )
+create_train_val_data_loaders() splits the train_dataset into trainloader and
+valloader using torch.utils.data.random_split() as follows:
+def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
+    test_abs = int(len(dataset) * 0.6)
+    train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) -
+test_abs])
+    trainloader = torch.utils.data.DataLoader(
+        train_subset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    valloader = torch.utils.data.DataLoader(
+        val_subset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    return trainloader, valloader
+The optimizer is set up as follows:
+lr_mult_instance = net.lr_mult
+optimizer = optimizer_handler(optimizer_name=optimizer_instance,
+params=net.parameters(), lr_mult=lr_mult_instance)
+   1. evaluate_hold_out() sets the net attributes such as epochs, batch_size,
+      optimizer, and patience. For each epoch, the methods train_hold_out() and
+      validate_fold_or_hold_out() are called, the former for training and the
+      latter for validation and early stopping. The validation loss from the
+      last epoch (not the best validation loss) is returned from
+      evaluate_hold_out.
+   2. The method train_hold_out() is implemented as follows:
+def train_hold_out(net, trainloader, batch_size, loss_function, optimizer,
+device, show_batch_interval=10_000):
+    running_loss = 0.0
+    epoch_steps = 0
+    for i, data in enumerate(trainloader, 0):
+        inputs, labels = data
+        inputs, labels = inputs.to(device), labels.to(device)
+        optimizer.zero_grad()
+        outputs = net(inputs)
+        loss = loss_function(outputs, labels)
+        loss.backward()
+        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
+        optimizer.step()
+        running_loss += loss.item()
+        epoch_steps += 1
+        if i % show_batch_interval == (show_batch_interval - 1):  # print every
+show_batch_interval mini-batches
+            print(
+                "Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
+                % (i + 1, int(batch_size), running_loss / epoch_steps)
+            )
+            running_loss = 0.0
+    return loss.item()
+   1. The method validate_fold_or_hold_out() is implemented as follows:
+def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
+    val_loss = 0.0
+    val_steps = 0
+    metric.reset()
+    for i, data in enumerate(valloader, 0):
+        with torch.no_grad():
+            inputs, labels = data
+            inputs, labels = inputs.to(device), labels.to(device)
+            outputs = net(inputs)
+            _, predicted = torch.max(outputs.data, 1)
+            metric_value = metric(predicted, labels).to(device)
+            loss = loss_function(outputs, labels)
+            val_loss += loss.cpu().numpy()
+            val_steps += 1
+    loss = val_loss / val_steps
+    metric_value = metric.compute()
+    return metric_value, loss
+
+*** Detailed Description of the "test_hold_out" Setting ***
+It uses the loss function specfied in fun_control and the metric specified in
+fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar
+      to the "train_hold_out" setting with one exception: It passes an
+      additional test data set to evaluate_hold_out() as follows:
+test_dataset=fun_control["test"]
+evaluate_hold_out() calls create_train_test_data_loaders instead of
+create_train_val_data_loaders as follows: The two data sets are used in
+create_train_test_data_loaders as follows:
+def create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset,
+num_workers=0):
+    trainloader = torch.utils.data.DataLoader(
+        dataset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    testloader = torch.utils.data.DataLoader(
+        test_dataset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    return trainloader, testloader
+   1. The following steps are identical to the "train_hold_out" setting. Only a
+      different data loader is used for testing.
+
+*** Detailed Description of the "train_cv" Setting ***
+It uses the loss function specfied in fun_control and the metric specified in
+fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
+df_eval, _ = evaluate_cv(
+    model,
+    dataset=fun_control["train"],
+    shuffle=self.fun_control["shuffle"],
+    device=self.fun_control["device"],
+    show_batch_interval=self.fun_control["show_batch_interval"],
+)
+Note: Only the data set fun_control["train"] is used for CV. 3. In `evaluate_cv
+(), the following steps are performed: The optimizer is set up as follows:
+lr_instance = net.lr
+optimizer = optimizer_handler(optimizer_name=optimizer_instance,
+params=net.parameters(), lr_mult=lr_mult_instance)
+evaluate_cv() sets the net attributes such as epochs, batch_size, optimizer,
+and patience. CV is implemented as follows:
+kfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)
+for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
+    train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
+    val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
+    trainloader = torch.utils.data.DataLoader(
+        dataset, batch_size=batch_size_instance, sampler=train_subsampler,
+num_workers=num_workers
+    )
+    valloader = torch.utils.data.DataLoader(
+        dataset, batch_size=batch_size_instance, sampler=val_subsampler,
+num_workers=num_workers
+    )
+    reset_weights(net)
+    # Train fold for several epochs:
+    train_fold(
+        net,
+        trainloader,
+        epochs_instance,
+        loss_function,
+        optimizer,
+        device,
+        show_batch_interval=show_batch_interval,
+    )
+    # Validate fold: use only loss for tuning
+    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net,
+valloader, loss_function, device)
+df_eval = sum(loss_values.values()) / len(loss_values.values())
+   1. The method train_fold() is implemented as follows:
+def train_fold(net, trainloader, epochs, loss_function, optimizer, device,
+show_batch_interval=10_000):
+    for epoch in range(epochs):
+        print(f"Epoch: {epoch + 1}")
+        running_loss = 0.0
+        epoch_steps = 0
+        for i, data in enumerate(trainloader, 0):
+            inputs, labels = data
+            inputs, labels = inputs.to(device), labels.to(device)
+            optimizer.zero_grad()
+            outputs = net(inputs)
+            loss = loss_function(outputs, labels)
+            loss.backward()
+            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
+            optimizer.step()
+            # the following is for printing the statistic only
+            running_loss += loss.item()
+            epoch_steps += 1
+            if i % show_batch_interval == (show_batch_interval - 1):  # print
+every show_batch_interval mini-batches
+                print("Batch: %5d. Training Loss (running): %.3f" % (i + 1,
+running_loss / epoch_steps))
+                running_loss = 0.0
+   1. The method validate_fold_or_hold_out() is implemented as shown above. In
+      contrast to the hold-out setting, it is called for each of the \(k\)
+      folds. The results are stored in a dictionaries metric_values and
+      loss_values as follows:
+    # Validate fold: use only loss for tuning
+    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net,
+valloader, loss_function, device)
+df_eval = sum(loss_values.values()) / len(loss_values.values())
+The results are averaged over the \(k\) folds and returned as df_eval.
+
+*** Detailed Description of the "test_cv" Setting ***
+It uses the loss function specfied in fun_control and the metric specified in
+fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
+df_eval, _ = evaluate_cv(
+    model,
+    dataset=fun_control["test"],
+    shuffle=self.fun_control["shuffle"],
+    device=self.fun_control["device"],
+    show_batch_interval=self.fun_control["show_batch_interval"],
+)
+Note: The data set fun_control["test"] is used for CV. The rest is the same as
+for the "train_cv" setting.
+
+*** Settings for the Final Evaluation of the Tuned Architecture ***
+** Training of the Tuned Architecture **
+train_tuned(model, train): train the model with the best hyperparameter
+configuration (or simply the default) on the training data set. It splits the
+traindata into new train and validation sets using
+create_train_val_data_loaders(), which calls torch.utils.data.random_split()
+internally. Currently, 60% of the data is used for training and 40% for
+validation. The train data is used for training the model with train_hold_out
+(). The validation data is used for early stopping using
+validate_fold_or_hold_out() on the validation data set.
+train_tuned() is just a wrapper to evaluate_hold_out using the train data set.
+It is implemented as follows:
+def train_tuned(net, train_dataset, shuffle, loss_function, metric,
+device=None, show_batch_interval=10_000, path=None):
+    evaluate_hold_out(
+        net=net,
+        train_dataset=train_dataset,
+        shuffle=shuffle,
+        test_dataset=None,
+        loss_function=loss_function,
+        metric=metric,
+        device=device,
+        show_batch_interval=show_batch_interval,
+        path=path,
+    )
+Note: During training, shuffle is set to True, whereas during testing, shuffle
+is set to False.
+
+** Testing of the Tuned Architecture **
+test_tuned(model, test): test the model on the test data set. No data splitting
+is performed. The (trained) model is evaluated using the
+validate_fold_or_hold_out() function.
+Note: During training, shuffle is set to True, whereas during testing, shuffle
+is set to False.
+def test_tuned(net, shuffle, test_dataset=None, loss_function=None,
+metric=None, device=None, path=None):
+    batch_size_instance = net.batch_size
+    removed_attributes, net = get_removed_attributes_and_base_net(net)
+    if path is not None:
+        net.load_state_dict(torch.load(path))
+        net.eval()
+    try:
+        device = getDevice(device=device)
+        if torch.cuda.is_available():
+            device = "cuda:0"
+            if torch.cuda.device_count() > 1:
+                print("We will use", torch.cuda.device_count(), "GPUs!")
+                net = nn.DataParallel(net)
+        net.to(device)
+        valloader = torch.utils.data.DataLoader(
+            test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle,
+num_workers=0
+        )
+        metric_value, loss = validate_fold_or_hold_out(
+            net, valloader=valloader, loss_function=loss_function,
+metric=metric, device=device
+        )
+        df_eval = loss
+        df_metric = metric_value
+        df_preds = np.nan
+    except Exception as err:
+        print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type
+(err)=}")
+        df_eval = np.nan
+        df_metric = np.nan
+        df_preds = np.nan
+    add_attributes(net, removed_attributes)
+    print(f"Final evaluation: Validation loss: {df_eval}")
+    print(f"Final evaluation: Validation metric: {df_metric}")
+    print("----------------------------------------------")
+    return df_eval, df_preds, df_metric
 
 **** Loss Functions and Metrics ****
-The key "criterion" specifies the loss function which is used during the
+The key "loss_function" specifies the loss function which is used during the
 optimization. There are several different loss functions under PyTorchâs nn
 package. For example, a simple loss is MSELoss, which computes the mean-squared
 error between the output and the target. In this tutorial we will use
 CrossEntropyLoss, because it is also used in the PyTorch tutorial.
-fun_control = modify_hyper_parameter_levels(fun_control, "criterion",
-["CrossEntropyLoss"])
+from torch.nn import CrossEntropyLoss
+loss_function = CrossEntropyLoss()
+fun_control.update({"loss_function": loss_function})
 In addition to the loss functions, spotPython provides access to a large number
 of metrics. The key "metric_sklearn" is used for metrics that follow the
-scikit-learn conventions4. Because the PyTorch tutorial uses the accuracy as
-metric, we use the same metric here. Currently, accuracy is computed in the
-tutorialâs example code. Therefore, we will use the same implementation here
-and set the key "metric_sklearn" to None.
+scikit-learn conventions. The key "river_metric" is used for the river based
+evaluation (Montiel_et_al._2021) via eval_oml_iter_progressive, and the key
+"metric_torch" is used for the metrics from TorchMetrics. TorchMetrics is a
+collection of more than 90 PyTorch metrics4. Because the PyTorch tutorial uses
+the accuracy as metric, we use the same metric here. Currently, accuracy is
+computed in the tutorialâs example code. We will use TorchMetrics instead,
+because it offers:
+    * A standardized interface to increase reproducibility
+    * Reduces Boilerplate
+    * Distributed-training compatible
+    * Rigorously tested
+    * Automatic accumulation over batches
+    * Automatic synchronization between multiple devices
+Therefore, we set
+metric_torch = torchmetrics.Accuracy(task="multiclass", num_classes=10)
+loss_function = CrossEntropyLoss()
 weights = 1.0
-criterion = CrossEntropyLoss
+metric_torch = torchmetrics.Accuracy(task="multiclass", num_classes=10)
 shuffle = True
 eval = "train_hold_out"
 device = DEVICE
 show_batch_interval = 100_000
-save_model = True
 path="torch_model.pt"
 
 fun_control.update({
                "data_dir": None,
                "checkpoint_dir": None,
                "horizon": None,
                "oml_grace_period": None,
                "weights": weights,
                "step": None,
                "log_level": 50,
                "weight_coeff": None,
-               "metric": None,
+               "metric_torch": metric_torch,
+               "metric_river": None,
                "metric_sklearn": None,
-               "criterion": criterion,
+               "loss_function": loss_function,
                "shuffle": shuffle,
                "eval": eval,
                "device": device,
                "show_batch_interval": show_batch_interval,
-               "save_model": save_model,
                "path": path,
                })
 
 ***** Calling the SPOT Function *****
 Now, the dictionary fun_control contains all information needed for the
 hyperparameter tuning. Before the hyperparameter tuning is started, it is
 recommended to take a look at the experimental design. The method
 gen_design_table generates a design table as follows:
 print(gen_design_table(fun_control))
 This allows to check if all information is available and if the information is
-correct. Table 2 shows the experimental design for the hyperparameter tuning.
+correct. Table 3 shows the experimental design for the hyperparameter tuning.
 Hyperparameter transformations are shown in the column âtransformâ, e.g.,
 the l1 default is 5, which results in the value \(2^5 = 32\) for the network,
 because the transformation transform_power_2_int was selected in the JSON file.
 The default value of the batch_size is set to 4, which results in a batch size
 of \(2^4 = 16\).
-  Table 2: Experimental design for the hyperparameter tuning. The
-table shows the hyperparameters, their types, default values, lower
-       and upper bounds, and the transformation function. The
-  transformation function is used to transform the hyperparameter
-     values from the unit hypercube to the original domain. The
-  transformation function is applied to the hyperparameter values
-          before the evaluation of the objective function.
-name       type   default          lower upper transform
-l1         int    5                2     9     transform_power_2_int
-l2         int    5                2     9     transform_power_2_int
-lr         float  0.001            0.001 0.001 None
-batch_size int    4                1     5     transform_power_2_int
-epochs     int    3                3     4     transform_power_2_int
-k_folds    int    2                0     0     None
-patience   int    5                3     3     None
-optimizer  factor SGD              0     9     None
-criterion  factor CrossEntropyLoss 0     0     None
+Table 3: Experimental design for the hyperparameter tuning.
+ The table shows the hyperparameters, their types, default
+  values, lower and upper bounds, and the transformation
+function. The transformation function is used to transform
+ the hyperparameter values from the unit hypercube to the
+original domain. The transformation function is applied to
+  the hyperparameter values before the evaluation of the
+                    objective function.
+name       type   default lower upper transform
+l1         int    5       2     9     transform_power_2_int
+l2         int    5       2     9     transform_power_2_int
+lr         float  0.001   0.001 0.001 None
+batch_size int    4       1     5     transform_power_2_int
+epochs     int    3       3     4     transform_power_2_int
+k_folds    int    2       0     0     None
+patience   int    5       3     3     None
+optimizer  factor SGD     0     9     None
 The objective function fun_torch is selected next. It implements an interface
 from PyTorchâs training, validation, and testing methods to spotPython.
 fun = HyperTorch().fun_torch
 The spotPython hyperparameter tuning is started by calling the Spot function.
 Here, we will run the tuner for approximately 30 minutes (max_time). Note: the
 initial design is always evaluated in the spotPython run. As a consequence, the
 run may take longer than specified by max_time, because the evaluation time of
@@ -734,54 +1032,77 @@
                                       "model_optimizer":
 differential_evolution,
                                       "model_fun_evals": 10_000,
                                       "log_level": 50
                                       })
 spot_tuner.run(X_start=X_start)
 During the run, the following output is shown:
-config: {'l1': 8, 'l2': 16, 'lr': 0.001, 'batch_size': 2,
-'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'NAdam',
-'criterion': CrossEntropyLoss()}
+config: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16,
+'k_folds': 0, 'patience': 3, 'optimizer': 'Adadelta', 'sgd_momentum': 0.9}
 Epoch: 1
-Loss on hold-out set: 1.798599960240349
-Accuracy on hold-out set: 0.38035
+Loss on hold-out set: 1.602842689704895
+Accuracy on hold-out set: 0.4006
+Metric value on hold-out data: 0.40059998631477356
 Epoch: 2
-Loss on hold-out set: 1.681505929086823
-Accuracy on hold-out set: 0.4163
+Loss on hold-out set: 1.4648857820034027
+Accuracy on hold-out set: 0.47685
+Metric value on hold-out data: 0.4768500030040741
 Epoch: 3
-Loss on hold-out set: 1.6875325478885324
-Accuracy on hold-out set: 0.42245
+Loss on hold-out set: 1.403354868555069
+Accuracy on hold-out set: 0.482
+Metric value on hold-out data: 0.4819999933242798
 Epoch: 4
-Loss on hold-out set: 1.6695034023197601
-Accuracy on hold-out set: 0.45265
+Loss on hold-out set: 1.384560032081604
+Accuracy on hold-out set: 0.49065
+Metric value on hold-out data: 0.4906499981880188
 Epoch: 5
-Loss on hold-out set: 1.6984369342865335
-Accuracy on hold-out set: 0.45085
+Loss on hold-out set: 1.4326466094970702
+Accuracy on hold-out set: 0.4809
+Metric value on hold-out data: 0.48089998960494995
 Epoch: 6
-Loss on hold-out set: 1.6061365829033545
-Accuracy on hold-out set: 0.4527
+Loss on hold-out set: 1.3759961807250976
+Accuracy on hold-out set: 0.4995
+Metric value on hold-out data: 0.49950000643730164
 Epoch: 7
-Loss on hold-out set: 1.7061124059396433
-Accuracy on hold-out set: 0.4566
+Loss on hold-out set: 1.3684927892208099
+Accuracy on hold-out set: 0.50695
+Metric value on hold-out data: 0.5069500207901001
 Epoch: 8
-Loss on hold-out set: 1.7162298802530742
-Accuracy on hold-out set: 0.4504
+Loss on hold-out set: 1.3642385012149811
+Accuracy on hold-out set: 0.506
+Metric value on hold-out data: 0.5059999823570251
 Epoch: 9
-Loss on hold-out set: 1.6683832777252945
-Accuracy on hold-out set: 0.47205
-Early stopping at epoch 8
-Returned to Spot: Validation loss: 1.6683832777252945
+Loss on hold-out set: 1.3157437609672546
+Accuracy on hold-out set: 0.5304
+Metric value on hold-out data: 0.5303999781608582
+Epoch: 10
+Loss on hold-out set: 1.3481314319610596
+Accuracy on hold-out set: 0.5268
+Metric value on hold-out data: 0.5267999768257141
+Epoch: 11
+Loss on hold-out set: 1.3608774542331696
+Accuracy on hold-out set: 0.51525
+Metric value on hold-out data: 0.515250027179718
+Epoch: 12
+Loss on hold-out set: 1.359324642753601
+Accuracy on hold-out set: 0.52355
+Metric value on hold-out data: 0.5235499739646912
+Early stopping at epoch 11
+Returned to Spot: Validation loss: 1.359324642753601
+----------------------------------------------
 
 ***** Results *****
 After the hyperparameter tuning run is finished, the progress of the
 hyperparameter tuning can be visualized. The following code generates the
 progress plot from Figure 2.
 spot_tuner.plot_progress(log_y=False, filename="./figures" +
-experiment_name+"_progress.pdf")
+experiment_name+"_progress.png")
 Figure 1: ?(caption)
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_progress.png]
 Figure 2: Progress plot. Black dots denote results from the initial design. Red
 dots illustrate the improvement found by the surrogate model based optimization
 (surrogate model based optimization).
 Figure 2 shows a typical behaviour that can be observed in many hyperparameter
 studies (Bartz_et_al._2022): the largest improvement is obtained during the
 evaluation of the initial design. The surrogate model based optimization-
 optimization with the surrogate refines the results. Figure 2 also illustrates
@@ -790,37 +1111,39 @@
 similar to the black dots, whereas spotPython uses a surrogate model based
 optimization and presents results represented by red dots in Figure 2. The
 surrogate model based optimization is considered to be more efficient than a
 random search, because the surrogate model guides the search towards promising
 regions in the hyperparameter space.
 In addition to the improved (âoptimizedâ) hyperparameter values, spotPython
 allows a statistical analysis, e.g., a sensitivity analysis, of the results. We
-can print the results of the hyperparameter tuning, see Table 3.
+can print the results of the hyperparameter tuning, see Table 4.
 print(gen_design_table(fun_control=fun_control, spot=spot_tuner))
-    Table 3: Results of the hyperparameter tuning. The table shows the
-hyperparameters, their types, default values, lower and upper bounds, and
-   the transformation function. The column âtunedâ shows the tuned
-     values. The column âimportanceâ shows the importance of the
-   hyperparameters. The column âstarsâ shows the importance of the
-hyperparameters in stars. The importance is computed by the SPOT software.
-name      type   default      lower upper tuned transform importance stars
-l1        int    5            2.0   9.0   7.0   pow_2_int 100.00     ***
-l2        int    5            2.0   9.0   3.0   pow_2_int 96.29      ***
-lr        float  0.001        0.001 0.001 0.001 None      0.00
-batchsize int    4            1.0   5.0   4.0   pow_2_int 0.00
-epochs    int    3            3.0   4.0   4.0   pow_2_int 4.18       *
-k_folds   int    2            0.0   0.0   0.0   None      0.00
-patience  int    5            3.0   3.0   3.0   None      0.00
-optimizer factor SGD          0.0   9.0   3.0   None      0.16       .
-criterion factor CrossEntLoss 0.0   0.0   0.0   None      0.00
+ Table 4: Results of the hyperparameter tuning. The table shows the
+hyperparameters, their types, default values, lower and upper bounds,
+  and the transformation function. The column âtunedâ shows the
+tuned values. The column âimportanceâ shows the importance of the
+ hyperparameters. The column âstarsâ shows the importance of the
+  hyperparameters in stars. The importance is computed by the SPOT
+                              software.
+name      type   default lower upper tuned transform importance stars
+l1        int    5       2.0   9.0   7.0   pow_2_int 100.00     ***
+l2        int    5       2.0   9.0   3.0   pow_2_int 96.29      ***
+lr_mult   float  1.0     0.1   10.0  0.1   None      0.00
+batchsize int    4       1.0   5.0   4.0   pow_2_int 0.00
+epochs    int    3       3.0   4.0   4.0   pow_2_int 4.18       *
+k_folds   int    2       0.0   0.0   0.0   None      0.00
+patience  int    5       3.0   3.0   3.0   None      0.00
+optimizer factor SGD     0.0   9.0   3.0   None      0.16       .
 To visualize the most important hyperparameters, spotPython provides the
 function plot_importance. The following code generates the importance plot from
 Figure 3.
 spot_tuner.plot_importance(threshold=0.025, filename="./figures" +
-experiment_name+"_importance.pdf")
+experiment_name+"_importance.png")
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_importance.png]
 Figure 3: Variable importance
 
 ***** Get SPOT Results *****
 The architecture of the spotPython model can be obtained by the following code:
 X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))
 model_spot = get_one_core_model_from_X(X, fun_control)
 model_spot
@@ -855,41 +1178,55 @@
   (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
   (fc1): Linear(in_features=400, out_features=32, bias=True)
   (fc2): Linear(in_features=32, out_features=32, bias=True)
   (fc3): Linear(in_features=32, out_features=10, bias=True)
 )
 
 ***** Evaluation of the Tuned Architecture *****
-The method train_save takes a model architecture without trained weights and
+The method train_tuned takes a model architecture without trained weights and
 trains this model with the train data. The train data is split into train and
 validation data. The validation data is used for early stopping. The trained
 model weights are saved as a dictionary.
 This evaluation is similar to the final evaluation in PyTorch (2023a).
-train_save(net=model_default, train_dataset=train, shuffle=True,
-        device = "cpu", show_batch_interval=1_000,
-        path="model_default_trained.pt", save_model=True)
-test_saved(net=model_default, test_dataset=test, shuffle=False,
-        device = "cpu", path="model_default_trained.pt")
-The following code trains the model model_spot and saves the weights of the
-trained model to the file model_spot_trained.pt.
-train_save(net=model_spot, train_dataset=train,
-                shuffle=True, path="model_spot_trained.pt", save_model=True)
+train_tuned(net=model_default, train_dataset=train, shuffle=True,
+        loss_function=fun_control["loss_function"],
+        metric=fun_control["metric_torch"],
+        device = DEVICE, show_batch_interval=1_000,)
+test_tuned(net=model_default, test_dataset=test,
+        loss_function=fun_control["loss_function"],
+        metric=fun_control["metric_torch"],
+        shuffle=False,
+        device = DEVICE)
+The following code trains the model model_spot. If path is set to a filename,
+e.g., path = "model_spot_trained.pt", the weights of the trained model will be
+saved to this file.
+train_tuned(net=model_spot, train_dataset=train,
+        loss_function=fun_control["loss_function"],
+        metric=fun_control["metric_torch"],
+        shuffle=True,
+        device = DEVICE,
+        path=None)
 Loss on hold-out set: 1.2267619131326675
 Accuracy on hold-out set: 0.58955
 Early stopping at epoch 13
-test_saved(net=model_spot, test_dataset=test,
-            shuffle=False, path="model_spot_trained.pt")
+If path is set to a filename, e.g., path = "model_spot_trained.pt", the weights
+of the trained model will be loaded from this file.
+test_tuned(net=model_spot, test_dataset=test,
+            shuffle=False,
+            loss_function=fun_control["loss_function"],
+            metric=fun_control["metric_torch"],
+            device = DEVICE)
 Loss on hold-out set: 1.242568492603302
 Accuracy on hold-out set: 0.5957
 
 ***** Comparison with Default Hyperparameters and Ray Tune *****
-Table 4 shows the loss and accuracy of the default model, the model with the
+Table 5 shows the loss and accuracy of the default model, the model with the
 hyperparameters from SPOT, and the model with the hyperparameters from ray
 [tune].
- Table 4: Comparison of the loss and accuracy of the default
+ Table 5: Comparison of the loss and accuracy of the default
  model, the model with the hyperparameters from SPOT, and the
 model with the hyperparameters from ray[tune]. ray[tune] only
    shows the validation loss, because training loss is not
                     reported by ray[tune].
 Model      Validation Loss Validation Accuracy Loss   Accuracy
 Default    2.1221          0.2452              2.1182 0.2425
 spotPython 1.2268          0.5896              1.2426 0.5957
@@ -909,28 +1246,40 @@
 min_z = min(spot_tuner.y)
 max_z = max(spot_tuner.y)
 n = spot_tuner.k
 for i in var_plots:
     for j in var_plots:
         if j > i:
             filename = "./figures" + experiment_name+"_contour_"+str(i)+"_"+str
-(j)+".pdf"
+(j)+".png"
             spot_tuner.plot_contour(i=i, j=j, min_z=min_z, max_z = max_z,
 filename=filename)
 Figure 4: ?(caption)
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_contour_0_1.png]
 Figure 5: Contour plot of the loss as a function of l1 and l2, i.e., the number
 of neurons in the layers.
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_contour_0_3.png]
 Figure 6: Contour plot of the loss as a function of the number of epochs and
 the neurons in layer l1.
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_contour_0_4.png]
 Figure 7: Contour plot of the loss as a function of the optimizer and the
 neurons in layer l1.
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_contour_1_3.png]
 Figure 8: Contour plot of the loss as a function of the number of epochs and
 the neurons in layer l2.
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_contour_1_4.png]
 Figure 9: Contour plot of the loss as a function of the optimizer and the
 neurons in layer l2.
+[./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
+33_contour_3_4.png]
 Figure 10: Contour plot of the loss as a function of the optimizer and the
 number of epochs.
 Figure 5 to Figure 10 show the contour plots of the loss as a function of the
 hyperparameters. These plots are very helpful for benchmark studies and for
 understanding neural networks. spotPython provides additional tools for a
 visual inspection of the results and give valuable insights into the
 hyperparameter tuning process. This is especially useful for model
@@ -1042,9 +1391,8 @@
 beginner/blitz/cifar10_tutorial.html.
 ***** Footnotes *****
    1. https://github.com/sequential-parameter-optimizationâ©ï¸
    2. Alternatively, the source code can be downloaded from gitHub: https://
       github.com/sequential-parameter-optimization/spotPython.â©ï¸
    3. We were not able to install Ray Tune on our system. Therefore, we used
       the results from the PyTorch tutorial.â©ï¸
-   4. The key "metric" is used for the river based evaluation (Montiel_et_al.
-      2021) via eval_oml_iter_progressive.â©ï¸
+   4. https://torchmetrics.readthedocs.io/en/latest/.â©ï¸
```

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/figures/parallel.png` & `spotPython-0.2.0/docs/figures/parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/search.json` & `spotPython-0.2.0/docs/search.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.938888888888889%*

 * *Differences: {'1': "{'text': 'Setup\\nBefore we consider the detailed experimental setup, we select the "*

 * *      'parameters that affect run time, initial design size and the device that is '*

 * *      'used.\\n\\nMAX_TIME = 60\\nINIT_SIZE = 20\\nDEVICE = "cpu" # "cuda:0"\'}',*

 * * '10': "{'text': 'Results\\nAfter the hyperparameter tuning run is finished, the progress of the "*

 * *       'hyperparameter tuning can be visualized. The following code generates the progress plot '*

 * *       'from Figure\\xa02.\\n\\n\\nspot_tuner.plot_prog […]*

```diff
@@ -6,15 +6,15 @@
         "text": "Hyperparameter tuning is an important, but often difficult and computationally intensive task. Changing the architecture of a neural network or the learning rate of an optimizer can have a significant impact on the performance.\nThe goal of hyperparameter tuning is to optimize the hyperparameters in a way that improves the performance of the machine learning or deep learning model. The simplest, but also most computationally expensive, approach uses manual search (or trial-and-error (Meignan et al. 2015)). Commonly encountered is simple random search, i.e., random and repeated selection of hyperparameters for evaluation, and lattice search (\u201cgrid search\u201d). In addition, methods that perform directed search and other model-free algorithms, i.e., algorithms that do not explicitly rely on a model, e.g., evolution strategies (Bartz-Beielstein et al. 2014) or pattern search (Lewis, Torczon, and Trosset 2000) play an important role. Also, \u201chyperband\u201d, i.e., a multi-armed bandit strategy that dynamically allocates resources to a set of random configurations and uses successive bisections to stop configurations with poor performance (Li et al. 2016), is very common in hyperparameter tuning. The most sophisticated and efficient approaches are the Bayesian optimization and surrogate model based optimization methods, which are based on the optimization of cost functions determined by simulations or experiments.\nWe consider below a surrogate model based optimization-based hyperparameter tuning approach based on the Python version of the SPOT (\u201cSequential Parameter Optimization Toolbox\u201d) (Bartz-Beielstein, Lasarczyk, and Preuss 2005), which is suitable for situations where only limited resources are available. This may be due to limited availability and cost of hardware, or due to the fact that confidential data may only be processed locally, e.g., due to legal requirements. Furthermore, in our approach, the understanding of algorithms is seen as a key tool for enabling transparency and explainability. This can be enabled, for example, by quantifying the contribution of machine learning and deep learning components (nodes, layers, split decisions, activation functions, etc.). Understanding the importance of hyperparameters and the interactions between multiple hyperparameters plays a major role in the interpretability and explainability of machine learning models. SPOT provides statistical tools for understanding hyperparameters and their interactions. Last but not least, it should be noted that the SPOT software code is available in the open source spotPython package on github1, allowing replicability of the results. This tutorial descries the Python variant of SPOT, which is called spotPython. The R implementation is described in Bartz et al. (2022). SPOT is an established open source software that has been maintained for more than 15 years (Bartz-Beielstein, Lasarczyk, and Preuss 2005) (Bartz et al. 2022).\nThis tutorial is structured as follows. The concept of the hyperparameter tuning software spotPython is described in Section\u00a02. Section\u00a03 describes the integration of spotPython into the PyTorch training workflow and presents the results. Finally, Section\u00a04 presents a summary and an outlook.\n\n\n\n\n\n\nNote\n\n\n\nThe corresponding .ipynb notebook (Bartz-Beielstein 2023) is updated regularly and reflects updates and changes in the spotPython package. It can be downloaded from https://github.com/sequential-parameter-optimization/spotPython/blob/main/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb.",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-setup",
         "objectID": "bart23e.html#sec-setup",
         "section": "Setup",
-        "text": "Setup\nBefore we consider the detailed experimental setup, we select the parameters that affect run time, initial design size and the device that is used.\n\nMAX_TIME = 60\nINIT_SIZE = 10\nDEVICE = \"cpu\" # \"cuda:0\"",
+        "text": "Setup\nBefore we consider the detailed experimental setup, we select the parameters that affect run time, initial design size and the device that is used.\n\nMAX_TIME = 60\nINIT_SIZE = 20\nDEVICE = \"cpu\" # \"cuda:0\"",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#initialization-of-the-fun_control-dictionary",
         "objectID": "bart23e.html#initialization-of-the-fun_control-dictionary",
         "section": "Initialization of the fun_control Dictionary",
         "text": "Initialization of the fun_control Dictionary\nspotPython uses a Python dictionary for storing the information required for the hyperparameter tuning process. This dictionary is called fun_control and is initialized with the function fun_control_init. The function fun_control_init returns a skeleton dictionary. The dictionary is filled with the required information for the hyperparameter tuning process. It stores the hyperparameter tuning settings, e.g., the deep learning network architecture that should be tuned, the classification (or regression) problem, and the data that is used for the tuning. The dictionary is used as an input for the SPOT function.\n\nfun_control = fun_control_init()",
@@ -34,50 +34,50 @@
         "text": "Specification of the Preprocessing Model\nAfter the training and test data are specified and added to the fun_control dictionary, spotPython allows the specification of a data preprocessing pipeline, e.g., for the scaling of the data or for the one-hot encoding of categorical variables. The preprocessing model is called prep_model (\u201cpreparation\u201d or pre-processing) and includes steps that are not subject to the hyperparameter tuning process. The preprocessing model is specified in the fun_control dictionary. The preprocessing model can be implemented as a sklearn pipeline. The following code shows a typical preprocessing pipeline:\ncategorical_columns = [\"cities\", \"colors\"]\none_hot_encoder = OneHotEncoder(handle_unknown=\"ignore\",\n                                    sparse_output=False)\nprep_model = ColumnTransformer(\n        transformers=[\n             (\"categorical\", one_hot_encoder, categorical_columns),\n         ],\n         remainder=StandardScaler(),\n     )\nBecause the Ray Tune (ray[tune]) hyperparameter tuning as described in PyTorch (2023a) does not use a preprocessing model, the preprocessing model is set to None here.\n\nprep_model = None\nfun_control.update({\"prep_model\": prep_model})",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-selection-of-the-algorithm",
         "objectID": "bart23e.html#sec-selection-of-the-algorithm",
         "section": "Select algorithm and core_model_hyper_dict",
-        "text": "Select algorithm and core_model_hyper_dict\nThe same neural network model as implemented in the section \u201cConfigurable neural network\u201d of the PyTorch tutorial (PyTorch 2023a) is used here. We will show the implementation from PyTorch (2023a) in Section\u00a03.5.1 first, before the extended implementation with spotPython is shown in Section\u00a03.5.2.\n\nImplementing a Configurable Neural Network With Ray Tune\nWe used the same hyperparameters that are implemented as configurable in the PyTorch tutorial. We specify the layer sizes, namely l1 and l2, of the fully connected layers:\nclass Net(nn.Module):\n    def __init__(self, l1=120, l2=84):\n        super(Net, self).__init__()\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\n\nThe learning rate, i.e., lr, of the optimizer is made configurable, too:\noptimizer = optim.SGD(net.parameters(), lr=config[\"lr\"], momentum=0.9)\n\n\nImplementing a Configurable Neural Network With spotPython\nspotPython implements a class which is similar to the class described in the PyTorch tutorial. The class is called Net_CIFAR10 and is implemented in the file netcifar10.py.\nimport spotPython.torch.netcore as netcore\nclass Net_CIFAR10(netcore.Net_Core):\n    def __init__(self, l1, l2, lr, batch_size, epochs, k_folds, patience):\n        super(Net_CIFAR10, self).__init__(\n            lr=lr, batch_size=batch_size, epochs=epochs, k_folds=k_folds,\n            patience=patience\n        )\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\nNet_CIFAR10 inherits from the class Net_Core which is implemented in the file netcore.py. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate lr, the batch size batch_size, the number of epochs epochs, the number of folds k_folds for the cross validation, and the patience patience for the early stopping. The class Net_Core is shown below.\nfrom torch import nn\n\n\nclass Net_Core(nn.Module):\n    def __init__(self, lr, batch_size, epochs, k_folds, patience):\n        super(Net_Core, self).__init__()\n        self.lr = lr\n        self.batch_size = batch_size\n        self.epochs = epochs\n        self.k_folds = k_folds\n        self.patience = patience\n\n\nComparison of the Approach Described in the PyTorch Tutorial With spotPython\nComparing the class Net from the PyTorch tutorial and the class Net_CIFAR10 from spotPython, we see that the class Net_CIFAR10 has additional attributes and does not inherit from nn directly. It adds an additional class, Net_core, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate lr or the batch size batch_size.\nspotPython\u2019s core_model implements an instance of the Net_CIFAR10 class. In addition to the basic neural network model, the core_model can use these additional attributes. spotPython provides methods for handling these additional attributes to guarantee 100% compatibility with the PyTorch classes. The method add_core_model_to_fun_control adds the hyperparameters and additional attributes to the fun_control dictionary. The method is shown below.\n\ncore_model = Net_CIFAR10\nfun_control = add_core_model_to_fun_control(core_model=core_model,\n                              fun_control=fun_control,\n                              hyper_dict=TorchHyperDict,\n                              filename=None)\n\n\n\n\n\n\n\nNote\n\n\n\nIn addition to the class Net from the PyTorch tutorial, the class Net_CIFAR10 has additional attributes, e.g.:\n\nlearning rate (lr),\nbatch size (batch_size),\nepochs (epochs),\nk_folds (k_folds), and\nearly stopping criterion \u201cpatience\u201d (patience)\n\nFurther attributes can be easily added to the class, e.g., optimizer or loss_function.",
+        "text": "Select algorithm and core_model_hyper_dict\nThe same neural network model as implemented in the section \u201cConfigurable neural network\u201d of the PyTorch tutorial (PyTorch 2023a) is used here. We will show the implementation from PyTorch (2023a) in Section\u00a03.5.1 first, before the extended implementation with spotPython is shown in Section\u00a03.5.2.\n\nImplementing a Configurable Neural Network With Ray Tune\nWe used the same hyperparameters that are implemented as configurable in the PyTorch tutorial. We specify the layer sizes, namely l1 and l2, of the fully connected layers:\nclass Net(nn.Module):\n    def __init__(self, l1=120, l2=84):\n        super(Net, self).__init__()\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\n\nThe learning rate, i.e., lr, of the optimizer is made configurable, too:\noptimizer = optim.SGD(net.parameters(), lr=config[\"lr\"], momentum=0.9)\n\n\nImplementing a Configurable Neural Network With spotPython\nspotPython implements a class which is similar to the class described in the PyTorch tutorial. The class is called Net_CIFAR10 and is implemented in the file netcifar10.py.\nimport spotPython.torch.netcore as netcore\nclass Net_CIFAR10(netcore.Net_Core):\n    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):\n        super(Net_CIFAR10, self).__init__(\n            lr_mult=lr_mult, batch_size=batch_size, epochs=epochs, k_folds=k_folds,\n            patience=patience\n        )\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\nNet_CIFAR10 inherits from the class Net_Core which is implemented in the file netcore.py. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate multiplier lr_mult, the batch size batch_size, the number of epochs epochs, the number of folds k_folds for the cross validation, and the patience patience for the early stopping. The class Net_Core is shown below.\nfrom torch import nn\n\n\nclass Net_Core(nn.Module):\n    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):\n        super(Net_Core, self).__init__()\n        self.lr_mult = lr_mult\n        self.batch_size = batch_size\n        self.epochs = epochs\n        self.k_folds = k_folds\n        self.patience = patience\n\n\nComparison of the Approach Described in the PyTorch Tutorial With spotPython\nComparing the class Net from the PyTorch tutorial and the class Net_CIFAR10 from spotPython, we see that the class Net_CIFAR10 has additional attributes and does not inherit from nn directly. It adds an additional class, Net_core, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate multiplier lr_mult or the batch size batch_size.\nspotPython\u2019s core_model implements an instance of the Net_CIFAR10 class. In addition to the basic neural network model, the core_model can use these additional attributes. spotPython provides methods for handling these additional attributes to guarantee 100% compatibility with the PyTorch classes. The method add_core_model_to_fun_control adds the hyperparameters and additional attributes to the fun_control dictionary. The method is shown below.\n\ncore_model = Net_CIFAR10\nfun_control = add_core_model_to_fun_control(core_model=core_model,\n                              fun_control=fun_control,\n                              hyper_dict=TorchHyperDict,\n                              filename=None)\n\n\n\n\n\n\n\nNote\n\n\n\nIn addition to the class Net from the PyTorch tutorial, the class Net_CIFAR10 has additional attributes, e.g.:\n\nlearning rate (lr),\nbatch size (batch_size),\nepochs (epochs),\nk_folds (k_folds), and\nearly stopping criterion \u201cpatience\u201d (patience)\n\nFurther attributes can be easily added to the class, e.g., optimizer.",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-search-space",
         "objectID": "bart23e.html#sec-search-space",
         "section": "The Search Space",
-        "text": "The Search Space\nIn Section\u00a03.6.1, we first describe how to configure the search space with ray[tune] (as shown in PyTorch (2023a)) and then how to configure the search space with spotPython in Section\u00a03.6.2.\n\nConfiguring the Search Space With Ray Tune\nRay Tune\u2019s search space can be configured as follows (PyTorch 2023a):\nconfig = {\n    \"l1\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"l2\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"lr\": tune.loguniform(1e-4, 1e-1),\n    \"batch_size\": tune.choice([2, 4, 8, 16])\n}\nThe tune.sample_from() function enables the user to define sample methods to obtain hyperparameters. In this example, the l1 and l2 parameters should be powers of 2 between 4 and 256, so either 4, 8, 16, 32, 64, 128, or 256. The lr (learning rate) should be uniformly sampled between 0.0001 and 0.1. Lastly, the batch size is a choice between 2, 4, 8, and 16.\nAt each trial, ray[tune] will randomly sample a combination of parameters from these search spaces. It will then train a number of models in parallel and find the best performing one among these. ray[tune] uses the ASHAScheduler which will terminate bad performing trials early.\n\n\nConfiguring the Search Space With spotPython\n\nThe hyper_dict Hyperparameters for the Selected Algorithm\nspotPython uses simple JSON files for the specification of the hyperparameters. Users can specify their individual JSON files, or they can use the JSON files provided by spotPython. The JSON file for the core_model is called torch_hyper_dict.json.\nIn contrast to ray[tune], spotPython can handle numerical, boolean, and categorical hyperparameters. They can be specified in the JSON file in a similar way as the numerical hyperparameters as shown below:\n\"factor_hyperparameter\": {\n    \"levels\": [\"A\", \"B\", \"C\"],\n    \"type\": \"factor\",\n    \"default\": \"B\",\n    \"transform\": \"None\",\n    \"core_model_parameter_type\": \"str\",\n    \"lower\": 0,\n    \"upper\": 2},\nEach entry in the JSON file represents one hyperparameter with the following structure: type, default, transform, lower, and upper. The corresponding entries for the Net_CIFAR10 class are shown below.\n{\"Net_CIFAR10\":\n    {\n        \"l1\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"l2\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"lr\": {\n            \"type\": \"float\",\n            \"default\": 1e-03,\n            \"transform\": \"None\",\n            \"lower\": 1e-05,\n            \"upper\": 1e-02},\n        \"batch_size\": {\n            \"type\": \"int\",\n            \"default\": 4,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"epochs\": {\n            \"type\": \"int\",\n            \"default\": 3,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"k_folds\": {\n            \"type\": \"int\",\n            \"default\": 2,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 3},\n        \"patience\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 10},\n        \"optimizer\": {\n            \"levels\": [\"Adadelta\",\n                       \"Adagrad\",\n                       \"Adam\",\n                       \"AdamW\",\n                       \"SparseAdam\",\n                       \"Adamax\",\n                       \"ASGD\",\n                       \"LBFGS\",\n                       \"NAdam\",\n                       \"RAdam\",\n                       \"RMSprop\",\n                       \"Rprop\",\n                       \"SGD\"],\n            \"type\": \"factor\",\n            \"default\": \"SGD\",\n            \"transform\": \"None\",\n            \"class_name\": \"torch.optim\",\n            \"core_model_parameter_type\": \"str\",\n            \"lower\": 0,\n            \"upper\": 12},\n        \"criterion\": {\n            \"levels\": [\"L1Loss\",\n                       \"MSELoss\",\n                       \"CrossEntropyLoss\",\n                       \"CTCLoss\",\n                       \"NLLLoss\",\n                       \"PoissonNLLLoss\",\n                       \"GaussianNLLLoss\",\n                       \"KLDivLoss\",\n                       \"BCELoss\",\n                       \"BCEWithLogitsLoss\",\n                       \"MarginRankingLoss\",\n                       \"HingeEmbeddingLoss\",\n                       \"MultiLabelMarginLoss\",\n                       \"HuberLoss\",\n                       \"SmoothL1Loss\",\n                       \"SoftMarginLoss\",\n                       \"MultiLabelSoftMarginLoss\",\n                       \"CosineEmbeddingLoss\",\n                       \"MultiMarginLoss\",\n                       \"TripletMarginLoss\",\n                       \"TripletMarginWithDistanceLoss\"],\n            \"type\": \"factor\",\n            \"default\": \"CrossEntropyLoss\",\n            \"transform\": \"None\",\n            \"class_name\": \"torch.nn\",\n            \"core_model_parameter_type\": \"instance()\",\n            \"lower\": 0,\n            \"upper\": 20}\n    }\n}",
+        "text": "The Search Space\nIn Section\u00a03.6.1, we first describe how to configure the search space with ray[tune] (as shown in PyTorch (2023a)) and then how to configure the search space with spotPython in Section\u00a03.6.2.\n\nConfiguring the Search Space With Ray Tune\nRay Tune\u2019s search space can be configured as follows (PyTorch 2023a):\nconfig = {\n    \"l1\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"l2\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"lr\": tune.loguniform(1e-4, 1e-1),\n    \"batch_size\": tune.choice([2, 4, 8, 16])\n}\nThe tune.sample_from() function enables the user to define sample methods to obtain hyperparameters. In this example, the l1 and l2 parameters should be powers of 2 between 4 and 256, so either 4, 8, 16, 32, 64, 128, or 256. The lr (learning rate) should be uniformly sampled between 0.0001 and 0.1. Lastly, the batch size is a choice between 2, 4, 8, and 16.\nAt each trial, ray[tune] will randomly sample a combination of parameters from these search spaces. It will then train a number of models in parallel and find the best performing one among these. ray[tune] uses the ASHAScheduler which will terminate bad performing trials early.\n\n\nConfiguring the Search Space With spotPython\n\nThe hyper_dict Hyperparameters for the Selected Algorithm\nspotPython uses simple JSON files for the specification of the hyperparameters. Users can specify their individual JSON files, or they can use the JSON files provided by spotPython. The JSON file for the core_model is called torch_hyper_dict.json.\nIn contrast to ray[tune], spotPython can handle numerical, boolean, and categorical hyperparameters. They can be specified in the JSON file in a similar way as the numerical hyperparameters as shown below:\n\"factor_hyperparameter\": {\n    \"levels\": [\"A\", \"B\", \"C\"],\n    \"type\": \"factor\",\n    \"default\": \"B\",\n    \"transform\": \"None\",\n    \"core_model_parameter_type\": \"str\",\n    \"lower\": 0,\n    \"upper\": 2},\nEach entry in the JSON file represents one hyperparameter with the following structure: type, default, transform, lower, and upper. The corresponding entries for the Net_CIFAR10 class are shown below.\n{\"Net_CIFAR10\":\n    {\n        \"l1\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"l2\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"lr_mult\": {\n            \"type\": \"float\",\n            \"default\": 1.0,\n            \"transform\": \"None\",\n            \"lower\": 0.1,\n            \"upper\": 10},\n        \"batch_size\": {\n            \"type\": \"int\",\n            \"default\": 4,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"epochs\": {\n            \"type\": \"int\",\n            \"default\": 3,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"k_folds\": {\n            \"type\": \"int\",\n            \"default\": 2,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 3},\n        \"patience\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 10},\n        \"optimizer\": {\n            \"levels\": [\"Adadelta\",\n                       \"Adagrad\",\n                       \"Adam\",\n                       \"AdamW\",\n                       \"SparseAdam\",\n                       \"Adamax\",\n                       \"ASGD\",\n                       \"LBFGS\",\n                       \"NAdam\",\n                       \"RAdam\",\n                       \"RMSprop\",\n                       \"Rprop\",\n                       \"SGD\"],\n            \"type\": \"factor\",\n            \"default\": \"SGD\",\n            \"transform\": \"None\",\n            \"class_name\": \"torch.optim\",\n            \"core_model_parameter_type\": \"str\",\n            \"lower\": 0,\n            \"upper\": 12},\n        \"sgd_momentum\": {\n            \"type\": \"float\",\n            \"default\": 0.0,\n            \"transform\": \"None\",\n            \"lower\": 0.0,\n            \"upper\": 1.0}\n    }\n}",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-modification-of-hyperparameters",
         "objectID": "bart23e.html#sec-modification-of-hyperparameters",
         "section": "Modifying the Hyperparameters",
-        "text": "Modifying the Hyperparameters\nRay tune (PyTorch 2023a) does not provide a way to change the specified hyperparameters without re-compilation. However, spotPython provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters without re-compilation of the Python source code. These functions are described in the following.\n\nModify hyper_dict Hyperparameters for the Selected Algorithm aka core_model\nAfter specifying the model, the corresponding hyperparameters, their types and bounds are loaded from the JSON file torch_hyper_dict.json. After loading, the user can modify the hyperparameters, e.g., the bounds. spotPython provides a simple rule for de-activating hyperparameters: If the lower and the upper bound are set to identical values, the hyperparameter is de-activated. This is useful for the hyperparameter tuning, because it allows to specify a hyperparameter in the JSON file, but to de-activate it in the fun_control dictionary. This is done in the next step.\n\n\nModify Hyperparameters of Type numeric and integer (boolean)\nSince the hyperparameter k_folds is not used in the PyTorch tutorial, it is de-activated here by setting the lower and upper bound to the same value. Note, k_folds is of type \u201cinteger\u201d.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"batch_size\", bounds=[1, 5])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"k_folds\", bounds=[0, 0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"patience\", bounds=[3, 3])\nfun_control[\"core_model_hyper_dict\"]\n\n\n\nModify Hyperparameter of Type factor\nIn a similar manner as for the numerical hyperparameters, the categorical hyperparameters can be modified. New configurations can be chosen by adding or deleting levels. For example, the hyperparameter optimizer can be re-configured as follows:\nIn the following setting, two optimizers (\"SGD\" and \"Adam\") will be compared during the spotPython hyperparameter tuning. The hyperparameter optimizer is active.\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\", \"Adam\"])\n\nThe hyperparameter optimizer can be de-activated by choosing only one value (level), here: \"SGD\".\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\"])\n\nAs discussed in Section\u00a03.7.4, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in spotPython by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. Rprop was remmoved, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since SparseAdam does not support dense gradients, Adam was used instead. Therefore, there are 10 default optimizers:\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\",[\"Adadelta\",\n     \"Adagrad\", \"Adam\", \"AdamW\", \"Adamax\", \"ASGD\", \"NAdam\", \"RAdam\",\n      \"RMSprop\", \"SGD\"])\n\n\n\nOptimizers\nTable\u00a01 shows some of the optimizers available in PyTorch:\n\n\nTable\u00a01: Optimizers available in PyTorch (selection). \u201cmom\u201d denotes momentum, \u201cweight\u201d weight_decay, \u201cdamp\u201d dampening, \u201cnest\u201d nesterov, and \u201clr_sc\u201d learning rate for scaling delta. The default values are shown in the table.\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nOptimizer\nlr\nmom\nweight\ndamp\nnest\nrho\nlr_sc\nlr_decay\nbetas\n\n\n\n\nSGD\nrequired\nfloat: 0\nfloat: 0\nfloat: 0\nbool: False\n-\n-\n-\n-\n\n\nAdadelta\n-\n-\nfloat: 0\n-\n-\nfloat: 0.9\nfloat: 1.0\n-\n-\n\n\nAdagrad\nfloat: 1e-2\n-\nfloat: 0\n-\n-\n-\n-\nfloat: 0\n-\n\n\nAdam\nfloat: 1e-3\n-\nfloat: 0\n-\n-\n-\n-\n-\nTuple[float, float]: (0.9, 0.999)\n\n\nAdamW\nfloat: 1e-3\n-\nfloat: 1e-2\n-\n-\n-\n-\n-\nTuple[float, float]: (0.9, 0.999)\n\n\nSparseAdam\nfloat: 1e-3\n-\n-\n-\n-\n-\n-\n-\nTuple[float, float]: (0.9, 0.999)\n\n\n\n\nspotPython implements an optimization handler that maps the optimizer names to the corresponding PyTorch optimizers.\n\n\n\n\n\n\nA note on LBFGS\n\n\n\nPyTorch\u2019s LBFGS optimizer is deactivated in spotPython by default, because it does not perform very well. The PyTorch documentation, see https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS, states:\n\nThis is a very memory intensive optimizer (it requires additional param_bytes * (history_size + 1) bytes). If it doesn\u2019t fit in memory try reducing the history size, or use a different algorithm.\n\nFurthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial. The reason is that the LBFGS optimizer requires the closure function, which is not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is recommended here.\n\n\nSince there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only. Thus, the learning rate, which affects the SGD optimizer, will be set to a fixed value. We choose the default value of 1e-3 for the learning rate, because it is used in other PyTorch examples. We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"lr\", bounds=[1e-3, 1e-3])",
+        "text": "Modifying the Hyperparameters\nRay tune (PyTorch 2023a) does not provide a way to change the specified hyperparameters without re-compilation. However, spotPython provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters without re-compilation of the Python source code. These functions are described in the following.\n\nModify hyper_dict Hyperparameters for the Selected Algorithm aka core_model\nAfter specifying the model, the corresponding hyperparameters, their types and bounds are loaded from the JSON file torch_hyper_dict.json. After loading, the user can modify the hyperparameters, e.g., the bounds. spotPython provides a simple rule for de-activating hyperparameters: If the lower and the upper bound are set to identical values, the hyperparameter is de-activated. This is useful for the hyperparameter tuning, because it allows to specify a hyperparameter in the JSON file, but to de-activate it in the fun_control dictionary. This is done in the next step.\n\n\nModify Hyperparameters of Type numeric and integer (boolean)\nSince the hyperparameter k_folds is not used in the PyTorch tutorial, it is de-activated here by setting the lower and upper bound to the same value. Note, k_folds is of type \u201cinteger\u201d.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"batch_size\", bounds=[1, 5])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"k_folds\", bounds=[0, 0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"patience\", bounds=[3, 3])\nfun_control[\"core_model_hyper_dict\"]\n\n\n\nModify Hyperparameter of Type factor\nIn a similar manner as for the numerical hyperparameters, the categorical hyperparameters can be modified. New configurations can be chosen by adding or deleting levels. For example, the hyperparameter optimizer can be re-configured as follows:\nIn the following setting, two optimizers (\"SGD\" and \"Adam\") will be compared during the spotPython hyperparameter tuning. The hyperparameter optimizer is active.\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\", \"Adam\"])\n\nThe hyperparameter optimizer can be de-activated by choosing only one value (level), here: \"SGD\".\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\"])\n\nAs discussed in Section\u00a03.7.4, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in spotPython by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. Rprop was removed, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since SparseAdam does not support dense gradients, Adam was used instead. Therefore, there are 10 default optimizers:\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\",[\"Adadelta\",\n     \"Adagrad\", \"Adam\", \"AdamW\", \"Adamax\", \"ASGD\", \"NAdam\", \"RAdam\",\n      \"RMSprop\", \"SGD\"])\n\n\n\nOptimizers\nTable\u00a01 shows some of the optimizers available in PyTorch:\n\n\nTable\u00a01: Optimizers available in PyTorch (selection). \u201cmom\u201d denotes momentum, \u201cweight\u201d weight_decay, \u201cdamp\u201d dampening, \u201cnest\u201d nesterov, \u201clr_sc\u201d learning rate for scaling delta, \u201cmom_dec\u201d for momentum_decay, and \u201cstep_s\u201d for step_sizes. The default values are shown in the table.\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nOptimizer\nlr\nmom\nweight\ndamp\nnest\nrho\nlr_sc\nlr_decay\nbetas\nlambd\nalpha\nmom_decay\netas\nstep_s\n\n\n\n\nAdadelta\n-\n-\n0.\n-\n-\n0.9\n1.0\n-\n-\n-\n-\n-\n-\n-\n\n\nAdagrad\n1e-2\n-\n0.\n-\n-\n-\n-\n0.\n-\n-\n-\n-\n-\n-\n\n\nAdam\n1e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nAdamW\n1e-3\n-\n1e-2\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nSparseAdam\n1e-3\n-\n-\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nAdamax\n2e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9, 0.999)\n-\n-\n-\n-\n-\n\n\nASGD\n1e-2\n0.9\n0.\n-\nFalse\n-\n-\n-\n-\n1e-4\n0.75\n-\n-\n-\n\n\nLBFGS\n1.\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n\n\nNAdam\n2e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n0\n-\n-\n\n\nRAdam\n1e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nRMSprop\n1e-2\n0.\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nRprop\n1e-2\n-\n-\n-\n-\n-\n-\n-\n-\n-\n(0.5,1.2)\n(1e-6, 50)\n-\n-\n\n\nSGD\nrequired\n0.\n0.\n0.\nFalse\n-\n-\n-\n-\n-\n-\n-\n-\n-\n\n\n\n\nspotPython implements an optimization handler that maps the optimizer names to the corresponding PyTorch optimizers.\n\n\n\n\n\n\nA note on LBFGS\n\n\n\nWe recommend deactivating PyTorch\u2019s LBFGS optimizer, because it does not perform very well. The PyTorch documentation, see https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS, states:\n\nThis is a very memory intensive optimizer (it requires additional param_bytes * (history_size + 1) bytes). If it doesn\u2019t fit in memory try reducing the history size, or use a different algorithm.\n\nFurthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial. The reason is that the LBFGS optimizer requires the closure function, which is not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is recommended here.\n\n\nSince there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only.\n\n\n\n\n\n\nA note on the learning rate\n\n\n\nspotPython provides a multiplier for the default learning rates, because optimizers use different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore, we recommend fixing the learning rate for all optimizers if multiple optimizers are used. This can be done by setting the lower and upper bounds of the learning rate multiplier to the same value as shown below.\n\n\nThus, the learning rate, which affects the SGD optimizer, will be set to a fixed value. We choose the default value of 1e-3 for the learning rate, because it is used in other PyTorch examples (it is also the default value used by spotPython as defined in the optimizer_handler() method). We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.\nFor the same reason, we will fix the sgd_momentum to 0.9.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"lr_mult\", bounds=[1.0, 1.0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"sgd_momentum\", bounds=[0.9, 0.9])",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-selection-of-target-function",
         "objectID": "bart23e.html#sec-selection-of-target-function",
         "section": "Evaluation",
-        "text": "Evaluation\nThe evaluation procedure requires the specification of two elements:\n\nthe way how the data is split into a train and a test set and\nthe loss function (and a metric).\n\n\nHold-out Data Split and Cross-Validation\nAs a default, spotPython provides a standard hold-out data split and cross validation.\n\nHold-out Data Split\nIf a hold-out data split is used, the data will be partitioned into a training, a validation, and a test data set. The split depends on the setting of the eval parameter. If eval is set to train_hold_out, one data set, usually the original training data set, is split into a new training and a validation data set. The training data set is used for training the model. The validation data set is used for the evaluation of the hyperparameter configuration and early stopping to prevent overfitting. In this case, the original test data set is not used. The following splits are performed in the hold-out setting: \\(\\{\\text{train}_0, \\text{test}\\} \\rightarrow \\{\\text{train}_1, \\text{validation}_1, \\text{test}\\}\\), where \\(\\text{train}_1 \\cup \\text{validation}_1 = \\text{train}_0\\).\n\n\n\n\n\n\nNote\n\n\n\nspotPython returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.\nSummarizing, the following splits are performed in the hold-out setting:\n\nRun spotPython with eval set to train_hold_out to determine the best hyperparameter configuration.\nTrain the model with the best hyperparameter configuration on the training data set:\n\ntrain_save(model_spot, train, \"model_spot.pt\").\n\nTest the model on the test data:\n\ntest_saved(model_spot, test, \"model_spot.pt\")\n\n\nThese steps will be exemplified in the following sections.\n\n\nIn addition to this hold-out setting, spotPython provides another hold-out setting, where an explicit test data is specified by the user that will be used as the validation set. To choose this option, the eval parameter is set to test_hold_out. In this case, the training data set is used for the model training. Then, the explicitly defined test data set is used for the evaluation of the hyperparameter configuration (the validation).\n\n\nCross-Validation\nThe cross validation setting is used by setting the eval parameter to train_cv or test_cv. In both cases, the data set is split into \\(k\\) folds. The model is trained on \\(k-1\\) folds and evaluated on the remaining fold. This is repeated \\(k\\) times, so that each fold is used exactly once for evaluation. The final evaluation is performed on the test data set. The cross validation setting is useful for small data sets, because it allows to use all data for training and evaluation. However, it is computationally expensive, because the model has to be trained \\(k\\) times.\n\n\n\n\n\n\nNote\n\n\n\nCombinations of the above settings are possible, e.g., cross validation can be used for training and hold-out for evaluation or . Also, cross validation can be used for training and testing. Because cross validation is not used in the PyTorch tutorial (PyTorch 2023a), it is not considered further here.\n\n\n\n\n\nLoss Functions and Metrics\nThe key \"criterion\" specifies the loss function which is used during the optimization. There are several different loss functions under PyTorch\u2019s nn package. For example, a simple loss is MSELoss, which computes the mean-squared error between the output and the target. In this tutorial we will use CrossEntropyLoss, because it is also used in the PyTorch tutorial.\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"criterion\", [\"CrossEntropyLoss\"])\n\nIn addition to the loss functions, spotPython provides access to a large number of metrics. The key \"metric_sklearn\" is used for metrics that follow the scikit-learn conventions4. Because the PyTorch tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial\u2019s example code. Therefore, we will use the same implementation here and set the key \"metric_sklearn\" to None.\n\nweights = 1.0\ncriterion = CrossEntropyLoss\nshuffle = True\neval = \"train_hold_out\"\ndevice = DEVICE\nshow_batch_interval = 100_000\nsave_model = True\npath=\"torch_model.pt\"\n\nfun_control.update({\n               \"data_dir\": None,\n               \"checkpoint_dir\": None,\n               \"horizon\": None,\n               \"oml_grace_period\": None,\n               \"weights\": weights,\n               \"step\": None,\n               \"log_level\": 50,\n               \"weight_coeff\": None,\n               \"metric\": None,\n               \"metric_sklearn\": None,\n               \"criterion\": criterion,\n               \"shuffle\": shuffle,\n               \"eval\": eval,\n               \"device\": device,\n               \"show_batch_interval\": show_batch_interval,\n               \"save_model\": save_model,\n               \"path\": path,\n               })",
+        "text": "Evaluation\nThe evaluation procedure requires the specification of two elements:\n\nthe way how the data is split into a train and a test set and\nthe loss function (and a metric).\n\n\nHold-out Data Split and Cross-Validation\nAs a default, spotPython provides a standard hold-out data split and cross validation.\n\nHold-out Data Split\nIf a hold-out data split is used, the data will be partitioned into a training, a validation, and a test data set. The split depends on the setting of the eval parameter. If eval is set to train_hold_out, one data set, usually the original training data set, is split into a new training and a validation data set. The training data set is used for training the model. The validation data set is used for the evaluation of the hyperparameter configuration and early stopping to prevent overfitting. In this case, the original test data set is not used. The following splits are performed in the hold-out setting: \\(\\{\\text{train}_0, \\text{test}\\} \\rightarrow \\{\\text{train}_1, \\text{validation}_1, \\text{test}\\}\\), where \\(\\text{train}_1 \\cup \\text{validation}_1 = \\text{train}_0\\).\n\n\n\n\n\n\nNote\n\n\n\nspotPython returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.\nSummarizing, the following splits are performed in the hold-out setting:\n\nRun spotPython with eval set to train_hold_out to determine the best hyperparameter configuration.\nTrain the model with the best hyperparameter configuration on the training data set:\n\ntrain_tuned(model_spot, train, \"model_spot.pt\").\n\nTest the model on the test data:\n\ntest_tuned(model_spot, test, \"model_spot.pt\")\n\n\nThese steps will be exemplified in the following sections.\n\n\nIn addition to this hold-out setting, spotPython provides another hold-out setting, where an explicit test data is specified by the user that will be used as the validation set. To choose this option, the eval parameter is set to test_hold_out. In this case, the training data set is used for the model training. Then, the explicitly defined test data set is used for the evaluation of the hyperparameter configuration (the validation).\n\n\nCross-Validation\nThe cross validation setting is used by setting the eval parameter to train_cv or test_cv. In both cases, the data set is split into \\(k\\) folds. The model is trained on \\(k-1\\) folds and evaluated on the remaining fold. This is repeated \\(k\\) times, so that each fold is used exactly once for evaluation. The final evaluation is performed on the test data set. The cross validation setting is useful for small data sets, because it allows to use all data for training and evaluation. However, it is computationally expensive, because the model has to be trained \\(k\\) times.\n\n\n\n\n\n\nNote\n\n\n\nCombinations of the above settings are possible, e.g., cross validation can be used for training and hold-out for evaluation or vice versa. Also, cross validation can be used for training and testing. Because cross validation is not used in the PyTorch tutorial (PyTorch 2023a), it is not considered further here.\n\n\n\n\nOverview of the Evaluation Settings\n\nSettings for the Hyperparameter Tuning\nTable\u00a02 provides an overview of the training evaluations.\n\n\nTable\u00a02: Overview of the evaluation settings.\n\n\n\n\n\n\n\n\n\neval\ntrain\ntest\nfunction\ncomment\n\n\n\n\n\"train_hold_out\"\n\\(\\checkmark\\)\n\ntrain_hold_out(), validate_fold_or_hold_out() for early stopping\nsplits the train data set internally\n\n\n\"test_hold_out\"\n\\(\\checkmark\\)\n\\(\\checkmark\\)\ntrain_hold_out(), validate_fold_or_hold_out() for early stopping\nuse the test data set for validate_fold_or_hold_out()\n\n\n\"train_cv\"\n\\(\\checkmark\\)\n\nevaluate_cv(net, train)\nCV using the train data set\n\n\n\"test_cv\"\n\n\\(\\checkmark\\)\nevaluate_cv(net, test)\nCV using the test data set . Identical to \"train_cv\", uses only test data.\n\n\n\n\n\n\"train_cv\" and \"test_cv\" use sklearn.model_selection.KFold() internally.\n\n\n\n\nDetailed Description of the \"train_hold_out\" Setting\nThe \"train_hold_out\" setting is used by default. It uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as follows:\n\n\ndf_eval, _ = evaluate_hold_out(\n    model,\n    train_dataset=fun_control[\"train\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    loss_function=self.fun_control[\"loss_function\"],\n    metric=self.fun_control[\"metric_torch\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n    path=self.fun_control[\"path\"],\n) \n\nNote: Only the data set fun_control[\"train\"] is used for training and validation. It is used as follows:\n\ntrainloader, valloader = create_train_val_data_loaders(\n                dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle\n            )\n\ncreate_train_val_data_loaders() splits the train_dataset into trainloader and valloader using torch.utils.data.random_split() as follows:\n\ndef create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):\n    test_abs = int(len(dataset) * 0.6)\n    train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) - test_abs])\n    trainloader = torch.utils.data.DataLoader(\n        train_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    valloader = torch.utils.data.DataLoader(\n        val_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    return trainloader, valloader\n\nThe optimizer is set up as follows:\n\nlr_mult_instance = net.lr_mult\noptimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_mult=lr_mult_instance)\n\n\nevaluate_hold_out() sets the net attributes such as epochs, batch_size, optimizer, and patience. For each epoch, the methods train_hold_out() and validate_fold_or_hold_out() are called, the former for training and the latter for validation and early stopping. The validation loss from the last epoch (not the best validation loss) is returned from evaluate_hold_out.\nThe method train_hold_out() is implemented as follows:\n\n\ndef train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval=10_000):\n    running_loss = 0.0\n    epoch_steps = 0\n    for i, data in enumerate(trainloader, 0):\n        inputs, labels = data\n        inputs, labels = inputs.to(device), labels.to(device)\n        optimizer.zero_grad()\n        outputs = net(inputs)\n        loss = loss_function(outputs, labels)\n        loss.backward()\n        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)\n        optimizer.step()\n        running_loss += loss.item()\n        epoch_steps += 1\n        if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches\n            print(\n                \"Batch: %5d. Batch Size: %d. Training Loss (running): %.3f\"\n                % (i + 1, int(batch_size), running_loss / epoch_steps)\n            )\n            running_loss = 0.0\n    return loss.item()\n\n\nThe method validate_fold_or_hold_out() is implemented as follows:\n\n\ndef validate_fold_or_hold_out(net, valloader, loss_function, metric, device):\n    val_loss = 0.0\n    val_steps = 0\n    metric.reset()\n    for i, data in enumerate(valloader, 0):\n        with torch.no_grad():\n            inputs, labels = data\n            inputs, labels = inputs.to(device), labels.to(device)\n            outputs = net(inputs)\n            _, predicted = torch.max(outputs.data, 1)\n            metric_value = metric(predicted, labels).to(device)\n            loss = loss_function(outputs, labels)\n            val_loss += loss.cpu().numpy()\n            val_steps += 1\n    loss = val_loss / val_steps\n    metric_value = metric.compute()\n    return metric_value, loss\n\n\n\nDetailed Description of the \"test_hold_out\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar to the \"train_hold_out\" setting with one exception: It passes an additional test data set to evaluate_hold_out() as follows:\n\n\ntest_dataset=fun_control[\"test\"]\n\nevaluate_hold_out() calls create_train_test_data_loaders instead of create_train_val_data_loaders as follows: The two data sets are used in create_train_test_data_loaders as follows:\n\ndef create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers=0):\n    trainloader = torch.utils.data.DataLoader(\n        dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    testloader = torch.utils.data.DataLoader(\n        test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    return trainloader, testloader\n\n\nThe following steps are identical to the \"train_hold_out\" setting. Only a different data loader is used for testing.\n\n\n\nDetailed Description of the \"train_cv\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:\n\n\ndf_eval, _ = evaluate_cv(\n    model,\n    dataset=fun_control[\"train\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n)\n\nNote: Only the data set fun_control[\"train\"] is used for CV. 3. In `evaluate_cv(), the following steps are performed: The optimizer is set up as follows:\n\nlr_instance = net.lr\noptimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_mult=lr_mult_instance)\n\nevaluate_cv() sets the net attributes such as epochs, batch_size, optimizer, and patience. CV is implemented as follows:\n\nkfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)\nfor fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):\n    train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)\n    val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)\n    trainloader = torch.utils.data.DataLoader(\n        dataset, batch_size=batch_size_instance, sampler=train_subsampler, num_workers=num_workers\n    )\n    valloader = torch.utils.data.DataLoader(\n        dataset, batch_size=batch_size_instance, sampler=val_subsampler, num_workers=num_workers\n    )\n    reset_weights(net)\n    # Train fold for several epochs:\n    train_fold(\n        net,\n        trainloader,\n        epochs_instance,\n        loss_function,\n        optimizer,\n        device,\n        show_batch_interval=show_batch_interval,\n    )\n    # Validate fold: use only loss for tuning\n    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)\ndf_eval = sum(loss_values.values()) / len(loss_values.values())\n\n\nThe method train_fold() is implemented as follows:\n\n\ndef train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval=10_000):\n    for epoch in range(epochs):\n        print(f\"Epoch: {epoch + 1}\")\n        running_loss = 0.0\n        epoch_steps = 0\n        for i, data in enumerate(trainloader, 0):\n            inputs, labels = data\n            inputs, labels = inputs.to(device), labels.to(device)\n            optimizer.zero_grad()\n            outputs = net(inputs)\n            loss = loss_function(outputs, labels)\n            loss.backward()\n            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)\n            optimizer.step()\n            # the following is for printing the statistic only\n            running_loss += loss.item()\n            epoch_steps += 1\n            if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches\n                print(\"Batch: %5d. Training Loss (running): %.3f\" % (i + 1, running_loss / epoch_steps))\n                running_loss = 0.0\n\n\nThe method validate_fold_or_hold_out() is implemented as shown above. In contrast to the hold-out setting, it is called for each of the \\(k\\) folds. The results are stored in a dictionaries metric_values and loss_values as follows:\n\n\n    # Validate fold: use only loss for tuning\n    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)\ndf_eval = sum(loss_values.values()) / len(loss_values.values())\n\nThe results are averaged over the \\(k\\) folds and returned as df_eval.\n\n\nDetailed Description of the \"test_cv\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:\n\n\ndf_eval, _ = evaluate_cv(\n    model,\n    dataset=fun_control[\"test\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n)\n\nNote: The data set fun_control[\"test\"] is used for CV. The rest is the same as for the \"train_cv\" setting.\n\n\nSettings for the Final Evaluation of the Tuned Architecture\n\nTraining of the Tuned Architecture\ntrain_tuned(model, train): train the model with the best hyperparameter configuration (or simply the default) on the training data set. It splits the traindata into new train and validation sets using create_train_val_data_loaders(), which calls torch.utils.data.random_split() internally. Currently, 60% of the data is used for training and 40% for validation. The train data is used for training the model with train_hold_out(). The validation data is used for early stopping using validate_fold_or_hold_out() on the validation data set.\ntrain_tuned() is just a wrapper to evaluate_hold_out using the train data set. It is implemented as follows:\n\ndef train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_interval=10_000, path=None):\n    evaluate_hold_out(\n        net=net,\n        train_dataset=train_dataset,\n        shuffle=shuffle,\n        test_dataset=None,\n        loss_function=loss_function,\n        metric=metric,\n        device=device,\n        show_batch_interval=show_batch_interval,\n        path=path,\n    )\n\nNote: During training, shuffle is set to True, whereas during testing, shuffle is set to False.\n\n\nTesting of the Tuned Architecture\ntest_tuned(model, test): test the model on the test data set. No data splitting is performed. The (trained) model is evaluated using the validate_fold_or_hold_out() function.\nNote: During training, shuffle is set to True, whereas during testing, shuffle is set to False.\n\ndef test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None, path=None):\n    batch_size_instance = net.batch_size\n    removed_attributes, net = get_removed_attributes_and_base_net(net)\n    if path is not None:\n        net.load_state_dict(torch.load(path))\n        net.eval()\n    try:\n        device = getDevice(device=device)\n        if torch.cuda.is_available():\n            device = \"cuda:0\"\n            if torch.cuda.device_count() &gt; 1:\n                print(\"We will use\", torch.cuda.device_count(), \"GPUs!\")\n                net = nn.DataParallel(net)\n        net.to(device)\n        valloader = torch.utils.data.DataLoader(\n            test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0\n        )\n        metric_value, loss = validate_fold_or_hold_out(\n            net, valloader=valloader, loss_function=loss_function, metric=metric, device=device\n        )\n        df_eval = loss\n        df_metric = metric_value\n        df_preds = np.nan\n    except Exception as err:\n        print(f\"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}\")\n        df_eval = np.nan\n        df_metric = np.nan\n        df_preds = np.nan\n    add_attributes(net, removed_attributes)\n    print(f\"Final evaluation: Validation loss: {df_eval}\")\n    print(f\"Final evaluation: Validation metric: {df_metric}\")\n    print(\"----------------------------------------------\")\n    return df_eval, df_preds, df_metric\n\n\n\n\n\nLoss Functions and Metrics\nThe key \"loss_function\" specifies the loss function which is used during the optimization. There are several different loss functions under PyTorch\u2019s nn package. For example, a simple loss is MSELoss, which computes the mean-squared error between the output and the target. In this tutorial we will use CrossEntropyLoss, because it is also used in the PyTorch tutorial.\n\nfrom torch.nn import CrossEntropyLoss\nloss_function = CrossEntropyLoss()\nfun_control.update({\"loss_function\": loss_function})\n\nIn addition to the loss functions, spotPython provides access to a large number of metrics. The key \"metric_sklearn\" is used for metrics that follow the scikit-learn conventions. The key \"river_metric\" is used for the river based evaluation (Montiel et al. 2021) via eval_oml_iter_progressive, and the key \"metric_torch\" is used for the metrics from TorchMetrics. TorchMetrics is a collection of more than 90 PyTorch metrics4. Because the PyTorch tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial\u2019s example code. We will use TorchMetrics instead, because it offers:\n\nA standardized interface to increase reproducibility\nReduces Boilerplate\nDistributed-training compatible\nRigorously tested\nAutomatic accumulation over batches\nAutomatic synchronization between multiple devices\n\nTherefore, we set\n\nmetric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=10)\n\n\nloss_function = CrossEntropyLoss()\nweights = 1.0\nmetric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=10)\nshuffle = True\neval = \"train_hold_out\"\ndevice = DEVICE\nshow_batch_interval = 100_000\npath=\"torch_model.pt\"\n\nfun_control.update({\n               \"data_dir\": None,\n               \"checkpoint_dir\": None,\n               \"horizon\": None,\n               \"oml_grace_period\": None,\n               \"weights\": weights,\n               \"step\": None,\n               \"log_level\": 50,\n               \"weight_coeff\": None,\n               \"metric_torch\": metric_torch,\n               \"metric_river\": None,\n               \"metric_sklearn\": None,\n               \"loss_function\": loss_function,\n               \"shuffle\": shuffle,\n               \"eval\": eval,\n               \"device\": device,\n               \"show_batch_interval\": show_batch_interval,\n               \"path\": path,\n               })",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-call-the-hyperparameter-tuner",
         "objectID": "bart23e.html#sec-call-the-hyperparameter-tuner",
         "section": "Calling the SPOT Function",
-        "text": "Calling the SPOT Function\nNow, the dictionary fun_control contains all information needed for the hyperparameter tuning. Before the hyperparameter tuning is started, it is recommended to take a look at the experimental design. The method gen_design_table generates a design table as follows:\n\nprint(gen_design_table(fun_control))\n\nThis allows to check if all information is available and if the information is correct. Table\u00a02 shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column \u201ctransform\u201d, e.g., the l1 default is 5, which results in the value \\(2^5 = 32\\) for the network, because the transformation transform_power_2_int was selected in the JSON file. The default value of the batch_size is set to 4, which results in a batch size of \\(2^4 = 16\\).\n\n\nTable\u00a02: Experimental design for the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The transformation function is used to transform the hyperparameter values from the unit hypercube to the original domain. The transformation function is applied to the hyperparameter values before the evaluation of the objective function.\n\n\n\n\n\n\n\n\n\n\nname\ntype\ndefault\nlower\nupper\ntransform\n\n\n\n\nl1\nint\n5\n2\n9\ntransform_power_2_int\n\n\nl2\nint\n5\n2\n9\ntransform_power_2_int\n\n\nlr\nfloat\n0.001\n0.001\n0.001\nNone\n\n\nbatch_size\nint\n4\n1\n5\ntransform_power_2_int\n\n\nepochs\nint\n3\n3\n4\ntransform_power_2_int\n\n\nk_folds\nint\n2\n0\n0\nNone\n\n\npatience\nint\n5\n3\n3\nNone\n\n\noptimizer\nfactor\nSGD\n0\n9\nNone\n\n\ncriterion\nfactor\nCrossEntropyLoss\n0\n0\nNone\n\n\n\n\nThe objective function fun_torch is selected next. It implements an interface from PyTorch\u2019s training, validation, and testing methods to spotPython.\n\nfun = HyperTorch().fun_torch\n\nThe spotPython hyperparameter tuning is started by calling the Spot function. Here, we will run the tuner for approximately 30 minutes (max_time). Note: the initial design is always evaluated in the spotPython run. As a consequence, the run may take longer than specified by max_time, because the evaluation time of initial design (here: init_size, 10 points) is performed independently of max_time.\n\nspot_tuner = spot.Spot(fun=fun,\n                   lower = lower,\n                   upper = upper,\n                   fun_evals = inf,\n                   fun_repeats = 1,\n                   max_time = MAX_TIME,\n                   noise = False,\n                   tolerance_x = np.sqrt(np.spacing(1)),\n                   var_type = var_type,\n                   var_name = var_name,\n                   infill_criterion = \"y\",\n                   n_points = 1,\n                   seed=123,\n                   log_level = 50,\n                   show_models= False,\n                   show_progress= True,\n                   fun_control = fun_control,\n                   design_control={\"init_size\": INIT_SIZE,\n                                   \"repeats\": 1},\n                   surrogate_control={\"noise\": True,\n                                      \"cod_type\": \"norm\",\n                                      \"min_theta\": -4,\n                                      \"max_theta\": 3,\n                                      \"n_theta\": len(var_name),\n                                      \"model_optimizer\": differential_evolution,\n                                      \"model_fun_evals\": 10_000,\n                                      \"log_level\": 50\n                                      })\nspot_tuner.run(X_start=X_start)\n\nDuring the run, the following output is shown:\nconfig: {'l1': 8, 'l2': 16, 'lr': 0.001, 'batch_size': 2, \n'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'NAdam', \n'criterion': CrossEntropyLoss()}\nEpoch: 1\nLoss on hold-out set: 1.798599960240349\nAccuracy on hold-out set: 0.38035\nEpoch: 2\nLoss on hold-out set: 1.681505929086823\nAccuracy on hold-out set: 0.4163\nEpoch: 3\nLoss on hold-out set: 1.6875325478885324\nAccuracy on hold-out set: 0.42245\nEpoch: 4\nLoss on hold-out set: 1.6695034023197601\nAccuracy on hold-out set: 0.45265\nEpoch: 5\nLoss on hold-out set: 1.6984369342865335\nAccuracy on hold-out set: 0.45085\nEpoch: 6\nLoss on hold-out set: 1.6061365829033545\nAccuracy on hold-out set: 0.4527\nEpoch: 7\nLoss on hold-out set: 1.7061124059396433\nAccuracy on hold-out set: 0.4566\nEpoch: 8\nLoss on hold-out set: 1.7162298802530742\nAccuracy on hold-out set: 0.4504\nEpoch: 9\nLoss on hold-out set: 1.6683832777252945\nAccuracy on hold-out set: 0.47205\nEarly stopping at epoch 8\nReturned to Spot: Validation loss: 1.6683832777252945",
+        "text": "Calling the SPOT Function\nNow, the dictionary fun_control contains all information needed for the hyperparameter tuning. Before the hyperparameter tuning is started, it is recommended to take a look at the experimental design. The method gen_design_table generates a design table as follows:\n\nprint(gen_design_table(fun_control))\n\nThis allows to check if all information is available and if the information is correct. Table\u00a03 shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column \u201ctransform\u201d, e.g., the l1 default is 5, which results in the value \\(2^5 = 32\\) for the network, because the transformation transform_power_2_int was selected in the JSON file. The default value of the batch_size is set to 4, which results in a batch size of \\(2^4 = 16\\).\n\n\nTable\u00a03: Experimental design for the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The transformation function is used to transform the hyperparameter values from the unit hypercube to the original domain. The transformation function is applied to the hyperparameter values before the evaluation of the objective function.\n\n\n\n\n\n\n\n\n\n\nname\ntype\ndefault\nlower\nupper\ntransform\n\n\n\n\nl1\nint\n5\n2\n9\ntransform_power_2_int\n\n\nl2\nint\n5\n2\n9\ntransform_power_2_int\n\n\nlr\nfloat\n0.001\n0.001\n0.001\nNone\n\n\nbatch_size\nint\n4\n1\n5\ntransform_power_2_int\n\n\nepochs\nint\n3\n3\n4\ntransform_power_2_int\n\n\nk_folds\nint\n2\n0\n0\nNone\n\n\npatience\nint\n5\n3\n3\nNone\n\n\noptimizer\nfactor\nSGD\n0\n9\nNone\n\n\n\n\nThe objective function fun_torch is selected next. It implements an interface from PyTorch\u2019s training, validation, and testing methods to spotPython.\n\nfun = HyperTorch().fun_torch\n\nThe spotPython hyperparameter tuning is started by calling the Spot function. Here, we will run the tuner for approximately 30 minutes (max_time). Note: the initial design is always evaluated in the spotPython run. As a consequence, the run may take longer than specified by max_time, because the evaluation time of initial design (here: init_size, 10 points) is performed independently of max_time.\n\nspot_tuner = spot.Spot(fun=fun,\n                   lower = lower,\n                   upper = upper,\n                   fun_evals = inf,\n                   fun_repeats = 1,\n                   max_time = MAX_TIME,\n                   noise = False,\n                   tolerance_x = np.sqrt(np.spacing(1)),\n                   var_type = var_type,\n                   var_name = var_name,\n                   infill_criterion = \"y\",\n                   n_points = 1,\n                   seed=123,\n                   log_level = 50,\n                   show_models= False,\n                   show_progress= True,\n                   fun_control = fun_control,\n                   design_control={\"init_size\": INIT_SIZE,\n                                   \"repeats\": 1},\n                   surrogate_control={\"noise\": True,\n                                      \"cod_type\": \"norm\",\n                                      \"min_theta\": -4,\n                                      \"max_theta\": 3,\n                                      \"n_theta\": len(var_name),\n                                      \"model_optimizer\": differential_evolution,\n                                      \"model_fun_evals\": 10_000,\n                                      \"log_level\": 50\n                                      })\nspot_tuner.run(X_start=X_start)\n\nDuring the run, the following output is shown:\nconfig: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'Adadelta', 'sgd_momentum': 0.9}\nEpoch: 1\nLoss on hold-out set: 1.602842689704895\nAccuracy on hold-out set: 0.4006\nMetric value on hold-out data: 0.40059998631477356\nEpoch: 2\nLoss on hold-out set: 1.4648857820034027\nAccuracy on hold-out set: 0.47685\nMetric value on hold-out data: 0.4768500030040741\nEpoch: 3\nLoss on hold-out set: 1.403354868555069\nAccuracy on hold-out set: 0.482\nMetric value on hold-out data: 0.4819999933242798\nEpoch: 4\nLoss on hold-out set: 1.384560032081604\nAccuracy on hold-out set: 0.49065\nMetric value on hold-out data: 0.4906499981880188\nEpoch: 5\nLoss on hold-out set: 1.4326466094970702\nAccuracy on hold-out set: 0.4809\nMetric value on hold-out data: 0.48089998960494995\nEpoch: 6\nLoss on hold-out set: 1.3759961807250976\nAccuracy on hold-out set: 0.4995\nMetric value on hold-out data: 0.49950000643730164\nEpoch: 7\nLoss on hold-out set: 1.3684927892208099\nAccuracy on hold-out set: 0.50695\nMetric value on hold-out data: 0.5069500207901001\nEpoch: 8\nLoss on hold-out set: 1.3642385012149811\nAccuracy on hold-out set: 0.506\nMetric value on hold-out data: 0.5059999823570251\nEpoch: 9\nLoss on hold-out set: 1.3157437609672546\nAccuracy on hold-out set: 0.5304\nMetric value on hold-out data: 0.5303999781608582\nEpoch: 10\nLoss on hold-out set: 1.3481314319610596\nAccuracy on hold-out set: 0.5268\nMetric value on hold-out data: 0.5267999768257141\nEpoch: 11\nLoss on hold-out set: 1.3608774542331696\nAccuracy on hold-out set: 0.51525\nMetric value on hold-out data: 0.515250027179718\nEpoch: 12\nLoss on hold-out set: 1.359324642753601\nAccuracy on hold-out set: 0.52355\nMetric value on hold-out data: 0.5235499739646912\nEarly stopping at epoch 11\nReturned to Spot: Validation loss: 1.359324642753601\n----------------------------------------------",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-results-tuning",
         "objectID": "bart23e.html#sec-results-tuning",
         "section": "Results",
-        "text": "Results\nAfter the hyperparameter tuning run is finished, the progress of the hyperparameter tuning can be visualized. The following code generates the progress plot from Figure\u00a02.\n\n\nspot_tuner.plot_progress(log_y=False, filename=\"./figures\" + experiment_name+\"_progress.pdf\")\nFigure\u00a01: ?(caption)\n\n\n\n\n\nFigure\u00a02: Progress plot. Black dots denote results from the initial design. Red dots illustrate the improvement found by the surrogate model based optimization (surrogate model based optimization).\n\n\nFigure\u00a02 shows a typical behaviour that can be observed in many hyperparameter studies (Bartz et al. 2022): the largest improvement is obtained during the evaluation of the initial design. The surrogate model based optimization-optimization with the surrogate refines the results. Figure\u00a02 also illustrates one major difference between ray[tune] as used in PyTorch (2023a) and spotPython: the ray[tune] uses a random search and will generate results similar to the black dots, whereas spotPython uses a surrogate model based optimization and presents results represented by red dots in Figure\u00a02. The surrogate model based optimization is considered to be more efficient than a random search, because the surrogate model guides the search towards promising regions in the hyperparameter space.\nIn addition to the improved (\u201coptimized\u201d) hyperparameter values, spotPython allows a statistical analysis, e.g., a sensitivity analysis, of the results. We can print the results of the hyperparameter tuning, see Table\u00a03.\n\nprint(gen_design_table(fun_control=fun_control, spot=spot_tuner))\n\n\n\nTable\u00a03: Results of the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The column \u201ctuned\u201d shows the tuned values. The column \u201cimportance\u201d shows the importance of the hyperparameters. The column \u201cstars\u201d shows the importance of the hyperparameters in stars. The importance is computed by the SPOT software.\n\n\n\n\n\n\n\n\n\n\n\n\n\nname\ntype\ndefault\nlower\nupper\ntuned\ntransform\nimportance\nstars\n\n\n\n\nl1\nint\n5\n2.0\n9.0\n7.0\npow_2_int\n100.00\n***\n\n\nl2\nint\n5\n2.0\n9.0\n3.0\npow_2_int\n96.29\n***\n\n\nlr\nfloat\n0.001\n0.001\n0.001\n0.001\nNone\n0.00\n\n\n\nbatchsize\nint\n4\n1.0\n5.0\n4.0\npow_2_int\n0.00\n\n\n\nepochs\nint\n3\n3.0\n4.0\n4.0\npow_2_int\n4.18\n*\n\n\nk_folds\nint\n2\n0.0\n0.0\n0.0\nNone\n0.00\n\n\n\npatience\nint\n5\n3.0\n3.0\n3.0\nNone\n0.00\n\n\n\noptimizer\nfactor\nSGD\n0.0\n9.0\n3.0\nNone\n0.16\n.\n\n\ncriterion\nfactor\nCrossEntLoss\n0.0\n0.0\n0.0\nNone\n0.00\n\n\n\n\n\nTo visualize the most important hyperparameters, spotPython provides the function plot_importance. The following code generates the importance plot from Figure\u00a03.\n\nspot_tuner.plot_importance(threshold=0.025, filename=\"./figures\" + experiment_name+\"_importance.pdf\")\n\n\n\n\nFigure\u00a03: Variable importance",
+        "text": "Results\nAfter the hyperparameter tuning run is finished, the progress of the hyperparameter tuning can be visualized. The following code generates the progress plot from Figure\u00a02.\n\n\nspot_tuner.plot_progress(log_y=False, filename=\"./figures\" + experiment_name+\"_progress.png\")\nFigure\u00a01: ?(caption)\n\n\n\n\n\nFigure\u00a02: Progress plot. Black dots denote results from the initial design. Red dots illustrate the improvement found by the surrogate model based optimization (surrogate model based optimization).\n\n\nFigure\u00a02 shows a typical behaviour that can be observed in many hyperparameter studies (Bartz et al. 2022): the largest improvement is obtained during the evaluation of the initial design. The surrogate model based optimization-optimization with the surrogate refines the results. Figure\u00a02 also illustrates one major difference between ray[tune] as used in PyTorch (2023a) and spotPython: the ray[tune] uses a random search and will generate results similar to the black dots, whereas spotPython uses a surrogate model based optimization and presents results represented by red dots in Figure\u00a02. The surrogate model based optimization is considered to be more efficient than a random search, because the surrogate model guides the search towards promising regions in the hyperparameter space.\nIn addition to the improved (\u201coptimized\u201d) hyperparameter values, spotPython allows a statistical analysis, e.g., a sensitivity analysis, of the results. We can print the results of the hyperparameter tuning, see Table\u00a04.\n\nprint(gen_design_table(fun_control=fun_control, spot=spot_tuner))\n\n\n\nTable\u00a04: Results of the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The column \u201ctuned\u201d shows the tuned values. The column \u201cimportance\u201d shows the importance of the hyperparameters. The column \u201cstars\u201d shows the importance of the hyperparameters in stars. The importance is computed by the SPOT software.\n\n\n\n\n\n\n\n\n\n\n\n\n\nname\ntype\ndefault\nlower\nupper\ntuned\ntransform\nimportance\nstars\n\n\n\n\nl1\nint\n5\n2.0\n9.0\n7.0\npow_2_int\n100.00\n***\n\n\nl2\nint\n5\n2.0\n9.0\n3.0\npow_2_int\n96.29\n***\n\n\nlr_mult\nfloat\n1.0\n0.1\n10.0\n0.1\nNone\n0.00\n\n\n\nbatchsize\nint\n4\n1.0\n5.0\n4.0\npow_2_int\n0.00\n\n\n\nepochs\nint\n3\n3.0\n4.0\n4.0\npow_2_int\n4.18\n*\n\n\nk_folds\nint\n2\n0.0\n0.0\n0.0\nNone\n0.00\n\n\n\npatience\nint\n5\n3.0\n3.0\n3.0\nNone\n0.00\n\n\n\noptimizer\nfactor\nSGD\n0.0\n9.0\n3.0\nNone\n0.16\n.\n\n\n\n\nTo visualize the most important hyperparameters, spotPython provides the function plot_importance. The following code generates the importance plot from Figure\u00a03.\n\nspot_tuner.plot_importance(threshold=0.025, filename=\"./figures\" + experiment_name+\"_importance.png\")\n\n\n\n\nFigure\u00a03: Variable importance",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-get-spot-results",
         "objectID": "bart23e.html#sec-get-spot-results",
         "section": "Get SPOT Results",
         "text": "Get SPOT Results\nThe architecture of the spotPython model can be obtained by the following code:\n\nX = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))\nmodel_spot = get_one_core_model_from_X(X, fun_control)\nmodel_spot\n\nFirst, the numerical representation of the hyperparameters are obtained, i.e., the numpy array X is generated. This array is then used to generate the model model_spot by the function get_one_core_model_from_X. The model model_spot has the following architecture:\nNet_CIFAR10(\n  (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))\n  (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)\n  (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))\n  (fc1): Linear(in_features=400, out_features=64, bias=True)\n  (fc2): Linear(in_features=64, out_features=32, bias=True)\n  (fc3): Linear(in_features=32, out_features=10, bias=True)\n)",
@@ -90,39 +90,39 @@
         "text": "Get Default Hyperparameters\nIn a similar manner as in Section\u00a03.11, the default hyperparameters can be obtained.\n\n# fun_control was modified, we generate a new one with the original default hyperparameters\nfc = copy.deepcopy(fun_control)\nfc.update({\"core_model_hyper_dict\": hyper_dict[fun_control[\"core_model\"].__name__]})\nmodel_default = get_one_core_model_from_X(X_start, fun_control=fc)\n\nThe corresponding default model has the following architecture:\nNet_CIFAR10(\n  (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))\n  (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)\n  (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))\n  (fc1): Linear(in_features=400, out_features=32, bias=True)\n  (fc2): Linear(in_features=32, out_features=32, bias=True)\n  (fc3): Linear(in_features=32, out_features=10, bias=True)\n)",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#evaluation-of-the-tuned-architecture",
         "objectID": "bart23e.html#evaluation-of-the-tuned-architecture",
         "section": "Evaluation of the Tuned Architecture",
-        "text": "Evaluation of the Tuned Architecture\nThe method train_save takes a model architecture without trained weights and trains this model with the train data. The train data is split into train and validation data. The validation data is used for early stopping. The trained model weights are saved as a dictionary.\nThis evaluation is similar to the final evaluation in PyTorch (2023a).\n\ntrain_save(net=model_default, train_dataset=train, shuffle=True,\n        device = \"cpu\", show_batch_interval=1_000, \n        path=\"model_default_trained.pt\", save_model=True)\ntest_saved(net=model_default, test_dataset=test, shuffle=False, \n        device = \"cpu\", path=\"model_default_trained.pt\")\n\nThe following code trains the model model_spot and saves the weights of the trained model to the file model_spot_trained.pt.\n\ntrain_save(net=model_spot, train_dataset=train,\n                shuffle=True, path=\"model_spot_trained.pt\", save_model=True)\n\nLoss on hold-out set: 1.2267619131326675\nAccuracy on hold-out set: 0.58955\nEarly stopping at epoch 13\n\ntest_saved(net=model_spot, test_dataset=test,\n            shuffle=False, path=\"model_spot_trained.pt\")\n\nLoss on hold-out set: 1.242568492603302\nAccuracy on hold-out set: 0.5957",
+        "text": "Evaluation of the Tuned Architecture\nThe method train_tuned takes a model architecture without trained weights and trains this model with the train data. The train data is split into train and validation data. The validation data is used for early stopping. The trained model weights are saved as a dictionary.\nThis evaluation is similar to the final evaluation in PyTorch (2023a).\n\ntrain_tuned(net=model_default, train_dataset=train, shuffle=True,\n        loss_function=fun_control[\"loss_function\"],\n        metric=fun_control[\"metric_torch\"],\n        device = DEVICE, show_batch_interval=1_000,)\ntest_tuned(net=model_default, test_dataset=test, \n        loss_function=fun_control[\"loss_function\"],\n        metric=fun_control[\"metric_torch\"],\n        shuffle=False, \n        device = DEVICE)\n\nThe following code trains the model model_spot. If path is set to a filename, e.g., path = \"model_spot_trained.pt\", the weights of the trained model will be saved to this file.\n\ntrain_tuned(net=model_spot, train_dataset=train,\n        loss_function=fun_control[\"loss_function\"],\n        metric=fun_control[\"metric_torch\"],\n        shuffle=True,\n        device = DEVICE,\n        path=None)\n\nLoss on hold-out set: 1.2267619131326675\nAccuracy on hold-out set: 0.58955\nEarly stopping at epoch 13\nIf path is set to a filename, e.g., path = \"model_spot_trained.pt\", the weights of the trained model will be loaded from this file.\n\ntest_tuned(net=model_spot, test_dataset=test,\n            shuffle=False,\n            loss_function=fun_control[\"loss_function\"],\n            metric=fun_control[\"metric_torch\"],\n            device = DEVICE)\n\nLoss on hold-out set: 1.242568492603302\nAccuracy on hold-out set: 0.5957",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#comparison-with-default-hyperparameters-and-ray-tune",
         "objectID": "bart23e.html#comparison-with-default-hyperparameters-and-ray-tune",
         "section": "Comparison with Default Hyperparameters and Ray Tune",
-        "text": "Comparison with Default Hyperparameters and Ray Tune\nTable\u00a04 shows the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune].\n\n\nTable\u00a04: Comparison of the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune]. ray[tune] only shows the validation loss, because training loss is not reported by ray[tune].\n\n\n\n\n\n\n\n\n\nModel\nValidation Loss\nValidation Accuracy\nLoss\nAccuracy\n\n\n\n\nDefault\n2.1221\n0.2452\n2.1182\n0.2425\n\n\nspotPython\n1.2268\n0.5896\n1.2426\n0.5957\n\n\nray[tune]\n1.1815\n0.5836\n-\n0.5806",
+        "text": "Comparison with Default Hyperparameters and Ray Tune\nTable\u00a05 shows the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune].\n\n\nTable\u00a05: Comparison of the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune]. ray[tune] only shows the validation loss, because training loss is not reported by ray[tune].\n\n\n\n\n\n\n\n\n\nModel\nValidation Loss\nValidation Accuracy\nLoss\nAccuracy\n\n\n\n\nDefault\n2.1221\n0.2452\n2.1182\n0.2425\n\n\nspotPython\n1.2268\n0.5896\n1.2426\n0.5957\n\n\nray[tune]\n1.1815\n0.5836\n-\n0.5806",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#detailed-hyperparameter-plots",
         "objectID": "bart23e.html#detailed-hyperparameter-plots",
         "section": "Detailed Hyperparameter Plots",
-        "text": "Detailed Hyperparameter Plots\nThe contour plots in this section visualize the interactions of the three most important hyperparameters, l1, l2, and epochs, and optimizer of the surrogate model used to optimize the hyperparameters. Since some of these hyperparameters take fatorial or integer values, sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook (Bartz-Beielstein 2023).\n\n\nthreshold = 0.025\nimpo = spot_tuner.print_importance(threshold=threshold, print_screen=True)\nvar_plots = [i for i, x in enumerate(impo) if x[1] &gt; threshold]\nmin_z = min(spot_tuner.y)\nmax_z = max(spot_tuner.y)\nn = spot_tuner.k\nfor i in var_plots:\n    for j in var_plots:\n        if j &gt; i:\n            filename = \"./figures\" + experiment_name+\"_contour_\"+str(i)+\"_\"+str(j)+\".pdf\"\n            spot_tuner.plot_contour(i=i, j=j, min_z=min_z, max_z = max_z, filename=filename)\nFigure\u00a04: ?(caption)\n\n\n\n\n\nFigure\u00a05: Contour plot of the loss as a function of l1 and l2, i.e., the number of neurons in the layers.\n\n\n\n\n\nFigure\u00a06: Contour plot of the loss as a function of the number of epochs and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a07: Contour plot of the loss as a function of the optimizer and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a08: Contour plot of the loss as a function of the number of epochs and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a09: Contour plot of the loss as a function of the optimizer and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a010: Contour plot of the loss as a function of the optimizer and the number of epochs.\n\n\nFigure\u00a05 to Figure\u00a010 show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. spotPython provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, Figure\u00a012 shows the parallel plot of the hyperparameters.\n\n\nspot_tuner.parallel_plot()\nFigure\u00a011: ?(caption)\n\n\n\n\n\nFigure\u00a012: Parallel plot",
+        "text": "Detailed Hyperparameter Plots\nThe contour plots in this section visualize the interactions of the three most important hyperparameters, l1, l2, and epochs, and optimizer of the surrogate model used to optimize the hyperparameters. Since some of these hyperparameters take fatorial or integer values, sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook (Bartz-Beielstein 2023).\n\n\nthreshold = 0.025\nimpo = spot_tuner.print_importance(threshold=threshold, print_screen=True)\nvar_plots = [i for i, x in enumerate(impo) if x[1] &gt; threshold]\nmin_z = min(spot_tuner.y)\nmax_z = max(spot_tuner.y)\nn = spot_tuner.k\nfor i in var_plots:\n    for j in var_plots:\n        if j &gt; i:\n            filename = \"./figures\" + experiment_name+\"_contour_\"+str(i)+\"_\"+str(j)+\".png\"\n            spot_tuner.plot_contour(i=i, j=j, min_z=min_z, max_z = max_z, filename=filename)\nFigure\u00a04: ?(caption)\n\n\n\n\n\nFigure\u00a05: Contour plot of the loss as a function of l1 and l2, i.e., the number of neurons in the layers.\n\n\n\n\n\nFigure\u00a06: Contour plot of the loss as a function of the number of epochs and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a07: Contour plot of the loss as a function of the optimizer and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a08: Contour plot of the loss as a function of the number of epochs and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a09: Contour plot of the loss as a function of the optimizer and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a010: Contour plot of the loss as a function of the optimizer and the number of epochs.\n\n\nFigure\u00a05 to Figure\u00a010 show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. spotPython provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, Figure\u00a012 shows the parallel plot of the hyperparameters.\n\n\nspot_tuner.parallel_plot()\nFigure\u00a011: ?(caption)\n\n\n\n\n\nFigure\u00a012: Parallel plot",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sample-output-from-ray-tunes-run",
         "objectID": "bart23e.html#sample-output-from-ray-tunes-run",
         "section": "Sample Output From Ray Tune\u2019s Run",
         "text": "Sample Output From Ray Tune\u2019s Run\nThe output from ray[tune] could look like this (PyTorch 2023b):\nNumber of trials: 10 (10 TERMINATED)\n------+------+-------------+--------------+---------+------------+--------------------+\n|   l1 |   l2 |          lr |   batch_size |    loss |   accuracy | training_iteration |\n+------+------+-------------+--------------+---------+------------+--------------------|\n|   64 |    4 | 0.00011629  |            2 | 1.87273 |     0.244  |                  2 |\n|   32 |   64 | 0.000339763 |            8 | 1.23603 |     0.567  |                  8 |\n|    8 |   16 | 0.00276249  |           16 | 1.1815  |     0.5836 |                 10 |\n|    4 |   64 | 0.000648721 |            4 | 1.31131 |     0.5224 |                  8 |\n|   32 |   16 | 0.000340753 |            8 | 1.26454 |     0.5444 |                  8 |\n|    8 |    4 | 0.000699775 |            8 | 1.99594 |     0.1983 |                  2 |\n|  256 |    8 | 0.0839654   |           16 | 2.3119  |     0.0993 |                  1 |\n|   16 |  128 | 0.0758154   |           16 | 2.33575 |     0.1327 |                  1 |\n|   16 |    8 | 0.0763312   |           16 | 2.31129 |     0.1042 |                  4 |\n|  128 |   16 | 0.000124903 |            4 | 2.26917 |     0.1945 |                  1 |\n+-----+------+------+-------------+--------------+---------+------------+--------------------+\nBest trial config: {'l1': 8, 'l2': 16, 'lr': 0.00276249, 'batch_size': 16, 'data_dir': '...'}\nBest trial final validation loss: 1.181501\nBest trial final validation accuracy: 0.5836\nBest trial test set accuracy: 0.5806",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#footnotes",
         "objectID": "bart23e.html#footnotes",
         "section": "Footnotes",
-        "text": "Footnotes\n\n\nhttps://github.com/sequential-parameter-optimization\u21a9\ufe0e\nAlternatively, the source code can be downloaded from gitHub: https://github.com/sequential-parameter-optimization/spotPython.\u21a9\ufe0e\nWe were not able to install Ray Tune on our system. Therefore, we used the results from the PyTorch tutorial.\u21a9\ufe0e\nThe key \"metric\" is used for the river based evaluation (Montiel et al. 2021) via eval_oml_iter_progressive.\u21a9\ufe0e",
+        "text": "Footnotes\n\n\nhttps://github.com/sequential-parameter-optimization\u21a9\ufe0e\nAlternatively, the source code can be downloaded from gitHub: https://github.com/sequential-parameter-optimization/spotPython.\u21a9\ufe0e\nWe were not able to install Ray Tune on our system. Therefore, we used the results from the PyTorch tutorial.\u21a9\ufe0e\nhttps://torchmetrics.readthedocs.io/en/latest/.\u21a9\ufe0e",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     }
 ]
```

### Comparing `spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap-icons.css` & `spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap-icons.woff` & `spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap.min.css` & `spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/bootstrap/bootstrap.min.js` & `spotPython-0.2.0/docs/site_libs/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/clipboard/clipboard.min.js` & `spotPython-0.2.0/docs/site_libs/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-html/anchor.min.js` & `spotPython-0.2.0/docs/site_libs/quarto-html/anchor.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-html/popper.min.js` & `spotPython-0.2.0/docs/site_libs/quarto-html/popper.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-html/quarto-syntax-highlighting.css` & `spotPython-0.2.0/docs/site_libs/quarto-html/quarto-syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-html/quarto.js` & `spotPython-0.2.0/docs/site_libs/quarto-html/quarto.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-html/tippy.css` & `spotPython-0.2.0/docs/site_libs/quarto-html/tippy.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-html/tippy.umd.min.js` & `spotPython-0.2.0/docs/site_libs/quarto-html/tippy.umd.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-nav/quarto-nav.js` & `spotPython-0.2.0/docs/site_libs/quarto-nav/quarto-nav.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-search/autocomplete.umd.js` & `spotPython-0.2.0/docs/site_libs/quarto-search/autocomplete.umd.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-search/fuse.min.js` & `spotPython-0.2.0/docs/site_libs/quarto-search/fuse.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/docs/site_libs/quarto-search/quarto-search.js` & `spotPython-0.2.0/docs/site_libs/quarto-search/quarto-search.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/00_spot_doc.ipynb` & `spotPython-0.2.0/notebooks/00_spot_doc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/01_spot_intro.ipynb` & `spotPython-0.2.0/notebooks/01_spot_intro.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/02_spot_multidim.ipynb` & `spotPython-0.2.0/notebooks/02_spot_multidim.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/03_spot_anisotropic.ipynb` & `spotPython-0.2.0/notebooks/03_spot_anisotropic.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/04_spot_sklearn_surrogate.ipynb` & `spotPython-0.2.0/notebooks/04_spot_sklearn_surrogate.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/05_spot_sklearn_optimizers.ipynb` & `spotPython-0.2.0/notebooks/05_spot_sklearn_optimizers.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/06_spot_gaussian.ipynb` & `spotPython-0.2.0/notebooks/06_spot_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/07_spot_ei.ipynb` & `spotPython-0.2.0/notebooks/07_spot_ei.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/08_spot_noisy.ipynb` & `spotPython-0.2.0/notebooks/08_spot_noisy.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/09_spot_ocba.ipynb` & `spotPython-0.2.0/notebooks/09_spot_ocba.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/10_spot_hpt_sklearn_classification.ipynb` & `spotPython-0.2.0/notebooks/10_spot_hpt_sklearn_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb` & `spotPython-0.2.0/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996212121212121%*

 * *Differences: {"'cells'": "{56: {'source': ['evaluate_hold_out(model_default, train_dataset = testset, "*

 * *            'shuffle=False, '*

 * *            'show_batch_interval=fun_control["show_batch_interval"],loss_function=self.fun_control["loss_function"], '*

 * *            'metric=self.fun_control["metric_torch"],)\']}, 57: {\'source\': '*

 * *            "['evaluate_hold_out(model_spot, train_dataset = testset, shuffle=False, "*

 * *            'show_batch_interval=fun_control["show_batch_interval"],loss_function=self.fun_control["loss_f […]*

```diff
@@ -713,24 +713,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_hold_out(model_default, train_dataset = testset, shuffle=False, show_batch_interval=fun_control[\"show_batch_interval\"])"
+                "evaluate_hold_out(model_default, train_dataset = testset, shuffle=False, show_batch_interval=fun_control[\"show_batch_interval\"],loss_function=self.fun_control[\"loss_function\"], metric=self.fun_control[\"metric_torch\"],)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_hold_out(model_spot, train_dataset = testset, shuffle=False, show_batch_interval=fun_control[\"show_batch_interval\"])"
+                "evaluate_hold_out(model_spot, train_dataset = testset, shuffle=False, show_batch_interval=fun_control[\"show_batch_interval\"],loss_function=self.fun_control[\"loss_function\"], metric=self.fun_control[\"metric_torch\"],)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `spotPython-0.1.8/notebooks/12_spot_hpt_torch_cifar10.ipynb` & `spotPython-0.2.0/notebooks/12_spot_hpt_torch_cifar10.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993243243243244%*

 * *Differences: {"'cells'": "{61: {'source': ['evaluate_hold_out(model_default, train_dataset = testset, "*

 * *            'shuffle=False,loss_function=self.fun_control["loss_function"], '*

 * *            'metric=self.fun_control["metric_torch"],)\']}, 62: {\'source\': '*

 * *            "['evaluate_hold_out(model_spot, train_dataset = testset, "*

 * *            'shuffle=False,loss_function=self.fun_control["loss_function"], '*

 * *            'metric=self.fun_control["metric_torch"],)\']}, 65: {\'source\': '*

 * *            "['evaluate_hold_out(ne […]*

```diff
@@ -809,24 +809,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_hold_out(model_default, train_dataset = testset, shuffle=False)"
+                "evaluate_hold_out(model_default, train_dataset = testset, shuffle=False,loss_function=self.fun_control[\"loss_function\"], metric=self.fun_control[\"metric_torch\"],)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_hold_out(model_spot, train_dataset = testset, shuffle=False)"
+                "evaluate_hold_out(model_spot, train_dataset = testset, shuffle=False,loss_function=self.fun_control[\"loss_function\"], metric=self.fun_control[\"metric_torch\"],)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -846,24 +846,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_hold_out(net=model_default, train_dataset=trainset, shuffle=False, test_dataset=testset)"
+                "evaluate_hold_out(net=model_default, train_dataset=trainset, shuffle=False, test_dataset=testset,loss_function=self.fun_control[\"loss_function\"], metric=self.fun_control[\"metric_torch\"],)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "evaluate_hold_out(net=model_spot, train_dataset=trainset, shuffle=False, test_dataset=testset)"
+                "evaluate_hold_out(net=model_spot, train_dataset=trainset, shuffle=False, test_dataset=testset,loss_function=self.fun_control[\"loss_function\"], metric=self.fun_control[\"metric_torch\"],)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `spotPython-0.1.8/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb` & `spotPython-0.2.0/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/15_spot_hpt_sklearn_regression.ipynb` & `spotPython-0.2.0/notebooks/15_spot_hpt_sklearn_regression.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb` & `spotPython-0.2.0/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.2.0/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures/spotModel.graffle` & `spotPython-0.2.0/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures/spotModel.pdf` & `spotPython-0.2.0/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures/spotModel.png` & `spotPython-0.2.0/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf` & `spotPython-0.2.0/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/notebooks/plot.png` & `spotPython-0.2.0/notebooks/plot.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/pyproject.toml` & `spotPython-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.1.8"
+version = "0.2.0"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.1.8/src/spotPython/budget/ocba.py` & `spotPython-0.2.0/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/build/kriging.py` & `spotPython-0.2.0/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/data/base.py` & `spotPython-0.2.0/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.2.0/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.2.0/src/spotPython/data/torch_hyper_dict.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8787878787878788%*

 * *Differences: {"'Net_CIFAR10'": "{'lr_mult': OrderedDict([('type', 'float'), ('default', 1.0), ('transform', "*

 * *                  "'None'), ('lower', 0.1), ('upper', 10.0)]), 'sgd_momentum': "*

 * *                  "OrderedDict([('type', 'float'), ('default', 0.0), ('transform', 'None'), "*

 * *                  "('lower', 0.0), ('upper', 1.0)]), delete: ['lr', 'loss_function']}",*

 * * "'Net_fashionMNIST'": "{'lr_mult': OrderedDict([('type', 'float'), ('default', 1.0), "*

 * *                       "('transform', 'None'), ('lower', 0.1), ( […]*

```diff
@@ -31,52 +31,20 @@
         "l2": {
             "default": 5,
             "lower": 2,
             "transform": "transform_power_2_int",
             "type": "int",
             "upper": 9
         },
-        "loss_function": {
-            "class_name": "torch.nn",
-            "core_model_parameter_type": "instance()",
-            "default": "CrossEntropyLoss",
-            "levels": [
-                "L1Loss",
-                "MSELoss",
-                "CrossEntropyLoss",
-                "CTCLoss",
-                "NLLLoss",
-                "PoissonNLLLoss",
-                "GaussianNLLLoss",
-                "KLDivLoss",
-                "BCELoss",
-                "BCEWithLogitsLoss",
-                "MarginRankingLoss",
-                "HingeEmbeddingLoss",
-                "MultiLabelMarginLoss",
-                "HuberLoss",
-                "SmoothL1Loss",
-                "SoftMarginLoss",
-                "MultiLabelSoftMarginLoss",
-                "CosineEmbeddingLoss",
-                "MultiMarginLoss",
-                "TripletMarginLoss",
-                "TripletMarginWithDistanceLoss"
-            ],
-            "lower": 0,
-            "transform": "None",
-            "type": "factor",
-            "upper": 20
-        },
-        "lr": {
-            "default": 0.001,
-            "lower": 1e-05,
+        "lr_mult": {
+            "default": 1.0,
+            "lower": 0.1,
             "transform": "None",
             "type": "float",
-            "upper": 0.01
+            "upper": 10.0
         },
         "optimizer": {
             "class_name": "torch.optim",
             "core_model_parameter_type": "str",
             "default": "SGD",
             "levels": [
                 "Adadelta",
@@ -99,14 +67,21 @@
         },
         "patience": {
             "default": 5,
             "lower": 2,
             "transform": "None",
             "type": "int",
             "upper": 10
+        },
+        "sgd_momentum": {
+            "default": 0.0,
+            "lower": 0.0,
+            "transform": "None",
+            "type": "float",
+            "upper": 1.0
         }
     },
     "Net_fashionMNIST": {
         "batch_size": {
             "default": 4,
             "lower": 1,
             "transform": "transform_power_2_int",
@@ -137,51 +112,20 @@
         "l2": {
             "default": 5,
             "lower": 2,
             "transform": "transform_power_2_int",
             "type": "int",
             "upper": 9
         },
-        "loss_function": {
-            "core_model_parameter_type": "str",
-            "default": "CrossEntropyLoss",
-            "levels": [
-                "L1Loss",
-                "MSELoss",
-                "CrossEntropyLoss",
-                "CTCLoss",
-                "NLLLoss",
-                "PoissonNLLLoss",
-                "GaussianNLLLoss",
-                "KLDivLoss",
-                "BCELoss",
-                "BCEWithLogitsLoss",
-                "MarginRankingLoss",
-                "HingeEmbeddingLoss",
-                "MultiLabelMarginLoss",
-                "HuberLoss",
-                "SmoothL1Loss",
-                "SoftMarginLoss",
-                "MultiLabelSoftMarginLoss",
-                "CosineEmbeddingLoss",
-                "MultiMarginLoss",
-                "TripletMarginLoss",
-                "TripletMarginWithDistanceLoss"
-            ],
-            "lower": 0,
-            "transform": "None",
-            "type": "factor",
-            "upper": 20
-        },
-        "lr": {
-            "default": 0.001,
-            "lower": 1e-05,
+        "lr_mult": {
+            "default": 1.0,
+            "lower": 0.1,
             "transform": "None",
             "type": "float",
-            "upper": 0.01
+            "upper": 10.0
         },
         "optimizer": {
             "core_model_parameter_type": "str",
             "default": "SGD",
             "levels": [
                 "Adadelta",
                 "Adagrad",
@@ -203,14 +147,21 @@
         },
         "patience": {
             "default": 5,
             "lower": 2,
             "transform": "None",
             "type": "int",
             "upper": 10
+        },
+        "sgd_momentum": {
+            "default": 0.0,
+            "lower": 0.0,
+            "transform": "None",
+            "type": "float",
+            "upper": 1.0
         }
     },
     "Template": {
         "bool_hyperparameter": {
             "core_model_parameter_type": "bool",
             "default": 0,
             "levels": [
```

### Comparing `spotPython-0.1.8/src/spotPython/design/spacefilling.py` & `spotPython-0.2.0/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/fun/hypersklearn.py` & `spotPython-0.2.0/src/spotPython/fun/hypersklearn.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/fun/hypertorch.py` & `spotPython-0.2.0/src/spotPython/fun/hypertorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,29 +86,31 @@
                         show_batch_interval=self.fun_control["show_batch_interval"],
                     )
                 elif self.fun_control["eval"] == "test_hold_out":
                     df_eval, _ = evaluate_hold_out(
                         model,
                         train_dataset=fun_control["train"],
                         shuffle=self.fun_control["shuffle"],
+                        loss_function=self.fun_control["loss_function"],
+                        metric=self.fun_control["metric_torch"],
                         test_dataset=fun_control["test"],
                         device=self.fun_control["device"],
                         show_batch_interval=self.fun_control["show_batch_interval"],
                         path=self.fun_control["path"],
-                        save_model=self.fun_control["save_model"],
                     )
                 else:  # eval == "train_hold_out"
                     df_eval, _ = evaluate_hold_out(
                         model,
                         train_dataset=fun_control["train"],
                         shuffle=self.fun_control["shuffle"],
+                        loss_function=self.fun_control["loss_function"],
+                        metric=self.fun_control["metric_torch"],
                         device=self.fun_control["device"],
                         show_batch_interval=self.fun_control["show_batch_interval"],
                         path=self.fun_control["path"],
-                        save_model=self.fun_control["save_model"],
                     )
             except Exception as err:
                 print(f"Error in fun_torch(). Call to evaluate_model failed. {err=}, {type(err)=}")
                 print("Setting df_eval to np.nan")
                 df_eval = np.nan
             z_res = np.append(z_res, fun_control["weights"] * df_eval)
         return z_res
```

### Comparing `spotPython-0.1.8/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.2.0/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.2.0/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.2.0/src/spotPython/hyperparameters/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 import torch.optim
 
 
-def optimizer_handler(optimizer_name: str, params, sgd_lr=0.9, **kwargs):
+def optimizer_handler(optimizer_name: str, params, lr_mult=1.0, **kwargs):
     if optimizer_name == "Adadelta":
         return torch.optim.Adadelta(
-            params, lr=1.0, rho=0.9, eps=1e-06, weight_decay=0, foreach=None, maximize=False, differentiable=False
+            params,
+            lr=lr_mult * 1.0,
+            rho=0.9,
+            eps=1e-06,
+            weight_decay=0,
+            foreach=None,
+            maximize=False,
+            differentiable=False,
         )
     elif optimizer_name == "Adagrad":
         return torch.optim.Adagrad(
             params,
-            lr=0.01,
+            lr=lr_mult * 0.01,
             lr_decay=0,
             weight_decay=0,
             initial_accumulator_value=0,
             eps=1e-10,
             foreach=None,
             maximize=False,
             differentiable=False,
         )
     elif optimizer_name == "Adam":
         return torch.optim.Adam(
             params,
-            lr=0.001,
+            lr=lr_mult * 0.001,
             betas=(0.9, 0.999),
             eps=1e-08,
             weight_decay=0,
             amsgrad=False,
             foreach=None,
             maximize=False,
             capturable=False,
             differentiable=False,
             fused=None,
         )
     elif optimizer_name == "AdamW":
         return torch.optim.AdamW(
             params,
-            lr=0.001,
+            lr=lr_mult * 0.001,
             betas=(0.9, 0.999),
             eps=1e-08,
             weight_decay=0.01,
             amsgrad=False,
             foreach=None,
             maximize=False,
             capturable=False,
@@ -47,82 +54,88 @@
             fused=None,
         )
     elif optimizer_name == "SparseAdam":
         return torch.optim.SparseAdam(params, lr=0.001, betas=(0.9, 0.999), eps=1e-08, maximize=False)
     elif optimizer_name == "Adamax":
         return torch.optim.Adamax(
             params,
-            lr=0.002,
+            lr=lr_mult * 0.002,
             betas=(0.9, 0.999),
             eps=1e-08,
             weight_decay=0,
             foreach=None,
             maximize=False,
             differentiable=False,
         )
     elif optimizer_name == "ASGD":
         return torch.optim.ASGD(
             params,
-            lr=0.01,
+            lr=lr_mult * 0.01,
             lambd=0.0001,
             alpha=0.75,
             t0=1000000.0,
             weight_decay=0,
             foreach=None,
             maximize=False,
             differentiable=False,
         )
     elif optimizer_name == "LBFGS":
         return torch.optim.LBFGS(
             params,
-            lr=1,
+            lr=lr_mult * 1,
             max_iter=20,
             max_eval=None,
             tolerance_grad=1e-07,
             tolerance_change=1e-09,
             history_size=100,
             line_search_fn=None,
         )
     elif optimizer_name == "NAdam":
         return torch.optim.NAdam(
             params,
-            lr=0.002,
+            lr=lr_mult * 0.002,
             betas=(0.9, 0.999),
             eps=1e-08,
             weight_decay=0,
             momentum_decay=0.004,
             foreach=None,
             differentiable=False,
         )
     elif optimizer_name == "RAdam":
         return torch.optim.RAdam(
             params, lr=0.001, betas=(0.9, 0.999), eps=1e-08, weight_decay=0, foreach=None, differentiable=False
         )
     elif optimizer_name == "RMSprop":
         return torch.optim.RMSprop(
             params,
-            lr=0.01,
+            lr=lr_mult * 0.01,
             alpha=0.99,
             eps=1e-08,
             weight_decay=0,
             momentum=0,
             centered=False,
             foreach=None,
             maximize=False,
             differentiable=False,
         )
     elif optimizer_name == "Rprop":
         return torch.optim.Rprop(
-            params, lr=0.01, etas=(0.5, 1.2), step_sizes=(1e-06, 50), foreach=None, maximize=False, differentiable=False
+            params,
+            lr=lr_mult * 0.01,
+            etas=(0.5, 1.2),
+            step_sizes=(1e-06, 50),
+            foreach=None,
+            maximize=False,
+            differentiable=False,
         )
     elif optimizer_name == "SGD":
         return torch.optim.SGD(
             params,
-            lr=sgd_lr,
-            momentum=0,
+            lr=lr_mult * 1e-3,
+            momentum=kwargs["sgd_momentum"],
             dampening=0,
             weight_decay=0,
             nesterov=False,
             maximize=False,
             foreach=None,
             differentiable=False,
         )
```

### Comparing `spotPython-0.1.8/src/spotPython/hyperparameters/values.py` & `spotPython-0.2.0/src/spotPython/hyperparameters/values.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/plot/contour.py` & `spotPython-0.2.0/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/plot/validation.py` & `spotPython-0.2.0/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/spot/spot.py` & `spotPython-0.2.0/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/torch/netcifar10.py` & `spotPython-0.2.0/src/spotPython/torch/netcifar10.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from torch import nn
 import torch.nn.functional as F
 import spotPython.torch.netcore as netcore
 
 
 class Net_CIFAR10(netcore.Net_Core):
-    def __init__(self, l1, l2, lr, batch_size, epochs, k_folds, patience, loss_function, optimizer):
+    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):
         super(Net_CIFAR10, self).__init__(
-            lr=lr,
+            lr_mult=lr_mult,
             batch_size=batch_size,
             epochs=epochs,
             k_folds=k_folds,
             patience=patience,
-            loss_function=loss_function,
             optimizer=optimizer,
+            sgd_momentum=sgd_momentum,
         )
         self.conv1 = nn.Conv2d(3, 6, 5)
         self.pool = nn.MaxPool2d(2, 2)
         self.conv2 = nn.Conv2d(6, 16, 5)
         self.fc1 = nn.Linear(16 * 5 * 5, l1)
         self.fc2 = nn.Linear(l1, l2)
         self.fc3 = nn.Linear(l2, 10)
```

### Comparing `spotPython-0.1.8/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.2.0/src/spotPython/torch/netfashionMNIST.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from torch import nn
 import spotPython.torch.netcore as netcore
 
 
 class Net_fashionMNIST(netcore.Net_Core):
-    def __init__(self, l1, l2, lr, batch_size, epochs, k_folds, patience, loss_function, optimizer):
+    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):
         super(Net_fashionMNIST, self).__init__(
-            lr=lr,
+            lr_mult=lr_mult,
             batch_size=batch_size,
             epochs=epochs,
             k_folds=k_folds,
             patience=patience,
-            loss_function=loss_function,
             optimizer=optimizer,
+            sgd_momentum=sgd_momentum,
         )
         self.flatten = nn.Flatten()
         self.linear_relu_stack = nn.Sequential(
             nn.Linear(28 * 28, l1), nn.ReLU(), nn.Linear(l1, l2), nn.ReLU(), nn.Linear(l2, 10)
         )
 
     def forward(self, x):
```

### Comparing `spotPython-0.1.8/src/spotPython/torch/traintest.py` & `spotPython-0.2.0/src/spotPython/torch/traintest.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,63 +56,82 @@
             running_loss += loss.item()
             epoch_steps += 1
             if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches
                 print("Batch: %5d. Training Loss (running): %.3f" % (i + 1, running_loss / epoch_steps))
                 running_loss = 0.0
 
 
-def validate_fold(net, valloader, loss_function, device):
+def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
     val_loss = 0.0
     val_steps = 0
     total = 0
     correct = 0
+    metric.reset()
     for i, data in enumerate(valloader, 0):
         with torch.no_grad():
             inputs, labels = data
             inputs, labels = inputs.to(device), labels.to(device)
             outputs = net(inputs)
+            # print(f"outputs: {outputs}")
+            # print(f"labels: {labels}")
             _, predicted = torch.max(outputs.data, 1)
+            # print(f"predicted: {predicted}")
             total += labels.size(0)
+            # print(f"total: {total}")
             correct += (predicted == labels).sum().item()
+            # print(f"correct: {correct}")
+            #
+            metric_value = metric(predicted, labels).to(device)
+            # print(f"Accuracy on batch {i}: {acc}")
+            #
             loss = loss_function(outputs, labels)
             val_loss += loss.cpu().numpy()
             val_steps += 1
-    # return 100.0 * (correct / total)
     accuracy = correct / total
     loss = val_loss / val_steps
     print(f"Loss on hold-out set: {loss}")
     print(f"Accuracy on hold-out set: {accuracy}")
-    return accuracy, loss
+    # metric on all batches using custom accumulation
+    metric_value = metric.compute()
+    print(f"Metric value on hold-out data: {metric_value}")
+    return metric_value, loss
 
 
 def evaluate_cv(
     net,
     dataset,
     shuffle=False,
     num_workers=0,
     device=None,
     show_batch_interval=10_000,
 ):
-    lr_instance = net.lr
+    lr_mult_instance = net.lr_mult
     epochs_instance = net.epochs
     batch_size_instance = net.batch_size
     k_folds_instance = net.k_folds
     loss_function_instance = net.loss_function
     optimizer_instance = net.optimizer
+    sgd_momentum_instance = net.sgd_momentum
     removed_attributes, net = get_removed_attributes_and_base_net(net)
-    results = {}
+    metric_values = {}
+    loss_values = {}
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
-        optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), sgd_lr=lr_instance)
+        optimizer = optimizer_handler(
+            optimizer_name=optimizer_instance,
+            params=net.parameters(),
+            lr_mult=lr_mult_instance,
+            sgd_momentum=sgd_momentum_instance,
+        )
         loss_function = loss_function_instance
         kfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)
         for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
             print(f"Fold: {fold + 1}")
             train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
             val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
             trainloader = torch.utils.data.DataLoader(
@@ -128,51 +147,61 @@
                 trainloader,
                 epochs_instance,
                 loss_function,
                 optimizer,
                 device,
                 show_batch_interval=show_batch_interval,
             )
-            # Validate fold: use only accuracy for now, loss is not used
-            results[fold], _ = validate_fold(net, valloader, loss_function, device)
-        df_eval = sum(results.values()) / len(results.values())
+            # Validate fold: use only loss for tuning
+            metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)
+        df_eval = sum(loss_values.values()) / len(loss_values.values())
         df_preds = np.nan
     except Exception as err:
         print(f"Error in Net_Core. Call to evaluate_cv() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     add_attributes(net, removed_attributes)
     return df_eval, df_preds
 
 
 def evaluate_hold_out(
-    net, train_dataset, shuffle, test_dataset=None, device=None, show_batch_interval=10_000, path=None, save_model=False
+    net,
+    train_dataset,
+    shuffle,
+    test_dataset=None,
+    loss_function=None,
+    metric=None,
+    device=None,
+    show_batch_interval=10_000,
+    path=None,
 ):
-    lr_instance = net.lr
+    lr_mult_instance = net.lr_mult
     epochs_instance = net.epochs
     batch_size_instance = net.batch_size
-    loss_function_instance = net.loss_function
     optimizer_instance = net.optimizer
     patience_instance = net.patience
+    sgd_momentum_instance = net.sgd_momentum
     removed_attributes, net = get_removed_attributes_and_base_net(net)
-    print(f"Removed attributes: {removed_attributes}")
-    print(f"Optimizer_instatance: {optimizer_instance}")
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
         # loss_function = nn.CrossEntropyLoss()
         # TODO: optimizer = optim.Adam(net.parameters(), lr=lr)
         # optimizer = optim.SGD(net.parameters(), lr=lr, momentum=0.9)
-        optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), sgd_lr=lr_instance)
-        loss_function = loss_function_instance
+        optimizer = optimizer_handler(
+            optimizer_name=optimizer_instance,
+            params=net.parameters(),
+            lr_mult=lr_mult_instance,
+            sgd_momentum=sgd_momentum_instance,
+        )
         if test_dataset is None:
             trainloader, valloader = create_train_val_data_loaders(
                 dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle
             )
         else:
             trainloader, valloader = create_train_test_data_loaders(
                 dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle, test_dataset=test_dataset
@@ -193,23 +222,23 @@
                 loss_function=loss_function,
                 optimizer=optimizer,
                 device=device,
                 show_batch_interval=show_batch_interval,
             )
             # TODO: scheduler.step()
             # Early stopping check. Calculate validation loss from one epoch:
-            val_accuracy, val_loss = validate_hold_out(
-                net, valloader=valloader, loss_function=loss_function, device=device
+            val_accuracy, val_loss = validate_fold_or_hold_out(
+                net, valloader=valloader, loss_function=loss_function, metric=metric, device=device
             )
             if val_loss < best_val_loss:
                 best_val_loss = val_loss
                 counter = 0
                 # save model:
-                if save_model:
-                    torch.save({"model_state_dict": net.state_dict()}, path)
+                if path is not None:
+                    torch.save(net.state_dict(), path)
             else:
                 counter += 1
                 if counter >= patience_instance:
                     print(f"Early stopping at epoch {epoch}")
                     break
         df_eval = val_loss
         df_preds = np.nan
@@ -253,143 +282,65 @@
         inputs, labels = inputs.to(device), labels.to(device)
         optimizer.zero_grad()
         outputs = net(inputs)
         loss = loss_function(outputs, labels)
         loss.backward()
         torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
         optimizer.step()
-        # print statistics
         running_loss += loss.item()
         epoch_steps += 1
         if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches
             print(
                 "Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
                 % (i + 1, int(batch_size), running_loss / epoch_steps)
             )
             running_loss = 0.0
     return loss.item()
 
 
-def validate_hold_out(net, valloader, loss_function, device):
-    val_loss = 0.0
-    val_steps = 0
-    total = 0
-    correct = 0
-    pred_list = []
-    with torch.no_grad():
-        for i, data in enumerate(valloader, 0):
-            inputs, labels = data
-            inputs, labels = inputs.to(device), labels.to(device)
-            outputs = net(inputs)
-            _, predicted = torch.max(outputs.data, 1)
-            pred_list.append(predicted)
-            total += labels.size(0)
-            correct += (predicted == labels).sum().item()
-            loss = loss_function(outputs, labels)
-            val_loss += loss.cpu().numpy()
-            val_steps += 1
-    accuracy = correct / total
-    loss = val_loss / val_steps
-    print(f"Loss on hold-out set: {loss}")
-    print(f"Accuracy on hold-out set: {accuracy}")
-    return accuracy, loss
-
-
-def train_save(net, train_dataset, shuffle, device=None, show_batch_interval=10_000, path=None, save_model=False):
-    lr_instance = net.lr
-    epochs_instance = net.epochs
-    batch_size_instance = net.batch_size
-    loss_function_instance = net.loss_function
-    optimizer_instance = net.optimizer
-    patience_instance = net.patience
-    removed_attributes, net = get_removed_attributes_and_base_net(net)
-    try:
-        device = getDevice(device=device)
-        if torch.cuda.is_available():
-            device = "cuda:0"
-            if torch.cuda.device_count() > 1:
-                print("We will use", torch.cuda.device_count(), "GPUs!")
-                net = nn.DataParallel(net)
-        net.to(device)
-        # loss_function = nn.CrossEntropyLoss()
-        # TODO: optimizer = optim.Adam(net.parameters(), lr=lr)
-        # optimizer = optim.SGD(net.parameters(), lr=lr, momentum=0.9)
-        optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), sgd_lr=lr_instance)
-        loss_function = loss_function_instance
-        trainloader, valloader = create_train_val_data_loaders(
-            dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle
-        )
-        # TODO: scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=30, gamma=0.1)
-        # Early stopping parameters
-        patience = patience_instance
-        best_val_loss = float("inf")
-        counter = 0
-        # We only have "one fold" which is trained for several epochs
-        # (we do not have to reset the weights for each fold):
-        for epoch in range(epochs_instance):
-            print(f"Epoch: {epoch + 1}")
-            # training loss from one epoch:
-            _ = train_hold_out(
-                net=net,
-                trainloader=trainloader,
-                batch_size=batch_size_instance,
-                loss_function=loss_function,
-                optimizer=optimizer,
-                device=device,
-                show_batch_interval=show_batch_interval,
-            )
-            # TODO: scheduler.step()
-            # Early stopping check. Calculate validation loss from one epoch:
-            val_accuracy, val_loss = validate_hold_out(
-                net, valloader=valloader, loss_function=loss_function, device=device
-            )
-            if val_loss < best_val_loss:
-                best_val_loss = val_loss
-                counter = 0
-                # save model:
-                if save_model:
-                    torch.save({"model_state_dict": net.state_dict()}, path)
-            else:
-                counter += 1
-                if counter >= patience:
-                    print(f"Early stopping at epoch {epoch}")
-                    break
-        df_eval = val_loss
-        df_preds = np.nan
-    except Exception as err:
-        print(f"Error in Net_Core. Call to evaluate_hold_out() failed. {err=}, {type(err)=}")
-        df_eval = np.nan
-        df_preds = np.nan
-    add_attributes(net, removed_attributes)
-    print(f"Returned to Spot: Validation loss: {df_eval}")
-    print("----------------------------------------------")
-    return df_eval, df_preds
+def train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_interval=10_000, path=None):
+    evaluate_hold_out(
+        net=net,
+        train_dataset=train_dataset,
+        shuffle=shuffle,
+        test_dataset=None,
+        loss_function=loss_function,
+        metric=metric,
+        device=device,
+        show_batch_interval=show_batch_interval,
+        path=path,
+    )
 
 
-def test_saved(net, shuffle, test_dataset=None, device=None):
+def test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None, path=None):
     batch_size_instance = net.batch_size
-    loss_function_instance = net.loss_function
     removed_attributes, net = get_removed_attributes_and_base_net(net)
+    if path is not None:
+        net.load_state_dict(torch.load(path))
+        net.eval()
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
-        # loss_function = nn.CrossEntropyLoss()
-        loss_function = loss_function_instance
         valloader = torch.utils.data.DataLoader(
             test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0
         )
-        val_accuracy, val_loss = validate_hold_out(net, valloader=valloader, loss_function=loss_function, device=device)
-        df_eval = val_loss
+        metric_value, loss = validate_fold_or_hold_out(
+            net, valloader=valloader, loss_function=loss_function, metric=metric, device=device
+        )
+        df_eval = loss
+        df_metric = metric_value
         df_preds = np.nan
     except Exception as err:
-        print(f"Error in Net_Core. Call to evaluate_hold_out() failed. {err=}, {type(err)=}")
+        print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}")
         df_eval = np.nan
+        df_metric = np.nan
         df_preds = np.nan
     add_attributes(net, removed_attributes)
-    print(f"Returned to Spot: Validation loss: {df_eval}")
+    print(f"Final evaluation: Validation loss: {df_eval}")
+    print(f"Final evaluation: Validation metric: {df_metric}")
     print("----------------------------------------------")
-    return df_eval, df_preds
+    return df_eval, df_preds, df_metric
```

### Comparing `spotPython-0.1.8/src/spotPython/utils/aggregate.py` & `spotPython-0.2.0/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/compare.py` & `spotPython-0.2.0/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/convert.py` & `spotPython-0.2.0/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/device.py` & `spotPython-0.2.0/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/eda.py` & `spotPython-0.2.0/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/init.py` & `spotPython-0.2.0/src/spotPython/utils/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 def fun_control_init():
     """Initialize fun_control dictionary.
     Args:
         None
-        Returns:
-            fun_control (dict): A dictionary containing the information about the core model and the hyperparameters.
-        Example:
-            >>> fun_control_init()
-            {'data': None,
-                'train': None,
-                'test': None,
-                'n_samples': None,
-                'target_column': None,
-                'shuffle': None,
-                'k_folds': None,
-                'device': None}
+    Returns:
+    fun_control (dict): A dictionary containing the information about the core model, loss function, metrics,
+    and the hyperparameters.
+    Example:
+        >>> fun_control = fun_control_init()
+        >>> fun_control
+        {'data': None,
+        'train': None,
+        'test': None,
+        'loss_function': None,
+        'metric_sklearn': None,
+        'metric_river': None,
+        'metric_torch': None,
+        'metric_params': {},
+        'prep_model': None,
+        'n_samples': None,
+        'target_column': None,
+        'shuffle': None,
+        'eval': None,
+        'k_folds': None,
+        'optimizer': None,
+        'device': None,
+        'show_batch_interval': 1000000,
+        'path': None,
+        'save_model': False}
     """
     fun_control = {
-        "criterion": None,
+        "data": None,
+        "train": None,
+        "test": None,
+        "loss_function": None,
         "metric_sklearn": None,
         "metric_river": None,
+        "metric_torch": None,
         "metric_params": {},
         "prep_model": None,
-        "data": None,
-        "train": None,
-        "test": None,
         "n_samples": None,
         "target_column": None,
         "shuffle": None,
         "eval": None,
         "k_folds": None,
         "optimizer": None,
         "device": None,
```

### Comparing `spotPython-0.1.8/src/spotPython/utils/metrics.py` & `spotPython-0.2.0/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/progress.py` & `spotPython-0.2.0/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/repair.py` & `spotPython-0.2.0/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython/utils/transform.py` & `spotPython-0.2.0/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.2.0/src/spotPython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.1.8
+Version: 0.2.0
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.1.8/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.2.0/src/spotPython.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -44,24 +44,15 @@
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
 Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
 docs/bart23e.html
 docs/bart23e.pdf
 docs/index.html
 docs/search.json
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
-docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
 docs/figures/parallel.png
-docs/img/spotLogo.png
 docs/site_libs/bootstrap/bootstrap-icons.css
 docs/site_libs/bootstrap/bootstrap-icons.woff
 docs/site_libs/bootstrap/bootstrap.min.css
 docs/site_libs/bootstrap/bootstrap.min.js
 docs/site_libs/clipboard/clipboard.min.js
 docs/site_libs/quarto-html/anchor.min.js
 docs/site_libs/quarto-html/popper.min.js
@@ -113,14 +104,22 @@
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
 notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
 notebooks/plot.png
 notebooks/data/torch/model_spot_trained.pt
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
 notebooks/figures/spotModel.graffle
 notebooks/figures/spotModel.pdf
 notebooks/figures/spotModel.png
 src/spotPython/_version.py
 src/spotPython.egg-info/PKG-INFO
 src/spotPython.egg-info/SOURCES.txt
 src/spotPython.egg-info/dependency_links.txt
```

### Comparing `spotPython-0.1.8/test/test_aggregate_mean_var.py` & `spotPython-0.2.0/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_build_Psi.py` & `spotPython-0.2.0/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_build_U.py` & `spotPython-0.2.0/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_build_psi_vec.py` & `spotPython-0.2.0/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_evaluate_new_X.py` & `spotPython-0.2.0/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_evaluate_new_solutions.py` & `spotPython-0.2.0/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_extract_from_bounds.py` & `spotPython-0.2.0/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_generate_design.py` & `spotPython-0.2.0/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_infill.py` & `spotPython-0.2.0/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_nat_to_cod.py` & `spotPython-0.2.0/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_nat_to_cod_init.py` & `spotPython-0.2.0/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_ocba.py` & `spotPython-0.2.0/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_repair_non_numeric.py` & `spotPython-0.2.0/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_set_de_bounds.py` & `spotPython-0.2.0/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_show_progress.py` & `spotPython-0.2.0/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_suggest_new_X.py` & `spotPython-0.2.0/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.8/test/test_update_surrogate.py` & `spotPython-0.2.0/test/test_update_surrogate.py`

 * *Files identical despite different names*

