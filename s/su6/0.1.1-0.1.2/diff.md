# Comparing `tmp/su6-0.1.1.tar.gz` & `tmp/su6-0.1.2.tar.gz`

## Comparing `su6-0.1.1.tar` & `su6-0.1.2.tar`

### file list

```diff
@@ -1,607 +1,608 @@
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 su6-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/locale.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/locale.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    39910 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45562 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182278 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27933 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94562 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175685 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112532 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/__about__.data.json
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/__about__.meta.json
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/__init__.data.json
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/__init__.meta.json
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/cli.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/cli.meta.json
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/core.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/su6_checker/core.meta.json
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/tests/__init__.data.json
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/tests/__init__.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    59399 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33728 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.1.1/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.1/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 su6-0.1.1/src/su6_checker/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 su6-0.1.1/src/su6_checker/__init__.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 su6-0.1.1/src/su6_checker/cli.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 su6-0.1.1/src/su6_checker/core.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6-0.1.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 su6-0.1.1/README.md
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 su6-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 su6-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/locale.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/locale.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    39910 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45562 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182278 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27933 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94562 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175685 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112532 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/__about__.data.json
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/__about__.meta.json
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/__init__.data.json
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/__init__.meta.json
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/cli.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/cli.meta.json
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/core.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/su6_checker/core.meta.json
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/tests/__init__.data.json
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/tests/__init__.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    59399 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33728 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.1.2/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.1.2/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 su6-0.1.2/src/su6_checker/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 su6-0.1.2/src/su6_checker/__init__.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 su6-0.1.2/src/su6_checker/cli.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 su6-0.1.2/src/su6_checker/core.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 su6-0.1.2/README.md
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 su6-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-0.1.2/PKG-INFO
```

