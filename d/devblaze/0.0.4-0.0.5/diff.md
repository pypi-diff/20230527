# Comparing `tmp/devblaze-0.0.4.tar.gz` & `tmp/devblaze-0.0.5.tar.gz`

## Comparing `devblaze-0.0.4.tar` & `devblaze-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,108 @@
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 devblaze-0.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devblaze-0.0.4/Makefile
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 devblaze-0.0.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/2f88094502ec7f89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/35fe71a4dd87ac17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/5eb4f5434501f633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/609322798689986d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/75c6f13fc972def1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/7b71c0436bbfd443
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/99e45b1bd08c7e6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/a71860a9be908f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/aa0d0bc3ca67ba4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.4/.ruff_cache/content/d62bd5c9e0fb954f
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/constants.py
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screens/__init__.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screens/base_app.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screens/code_browser.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screens/error.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screens/quit.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/screens/success.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/static/checkbox.css
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/static/code_browser.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/static/cookiecutter.css
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/static/modal.css
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/static/radio_set_changed.css
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 devblaze-0.0.4/devblaze/textual_utils/static/test.css
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 devblaze-0.0.4/scripts/format.sh
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 devblaze-0.0.4/scripts/lint.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devblaze-0.0.4/scripts/test.sh
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 devblaze-0.0.4/tests/test_version.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devblaze-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 devblaze-0.0.4/LICENSE
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 devblaze-0.0.4/README.md
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 devblaze-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 devblaze-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 devblaze-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devblaze-0.0.5/Makefile
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 devblaze-0.0.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/12b5f8b4e92354df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/153e189aeac79c82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/16ceaabae4bea9b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/180767816128439d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/20307a63db2f238a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/20cce0f7f910d20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/278322d9f93f4a9f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/28bca51a4e3e9f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/29a74a8acaeb818c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/2c6f7b3c67952c5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/2f91bdc101257488
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/320867a4761d5089
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/3421c7b7800a1e71
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/344ef79fd465fbca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/34fa1e8d4497dac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/3cd11faced859719
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/3d561ab267ae7a33
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/481881b623fb0448
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/4eb6863b21733e0b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/54e602cc115368d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/57c1c0f56a85875f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/5eb4f5434501f633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/5fbb3042b6d71b6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/607500b5532d3430
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/6281a5a40c5bd052
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/66bf0724d155656f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/66c968b454597476
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/679c013790f4c7ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/6a0fdaade9fbc1bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/6af0f12c21c94f39
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/70af7f72e6fe970d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/71016357684fb7b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/7567022680976c56
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/75e337f252651c97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/7a29d411a9a3d422
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/7a569873523e2155
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/7df253c45183d1ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/86cc2233f9ce79e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/955fe5e7d44afe85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/9838339761c67fd2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/98cd9935806e7cad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/a29616f5030a8fe1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/a66b6318531c92e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/aca1234cf2f2b4b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/b253269f6332c439
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/b35d5e3da7cb3bce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/b97f98efbbafb501
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bb45fb21411e73f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bb738454031952da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bba37e44ab0a1e2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bbdd7d1288effe36
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bc496f5596f85b05
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bc90f693a1e69ecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/beb9ab9dd5c5ea1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/bf7c2b14f8bf8af7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/c07e315008424931
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/c4deac4be9d792ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/ca335461e900e94a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/cefc67049cdc3090
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/d45fc170e1f59a3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/d5e32fc4d995f27d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/daa87c83cdac8911
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/ddcfd541af269dff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/de147fee78bf2aef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/e1f24f2ee8e49b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/eb4249197d5b3e41
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/f164057db031112e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/f6e982575c945547
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/f8271bd16f1e13bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.5/.ruff_cache/content/fe5a895f2f588aa9
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/__init__.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/app.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/__init__.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/containers/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/containers/base.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/containers/project.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/containers/use_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/modals/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/modals/success.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/screens/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/screens/base_app.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/screens/project.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/screens/use_service.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/static/demo.css
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/static/modals.css
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/static/project-info.css
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/static/test.css
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/static/test_screen.css
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/static/use-service.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/widgets/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/widgets/inputs.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 devblaze-0.0.5/devblaze/textual_utils/widgets/radio_sets.py
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 devblaze-0.0.5/scripts/format.sh
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 devblaze-0.0.5/scripts/lint.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devblaze-0.0.5/scripts/test.sh
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 devblaze-0.0.5/tests/test_version.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 devblaze-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 devblaze-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 devblaze-0.0.5/README.md
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 devblaze-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 devblaze-0.0.5/PKG-INFO
```

### Comparing `devblaze-0.0.4/CONTRIBUTING.md` & `devblaze-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.4/.github/PULL_REQUEST_TEMPLATE.md` & `devblaze-0.0.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.4/devblaze/main.py` & `devblaze-0.0.5/devblaze/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 from rich.console import Console
 from rich.table import Table
 
-from devblaze.textual_utils.screen import CookiecutterApp
+from app import CookiecutterApp
 
 
 def main():
     parser = argparse.ArgumentParser(prog="devblaze", add_help=False)
     parser.add_argument(
         "command",
         nargs="?",
```

### Comparing `devblaze-0.0.4/devblaze/textual_utils/screen.py` & `devblaze-0.0.5/devblaze/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,19 @@
     Label,
     Header,
     Footer,
     RadioSet,
     RadioButton,
 )
 from textual.reactive import reactive
-from cookiecutter.main import cookiecutter
 
-from devblaze.textual_utils.screens.error import ErrorScreen
-from devblaze.textual_utils.screens.quit import QuitScreen
-from devblaze.textual_utils.screens.success import SuccessScreen
+
+from cookiecutter.main import cookiecutter
 from devblaze.textual_utils.constants import CSS_PATH
