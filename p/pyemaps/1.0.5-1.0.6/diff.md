# Comparing `tmp/pyemaps-1.0.5.tar.gz` & `tmp/pyemaps-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-cf4xvpon\pyemaps-1.0.5.tar", last modified: Fri May 12 19:13:28 2023, max compression
+gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-psmco31c\pyemaps-1.0.6.tar", last modified: Sat May 27 18:57:36 2023, max compression
```

## Comparing `pyemaps-1.0.5.tar` & `pyemaps-1.0.6.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/
--rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.5/COPYING
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/CifFile/
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/CifFile/src/
--rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.5/CifFile/src/CifFile_module.py
--rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.5/CifFile/src/StarFile.py
--rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/TypeContentsParser.py
--rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_1_0.py
--rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_1_1.py
--rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_2_0.py
--rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_STAR2.py
--rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/CifFile/src/drel/
--rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/__init__.py
--rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/drel_ast_yacc.py
--rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/drel_lex.py
--rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/drel_runtime.py
--rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/parsetab.py
--rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/py_from_ast.py
--rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/parsetab.py
--rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/yapps3_compiled_rt.py
--rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      885 2023-05-12 19:13:28.000000 pyemaps-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.5/README.md
--rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.5/__config__.py
--rw-rw-rw-   0        0        0     6016 2023-05-12 19:12:49.000000 pyemaps-1.0.5/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.5/__main__.py
--rw-rw-rw-   0        0        0       21 2023-05-12 19:13:05.000000 pyemaps-1.0.5/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/cdata/
--rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Aluminium.xtl
--rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/AluminiumOxide.xtl
--rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Aluminium_FCC.xtl
--rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BariumTitanate_180k.xtl
--rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BariumTitanate_270k.xtl
--rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BariumTitanate_Tetra.xtl
--rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BiMnO3.xtl
--rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Boron_Tetra.xtl
--rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CadmiumSelenide_Hex.xtl
--rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CadmiumSulfide_Cubic.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CadmiumSulfide_Hex.xtl
--rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Chromium_BCC.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CoSb3_Skutterudite.xtl
--rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CopperOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Copper_FCC.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Cu2O_Cuprite.xtl
--rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Diamond.xtl
--rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/ErbiumPyrogermanate.xtl
--rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/FePd_Tetra.xtl
--rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/FeS2_Pyrite.xtl
--rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/GalliumAntimonide.xtl
--rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/GalliumArsenide.xtl
--rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/GalliumNitride.xtl
--rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Germanium.xtl
--rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Gold_FCC.xtl
--rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/IndiumArsenide.xtl
--rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/LaMnO3.xtl
--rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/LeadZirconateTitanate.xtl
--rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Li2MnO3.xtl
--rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/NaFeO2.xtl
--rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Nb3Sn.xtl
--rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Pentacene.xtl
--rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.5/cdata/SiAlONa.xtl
--rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Silicon.xtl
--rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/StrontiumTitanate.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TelluriumDioxide.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TinDioxide_RT.xtl
--rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TitaniumDioxide_Anatase.xtl
--rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TitaniumDioxide_Rutile.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TungstenDiselenide.xtl
--rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/VanadiumDioxide_RT.xtl
--rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/ZincOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Zinc_HCP.xtl
--rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/ZirconiumNitride.xtl
--rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/limno2.xtl
--rw-rw-rw-   0        0        0    41588 2023-05-07 18:11:19.000000 pyemaps-1.0.5/crystals.py
--rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.5/ddiffs.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/diffract/
--rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.5/diffract/__init__.py
--rw-rw-rw-   0        0        0    28522 2023-05-12 19:12:49.000000 pyemaps-1.0.5/diffract/bloch_dec.py
--rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/csf_dec.py
--rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/dif_dec.py
--rw-rw-rw-   0        0        0     5020 2023-05-12 19:12:49.000000 pyemaps-1.0.5/diffract/dpgen_dec.py
--rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/mxtal_dec.py
--rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/powder_dec.py
--rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.5/diffract/stereo_dec.py
--rw-rw-rw-   0        0        0    19525 2023-05-05 16:35:51.000000 pyemaps-1.0.5/display.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/ediom/
--rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.5/ediom/ediom.py
--rw-rw-rw-   0        0        0    35563 2023-05-11 01:51:41.000000 pyemaps-1.0.5/ediom/ediom_dec.py
--rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.5/emcontrols.py
--rw-rw-rw-   0        0        0     7175 2023-04-03 21:05:15.000000 pyemaps-1.0.5/errors.py
--rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.5/fileutils.py
--rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.5/kdiffs.py
--rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.5/license.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/
--rw-rw-rw-   0        0        0      885 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5768 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/samples/
--rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/al.img
--rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.5/samples/al_db.bin
--rw-rw-rw-   0        0        0     2703 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/al_ediom.py
--rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/powder.py
--rw-rw-rw-   0        0        0     3625 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/si_bloch.py
--rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.5/samples/si_constructor.py
--rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/si_csf.py
--rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.5/samples/si_dif.py
--rw-rw-rw-   0        0        0      795 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/si_dpgen.py
--rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/si_pyemaps.py
--rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/si_rawblochimgs.py
--rw-rw-rw-   0        0        0     3884 2023-05-12 19:12:49.000000 pyemaps-1.0.5/samples/si_scm.py
--rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/si_stereo.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/scattering/
--rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.5/scattering/__init__.py
--rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.5/scattering/sct_dec.py
--rw-rw-rw-   0        0        0      734 2023-05-12 19:13:28.000000 pyemaps-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0    21517 2023-05-07 18:11:19.000000 pyemaps-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/spg/
--rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.5/spg/__init__.py
--rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.5/spg/spg_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/
+-rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.6/COPYING
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/CifFile/
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/CifFile/src/
+-rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.6/CifFile/src/CifFile_module.py
+-rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.6/CifFile/src/StarFile.py
+-rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/TypeContentsParser.py
+-rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_1_0.py
+-rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_1_1.py
+-rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_2_0.py
+-rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/YappsStarParser_STAR2.py
+-rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/CifFile/src/drel/
+-rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/__init__.py
+-rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/drel_ast_yacc.py
+-rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/drel_lex.py
+-rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/drel_runtime.py
+-rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/parsetab.py
+-rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/drel/py_from_ast.py
+-rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/parsetab.py
+-rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.6/CifFile/src/yapps3_compiled_rt.py
+-rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      885 2023-05-27 18:57:36.000000 pyemaps-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.6/README.md
+-rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.6/__config__.py
+-rw-rw-rw-   0        0        0     6050 2023-05-27 18:00:42.000000 pyemaps-1.0.6/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.6/__main__.py
+-rw-rw-rw-   0        0        0       21 2023-05-27 18:57:19.000000 pyemaps-1.0.6/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/cdata/
+-rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Aluminium.xtl
+-rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/AluminiumOxide.xtl
+-rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Aluminium_FCC.xtl
+-rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BariumTitanate_180k.xtl
+-rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BariumTitanate_270k.xtl
+-rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BariumTitanate_Tetra.xtl
+-rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/BiMnO3.xtl
+-rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Boron_Tetra.xtl
+-rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CadmiumSelenide_Hex.xtl
+-rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CadmiumSulfide_Cubic.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CadmiumSulfide_Hex.xtl
+-rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Chromium_BCC.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CoSb3_Skutterudite.xtl
+-rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/CopperOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Copper_FCC.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Cu2O_Cuprite.xtl
+-rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Diamond.xtl
+-rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/ErbiumPyrogermanate.xtl
+-rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/FePd_Tetra.xtl
+-rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/FeS2_Pyrite.xtl
+-rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/GalliumAntimonide.xtl
+-rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/GalliumArsenide.xtl
+-rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/GalliumNitride.xtl
+-rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Germanium.xtl
+-rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Gold_FCC.xtl
+-rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/IndiumArsenide.xtl
+-rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/LaMnO3.xtl
+-rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/LeadZirconateTitanate.xtl
+-rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Li2MnO3.xtl
+-rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/NaFeO2.xtl
+-rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Nb3Sn.xtl
+-rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Pentacene.xtl
+-rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.6/cdata/SiAlONa.xtl
+-rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Silicon.xtl
+-rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/StrontiumTitanate.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TelluriumDioxide.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TinDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TitaniumDioxide_Anatase.xtl
+-rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TitaniumDioxide_Rutile.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/TungstenDiselenide.xtl
+-rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/VanadiumDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/ZincOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/Zinc_HCP.xtl
+-rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/ZirconiumNitride.xtl
+-rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.6/cdata/limno2.xtl
+-rw-rw-rw-   0        0        0    41593 2023-05-27 18:00:42.000000 pyemaps-1.0.6/crystals.py
+-rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.6/ddiffs.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/diffract/
+-rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.6/diffract/__init__.py
+-rw-rw-rw-   0        0        0    28522 2023-05-12 19:12:49.000000 pyemaps-1.0.6/diffract/bloch_dec.py
+-rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/csf_dec.py
+-rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/dif_dec.py
+-rw-rw-rw-   0        0        0     5020 2023-05-12 19:12:49.000000 pyemaps-1.0.6/diffract/dpgen_dec.py
+-rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/mxtal_dec.py
+-rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.6/diffract/powder_dec.py
+-rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.6/diffract/stereo_dec.py
+-rw-rw-rw-   0        0        0    20247 2023-05-27 18:00:42.000000 pyemaps-1.0.6/display.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/ediom/
+-rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.6/ediom/ediom.py
+-rw-rw-rw-   0        0        0    35563 2023-05-27 18:19:14.000000 pyemaps-1.0.6/ediom/ediom_dec.py
+-rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.6/emcontrols.py
+-rw-rw-rw-   0        0        0     7175 2023-05-26 02:13:51.000000 pyemaps-1.0.6/errors.py
+-rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.6/fileutils.py
+-rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.6/kdiffs.py
+-rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.6/license.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5789 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 18:57:36.000000 pyemaps-1.0.6/pyemaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/samples/
+-rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/al.img
+-rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.6/samples/al_db.bin
+-rw-rw-rw-   0        0        0      797 2023-05-27 18:28:39.000000 pyemaps-1.0.6/samples/al_dpgen.py
+-rw-rw-rw-   0        0        0     3899 2023-05-27 18:00:42.000000 pyemaps-1.0.6/samples/al_ediom.py
+-rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/powder.py
+-rw-rw-rw-   0        0        0     3610 2023-05-27 18:00:42.000000 pyemaps-1.0.6/samples/si_bloch.py
+-rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.6/samples/si_constructor.py
+-rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.6/samples/si_csf.py
+-rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.6/samples/si_dif.py
+-rw-rw-rw-   0        0        0     1698 2023-05-27 18:00:42.000000 pyemaps-1.0.6/samples/si_lacbed.py
+-rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/si_pyemaps.py
+-rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.6/samples/si_rawblochimgs.py
+-rw-rw-rw-   0        0        0     3884 2023-05-12 19:12:49.000000 pyemaps-1.0.6/samples/si_scm.py
+-rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.6/samples/si_stereo.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/scattering/
+-rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.6/scattering/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.6/scattering/sct_dec.py
+-rw-rw-rw-   0        0        0      734 2023-05-27 18:57:36.000000 pyemaps-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0    21587 2023-05-27 18:00:42.000000 pyemaps-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:57:36.000000 pyemaps-1.0.6/spg/
+-rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.6/spg/__init__.py
+-rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.6/spg/spg_dec.py
```

### Comparing `pyemaps-1.0.5/COPYING` & `pyemaps-1.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/CifFile_module.py` & `pyemaps-1.0.6/CifFile/src/CifFile_module.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/StarFile.py` & `pyemaps-1.0.6/CifFile/src/StarFile.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/TypeContentsParser.py` & `pyemaps-1.0.6/CifFile/src/TypeContentsParser.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/YappsStarParser_1_0.py` & `pyemaps-1.0.6/CifFile/src/YappsStarParser_1_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/YappsStarParser_1_1.py` & `pyemaps-1.0.6/CifFile/src/YappsStarParser_1_1.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/YappsStarParser_2_0.py` & `pyemaps-1.0.6/CifFile/src/YappsStarParser_2_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/YappsStarParser_STAR2.py` & `pyemaps-1.0.6/CifFile/src/YappsStarParser_STAR2.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/drel/drel_ast_yacc.py` & `pyemaps-1.0.6/CifFile/src/drel/drel_ast_yacc.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/drel/drel_lex.py` & `pyemaps-1.0.6/CifFile/src/drel/drel_lex.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/drel/drel_runtime.py` & `pyemaps-1.0.6/CifFile/src/drel/drel_runtime.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/drel/parsetab.py` & `pyemaps-1.0.6/CifFile/src/drel/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/drel/py_from_ast.py` & `pyemaps-1.0.6/CifFile/src/drel/py_from_ast.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/parsetab.py` & `pyemaps-1.0.6/CifFile/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/CifFile/src/yapps3_compiled_rt.py` & `pyemaps-1.0.6/CifFile/src/yapps3_compiled_rt.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/PKG-INFO` & `pyemaps-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyemaps-1.0.5/__config__.py` & `pyemaps-1.0.6/__config__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/__init__.py` & `pyemaps-1.0.6/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     # Default excitation from backend: DEF_EXCITATION (low, high)
     # Default gmax from backend: DEF_GMAX  
     # Default bmin from backend: DEF_BMIN  
     # Default intensity from backend: DEF_INTENSITY (low, high)
     # Default gctl from backend: DEF_GCTL  
     # Default zctl from backend: DEF_ZCTL
 #------------------------------------------------------------------------