### Comparing `su6-0.1.1/.mypy_cache/3.11/__future__.data.json` & `su6-0.1.2/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/__future__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_ast.data.json` & `su6-0.1.2/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_ast.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_codecs.data.json` & `su6-0.1.2/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_codecs.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_collections_abc.data.json` & `su6-0.1.2/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_csv.data.json` & `su6-0.1.2/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_csv.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_ctypes.data.json` & `su6-0.1.2/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_ctypes.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_decimal.data.json` & `su6-0.1.2/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_decimal.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_operator.data.json` & `su6-0.1.2/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_operator.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_random.data.json` & `su6-0.1.2/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_random.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_stat.data.json` & `su6-0.1.2/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_stat.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_thread.data.json` & `su6-0.1.2/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_thread.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_warnings.data.json` & `su6-0.1.2/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_warnings.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_weakref.data.json` & `su6-0.1.2/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_weakref.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_weakrefset.data.json` & `su6-0.1.2/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/abc.data.json` & `su6-0.1.2/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/abc.meta.json` & `su6-0.1.2/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/argparse.data.json` & `su6-0.1.2/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/argparse.meta.json` & `su6-0.1.2/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/array.data.json` & `su6-0.1.2/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/array.meta.json` & `su6-0.1.2/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/ast.data.json` & `su6-0.1.2/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/ast.meta.json` & `su6-0.1.2/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/builtins.data.json` & `su6-0.1.2/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/builtins.meta.json` & `su6-0.1.2/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/codecs.data.json` & `su6-0.1.2/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/codecs.meta.json` & `su6-0.1.2/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/colorsys.data.json` & `su6-0.1.2/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/colorsys.meta.json` & `su6-0.1.2/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/configparser.data.json` & `su6-0.1.2/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/configparser.meta.json` & `su6-0.1.2/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/contextlib.data.json` & `su6-0.1.2/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/contextlib.meta.json` & `su6-0.1.2/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/copy.data.json` & `su6-0.1.2/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/copy.meta.json` & `su6-0.1.2/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/csv.data.json` & `su6-0.1.2/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/csv.meta.json` & `su6-0.1.2/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/dataclasses.data.json` & `su6-0.1.2/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/dataclasses.meta.json` & `su6-0.1.2/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/datetime.data.json` & `su6-0.1.2/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/datetime.meta.json` & `su6-0.1.2/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/decimal.data.json` & `su6-0.1.2/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/decimal.meta.json` & `su6-0.1.2/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/difflib.data.json` & `su6-0.1.2/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/difflib.meta.json` & `su6-0.1.2/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/dis.data.json` & `su6-0.1.2/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/dis.meta.json` & `su6-0.1.2/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/enum.data.json` & `su6-0.1.2/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/enum.meta.json` & `su6-0.1.2/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/errno.data.json` & `su6-0.1.2/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/errno.meta.json` & `su6-0.1.2/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/fractions.data.json` & `su6-0.1.2/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/fractions.meta.json` & `su6-0.1.2/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/functools.data.json` & `su6-0.1.2/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/functools.meta.json` & `su6-0.1.2/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/genericpath.data.json` & `su6-0.1.2/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/genericpath.meta.json` & `su6-0.1.2/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/getpass.data.json` & `su6-0.1.2/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/getpass.meta.json` & `su6-0.1.2/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/gettext.data.json` & `su6-0.1.2/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/gettext.meta.json` & `su6-0.1.2/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/glob.data.json` & `su6-0.1.2/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/glob.meta.json` & `su6-0.1.2/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/inspect.data.json` & `su6-0.1.2/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/inspect.meta.json` & `su6-0.1.2/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/io.data.json` & `su6-0.1.2/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/io.meta.json` & `su6-0.1.2/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/itertools.data.json` & `su6-0.1.2/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/itertools.meta.json` & `su6-0.1.2/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/linecache.data.json` & `su6-0.1.2/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/linecache.meta.json` & `su6-0.1.2/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/locale.data.json` & `su6-0.1.2/.mypy_cache/3.11/locale.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/locale.meta.json` & `su6-0.1.2/.mypy_cache/3.11/locale.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/marshal.data.json` & `su6-0.1.2/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/marshal.meta.json` & `su6-0.1.2/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/math.data.json` & `su6-0.1.2/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/math.meta.json` & `su6-0.1.2/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mmap.data.json` & `su6-0.1.2/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mmap.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/msvcrt.data.json` & `su6-0.1.2/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/msvcrt.meta.json` & `su6-0.1.2/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/numbers.data.json` & `su6-0.1.2/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/numbers.meta.json` & `su6-0.1.2/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/opcode.data.json` & `su6-0.1.2/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/opcode.meta.json` & `su6-0.1.2/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/operator.data.json` & `su6-0.1.2/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/operator.meta.json` & `su6-0.1.2/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pathlib.data.json` & `su6-0.1.2/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pathlib.meta.json` & `su6-0.1.2/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pickle.data.json` & `su6-0.1.2/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pickle.meta.json` & `su6-0.1.2/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/platform.data.json` & `su6-0.1.2/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/platform.meta.json` & `su6-0.1.2/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/posixpath.data.json` & `su6-0.1.2/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/posixpath.meta.json` & `su6-0.1.2/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pty.data.json` & `su6-0.1.2/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pty.meta.json` & `su6-0.1.2/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pydoc.data.json` & `su6-0.1.2/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/pydoc.meta.json` & `su6-0.1.2/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/random.data.json` & `su6-0.1.2/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/random.meta.json` & `su6-0.1.2/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/re.data.json` & `su6-0.1.2/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/re.meta.json` & `su6-0.1.2/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/reprlib.data.json` & `su6-0.1.2/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/reprlib.meta.json` & `su6-0.1.2/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/shlex.data.json` & `su6-0.1.2/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/shlex.meta.json` & `su6-0.1.2/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/shutil.data.json` & `su6-0.1.2/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/shutil.meta.json` & `su6-0.1.2/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sre_compile.data.json` & `su6-0.1.2/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sre_compile.meta.json` & `su6-0.1.2/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sre_constants.data.json` & `su6-0.1.2/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sre_constants.meta.json` & `su6-0.1.2/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sre_parse.data.json` & `su6-0.1.2/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sre_parse.meta.json` & `su6-0.1.2/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/stat.data.json` & `su6-0.1.2/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/stat.meta.json` & `su6-0.1.2/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/string.data.json` & `su6-0.1.2/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/string.meta.json` & `su6-0.1.2/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/subprocess.data.json` & `su6-0.1.2/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/subprocess.meta.json` & `su6-0.1.2/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sys.data.json` & `su6-0.1.2/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/sys.meta.json` & `su6-0.1.2/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/tempfile.data.json` & `su6-0.1.2/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/tempfile.meta.json` & `su6-0.1.2/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/termios.data.json` & `su6-0.1.2/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/termios.meta.json` & `su6-0.1.2/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/textwrap.data.json` & `su6-0.1.2/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/textwrap.meta.json` & `su6-0.1.2/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/threading.data.json` & `su6-0.1.2/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/threading.meta.json` & `su6-0.1.2/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/time.data.json` & `su6-0.1.2/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/time.meta.json` & `su6-0.1.2/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/traceback.data.json` & `su6-0.1.2/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/traceback.meta.json` & `su6-0.1.2/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/tty.data.json` & `su6-0.1.2/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/tty.meta.json` & `su6-0.1.2/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/types.data.json` & `su6-0.1.2/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/types.meta.json` & `su6-0.1.2/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typing.data.json` & `su6-0.1.2/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typing.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typing_extensions.data.json` & `su6-0.1.2/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/uuid.data.json` & `su6-0.1.2/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/uuid.meta.json` & `su6-0.1.2/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/warnings.data.json` & `su6-0.1.2/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/warnings.meta.json` & `su6-0.1.2/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/weakref.data.json` & `su6-0.1.2/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/weakref.meta.json` & `su6-0.1.2/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/webbrowser.data.json` & `su6-0.1.2/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/webbrowser.meta.json` & `su6-0.1.2/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/zlib.data.json` & `su6-0.1.2/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/zlib.meta.json` & `su6-0.1.2/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/_compat.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/_compat.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/core.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/core.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/decorators.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/decorators.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/exceptions.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/formatting.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/formatting.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/globals.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/globals.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/parser.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/parser.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/termui.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/termui.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/types.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/types.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/utils.data.json` & `su6-0.1.2/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/click/utils.meta.json` & `su6-0.1.2/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/collections/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/collections/abc.data.json` & `su6-0.1.2/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/collections/abc.meta.json` & `su6-0.1.2/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-0.1.2/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-0.1.2/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/charset.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/charset.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/errors.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/errors.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/header.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/header.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/message.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/message.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/policy.data.json` & `su6-0.1.2/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/email/policy.meta.json` & `su6-0.1.2/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/html/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/html/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/html/entities.data.json` & `su6-0.1.2/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/html/entities.meta.json` & `su6-0.1.2/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/abc.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-0.1.2/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/json/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/json/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/json/decoder.data.json` & `su6-0.1.2/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/json/decoder.meta.json` & `su6-0.1.2/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/json/encoder.data.json` & `su6-0.1.2/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/json/encoder.meta.json` & `su6-0.1.2/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/logging/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-0.1.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-0.1.2/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/os/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/os/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/os/path.data.json` & `su6-0.1.2/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/os/path.meta.json` & `su6-0.1.2/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/__main__.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_extension.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_loop.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_pick.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_stack.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_timer.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_windows.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/abc.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/abc.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/align.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/align.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/ansi.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/box.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/box.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/cells.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/cells.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/color.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/color.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/columns.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/columns.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/console.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/console.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/constrain.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/containers.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/containers.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/control.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/control.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/emoji.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/errors.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/errors.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/json.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/json.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/live.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/live.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/live_render.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/markdown.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/markup.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/markup.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/measure.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/measure.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/padding.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/padding.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/pager.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/pager.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/palette.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/palette.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/panel.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/panel.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/pretty.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/protocol.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/region.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/region.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/repr.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/repr.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/rule.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/rule.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/scope.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/scope.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/screen.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/screen.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/segment.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/segment.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/spinner.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/status.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/status.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/style.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/style.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/styled.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/styled.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/syntax.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/table.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/table.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/text.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/text.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/theme.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/theme.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/themes.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/themes.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/traceback.data.json` & `su6-0.1.2/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-0.1.2/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/__about__.data.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/__about__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/__about__.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'hash'": "'3b783f3c154061e83845163b5a94ead2f97a56cb1277ecb8de6d70383417cd06'",*

 * * "'mtime'": '1685144709'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "74d2836b8847b9f74608a35601c62e2eac7b5ff19af9624046e574917af0e26f",