+from devblaze.textual_utils.modals.success import SuccessScreen
 
 
 class CookiecutterApp(App[None]):
     """Prompts for project_type and project_name, then runs cookiecutter."""
 
     CSS_PATH = CSS_PATH
     BINDINGS = [
@@ -54,22 +53,24 @@
         with Horizontal():
             yield Label("Project Type", id="project_type_label")
             with RadioSet(id="project_type_set"):
                 yield RadioButton("django", id="project_type")
                 yield RadioButton("ddd")
         yield Grid(
             Input(
-                placeholder="Enter project name", id="project_name",
+                placeholder="Enter project name",
+                id="project_name",
             ),
             Input(placeholder="Enter app name", id="app_name"),
             Input(
                 placeholder="Enter project base name",
                 id="project_base_name",
             ),
-            id="project_inputs_grid", classes="hidden"
+            id="project_inputs_grid",
+            classes="hidden",
         )
         with Horizontal():
             yield Label("Use Git", id="use_git_label", classes="hidden")
             with RadioSet(id="use_git_set", classes="hidden"):
                 yield RadioButton("Yes", id="use_git")
                 yield RadioButton("No")
         with Horizontal():
@@ -111,15 +112,17 @@
             self.project_name = event.value.strip()
 
         if event.input.id == "app_name":
             self.app_name = event.value.strip()
 
         if event.input.id == "project_base_name":
             self.query_one(TextLog).write(
-                f"Project Type: {self.project_type}, Project Name: {self.project_name}, App Name: {self.app_name}, Project Base Name: {self.project_base_name}"
+                f"Project Type: {self.project_type},"
+                f" Project Name: {self.project_name},"
+                f" App Name: {self.app_name}, Project Base Name: {self.project_base_name}"
             )
             self.project_base_name = event.value.strip()
             self.query_one("#project_inputs_grid").add_class("hidden")
             self.query_one("#use_git_set").remove_class("hidden")
             self.query_one("#use_git_label").remove_class("hidden")
             self.query_one("#use_git_set").focus()
             self.use_git = self.query_one("#use_git").value
@@ -172,15 +175,15 @@
         self.query_one("#use_postgres_set").add_class("hidden")
         self.query_one("#use_celery_set").remove_class("hidden")
         self.query_one("#use_celery_set").focus()
         self.use_celery = bool(event.pressed.label)
         self.query_one("#use_celery_set").add_class("hidden")
 
     def action_request_quit(self) -> None:
-        self.push_screen(QuitScreen())
+        self.push_screen(SuccessScreen())
 
     def action_on_success(self) -> None:
         self.push_screen(SuccessScreen())
 
     def try_run_cookiecutter(self):
         self.query_one(TextLog).write(f"Project type: {self.project_type}")
         self.query_one(TextLog).write(f"Project name: {self.project_name}")
@@ -216,13 +219,13 @@
                     "use_nginx": self.use_nginx,
                     "use_traefik": self.use_traefik,
                 },
             )
             self.action_on_success()
         except Exception as e:
             self.query_one(TextLog).write(f"Error: {e}")
-            self.push_screen(ErrorScreen(str(e)))
+            self.push_screen(SuccessScreen(str(e)))
 
 
 if __name__ == "__main__":
     app = CookiecutterApp()
     app.run()
```

### Comparing `devblaze-0.0.4/devblaze/textual_utils/screens/success.py` & `devblaze-0.0.5/devblaze/textual_utils/modals/success.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
+from typing import TYPE_CHECKING
 
-from textual.app import ComposeResult
 from textual.containers import Grid
 from textual.screen import ModalScreen
-from textual.widgets import Label, Button
+from textual.widgets import Button, Label
 
-from devblaze.textual_utils.constants import CSS_PATH
+if TYPE_CHECKING:
+    from textual.app import ComposeResult
 
 
 class SuccessScreen(ModalScreen):
     """Screen with a dialog to quit."""
 
-    CSS_PATH = CSS_PATH
     BINDINGS = [("enter", "on_success", "Ok")]
 
     def compose(self) -> ComposeResult:
         yield Grid(
             Label("Project created successfully!", id="success"),
-            Button("Ok", variant="primary", id="ok"),
+            Button("Ok", variant="success", id="ok"),
             id="dialog",
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "ok":
             self.app.exit()
```

### Comparing `devblaze-0.0.4/.gitignore` & `devblaze-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.4/LICENSE` & `devblaze-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.4/README.md` & `devblaze-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.4/pyproject.toml` & `devblaze-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,47 +2,53 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "devblaze"
 description = "A tool for creating and managing development and production environments."
 readme = "README.md"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Environment :: Web Environment",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: Utilities",
+    "Topic :: System :: Logging",
 ]
 dependencies = [
     "cookiecutter ==2.1.1",
     "textual ==0.24.1",
 ]
 dynamic = ["version"]
 
+[project.license]
+text = "MIT"
+
+[[project.authors]]
+name = "Lirim Shala"
+email = "lirrishala@gmail.com"
+
 [project.urls]
 Homepage = "https://github.com/godd0t/devblaze"
 
-[project.license]
-file = "LICENSE"
-
 [project.scripts]
 devblaze = "devblaze.main:main"
 
 [project.optional-dependencies]
 dev = [
     "black ==23.3.0",
-    "build ==0.10.0",
     "ruff ==0.0.267",
     "twine ==4.0.2",
+    "build ==0.10.0",
 ]
 
 [tool.hatchling]
 allow-direct-references = true
 
 [tool.hatch.version]
 path = "devblaze/__init__.py"
```

