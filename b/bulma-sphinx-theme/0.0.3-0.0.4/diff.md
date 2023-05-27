# Comparing `tmp/bulma_sphinx_theme-0.0.3.tar.gz` & `tmp/bulma_sphinx_theme-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.3.tar", last modified: Sat May 27 02:01:34 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.4.tar", last modified: Sat May 27 11:44:01 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.3.tar` & `bulma_sphinx_theme-0.0.4.tar`

### file list

```diff
@@ -1,173 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:34.738805 bulma_sphinx_theme-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-27 02:01:16.034637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_admonitions--.sass
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/_tippy.sass
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/sphinxext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-27 02:01:16.038637 bulma_sphinx_theme-0.0.3/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:01.808868 bulma_sphinx_theme-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.4/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.3/LICENSE` & `bulma_sphinx_theme-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/README.md` & `bulma_sphinx_theme-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.4/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/_static/logo.svg` & `bulma_sphinx_theme-0.0.4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/conf.py` & `bulma_sphinx_theme-0.0.4/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "myst_parser",
-    "sphinx_tippy",
     "sphinx_inline_tabs",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx_togglebutton",
     "sphinx_subfigure",
     "bulma_sphinx_theme.demo.sphinxext",
 ]
@@ -100,18 +99,7 @@
     "source_directory": "docs/",
     "use_edit_page_button": True,
     "fix_navbar": True,
     "navbar_start": [],
     "navbar_end": ["navbar-nav.html", "header-icons.html"],
     "have_top_navbar": True,
 }
-
-## Sphinx Tippy configuration, see https://sphinx-tippy.readthedocs.io/en/latest/
-# tippy_props = {"interactive": True}
-tippy_tip_selector = (
-    "figure, table, img, p, aside, div.admonition, div.literal-block-wrapper, div.math"
-)
-tippy_anchor_parent_selector = "article.article-container"
-
-tippy_enable_wikitips = False
-tippy_enable_doitips = False
-tippy_enable_mathjax = True
```

### Comparing `bulma_sphinx_theme-0.0.3/docs/develop.md` & `bulma_sphinx_theme-0.0.4/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.4/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/docs/web-components.rst` & `bulma_sphinx_theme-0.0.4/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/noxfile.py` & `bulma_sphinx_theme-0.0.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/package-lock.json` & `bulma_sphinx_theme-0.0.4/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/package.json` & `bulma_sphinx_theme-0.0.4/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/pyproject.toml` & `bulma_sphinx_theme-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import os
 import sphinx.application
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
-from ._toctree import add_toctree_functions
-from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
-from .utils import get_theme_options
+from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
@@ -55,29 +53,29 @@
     if "scripts" in context:
         _add_asset_hashes(
             context["scripts"],
             ["scripts/bulma-sphinx-theme.js"],
         )
 
     # determine the startdepth for building the theme
-    theme_options = get_theme_options(app)
+    theme_options = utils.get_theme_options(app)
     start_depth = theme_options.get("have_top_navbar", True)
     if not isinstance(start_depth, bool):
         start_depth = True
     context["start_depth"] = int(start_depth)
 
     # Basic constants
     context["theme_version"] = __version__
     # Translations
     translation = get_translation(MESSAGE_CATALOG_NAME)
     context["translate"] = translation
 
 
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
-    theme_options = get_theme_options(app)
+    theme_options = utils.get_theme_options(app)
 
     if not theme_options.get("have_top_navbar"):
         theme_options["fix_navbar"] = False
 
     # Add an analytics ID to the site if provided
     analytics = theme_options.get("analytics", {})
     if analytics:
@@ -111,14 +109,15 @@
         "theme_footer",
         "theme_article_top_left",
         "theme_article_top_right",
         "theme_article_bottom_left",
         "theme_article_bottom_right",
         "theme_navbar_start",
         "theme_navbar_end",
+        "theme_navbar_include_directly",
         "theme_information_panel",
         "sidebars",
     ]
 
     for section in template_sections:
         if context.get(section):
             # Break apart `,` separated strings so we can use , in the defaults
@@ -135,24 +134,25 @@
 
 def setup(app: sphinx.application.Sphinx) -> Dict[str, Any]:
     """Entry point for sphinx theming."""
     app.require_sphinx("3.0")
 
     theme_dir = _get_html_theme_path()
     app.add_html_theme("bulma_sphinx_theme", theme_dir)