+    "hash": "3b783f3c154061e83845163b5a94ead2f97a56cb1277ecb8de6d70383417cd06",
     "id": "su6_checker.__about__",
     "ignore_all": false,
     "interface_hash": "a79aa7369a97c75e7bfc1e2f3354408dc43aee52edbee9bbe45bc7e844e176b6",
-    "mtime": 1685144387,
+    "mtime": 1685144709,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/cli.data.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/cli.meta.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/core.data.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/su6_checker/core.meta.json` & `su6-0.1.2/.mypy_cache/3.11/su6_checker/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/tests/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/tests/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_typing.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/colors.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/colors.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/completion.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/completion.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/core.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/core.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/main.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/main.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/models.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/models.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/params.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/params.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/utils.data.json` & `su6-0.1.2/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/typer/utils.meta.json` & `su6-0.1.2/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-0.1.2/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-0.1.2/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/urllib/parse.data.json` & `su6-0.1.2/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-0.1.2/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-0.1.2/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.ruff_cache/content/684d0841c18787fb` & `su6-0.1.2/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.ruff_cache/content/b8d965aa2b8fd993` & `su6-0.1.2/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/.ruff_cache/content/be4a1815dbb4c4` & `su6-0.1.2/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/src/su6_checker/cli.py` & `su6-0.1.2/src/su6_checker/cli.py`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/src/su6_checker/core.py` & `su6-0.1.2/src/su6_checker/core.py`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/LICENSE.txt` & `su6-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/README.md` & `su6-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # su6-checker
 