+    PKG_TYPE = dif.get_pkgtype()
     (sgmn, 
      sgmx, 
      DEF_GMAX, 
      DEF_BMIN, 
      intc, 
      intz, 
      DEF_GCTL,
```

### Comparing `pyemaps-1.0.5/__main__.py` & `pyemaps-1.0.6/__main__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/BiMnO3.xtl` & `pyemaps-1.0.6/cdata/BiMnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/Boron_Tetra.xtl` & `pyemaps-1.0.6/cdata/Boron_Tetra.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/ErbiumPyrogermanate.xtl` & `pyemaps-1.0.6/cdata/ErbiumPyrogermanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/FeS2_Pyrite.xtl` & `pyemaps-1.0.6/cdata/FeS2_Pyrite.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/LeadZirconateTitanate.xtl` & `pyemaps-1.0.6/cdata/LeadZirconateTitanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/Li2MnO3.xtl` & `pyemaps-1.0.6/cdata/Li2MnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/Pentacene.xtl` & `pyemaps-1.0.6/cdata/Pentacene.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/cdata/SiAlONa.xtl` & `pyemaps-1.0.6/cdata/SiAlONa.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/crystals.py` & `pyemaps-1.0.6/crystals.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,15 +526,15 @@
 
         self._loc=[0.0]*(keylen-1)
         self._loc[-1] = 1.0 
 
         for i in range(len(locdata)):
             self._loc[i] = locdata[i]
 
-        self._data = dict(zip(akeys, self._loc))
+        self._data = dict(zip(akeys[1:], self._loc))
                 
     def __eq__(self, other):
         if not isinstance(other, Atom):
             return False
 
         if self._atype != other.atype: 
             return False
@@ -1107,15 +1107,15 @@
             if k == '_name' or k == '_dw':
                 yield (k[1:], getattr(self, k))
             if k == "_cell":
                  yield('cell', dict(self._cell))
             if k == "_spg":
                  yield('spg', dict(self._spg))
             if k == "_atoms":
-                 yield('atoms', [dict(a) for a in self.atoms])
+                 yield('atoms', [dict(a) for a in self._atoms])
 
     def loaded(self):
         '''
         Check to see if crystal data is loaded into simulation module
         or not.
         
         :return: `True` - loaded; otherwise `False`
```

### Comparing `pyemaps-1.0.5/ddiffs.py` & `pyemaps-1.0.6/ddiffs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/__init__.py` & `pyemaps-1.0.6/diffract/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/bloch_dec.py` & `pyemaps-1.0.6/diffract/bloch_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/csf_dec.py` & `pyemaps-1.0.6/diffract/csf_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/dif_dec.py` & `pyemaps-1.0.6/diffract/dif_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/dpgen_dec.py` & `pyemaps-1.0.6/diffract/dpgen_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/mxtal_dec.py` & `pyemaps-1.0.6/diffract/mxtal_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/powder_dec.py` & `pyemaps-1.0.6/diffract/powder_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/diffract/stereo_dec.py` & `pyemaps-1.0.6/diffract/stereo_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/display.py` & `pyemaps-1.0.6/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,15 @@
                         verticalalignment='bottom' if mode == 1 else 'center')
            
         if self.cShow:
             self.plotControls(emc,iax)
 
 
     def plotDDif(self):
+        # import matplotlib.colors as colors
         from matplotlib.colors import LinearSegmentedColormap
 
         idx, emc, img, color = self.difData
         
         if self.layout == 'table':
             n1, n2 = _getGridPos(idx, 3)
         else:
@@ -212,16 +213,31 @@
         clrMap = gclrs #default to grey
         if color:
             clrMap = LinearSegmentedColormap.from_list("mycmap", clrs)
 
         iax.clear()
         iax.set_axis_off()
 
-
-        iax.imshow(img, cmap=clrMap)
+# image intensity check: 
+# if intensity is below threshold, 
+# don't display the image
+        imax = img.max()
+        if imax < 1.0e-10:
+            ishape = np.shape(img)
+            img = np.zeros(ishape)
+            wmsg = "No intensity detected at: \n\n" + emc.plot_format()
+            iax.text(ishape[0]/2,ishape[1]/2, 
+                        wmsg,
+                        {'color': 'white', 'fontsize': 10},
+                        horizontalalignment='center',
+                        verticalalignment='center')
+
+        iax.imshow(img, 
+                #    norm=colors.LogNorm(vmin=imin, vmax=imax),  --- logrithmatic image normalization, not used now
+                   cmap=clrMap)
         if self.cShow:
             self.plotControls(emc,iax)
 
 
     def plotControls(self, emc, ax):
         controls_text = emc.plot_format()
```

### Comparing `pyemaps-1.0.5/ediom/ediom.py` & `pyemaps-1.0.6/ediom/ediom.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/ediom/ediom_dec.py` & `pyemaps-1.0.6/ediom/ediom_dec.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,15 +604,15 @@
         # _displayImage(mask.reshape(mr,mc), fsize =(mr, mc), isMask = True)
         return 0
     
     def loadDPDB(self, dbfn, bShowDBMap=False):
         """
         Loads the diffraction database file *dbfn* into ediom for diffraction peak searching and indexing.
 
-        See sample code *si_dpgen.py* for how to generate a diffraction pattern database with
+        See sample code *al_dpgen.py* for how to generate a diffraction pattern database with
         pyemaps `generateDPDB <pyemaps.crystals.html#pyemaps.crystals.Crystal.generateDPDB>`_.
 
         The database file can also be saved and reused.
 
         :param dbfn: DP database file name.
         :type dbfn: string, required
```

### Comparing `pyemaps-1.0.5/emcontrols.py` & `pyemaps-1.0.6/emcontrols.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/errors.py` & `pyemaps-1.0.6/errors.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/fileutils.py` & `pyemaps-1.0.6/fileutils.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/kdiffs.py` & `pyemaps-1.0.6/kdiffs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/license.txt` & `pyemaps-1.0.6/license.txt`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/pyemaps.egg-info/PKG-INFO` & `pyemaps-1.0.6/pyemaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyemaps-1.0.5/pyemaps.egg-info/SOURCES.txt` & `pyemaps-1.0.6/pyemaps.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -140,21 +140,22 @@
 pyemaps.egg-info/PKG-INFO
 pyemaps.egg-info/SOURCES.txt
 pyemaps.egg-info/dependency_links.txt
 pyemaps.egg-info/requires.txt
 pyemaps.egg-info/top_level.txt
 samples/al.img
 samples/al_db.bin
+samples/al_dpgen.py
 samples/al_ediom.py
 samples/powder.py
 samples/si_bloch.py
 samples/si_constructor.py
 samples/si_csf.py
 samples/si_dif.py
-samples/si_dpgen.py
+samples/si_lacbed.py
 samples/si_pyemaps.py
 samples/si_rawblochimgs.py
 samples/si_scm.py
 samples/si_stereo.py
 scattering/__init__.py
 scattering/sct_dec.py
 spg/__init__.py
```

### Comparing `pyemaps-1.0.5/samples/al.img` & `pyemaps-1.0.6/samples/al.img`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/al_db.bin` & `pyemaps-1.0.6/samples/al_db.bin`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/powder.py` & `pyemaps-1.0.6/samples/powder.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_bloch.py` & `pyemaps-1.0.6/samples/si_bloch.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 You should have received a copy of the GNU General Public License
 along with pyemaps.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact supprort@emlabsoftware.com for any questions and comments.
 ___________________________
 
-This sample code is to demostrate using pyemaps to generate and render
-dynamic diffraction patterns while controls. 
-
 Author:     EMLab Solutions, Inc.
-Date:       July 07, 2022    
+Date:       July 07, 2022  
+
+This sample code is to demostrate using pyemaps to generate and render
+dynamic diffraction patterns.   
 
 """
 
 from pyemaps import EMC, DEF_CBED_DSIZE
 
 MAX_PROCWORKERS = 4
```

### Comparing `pyemaps-1.0.5/samples/si_constructor.py` & `pyemaps-1.0.6/samples/si_constructor.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_csf.py` & `pyemaps-1.0.6/samples/si_csf.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_dif.py` & `pyemaps-1.0.6/samples/si_dif.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_dpgen.py` & `pyemaps-1.0.6/samples/al_dpgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-def si_dpdb(cname='Silicon'):
+def al_dpdb(cname='Aluminium'):
     from pyemaps import Crystal as cr
     from pyemaps import EMC, SIMC
     import os
    
     
     cryst = cr.from_builtin(cname)
 
@@ -21,8 +21,8 @@
 
     if dbfn is None or not os.path.exists(dbfn):
         print(f'Error finding generated DP database file')
         return -1
 
 
 if __name__ == '__main__':
-    si_dpdb()
+    al_dpdb()
```

### Comparing `pyemaps-1.0.5/samples/si_pyemaps.py` & `pyemaps-1.0.6/samples/si_pyemaps.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_rawblochimgs.py` & `pyemaps-1.0.6/samples/si_rawblochimgs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_scm.py` & `pyemaps-1.0.6/samples/si_scm.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/samples/si_stereo.py` & `pyemaps-1.0.6/samples/si_stereo.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/scattering/__init__.py` & `pyemaps-1.0.6/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/setup.cfg` & `pyemaps-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/setup.py` & `pyemaps-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,21 +78,23 @@
 #             #   '-libs:static',
 #               '-MT',
 #               '-assume:buffered_io',
 #               '-traceback',
 #               '-c']
               
 compile_args_lin= ['-m64',
+                   '-fpic',
                    '-WB', 
                    '-qopenmp', 
                    '-qmkl', 
-                   '-heap-arrays', 
-	               '-r8', 
+                   '-heap-arrays 1024', 
+	            #    '-r8', 
                    '-fpp', 
                 #    '-warn nointerfaces',
+                    '-warn all',
                    '-O3',
                 #    'fp-stack-check',
                    '-c']
 
 intel_libs = ['mkl_intel_lp64',
               'mkl_intel_thread',
               'mkl_core',
```

### Comparing `pyemaps-1.0.5/spg/__init__.py` & `pyemaps-1.0.6/spg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.5/spg/spg_dec.py` & `pyemaps-1.0.6/spg/spg_dec.py`

 * *Files identical despite different names*