-    app.add_post_transform(ShortenLinkTransform)
-    app.add_post_transform(WrapTableAndMathInAContainerTransform)
+    app.add_post_transform(transforms.ShortenLinkTransform)
+    app.add_post_transform(transforms.WrapTableAndMathInAContainerTransform)
     # Translations
     locale_dir = os.path.join(theme_dir, "static", "locales")
     app.add_message_catalog(MESSAGE_CATALOG_NAME, locale_dir)
 
     app.connect("html-page-context", _html_page_context)
     app.connect("html-page-context", update_and_remove_templates)
-    app.connect("html-page-context", add_toctree_functions)
+    app.connect("html-page-context", toctree.add_toctree_functions)
     app.connect("builder-inited", _builder_inited)
+    app.connect("build-finished", pygment.overwrite_pygments_css)
     app.config.templates_path.append(str(theme_dir / "components"))
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
         "version": __version__,
     }
```

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_toctree.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_transforms.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/_translations.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 // the icons for theme change
 .theme-switch-button {
   // overide bootstrap settings
   padding: 0; // We pad the `span` not the container
-  color: var(--color-foreground-muted);
+  color: var(--bst-color-text-muted);
   width: fit-content;
   aspect-ratio: 1 / 1;
   background: none;
   border: none;
 
   span {
     display: none;
     padding: 0.5em;
 
     &:hover,
     &:active,
     &:focus {
       text-decoration: none;
-      color: var(--color-brand-primary);
+      color: var(--bst-color-primary);
     }
   }
 }
 
 html[data-mode="auto"] .theme-switch-button span[data-mode="auto"] {
   display: flex;
 }
```

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   border-spacing: 0
   border-collapse: collapse
 
   box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), 0 0 0.0625rem rgba(0, 0, 0, 0.1)
 
   th
     background: var(--bst-color-background-sidenav)
+    color: var(--bst-color-text-base)
 
   td,
   th
     // Space things out properly
     padding: 0 0.25rem
 
     // Get the borders looking just-right.
```

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 .bulma-tocnav {
   width: var(--tocnav-width);
   padding: 0 1rem;
+  word-break: break-all;
 
   .toc-wrapper {
     position: sticky;
     top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
-    overflow: hidden;
+    overflow-y: auto;
+    max-height: calc(
+      100vh - var(--navbar-height) - var(--top-content-to-navbar-gap)
+    );
   }
 
   ul.table-of-contents {
     font-size: var(--toc-font-size);
 
     li {
       border-left: 1px solid var(--bst-color-border);
```

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {#
 This is where user-provided CSS variables get converted into actual values.
 #}
-{% macro declare_icon_links(icon_list) -%}
+{% macro declare_icon_links(icon_list, icon_class="") -%}
 {% if icon_list -%}
 {% for icon_dict in icon_list -%}
-<a href="{{ icon_dict.url }}" target="_blank" title="{{ icon_dict.name }}" class="navbar-item ext-link">
+<a href="{{ icon_dict.url }}" target="_blank" title="{{ icon_dict.name }}" class="{{ icon_class }} ext-link">
     {% if icon_dict.class %}
     <i class="{{ icon_dict.class }}"></i>
     {% elif icon_dict.material_icons %}
     <i class="material-icons">{{ icon_dict.material_icons }}</i>
     {% elif icon_dict.fontawesome %}
     <i class="{{ icon_dict.fontawesome }}"></i>
     {% elif icon_dict.image %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {# This is where user-provided CSS variables get converted into actual values.
-#} {% macro declare_icon_links(icon_list) -%} {% if icon_list -%} {% for
-icon_dict in icon_list -%}
+#} {% macro declare_icon_links(icon_list, icon_class="") -%} {% if icon_list -
+%} {% for icon_dict in icon_list -%}
 {%_if_icon_dict.class_%}__{%_elif_icon_dict.material_icons_%}_{
 {_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_elif
 icon_dict.image_%}_[{{_icon_dict.name_}}]_{%_endif_%}
  {% endfor %} {%- endif %} {%- endmacro %}
```

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.3/webpack.config.js` & `bulma_sphinx_theme-0.0.4/webpack.config.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     Compilation
 } = require("webpack");
 
 // Compile our translation files
 const {
     exec
 } = require("child_process");
-exec("python src/bulma_sphinx_theme/_translations.py");
+exec("python src/bulma_sphinx_theme/translations.py");
 
 const scriptPath = resolve(__dirname, "src/bulma_sphinx_theme/assets/scripts");
 const stylePath = resolve(__dirname, "src/bulma_sphinx_theme/assets/styles");
 const staticPath = resolve(__dirname, "src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static");
 const vendorPath = resolve(staticPath, "vendor");
 
 /*******************************************************************************
```

### Comparing `bulma_sphinx_theme-0.0.3/PKG-INFO` & `bulma_sphinx_theme-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.3
+Version: 0.0.4
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.3 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.4 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