-[![PyPI - Version](https://img.shields.io/pypi/v/su6-checker.svg)](https://pypi.org/project/su6)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6-checker.svg)](https://pypi.org/project/su6)
+[![PyPI - Version](https://img.shields.io/pypi/v/su6.svg)](https://pypi.org/project/su6)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6.svg)](https://pypi.org/project/su6)
 
 -----
 su6 (6 is pronounced as '/zɛs/' in Dutch, so 'su6' is basically 'success')  
 This package will hopefully help achieve that!
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pip install su6-checker
 ```
 
 ## Usage
+
 ```console
 su6 --help
 # or, easiest to start:
 su6 all
 ```
 
 ## License
 
 `su6-checker` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog
+
+See `CHANGELOG.md` [on GitHub](https://github.com/robinvandernoord/su6-checker/blob/master/CHANGELOG.md)
```

### Comparing `su6-0.1.1/pyproject.toml` & `su6-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `su6-0.1.1/PKG-INFO` & `su6-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python cli tool to use tools for some common code quality checks (opinionated)
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-checker#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-checker/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-checker
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -25,36 +25,42 @@
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: python-semantic-release; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # su6-checker
 
-[![PyPI - Version](https://img.shields.io/pypi/v/su6-checker.svg)](https://pypi.org/project/su6)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6-checker.svg)](https://pypi.org/project/su6)
+[![PyPI - Version](https://img.shields.io/pypi/v/su6.svg)](https://pypi.org/project/su6)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6.svg)](https://pypi.org/project/su6)
 
 -----
 su6 (6 is pronounced as '/zɛs/' in Dutch, so 'su6' is basically 'success')  
 This package will hopefully help achieve that!
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pip install su6-checker
 ```
 
 ## Usage
+
 ```console
 su6 --help
 # or, easiest to start:
 su6 all
 ```
 
 ## License
 
 `su6-checker` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog
+
+See `CHANGELOG.md` [on GitHub](https://github.com/robinvandernoord/su6-checker/blob/master/CHANGELOG.md)
```

