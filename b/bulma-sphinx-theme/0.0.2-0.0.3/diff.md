# Comparing `tmp/bulma_sphinx_theme-0.0.2.tar.gz` & `tmp/bulma_sphinx_theme-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.2.tar", last modified: Thu May 25 08:29:01 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.3.tar", last modified: Sat May 27 02:01:34 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.2.tar` & `bulma_sphinx_theme-0.0.3.tar`

### file list

```diff
@@ -1,167 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:29:01.740501 bulma_sphinx_theme-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/_static/logo-.png
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_sidenav-panel.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/sphinxext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:34.738805 bulma_sphinx_theme-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_admonitions--.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/_tippy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/sphinxext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.3/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.2/LICENSE` & `bulma_sphinx_theme-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/README.md` & `bulma_sphinx_theme-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.3/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/conf.py` & `bulma_sphinx_theme-0.0.3/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "myst_parser",
+    "sphinx_tippy",
     "sphinx_inline_tabs",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx_togglebutton",
     "sphinx_subfigure",
     "bulma_sphinx_theme.demo.sphinxext",
 ]
@@ -44,28 +45,28 @@
 
 templates_path = ["_templates"]
 html_static_path = ["_static"]
 html_theme = "bulma_sphinx_theme"
 html_title = "A sphinx theme on bulma"
 html_favicon = "_static/favicon.png"
 html_last_updated_fmt = ""
-html_logo = "_static/logo-.png"
+html_logo = "_static/logo.svg"
 html_show_sourcelink = True
 
 todo_include_todos = True
 
 # https://github.com/hung1001/font-awesome-pro-v6
 html_css_files = [
     "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
 ]
 
 html_theme_options = {
     "header_links_before_dropdown": 3,
     "navbar_color_style": "is-white",  # see styles: https://bulma.io/documentation/components/navbar/#colors
-    "logo": {"text": "Bulma Sphinx", "logo": "_static/logo-.png"},
+    "logo": {"text": "Bulma Sphinx Theme", "logo": "_static/logo.svg"},
     "header_icons": [
         {
             "name": "Github",
             "url": "https://github.com/zclab/bulma-sphinx-theme",
             "image": "https://www.svgrepo.com/show/433505/github-o.svg",
         },
         {
@@ -97,8 +98,20 @@
     "source_repository": "https://github.com/zclab/bulma-sphinx-theme",
     "source_branch": "main",
     "source_directory": "docs/",
     "use_edit_page_button": True,
     "fix_navbar": True,
     "navbar_start": [],
     "navbar_end": ["navbar-nav.html", "header-icons.html"],
+    "have_top_navbar": True,
 }
+
+## Sphinx Tippy configuration, see https://sphinx-tippy.readthedocs.io/en/latest/
+# tippy_props = {"interactive": True}
+tippy_tip_selector = (
+    "figure, table, img, p, aside, div.admonition, div.literal-block-wrapper, div.math"
+)
+tippy_anchor_parent_selector = "article.article-container"
+
+tippy_enable_wikitips = False
+tippy_enable_doitips = False
+tippy_enable_mathjax = True
```

### Comparing `bulma_sphinx_theme-0.0.2/docs/develop.md` & `bulma_sphinx_theme-0.0.3/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.3/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/docs/web-components.rst` & `bulma_sphinx_theme-0.0.3/docs/web-components.rst`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
    To use the :code:`sphinx-panels` extention, add these lines to your custom CSS to overwrite the shadows of the panels:
 
    .. code-block:: css
 
        /* overwrite panels shadows using pydata-sphinx-theme variable */
        .shadow {
-           box-shadow: 0 0.5rem 1rem var(--pst-color-shadow) !important;
+           box-shadow: 0 0.5rem 1rem var(--bst-color-shadow) !important;
        }
 
    This modification is not needed when using the :code:`sphinx-design` extention.
 
 Below you can find some examples of the components created with the :code:`sphinx-design` extension.
 
 .. _badges-buttons:
```

### Comparing `bulma_sphinx_theme-0.0.2/noxfile.py` & `bulma_sphinx_theme-0.0.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/package-lock.json` & `bulma_sphinx_theme-0.0.3/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/package.json` & `bulma_sphinx_theme-0.0.3/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/pyproject.toml` & `bulma_sphinx_theme-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from ._toctree import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
 from .utils import get_theme_options
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
@@ -54,32 +54,34 @@
         )
     if "scripts" in context:
         _add_asset_hashes(
             context["scripts"],
             ["scripts/bulma-sphinx-theme.js"],
         )
 
+    # determine the startdepth for building the theme
+    theme_options = get_theme_options(app)
+    start_depth = theme_options.get("have_top_navbar", True)
+    if not isinstance(start_depth, bool):
+        start_depth = True
+    context["start_depth"] = int(start_depth)
+
     # Basic constants
     context["theme_version"] = __version__
     # Translations
     translation = get_translation(MESSAGE_CATALOG_NAME)
     context["translate"] = translation
 
 
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
-    def _update_default(key: str, *, new_default: Any) -> None:
-        app.config.values[key] = (new_default, *app.config.values[key][1:])
-
-    # Change the default permalinks icon
-    _update_default("html_permalinks_icon", new_default="#")
-
-
-def _update_config(app: sphinx.application.Sphinx) -> None:
     theme_options = get_theme_options(app)
 
+    if not theme_options.get("have_top_navbar"):
+        theme_options["fix_navbar"] = False
+
     # Add an analytics ID to the site if provided
     analytics = theme_options.get("analytics", {})
     if analytics:
         # Google Analytics
         gid = analytics.get("google_analytics_id")
 
         if gid:
@@ -91,26 +93,33 @@
                 gtag('config', '{gid}');
             """
 
             # Link the JS files
             app.add_js_file(gid_js_path, loading_method="async")
             app.add_js_file(None, body=gid_script)
 
+    def _update_default(key: str, *, new_default: Any) -> None:
+        app.config.values[key] = (new_default, *app.config.values[key][1:])
+
+    # Change the default permalinks icon
+    _update_default("html_permalinks_icon", new_default="#")
+
 
 def update_and_remove_templates(
     app: sphinx.application.Sphinx, pagename: str, templatename: str, context, doctree
 ) -> None:
     template_sections = [
         "theme_footer",
         "theme_article_top_left",
         "theme_article_top_right",
         "theme_article_bottom_left",
         "theme_article_bottom_right",
         "theme_navbar_start",
         "theme_navbar_end",
+        "theme_information_panel",
         "sidebars",
     ]
 
     for section in template_sections:
         if context.get(section):
             # Break apart `,` separated strings so we can use , in the defaults
             if isinstance(context.get(section), str):
@@ -136,15 +145,14 @@
     locale_dir = os.path.join(theme_dir, "static", "locales")
     app.add_message_catalog(MESSAGE_CATALOG_NAME, locale_dir)
 
     app.connect("html-page-context", _html_page_context)
     app.connect("html-page-context", update_and_remove_templates)
     app.connect("html-page-context", add_toctree_functions)
     app.connect("builder-inited", _builder_inited)
-    app.connect("builder-inited", _update_config)
     app.config.templates_path.append(str(theme_dir / "components"))
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
         "version": __version__,
     }
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_toctree.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_transforms.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_translations.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,78 @@
 import Gumshoe from "./gumshoe-patched.js";
 
 var tocScroll = null;
 var header = null;
 var lastScrollTop = window.pageYOffset || document.documentElement.scrollTop;
 const GO_TO_TOP_OFFSET = 64;
+var prefersDark = window.matchMedia("(prefers-color-scheme: dark)");
+
+/*******************************************************************************
+ * Theme switcher
+ */
+
+function autoTheme(e) {
+    document.documentElement.dataset.theme = prefersDark.matches ?
+        "dark" :
+        "light";
+}
+
+function setTheme(mode) {
+    if (mode !== "light" && mode !== "dark" && mode !== "auto") {
+        console.error(`Got invalid theme mode: ${mode}. Resetting to auto.`);
+        mode = "auto";
+    }
+
+    // get the theme
+    var colorScheme = prefersDark.matches ? "dark" : "light";
+    document.documentElement.dataset.mode = mode;
+    var theme = mode == "auto" ? colorScheme : mode;
+    document.documentElement.dataset.theme = theme;
+
+    // save mode and theme
+    localStorage.setItem("mode", mode);
+    localStorage.setItem("theme", theme);
+    console.log(`[BST]: Changed to ${mode} mode using the ${theme} theme.`);
+
+    // add a listener if set on auto
+    prefersDark.onchange = mode == "auto" ? autoTheme : "";
+}
+
+function cycleMode() {
+    const defaultMode = document.documentElement.dataset.defaultMode || "auto";
+    const currentMode = localStorage.getItem("mode") || defaultMode;
+
+    var loopArray = (arr, current) => {
+        var nextPosition = arr.indexOf(current) + 1;
+        if (nextPosition === arr.length) {
+            nextPosition = 0;
+        }
+        return arr[nextPosition];
+    };
+
+    // make sure the next theme after auto is always a change
+    var modeList = prefersDark.matches ?
+        ["auto", "light", "dark"] :
+        ["auto", "dark", "light"];
+    var newMode = loopArray(modeList, currentMode);
+    setTheme(newMode);
+}
+
+function addModeListener() {
+    // the theme was set a first time using the initial mini-script
+    // running setMode will ensure the use of the dark mode if auto is selected
+    setTheme(document.documentElement.dataset.mode);
+
+    // Attach event handlers for toggling themes colors
+    document.querySelectorAll(".theme-switch-button").forEach((el) => {
+        el.addEventListener("click", cycleMode);
+    });
+}
+
+////////////////////////////////////////////////////////////////////////////////
 
 function scrollHandlerForHeader() {
     if (Math.floor(header.getBoundingClientRect().top) == 0) {
         header.classList.add("scrolled");
     } else {
         header.classList.remove("scrolled");
     }
@@ -115,15 +180,15 @@
         recursive: true,
         navClass: "scroll-current",
         nested: true,
         nestedClass: "scroll-current", //
         events: true,
         offset: () => {
             let rem = parseFloat(getComputedStyle(document.documentElement).fontSize);
-            return header.getBoundingClientRect().height + 0.5 * rem + 1;
+            return header.getBoundingClientRect().height + 1.0 * rem + 1;
         },
     });
 }
 
 function setup() {
     setupScrollHandler();
     addTOCInteractivity();
@@ -279,14 +344,15 @@
  */
 
 ////////////////////////////////////////////////////////////////////////////////
 // Main entrypoint
 ////////////////////////////////////////////////////////////////////////////////
 function main() {
     document.body.parentNode.classList.remove("no-js");
+    addModeListener();
     setupSearchButtons();
     setupDropdwon();
     header = document.querySelector(".navbar");
     tocScroll = document.querySelector(".toc-scroll");
     setup();
 }
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   left: 0;
   // top: 1rem;
   padding: 0.5rem;
   padding-right: 0.75rem;
   border-radius: 1.2rem;
   font-size: 1rem;
 
-  background: var(--color-background-primary);
+  background: var(--bst-color-background);
   box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), #6b728080 0px 0px 1px 0px;
 
   z-index: 10;
 
   margin-left: 50%;
   transform: translateX(-50%);
 
@@ -33,15 +33,15 @@
   .show-back-to-top & {
     display: flex;
     align-items: center;
   }
 }
 
 a.back-to-top {
-  color: var(--font-color-main);
+  color: var(--bst-color-text-base);
 
   &:hover {
     text-decoration: none;
-    background: var(--color-brand-primary);
+    background: var(--bst-color-primary);
     color: white;
   }
 }
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files 26% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 
   .pre-next__link__label::after {
     content: " »";
   }
 }
 
 .pre-next__link {
-  border: 1px solid var(--color-background-border);
+  border: 1px solid var(--bst-color-border);
   border-radius: 0.5rem;
   display: block;
   height: 100%;
   line-height: 1.25;
   padding: 1rem;
   transition: border-color 200ms cubic-bezier(0.08, 0.52, 0.52, 1);
 
   &:hover {
-    border-color: var(--color-brand-primary);
+    border-color: var(--bst-color-primary);
     text-decoration: none;
   }
 }
 
 .pre-next__link--prev {
   .pre-next__link__label:before {
     content: "« ";
   }
 }
 
 .pre-next__link__sublabel {
-  color: var(--color-foreground-secondary);
+  color: var(--bst-color-text-muted);
   font-weight: 600;
 }
 
 .pre-next__link__label {
   word-break: break-word;
 }
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_admonitions.sass` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_admonitions--.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 // Abbreviations
 abbr[title]
   cursor: help
 
 // "Problematic" content, as identified by Sphinx
 .problematic
-  color: var(--color-problematic)
+  color: var(--bst-color-danger)
 
 // Keyboard / Mouse "instructions"
 kbd:not(.compound)
   margin: 0 0.2rem
   padding: 0 0.2rem
   border-radius: 0.2rem
-  border: 1px solid var(--color-background-border)
-  color: var(--color-foreground-primary)
+  border: 1px solid var(--bst-color-border)
+  color: var(--bst-color-text-base)
   vertical-align: text-bottom
 
   font-size: var(--font-size--small--3)
   display: inline-block
 
-  box-shadow: 0 0.0625rem 0 rgba(0, 0, 0, 0.2), inset 0 0 0 0.125rem var(--color-background-primary)
+  box-shadow: 0 0.0625rem 0 rgba(0, 0, 0, 0.2), inset 0 0 0 0.125rem var(--bst-color-background)
 
-  background-color: var(--color-background-secondary)
+  background-color: var(--bst-color-surface)
 
 // Blockquote
 blockquote
-  border-left: 4px solid var(--color-background-border)
-  background: var(--color-background-secondary)
+  border-left: 4px solid var(--bst-color-border)
+  background: var(--bst-color-surface)
 
   margin-left: 0
   margin-right: 0
   padding: 0.5rem 1rem
 
   .attribution
     font-weight: 600
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files 14% similar despite different names*

```diff
@@ -12,25 +12,25 @@
   border-radius: 0.2rem
   border-spacing: 0
   border-collapse: collapse
 
   box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), 0 0 0.0625rem rgba(0, 0, 0, 0.1)
 
   th
-    background: var(--color-table-header-background)
+    background: var(--bst-color-background-sidenav)
 
   td,
   th
     // Space things out properly
     padding: 0 0.25rem
 
     // Get the borders looking just-right.
-    border-left: 1px solid var(--color-table-border)
-    border-right: 1px solid var(--color-table-border)
-    border-bottom: 1px solid var(--color-table-border)
+    border-left: 1px solid var(--bst-color-border)
+    border-right: 1px solid var(--bst-color-border)
+    border-bottom: 1px solid var(--bst-color-border)
 
     p
       margin: 0.25rem
 
     &:first-child
       border-left: none
     &:last-child
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files 12% similar despite different names*

```diff
@@ -38,42 +38,42 @@
   h1,
   h2,
   h3,
   h4,
   h5,
   h6
     &:nth-of-type(1)
-      background-color: var(--color-highlight-on-target)
+      background-color: var(--bst-color-target)
       // .headerlink
       //   visibility: visible
       code.literal
         background-color: transparent
 
 table:target > caption,
 figure:target
-  background-color: var(--color-highlight-on-target)
+  background-color: var(--bst-color-target)
 
 // Inline page contents
 .this-will-duplicate-information-and-it-is-still-useful-here li :target
-  background-color: var(--color-highlight-on-target)
+  background-color: var(--bst-color-target)
 
 // Code block permalinks
 .literal-block-wrapper:target .code-block-caption
-  background-color: var(--color-highlight-on-target)
+  background-color: var(--bst-color-target)
 
 // When a definition list item is selected
 //
 //   There isn't really an alternative to !important here, due to the
 //   high-specificity of API documentation's selector.
 dt:target
-  background-color: var(--color-highlight-on-target) !important
+  background-color: var(--bst-color-target) !important
 
 // When a footnote reference is selected
 .footnote > dt:target + dd,
 .footnote-reference:target
-  background-color: var(--color-highlight-on-target)
+  background-color: var(--bst-color-target)
 
 aside.footnote:target
-  background-color: var(--color-highlight-on-target)
+  background-color: var(--bst-color-target)
 
 div.citation:target
-  background-color: var(--color-highlight-on-target)
+  background-color: var(--bst-color-target)
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     overflow: hidden;
   }
 
   ul.table-of-contents {
     font-size: var(--toc-font-size);
 
     li {
-      border-left: 1px solid var(--color-background-border);
+      border-left: 1px solid var(--bst-color-border);
 
       a {
         display: inline-block;
-        color: var(--color-toc-title-text);
+        color: var(--bst-color-text-base);
         padding-left: 16px;
         height: 1.6rem;
         line-height: 1.5rem;
       }
 
       &.scroll-current > .reference {
         border-left: 1px solid $link;
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-// Fonts used by this theme.
-//
-// There are basically two things here -- using the system font stack and
-// defining sizes for various elements in %ages. We could have also used `em`
-// but %age is easier to reason about for me.
-
-@mixin fonts {
+html {
   --font-stack: BlinkMacSystemFont, -apple-system, Segoe UI, Roboto, Oxygen,
     Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, Helvetica, Arial,
     sans-serif;
   --font-stack--monospace: monospace;
 
   --font-size--normal: 100%;
   --font-size--small: 90%;
@@ -33,8 +27,11 @@
   --admonition-title-font-size: 1em;
 
   // Code
   --code-font-size: var(--font-size--small);
 
   // API
   --api-font-size: var(--font-size--small);
+
+  // Admonition styles
+  --bst-admonition-font-weight-heading: 600;
 }
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files 2% similar despite different names*

```diff
@@ -28,7 +28,11 @@
 );
 
 @mixin icons {
   @each $name, $glyph in $icons {
     --icon-#{$name}: #{$glyph};
   }
 }
+
+html {
+  @include icons;
+}
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     <title>{{ docstitle|striptags|e }}</title>
     {% else %}
     <title>{{ title|striptags|e }} - {{ docstitle|striptags|e }}</title>
     {% endif %}
     {%- endblock htmltitle -%}
 
     {%- block styles -%}
+    <script data-cfasync="false">
+        document.documentElement.dataset.mode = localStorage.getItem("mode") || "{{ default_mode }}";
+        document.documentElement.dataset.theme = localStorage.getItem("theme") || "light";
+    </script>
+
     {# Custom stylesheets #}
     {%- block regular_styles -%}
     {%- for css in css_files -%}
     {% if css|attr("filename") -%}
     {{ css_tag(css) }}
     {%- else -%}
     <link rel="stylesheet" href="{{ pathto(css, 1)|e }}" type="text/css" />
```

#### html2text {}

```diff
@@ -17,17 +17,17 @@
  {%- endif %} {%- if prev %}
  {%- endif %} {#- rel="canonical" (set by html_baseurl) -#} {%- if pageurl %}
  {%- endif %} {%- endblock linktags %} {# Favicon #} {%- if favicon_url -%}
  {%- endif -%} {%- endblock site_meta -%} {#- Site title -#} {%- block
 htmltitle -%} {% if not docstitle %}
 {% elif pagename == master_doc %}
 {% else %}
-{% endif %} {%- endblock htmltitle -%} {%- block styles -%} {# Custom
-stylesheets #} {%- block regular_styles -%} {%- for css in css_files -%} {% if
-css|attr("filename") -%} {{ css_tag(css) }} {%- else -%}
+{% endif %} {%- endblock htmltitle -%} {%- block styles -%}
+ {# Custom stylesheets #} {%- block regular_styles -%} {%- for css in css_files
+-%} {% if css|attr("filename") -%} {{ css_tag(css) }} {%- else -%}
  {%- endif %} {% endfor -%} {%- endblock regular_styles -%} {#- Theme-related
 stylesheets -#} {%- block theme_styles %} {% include "partials/
 _css_variables_define.html" with context %} {%- endblock theme_styles -%} {%-
 block extra_styles %} {%- endblock extra_styles -%} {{ _webpack.head_js_preload
 () }} {%- endblock styles -%} {#- Custom front matter #} {%- block extrahead -
 %}{%- endblock extrahead -%}
 {% block htmlbody %} {% endblock htmlbody %} {%- block scripts -%} {# Custom JS
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-<div class="sidenav-panel">
-    {% include "components/search-button.html" %}
-
-    <div class="level">
-        <div class="level-left">
-            <div class="select is-small level-item">
-                <select>
-                    <option>Select</option>
-                    <option>With options</option>
-                </select>
-            </div>
-            <a href="#" class="level-item">
-                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-sun" width="44" height="44"
-                    viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round"
-                    stroke-linejoin="round">
-                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                    <path d="M12 12m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0" />
-                    <path
-                        d="M3 12h1m8 -9v1m8 8h1m-9 8v1m-6.4 -15.4l.7 .7m12.1 -.7l-.7 .7m0 11.4l.7 .7m-12.1 -.7l-.7 .7" />
-                </svg>
-            </a>
+<div class="level">
+    <div class="level-left">
+        <div class="select is-small level-item">
+            <select>
+                <option>Select</option>
+                <option>With options</option>
+            </select>
         </div>
+        <a href="#" class="level-item">
+            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-sun" width="44" height="44"
+                viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round"
+                stroke-linejoin="round">
+                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+                <path d="M12 12m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0" />
+                <path d="M3 12h1m8 -9v1m8 8h1m-9 8v1m-6.4 -15.4l.7 .7m12.1 -.7l-.7 .7m0 11.4l.7 .7m-12.1 -.7l-.7 .7" />
+            </svg>
+        </a>
+    </div>
 
-        <div class="level-right">
-            <a href="{%- if theme_source_repository -%} {{ theme_source_repository }} {%- else -%} {{ pathto(root_doc) }} {%- endif -%}"
-                class="level-item">
-                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-github" width="44"
-                    height="44" viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none"
-                    stroke-linecap="round" stroke-linejoin="round">
-                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                    <path
-                        d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5" />
-                </svg>
-            </a>
-        </div>
+    <div class="level-right">
+        <a href="{%- if theme_source_repository -%} {{ theme_source_repository }} {%- else -%} {{ pathto(root_doc) }} {%- endif -%}"
+            class="level-item">
+            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-github" width="44"
+                height="44" viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round"
+                stroke-linejoin="round">
+                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+                <path
+                    d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5" />
+            </svg>
+        </a>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,4 +1,3 @@
-{% include "components/search-button.html" %}
 [One of: Select/With options]
 ____
 ___
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 {% extends "base.html" %}
 
 {%- set sidebar_nav_html = generate_toctree_html(
 "sidebar",
+startdepth=start_depth,
 show_nav_level=theme_show_nav_level|int,
 maxdepth=theme_navigation_depth|int,
 collapse=theme_collapse_navigation|tobool,
 includehidden=True,
 titles_only=True)
 -%}
 
-{%- set head_nav_html = generate_header_nav_html(n_links_before_dropdown=theme_header_links_before_dropdown)
--%}
-
 {% block htmlbody -%}
 
 {% block docs_headnav %}
+{% if theme_have_top_navbar %}
 <nav class="navbar has-shadow {% if theme_fix_navbar %} is-fixed-top {% endif %} {% if theme_navbar_color_style %} {{ theme_navbar_color_style }} {% endif %}"
     role="navigation" aria-label="main navigation">
     {% include "sections/headnav.html" %}
 </nav>
+{% endif %}
 {% endblock docs_headnav %}
 
 {%- block mainbody -%}
 <div class="bulma-main">
     <div class="main-wrapper">
         {% if theme_show_back_to_top %}
         {%- include "components/back-to-top.html" -%}
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 stylesheet = styles/bulma-sphinx-theme.css
 pygments_style = tango
 # sidebar-start
 sidebars = sidenav-nav.html
 # sidebar-end
 
 [options]
+have_top_navbar = True
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
 header_links_before_dropdown = 4
 external_links =
 header_icons =
 logo =
@@ -35,7 +36,8 @@
 source_repository =
 source_branch =
 source_directory =
 source_edit_link =
 show_prev_next = True
 css_variables =
 dark_css_variables =
+information_panel = theme-swither.html
```

### Comparing `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/webpack.config.js` & `bulma_sphinx_theme-0.0.3/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.2/PKG-INFO` & `bulma_sphinx_theme-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.2
+Version: 0.0.3
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.2 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.3 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

