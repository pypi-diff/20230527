# Comparing `tmp/pxblat-0.1.5.tar.gz` & `tmp/pxblat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxblat-0.1.5.tar", max compression
+gzip compressed data, was "pxblat-0.1.6.tar", max compression
```

## Comparing `pxblat-0.1.5.tar` & `pxblat-0.1.6.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0     1067 2023-05-26 22:35:27.427823 pxblat-0.1.5/LICENSE
--rw-r--r--   0        0        0     4885 2023-05-26 22:35:27.427823 pxblat-0.1.5/README.md
--rw-r--r--   0        0        0     8696 2023-05-26 22:35:27.951817 pxblat-0.1.5/build.py
--rw-r--r--   0        0        0     2533 2023-05-26 22:36:04.495454 pxblat-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/__init__.py
--rw-r--r--   0        0        0       40 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/cli/__init__.py
--rw-r--r--   0        0        0      365 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/cli/cli.py
--rw-r--r--   0        0        0     6221 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/cli/client.py
--rw-r--r--   0        0        0     2325 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/cli/fa2twobit.py
--rw-r--r--   0        0        0      214 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/cli/log.py
--rw-r--r--   0        0        0     7914 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/cli/server.py
--rw-r--r--   0        0        0       54 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/__init__.py
--rw-r--r--   0        0        0    22786 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/__init__.pyi
--rw-r--r--   0        0        0       40 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/.clang-format
--rw-r--r--   0        0        0     1966 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/_extc.cpp
--rw-r--r--   0        0        0       11 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/_extc.modules
--rw-r--r--   0        0        0       81 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/_extc.sources
--rw-r--r--   0        0        0     2163 2023-05-26 22:35:27.955817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
--rw-r--r--   0        0        0    10994 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/gfClient.cpp
--rw-r--r--   0        0        0    20542 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/gfServer.cpp
--rw-r--r--   0        0        0     2721 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/gfServer_1.cpp
--rw-r--r--   0        0        0     3431 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/binder/pygfServer.cpp
--rw-r--r--   0        0        0    33509 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/bs_thread_pool.hpp
--rw-r--r--   0        0        0    28417 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/dbg.h
--rw-r--r--   0        0        0     1986 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/faToTwoBit.cpp
--rw-r--r--   0        0        0     1243 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/faToTwoBit.hpp
--rw-r--r--   0        0        0    13734 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/gfClient.cpp
--rw-r--r--   0        0        0     4866 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/gfClient.hpp
--rw-r--r--   0        0        0     6429 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/gfClient2.cpp
--rw-r--r--   0        0        0      506 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/gfClient2.hpp
--rw-r--r--   0        0        0    60953 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/gfServer.cpp
--rw-r--r--   0        0        0    11648 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/gfServer.hpp
--rw-r--r--   0        0        0    11360 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/pygfServer.cpp
--rw-r--r--   0        0        0      979 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/bindings/pygfServer.hpp
--rw-r--r--   0        0        0    24597 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/blat.c
--rw-r--r--   0        0        0     3485 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/faToTwoBit.c
--rw-r--r--   0        0        0     9944 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/gfClient.c
--rw-r--r--   0        0        0    53782 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/gfServer.c
--rw-r--r--   0        0        0       40 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/.clang-format
--rw-r--r--   0        0        0     2088 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/bandExt.h
--rw-r--r--   0        0        0     1073 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/base64.h
--rw-r--r--   0        0        0    27036 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/cheapcgi.h
--rw-r--r--   0        0        0     2097 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/filePath.h
--rw-r--r--   0        0        0      871 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/gfxPoly.h
--rw-r--r--   0        0        0     1034 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/hex.h
--rw-r--r--   0        0        0    10111 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/htmlPage.h
--rw-r--r--   0        0        0     9985 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/htmshell.h
--rw-r--r--   0        0        0      332 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/https.h
--rw-r--r--   0        0        0     4404 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/internet.h
--rw-r--r--   0        0        0     1990 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/kxTok.h
--rw-r--r--   0        0        0    16767 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/memgfx.h
--rw-r--r--   0        0        0     2997 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/mime.h
--rw-r--r--   0        0        0     1166 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/portimpl.h
--rw-r--r--   0        0        0     4401 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/rbTree.h
--rw-r--r--   0        0        0      164 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/aux/srcVersion.h
--rw-r--r--   0        0        0      916 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/core/aliType.h
--rw-r--r--   0        0        0    10193 2023-05-26 22:35:27.959817 pxblat-0.1.5/src/pxblat/extc/include/core/axt.h
--rw-r--r--   0        0        0     6449 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/bPlusTree.h
--rw-r--r--   0        0        0     4355 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/binRange.h
--rw-r--r--   0        0        0     3456 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/bits.h
--rw-r--r--   0        0        0     5877 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/chain.h
--rw-r--r--   0        0        0     1839 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/chainBlock.h
--rw-r--r--   0        0        0    56916 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/common.h
--rw-r--r--   0        0        0     4198 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/dlist.h
--rw-r--r--   0        0        0     2681 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/dnaseq.h
--rw-r--r--   0        0        0    10058 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/dnautil.h
--rw-r--r--   0        0        0     3658 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/dystring.h
--rw-r--r--   0        0        0     2795 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/errAbort.h
--rw-r--r--   0        0        0     2128 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/errCatch.h
--rw-r--r--   0        0        0     5228 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/fa.h
--rw-r--r--   0        0        0    10590 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/fuzzyFind.h
--rw-r--r--   0        0        0    19945 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/genoFind.h
--rw-r--r--   0        0        0     1115 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/gfClientLib.h
--rw-r--r--   0        0        0     2884 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/gfInternal.h
--rw-r--r--   0        0        0    12187 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/hash.h
--rw-r--r--   0        0        0    14055 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/linefile.h
--rw-r--r--   0        0        0     3618 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/localmem.h
--rw-r--r--   0        0        0    10130 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/maf.h
--rw-r--r--   0        0        0     1786 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/memalloc.h
--rw-r--r--   0        0        0    12155 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/net.h
--rw-r--r--   0        0        0    12162 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/netlib.h
--rw-r--r--   0        0        0     4114 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/nib.h
--rw-r--r--   0        0        0     8773 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/obscure.h
--rw-r--r--   0        0        0      605 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/ooc.h
--rw-r--r--   0        0        0     3981 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/options.h
--rw-r--r--   0        0        0     1910 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/patSpace.h
--rw-r--r--   0        0        0     7300 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/pipeline.h
--rw-r--r--   0        0        0     6256 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/portable.h
--rw-r--r--   0        0        0    14633 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/psl.h
--rw-r--r--   0        0        0     4818 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/rangeTree.h
--rw-r--r--   0        0        0     2459 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/repMask.h
--rw-r--r--   0        0        0     3070 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/sig.h
--rw-r--r--   0        0        0     6814 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/sqlList.h
--rw-r--r--   0        0        0     3444 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/sqlNum.h
--rw-r--r--   0        0        0     2492 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/supStitch.h
--rw-r--r--   0        0        0     2086 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/trans3.h
--rw-r--r--   0        0        0     8657 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/twoBit.h
--rw-r--r--   0        0        0     9058 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/udc.h
--rw-r--r--   0        0        0     1821 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/core/verbose.h
--rw-r--r--   0        0        0        0 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/net/gfNet.h
--rw-r--r--   0        0        0     2278 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/include/net/log.h
--rw-r--r--   0        0        0       40 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/src/.clang-format
--rw-r--r--   0        0        0    31426 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/src/aux/axt.c
--rw-r--r--   0        0        0    14386 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/src/aux/bandExt.c
--rw-r--r--   0        0        0     2996 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/src/aux/base64.c
--rw-r--r--   0        0        0    11289 2023-05-26 22:35:27.963817 pxblat-0.1.5/src/pxblat/extc/src/aux/binRange.c
--rw-r--r--   0        0        0    25709 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/blastOut.c
--rw-r--r--   0        0        0    80472 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/cheapcgi.c
--rw-r--r--   0        0        0    32618 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/ffSeedExtend.c
--rw-r--r--   0        0        0     6436 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/filePath.c
--rw-r--r--   0        0        0     2363 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/hex.c
--rw-r--r--   0        0        0    53011 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/htmlPage.c
--rw-r--r--   0        0        0    46630 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/htmshell.c
--rw-r--r--   0        0        0    27672 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/https.c
--rw-r--r--   0        0        0     2489 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/intExp.c
--rw-r--r--   0        0        0    16703 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/internet.c
--rw-r--r--   0        0        0    24031 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/maf.c
--rw-r--r--   0        0        0     2306 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/mafFromAxt.c
--rw-r--r--   0        0        0    16690 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/mime.c
--rw-r--r--   0        0        0    62706 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/net.c
--rw-r--r--   0        0        0    62778 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/netlib.c
--rw-r--r--   0        0        0     1742 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/ooc.c
--rw-r--r--   0        0        0    11962 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/patSpace.c
--rw-r--r--   0        0        0     3896 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/portimpl.c
--rw-r--r--   0        0        0    13003 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/rangeTree.c
--rw-r--r--   0        0        0    18572 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/rbTree.c
--rw-r--r--   0        0        0     5678 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/repMask.c
--rw-r--r--   0        0        0      848 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/servBrcMcw.c
--rw-r--r--   0        0        0     1033 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/servCrunx.c
--rw-r--r--   0        0        0      864 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/servcis.c
--rw-r--r--   0        0        0      906 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/servmsII.c
--rw-r--r--   0        0        0      921 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/servpws.c
--rw-r--r--   0        0        0    27041 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/sqlList.c
--rw-r--r--   0        0        0     7239 2023-05-26 22:35:27.967817 pxblat-0.1.5/src/pxblat/extc/src/aux/sqlNum.c
--rw-r--r--   0        0        0     3898 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/aux/wildcmp.c
--rw-r--r--   0        0        0      930 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/aliType.c
--rw-r--r--   0        0        0    19732 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/bPlusTree.c
--rw-r--r--   0        0        0     9051 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/bits.c
--rw-r--r--   0        0        0    17259 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/chain.c
--rw-r--r--   0        0        0    17077 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/chainBlock.c
--rw-r--r--   0        0        0    90522 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/common.c
--rw-r--r--   0        0        0     9450 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/dlist.c
--rw-r--r--   0        0        0     4604 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/dnaseq.c
--rw-r--r--   0        0        0    29952 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/dnautil.c
--rw-r--r--   0        0        0     7156 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/dystring.c
--rw-r--r--   0        0        0    12046 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/errAbort.c
--rw-r--r--   0        0        0     3932 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/errCatch.c
--rw-r--r--   0        0        0    15611 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/fa.c
--rw-r--r--   0        0        0     3714 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/ffAli.c
--rw-r--r--   0        0        0    10802 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/ffAliHelp.c
--rw-r--r--   0        0        0     4868 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/ffScore.c
--rw-r--r--   0        0        0    40189 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/fuzzyFind.c
--rw-r--r--   0        0        0    70461 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/genoFind.c
--rw-r--r--   0        0        0    52425 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/gfBlatLib.c
--rw-r--r--   0        0        0     6363 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/gfClientLib.c
--rw-r--r--   0        0        0     3845 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/gfInternal.c
--rw-r--r--   0        0        0    18190 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/gfOut.c
--rw-r--r--   0        0        0    22265 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/hash.c
--rw-r--r--   0        0        0     5273 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/kxTok.c
--rw-r--r--   0        0        0    40326 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/linefile.c
--rw-r--r--   0        0        0     7256 2023-05-26 22:35:27.971817 pxblat-0.1.5/src/pxblat/extc/src/core/localmem.c
--rw-r--r--   0        0        0    15074 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/memalloc.c
--rw-r--r--   0        0        0    12778 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/nib.c
--rw-r--r--   0        0        0    24969 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/obscure.c
--rw-r--r--   0        0        0    13012 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/options.c
--rw-r--r--   0        0        0    20522 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/osunix.c
--rw-r--r--   0        0        0    23419 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/pipeline.c
--rw-r--r--   0        0        0    63467 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/psl.c
--rw-r--r--   0        0        0     1203 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/servcl.c
--rw-r--r--   0        0        0    26961 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/supStitch.c
--rw-r--r--   0        0        0     3216 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/trans3.c
--rw-r--r--   0        0        0    33527 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/twoBit.c
--rw-r--r--   0        0        0    71967 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/udc.c
--rw-r--r--   0        0        0     4255 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/core/verbose.c
--rw-r--r--   0        0        0     2571 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/net/gfNet.c
--rw-r--r--   0        0        0     8795 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/extc/src/net/log.c
--rw-r--r--   0        0        0     3052 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/parser.py
--rw-r--r--   0        0        0        0 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/py.typed
--rw-r--r--   0        0        0     1042 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/server/__init__.py
--rw-r--r--   0        0        0     9920 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/server/basic.py
--rw-r--r--   0        0        0     3514 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/server/client.py
--rw-r--r--   0        0        0     6789 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/server/server.py
--rw-r--r--   0        0        0      725 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/server/status.py
--rw-r--r--   0        0        0      115 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/server/utils.py
--rw-r--r--   0        0        0     3431 2023-05-26 22:35:27.975817 pxblat-0.1.5/src/pxblat/utils.py
--rw-r--r--   0        0        0     6461 1970-01-01 00:00:00.000000 pxblat-0.1.5/setup.py
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 pxblat-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-27 06:02:16.177192 pxblat-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5596 2023-05-27 06:03:03.530489 pxblat-0.1.6/README.md
+-rw-r--r--   0        0        0     8696 2023-05-27 06:02:16.609204 pxblat-0.1.6/build.py
+-rw-r--r--   0        0        0     2582 2023-05-27 06:03:03.530489 pxblat-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1092 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/cli.py
+-rw-r--r--   0        0        0     5944 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/client.py
+-rw-r--r--   0        0        0     2325 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/fa2twobit.py
+-rw-r--r--   0        0        0      214 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/log.py
+-rw-r--r--   0        0        0     7914 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/server.py
+-rw-r--r--   0        0        0       54 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/__init__.py
+-rw-r--r--   0        0        0    22786 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/.clang-format
+-rw-r--r--   0        0        0     1966 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.cpp
+-rw-r--r--   0        0        0       11 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.modules
+-rw-r--r--   0        0        0       81 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.sources
+-rw-r--r--   0        0        0     2163 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
+-rw-r--r--   0        0        0    10994 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfClient.cpp
+-rw-r--r--   0        0        0    20542 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer.cpp
+-rw-r--r--   0        0        0     2721 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer_1.cpp
+-rw-r--r--   0        0        0     3431 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/pygfServer.cpp
+-rw-r--r--   0        0        0    33509 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/bs_thread_pool.hpp
+-rw-r--r--   0        0        0    28417 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/dbg.h
+-rw-r--r--   0        0        0     1986 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.cpp
+-rw-r--r--   0        0        0     1243 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.hpp
+-rw-r--r--   0        0        0    13734 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.cpp
+-rw-r--r--   0        0        0     4866 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.hpp
+-rw-r--r--   0        0        0     6429 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient2.cpp
+-rw-r--r--   0        0        0      506 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient2.hpp
+-rw-r--r--   0        0        0    60953 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.cpp
+-rw-r--r--   0        0        0    11648 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.hpp
+-rw-r--r--   0        0        0    11360 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.cpp
+-rw-r--r--   0        0        0      979 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.hpp
+-rw-r--r--   0        0        0    24597 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/blat.c
+-rw-r--r--   0        0        0     3485 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/faToTwoBit.c
+-rw-r--r--   0        0        0     9944 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/gfClient.c
+-rw-r--r--   0        0        0    53782 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/gfServer.c
+-rw-r--r--   0        0        0       40 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/.clang-format
+-rw-r--r--   0        0        0     2088 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/bandExt.h
+-rw-r--r--   0        0        0     1073 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/base64.h
+-rw-r--r--   0        0        0    27036 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/cheapcgi.h
+-rw-r--r--   0        0        0     2097 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/filePath.h
+-rw-r--r--   0        0        0      871 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/gfxPoly.h
+-rw-r--r--   0        0        0     1034 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/hex.h
+-rw-r--r--   0        0        0    10111 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/htmlPage.h
+-rw-r--r--   0        0        0     9985 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/htmshell.h
+-rw-r--r--   0        0        0      332 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/https.h
+-rw-r--r--   0        0        0     4404 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/internet.h
+-rw-r--r--   0        0        0     1990 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/kxTok.h
+-rw-r--r--   0        0        0    16767 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/memgfx.h
+-rw-r--r--   0        0        0     2997 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/mime.h
+-rw-r--r--   0        0        0     1166 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/portimpl.h
+-rw-r--r--   0        0        0     4401 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/rbTree.h
+-rw-r--r--   0        0        0      164 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/srcVersion.h
+-rw-r--r--   0        0        0      916 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/aliType.h
+-rw-r--r--   0        0        0    10193 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/axt.h
+-rw-r--r--   0        0        0     6449 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/bPlusTree.h
+-rw-r--r--   0        0        0     4355 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/binRange.h
+-rw-r--r--   0        0        0     3456 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/bits.h
+-rw-r--r--   0        0        0     5877 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/chain.h
+-rw-r--r--   0        0        0     1839 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/chainBlock.h
+-rw-r--r--   0        0        0    56916 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/common.h
+-rw-r--r--   0        0        0     4198 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dlist.h
+-rw-r--r--   0        0        0     2681 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dnaseq.h
+-rw-r--r--   0        0        0    10058 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dnautil.h
+-rw-r--r--   0        0        0     3658 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dystring.h
+-rw-r--r--   0        0        0     2795 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/errAbort.h
+-rw-r--r--   0        0        0     2128 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/errCatch.h
+-rw-r--r--   0        0        0     5228 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/fa.h
+-rw-r--r--   0        0        0    10590 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/fuzzyFind.h
+-rw-r--r--   0        0        0    19945 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/genoFind.h
+-rw-r--r--   0        0        0     1115 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/gfClientLib.h
+-rw-r--r--   0        0        0     2884 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/gfInternal.h
+-rw-r--r--   0        0        0    12187 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/hash.h
+-rw-r--r--   0        0        0    14055 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/linefile.h
+-rw-r--r--   0        0        0     3618 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/localmem.h
+-rw-r--r--   0        0        0    10130 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/maf.h
+-rw-r--r--   0        0        0     1786 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/memalloc.h
+-rw-r--r--   0        0        0    12155 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/net.h
+-rw-r--r--   0        0        0    12162 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/netlib.h
+-rw-r--r--   0        0        0     4114 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/nib.h
+-rw-r--r--   0        0        0     8773 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/obscure.h
+-rw-r--r--   0        0        0      605 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/ooc.h
+-rw-r--r--   0        0        0     3981 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/options.h
+-rw-r--r--   0        0        0     1910 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/patSpace.h
+-rw-r--r--   0        0        0     7300 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/pipeline.h
+-rw-r--r--   0        0        0     6256 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/portable.h
+-rw-r--r--   0        0        0    14633 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/psl.h
+-rw-r--r--   0        0        0     4818 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/rangeTree.h
+-rw-r--r--   0        0        0     2459 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/repMask.h
+-rw-r--r--   0        0        0     3070 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/sig.h
+-rw-r--r--   0        0        0     6814 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/sqlList.h
+-rw-r--r--   0        0        0     3444 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/sqlNum.h
+-rw-r--r--   0        0        0     2492 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/supStitch.h
+-rw-r--r--   0        0        0     2086 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/trans3.h
+-rw-r--r--   0        0        0     8657 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/twoBit.h
+-rw-r--r--   0        0        0     9058 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/udc.h
+-rw-r--r--   0        0        0     1821 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/verbose.h
+-rw-r--r--   0        0        0        0 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/net/gfNet.h
+-rw-r--r--   0        0        0     2278 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/net/log.h
+-rw-r--r--   0        0        0       40 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/.clang-format
+-rw-r--r--   0        0        0    31426 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/axt.c
+-rw-r--r--   0        0        0    14386 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/bandExt.c
+-rw-r--r--   0        0        0     2996 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/base64.c
+-rw-r--r--   0        0        0    11289 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/binRange.c
+-rw-r--r--   0        0        0    25709 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/blastOut.c
+-rw-r--r--   0        0        0    80472 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/cheapcgi.c
+-rw-r--r--   0        0        0    32618 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/ffSeedExtend.c
+-rw-r--r--   0        0        0     6436 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/filePath.c
+-rw-r--r--   0        0        0     2363 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/hex.c
+-rw-r--r--   0        0        0    53011 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/htmlPage.c
+-rw-r--r--   0        0        0    46630 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/htmshell.c
+-rw-r--r--   0        0        0    27672 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/https.c
+-rw-r--r--   0        0        0     2489 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/intExp.c
+-rw-r--r--   0        0        0    16703 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/internet.c
+-rw-r--r--   0        0        0    24031 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/maf.c
+-rw-r--r--   0        0        0     2306 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/mafFromAxt.c
+-rw-r--r--   0        0        0    16690 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/mime.c
+-rw-r--r--   0        0        0    62706 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/net.c
+-rw-r--r--   0        0        0    62778 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/netlib.c
+-rw-r--r--   0        0        0     1742 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/ooc.c
+-rw-r--r--   0        0        0    11962 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/patSpace.c
+-rw-r--r--   0        0        0     3896 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/portimpl.c
+-rw-r--r--   0        0        0    13003 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/rangeTree.c
+-rw-r--r--   0        0        0    18572 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/rbTree.c
+-rw-r--r--   0        0        0     5678 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/repMask.c
+-rw-r--r--   0        0        0      848 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servBrcMcw.c
+-rw-r--r--   0        0        0     1033 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servCrunx.c
+-rw-r--r--   0        0        0      864 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servcis.c
+-rw-r--r--   0        0        0      906 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servmsII.c
+-rw-r--r--   0        0        0      921 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servpws.c
+-rw-r--r--   0        0        0    27041 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/sqlList.c
+-rw-r--r--   0        0        0     7239 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/sqlNum.c
+-rw-r--r--   0        0        0     3898 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/wildcmp.c
+-rw-r--r--   0        0        0      930 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/aliType.c
+-rw-r--r--   0        0        0    19732 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/bPlusTree.c
+-rw-r--r--   0        0        0     9051 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/bits.c
+-rw-r--r--   0        0        0    17259 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/chain.c
+-rw-r--r--   0        0        0    17077 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/chainBlock.c
+-rw-r--r--   0        0        0    90522 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/common.c
+-rw-r--r--   0        0        0     9450 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dlist.c
+-rw-r--r--   0        0        0     4604 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dnaseq.c
+-rw-r--r--   0        0        0    29952 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dnautil.c
+-rw-r--r--   0        0        0     7156 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dystring.c
+-rw-r--r--   0        0        0    12046 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/errAbort.c
+-rw-r--r--   0        0        0     3932 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/errCatch.c
+-rw-r--r--   0        0        0    15611 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/fa.c
+-rw-r--r--   0        0        0     3714 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/ffAli.c
+-rw-r--r--   0        0        0    10802 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/ffAliHelp.c
+-rw-r--r--   0        0        0     4868 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/ffScore.c
+-rw-r--r--   0        0        0    40189 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/fuzzyFind.c
+-rw-r--r--   0        0        0    70461 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/genoFind.c
+-rw-r--r--   0        0        0    52425 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfBlatLib.c
+-rw-r--r--   0        0        0     6363 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfClientLib.c
+-rw-r--r--   0        0        0     3845 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfInternal.c
+-rw-r--r--   0        0        0    18190 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfOut.c
+-rw-r--r--   0        0        0    22265 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/hash.c
+-rw-r--r--   0        0        0     5273 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/kxTok.c
+-rw-r--r--   0        0        0    40326 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/linefile.c
+-rw-r--r--   0        0        0     7256 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/localmem.c
+-rw-r--r--   0        0        0    15074 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/memalloc.c
+-rw-r--r--   0        0        0    12778 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/nib.c
+-rw-r--r--   0        0        0    24969 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/obscure.c
+-rw-r--r--   0        0        0    13012 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/options.c
+-rw-r--r--   0        0        0    20522 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/osunix.c
+-rw-r--r--   0        0        0    23419 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/pipeline.c
+-rw-r--r--   0        0        0    63467 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/psl.c
+-rw-r--r--   0        0        0     1203 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/servcl.c
+-rw-r--r--   0        0        0    26961 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/supStitch.c
+-rw-r--r--   0        0        0     3216 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/trans3.c
+-rw-r--r--   0        0        0    33527 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/twoBit.c
+-rw-r--r--   0        0        0    71967 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/udc.c
+-rw-r--r--   0        0        0     4255 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/verbose.c
+-rw-r--r--   0        0        0     2571 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/net/gfNet.c
+-rw-r--r--   0        0        0     8795 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/net/log.c
+-rw-r--r--   0        0        0     3052 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/parser.py
+-rw-r--r--   0        0        0        0 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/py.typed
+-rw-r--r--   0        0        0     1042 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/__init__.py
+-rw-r--r--   0        0        0    16982 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/basic.py
+-rw-r--r--   0        0        0     4680 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/client.py
+-rw-r--r--   0        0        0    10076 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/server.py
+-rw-r--r--   0        0        0     1041 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/status.py
+-rw-r--r--   0        0        0      115 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/utils.py
+-rw-r--r--   0        0        0     3431 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/utils.py
+-rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 pxblat-0.1.6/setup.py
+-rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 pxblat-0.1.6/PKG-INFO
```

### Comparing `pxblat-0.1.5/LICENSE` & `pxblat-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/README.md` & `pxblat-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 [![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)
 [![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)
 [![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)
 [![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)
 [![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)
-[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge&token=71639758-1cb2-48ed-a3b6-a79c60e568a5)](https://app.codecov.io/gh/cauliyang/pxblat)
+[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge)](https://app.codecov.io/gh/cauliyang/pxblat)
 [![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)
 [![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)
+[![release](https://img.shields.io/github/release-date/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/releases)
+[![issue](https://img.shields.io/github/issues-raw/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc)
 [![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)
+[![All Contributors](https://img.shields.io/github/all-contributors/cauliyang/pxblat?color=ee8449&style=flat-the-badge)](#contributors)
 
 ---
 
 ## 📚 Table of Contents
 
 - [📚 Table of Contents](#-table-of-contents)
 - [🔮 Features](#-features)
@@ -43,14 +46,16 @@
 - [x] parse gfserver query result
 - [x] benchmarking multi connection and original version
 - [x] test result with original version
 - [x] fix build.py to build ssl, hts, maybe libuv when install with pip
 - [ ] add tool to conda channel
 - [x] add tool to pip
 - [ ] change abort to throw exceptions
+- [ ] implement psl2sam
+- [ ] implement twobit2fa
 
 ---
 
 ## 🚀 Getting Started
 
 ```sh
 pip install pxblat
@@ -131,14 +136,25 @@
 
 ---
 
 ## 🪪 License
 
 This project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.
 
+## Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
 ---
 
 ## 🙏 Acknowledgments
 
 [📌 INSERT-DESCRIPTION]
 
 ---
```

### Comparing `pxblat-0.1.5/build.py` & `pxblat-0.1.6/build.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/pyproject.toml` & `pxblat-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxblat"
-version = "0.1.5"
+version = "0.1.6"
 description = "A native python binding for blat suit"
 authors = ["Yangyang Li <yangyang.li@northwestern.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -13,39 +13,44 @@
 setuptools = "^67.7.2"
 rich = "^13.3.5"
 pysimdjson = "^5.0.2"
 biopython = "^1.81"
 typer = "^0.9.0"
 deprecated = "^1.2.13"
 mashumaro = "^3.7"
+numpy = "^1.24.3"
 
 
 [tool.poetry.scripts]
-pxblat="pxblat.cli.cli:app"
+pxblat = "pxblat.cli.cli:app"
 
 
 [tool.ruff]
 line-length = 120
 fix = true
 extend-ignore = ["E501"]
 select = [
   # pyflakes
   "F",
   # pycodestyle
-  "E", "W",
+  "E",
+  "W",
   # flake8-2020
   "YTT",
   # flake8-bugbear
   "B",
   # flake8-quotes
   "Q",
   # flake8-debugger
   "T10",
   # pylint
-  "PLC", "PLE", "PLR", "PLW",
+  "PLC",
+  "PLE",
+  "PLR",
+  "PLW",
   # misc lints
   "PIE",
   # flake8-pyi
   "PYI",
   # tidy imports
   "TID",
   # implicit string concatenation
@@ -101,28 +106,27 @@
 [tool.coverage.run]
 branch = true
 source = ["pxblat", "tests"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 40
+ignore_errors = true
 
 
 [tool.mypy]
 strict = false
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 ignore_missing_imports = true
 
 
-
-
 [tool.poetry.build]
 script = "build.py"
-generate-setup-file=true
+generate-setup-file = true
 
 [build-system]
 requires = ["pybind11>2.9.1", "poetry-core>=1.2.0", "setuptools>=40.6.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pxblat-0.1.5/src/pxblat/cli/client.py` & `pxblat-0.1.6/src/pxblat/cli/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,15 +140,7 @@
         .withMaxIntron(maxIntron)
         .withGenome(genome)
         .withGenomeDataDir(genomeDataDir)
         .build()
     )
 
     pygfClient(client_option)
-
-    # try:
-    #     ret_decode = ret.decode().rsplit("\n", 1)[0]  # type: ignore
-    # except UnicodeDecodeError:
-    #     ret_decode = ret.decode("latin-1").rsplit("\n", 1)[0]  # type: ignore
-
-    # with outpsl.open("w") as f:
-    #     f.write(ret_decode)  # type: ignore
```

### Comparing `pxblat-0.1.5/src/pxblat/cli/fa2twobit.py` & `pxblat-0.1.6/src/pxblat/cli/fa2twobit.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/cli/server.py` & `pxblat-0.1.6/src/pxblat/cli/server.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/__init__.pyi` & `pxblat-0.1.6/src/pxblat/extc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/binder/_extc.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/binder/faToTwoBit.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/binder/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/binder/gfClient.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfClient.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/binder/gfServer.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/binder/gfServer_1.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer_1.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/binder/pygfServer.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/binder/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/bs_thread_pool.hpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/bs_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/dbg.h` & `pxblat-0.1.6/src/pxblat/extc/bindings/dbg.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/faToTwoBit.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/faToTwoBit.hpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/gfClient.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/gfClient.hpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/gfClient2.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/gfClient2.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/gfServer.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/gfServer.hpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/pygfServer.cpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/bindings/pygfServer.hpp` & `pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/blat.c` & `pxblat-0.1.6/src/pxblat/extc/blat.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/faToTwoBit.c` & `pxblat-0.1.6/src/pxblat/extc/faToTwoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/gfClient.c` & `pxblat-0.1.6/src/pxblat/extc/gfClient.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/gfServer.c` & `pxblat-0.1.6/src/pxblat/extc/gfServer.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/bandExt.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/bandExt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/base64.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/base64.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/cheapcgi.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/cheapcgi.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/filePath.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/filePath.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/gfxPoly.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/gfxPoly.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/hex.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/hex.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/htmlPage.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/htmlPage.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/htmshell.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/htmshell.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/internet.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/internet.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/kxTok.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/kxTok.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/memgfx.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/memgfx.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/mime.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/mime.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/portimpl.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/portimpl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/aux/rbTree.h` & `pxblat-0.1.6/src/pxblat/extc/include/aux/rbTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/aliType.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/aliType.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/axt.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/axt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/bPlusTree.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/bPlusTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/binRange.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/binRange.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/bits.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/bits.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/chain.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/chain.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/chainBlock.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/chainBlock.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/common.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/common.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/dlist.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/dlist.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/dnaseq.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/dnaseq.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/dnautil.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/dnautil.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/dystring.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/dystring.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/errAbort.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/errAbort.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/errCatch.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/errCatch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/fa.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/fa.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/fuzzyFind.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/fuzzyFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/genoFind.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/genoFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/gfClientLib.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/gfClientLib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/gfInternal.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/gfInternal.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/hash.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/hash.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/linefile.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/linefile.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/localmem.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/localmem.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/maf.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/maf.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/memalloc.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/memalloc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/net.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/net.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/netlib.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/netlib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/nib.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/nib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/obscure.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/obscure.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/ooc.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/ooc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/options.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/options.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/patSpace.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/patSpace.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/pipeline.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/portable.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/portable.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/psl.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/psl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/rangeTree.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/rangeTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/repMask.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/repMask.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/sig.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/sig.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/sqlList.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/sqlList.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/sqlNum.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/sqlNum.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/supStitch.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/supStitch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/trans3.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/trans3.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/twoBit.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/twoBit.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/udc.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/udc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/core/verbose.h` & `pxblat-0.1.6/src/pxblat/extc/include/core/verbose.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/include/net/log.h` & `pxblat-0.1.6/src/pxblat/extc/include/net/log.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/axt.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/axt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/bandExt.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/bandExt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/base64.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/base64.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/binRange.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/binRange.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/blastOut.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/blastOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/cheapcgi.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/cheapcgi.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/ffSeedExtend.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/ffSeedExtend.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/filePath.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/filePath.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/hex.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/hex.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/htmlPage.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/htmlPage.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/htmshell.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/htmshell.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/https.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/https.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/intExp.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/intExp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/internet.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/internet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/maf.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/maf.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/mafFromAxt.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/mafFromAxt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/mime.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/mime.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/net.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/net.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/netlib.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/netlib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/ooc.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/ooc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/patSpace.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/patSpace.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/portimpl.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/portimpl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/rangeTree.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/rangeTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/rbTree.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/rbTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/repMask.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/repMask.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/servBrcMcw.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/servBrcMcw.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/servCrunx.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/servCrunx.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/servcis.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/servcis.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/servmsII.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/servmsII.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/servpws.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/servpws.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/sqlList.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/sqlList.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/sqlNum.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/sqlNum.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/aux/wildcmp.c` & `pxblat-0.1.6/src/pxblat/extc/src/aux/wildcmp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/aliType.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/aliType.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/bPlusTree.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/bPlusTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/bits.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/bits.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/chain.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/chain.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/chainBlock.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/chainBlock.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/common.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/common.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/dlist.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/dlist.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/dnaseq.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/dnaseq.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/dnautil.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/dnautil.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/dystring.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/dystring.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/errAbort.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/errAbort.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/errCatch.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/errCatch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/fa.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/fa.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/ffAli.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/ffAli.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/ffAliHelp.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/ffAliHelp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/ffScore.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/ffScore.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/fuzzyFind.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/fuzzyFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/genoFind.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/genoFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/gfBlatLib.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/gfBlatLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/gfClientLib.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/gfClientLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/gfInternal.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/gfInternal.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/gfOut.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/gfOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/hash.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/hash.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/kxTok.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/kxTok.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/linefile.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/linefile.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/localmem.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/localmem.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/memalloc.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/memalloc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/nib.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/nib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/obscure.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/obscure.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/options.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/options.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/osunix.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/osunix.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/pipeline.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/pipeline.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/psl.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/psl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/servcl.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/servcl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/supStitch.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/supStitch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/trans3.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/trans3.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/twoBit.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/twoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/udc.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/udc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/core/verbose.c` & `pxblat-0.1.6/src/pxblat/extc/src/core/verbose.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/net/gfNet.c` & `pxblat-0.1.6/src/pxblat/extc/src/net/gfNet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/extc/src/net/log.c` & `pxblat-0.1.6/src/pxblat/extc/src/net/log.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/parser.py` & `pxblat-0.1.6/src/pxblat/parser.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/server/__init__.py` & `pxblat-0.1.6/src/pxblat/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/src/pxblat/server/basic.py` & `pxblat-0.1.6/src/pxblat/server/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,368 +1,297 @@
-import errno
-import socket
-import time
 import typing as t
-import warnings
-from collections import Counter
+from contextlib import ContextDecorator
 from multiprocessing import Process
+from pathlib import Path
+from typing import Union
 
-from deprecated import deprecated  # type: ignore
-from pxblat.extc import faToTwoBit
 from pxblat.extc import gfServerOption
-from pxblat.extc import pygetFileList
-from pxblat.extc import pyqueryServer
 from pxblat.extc import pystartServer
-from pxblat.extc import startServer
 from pxblat.extc import UsageStats
 
+from .basic import check_port_in_use
+from .basic import files
+from .basic import find_free_port
+from .basic import logger
+from .basic import server_query
+from .basic import status_server
+from .basic import stop_server
+from .basic import wait_server_ready
 from .status import Status
-from .utils import logger
 
-DEFAULT_PORT = 65000
 
-
-def check_host_port(host: str, port: int):
-    if not isinstance(host, str):
-        raise RuntimeError("host must be str")
-
-    if not isinstance(port, int):
-        raise RuntimeError("port must be number")
-
-
-def check_port_in_use(host: str, port: int = DEFAULT_PORT, tries: int = 3):
-    res = []
-    for _ in range(tries):
-        res.append(_check_port_in_use_by_connect(host, port))
-
-    counter = Counter(res)
-
-    logger.debug(f"{res}")
-
-    if counter[True] > counter[False]:
-        return True
-    else:
-        return False
-
-
-def _check_port_in_use_by_status(
-    host: str, port: int, gfserver_option: gfServerOption
-) -> bool:
-    """Check the port is in use by status_server
-
-    Args:
-        host: host name
-        port: port number
-        gfserver_option: server option for the opening server
-
-    Returns:
-        True if the port is in use
-
-    note:
-        The server option can be default value and will not influence result
-        Also, it can detect if the port is opened by gfServer as well
+def create_server_option() -> gfServerOption:
     """
-    logger.debug(f"check port {host}:{port}")
-    return check_server_status(host, port, gfserver_option)
-
-
-def _check_port_in_use_by_connect(host: str, port: int):
-    """Check the port is in use by connect to the port
-
-    Args:
-        host: host name
-        port: port number
+    Creates a new gfServerOption object with default values.
 
     Returns:
-        True if the port is in use
-
-    note:
-        The function has same feature as `_check_port_in_use_by_status`
-        It check the port if it is in use by connect to the port.
-        But it cannot detect if the port is opened by gfServer
+        gfServerOption: A new gfServerOption object with default values.
     """
-    return check_port_open(host, port)
-
+    return gfServerOption()
 
-@deprecated(
-    reason="The func will generate false alarm. Please use `_check_port_in_use_by_status` or  `_check_port_in_use_by_connect` instead"
-)
-def _check_port_in_use_by_bind(host: str, port: int = DEFAULT_PORT):
-    """Check the port is in use by bind to the port
-
-    Args:
-        host: host name
-        port: port number
 
-    Returns:
-        True if the port is in use
-
-    note:
-        The function check the port if it is in use by bind to the port.
-        It is not reliable as `_check_port_in_use_by_connect` or `_check_port_in_use_by_status`
-    """
-    logger.debug(f"check port {host}:{port}")
-    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    try:
-        s.bind((host, port))
-    except socket.error as e:
-        logger.debug(f"port {host}:{port} is in use {e}")
-        if e.errno == errno.EADDRINUSE:
-            return True
-
-        raise e
-
-    s.close()
-    return False
-
-
-def wait_server_ready(
-    host: str, port: int, timeout: int = 60, gfserver_option=None
-) -> None:
-    """
-    Wait for a server to become ready by checking if a given port is open or if a specific server status is reached.
-
-    Args:
-        host (str): The hostname or IP address of the server to check.
-        port (int): The port number to check for open status.
-        timeout (int, optional): The maximum number of seconds to wait for the server to become ready. Defaults to 60.
-        gfserver_option (str, optional): The specific server status to check for. If None, the function will check for an open port. Defaults to None.
-
-    Raises:
-        RuntimeError: If the server does not become ready within the specified timeout.
-
-    Returns:
-        None
-    """
-    start = time.perf_counter()
-
-    if gfserver_option is None:
-        warnings.warn(
-            "Use `check_server_status` instead of `check_port_open` when wait for ready",
-            stacklevel=1,
+class Server(ContextDecorator):
+    def __init__(
+        self,
+        host: str,
+        port: int,
+        two_bit: Union[Path, str],
+        option: gfServerOption,
+        daemon=True,
+        use_others: bool = False,
+        timeout: int = 60,
+        block: bool = False,
+    ):
+        """Initializes a gfServer object with the given parameters.
+
+        Args:
+            host (str): The hostname or IP address to bind the server to.
+            port (int): The port number to bind the server to.
+            two_bit (Union[Path, str]): The path to the 2bit file or the URL of the 2bit file.
+            option (gfServerOption): The options to use when starting the server.
+            daemon (bool, optional): Whether to run the server as a daemon process. Defaults to True.
+            use_others (bool, optional): Whether to allow other users to access the server. Defaults to False.
+            timeout (int, optional): The number of seconds to wait for the server to start. Defaults to 60.
+            block (bool, optional): Whether to block until the server is ready. Defaults to False.
+
+        Raises:
+            ValueError: If the given two_bit file or URL is invalid.
+            OSError: If there is an error starting the server process.
+
+        Returns:
+            None
+
+        """
+        self._host = host
+        self._port = port
+
+        self.two_bit = two_bit
+        self.option = option
+        self.stat = UsageStats()
+
+        self.use_others = use_others
+        self.timeout = timeout
+        self.daemon = daemon
+
+        self._block = block
+        self._is_ready = False
+        self._is_open = True
+        self._process = None
+
+    @property
+    def host(self):
+        return self._host
+
+    @host.setter
+    def host(self, value: str):
+        self._host = value
+
+    @property
+    def port(self) -> int:
+        return self._port
+
+    @port.setter
+    def port(self, value: int):
+        self._port = value
+
+    def _start_b(self):
+        """Start server in blocking mode."""
+        two_bit_file = (
+            self.two_bit if isinstance(self.two_bit, str) else self.two_bit.as_posix()
         )
-        while not check_port_open(host, port):
-            time.sleep(1)
-            if time.perf_counter() - start > timeout:
-                raise RuntimeError("wait for server ready timeout")
-    else:
-        while not check_server_status(host, port, gfserver_option):
-            time.sleep(1)
-            if time.perf_counter() - start > timeout:
-                raise RuntimeError("wait for server ready timeout")
-
-
-def check_server_status(
-    host: str,
-    port: int,
-    gfserver_option: gfServerOption,
-) -> bool:
-    try:
-        status_server(host, port, gfserver_option)
-    except ConnectionRefusedError:
-        return False
-    else:
-        return True
-
-
-def check_port_open(host: str, port: int) -> bool:
-    """Check the port is open and can accept message or not.
-
-    Args:
-        host: Hostname
-        port: Port number
-
-    Returns:
-        True if the port is open and can accept message, otherwise False.
-    """
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        return s.connect_ex((host, port)) == 0
-
-
-def gfSignature() -> str:
-    return "0ddf270562684f29"
-
+        try:
+            if check_port_in_use(self.host, self.port):
+                if self.use_others:
+                    self._is_open = False
+                    # WARN: Use server that is already open. However, the server may be not opened by gfServer <05-16-23>
+                    # Hence, the `wait_server_ready` may be timeout.
+
+                    # wait_server_ready(host, port, timeout)
+                else:
+                    self._is_open = True
+                    new_port = find_free_port(self.host, start=self.port + 1)
+                    self.port = new_port
+                    pystartServer(
+                        self.host,
+                        str(self.port),
+                        1,
+                        [two_bit_file],
+                        self.option,
+                        self.stat,
+                    )
+            else:
+                pystartServer(
+                    self.host, str(self.port), 1, [two_bit_file], self.option, self.stat
+                )
+        except Exception as e:
+            raise e
 
-def fa_to_two_bit(
-    inFiles: t.List[str],
-    outFile: str,
-    noMask: bool = False,
-    stripVersion: bool = False,
-    ignoreDups: bool = False,
-    useLong: bool = False,
-):
-    return faToTwoBit(inFiles, outFile, noMask, stripVersion, ignoreDups, useLong)
-
-
-def status_server(
-    host: str, port: int, options: gfServerOption, instance=False
-) -> t.Union[Status, t.Dict[str, str]]:
-    if not options.genome:
-        message = f"{gfSignature()}status".encode()
-    else:
-        temp = "transInfo" if options.trans else "untransInfo"
-        message = (
-            f"{gfSignature()}{temp} {options.genome} {options.genomeDataDir}".encode()
+    def _start_nb(self):
+        two_bit_file = (
+            self.two_bit if isinstance(self.two_bit, str) else self.two_bit.as_posix()
         )
-
-    data = b""
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        s.connect((host, port))
-        s.sendall(message)
-        while True:
-            data += s.recv(1024)
-            if b"end" in data:
-                break
-
-        mapping = {
-            b"\x00": b"\n",
-            b"\x03": b"\n",
-            b"\x04": b"\n",
-            b"\x07": b"\n",
-            b"\x08": b"\n",
-            b"\x11": b"\n",
-            b"\x10": b"\n",
-            b"\x0b": b"\n",
-            b"\x0c": b"\n",
-            b"\x0e": b"\n",
-            b"\x0f": b"\n",
-            b"\t": b"\n",
-            b"end": b"",
-        }
-
-    for k, v in mapping.items():
-        data = data.replace(k, v)
-
-    data_dict = {
-        " ".join(line.split()[:-1]): line.split()[-1]
-        for line in data.decode("utf-8").strip().split("\n")
-    }
-
-    if instance:
-        return Status.from_dict(data_dict)
-
-    return data_dict
-
-
-def stop_server(host: str, port: int):
-    message = f"{gfSignature()}quit".encode()
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        s.connect((host, port))
-        s.sendall(message)
-
-
-def files(host: str, port: int) -> list[str]:
-    ret_str = pygetFileList(host, str(port))
-    assert ret_str, "ret_str cannot be empty"
-    return [file for file in ret_str.split("\n") if file]
-
-
-def server_query(
-    intype: str, host: str, port: int, faName: str, isComplex: bool, isProt: bool
-):
-    re_str = pyqueryServer(intype, host, str(port), faName, isComplex, isProt)
-    return re_str
-
-
-def start_server(
-    host: str,
-    port: int,
-    two_bit_file: str,
-    option: gfServerOption,
-    stat: UsageStats,
-):
-    return startServer(host, str(port), 1, [two_bit_file], option, stat)
-
-
-def start_server_mt(
-    host: str,
-    port: int,
-    two_bit_file: str,
-    option: gfServerOption,
-    stat: UsageStats,
-    use_others: bool = False,
-    timeout: int = 60,
-    try_new_port: bool = True,
-):
-    """Start server in blocking mode.
-
-    Args:
-        host: host name
-        port: port number
-        two_bit_file: two bit file path
-        option: gfServeoption
-        stat: statastic for server
-    """
-    try:
-        if check_port_in_use(host, port):
-            if use_others:
-                pass
-                # wait_server_ready(host, port, timeout)
-                # status_server(host, port, option)
-            elif try_new_port:
-                port = find_free_port(host, start=port + 1)
-                pystartServer(host, str(port), 1, [two_bit_file], option, stat)
+        try:
+            if check_port_in_use(self.host, self.port):
+                logger.debug(f"{self.port} port in use")
+                if self.use_others:
+                    self._is_open = False
+                    # wait_server_ready(host, port, timeout)
+                else:
+                    self._is_open = True
+                    new_port = find_free_port(self._host, start=self.port + 1)
+                    self.port = new_port
+                    self._process = Process(
+                        target=pystartServer,
+                        args=(
+                            self.host,
+                            str(self.port),
+                            1,
+                            [two_bit_file],
+                            self.option,
+                            self.stat,
+                        ),
+                        daemon=self.daemon,
+                    )
             else:
-                raise ValueError(f"The port {port} is used")
-        else:
-            pystartServer(host, str(port), 1, [two_bit_file], option, stat)
-    except Exception as e:
-        raise e
-
-
-def start_server_mt_nb(
-    host: str,
-    port: int,
-    two_bit_file: str,
-    option: gfServerOption,
-    stat: UsageStats,
-    use_others: bool = False,
-    timeout: int = 60,
-    try_new_port: bool = True,
-) -> Process:
-    """Start server in non-blocking mode.
-
-    Args:
-        host: host name
-        port: port number
-        two_bit_file: two bit file path
-        option: gfServeoption
-        stat: statastic for server
-
-    Returns:
-        Process: a process object
-    """
-    process = Process(
-        target=start_server_mt,
-        args=(
-            host,
-            port,
-            two_bit_file,
-            option,
-            stat,
-            use_others,
-            timeout,
-            try_new_port,
-        ),
-        daemon=True,
-    )
+                self._is_open = True
+                logger.debug(f"{self.port} port not in use")
+                self._process = Process(
+                    target=pystartServer,
+                    args=(
+                        self.host,
+                        str(self.port),
+                        1,
+                        [two_bit_file],
+                        self.option,
+                        self.stat,
+                    ),
+                    daemon=self.daemon,
+                )
+        except Exception as e:
+            raise e
 
-    process.start()
-    return process
+        else:
+            if self._process is not None:
+                self._process.start()
 
+    def start(self):
+        """
+        Starts the gfServer instance in either blocking or non-blocking mode.
+
+        If the server is set to non-blocking mode, it will start the server in a separate process.
+        If the server is set to blocking mode, it will start the server in the current process.
+        """
+        if not self._block:
+            self._start_nb()
+        else:
+            self._start_b()
 
-def find_free_port(host: str, start: int = DEFAULT_PORT, end: int = 65535) -> int:
-    """Find an available port in the range of [start, end].
-    Args:
-        host: Hostname
-        start: Start port number
-        end: End port number
-    """
-    assert start < end
+    def stop(self):
+        """
+        Stops the gfServer instance if it is running.
+
+        This method sends a stop signal to the server process, causing it to terminate gracefully.
+        """
+        if self._is_open:
+            stop_server(self.host, self.port)
+
+    def status(self, instance=False) -> t.Union[t.Dict[str, str], Status]:
+        """
+        Retrieves the status of the gfServer instance.
+
+        Args:
+            instance (bool, optional): If True, returns a Status object. If False, returns a dictionary with status information. Defaults to False.
+
+        Returns:
+            t.Union[t.Dict[str, str], Status]: The status of the gfServer instance, either as a dictionary or a Status object.
+        """
+        return status_server(self.host, self.port, self.option, instance=instance)
+
+    def files(self) -> list[str]:
+        """
+        Retrieves the list of files served by the gfServer instance.
+
+        Returns:
+            list[str]: A list of file names served by the gfServer instance.
+        """
+        return files(self.host, self.port)
+
+    def query(self, intype: str, faName: str, isComplex: bool, isProt: bool) -> str:
+        """
+        Queries the gfServer instance with the given parameters.
+
+        Args:
+            intype (str): The type of input sequence. Must be one of "dna", "rna", or "protein".
+            faName (str): The name of the input sequence.
+            isComplex (bool): Whether the input sequence is complex.
+            isProt (bool): Whether the input sequence is a protein sequence.
+
+        Returns:
+            str: The result of the query as a string.
+        """
+        return server_query(intype, self.host, self.port, faName, isComplex, isProt)
+
+    def is_ready(self) -> bool:
+        """
+        Returns True if the server is ready to accept queries, False otherwise.
+
+        Returns:
+            bool: True if the server is ready to accept queries, False otherwise.
+        """
+        return self._is_ready
+
+    def is_open(self) -> bool:
+        """
+        Returns True if the server is open, False otherwise.
+
+        Returns:
+            bool: True if the server is open, False otherwise.
+        """
+        return self._is_open
+
+    def wait_ready(self, timeout: int = 60, restart: bool = False):
+        """Wait server ready in block mode.
+
+        Args:
+            timeout: Timeout for wait server ready.
+            restart: If timeout, restart server and wait again.
+
+        Raises:
+            RuntimeError: If server is not opened by gfServer or the server takes longer time to be ready, the `wait_server_ready` may be timeout.
+            If `restart` is True, the server will be restarted and wait again.
+        """
+        if not self._is_ready:
+            try:
+                wait_server_ready(self.host, self.port, timeout, self.option)
+            except RuntimeError as e:
+                if restart and self.use_others:
+                    self.use_others = False
+                    self.start()
+                    self.wait_ready(timeout * 2, restart)
+                else:
+                    raise RuntimeError(
+                        f"Timeout for Waitting for {self.host} {self.port} server ready due to server is not opened by gfServer or need longer time to wait"
+                    ) from e
+            else:
+                self._is_ready = True
 
-    for port in range(start, end):
-        try:
-            if not check_port_in_use(host, port):
-                return port
-        except socket.error as e:
-            raise e
-    raise RuntimeError(f"Cannot find available port in range [{start}, {end}]")
+    @classmethod
+    def create_option(cls):
+        """
+        Creates a dictionary of options for the gfServer instance.
+
+        Returns:
+            dict: A dictionary of options for the gfServer instance.
+        """
+        return create_server_option()
+
+    def __str__(self):
+        return f"Server({self.host}, {self.port}, ready: {self.is_ready()} open: {self.is_open()} {self.option})"
+
+    def __enter__(self):
+        print("start server")
+        self.start()
+        return self
+
+    def __exit__(self, *exc):
+        print("stop server")
+        self.stop()
```

### Comparing `pxblat-0.1.5/src/pxblat/server/status.py` & `pxblat-0.1.6/src/pxblat/server/status.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from mashumaro import DataClassDictMixin  # type: ignore
 from mashumaro import field_options  # type: ignore
 from mashumaro.mixins.json import DataClassJSONMixin  # type: ignore
 
 
 @dataclass
 class Status(DataClassJSONMixin, DataClassDictMixin):
+    """This class represents the status of a server.
+    It contains information about the server's version, type, host, port, tile size, step size, minimum match,
+    PCR requests, BLAT requests, number of bases, number of misses, number of no signals, number of trimmed reads,
+    and number of warnings.
+    """
+
     version: str
     serverType: str
     types: str = field(metadata=field_options(alias="type"))
     host: str
     port: int
     tileSize: int
     stepSize: int
```

### Comparing `pxblat-0.1.5/src/pxblat/utils.py` & `pxblat-0.1.6/src/pxblat/utils.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.5/setup.py` & `pxblat-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,28 +21,29 @@
                  'src/net/*']}
 
 install_requires = \
 ['biopython>=1.81,<2.0',
  'deprecated>=1.2.13,<2.0.0',
  'loguru>=0.7.0,<0.8.0',
  'mashumaro>=3.7,<4.0',
+ 'numpy>=1.24.3,<2.0.0',
  'pybind11>=2.10.4,<3.0.0',
  'pysimdjson>=5.0.2,<6.0.0',
  'rich>=13.3.5,<14.0.0',
  'setuptools>=67.7.2,<68.0.0',
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['pxblat = pxblat.cli.cli:app']}
 
 setup_kwargs = {
     'name': 'pxblat',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A native python binding for blat suit',
-    'long_description': "# PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT\n\n[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)\n[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)\n[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)\n[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)\n[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)\n[![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge&token=71639758-1cb2-48ed-a3b6-a79c60e568a5)](https://app.codecov.io/gh/cauliyang/pxblat)\n[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)\n[![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)\n[![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)\n\n---\n\n## 📚 Table of Contents\n\n- [📚 Table of Contents](#-table-of-contents)\n- [🔮 Features](#-features)\n- [🏎💨 Getting Started](#-getting-started)\n- [🤝 Contributing](#-contributing)\n- [\U0001faaa License](#-license)\n- [🙏 Acknowledgments](#-acknowledgments)\n\n---\n\n## 🔮 Features\n\n- no intermidiate files, all in memory\n- no system call\n- no need to bother with log files to get status of tool\n- no need to worry about file format\n- no other dependency\n- higher proformance and Ergonomics (compare with current blat endpoint)\n\n## To-do\n\n- [x] parser gfclient result\n- [x] parse gfserver query result\n- [x] benchmarking multi connection and original version\n- [x] test result with original version\n- [x] fix build.py to build ssl, hts, maybe libuv when install with pip\n- [ ] add tool to conda channel\n- [x] add tool to pip\n- [ ] change abort to throw exceptions\n\n---\n\n## 🚀 Getting Started\n\n```sh\npip install pxblat\n```\n\n```sh\nconda install pxblat\n```\n\n### ✅ Prerequisites\n\nBefore you begin, ensure that you have the following prerequisites installed:\n\n> `[📌  INSERT-PROJECT-PREREQUISITES]`\n\n### 💻 Installation\n\n1. Clone the pxblat repository:\n\n```sh\ngit clone https://github.com/cauliyang/pxblat.git\n```\n\n2. Change to the project directory:\n\n```sh\ncd pxblat\n```\n\n3. Install the dependencies:\n\n```sh\npoetry install\n```\n\n### 🤖 Using pxblat\n\n```sh\npxblat\n```\n\n### 🧪 Running Tests\n\n```sh\npytest\n```\n\n---\n\n## 🤝 Contributing\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```sh\ngit checkout -b new-feature-branch\n```\n\n4. Make changes to the project's codebase.\n5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.\n\n```sh\ngit commit -m 'Implemented new feature.'\n```\n\n6. Push your changes to your forked repository on GitHub using the following command\n\n```sh\ngit push origin new-feature-branch\n```\n\n7. Create a pull request to the original repository.\n   Open a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.\n   The project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n---\n\n## \U0001faaa License\n\nThis project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.\n\n---\n\n## 🙏 Acknowledgments\n\n[📌 INSERT-DESCRIPTION]\n\n---\n\n<!-- github-only -->\n",
+    'long_description': "# PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT\n\n[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)\n[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)\n[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)\n[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)\n[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)\n[![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge)](https://app.codecov.io/gh/cauliyang/pxblat)\n[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)\n[![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)\n[![release](https://img.shields.io/github/release-date/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/releases)\n[![issue](https://img.shields.io/github/issues-raw/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc)\n[![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)\n[![All Contributors](https://img.shields.io/github/all-contributors/cauliyang/pxblat?color=ee8449&style=flat-the-badge)](#contributors)\n\n---\n\n## 📚 Table of Contents\n\n- [📚 Table of Contents](#-table-of-contents)\n- [🔮 Features](#-features)\n- [🏎💨 Getting Started](#-getting-started)\n- [🤝 Contributing](#-contributing)\n- [\U0001faaa License](#-license)\n- [🙏 Acknowledgments](#-acknowledgments)\n\n---\n\n## 🔮 Features\n\n- no intermidiate files, all in memory\n- no system call\n- no need to bother with log files to get status of tool\n- no need to worry about file format\n- no other dependency\n- higher proformance and Ergonomics (compare with current blat endpoint)\n\n## To-do\n\n- [x] parser gfclient result\n- [x] parse gfserver query result\n- [x] benchmarking multi connection and original version\n- [x] test result with original version\n- [x] fix build.py to build ssl, hts, maybe libuv when install with pip\n- [ ] add tool to conda channel\n- [x] add tool to pip\n- [ ] change abort to throw exceptions\n- [ ] implement psl2sam\n- [ ] implement twobit2fa\n\n---\n\n## 🚀 Getting Started\n\n```sh\npip install pxblat\n```\n\n```sh\nconda install pxblat\n```\n\n### ✅ Prerequisites\n\nBefore you begin, ensure that you have the following prerequisites installed:\n\n> `[📌  INSERT-PROJECT-PREREQUISITES]`\n\n### 💻 Installation\n\n1. Clone the pxblat repository:\n\n```sh\ngit clone https://github.com/cauliyang/pxblat.git\n```\n\n2. Change to the project directory:\n\n```sh\ncd pxblat\n```\n\n3. Install the dependencies:\n\n```sh\npoetry install\n```\n\n### 🤖 Using pxblat\n\n```sh\npxblat\n```\n\n### 🧪 Running Tests\n\n```sh\npytest\n```\n\n---\n\n## 🤝 Contributing\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```sh\ngit checkout -b new-feature-branch\n```\n\n4. Make changes to the project's codebase.\n5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.\n\n```sh\ngit commit -m 'Implemented new feature.'\n```\n\n6. Push your changes to your forked repository on GitHub using the following command\n\n```sh\ngit push origin new-feature-branch\n```\n\n7. Create a pull request to the original repository.\n   Open a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.\n   The project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n---\n\n## \U0001faaa License\n\nThis project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\n---\n\n## 🙏 Acknowledgments\n\n[📌 INSERT-DESCRIPTION]\n\n---\n\n<!-- github-only -->\n",
     'author': 'Yangyang Li',
     'author_email': 'yangyang.li@northwestern.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pxblat-0.1.5/PKG-INFO` & `pxblat-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pxblat
-Version: 0.1.5
+Version: 0.1.6
 Summary: A native python binding for blat suit
 License: MIT
 Author: Yangyang Li
 Author-email: yangyang.li@northwestern.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: biopython (>=1.81,<2.0)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mashumaro (>=3.7,<4.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pybind11 (>=2.10.4,<3.0.0)
 Requires-Dist: pysimdjson (>=5.0.2,<6.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
@@ -30,18 +31,21 @@
 [![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)
 [![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)
 [![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)
 [![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)
 [![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)
-[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge&token=71639758-1cb2-48ed-a3b6-a79c60e568a5)](https://app.codecov.io/gh/cauliyang/pxblat)
+[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge)](https://app.codecov.io/gh/cauliyang/pxblat)
 [![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)
 [![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)
+[![release](https://img.shields.io/github/release-date/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/releases)
+[![issue](https://img.shields.io/github/issues-raw/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc)
 [![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)
+[![All Contributors](https://img.shields.io/github/all-contributors/cauliyang/pxblat?color=ee8449&style=flat-the-badge)](#contributors)
 
 ---
 
 ## 📚 Table of Contents
 
 - [📚 Table of Contents](#-table-of-contents)
 - [🔮 Features](#-features)
@@ -67,14 +71,16 @@
 - [x] parse gfserver query result
 - [x] benchmarking multi connection and original version
 - [x] test result with original version
 - [x] fix build.py to build ssl, hts, maybe libuv when install with pip
 - [ ] add tool to conda channel
 - [x] add tool to pip
 - [ ] change abort to throw exceptions
+- [ ] implement psl2sam
+- [ ] implement twobit2fa
 
 ---
 
 ## 🚀 Getting Started
 
 ```sh
 pip install pxblat
@@ -155,14 +161,25 @@
 
 ---
 
 ## 🪪 License
 
 This project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.
 
+## Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
 ---
 
 ## 🙏 Acknowledgments
 
 [📌 INSERT-DESCRIPTION]
 
 ---
```

