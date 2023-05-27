# Comparing `tmp/weewx-5.0.0b2.tar.gz` & `tmp/weewx-5.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weewx-5.0.0b2.tar", max compression
+gzip compressed data, was "weewx-5.0.0b3.tar", max compression
```

## Comparing `weewx-5.0.0b2.tar` & `weewx-5.0.0b3.tar`

### file list

```diff
@@ -1,457 +1,454 @@
--rw-r--r--   0        0        0    32472 2020-04-14 15:37:59.000000 weewx-5.0.0b2/LICENSE.txt
--rw-r--r--   0        0        0     3301 2023-05-21 20:58:20.127973 weewx-5.0.0b2/README.md
--rw-r--r--   0        0        0      230 2022-10-29 23:29:54.801313 weewx-5.0.0b2/bin/schemas/__init__.py
--rw-r--r--   0        0        0     3448 2023-03-10 17:12:41.226442 weewx-5.0.0b2/bin/schemas/wview.py
--rw-r--r--   0        0        0     5953 2023-03-10 17:12:41.226442 weewx-5.0.0b2/bin/schemas/wview_extended.py
--rw-r--r--   0        0        0     2105 2023-03-10 17:12:41.226442 weewx-5.0.0b2/bin/schemas/wview_small.py
--rwxr-xr-x   0        0        0    52419 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/wee_database.py
--rwxr-xr-x   0        0        0    16203 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/wee_debug.py
--rwxr-xr-x   0        0        0     2209 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/wee_device.py
--rwxr-xr-x   0        0        0    38964 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/wee_import.py
--rwxr-xr-x   0        0        0     5652 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/wee_reports.py
--rw-r--r--   0        0        0        0 2023-05-27 12:09:02.284998 weewx-5.0.0b2/bin/wee_resources/__init__.py
--rw-r--r--   0        0        0      306 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/bin/user/__init__.py
--rw-r--r--   0        0        0      324 2023-05-27 12:04:43.775995 weewx-5.0.0b2/bin/wee_resources/bin/user/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      398 2023-05-27 12:04:43.775995 weewx-5.0.0b2/bin/wee_resources/bin/user/__pycache__/extensions.cpython-37.pyc
--rw-r--r--   0        0        0      541 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/bin/user/extensions.py
--rw-r--r--   0        0        0    30946 2023-05-27 12:08:45.405187 weewx-5.0.0b2/bin/wee_resources/docs/404.html
--rw-r--r--   0        0        0     1870 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   113550 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js
--rw-r--r--   0        0        0   954048 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map
--rw-r--r--   0        0        0    17074 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js
--rw-r--r--   0        0        0   210371 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map
--rw-r--r--   0        0        0   113427 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css
--rw-r--r--   0        0        0    38997 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map
--rw-r--r--   0        0        0    12289 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css
--rw-r--r--   0        0        0     3635 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map
--rw-r--r--   0        0        0   192743 2023-05-27 12:08:45.449187 weewx-5.0.0b2/bin/wee_resources/docs/changes/index.html
--rw-r--r--   0        0        0    33623 2023-05-27 12:08:45.453187 weewx-5.0.0b2/bin/wee_resources/docs/copyright/index.html
--rw-r--r--   0        0        0      565 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/css/tocbot-4.12.0.css
--rw-r--r--   0        0        0      565 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/css/tocbot-4.3.1.css
--rw-r--r--   0        0        0    11924 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/css/weewx_ui.css
--rw-r--r--   0        0        0    60659 2023-05-27 12:08:45.517186 weewx-5.0.0b2/bin/wee_resources/docs/custom/appendix/index.html
--rw-r--r--   0        0        0   138803 2023-05-27 12:08:45.553186 weewx-5.0.0b2/bin/wee_resources/docs/custom/cheetah/index.html
--rw-r--r--   0        0        0    71015 2023-05-27 12:08:45.569186 weewx-5.0.0b2/bin/wee_resources/docs/custom/custom_reports/index.html
--rw-r--r--   0        0        0    58081 2023-05-27 12:08:45.577186 weewx-5.0.0b2/bin/wee_resources/docs/custom/database/index.html
--rw-r--r--   0        0        0    32622 2023-05-27 12:08:45.577186 weewx-5.0.0b2/bin/wee_resources/docs/custom/derived/index.html
--rw-r--r--   0        0        0    47003 2023-05-27 12:08:45.581186 weewx-5.0.0b2/bin/wee_resources/docs/custom/drivers/index.html
--rw-r--r--   0        0        0    38281 2023-05-27 12:08:45.585186 weewx-5.0.0b2/bin/wee_resources/docs/custom/extensions/index.html
--rw-r--r--   0        0        0    59542 2023-05-27 12:08:45.597185 weewx-5.0.0b2/bin/wee_resources/docs/custom/image_generator/index.html
--rw-r--r--   0        0        0    68886 2023-05-27 12:08:45.505186 weewx-5.0.0b2/bin/wee_resources/docs/custom/index.html
--rw-r--r--   0        0        0    62835 2023-05-27 12:08:45.609185 weewx-5.0.0b2/bin/wee_resources/docs/custom/localization/index.html
--rw-r--r--   0        0        0    45787 2023-05-27 12:08:45.617185 weewx-5.0.0b2/bin/wee_resources/docs/custom/multiple_bindings/index.html
--rw-r--r--   0        0        0   117586 2023-05-27 12:08:45.637185 weewx-5.0.0b2/bin/wee_resources/docs/custom/options_ref/index.html
--rw-r--r--   0        0        0    81357 2023-05-27 12:08:45.661185 weewx-5.0.0b2/bin/wee_resources/docs/custom/service_engine/index.html
--rw-r--r--   0        0        0    43656 2023-05-27 12:08:45.669185 weewx-5.0.0b2/bin/wee_resources/docs/custom/units/index.html
--rw-r--r--   0        0        0    73263 2023-05-27 12:08:45.465187 weewx-5.0.0b2/bin/wee_resources/docs/devnotes/index.html
--rw-r--r--   0        0        0     2747 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/examples/tag.htm
--rw-r--r--   0        0        0   182366 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/hardware.htm
--rw-r--r--   0        0        0    54196 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/antialias.gif
--rw-r--r--   0        0        0     3145 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/day-gap-not-shown.png
--rw-r--r--   0        0        0     3269 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/day-gap-showing.png
--rw-r--r--   0        0        0     7579 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/daycompare.png
--rw-r--r--   0        0        0     8705 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/daytemp_with_avg.png
--rw-r--r--   0        0        0     7803 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/dayvaporp.png
--rw-r--r--   0        0        0     7663 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/daywindvec.png
--rw-r--r--   0        0        0     1026 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/favicon.png
--rw-r--r--   0        0        0    38406 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/ferrites.jpg
--rw-r--r--   0        0        0     3638 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/funky_degree.png
--rw-r--r--   0        0        0    19123 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/image_parts.png
--rw-r--r--   0        0        0    86388 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/image_parts.xcf
--rw-r--r--   0        0        0     2136 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-apple.png
--rw-r--r--   0        0        0     4734 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-centos.png
--rw-r--r--   0        0        0    14541 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-debian.png
--rw-r--r--   0        0        0    24662 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-fedora.png
--rw-r--r--   0        0        0    12046 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-linux.png
--rw-r--r--   0        0        0    27245 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-mint.png
--rw-r--r--   0        0        0    15980 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-opensuse.png
--rw-r--r--   0        0        0    14374 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-pypi.svg
--rw-r--r--   0        0        0     1192 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-redhat.png
--rw-r--r--   0        0        0     3926 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-rpi.png
--rw-r--r--   0        0        0     7877 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-suse.png
--rw-r--r--   0        0        0    13954 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-ubuntu.png
--rw-r--r--   0        0        0    12208 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/logo-weewx.png
--rw-r--r--   0        0        0    35496 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/pipeline.png
--rw-r--r--   0        0        0     6709 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/sample_monthrain.png
--rw-r--r--   0        0        0    10107 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/sample_monthtempdew.png
--rw-r--r--   0        0        0    10649 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/weekgustoverlay.png
--rw-r--r--   0        0        0     8468 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/weektempdew.png
--rw-r--r--   0        0        0     6602 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/yeardiff.png
--rw-r--r--   0        0        0     7286 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/images/yearhilow.png
--rw-r--r--   0        0        0    35469 2023-05-27 12:08:45.425187 weewx-5.0.0b2/bin/wee_resources/docs/index.html
--rw-r--r--   0        0        0    32611 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/js/cash.js
--rw-r--r--   0        0        0    14828 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/js/cash.min.js
--rw-r--r--   0        0        0    11422 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/js/tocbot-4.12.0.js
--rw-r--r--   0        0        0    11422 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
--rw-r--r--   0        0        0     8892 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
--rw-r--r--   0        0        0     4640 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/js/weewx.js
--rw-r--r--   0        0        0    40090 2023-05-27 12:08:45.673185 weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/debian/index.html
--rw-r--r--   0        0        0    32984 2023-05-27 12:08:45.669185 weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/index.html
--rw-r--r--   0        0        0    53212 2023-05-27 12:08:45.685185 weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/pip/index.html
--rw-r--r--   0        0        0    39647 2023-05-27 12:08:45.689185 weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/redhat/index.html
--rw-r--r--   0        0        0    38980 2023-05-27 12:08:45.693184 weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/suse/index.html
--rw-r--r--   0        0        0    44882 2023-05-27 12:08:45.697184 weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html
--rw-r--r--   0        0        0    45914 2023-05-27 12:08:45.469187 weewx-5.0.0b2/bin/wee_resources/docs/report_scheduling/index.html
--rw-r--r--   0        0        0   646057 2023-05-27 12:08:45.833183 weewx-5.0.0b2/bin/wee_resources/docs/search/search_index.json
--rw-r--r--   0        0        0     9306 2023-05-27 12:08:45.313188 weewx-5.0.0b2/bin/wee_resources/docs/sitemap.xml
--rw-r--r--   0        0        0      636 2023-05-27 12:08:45.313188 weewx-5.0.0b2/bin/wee_resources/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    93063 2023-05-27 12:08:45.489187 weewx-5.0.0b2/bin/wee_resources/docs/sle/index.html
--rw-r--r--   0        0        0    35894 2023-05-27 12:08:45.493187 weewx-5.0.0b2/bin/wee_resources/docs/support/index.html
--rw-r--r--   0        0        0   101774 2023-05-27 12:08:45.305189 weewx-5.0.0b2/bin/wee_resources/docs/upgrading.htm
--rw-r--r--   0        0        0    34894 2023-05-27 12:08:45.705184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
--rw-r--r--   0        0        0    32661 2023-05-27 12:08:45.701184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/index.html
--rw-r--r--   0        0        0    38318 2023-05-27 12:08:45.705184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/installing-weewx/index.html
--rw-r--r--   0        0        0    37113 2023-05-27 12:08:45.713184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
--rw-r--r--   0        0        0    36130 2023-05-27 12:08:45.713184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/running-weewx/index.html
--rw-r--r--   0        0        0    36138 2023-05-27 12:08:45.717184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/system-requirements/index.html
--rw-r--r--   0        0        0    76783 2023-05-27 12:08:45.729184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html
--rw-r--r--   0        0        0    39572 2023-05-27 12:08:45.733184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/webserver-integration/index.html
--rw-r--r--   0        0        0    36611 2023-05-27 12:08:45.745184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
--rw-r--r--   0        0        0    36118 2023-05-27 12:08:45.749184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
--rw-r--r--   0        0        0    39542 2023-05-27 12:08:45.753184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
--rw-r--r--   0        0        0    40171 2023-05-27 12:08:45.757184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
--rw-r--r--   0        0        0    37139 2023-05-27 12:08:45.757184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
--rw-r--r--   0        0        0    35456 2023-05-27 12:08:45.741184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
--rw-r--r--   0        0        0    81553 2023-05-27 12:08:45.773184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
--rw-r--r--   0        0        0    37944 2023-05-27 12:08:45.773184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
--rw-r--r--   0        0        0    34481 2023-05-27 12:08:45.777184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
--rw-r--r--   0        0        0    35066 2023-05-27 12:08:45.781184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
--rw-r--r--   0        0        0    35274 2023-05-27 12:08:45.781184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
--rw-r--r--   0        0        0    57882 2023-05-27 12:08:45.789183 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
--rw-r--r--   0        0        0    67928 2023-05-27 12:08:45.797183 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
--rw-r--r--   0        0        0    33455 2023-05-27 12:08:45.801183 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
--rw-r--r--   0        0        0    54544 2023-05-27 12:08:45.809183 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
--rw-r--r--   0        0        0    40424 2023-05-27 12:08:45.741184 weewx-5.0.0b2/bin/wee_resources/docs/usersguide/where/index.html
--rw-r--r--   0        0        0    34364 2023-05-27 12:08:45.813183 weewx-5.0.0b2/bin/wee_resources/docs/utilities/index.html
--rw-r--r--   0        0        0   238749 2023-05-27 12:08:45.309188 weewx-5.0.0b2/bin/wee_resources/docs/utilities/utilities.htm
--rw-r--r--   0        0        0    55581 2023-05-27 12:08:45.825183 weewx-5.0.0b2/bin/wee_resources/docs/weectl/extension/index.html
--rw-r--r--   0        0        0    34019 2023-05-27 12:08:45.813183 weewx-5.0.0b2/bin/wee_resources/docs/weectl/index.html
--rw-r--r--   0        0        0    59933 2023-05-27 12:08:45.833183 weewx-5.0.0b2/bin/wee_resources/docs/weectl/station/index.html
--rw-r--r--   0        0        0     2503 2023-04-13 14:30:10.606500 weewx-5.0.0b2/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc
--rw-r--r--   0        0        0     3135 2023-03-14 22:33:02.247096 weewx-5.0.0b2/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc
--rw-r--r--   0        0        0     3097 2023-03-13 19:28:02.920821 weewx-5.0.0b2/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
--rw-r--r--   0        0        0    10729 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/alarm.py
--rw-r--r--   0        0        0      179 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/basic/changelog
--rw-r--r--   0        0        0     1563 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/basic/install.py
--rw-r--r--   0        0        0     1243 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/basic/readme.md
--rw-r--r--   0        0        0     1510 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/basic.css
--rw-r--r--   0        0        0     6451 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/current.inc
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/favicon.ico
--rw-r--r--   0        0        0    11292 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/hilo.inc
--rw-r--r--   0        0        0     1665 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
--rw-r--r--   0        0        0     2216 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
--rw-r--r--   0        0        0     2408 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
--rw-r--r--   0        0        0     3173 2023-03-13 13:33:49.291977 weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/skin.conf
--rw-r--r--   0        0        0     1965 2023-04-13 14:30:10.534500 weewx-5.0.0b2/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
--rw-r--r--   0        0        0     2140 2023-04-13 14:30:10.562500 weewx-5.0.0b2/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
--rw-r--r--   0        0        0     3175 2023-04-13 14:30:10.562500 weewx-5.0.0b2/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
--rw-r--r--   0        0        0     2128 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/colorize/colorize_1.py
--rw-r--r--   0        0        0     2617 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/colorize/colorize_2.py
--rw-r--r--   0        0        0     4001 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/colorize/colorize_3.py
--rw-r--r--   0        0        0     4180 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
--rw-r--r--   0        0        0      269 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/fileparse/changelog
--rw-r--r--   0        0        0      835 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/fileparse/install.py
--rw-r--r--   0        0        0     2086 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/fileparse/readme.md
--rw-r--r--   0        0        0    10792 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/lowBattery.py
--rw-r--r--   0        0        0     1108 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/examples/mem.py
--rw-r--r--   0        0        0     5986 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/pmon/bin/user/pmon.py
--rw-r--r--   0        0        0      341 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/pmon/changelog
--rw-r--r--   0        0        0     1511 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/pmon/install.py
--rw-r--r--   0        0        0     2628 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/pmon/readme.md
--rw-r--r--   0        0        0      507 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
--rw-r--r--   0        0        0     1234 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
--rw-r--r--   0        0        0     4334 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/tests/test_vaporpressure.py
--rw-r--r--   0        0        0     4285 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/examples/vaporpressure.py
--rw-r--r--   0        0        0     3034 2023-05-27 12:04:35.723779 weewx-5.0.0b2/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc
--rw-r--r--   0        0        0     5662 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/xstats/bin/user/xstats.py
--rw-r--r--   0        0        0      146 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/xstats/changelog
--rw-r--r--   0        0        0      850 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/xstats/install.py
--rw-r--r--   0        0        0     2923 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/xstats/readme.txt
--rw-r--r--   0        0        0     2138 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
--rw-r--r--   0        0        0      591 2023-05-21 20:58:20.143972 weewx-5.0.0b2/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
--rw-r--r--   0        0        0      676 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Ftp/skin.conf
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/favicon.ico
--rw-r--r--   0        0        0     2573 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/index.html.tmpl
--rw-r--r--   0        0        0     1021 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/de.conf
--rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/en.conf
--rw-r--r--   0        0        0     1101 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/nl.conf
--rw-r--r--   0        0        0     2940 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/no.conf
--rw-r--r--   0        0        0      671 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/mobile.css
--rw-r--r--   0        0        0     5171 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Mobile/skin.conf
--rw-r--r--   0        0        0      760 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Rsync/skin.conf
--rw-r--r--   0        0        0     2667 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5460 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     1482 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/about.inc
--rw-r--r--   0        0        0      674 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/analytics.inc
--rw-r--r--   0        0        0     1137 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/celestial.html.tmpl
--rw-r--r--   0        0        0     6214 2023-05-27 01:44:03.524449 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/celestial.inc
--rw-r--r--   0        0        0     1291 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/current.inc
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/favicon.ico
--rw-r--r--   0        0        0   172876 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
--rw-r--r--   0        0        0   169744 2023-03-13 13:33:49.295977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
--rw-r--r--   0        0        0     4383 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OFL.txt
--rw-r--r--   0        0        0   224592 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
--rw-r--r--   0        0        0   217360 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    20248 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans.woff
--rw-r--r--   0        0        0    10352 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
--rw-r--r--   0        0        0     4348 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/license.txt
--rw-r--r--   0        0        0     4360 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/hilo.inc
--rw-r--r--   0        0        0      858 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/identifier.inc
--rw-r--r--   0        0        0     2787 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/index.html.tmpl
--rw-r--r--   0        0        0     9216 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/cn.conf
--rw-r--r--   0        0        0     9844 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/cz.conf
--rw-r--r--   0        0        0     9745 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/de.conf
--rw-r--r--   0        0        0     9459 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/en.conf
--rw-r--r--   0        0        0    10702 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/es.conf
--rw-r--r--   0        0        0    10673 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/fr.conf
--rw-r--r--   0        0        0    11838 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/gr.conf
--rw-r--r--   0        0        0     9947 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/it.conf
--rw-r--r--   0        0        0     9548 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/nl.conf
--rw-r--r--   0        0        0    10705 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/no.conf
--rw-r--r--   0        0        0    15356 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/th.conf
--rw-r--r--   0        0        0      920 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/map.inc
--rw-r--r--   0        0        0      572 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/radar.inc
--rw-r--r--   0        0        0     4373 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/rss.xml.tmpl
--rw-r--r--   0        0        0      642 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/satellite.inc
--rw-r--r--   0        0        0     5406 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/seasons.css
--rw-r--r--   0        0        0     6404 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/seasons.js
--rw-r--r--   0        0        0     3947 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/sensors.inc
--rw-r--r--   0        0        0    27402 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/skin.conf
--rw-r--r--   0        0        0     1294 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/statistics.html.tmpl
--rw-r--r--   0        0        0     3971 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/statistics.inc
--rw-r--r--   0        0        0     2771 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/sunmoon.inc
--rw-r--r--   0        0        0      987 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/tabular.html.tmpl
--rw-r--r--   0        0        0     2450 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
--rw-r--r--   0        0        0     1115 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Seasons/titlebar.inc
--rw-r--r--   0        0        0     1804 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/custom.js
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/favicon.ico
--rw-r--r--   0        0        0     1043 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     2457 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1639 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/de.conf
--rw-r--r--   0        0        0     1554 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/en.conf
--rw-r--r--   0        0        0     1594 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/nl.conf
--rw-r--r--   0        0        0     3530 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/no.conf
--rw-r--r--   0        0        0     1502 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     7806 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/skin.conf
--rw-r--r--   0        0        0     1588 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/temp.html.tmpl
--rw-r--r--   0        0        0     1681 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/wind.html.tmpl
--rw-r--r--   0        0        0     2591 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5364 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     8546 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
--rw-r--r--   0        0        0       76 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/band.gif
--rw-r--r--   0        0        0     2593 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
--rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/drops.gif
--rw-r--r--   0        0        0     1386 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
--rw-r--r--   0        0        0     2277 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
--rw-r--r--   0        0        0     8609 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/night.gif
--rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/favicon.ico
--rw-r--r--   0        0        0   313856 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
--rw-r--r--   0        0        0    20739 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/index.html.tmpl
--rw-r--r--   0        0        0     9390 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/de.conf
--rw-r--r--   0        0        0     9264 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/en.conf
--rw-r--r--   0        0        0     9765 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/fr.conf
--rw-r--r--   0        0        0     9356 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/nl.conf
--rw-r--r--   0        0        0    10875 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/no.conf
--rw-r--r--   0        0        0    15140 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/month.html.tmpl
--rw-r--r--   0        0        0    16429 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/skins/Standard/skin.conf
--rw-r--r--   0        0        0     1456 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/custom.js
--rw-r--r--   0        0        0     1012 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     1918 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
--rw-r--r--   0        0        0     1394 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     1441 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
--rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
--rw-r--r--   0        0        0    15057 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/week.html.tmpl
--rw-r--r--   0        0        0     3533 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/weewx.css
--rw-r--r--   0        0        0     9990 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/skins/Standard/year.html.tmpl
--rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-05-21 20:58:20.147972 weewx-5.0.0b2/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0b2/bin/wee_resources/util/systemd/weewx.service
--rw-r--r--   0        0        0    18354 2023-05-27 11:55:14.432172 weewx-5.0.0b2/bin/wee_resources/weewx.conf
--rw-r--r--   0        0        0    25898 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weecfg/__init__.py
--rw-r--r--   0        0        0    26461 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weecfg/database.py
--rw-r--r--   0        0        0    24020 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weecfg/extension.py
--rw-r--r--   0        0        0    33749 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weecfg/station_config.py
--rw-r--r--   0        0        0    45364 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weecfg/update_config.py
--rwxr-xr-x   0        0        0     1455 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weectl.py
--rw-r--r--   0        0        0      139 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weectllib/__init__.py
--rw-r--r--   0        0        0     6429 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weectllib/parse_extension.py
--rw-r--r--   0        0        0    17231 2023-05-21 20:58:20.127973 weewx-5.0.0b2/bin/weectllib/parse_station.py
--rw-r--r--   0        0        0     4538 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weedb/NOTES.md
--rw-r--r--   0        0        0     6717 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weedb/__init__.py
--rw-r--r--   0        0        0    11213 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weedb/mysql.py
--rw-r--r--   0        0        0    11161 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weedb/sqlite.py
--rw-r--r--   0        0        0      255 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeimport/__init__.py
--rw-r--r--   0        0        0    11110 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeimport/csvimport.py
--rw-r--r--   0        0        0    20265 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeimport/cumulusimport.py
--rw-r--r--   0        0        0    35701 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeimport/wdimport.py
--rw-r--r--   0        0        0    18225 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeimport/weathercatimport.py
--rw-r--r--   0        0        0    69526 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeimport/weeimport.py
--rw-r--r--   0        0        0    17222 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeimport/wuimport.py
--rw-r--r--   0        0        0      367 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeplot/__init__.py
--rw-r--r--   0        0        0    33267 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeplot/genplot.py
--rw-r--r--   0        0        0    24811 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeplot/utilities.py
--rw-r--r--   0        0        0     1633 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeutil/Moon.py
--rw-r--r--   0        0        0    18296 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeutil/Sun.py
--rw-r--r--   0        0        0      142 2022-10-29 23:29:54.809313 weewx-5.0.0b2/bin/weeutil/__init__.py
--rw-r--r--   0        0        0     9408 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeutil/config.py
--rw-r--r--   0        0        0    12986 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeutil/ftpupload.py
--rw-r--r--   0        0        0     3150 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeutil/log.py
--rw-r--r--   0        0        0     5896 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weeutil/logger.py
--rw-r--r--   0        0        0     6593 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeutil/rsyncupload.py
--rw-r--r--   0        0        0     2224 2023-03-10 17:12:41.230442 weewx-5.0.0b2/bin/weeutil/timediff.py
--rw-r--r--   0        0        0    65551 2023-05-23 12:05:35.670867 weewx-5.0.0b2/bin/weeutil/weeutil.py
--rw-r--r--   0        0        0     5929 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/__init__.py
--rw-r--r--   0        0        0    26063 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/accum.py
--rw-r--r--   0        0        0    25229 2023-05-25 22:38:54.598425 weewx-5.0.0b2/bin/weewx/almanac.py
--rw-r--r--   0        0        0    33390 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/cheetahgenerator.py
--rw-r--r--   0        0        0     3393 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/crc16.py
--rw-r--r--   0        0        0     2888 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/daemon.py
--rw-r--r--   0        0        0    11955 2023-05-25 22:39:39.742132 weewx-5.0.0b2/bin/weewx/defaults.py
--rw-r--r--   0        0        0     5147 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/__init__.py
--rw-r--r--   0        0        0    38987 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/drivers/acurite.py
--rw-r--r--   0        0        0    64005 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/cc3000.py
--rw-r--r--   0        0        0    78592 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/fousb.py
--rw-r--r--   0        0        0    14931 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/drivers/simulator.py
--rw-r--r--   0        0        0    99881 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/drivers/te923.py
--rw-r--r--   0        0        0    15797 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/drivers/ultimeter.py
--rw-r--r--   0        0        0   139705 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/vantage.py
--rw-r--r--   0        0        0    17795 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/drivers/wmr100.py
--rw-r--r--   0        0        0    72747 2023-03-10 17:12:41.238442 weewx-5.0.0b2/bin/weewx/drivers/wmr300.py
--rw-r--r--   0        0        0    29536 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/wmr9x8.py
--rw-r--r--   0        0        0    18843 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/ws1.py
--rw-r--r--   0        0        0    79489 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/drivers/ws23xx.py
--rw-r--r--   0        0        0   173578 2023-03-10 17:12:41.242442 weewx-5.0.0b2/bin/weewx/drivers/ws28xx.py
--rw-r--r--   0        0        0    37475 2023-05-21 20:58:20.131973 weewx-5.0.0b2/bin/weewx/engine.py
--rw-r--r--   0        0        0      276 2023-03-10 17:12:41.242442 weewx-5.0.0b2/bin/weewx/filegenerator.py
--rw-r--r--   0        0        0    18278 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewx/imagegenerator.py
--rw-r--r--   0        0        0    73115 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewx/manager.py
--rw-r--r--   0        0        0     3187 2023-03-10 17:12:41.242442 weewx-5.0.0b2/bin/weewx/qc.py
--rw-r--r--   0        0        0    37780 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewx/reportengine.py
--rw-r--r--   0        0        0    79107 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewx/restx.py
--rw-r--r--   0        0        0     7207 2023-03-10 17:12:41.242442 weewx-5.0.0b2/bin/weewx/station.py
--rw-r--r--   0        0        0    31690 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewx/tags.py
--rw-r--r--   0        0        0    71594 2023-05-25 13:51:36.184172 weewx-5.0.0b2/bin/weewx/units.py
--rw-r--r--   0        0        0    25248 2023-03-10 17:12:41.246442 weewx-5.0.0b2/bin/weewx/uwxutils.py
--rw-r--r--   0        0        0      246 2023-03-10 17:12:41.246442 weewx-5.0.0b2/bin/weewx/wxengine.py
--rw-r--r--   0        0        0    30034 2023-03-10 17:12:41.246442 weewx-5.0.0b2/bin/weewx/wxformulas.py
--rw-r--r--   0        0        0      367 2023-03-10 17:12:41.246442 weewx-5.0.0b2/bin/weewx/wxmanager.py
--rw-r--r--   0        0        0     7270 2023-03-10 17:12:41.246442 weewx-5.0.0b2/bin/weewx/wxservices.py
--rw-r--r--   0        0        0    34292 2023-03-10 17:12:41.246442 weewx-5.0.0b2/bin/weewx/wxxtypes.py
--rw-r--r--   0        0        0    55988 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewx/xtypes.py
--rwxr-xr-x   0        0        0     9681 2023-05-21 20:58:20.135973 weewx-5.0.0b2/bin/weewxd.py
--rw-r--r--   0        0        0    12175 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/changelog.el
--rw-r--r--   0        0        0    12070 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/changelog.suse
--rw-r--r--   0        0        0     2731 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/debian/README
--rw-r--r--   0        0        0    21315 2023-05-27 12:08:16.857448 weewx-5.0.0b2/pkg/debian/changelog
--rw-r--r--   0        0        0        3 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/debian/compat
--rw-r--r--   0        0        0       36 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/debian/conffiles
--rwxr-xr-x   0        0        0     3398 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/debian/config
--rw-r--r--   0        0        0      724 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/debian/control
--rw-r--r--   0        0        0      926 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/debian/copyright
--rwxr-xr-x   0        0        0     8937 2023-05-21 20:58:20.143972 weewx-5.0.0b2/pkg/debian/postinst
--rwxr-xr-x   0        0        0      906 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/debian/postrm
--rwxr-xr-x   0        0        0      410 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/debian/preinst
--rwxr-xr-x   0        0        0      693 2023-05-21 20:58:20.147972 weewx-5.0.0b2/pkg/debian/prerm
--rwxr-xr-x   0        0        0     2985 2023-05-27 11:52:09.345505 weewx-5.0.0b2/pkg/debian/rules
--rw-r--r--   0        0        0       12 2020-03-05 01:18:46.000000 weewx-5.0.0b2/pkg/debian/source/format
--rw-r--r--   0        0        0     5501 2023-05-21 20:58:20.147972 weewx-5.0.0b2/pkg/debian/templates
--rw-r--r--   0        0        0     1708 2023-05-21 20:58:20.147972 weewx-5.0.0b2/pkg/index-apt.html
--rw-r--r--   0        0        0     1728 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/index-suse.html
--rw-r--r--   0        0        0     1714 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/index-yum.html
--rwxr-xr-x   0        0        0     9874 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/mkchangelog.pl
--rw-r--r--   0        0        0       79 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/weewx-el8.repo
--rw-r--r--   0        0        0       57 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/weewx-python2.list
--rw-r--r--   0        0        0       56 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/weewx-python3.list
--rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/weewx-suse12.repo
--rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/weewx-suse15.repo
--rw-r--r--   0        0        0     2201 2023-03-10 17:12:41.258442 weewx-5.0.0b2/pkg/weewx.smf
--rw-r--r--   0        0        0     7144 2023-05-27 12:03:01.691948 weewx-5.0.0b2/pkg/weewx.spec.in
--rw-r--r--   0        0        0     2844 2023-05-27 12:06:51.409693 weewx-5.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      154 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/apache/conf-available/weewx.conf
--rw-r--r--   0        0        0      167 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/apache/conf.d/weewx.conf
--rw-r--r--   0        0        0      136 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/default/weewx
--rwxr-xr-x   0        0        0     8897 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/i18n/i18n-report
--rw-r--r--   0        0        0     9052 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/import/csv-example.conf
--rw-r--r--   0        0        0     8250 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/import/cumulus-example.conf
--rw-r--r--   0        0        0    14923 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/import/wd-example.conf
--rw-r--r--   0        0        0     7100 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/import/weathercat-example.conf
--rw-r--r--   0        0        0     6202 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/import/wu-example.conf
--rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0b2/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0     1800 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/logrotate.d/weewx
--rw-r--r--   0        0        0       83 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/logwatch/conf/logfiles/weewx.conf
--rw-r--r--   0        0        0       32 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/logwatch/conf/services/weewx.conf
--rwxr-xr-x   0        0        0    54942 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/logwatch/scripts/services/weewx
--rw-r--r--   0        0        0       82 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/newsyslog.d/weewx.conf
--rw-r--r--   0        0        0     2219 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/rsyslog.d/weewx.conf
--rwxr-xr-x   0        0        0      319 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/wee_database
--rwxr-xr-x   0        0        0      316 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/wee_debug
--rwxr-xr-x   0        0        0      317 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/wee_device
--rwxr-xr-x   0        0        0      317 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/wee_import
--rwxr-xr-x   0        0        0      318 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/wee_reports
--rwxr-xr-x   0        0        0      313 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/weectl
--rwxr-xr-x   0        0        0      313 2023-05-21 20:58:20.147972 weewx-5.0.0b2/util/scripts/weewxd
--rw-r--r--   0        0        0     2564 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/solaris/weewx-smf.xml
--rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0b2/util/systemd/weewx.service
--rw-r--r--   0        0        0       34 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/tmpfiles.d/weewx.conf
--rw-r--r--   0        0        0      149 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/udev/rules.d/acurite.rules
--rw-r--r--   0        0        0      135 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/udev/rules.d/cc3000.rules
--rw-r--r--   0        0        0      153 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/udev/rules.d/fousb.rules
--rw-r--r--   0        0        0      147 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/udev/rules.d/te923.rules
--rw-r--r--   0        0        0      624 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/udev/rules.d/vantage.rules
--rw-r--r--   0        0        0     1560 2023-03-10 17:12:41.266442 weewx-5.0.0b2/util/udev/rules.d/weewx.rules
--rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/udev/rules.d/wmr100.rules
--rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/udev/rules.d/wmr300.rules
--rw-r--r--   0        0        0      152 2020-04-14 15:38:00.000000 weewx-5.0.0b2/util/udev/rules.d/ws28xx.rules
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 weewx-5.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0    32472 2020-04-14 15:37:59.000000 weewx-5.0.0b3/LICENSE.txt
+-rw-r--r--   0        0        0     3301 2023-05-21 20:58:20.127973 weewx-5.0.0b3/README.md
+-rw-r--r--   0        0        0      230 2022-10-29 23:29:54.801313 weewx-5.0.0b3/bin/schemas/__init__.py
+-rw-r--r--   0        0        0     3448 2023-03-10 17:12:41.226442 weewx-5.0.0b3/bin/schemas/wview.py
+-rw-r--r--   0        0        0     5953 2023-03-10 17:12:41.226442 weewx-5.0.0b3/bin/schemas/wview_extended.py
+-rw-r--r--   0        0        0     2105 2023-03-10 17:12:41.226442 weewx-5.0.0b3/bin/schemas/wview_small.py
+-rwxr-xr-x   0        0        0    52419 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/wee_database.py
+-rwxr-xr-x   0        0        0    16203 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/wee_debug.py
+-rwxr-xr-x   0        0        0     2209 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/wee_device.py
+-rwxr-xr-x   0        0        0    38964 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/wee_import.py
+-rwxr-xr-x   0        0        0     5652 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/wee_reports.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:04:34.117140 weewx-5.0.0b3/bin/wee_resources/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/bin/user/__init__.py
+-rw-r--r--   0        0        0      541 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/bin/user/extensions.py
+-rw-r--r--   0        0        0    30946 2023-05-27 15:04:07.829326 weewx-5.0.0b3/bin/wee_resources/docs/404.html
+-rw-r--r--   0        0        0     1870 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113550 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js
+-rw-r--r--   0        0        0   954048 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map
+-rw-r--r--   0        0        0    17074 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     7973 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     1031 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2062 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js
+-rw-r--r--   0        0        0   210371 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map
+-rw-r--r--   0        0        0   113427 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css
+-rw-r--r--   0        0        0    38997 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map
+-rw-r--r--   0        0        0    12289 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css
+-rw-r--r--   0        0        0     3635 2023-05-27 15:04:07.733327 weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map
+-rw-r--r--   0        0        0   192743 2023-05-27 15:04:07.873326 weewx-5.0.0b3/bin/wee_resources/docs/changes/index.html
+-rw-r--r--   0        0        0    33623 2023-05-27 15:04:07.877326 weewx-5.0.0b3/bin/wee_resources/docs/copyright/index.html
+-rw-r--r--   0        0        0      565 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/css/tocbot-4.12.0.css
+-rw-r--r--   0        0        0      565 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/css/tocbot-4.3.1.css
+-rw-r--r--   0        0        0    11924 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/css/weewx_ui.css
+-rw-r--r--   0        0        0    60659 2023-05-27 15:04:07.941326 weewx-5.0.0b3/bin/wee_resources/docs/custom/appendix/index.html
+-rw-r--r--   0        0        0   138803 2023-05-27 15:04:07.981325 weewx-5.0.0b3/bin/wee_resources/docs/custom/cheetah/index.html
+-rw-r--r--   0        0        0    71015 2023-05-27 15:04:07.993325 weewx-5.0.0b3/bin/wee_resources/docs/custom/custom_reports/index.html
+-rw-r--r--   0        0        0    58081 2023-05-27 15:04:08.005325 weewx-5.0.0b3/bin/wee_resources/docs/custom/database/index.html
+-rw-r--r--   0        0        0    32622 2023-05-27 15:04:08.005325 weewx-5.0.0b3/bin/wee_resources/docs/custom/derived/index.html
+-rw-r--r--   0        0        0    47003 2023-05-27 15:04:08.009325 weewx-5.0.0b3/bin/wee_resources/docs/custom/drivers/index.html
+-rw-r--r--   0        0        0    38281 2023-05-27 15:04:08.013325 weewx-5.0.0b3/bin/wee_resources/docs/custom/extensions/index.html
+-rw-r--r--   0        0        0    59542 2023-05-27 15:04:08.025325 weewx-5.0.0b3/bin/wee_resources/docs/custom/image_generator/index.html
+-rw-r--r--   0        0        0    68886 2023-05-27 15:04:07.929326 weewx-5.0.0b3/bin/wee_resources/docs/custom/index.html
+-rw-r--r--   0        0        0    62835 2023-05-27 15:04:08.037325 weewx-5.0.0b3/bin/wee_resources/docs/custom/localization/index.html
+-rw-r--r--   0        0        0    45787 2023-05-27 15:04:08.045325 weewx-5.0.0b3/bin/wee_resources/docs/custom/multiple_bindings/index.html
+-rw-r--r--   0        0        0   117586 2023-05-27 15:04:08.065325 weewx-5.0.0b3/bin/wee_resources/docs/custom/options_ref/index.html
+-rw-r--r--   0        0        0    81357 2023-05-27 15:04:08.093325 weewx-5.0.0b3/bin/wee_resources/docs/custom/service_engine/index.html
+-rw-r--r--   0        0        0    43656 2023-05-27 15:04:08.097324 weewx-5.0.0b3/bin/wee_resources/docs/custom/units/index.html
+-rw-r--r--   0        0        0    73263 2023-05-27 15:04:07.885326 weewx-5.0.0b3/bin/wee_resources/docs/devnotes/index.html
+-rw-r--r--   0        0        0     2747 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/examples/tag.htm
+-rw-r--r--   0        0        0   182366 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/hardware.htm
+-rw-r--r--   0        0        0    54196 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/images/antialias.gif
+-rw-r--r--   0        0        0     3145 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/images/day-gap-not-shown.png
+-rw-r--r--   0        0        0     3269 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/images/day-gap-showing.png
+-rw-r--r--   0        0        0     7579 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/images/daycompare.png
+-rw-r--r--   0        0        0     8705 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/images/daytemp_with_avg.png
+-rw-r--r--   0        0        0     7803 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/images/dayvaporp.png
+-rw-r--r--   0        0        0     7663 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/daywindvec.png
+-rw-r--r--   0        0        0     1026 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/favicon.png
+-rw-r--r--   0        0        0    38406 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/ferrites.jpg
+-rw-r--r--   0        0        0     3638 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/funky_degree.png
+-rw-r--r--   0        0        0    19123 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/image_parts.png
+-rw-r--r--   0        0        0    86388 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/image_parts.xcf
+-rw-r--r--   0        0        0     2136 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-apple.png
+-rw-r--r--   0        0        0     4734 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-centos.png
+-rw-r--r--   0        0        0    14541 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-debian.png
+-rw-r--r--   0        0        0    24662 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-fedora.png
+-rw-r--r--   0        0        0    12046 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-linux.png
+-rw-r--r--   0        0        0    27245 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-mint.png
+-rw-r--r--   0        0        0    15980 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-opensuse.png
+-rw-r--r--   0        0        0    14374 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-pypi.svg
+-rw-r--r--   0        0        0     1192 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-redhat.png
+-rw-r--r--   0        0        0     3926 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-rpi.png
+-rw-r--r--   0        0        0     7877 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-suse.png
+-rw-r--r--   0        0        0    13954 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-ubuntu.png
+-rw-r--r--   0        0        0    12208 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/logo-weewx.png
+-rw-r--r--   0        0        0    35496 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/pipeline.png
+-rw-r--r--   0        0        0     6709 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/sample_monthrain.png
+-rw-r--r--   0        0        0    10107 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/sample_monthtempdew.png
+-rw-r--r--   0        0        0    10649 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/weekgustoverlay.png
+-rw-r--r--   0        0        0     8468 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/weektempdew.png
+-rw-r--r--   0        0        0     6602 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/yeardiff.png
+-rw-r--r--   0        0        0     7286 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/images/yearhilow.png
+-rw-r--r--   0        0        0    35469 2023-05-27 15:04:07.845326 weewx-5.0.0b3/bin/wee_resources/docs/index.html
+-rw-r--r--   0        0        0    32611 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/js/cash.js
+-rw-r--r--   0        0        0    14828 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/js/cash.min.js
+-rw-r--r--   0        0        0    11422 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/js/tocbot-4.12.0.js
+-rw-r--r--   0        0        0    11422 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
+-rw-r--r--   0        0        0     8892 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
+-rw-r--r--   0        0        0     4640 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/js/weewx.js
+-rw-r--r--   0        0        0    40090 2023-05-27 15:04:08.105324 weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/debian/index.html
+-rw-r--r--   0        0        0    32984 2023-05-27 15:04:08.101324 weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/index.html
+-rw-r--r--   0        0        0    53212 2023-05-27 15:04:08.113324 weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/pip/index.html
+-rw-r--r--   0        0        0    39647 2023-05-27 15:04:08.117324 weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/redhat/index.html
+-rw-r--r--   0        0        0    38980 2023-05-27 15:04:08.121324 weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/suse/index.html
+-rw-r--r--   0        0        0    44882 2023-05-27 15:04:08.129324 weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html
+-rw-r--r--   0        0        0    45914 2023-05-27 15:04:07.893326 weewx-5.0.0b3/bin/wee_resources/docs/report_scheduling/index.html
+-rw-r--r--   0        0        0   646057 2023-05-27 15:04:08.269323 weewx-5.0.0b3/bin/wee_resources/docs/search/search_index.json
+-rw-r--r--   0        0        0     9306 2023-05-27 15:04:07.737327 weewx-5.0.0b3/bin/wee_resources/docs/sitemap.xml
+-rw-r--r--   0        0        0      636 2023-05-27 15:04:07.737327 weewx-5.0.0b3/bin/wee_resources/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    93063 2023-05-27 15:04:07.913326 weewx-5.0.0b3/bin/wee_resources/docs/sle/index.html
+-rw-r--r--   0        0        0    35894 2023-05-27 15:04:07.917326 weewx-5.0.0b3/bin/wee_resources/docs/support/index.html
+-rw-r--r--   0        0        0   101774 2023-05-27 15:04:07.725327 weewx-5.0.0b3/bin/wee_resources/docs/upgrading.htm
+-rw-r--r--   0        0        0    34894 2023-05-27 15:04:08.133324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
+-rw-r--r--   0        0        0    32661 2023-05-27 15:04:08.133324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/index.html
+-rw-r--r--   0        0        0    38318 2023-05-27 15:04:08.137324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/installing-weewx/index.html
+-rw-r--r--   0        0        0    37113 2023-05-27 15:04:08.141324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
+-rw-r--r--   0        0        0    36130 2023-05-27 15:04:08.145324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/running-weewx/index.html
+-rw-r--r--   0        0        0    36138 2023-05-27 15:04:08.149324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/system-requirements/index.html
+-rw-r--r--   0        0        0    76783 2023-05-27 15:04:08.157324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html
+-rw-r--r--   0        0        0    39572 2023-05-27 15:04:08.165324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/webserver-integration/index.html
+-rw-r--r--   0        0        0    36611 2023-05-27 15:04:08.177324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
+-rw-r--r--   0        0        0    36118 2023-05-27 15:04:08.181324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
+-rw-r--r--   0        0        0    39542 2023-05-27 15:04:08.185324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
+-rw-r--r--   0        0        0    40171 2023-05-27 15:04:08.189324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
+-rw-r--r--   0        0        0    37139 2023-05-27 15:04:08.193324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
+-rw-r--r--   0        0        0    35456 2023-05-27 15:04:08.173324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
+-rw-r--r--   0        0        0    81553 2023-05-27 15:04:08.205324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
+-rw-r--r--   0        0        0    37944 2023-05-27 15:04:08.209324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
+-rw-r--r--   0        0        0    34481 2023-05-27 15:04:08.209324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
+-rw-r--r--   0        0        0    35066 2023-05-27 15:04:08.213324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
+-rw-r--r--   0        0        0    35274 2023-05-27 15:04:08.217324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
+-rw-r--r--   0        0        0    57882 2023-05-27 15:04:08.225324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
+-rw-r--r--   0        0        0    67928 2023-05-27 15:04:08.233323 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
+-rw-r--r--   0        0        0    33455 2023-05-27 15:04:08.233323 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
+-rw-r--r--   0        0        0    54544 2023-05-27 15:04:08.241324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
+-rw-r--r--   0        0        0    40424 2023-05-27 15:04:08.173324 weewx-5.0.0b3/bin/wee_resources/docs/usersguide/where/index.html
+-rw-r--r--   0        0        0    34364 2023-05-27 15:04:08.245324 weewx-5.0.0b3/bin/wee_resources/docs/utilities/index.html
+-rw-r--r--   0        0        0   238749 2023-05-27 15:04:07.729327 weewx-5.0.0b3/bin/wee_resources/docs/utilities/utilities.htm
+-rw-r--r--   0        0        0    55581 2023-05-27 15:04:08.261323 weewx-5.0.0b3/bin/wee_resources/docs/weectl/extension/index.html
+-rw-r--r--   0        0        0    34019 2023-05-27 15:04:08.249323 weewx-5.0.0b3/bin/wee_resources/docs/weectl/index.html
+-rw-r--r--   0        0        0    59933 2023-05-27 15:04:08.265323 weewx-5.0.0b3/bin/wee_resources/docs/weectl/station/index.html
+-rw-r--r--   0        0        0     2503 2023-04-13 14:30:10.606500 weewx-5.0.0b3/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc
+-rw-r--r--   0        0        0     3135 2023-03-14 22:33:02.247096 weewx-5.0.0b3/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc
+-rw-r--r--   0        0        0     3097 2023-03-13 19:28:02.920821 weewx-5.0.0b3/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
+-rw-r--r--   0        0        0    10729 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/alarm.py
+-rw-r--r--   0        0        0      179 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/basic/changelog
+-rw-r--r--   0        0        0     1563 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/basic/install.py
+-rw-r--r--   0        0        0     1243 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/basic/readme.md
+-rw-r--r--   0        0        0     1510 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/basic.css
+-rw-r--r--   0        0        0     6451 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/current.inc
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/favicon.ico
+-rw-r--r--   0        0        0    11292 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/hilo.inc
+-rw-r--r--   0        0        0     1665 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
+-rw-r--r--   0        0        0     2216 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
+-rw-r--r--   0        0        0     2408 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
+-rw-r--r--   0        0        0     3173 2023-03-13 13:33:49.291977 weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/skin.conf
+-rw-r--r--   0        0        0     1965 2023-04-13 14:30:10.534500 weewx-5.0.0b3/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
+-rw-r--r--   0        0        0     2140 2023-04-13 14:30:10.562500 weewx-5.0.0b3/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
+-rw-r--r--   0        0        0     3175 2023-04-13 14:30:10.562500 weewx-5.0.0b3/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
+-rw-r--r--   0        0        0     2128 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/colorize/colorize_1.py
+-rw-r--r--   0        0        0     2617 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/colorize/colorize_2.py
+-rw-r--r--   0        0        0     4001 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/colorize/colorize_3.py
+-rw-r--r--   0        0        0     4180 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
+-rw-r--r--   0        0        0      269 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/fileparse/changelog
+-rw-r--r--   0        0        0      835 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/fileparse/install.py
+-rw-r--r--   0        0        0     2086 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/fileparse/readme.md
+-rw-r--r--   0        0        0    10792 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/lowBattery.py
+-rw-r--r--   0        0        0     1108 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/examples/mem.py
+-rw-r--r--   0        0        0     5986 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/pmon/bin/user/pmon.py
+-rw-r--r--   0        0        0      341 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/pmon/changelog
+-rw-r--r--   0        0        0     1511 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/pmon/install.py
+-rw-r--r--   0        0        0     2628 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/pmon/readme.md
+-rw-r--r--   0        0        0      507 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
+-rw-r--r--   0        0        0     1234 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
+-rw-r--r--   0        0        0     4334 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/tests/test_vaporpressure.py
+-rw-r--r--   0        0        0     4285 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/examples/vaporpressure.py
+-rw-r--r--   0        0        0     5662 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/xstats/bin/user/xstats.py
+-rw-r--r--   0        0        0      146 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/xstats/changelog
+-rw-r--r--   0        0        0      850 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/xstats/install.py
+-rw-r--r--   0        0        0     2923 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/xstats/readme.txt
+-rw-r--r--   0        0        0     2138 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
+-rw-r--r--   0        0        0      591 2023-05-21 20:58:20.143972 weewx-5.0.0b3/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
+-rw-r--r--   0        0        0      676 2023-05-27 15:02:59.629809 weewx-5.0.0b3/bin/wee_resources/skins/Ftp/skin.conf
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/favicon.ico
+-rw-r--r--   0        0        0     2573 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/index.html.tmpl
+-rw-r--r--   0        0        0     1021 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/de.conf
+-rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/en.conf
+-rw-r--r--   0        0        0     1101 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/nl.conf
+-rw-r--r--   0        0        0     2940 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/no.conf
+-rw-r--r--   0        0        0      671 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/mobile.css
+-rw-r--r--   0        0        0     5171 2023-05-27 15:02:59.633809 weewx-5.0.0b3/bin/wee_resources/skins/Mobile/skin.conf
+-rw-r--r--   0        0        0      760 2023-05-27 15:02:59.637809 weewx-5.0.0b3/bin/wee_resources/skins/Rsync/skin.conf
+-rw-r--r--   0        0        0     2667 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5460 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     1482 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/about.inc
+-rw-r--r--   0        0        0      674 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/analytics.inc
+-rw-r--r--   0        0        0     1137 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/celestial.html.tmpl
+-rw-r--r--   0        0        0     6214 2023-05-27 01:44:03.524449 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/celestial.inc
+-rw-r--r--   0        0        0     1291 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/current.inc
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/favicon.ico
+-rw-r--r--   0        0        0   172876 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
+-rw-r--r--   0        0        0   169744 2023-03-13 13:33:49.295977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
+-rw-r--r--   0        0        0     4383 2023-05-21 20:58:20.147972 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OFL.txt
+-rw-r--r--   0        0        0   224592 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   217360 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    20248 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans.woff
+-rw-r--r--   0        0        0    10352 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
+-rw-r--r--   0        0        0     4348 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/license.txt
+-rw-r--r--   0        0        0     4360 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/hilo.inc
+-rw-r--r--   0        0        0      858 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/identifier.inc
+-rw-r--r--   0        0        0     2787 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/index.html.tmpl
+-rw-r--r--   0        0        0     9216 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/cn.conf
+-rw-r--r--   0        0        0     9844 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/cz.conf
+-rw-r--r--   0        0        0     9745 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/de.conf
+-rw-r--r--   0        0        0     9459 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/en.conf
+-rw-r--r--   0        0        0    10702 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/es.conf
+-rw-r--r--   0        0        0    10673 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/fr.conf
+-rw-r--r--   0        0        0    11838 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/gr.conf
+-rw-r--r--   0        0        0     9947 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/it.conf
+-rw-r--r--   0        0        0     9548 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/nl.conf
+-rw-r--r--   0        0        0    10705 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/no.conf
+-rw-r--r--   0        0        0    15356 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/th.conf
+-rw-r--r--   0        0        0      920 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/map.inc
+-rw-r--r--   0        0        0      572 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/radar.inc
+-rw-r--r--   0        0        0     4373 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/rss.xml.tmpl
+-rw-r--r--   0        0        0      642 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/satellite.inc
+-rw-r--r--   0        0        0     5406 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/seasons.css
+-rw-r--r--   0        0        0     6404 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/seasons.js
+-rw-r--r--   0        0        0     3947 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/sensors.inc
+-rw-r--r--   0        0        0    27402 2023-05-27 15:02:59.637809 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/skin.conf
+-rw-r--r--   0        0        0     1294 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/statistics.html.tmpl
+-rw-r--r--   0        0        0     3971 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/statistics.inc
+-rw-r--r--   0        0        0     2771 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/sunmoon.inc
+-rw-r--r--   0        0        0      987 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/tabular.html.tmpl
+-rw-r--r--   0        0        0     2450 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
+-rw-r--r--   0        0        0     1115 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Seasons/titlebar.inc
+-rw-r--r--   0        0        0     1804 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/custom.js
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/favicon.ico
+-rw-r--r--   0        0        0     1043 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     2457 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1639 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/de.conf
+-rw-r--r--   0        0        0     1554 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/en.conf
+-rw-r--r--   0        0        0     1594 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/nl.conf
+-rw-r--r--   0        0        0     3530 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/no.conf
+-rw-r--r--   0        0        0     1502 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     7806 2023-05-27 15:02:59.641809 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/skin.conf
+-rw-r--r--   0        0        0     1588 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/temp.html.tmpl
+-rw-r--r--   0        0        0     1681 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0     2591 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5364 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     8546 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
+-rw-r--r--   0        0        0       76 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/band.gif
+-rw-r--r--   0        0        0     2593 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
+-rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/drops.gif
+-rw-r--r--   0        0        0     1386 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
+-rw-r--r--   0        0        0     2277 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
+-rw-r--r--   0        0        0     8609 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/night.gif
+-rw-r--r--   0        0        0     1150 2023-03-13 13:33:49.299977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/favicon.ico
+-rw-r--r--   0        0        0   313856 2023-05-21 20:58:20.147972 weewx-5.0.0b3/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0        0        0    20739 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/index.html.tmpl
+-rw-r--r--   0        0        0     9390 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/de.conf
+-rw-r--r--   0        0        0     9264 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/en.conf
+-rw-r--r--   0        0        0     9765 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/fr.conf
+-rw-r--r--   0        0        0     9356 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/nl.conf
+-rw-r--r--   0        0        0    10875 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/no.conf
+-rw-r--r--   0        0        0    15140 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/month.html.tmpl
+-rw-r--r--   0        0        0    16429 2023-05-27 15:02:59.645809 weewx-5.0.0b3/bin/wee_resources/skins/Standard/skin.conf
+-rw-r--r--   0        0        0     1456 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/custom.js
+-rw-r--r--   0        0        0     1012 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     1918 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1000 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
+-rw-r--r--   0        0        0     1394 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     1441 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
+-rw-r--r--   0        0        0     1508 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0    15057 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/week.html.tmpl
+-rw-r--r--   0        0        0     3533 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/weewx.css
+-rw-r--r--   0        0        0     9990 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/skins/Standard/year.html.tmpl
+-rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-05-21 20:58:20.147972 weewx-5.0.0b3/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0b3/bin/wee_resources/util/systemd/weewx.service
+-rw-r--r--   0        0        0    18354 2023-05-27 15:02:59.625809 weewx-5.0.0b3/bin/wee_resources/weewx.conf
+-rw-r--r--   0        0        0    25898 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weecfg/__init__.py
+-rw-r--r--   0        0        0    26461 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weecfg/database.py
+-rw-r--r--   0        0        0    24020 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weecfg/extension.py
+-rw-r--r--   0        0        0    33749 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weecfg/station_config.py
+-rw-r--r--   0        0        0    45364 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weecfg/update_config.py
+-rwxr-xr-x   0        0        0     1455 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weectl.py
+-rw-r--r--   0        0        0      139 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weectllib/__init__.py
+-rw-r--r--   0        0        0     6429 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weectllib/parse_extension.py
+-rw-r--r--   0        0        0    17231 2023-05-21 20:58:20.127973 weewx-5.0.0b3/bin/weectllib/parse_station.py
+-rw-r--r--   0        0        0     4538 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weedb/NOTES.md
+-rw-r--r--   0        0        0     6717 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weedb/__init__.py
+-rw-r--r--   0        0        0    11213 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weedb/mysql.py
+-rw-r--r--   0        0        0    11161 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weedb/sqlite.py
+-rw-r--r--   0        0        0      255 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeimport/__init__.py
+-rw-r--r--   0        0        0    11110 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeimport/csvimport.py
+-rw-r--r--   0        0        0    20265 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeimport/cumulusimport.py
+-rw-r--r--   0        0        0    35701 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeimport/wdimport.py
+-rw-r--r--   0        0        0    18225 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeimport/weathercatimport.py
+-rw-r--r--   0        0        0    69526 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeimport/weeimport.py
+-rw-r--r--   0        0        0    17222 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeimport/wuimport.py
+-rw-r--r--   0        0        0      367 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeplot/__init__.py
+-rw-r--r--   0        0        0    33267 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeplot/genplot.py
+-rw-r--r--   0        0        0    24811 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeplot/utilities.py
+-rw-r--r--   0        0        0     1633 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeutil/Moon.py
+-rw-r--r--   0        0        0    18296 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeutil/Sun.py
+-rw-r--r--   0        0        0      142 2022-10-29 23:29:54.809313 weewx-5.0.0b3/bin/weeutil/__init__.py
+-rw-r--r--   0        0        0     9408 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeutil/config.py
+-rw-r--r--   0        0        0    12986 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeutil/ftpupload.py
+-rw-r--r--   0        0        0     3150 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeutil/log.py
+-rw-r--r--   0        0        0     5896 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weeutil/logger.py
+-rw-r--r--   0        0        0     6593 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeutil/rsyncupload.py
+-rw-r--r--   0        0        0     2224 2023-03-10 17:12:41.230442 weewx-5.0.0b3/bin/weeutil/timediff.py
+-rw-r--r--   0        0        0    65551 2023-05-23 12:05:35.670867 weewx-5.0.0b3/bin/weeutil/weeutil.py
+-rw-r--r--   0        0        0     5929 2023-05-27 15:02:59.649809 weewx-5.0.0b3/bin/weewx/__init__.py
+-rw-r--r--   0        0        0    26063 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/accum.py
+-rw-r--r--   0        0        0    25229 2023-05-25 22:38:54.598425 weewx-5.0.0b3/bin/weewx/almanac.py
+-rw-r--r--   0        0        0    33390 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/cheetahgenerator.py
+-rw-r--r--   0        0        0     3393 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/crc16.py
+-rw-r--r--   0        0        0     2888 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/daemon.py
+-rw-r--r--   0        0        0    11955 2023-05-25 22:39:39.742132 weewx-5.0.0b3/bin/weewx/defaults.py
+-rw-r--r--   0        0        0     5147 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/__init__.py
+-rw-r--r--   0        0        0    38987 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/drivers/acurite.py
+-rw-r--r--   0        0        0    64005 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/cc3000.py
+-rw-r--r--   0        0        0    78592 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/fousb.py
+-rw-r--r--   0        0        0    14931 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/drivers/simulator.py
+-rw-r--r--   0        0        0    99881 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/drivers/te923.py
+-rw-r--r--   0        0        0    15797 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/drivers/ultimeter.py
+-rw-r--r--   0        0        0   139705 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/vantage.py
+-rw-r--r--   0        0        0    17795 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/drivers/wmr100.py
+-rw-r--r--   0        0        0    72747 2023-03-10 17:12:41.238442 weewx-5.0.0b3/bin/weewx/drivers/wmr300.py
+-rw-r--r--   0        0        0    29536 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/wmr9x8.py
+-rw-r--r--   0        0        0    18843 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/ws1.py
+-rw-r--r--   0        0        0    79489 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/drivers/ws23xx.py
+-rw-r--r--   0        0        0   173578 2023-03-10 17:12:41.242442 weewx-5.0.0b3/bin/weewx/drivers/ws28xx.py
+-rw-r--r--   0        0        0    37475 2023-05-21 20:58:20.131973 weewx-5.0.0b3/bin/weewx/engine.py
+-rw-r--r--   0        0        0      276 2023-03-10 17:12:41.242442 weewx-5.0.0b3/bin/weewx/filegenerator.py
+-rw-r--r--   0        0        0    18278 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewx/imagegenerator.py
+-rw-r--r--   0        0        0    73115 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewx/manager.py
+-rw-r--r--   0        0        0     3187 2023-03-10 17:12:41.242442 weewx-5.0.0b3/bin/weewx/qc.py
+-rw-r--r--   0        0        0    37780 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewx/reportengine.py
+-rw-r--r--   0        0        0    79107 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewx/restx.py
+-rw-r--r--   0        0        0     7207 2023-03-10 17:12:41.242442 weewx-5.0.0b3/bin/weewx/station.py
+-rw-r--r--   0        0        0    31690 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewx/tags.py
+-rw-r--r--   0        0        0    71594 2023-05-25 13:51:36.184172 weewx-5.0.0b3/bin/weewx/units.py
+-rw-r--r--   0        0        0    25248 2023-03-10 17:12:41.246442 weewx-5.0.0b3/bin/weewx/uwxutils.py
+-rw-r--r--   0        0        0      246 2023-03-10 17:12:41.246442 weewx-5.0.0b3/bin/weewx/wxengine.py
+-rw-r--r--   0        0        0    30034 2023-03-10 17:12:41.246442 weewx-5.0.0b3/bin/weewx/wxformulas.py
+-rw-r--r--   0        0        0      367 2023-03-10 17:12:41.246442 weewx-5.0.0b3/bin/weewx/wxmanager.py
+-rw-r--r--   0        0        0     7270 2023-03-10 17:12:41.246442 weewx-5.0.0b3/bin/weewx/wxservices.py
+-rw-r--r--   0        0        0    34292 2023-03-10 17:12:41.246442 weewx-5.0.0b3/bin/weewx/wxxtypes.py
+-rw-r--r--   0        0        0    55988 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewx/xtypes.py
+-rwxr-xr-x   0        0        0     9681 2023-05-21 20:58:20.135973 weewx-5.0.0b3/bin/weewxd.py
+-rw-r--r--   0        0        0    12175 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/changelog.el
+-rw-r--r--   0        0        0    12070 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/changelog.suse
+-rw-r--r--   0        0        0     2731 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/debian/README
+-rw-r--r--   0        0        0    21471 2023-05-27 15:03:47.329472 weewx-5.0.0b3/pkg/debian/changelog
+-rw-r--r--   0        0        0        3 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/debian/compat
+-rw-r--r--   0        0        0       36 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/debian/conffiles
+-rwxr-xr-x   0        0        0     3398 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/debian/config
+-rw-r--r--   0        0        0      724 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/debian/control
+-rw-r--r--   0        0        0      926 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/debian/copyright
+-rwxr-xr-x   0        0        0     8937 2023-05-21 20:58:20.143972 weewx-5.0.0b3/pkg/debian/postinst
+-rwxr-xr-x   0        0        0      906 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/debian/postrm
+-rwxr-xr-x   0        0        0      410 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/debian/preinst
+-rwxr-xr-x   0        0        0      693 2023-05-21 20:58:20.147972 weewx-5.0.0b3/pkg/debian/prerm
+-rwxr-xr-x   0        0        0     2985 2023-05-27 11:52:09.345505 weewx-5.0.0b3/pkg/debian/rules
+-rw-r--r--   0        0        0       12 2020-03-05 01:18:46.000000 weewx-5.0.0b3/pkg/debian/source/format
+-rw-r--r--   0        0        0     5501 2023-05-21 20:58:20.147972 weewx-5.0.0b3/pkg/debian/templates
+-rw-r--r--   0        0        0     1708 2023-05-21 20:58:20.147972 weewx-5.0.0b3/pkg/index-apt.html
+-rw-r--r--   0        0        0     1728 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/index-suse.html
+-rw-r--r--   0        0        0     1714 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/index-yum.html
+-rwxr-xr-x   0        0        0     9874 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/mkchangelog.pl
+-rw-r--r--   0        0        0       79 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/weewx-el8.repo
+-rw-r--r--   0        0        0       57 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/weewx-python2.list
+-rw-r--r--   0        0        0       56 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/weewx-python3.list
+-rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/weewx-suse12.repo
+-rw-r--r--   0        0        0       83 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/weewx-suse15.repo
+-rw-r--r--   0        0        0     2201 2023-03-10 17:12:41.258442 weewx-5.0.0b3/pkg/weewx.smf
+-rw-r--r--   0        0        0     7144 2023-05-27 12:03:01.691948 weewx-5.0.0b3/pkg/weewx.spec.in
+-rw-r--r--   0        0        0     2844 2023-05-27 15:02:56.745830 weewx-5.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/apache/conf-available/weewx.conf
+-rw-r--r--   0        0        0      167 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/apache/conf.d/weewx.conf
+-rw-r--r--   0        0        0      136 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/default/weewx
+-rwxr-xr-x   0        0        0     8897 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/i18n/i18n-report
+-rw-r--r--   0        0        0     9052 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/import/csv-example.conf
+-rw-r--r--   0        0        0     8250 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/import/cumulus-example.conf
+-rw-r--r--   0        0        0    14923 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/import/wd-example.conf
+-rw-r--r--   0        0        0     7100 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/import/weathercat-example.conf
+-rw-r--r--   0        0        0     6202 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/import/wu-example.conf
+-rwxr-xr-x   0        0        0     6057 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-03-13 13:33:49.303977 weewx-5.0.0b3/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0     1800 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/logrotate.d/weewx
+-rw-r--r--   0        0        0       83 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/logwatch/conf/logfiles/weewx.conf
+-rw-r--r--   0        0        0       32 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/logwatch/conf/services/weewx.conf
+-rwxr-xr-x   0        0        0    54942 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/logwatch/scripts/services/weewx
+-rw-r--r--   0        0        0       82 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/newsyslog.d/weewx.conf
+-rw-r--r--   0        0        0     2219 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/rsyslog.d/weewx.conf
+-rwxr-xr-x   0        0        0      319 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/wee_database
+-rwxr-xr-x   0        0        0      316 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/wee_debug
+-rwxr-xr-x   0        0        0      317 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/wee_device
+-rwxr-xr-x   0        0        0      317 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/wee_import
+-rwxr-xr-x   0        0        0      318 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/wee_reports
+-rwxr-xr-x   0        0        0      313 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/weectl
+-rwxr-xr-x   0        0        0      313 2023-05-21 20:58:20.147972 weewx-5.0.0b3/util/scripts/weewxd
+-rw-r--r--   0        0        0     2564 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/solaris/weewx-smf.xml
+-rw-r--r--   0        0        0      536 2023-03-28 23:07:34.757396 weewx-5.0.0b3/util/systemd/weewx.service
+-rw-r--r--   0        0        0       34 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/tmpfiles.d/weewx.conf
+-rw-r--r--   0        0        0      149 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/udev/rules.d/acurite.rules
+-rw-r--r--   0        0        0      135 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/udev/rules.d/cc3000.rules
+-rw-r--r--   0        0        0      153 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/udev/rules.d/fousb.rules
+-rw-r--r--   0        0        0      147 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/udev/rules.d/te923.rules
+-rw-r--r--   0        0        0      624 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/udev/rules.d/vantage.rules
+-rw-r--r--   0        0        0     1560 2023-03-10 17:12:41.266442 weewx-5.0.0b3/util/udev/rules.d/weewx.rules
+-rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/udev/rules.d/wmr100.rules
+-rw-r--r--   0        0        0      158 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/udev/rules.d/wmr300.rules
+-rw-r--r--   0        0        0      152 2020-04-14 15:38:00.000000 weewx-5.0.0b3/util/udev/rules.d/ws28xx.rules
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 weewx-5.0.0b3/PKG-INFO
```

### Comparing `weewx-5.0.0b2/LICENSE.txt` & `weewx-5.0.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/README.md` & `weewx-5.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/schemas/wview.py` & `weewx-5.0.0b3/bin/schemas/wview.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/schemas/wview_extended.py` & `weewx-5.0.0b3/bin/schemas/wview_extended.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/schemas/wview_small.py` & `weewx-5.0.0b3/bin/schemas/wview_small.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_database.py` & `weewx-5.0.0b3/bin/wee_database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_debug.py` & `weewx-5.0.0b3/bin/wee_debug.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_device.py` & `weewx-5.0.0b3/bin/wee_device.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_import.py` & `weewx-5.0.0b3/bin/wee_import.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_reports.py` & `weewx-5.0.0b3/bin/wee_reports.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/bin/user/extensions.py` & `weewx-5.0.0b3/bin/wee_resources/bin/user/extensions.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/404.html` & `weewx-5.0.0b3/bin/wee_resources/docs/404.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       
         <meta name="author" content="Tom Keffer <tkeffer@gmail.com>">
       
       
       
       
       <link rel="icon" href="/images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/images/favicon.png` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/bundle.4b2c34cd.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/javascripts/workers/search.db81ec45.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/main.0d440cfe.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map` & `weewx-5.0.0b3/bin/wee_resources/docs/assets/stylesheets/palette.2505c338.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/changes/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/changes/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../hardware.htm">
       
       
         <link rel="next" href="../support/">
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Change log - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/copyright/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/copyright/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       
       
         <link rel="canonical" href="https://www.weewx.com/copyright/">
       
       
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>WeeWX Copyright {#weewx-copyright} - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/css/tocbot-4.12.0.css` & `weewx-5.0.0b3/bin/wee_resources/docs/css/tocbot-4.12.0.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/css/tocbot-4.3.1.css` & `weewx-5.0.0b3/bin/wee_resources/docs/css/tocbot-4.3.1.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/css/weewx_ui.css` & `weewx-5.0.0b3/bin/wee_resources/docs/css/weewx_ui.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/appendix/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/appendix/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../options_ref/">
       
       
         <link rel="next" href="../../utilities/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Appendix - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/cheetah/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/cheetah/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../custom_reports/">
       
       
         <link rel="next" href="../image_generator/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>The Cheetah generator - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/custom_reports/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/custom_reports/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../">
       
       
         <link rel="next" href="../cheetah/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Customizing reports - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/database/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/database/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../service_engine/">
       
       
         <link rel="next" href="../units/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Customizing the database - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/derived/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/derived/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../units/">
       
       
         <link rel="next" href="../drivers/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Derived types - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/drivers/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/drivers/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../derived/">
       
       
         <link rel="next" href="../extensions/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Custom drivers - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/extensions/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/extensions/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../drivers/">
       
       
         <link rel="next" href="../options_ref/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Extensions - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/image_generator/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/image_generator/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../cheetah/">
       
       
         <link rel="next" href="../multiple_bindings/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>The Image generator - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../usersguide/weewx-config-file/engine/">
       
       
         <link rel="next" href="custom_reports/">
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Introduction - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/localization/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/localization/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../multiple_bindings/">
       
       
         <link rel="next" href="../service_engine/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Localization - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/multiple_bindings/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/multiple_bindings/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../image_generator/">
       
       
         <link rel="next" href="../localization/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Multiple data bindings - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/options_ref/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/options_ref/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 000001d0: 0a20 2020 2020 200a 2020 2020 2020 3c6c  .      .      <l
 000001e0: 696e 6b20 7265 6c3d 2269 636f 6e22 2068  ink rel="icon" h
 000001f0: 7265 663d 222e 2e2f 2e2e 2f69 6d61 6765  ref="../../image
 00000200: 732f 6661 7669 636f 6e2e 706e 6722 3e0a  s/favicon.png">.
 00000210: 2020 2020 2020 3c6d 6574 6120 6e61 6d65        <meta name
 00000220: 3d22 6765 6e65 7261 746f 7222 2063 6f6e  ="generator" con
 00000230: 7465 6e74 3d22 6d6b 646f 6373 2d31 2e34  tent="mkdocs-1.4
-00000240: 2e32 2c20 6d6b 646f 6373 2d6d 6174 6572  .2, mkdocs-mater
+00000240: 2e33 2c20 6d6b 646f 6373 2d6d 6174 6572  .3, mkdocs-mater
 00000250: 6961 6c2d 392e 302e 3132 223e 0a20 2020  ial-9.0.12">.   
 00000260: 200a 2020 2020 0a20 2020 2020 200a 2020   .    .      .  
 00000270: 2020 2020 2020 3c74 6974 6c65 3e52 6566        <title>Ref
 00000280: 6572 656e 6365 3a20 6f70 7469 6f6e 7320  erence: options 
 00000290: 2d20 7765 6577 7820 646f 6375 6d65 6e74  - weewx document
 000002a0: 6174 696f 6e3c 2f74 6974 6c65 3e0a 2020  ation</title>.  
 000002b0: 2020 2020 0a20 2020 200a 2020 2020 0a20      .    .    .
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/service_engine/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/service_engine/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 000001d0: 7365 2f22 3e0a 2020 2020 2020 0a20 2020  se/">.      .   
 000001e0: 2020 203c 6c69 6e6b 2072 656c 3d22 6963     <link rel="ic
 000001f0: 6f6e 2220 6872 6566 3d22 2e2e 2f2e 2e2f  on" href="../../
 00000200: 696d 6167 6573 2f66 6176 6963 6f6e 2e70  images/favicon.p
 00000210: 6e67 223e 0a20 2020 2020 203c 6d65 7461  ng">.      <meta
 00000220: 206e 616d 653d 2267 656e 6572 6174 6f72   name="generator
 00000230: 2220 636f 6e74 656e 743d 226d 6b64 6f63  " content="mkdoc
-00000240: 732d 312e 342e 322c 206d 6b64 6f63 732d  s-1.4.2, mkdocs-
+00000240: 732d 312e 342e 332c 206d 6b64 6f63 732d  s-1.4.3, mkdocs-
 00000250: 6d61 7465 7269 616c 2d39 2e30 2e31 3222  material-9.0.12"
 00000260: 3e0a 2020 2020 0a20 2020 200a 2020 2020  >.    .    .    
 00000270: 2020 0a20 2020 2020 2020 203c 7469 746c    .        <titl
 00000280: 653e 4375 7374 6f6d 697a 696e 6720 7468  e>Customizing th
 00000290: 6520 7365 7276 6963 6520 656e 6769 6e65  e service engine
 000002a0: 202d 2077 6565 7778 2064 6f63 756d 656e   - weewx documen
 000002b0: 7461 7469 6f6e 3c2f 7469 746c 653e 0a20  tation</title>.
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/custom/units/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/custom/units/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../database/">
       
       
         <link rel="next" href="../derived/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Customizing units - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/devnotes/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/devnotes/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 000001c0: 7761 7265 2e68 746d 223e 0a20 2020 2020  ware.htm">.     
 000001d0: 200a 2020 2020 2020 3c6c 696e 6b20 7265   .      <link re
 000001e0: 6c3d 2269 636f 6e22 2068 7265 663d 222e  l="icon" href=".
 000001f0: 2e2f 696d 6167 6573 2f66 6176 6963 6f6e  ./images/favicon
 00000200: 2e70 6e67 223e 0a20 2020 2020 203c 6d65  .png">.      <me
 00000210: 7461 206e 616d 653d 2267 656e 6572 6174  ta name="generat
 00000220: 6f72 2220 636f 6e74 656e 743d 226d 6b64  or" content="mkd
-00000230: 6f63 732d 312e 342e 322c 206d 6b64 6f63  ocs-1.4.2, mkdoc
+00000230: 6f63 732d 312e 342e 332c 206d 6b64 6f63  ocs-1.4.3, mkdoc
 00000240: 732d 6d61 7465 7269 616c 2d39 2e30 2e31  s-material-9.0.1
 00000250: 3222 3e0a 2020 2020 0a20 2020 200a 2020  2">.    .    .  
 00000260: 2020 2020 0a20 2020 2020 2020 203c 7469      .        <ti
 00000270: 746c 653e 4e6f 7465 7320 666f 7220 6465  tle>Notes for de
 00000280: 7665 6c6f 7065 7273 202d 2077 6565 7778  velopers - weewx
 00000290: 2064 6f63 756d 656e 7461 7469 6f6e 3c2f   documentation</
 000002a0: 7469 746c 653e 0a20 2020 2020 200a 2020  title>.      .
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/examples/tag.htm` & `weewx-5.0.0b3/bin/wee_resources/docs/examples/tag.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/hardware.htm` & `weewx-5.0.0b3/bin/wee_resources/docs/hardware.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/antialias.gif` & `weewx-5.0.0b3/bin/wee_resources/docs/images/antialias.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/day-gap-not-shown.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/day-gap-not-shown.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/day-gap-showing.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/day-gap-showing.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/daycompare.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/daycompare.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/daytemp_with_avg.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/daytemp_with_avg.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/dayvaporp.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/dayvaporp.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/daywindvec.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/daywindvec.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/favicon.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/ferrites.jpg` & `weewx-5.0.0b3/bin/wee_resources/docs/images/ferrites.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/funky_degree.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/funky_degree.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/image_parts.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/image_parts.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/image_parts.xcf` & `weewx-5.0.0b3/bin/wee_resources/docs/images/image_parts.xcf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-apple.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-apple.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-centos.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-centos.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-debian.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-debian.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-fedora.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-fedora.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-linux.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-linux.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-mint.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-mint.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-opensuse.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-opensuse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-pypi.svg` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-redhat.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-redhat.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-rpi.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-rpi.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-suse.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-suse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-ubuntu.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-ubuntu.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/logo-weewx.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/logo-weewx.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/pipeline.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/sample_monthrain.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/sample_monthrain.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/sample_monthtempdew.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/sample_monthtempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/weekgustoverlay.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/weekgustoverlay.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/weektempdew.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/weektempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/yeardiff.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/yeardiff.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/images/yearhilow.png` & `weewx-5.0.0b3/bin/wee_resources/docs/images/yearhilow.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       
       
         <link rel="canonical" href="https://www.weewx.com/">
       
       
       
       <link rel="icon" href="images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/js/cash.js` & `weewx-5.0.0b3/bin/wee_resources/docs/js/cash.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/js/cash.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/js/cash.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/js/tocbot-4.12.0.js` & `weewx-5.0.0b3/bin/wee_resources/docs/js/tocbot-4.12.0.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/js/tocbot-4.12.0.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/js/tocbot-4.12.0.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/js/tocbot-4.3.1.min.js` & `weewx-5.0.0b3/bin/wee_resources/docs/js/tocbot-4.3.1.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/js/weewx.js` & `weewx-5.0.0b3/bin/wee_resources/docs/js/weewx.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/debian/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/debian/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../">
       
       
         <link rel="next" href="../redhat/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Debian - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         <link rel="canonical" href="https://www.weewx.com/quickstarts/">
       
       
       
         <link rel="next" href="debian/">
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Quick starts - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/pip/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/pip/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../suse/">
       
       
         <link rel="next" href="../v5-upgrade/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>pip - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/redhat/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/redhat/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../debian/">
       
       
         <link rel="next" href="../suse/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>RedHat - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/suse/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/suse/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../redhat/">
       
       
         <link rel="next" href="../pip/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>SuSE - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/quickstarts/v5-upgrade/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../pip/">
       
       
         <link rel="next" href="../../usersguide/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Migrating to V5 - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/report_scheduling/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/report_scheduling/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       
       
         <link rel="canonical" href="https://www.weewx.com/report_scheduling/">
       
       
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Scheduling report generation - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/search/search_index.json` & `weewx-5.0.0b3/bin/wee_resources/docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/sitemap.xml` & `weewx-5.0.0b3/bin/wee_resources/docs/sitemap.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/sitemap.xml.gz` & `weewx-5.0.0b3/bin/wee_resources/docs/sitemap.xml.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitemap.xml", last modified: Sat May 27 12:08:45 2023, max compression
+gzip compressed data, was "sitemap.xml", last modified: Sat May 27 15:04:07 2023, max compression
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/sle/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/sle/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       
       
         <link rel="canonical" href="https://www.weewx.com/sle/">
       
       
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Writing search list extensions - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/support/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/support/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         <link rel="canonical" href="https://www.weewx.com/support/">
       
       
         <link rel="prev" href="../changes/">
       
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Support - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/upgrading.htm` & `weewx-5.0.0b3/bin/wee_resources/docs/upgrading.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../webserver-integration/">
       
       
         <link rel="next" href="../mysql-mariadb-config/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Backup & restore - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../quickstarts/v5-upgrade/">
       
       
         <link rel="next" href="system-requirements/">
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Introduction - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/installing-weewx/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/installing-weewx/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../system-requirements/">
       
       
         <link rel="next" href="../where/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Installing WeeWX - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../backing-up-weewx/">
       
       
         <link rel="next" href="../troubleshooting-guide/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Configuring MySQL - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/running-weewx/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/running-weewx/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../where/">
       
       
         <link rel="next" href="../webserver-integration/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Running WeeWX - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/system-requirements/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/system-requirements/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../">
       
       
         <link rel="next" href="../installing-weewx/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>System requirements - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/troubleshooting-guide/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../mysql-mariadb-config/">
       
       
         <link rel="next" href="../weewx-config-file/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Troubleshooting - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/webserver-integration/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/webserver-integration/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../running-weewx/">
       
       
         <link rel="next" href="../backing-up-weewx/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Web server integration - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdtimesynch/">
       
       
         <link rel="next" href="../databases/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[DataBindings] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../data-bindings/">
       
       
         <link rel="next" href="../databasetypes/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[Databases] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../databases/">
       
       
         <link rel="next" href="../engine/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[DatabaseTypes] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../databasetypes/">
       
       
         <link rel="next" href="../../../custom/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[Engine] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../">
       
       
         <link rel="next" href="../stations-config/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>General options - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../troubleshooting-guide/">
       
       
         <link rel="next" href="general/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Overview - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 000001f0: 0a20 2020 2020 200a 2020 2020 2020 3c6c  .      .      <l
 00000200: 696e 6b20 7265 6c3d 2269 636f 6e22 2068  ink rel="icon" h
 00000210: 7265 663d 222e 2e2f 2e2e 2f2e 2e2f 696d  ref="../../../im
 00000220: 6167 6573 2f66 6176 6963 6f6e 2e70 6e67  ages/favicon.png
 00000230: 223e 0a20 2020 2020 203c 6d65 7461 206e  ">.      <meta n
 00000240: 616d 653d 2267 656e 6572 6174 6f72 2220  ame="generator" 
 00000250: 636f 6e74 656e 743d 226d 6b64 6f63 732d  content="mkdocs-
-00000260: 312e 342e 322c 206d 6b64 6f63 732d 6d61  1.4.2, mkdocs-ma
+00000260: 312e 342e 332c 206d 6b64 6f63 732d 6d61  1.4.3, mkdocs-ma
 00000270: 7465 7269 616c 2d39 2e30 2e31 3222 3e0a  terial-9.0.12">.
 00000280: 2020 2020 0a20 2020 200a 2020 2020 2020      .    .      
 00000290: 0a20 2020 2020 2020 203c 7469 746c 653e  .        <title>
 000002a0: 5b53 7461 7469 6f6e 5d20 2d20 7765 6577  [Station] - weew
 000002b0: 7820 646f 6375 6d65 6e74 6174 696f 6e3c  x documentation<
 000002c0: 2f74 6974 6c65 3e0a 2020 2020 2020 0a20  /title>.      . 
 000002d0: 2020 200a 2020 2020 0a20 2020 2020 203c     .    .      <
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdwxcalculate-config/">
       
       
         <link rel="next" href="../stdtimesynch/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdArchive] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdconvert-config/">
       
       
         <link rel="next" href="../stdqc-config/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdCalibrate] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdreport-config/">
       
       
         <link rel="next" href="../stdcalibrate-config/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdConvert] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdcalibrate-config/">
       
       
         <link rel="next" href="../stdwxcalculate-config/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdQC] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdrestful-config/">
       
       
         <link rel="next" href="../stdconvert-config/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdReport] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 000001f0: 636f 6e66 6967 2f22 3e0a 2020 2020 2020  config/">.      
 00000200: 0a20 2020 2020 203c 6c69 6e6b 2072 656c  .      <link rel
 00000210: 3d22 6963 6f6e 2220 6872 6566 3d22 2e2e  ="icon" href="..
 00000220: 2f2e 2e2f 2e2e 2f69 6d61 6765 732f 6661  /../../images/fa
 00000230: 7669 636f 6e2e 706e 6722 3e0a 2020 2020  vicon.png">.    
 00000240: 2020 3c6d 6574 6120 6e61 6d65 3d22 6765    <meta name="ge
 00000250: 6e65 7261 746f 7222 2063 6f6e 7465 6e74  nerator" content
-00000260: 3d22 6d6b 646f 6373 2d31 2e34 2e32 2c20  ="mkdocs-1.4.2, 
+00000260: 3d22 6d6b 646f 6373 2d31 2e34 2e33 2c20  ="mkdocs-1.4.3, 
 00000270: 6d6b 646f 6373 2d6d 6174 6572 6961 6c2d  mkdocs-material-
 00000280: 392e 302e 3132 223e 0a20 2020 200a 2020  9.0.12">.    .  
 00000290: 2020 0a20 2020 2020 200a 2020 2020 2020    .      .      
 000002a0: 2020 3c74 6974 6c65 3e5b 5374 6452 4553    <title>[StdRES
 000002b0: 5466 756c 5d20 2d20 7765 6577 7820 646f  Tful] - weewx do
 000002c0: 6375 6d65 6e74 6174 696f 6e3c 2f74 6974  cumentation</tit
 000002d0: 6c65 3e0a 2020 2020 2020 0a20 2020 200a  le>.      .    .
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdarchive/">
       
       
         <link rel="next" href="../data-bindings/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdTimeSynch] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../stdqc-config/">
       
       
         <link rel="next" href="../stdarchive/">
       
       <link rel="icon" href="../../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>[StdWXCalculate] - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/usersguide/where/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/usersguide/where/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../installing-weewx/">
       
       
         <link rel="next" href="../running-weewx/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Where to find things - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/utilities/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/utilities/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../custom/appendix/">
       
       
         <link rel="next" href="../weectl/">
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Overview - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/utilities/utilities.htm` & `weewx-5.0.0b3/bin/wee_resources/docs/utilities/utilities.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/weectl/extension/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/weectl/extension/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../station/">
       
       
         <link rel="next" href="../../upgrading.htm">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>weectl extension - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/weectl/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/weectl/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../utilities/">
       
       
         <link rel="next" href="station/">
       
       <link rel="icon" href="../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>Overview - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/docs/weectl/station/index.html` & `weewx-5.0.0b3/bin/wee_resources/docs/weectl/station/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       
         <link rel="prev" href="../">
       
       
         <link rel="next" href="../extension/">
       
       <link rel="icon" href="../../images/favicon.png">
-      <meta name="generator" content="mkdocs-1.4.2, mkdocs-material-9.0.12">
+      <meta name="generator" content="mkdocs-1.4.3, mkdocs-material-9.0.12">
     
     
       
         <title>weectl station - weewx documentation</title>
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc` & `weewx-5.0.0b3/bin/wee_resources/examples/__pycache__/seven_day.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc` & `weewx-5.0.0b3/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc` & `weewx-5.0.0b3/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/alarm.py` & `weewx-5.0.0b3/bin/wee_resources/examples/alarm.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/install.py` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/readme.md` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/basic.css` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/basic.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/current.inc` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/favicon.ico` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/hilo.inc` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/lang/en.conf` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/basic/skins/basic/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/examples/basic/skins/basic/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc` & `weewx-5.0.0b3/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc` & `weewx-5.0.0b3/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc` & `weewx-5.0.0b3/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/colorize/colorize_1.py` & `weewx-5.0.0b3/bin/wee_resources/examples/colorize/colorize_1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/colorize/colorize_2.py` & `weewx-5.0.0b3/bin/wee_resources/examples/colorize/colorize_2.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/colorize/colorize_3.py` & `weewx-5.0.0b3/bin/wee_resources/examples/colorize/colorize_3.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/fileparse/bin/user/fileparse.py` & `weewx-5.0.0b3/bin/wee_resources/examples/fileparse/bin/user/fileparse.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/fileparse/install.py` & `weewx-5.0.0b3/bin/wee_resources/examples/fileparse/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/fileparse/readme.md` & `weewx-5.0.0b3/bin/wee_resources/examples/fileparse/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/lowBattery.py` & `weewx-5.0.0b3/bin/wee_resources/examples/lowBattery.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/mem.py` & `weewx-5.0.0b3/bin/wee_resources/examples/mem.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/pmon/bin/user/pmon.py` & `weewx-5.0.0b3/bin/wee_resources/examples/pmon/bin/user/pmon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/pmon/install.py` & `weewx-5.0.0b3/bin/wee_resources/examples/pmon/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/pmon/readme.md` & `weewx-5.0.0b3/bin/wee_resources/examples/pmon/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/pmon/skins/pmon/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/examples/pmon/skins/pmon/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/tests/test_vaporpressure.py` & `weewx-5.0.0b3/bin/wee_resources/examples/tests/test_vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/vaporpressure.py` & `weewx-5.0.0b3/bin/wee_resources/examples/vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/xstats/bin/user/xstats.py` & `weewx-5.0.0b3/bin/wee_resources/examples/xstats/bin/user/xstats.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/xstats/install.py` & `weewx-5.0.0b3/bin/wee_resources/examples/xstats/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/xstats/readme.txt` & `weewx-5.0.0b3/bin/wee_resources/examples/xstats/readme.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/examples/xstats/skins/xstats/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/examples/xstats/skins/xstats/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/favicon.ico` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/de.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/en.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/nl.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/lang/no.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/mobile.css` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/mobile.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Mobile/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Mobile/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # configuration file for Mobile skin
 
 SKIN_NAME = Mobile
-SKIN_VERSION = 5.0.0b1
+SKIN_VERSION = 5.0.0b3
 
 [Extras]
     # Set this URL to display a radar image
     #radar_img = http://radar.weather.gov/ridge/lite/N0R/RTX_loop.gif
     # Set this URL for the radar image link
     #radar_url = http://radar.weather.gov/ridge/radar.php?product=NCR&rid=RTX&loop=yes
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Rsync/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Rsync/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 #                                                                             #
 # RSYNC CONFIGURATION FILE                                                    #
 #   This 'report' does not generate any files. Instead, we use the report     #
 #   engine to invoke rsync, which synchronizes files between two locations.   #
 ###############################################################################
 
 SKIN_NAME = Rsync
-SKIN_VERSION = 5.0.0b1
+SKIN_VERSION = 5.0.0b3
 
 [Generators]
     generator_list = weewx.reportengine.RsyncGenerator
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/about.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/about.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/analytics.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/analytics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/celestial.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/celestial.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/celestial.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/celestial.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/current.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/favicon.ico` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OFL.txt` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans.woff` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans.woff`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/OpenSans.woff2` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/OpenSans.woff2`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/font/license.txt` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/font/license.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/hilo.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/identifier.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/identifier.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/cn.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/cn.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/cz.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/cz.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/de.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/en.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/es.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/es.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/fr.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/gr.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/gr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/it.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/it.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/nl.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/no.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/lang/th.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/lang/th.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/map.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/map.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/radar.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/radar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/rss.xml.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/satellite.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/satellite.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/seasons.css` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/seasons.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/seasons.js` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/seasons.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/sensors.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/sensors.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # SEASONS SKIN CONFIGURATION FILE                                             #
 # Copyright (c) 2018-2021 Tom Keffer <tkeffer@gmail.com> and Matthew Wall     #
 # See the file LICENSE.txt for your rights.                                   #
 ###############################################################################
 
 SKIN_NAME = Seasons
-SKIN_VERSION = 5.0.0b1
+SKIN_VERSION = 5.0.0b3
 
 ###############################################################################
 
 # The following section is for any extra tags that you want to be available in
 # the templates
 
 [Extras]
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/statistics.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/statistics.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/statistics.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/statistics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/sunmoon.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/sunmoon.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/tabular.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/tabular.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/telemetry.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/telemetry.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Seasons/titlebar.inc` & `weewx-5.0.0b3/bin/wee_resources/skins/Seasons/titlebar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/barometer.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/favicon.ico` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/humidity.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/de.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/en.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/nl.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/lang/no.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/rain.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # configuration file for Smartphone skin
 
 SKIN_NAME = Smartphone
-SKIN_VERSION = 5.0.0b1
+SKIN_VERSION = 5.0.0b3
 
 [Extras]
     # Set this URL to display a radar image
     #radar_img = http://radar.weather.gov/ridge/lite/N0R/RTX_loop.gif
     # Set this URL for the radar image link
     #radar_url = http://radar.weather.gov/ridge/radar.php?product=NCR&rid=RTX&loop=yes
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/temp.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/temp.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Smartphone/wind.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/drops.gif` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/drops.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/flower.jpg` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/flower.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/backgrounds/night.gif` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/backgrounds/night.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/favicon.ico` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/de.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/en.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/fr.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/nl.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/lang/no.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/month.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/month.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/skin.conf` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # STANDARD SKIN CONFIGURATION FILE                                            #
 # Copyright (c) 2010-2021 Tom Keffer <tkeffer@gmail.com>                      #
 # See the file LICENSE.txt for your rights.                                   #
 ###############################################################################
 
 SKIN_NAME = Standard
-SKIN_VERSION = 5.0.0b1
+SKIN_VERSION = 5.0.0b3
 
 ###############################################################################
 
 # The following section is for any extra tags that you want to be available in the templates
 [Extras]
     
     # This radar image would be available as $Extras.radar_img
```

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/week.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/week.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/weewx.css` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/weewx.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/skins/Standard/year.html.tmpl` & `weewx-5.0.0b3/bin/wee_resources/skins/Standard/year.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx-multi` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.bsd` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.debian` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.freebsd` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.lsb` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.redhat` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/init.d/weewx.suse` & `weewx-5.0.0b3/bin/wee_resources/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b3/bin/wee_resources/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/util/systemd/weewx.service` & `weewx-5.0.0b3/bin/wee_resources/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/wee_resources/weewx.conf` & `weewx-5.0.0b3/bin/wee_resources/weewx.conf`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Whether to log successful operations. May get overridden below.
 log_success = True
 
 # Whether to log unsuccessful operations. May get overridden below.
 log_failure = True
 
 # Do not modify this. It is used when installing and updating weewx.
-version = 5.0.0b1
+version = 5.0.0b3
 
 ##############################################################################
 
 #   This section is for information about the station.
 
 [Station]
```

### Comparing `weewx-5.0.0b2/bin/weecfg/__init__.py` & `weewx-5.0.0b3/bin/weecfg/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weecfg/database.py` & `weewx-5.0.0b3/bin/weecfg/database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weecfg/extension.py` & `weewx-5.0.0b3/bin/weecfg/extension.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weecfg/station_config.py` & `weewx-5.0.0b3/bin/weecfg/station_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weecfg/update_config.py` & `weewx-5.0.0b3/bin/weecfg/update_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weectl.py` & `weewx-5.0.0b3/bin/weectl.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weectllib/parse_extension.py` & `weewx-5.0.0b3/bin/weectllib/parse_extension.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weectllib/parse_station.py` & `weewx-5.0.0b3/bin/weectllib/parse_station.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weedb/NOTES.md` & `weewx-5.0.0b3/bin/weedb/NOTES.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weedb/__init__.py` & `weewx-5.0.0b3/bin/weedb/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weedb/mysql.py` & `weewx-5.0.0b3/bin/weedb/mysql.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weedb/sqlite.py` & `weewx-5.0.0b3/bin/weedb/sqlite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeimport/csvimport.py` & `weewx-5.0.0b3/bin/weeimport/csvimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeimport/cumulusimport.py` & `weewx-5.0.0b3/bin/weeimport/cumulusimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeimport/wdimport.py` & `weewx-5.0.0b3/bin/weeimport/wdimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeimport/weathercatimport.py` & `weewx-5.0.0b3/bin/weeimport/weathercatimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeimport/weeimport.py` & `weewx-5.0.0b3/bin/weeimport/weeimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeimport/wuimport.py` & `weewx-5.0.0b3/bin/weeimport/wuimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeplot/genplot.py` & `weewx-5.0.0b3/bin/weeplot/genplot.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeplot/utilities.py` & `weewx-5.0.0b3/bin/weeplot/utilities.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/Moon.py` & `weewx-5.0.0b3/bin/weeutil/Moon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/Sun.py` & `weewx-5.0.0b3/bin/weeutil/Sun.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/config.py` & `weewx-5.0.0b3/bin/weeutil/config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/ftpupload.py` & `weewx-5.0.0b3/bin/weeutil/ftpupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/log.py` & `weewx-5.0.0b3/bin/weeutil/log.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/logger.py` & `weewx-5.0.0b3/bin/weeutil/logger.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/rsyncupload.py` & `weewx-5.0.0b3/bin/weeutil/rsyncupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/timediff.py` & `weewx-5.0.0b3/bin/weeutil/timediff.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weeutil/weeutil.py` & `weewx-5.0.0b3/bin/weeutil/weeutil.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/__init__.py` & `weewx-5.0.0b3/bin/weewx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #    See the file LICENSE.txt for your full rights.
 #
 """Package weewx, containing modules specific to the weewx runtime engine."""
 import os.path
 import sys
 import time
 
-__version__ = "5.0.0b1"
+__version__ = "5.0.0b3"
 
 # Holds the program launch time in unix epoch seconds:
 # Useful for calculating 'uptime.'
 launchtime_ts = time.time()
 
 # Set to true for extra debug information:
 debug = False
```

### Comparing `weewx-5.0.0b2/bin/weewx/accum.py` & `weewx-5.0.0b3/bin/weewx/accum.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/almanac.py` & `weewx-5.0.0b3/bin/weewx/almanac.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/cheetahgenerator.py` & `weewx-5.0.0b3/bin/weewx/cheetahgenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/crc16.py` & `weewx-5.0.0b3/bin/weewx/crc16.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/daemon.py` & `weewx-5.0.0b3/bin/weewx/daemon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/defaults.py` & `weewx-5.0.0b3/bin/weewx/defaults.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/__init__.py` & `weewx-5.0.0b3/bin/weewx/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/acurite.py` & `weewx-5.0.0b3/bin/weewx/drivers/acurite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/cc3000.py` & `weewx-5.0.0b3/bin/weewx/drivers/cc3000.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/fousb.py` & `weewx-5.0.0b3/bin/weewx/drivers/fousb.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/simulator.py` & `weewx-5.0.0b3/bin/weewx/drivers/simulator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/te923.py` & `weewx-5.0.0b3/bin/weewx/drivers/te923.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/ultimeter.py` & `weewx-5.0.0b3/bin/weewx/drivers/ultimeter.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/vantage.py` & `weewx-5.0.0b3/bin/weewx/drivers/vantage.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/wmr100.py` & `weewx-5.0.0b3/bin/weewx/drivers/wmr100.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/wmr300.py` & `weewx-5.0.0b3/bin/weewx/drivers/wmr300.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/wmr9x8.py` & `weewx-5.0.0b3/bin/weewx/drivers/wmr9x8.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/ws1.py` & `weewx-5.0.0b3/bin/weewx/drivers/ws1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/ws23xx.py` & `weewx-5.0.0b3/bin/weewx/drivers/ws23xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/drivers/ws28xx.py` & `weewx-5.0.0b3/bin/weewx/drivers/ws28xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/engine.py` & `weewx-5.0.0b3/bin/weewx/engine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/imagegenerator.py` & `weewx-5.0.0b3/bin/weewx/imagegenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/manager.py` & `weewx-5.0.0b3/bin/weewx/manager.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/qc.py` & `weewx-5.0.0b3/bin/weewx/qc.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/reportengine.py` & `weewx-5.0.0b3/bin/weewx/reportengine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/restx.py` & `weewx-5.0.0b3/bin/weewx/restx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/station.py` & `weewx-5.0.0b3/bin/weewx/station.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/tags.py` & `weewx-5.0.0b3/bin/weewx/tags.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/units.py` & `weewx-5.0.0b3/bin/weewx/units.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/uwxutils.py` & `weewx-5.0.0b3/bin/weewx/uwxutils.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/wxformulas.py` & `weewx-5.0.0b3/bin/weewx/wxformulas.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/wxservices.py` & `weewx-5.0.0b3/bin/weewx/wxservices.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/wxxtypes.py` & `weewx-5.0.0b3/bin/weewx/wxxtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewx/xtypes.py` & `weewx-5.0.0b3/bin/weewx/xtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/bin/weewxd.py` & `weewx-5.0.0b3/bin/weewxd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/changelog.el` & `weewx-5.0.0b3/pkg/changelog.el`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/changelog.suse` & `weewx-5.0.0b3/pkg/changelog.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/README` & `weewx-5.0.0b3/pkg/debian/README`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/changelog` & `weewx-5.0.0b3/pkg/debian/changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+weewx (5.0.0b3-1) unstable; urgency=low
+  * Update version numbers
+ -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Sat, 27 May 2023 08:03:33 -0700
 weewx (5.0.0b2-1) unstable; urgency=low
   * Remove utility wunderfixer.
   * Most almanac attributes now return a ValueHelper.
  -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Sat, 27 May 2023 05:07:43 -0700
 weewx (5.0.0b1-1) unstable; urgency=low
   * new upstream release
  -- Matthew Wall (weewx) <mwall@users.sourceforge.net>  Sat, 06 May 2023 07:35:56 -0400
```

### Comparing `weewx-5.0.0b2/pkg/debian/config` & `weewx-5.0.0b3/pkg/debian/config`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/control` & `weewx-5.0.0b3/pkg/debian/control`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/copyright` & `weewx-5.0.0b3/pkg/debian/copyright`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/postinst` & `weewx-5.0.0b3/pkg/debian/postinst`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/postrm` & `weewx-5.0.0b3/pkg/debian/postrm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/prerm` & `weewx-5.0.0b3/pkg/debian/prerm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/rules` & `weewx-5.0.0b3/pkg/debian/rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/debian/templates` & `weewx-5.0.0b3/pkg/debian/templates`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/index-apt.html` & `weewx-5.0.0b3/pkg/index-apt.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/index-suse.html` & `weewx-5.0.0b3/pkg/index-suse.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/index-yum.html` & `weewx-5.0.0b3/pkg/index-yum.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/mkchangelog.pl` & `weewx-5.0.0b3/pkg/mkchangelog.pl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/weewx.smf` & `weewx-5.0.0b3/pkg/weewx.smf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pkg/weewx.spec.in` & `weewx-5.0.0b3/pkg/weewx.spec.in`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/pyproject.toml` & `weewx-5.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weewx"
-version = "5.0.0b2"
+version = "5.0.0b3"
 description = "The WeeWX weather software system. This is an ALPHA release, and is likely to be unstable!"
 authors = ["Tom Keffer <tkeffer@gmail.com>"]
 license = "GPL3"
 readme = 'README.md'
 repository = "https://github.com/weewx/weewx"
 homepage = "https://weewx.com"
 documentation = "https://weewx.com/docs"
```

### Comparing `weewx-5.0.0b2/util/i18n/i18n-report` & `weewx-5.0.0b3/util/i18n/i18n-report`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/import/csv-example.conf` & `weewx-5.0.0b3/util/import/csv-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/import/cumulus-example.conf` & `weewx-5.0.0b3/util/import/cumulus-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/import/wd-example.conf` & `weewx-5.0.0b3/util/import/wd-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/import/weathercat-example.conf` & `weewx-5.0.0b3/util/import/weathercat-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/import/wu-example.conf` & `weewx-5.0.0b3/util/import/wu-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx-multi` & `weewx-5.0.0b3/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx.bsd` & `weewx-5.0.0b3/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx.debian` & `weewx-5.0.0b3/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx.freebsd` & `weewx-5.0.0b3/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx.lsb` & `weewx-5.0.0b3/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx.redhat` & `weewx-5.0.0b3/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/init.d/weewx.suse` & `weewx-5.0.0b3/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b3/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/logrotate.d/weewx` & `weewx-5.0.0b3/util/logrotate.d/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/logwatch/scripts/services/weewx` & `weewx-5.0.0b3/util/logwatch/scripts/services/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/rsyslog.d/weewx.conf` & `weewx-5.0.0b3/util/rsyslog.d/weewx.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/solaris/weewx-smf.xml` & `weewx-5.0.0b3/util/solaris/weewx-smf.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/systemd/weewx.service` & `weewx-5.0.0b3/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/udev/rules.d/vantage.rules` & `weewx-5.0.0b3/util/udev/rules.d/vantage.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/util/udev/rules.d/weewx.rules` & `weewx-5.0.0b3/util/udev/rules.d/weewx.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b2/PKG-INFO` & `weewx-5.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weewx
-Version: 5.0.0b2
+Version: 5.0.0b3
 Summary: The WeeWX weather software system. This is an ALPHA release, and is likely to be unstable!
 Home-page: https://weewx.com
 License: GPL3
 Author: Tom Keffer
 Author-email: tkeffer@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

