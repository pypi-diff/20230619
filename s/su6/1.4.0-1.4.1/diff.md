# Comparing `tmp/su6-1.4.0.tar.gz` & `tmp/su6-1.4.1.tar.gz`

## Comparing `su6-1.4.0.tar` & `su6-1.4.1.tar`

### file list

```diff
@@ -1,1456 +1,1460 @@
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 su6-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-1.4.0/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 su6-1.4.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/concurrency.data.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/concurrency.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/__init__.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/__init__.meta.json
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/cls.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/cls.meta.json
--rw-r--r--   0        0        0    28521 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/core.data.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/core.meta.json
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/errors.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/errors.meta.json
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/helpers.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/helpers.meta.json
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/postpone.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/postpone.meta.json
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/singleton.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/singleton.meta.json
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    31787 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    38285 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    17494 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    27179 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/android.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/android.meta.json
--rw-r--r--   0        0        0    42401 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/unix.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/unix.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    82219 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    25162 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    54890 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0    45733 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/plugins.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/su6/plugins.meta.json
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/__init__.meta.json
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/_compat.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/_compat.meta.json
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/_utils.meta.json
--rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/api.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/api.meta.json
--rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/container.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/container.meta.json
--rw-r--r--   0        0        0    33007 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/exceptions.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/exceptions.meta.json
--rw-r--r--   0        0        0   221620 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/items.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/items.meta.json
--rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/parser.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/parser.meta.json
--rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/source.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/source.meta.json
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_char.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_char.meta.json
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_document.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_document.meta.json
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.0/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-1.4.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-1.4.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-1.4.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 su6-1.4.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 su6-1.4.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/10595a931c3c881e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1065c8b44fadc39a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1086635a5970b925
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/10ab08017438a66a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/10c2ae33c509be23
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/11f25cfda4e2f210
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/122419b0bc04bb24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1322b93a2154c54a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/134e5e8c29726e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/13985ae090677282
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/146952ec4263c5d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/150d086b8b4de9d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/156301591af184f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1663be342a34f83
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1895bed4a0ed65d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1996a22aec44a5c0
--rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1a4449eb8b26a401
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1a4db4c4834af592
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1b0530edc3fe075e
--rw-r--r--   0        0        0    21464 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1b7872d6314f48b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1ce202f3daa889d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1cfd31ba4b0b7ef9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1dcbdc62e66ccf0e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1edace855ae3c841
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1f7ac4f892285f60
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/1fbfdffa4078f509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/20b40aca78f395e8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/219bf1f8f2938bd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/21b248d368a93ac8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/21cf950ddc412c7b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/22db1408b8f4a4b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/232d0222563916a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/23680c0655621b13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/247546336fc4bd59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/248d23bfc4586461
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/24e2ebef92fa75b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/25d9504d2b6847d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/26657ed11f8e66de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/269f98f304a03fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/28caf6cfecd38c1a
--rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/294d5a468695eb7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/29531d612e8a868a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2a383abdede299d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2a5d8d1386804aed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2a630c7d6d7faa40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2b0cdebce71424f0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2bc4a20be77b881b
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2bf27b960bc3ded1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2c189a9882594507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2c6eeab804b5c1f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2c9bbc6bae6b0f41
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2d77da04c7119543
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2e4746b83d2d1cf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2e6b6d5e70ae29db
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2e8708077cd0413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2f9e25dc2ce777cc
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/2face4e073dced28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/300f9a816018d49f
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/30e241b2876dc71f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/31813abf4ed82b53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3271e344462a0ee3
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/33004598889f4950
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/349f044f89b94587
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/34a4aaded634d537
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/34e1109d49bf09f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/356d28a11355e7a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/357e837fe90ee680
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/35ab5ee4981cdf8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/35ba35b3f04c192f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/36372ef94f8716cd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/36e48551be186a66
--rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/36f0bdaeef592d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/380a13ecd1a2af25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/38962215221b245a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/38d9da4e93811c4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/39285e72757cc499
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/399d3b28a1a1db47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3a74e1b5704e9b3f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3af645c926072f97
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3c6b70c96e832bc1
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3c7fb493febe6a55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3c9bb20c3b57bae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3ca706f99b2d38bf
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3ccdd2336c8c80e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3cf13d9d13babf93
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3db675ebeb97b2fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3e0ec316d612ddc6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3e35311bfb3345f8
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3f10d9d7687f3999
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/3f12e7a3fe46c220
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/417040cdeaa7bd81
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/429010e306ea9808
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/42f337caed884834
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/431bdba29473eca0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4536434fd84cdba5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/467fc2e82c277fd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/47affd4e531897a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/47ca38fe0242f05d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/47e54ee652d2f4c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4843e1c724479e6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/484730e7d1a4dcd9
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4880724f1f6a1ac8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/48bda5931a9eb062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/49fafbbbbadedf00
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4a63ed784e7c5ec0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4ac8c08e5b1b6650
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4b5890a0c8dc15df
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4cd4c52ee1dc7ffe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4cdd16a7f9738f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4eaf3b155fae0dfb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4f16c6852dea8eca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4f2c663677c63589
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/4fafe0dbefb778fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/50373733f4645c5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/514fb27e4aef5783
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/519ab6ce866ef11b
--rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/51de14ac05bcd5d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/529312a72d1177a1
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/534b8acecf74c47
--rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/536320baecd03af6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/538fc0618c4d4c31
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/53c0f85a3179a38f
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5436d767d06cf116
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/54637ff0aaaaf6b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/552fa1eb2057eecc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5548c3ce5fff0cca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/556b5cfaac0c49bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/55c947c0fa59929
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/568d77a0a0a64dbc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/56e83f1c5eeb3eba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/572ba1efb5bb3fd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/58240cde188220d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/584058f21d3e2fa1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/594d55ee247cbdef
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/59cfab1472b544fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5a6dc8ef65620223
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5af13ad9cc04e932
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5b8fb96822a8f127
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5b965ef6adf36c8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5badc1835a2b80e1
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5cc5d54a963753bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5da466fd7e3b19f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5e83ab1d520dc773
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5efe825a5e773b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/5fb3763e0810c38a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/62396a4dea084957
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/624348590d33bdc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6278996c2e6b2a87
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/63dbabe01e9e6756
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6550bbd98b1711bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6791fc0114ddc05
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6845ca4e0c56952b
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/68c4553df91c1f5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/69bb9ea6355c0c25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/69ffc3e7ad0aa6b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6a4adfab73a8d4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6a74d0efd6350f1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6b596d4ac1166741
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6b9f30172d33b6a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6bcca98e41cda3f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6beed9d45ff1a491
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6c989c6e4eea10bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6db20c27780d4a5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6db875fe1541793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6eab8cdd7b4ae170
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/6fc044c94dc3532a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/701212523f7b3b9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/70963c0c68bf76ac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/70bd045859d6cb20
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/70d6f3b95738758d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/729f212cc9c6cd5d
--rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/72a6612daca66426
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/72de7bec9ecb53aa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/733b2373fa4ae335
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7396a954cc3b124a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7485843a948a75b0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/755c9c217a06f932
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/76d56794deeb084d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/76fbe2af0f71bd4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/79a22043e5c16946
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/79c3fb2c81fd59a0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7a19353a5daa4a37
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7b3a1bf0b652398a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7bf45647f43eaf85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7c01d9689dd16a64
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7c37d34a0c059ec7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7c806e58272a88ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7cbc35f4e814db65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7cc3783d00621498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7dc27d897f910c11
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7e138932f0b9a1bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7eb1422c10ced038
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7eb17a25b4fa1d13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7f0f63895e369318
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/7f75cbd11ebac70a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8012caf4fb290dc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/80844117d21fe12b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/809075c58fb87c61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/80dbccb0d26b4b4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/80ded2016f4f413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/81e3edf198d6c468
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/81e6f787866d0ecf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/82ab0276d38aec9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/83a59cf9aceae1d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/83cdfb5da134b21f
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/84e2e26fc69ab274
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/84e8c31ce428d3ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/858df3976aef9624
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/868699acd08be339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/86c3e5b9f79f490f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/87a7b0840a5cf8c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/87d9b6d5e7bcb6c7
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/881c84062ed51136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/886d14b97dbd4f2e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8944dfd1b590bdd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/89c7a4d643f68517
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/89e58e5ee0d7d864
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8a0279b11d098d9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8a437c05421c6cb5
--rw-r--r--   0        0        0    20054 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8a5ec4ca9660671c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8b8acf1607bcb3f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8c34e85d573e230f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8d2f83aae152de29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8df3988e9368cbe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/8f33397e19bead30
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9019e33ca68d8935
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/902eb6f99ee41131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/906cef8208fbf28f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9080aaa3f2416b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/922bfc03482db456
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/92db151fe9967fd3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9352425265579062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/93fed7ae4120c88e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/945994955724de24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/94ffcc82bc7ee370
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/95df46a8e947b100
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9613cbbc5a7c60a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/968b32ac9319cc53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/97a72bc70808d2f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/97cbf45b388709d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/97df9d79e599f082
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/981eb70eb69fb3ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/98392e87ef3eb254
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/99d5decc6ca01825
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9a5552199a8b8bd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9bd08ae684645cf6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9c1285d5b3178abe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9cbaa57406e65f63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9d0f65e1ab7ca23
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9db15fb6e71bec4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9dda9185d48774f2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9e3b1a7c0f34103b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9e50a4d6fb3c9688
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9e558f66f216c4eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9e915e4e576201bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9ec2a872083329d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9edacb4de19eeb8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9f0f8b1c56898117
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9f2c57bc030e0b04
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/9f330edc61f02d3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a0572377dc282cac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a113f7e28da04408
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a24edf91b0bcff12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a2fe93c3bba310b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a38eff4f06853e65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a78089cbf54aff62
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a8da9d8efa986532
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a925b8cd7505ac0a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a92bb1bdda49ef61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/a943564382aec90a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/aa3f7accc1718239
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ab360402eb2d795e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ab4a97b5d68b837a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/abc8db1325696a17
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/abe0d13d37518e58
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ac5b9f591ce9edec
--rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ac8c237c67408442
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/acbc9f45cfeee4dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/acecedeb9f4dd91a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ad02b8e4575abc6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ae5a30e888e80958
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/aff288abf6945582
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b08de429bee9ce93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b2d26e3968f3c218
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b2f061a9d80cfa8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b4228843afe3d2eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b56a01688e02e5f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b5c4e8c097cbf198
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b5f69f56d932f0d1
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b6191d72e3d9a646
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b61cd4b71d14e881
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b7331c702909633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b7b1c8254943be90
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b7bcb1e4c5eea72b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b81f55dc9d767e8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b82ae772ad3347b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b89a404ae8aaa495
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b89dc34e1d21508f
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b8ab8c7df580ad75
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/b990e7d90d89db2a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ba0f74a0540d9a5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ba66feb1819b5312
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bbd87fc7f90c1f28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bd12e3fd28591ae6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bd1e909ba96cca61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bdd37795dc331d56
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bde6d6e902485336
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/bdeb811362915192
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/be5eb6e8ff99feab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/be9c428a6192e049
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/beb37e84505d7dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c0d14d0162a80714
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c10a38d72f60e675
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c121acc012633d2f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c18d3e52506df649
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c250dc207334d18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c25779f3e34a584a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c293dd30723003b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c3329258d804dff6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c40a4c8f88b65414
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c55a79e89225a078
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c62dd73faf917878
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c766d7d105d53e92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c82d4fd611732d02
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c88465e3c1dc503e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c8c7b8092b03fdd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/c9d297807d108576
--rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ca3d1e0ddece82f5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cb0e3b769b6a1727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cb2f84958966b77c
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cb326dd0ee5910c6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cbb8b9fccd8c8746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cc518cf199497e9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ccc4c37cd56e46e5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ccf15ba8d3af2d15
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cd61466cc4a76933
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ce0a51ca403a72f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ce7ae4869b72ad31
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cee8b7a480495342
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/cfa33b7a8aeb793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d085b6ebe7bb0389
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d0be3a4705e047c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d0fd170547b6bb47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d1c81941e3ef2e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d1d63b74d8d929b9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d203b8acf8460019
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d2cceb9cc8265e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d3a20b1509715554
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d551c518ebaaf23a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d5a9ce7dc11e5edc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d6b8c7cba735b946
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d825cf3987ee9f33
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d8444fda03b67f2b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d86a45eca9289fa5
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d954f2ee22d56fd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d9b321d36a255169
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/d9cd4c2a9ad4580d
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/da0cf7e13e17e6a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/da4aff17737df0c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/da94ab81ae4dffd1
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/db73ef232740be87
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/dc4a4b4b55cceada
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/dcb2ce27d1f7cc70
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/de1238012a6853f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/dec4fb820d1aee1f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/decdb847958ce882
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/dfc2e498a5736fb3
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e067c98663409f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e07d7deee3f2b1ed
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e24118b3523194dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e316b4f368a31a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e4a016e6cc51d759
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e59ac15827b7f1c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e6237a2dffed4f5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e6e7d13cd57b4fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e832a8f80eaf16d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e8ab3d919ff04fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e8cd5143f259cdce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/e98cf82519b9efc2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ea450af950172f80
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ebd9c23038b8db35
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ec04e1ad73846b2a
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ed03e948b89996b8
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ed645de094b6d7bb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/edbe26c4bd7599ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/ee965a83d6cd2aaa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f002d9727bf66a12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f1af1d1ebb07ad61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f2942d8cb87b15e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f4088198fa879c9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f41987c18d73e01d
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f4d6392808939633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f4e7c96257c9d24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f586c8a0f5c58b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f58e778cbde5b210
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f5d61064e60c404b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/f9ab84e0c6669bed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fa23c022574446ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fa2e112681e24616
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fa354595b122bf9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/faa3132a8644ec4d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fad49b925cd80258
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fb9901f753a46f52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fbd81c0d9b22b507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fd089a45384d0959
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 su6-1.4.0/.ruff_cache/content/fd17e608110a0864
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 su6-1.4.0/docs/plugins.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_2602a302b50854cf___about___py.html
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_2602a302b50854cf___init___py.html
--rw-r--r--   0        0        0   120042 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_2602a302b50854cf_cli_py.html
--rw-r--r--   0        0        0   161698 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_2602a302b50854cf_core_py.html
--rw-r--r--   0        0        0    92303 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_2602a302b50854cf_plugins_py.html
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_a44f0ac069e85531__shared_py.html
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_a44f0ac069e85531_test_about_py.html
--rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html
--rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/d_a44f0ac069e85531_test_core_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-1.4.0/htmlcov/style.css
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/bad.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/black_good_mypy_bad.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/except_pytest.toml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/fake_module.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/good.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/invalid.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/only_black.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/only_mypy.toml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/stop_after_first.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/bad.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/bad.meta.json
--rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-1.4.0/src/su6/__about__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 su6-1.4.0/src/su6/__init__.py
--rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 su6-1.4.0/src/su6/cli.py
--rw-r--r--   0        0        0    18263 2020-02-02 00:00:00.000000 su6-1.4.0/src/su6/core.py
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 su6-1.4.0/src/su6/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 su6-1.4.0/src/su6/py.typed
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-1.4.0/tests/_shared.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-1.4.0/tests/test_about.py
--rw-r--r--   0        0        0     9632 2020-02-02 00:00:00.000000 su6-1.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 su6-1.4.0/tests/test_core.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-1.4.0/tests/test_plugins.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 su6-1.4.0/tests/test_plugins_config.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-1.4.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 su6-1.4.0/README.md
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 su6-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 su6-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 su6-1.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-1.4.1/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 su6-1.4.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/concurrency.data.json
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/concurrency.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.meta.json
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.meta.json
+-rw-r--r--   0        0        0    29408 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/core.data.json
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/core.meta.json
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.meta.json
+-rw-r--r--   0        0        0    23607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.meta.json
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.meta.json
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.meta.json
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.meta.json
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    31787 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    38285 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    17494 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    27179 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    42401 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    82219 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    25162 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    54090 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0    45733 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/plugins.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/plugins.meta.json
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.meta.json
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.meta.json
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.meta.json
+-rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/api.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/api.meta.json
+-rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/container.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/container.meta.json
+-rw-r--r--   0        0        0    33007 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json
+-rw-r--r--   0        0        0   221620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/items.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/items.meta.json
+-rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.meta.json
+-rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/source.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/source.meta.json
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/10595a931c3c881e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1065c8b44fadc39a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1086635a5970b925
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/10ab08017438a66a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/10c2ae33c509be23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/11f25cfda4e2f210
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/122419b0bc04bb24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1322b93a2154c54a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/134e5e8c29726e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/13985ae090677282
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/146952ec4263c5d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/150d086b8b4de9d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/156301591af184f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1663be342a34f83
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1895bed4a0ed65d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1996a22aec44a5c0
+-rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1a4449eb8b26a401
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1a4db4c4834af592
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1b0530edc3fe075e
+-rw-r--r--   0        0        0    21464 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1b7872d6314f48b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1ce202f3daa889d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1cfd31ba4b0b7ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1dcbdc62e66ccf0e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1edace855ae3c841
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1f7ac4f892285f60
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1fbfdffa4078f509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/20b40aca78f395e8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/219bf1f8f2938bd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/21b248d368a93ac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/21cf950ddc412c7b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/22db1408b8f4a4b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/232d0222563916a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/23680c0655621b13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/247546336fc4bd59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/248d23bfc4586461
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/24e2ebef92fa75b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/25d9504d2b6847d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/26657ed11f8e66de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/269f98f304a03fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/28caf6cfecd38c1a
+-rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/294d5a468695eb7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/29531d612e8a868a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2a383abdede299d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2a5d8d1386804aed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2a630c7d6d7faa40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2b0cdebce71424f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2bc4a20be77b881b
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2bf27b960bc3ded1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2c189a9882594507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2c6eeab804b5c1f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2c9bbc6bae6b0f41
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2d77da04c7119543
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2e4746b83d2d1cf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2e6b6d5e70ae29db
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2e8708077cd0413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2f9e25dc2ce777cc
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2face4e073dced28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/300f9a816018d49f
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/30e241b2876dc71f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/31813abf4ed82b53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3271e344462a0ee3
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/33004598889f4950
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/349f044f89b94587
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/34a4aaded634d537
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/34e1109d49bf09f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/356d28a11355e7a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/357e837fe90ee680
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/35ab5ee4981cdf8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/35ba35b3f04c192f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/36372ef94f8716cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/36e48551be186a66
+-rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/36f0bdaeef592d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/380a13ecd1a2af25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/38962215221b245a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/38d9da4e93811c4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/39285e72757cc499
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/399d3b28a1a1db47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3a74e1b5704e9b3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3af645c926072f97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3c6b70c96e832bc1
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3c7fb493febe6a55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3c9bb20c3b57bae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3ca706f99b2d38bf
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3ccdd2336c8c80e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3cf13d9d13babf93
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3db675ebeb97b2fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3e0ec316d612ddc6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3e35311bfb3345f8
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3f10d9d7687f3999
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3f12e7a3fe46c220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/417040cdeaa7bd81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/429010e306ea9808
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/42f337caed884834
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/431bdba29473eca0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4536434fd84cdba5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/467fc2e82c277fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/47affd4e531897a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/47ca38fe0242f05d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/47e54ee652d2f4c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4843e1c724479e6a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/484730e7d1a4dcd9
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4880724f1f6a1ac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/48bda5931a9eb062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/49fafbbbbadedf00
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4a63ed784e7c5ec0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4ac8c08e5b1b6650
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4b5890a0c8dc15df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4cd4c52ee1dc7ffe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4cdd16a7f9738f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4eaf3b155fae0dfb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f16c6852dea8eca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f2c663677c63589
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4fafe0dbefb778fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/50373733f4645c5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/514fb27e4aef5783
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/519ab6ce866ef11b
+-rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/51de14ac05bcd5d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/529312a72d1177a1
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/534b8acecf74c47
+-rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/536320baecd03af6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/538fc0618c4d4c31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/53c0f85a3179a38f
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5436d767d06cf116
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/54637ff0aaaaf6b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/552fa1eb2057eecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5548c3ce5fff0cca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/556b5cfaac0c49bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/55c947c0fa59929
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/568d77a0a0a64dbc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/56e83f1c5eeb3eba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/572ba1efb5bb3fd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/58240cde188220d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/584058f21d3e2fa1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/594d55ee247cbdef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/59cfab1472b544fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5a6dc8ef65620223
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5af13ad9cc04e932
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5b8fb96822a8f127
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5b965ef6adf36c8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5badc1835a2b80e1
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5cc5d54a963753bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5da466fd7e3b19f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5e83ab1d520dc773
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5efe825a5e773b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5fb3763e0810c38a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/62396a4dea084957
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/624348590d33bdc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6278996c2e6b2a87
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/63dbabe01e9e6756
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6550bbd98b1711bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6791fc0114ddc05
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6845ca4e0c56952b
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/68c4553df91c1f5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/69bb9ea6355c0c25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/69ffc3e7ad0aa6b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6a4adfab73a8d4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6a74d0efd6350f1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6b596d4ac1166741
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6b9f30172d33b6a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6bcca98e41cda3f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6beed9d45ff1a491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6c989c6e4eea10bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6db20c27780d4a5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6db875fe1541793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6eab8cdd7b4ae170
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6fc044c94dc3532a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/701212523f7b3b9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/70963c0c68bf76ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/70bd045859d6cb20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/70d6f3b95738758d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/729f212cc9c6cd5d
+-rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/72a6612daca66426
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/72de7bec9ecb53aa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/733b2373fa4ae335
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7396a954cc3b124a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7485843a948a75b0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/755c9c217a06f932
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/75bb48e114159509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/76d56794deeb084d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/76fbe2af0f71bd4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/79a22043e5c16946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/79c3fb2c81fd59a0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7a19353a5daa4a37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7b3a1bf0b652398a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7bf45647f43eaf85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7c01d9689dd16a64
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7c37d34a0c059ec7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7c806e58272a88ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7cbc35f4e814db65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7cc3783d00621498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7dc27d897f910c11
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7e138932f0b9a1bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7eb1422c10ced038
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7eb17a25b4fa1d13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7f0f63895e369318
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7f75cbd11ebac70a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8012caf4fb290dc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/809075c58fb87c61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/80dbccb0d26b4b4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/80ded2016f4f413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/81e3edf198d6c468
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/81e6f787866d0ecf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/82ab0276d38aec9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/83a59cf9aceae1d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/83cdfb5da134b21f
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/84e2e26fc69ab274
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/84e8c31ce428d3ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/858df3976aef9624
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/868699acd08be339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/86c3e5b9f79f490f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/87a7b0840a5cf8c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/87d9b6d5e7bcb6c7
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/881c84062ed51136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/886d14b97dbd4f2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8944dfd1b590bdd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/89c7a4d643f68517
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/89e58e5ee0d7d864
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8a0279b11d098d9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8a437c05421c6cb5
+-rw-r--r--   0        0        0    20054 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8a5ec4ca9660671c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8b8acf1607bcb3f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8c34e85d573e230f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8d2f83aae152de29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8df3988e9368cbe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8f33397e19bead30
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9019e33ca68d8935
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/902eb6f99ee41131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/906cef8208fbf28f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9080aaa3f2416b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/922bfc03482db456
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/92db151fe9967fd3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9352425265579062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/93fed7ae4120c88e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/945994955724de24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/94ffcc82bc7ee370
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/95df46a8e947b100
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9613cbbc5a7c60a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/968b32ac9319cc53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/97a72bc70808d2f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/97cbf45b388709d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/97df9d79e599f082
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/981eb70eb69fb3ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/98392e87ef3eb254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/99d5decc6ca01825
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9a5552199a8b8bd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9bd08ae684645cf6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9c1285d5b3178abe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9cbaa57406e65f63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9d0f65e1ab7ca23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9db15fb6e71bec4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9dda9185d48774f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e3b1a7c0f34103b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e50a4d6fb3c9688
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e558f66f216c4eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e915e4e576201bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9ec2a872083329d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9edacb4de19eeb8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9f0f8b1c56898117
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9f2c57bc030e0b04
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9f330edc61f02d3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a0572377dc282cac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a113f7e28da04408
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a24edf91b0bcff12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a2fe93c3bba310b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a38eff4f06853e65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a78089cbf54aff62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a8da9d8efa986532
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a925b8cd7505ac0a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a92bb1bdda49ef61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a943564382aec90a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/aa3f7accc1718239
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ab360402eb2d795e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ab4a97b5d68b837a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/abc8db1325696a17
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/abe0d13d37518e58
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ac5b9f591ce9edec
+-rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ac8c237c67408442
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/acbc9f45cfeee4dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/acecedeb9f4dd91a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ad02b8e4575abc6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ae5a30e888e80958
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/aff288abf6945582
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b08de429bee9ce93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b2d26e3968f3c218
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b2f061a9d80cfa8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b4228843afe3d2eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b56a01688e02e5f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b5c4e8c097cbf198
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b5f69f56d932f0d1
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b6191d72e3d9a646
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b61cd4b71d14e881
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b7331c702909633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b7b1c8254943be90
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b7bcb1e4c5eea72b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b81f55dc9d767e8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b82ae772ad3347b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b89a404ae8aaa495
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b89dc34e1d21508f
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b8ab8c7df580ad75
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b990e7d90d89db2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ba0f74a0540d9a5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ba66feb1819b5312
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bbd87fc7f90c1f28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bd12e3fd28591ae6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bd1e909ba96cca61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bdd37795dc331d56
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bde6d6e902485336
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bdeb811362915192
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/be5eb6e8ff99feab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/be9c428a6192e049
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/beb37e84505d7dd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c0d14d0162a80714
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c10a38d72f60e675
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c121acc012633d2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c18d3e52506df649
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c250dc207334d18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c25779f3e34a584a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c293dd30723003b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c3329258d804dff6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c40a4c8f88b65414
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c55a79e89225a078
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c62dd73faf917878
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c766d7d105d53e92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c82d4fd611732d02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c88465e3c1dc503e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c8c7b8092b03fdd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c9d297807d108576
+-rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ca3d1e0ddece82f5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cb0e3b769b6a1727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cb2f84958966b77c
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cb326dd0ee5910c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cbb8b9fccd8c8746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cc518cf199497e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ccc4c37cd56e46e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ccf15ba8d3af2d15
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cd61466cc4a76933
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ce0a51ca403a72f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ce7ae4869b72ad31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cee8b7a480495342
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cfa33b7a8aeb793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d085b6ebe7bb0389
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d0be3a4705e047c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d0fd170547b6bb47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d1c81941e3ef2e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d1d63b74d8d929b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d203b8acf8460019
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d2cceb9cc8265e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d3a20b1509715554
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d551c518ebaaf23a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d5a9ce7dc11e5edc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d6b8c7cba735b946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d825cf3987ee9f33
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d8444fda03b67f2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d86a45eca9289fa5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d9198ab6e1ae45a0
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d954f2ee22d56fd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d9b321d36a255169
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d9cd4c2a9ad4580d
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/da0cf7e13e17e6a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/da4aff17737df0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/da94ab81ae4dffd1
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/db73ef232740be87
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dc4a4b4b55cceada
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dcb2ce27d1f7cc70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/de1238012a6853f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dec4fb820d1aee1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/decdb847958ce882
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dfc2e498a5736fb3
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e067c98663409f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e07d7deee3f2b1ed
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e24118b3523194dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e316b4f368a31a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e4a016e6cc51d759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e59ac15827b7f1c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e6237a2dffed4f5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e6e7d13cd57b4fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e832a8f80eaf16d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e8ab3d919ff04fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e8cd5143f259cdce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e98cf82519b9efc2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ea450af950172f80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ebd9c23038b8db35
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ec04e1ad73846b2a
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ed03e948b89996b8
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ed645de094b6d7bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/edbe26c4bd7599ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ee965a83d6cd2aaa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f002d9727bf66a12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f1af1d1ebb07ad61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f2942d8cb87b15e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f4088198fa879c9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f41987c18d73e01d
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f4d6392808939633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f4e7c96257c9d24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f586c8a0f5c58b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f58e778cbde5b210
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f5d61064e60c404b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f9ab84e0c6669bed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fa23c022574446ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fa2e112681e24616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fa354595b122bf9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/faa3132a8644ec4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fad49b925cd80258
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fb9901f753a46f52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fbd81c0d9b22b507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fd089a45384d0959
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fd17e608110a0864
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 su6-1.4.1/docs/plugins.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf___about___py.html
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf___init___py.html
+-rw-r--r--   0        0        0   120042 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf_cli_py.html
+-rw-r--r--   0        0        0   161698 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf_core_py.html
+-rw-r--r--   0        0        0    92303 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf_plugins_py.html
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531__shared_py.html
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_about_py.html
+-rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_cli_py.html
+-rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_core_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/style.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/bad.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/black_good_mypy_bad.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/empty.toml
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/except_pytest.toml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/fake_module.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/good.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/invalid.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/only_black.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/only_mypy.toml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/stop_after_first.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.meta.json
+-rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/__about__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/__init__.py
+-rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/cli.py
+-rw-r--r--   0        0        0    17551 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/core.py
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/py.typed
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-1.4.1/tests/_shared.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_about.py
+-rw-r--r--   0        0        0     9632 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_core.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_plugins.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_plugins_config.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-1.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 su6-1.4.1/README.md
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 su6-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 su6-1.4.1/PKG-INFO
```

### Comparing `su6-1.4.0/CHANGELOG.md` & `su6-1.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.1 (2023-06-19)
+
+### Fix
+
+* **config:** Use .update functionality from `configuraptor`. ([`aa09931`](https://github.com/robinvandernoord/su6-checker/commit/aa0993167e42d878689723a9d337bdc244082914))
+
 ## v1.4.0 (2023-06-15)
 
 ### Feature
 
 * **json:** Allow json-indent via tool config ([`f4f353c`](https://github.com/robinvandernoord/su6-checker/commit/f4f353cab028cdc37707051f4be829d4f1426fb0))
 
 ## v1.3.2 (2023-06-15)
```

### Comparing `su6-1.4.0/coverage.svg` & `su6-1.4.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/__future__.data.json` & `su6-1.4.1/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/__future__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_ast.data.json` & `su6-1.4.1/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_ast.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_codecs.data.json` & `su6-1.4.1/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_codecs.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_collections_abc.data.json` & `su6-1.4.1/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_csv.data.json` & `su6-1.4.1/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_csv.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_ctypes.data.json` & `su6-1.4.1/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_ctypes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_decimal.data.json` & `su6-1.4.1/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_decimal.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_operator.data.json` & `su6-1.4.1/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_operator.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_random.data.json` & `su6-1.4.1/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_random.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_socket.data.json` & `su6-1.4.1/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_socket.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_stat.data.json` & `su6-1.4.1/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_stat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_thread.data.json` & `su6-1.4.1/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_thread.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_warnings.data.json` & `su6-1.4.1/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_warnings.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_weakref.data.json` & `su6-1.4.1/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_weakref.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_weakrefset.data.json` & `su6-1.4.1/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/abc.data.json` & `su6-1.4.1/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/abc.meta.json` & `su6-1.4.1/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/argparse.data.json` & `su6-1.4.1/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/argparse.meta.json` & `su6-1.4.1/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/array.data.json` & `su6-1.4.1/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/array.meta.json` & `su6-1.4.1/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ast.data.json` & `su6-1.4.1/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ast.meta.json` & `su6-1.4.1/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/builtins.data.json` & `su6-1.4.1/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/builtins.meta.json` & `su6-1.4.1/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/codecs.data.json` & `su6-1.4.1/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/codecs.meta.json` & `su6-1.4.1/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/colorsys.data.json` & `su6-1.4.1/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/colorsys.meta.json` & `su6-1.4.1/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configparser.data.json` & `su6-1.4.1/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configparser.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/contextlib.data.json` & `su6-1.4.1/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/contextlib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/contextvars.data.json` & `su6-1.4.1/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/contextvars.meta.json` & `su6-1.4.1/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/copy.data.json` & `su6-1.4.1/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/copy.meta.json` & `su6-1.4.1/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/copyreg.data.json` & `su6-1.4.1/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/copyreg.meta.json` & `su6-1.4.1/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/csv.data.json` & `su6-1.4.1/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/csv.meta.json` & `su6-1.4.1/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/dataclasses.data.json` & `su6-1.4.1/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/dataclasses.meta.json` & `su6-1.4.1/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/datetime.data.json` & `su6-1.4.1/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/datetime.meta.json` & `su6-1.4.1/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/decimal.data.json` & `su6-1.4.1/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/decimal.meta.json` & `su6-1.4.1/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/difflib.data.json` & `su6-1.4.1/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/difflib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/dis.data.json` & `su6-1.4.1/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/dis.meta.json` & `su6-1.4.1/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/enum.data.json` & `su6-1.4.1/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/enum.meta.json` & `su6-1.4.1/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/errno.data.json` & `su6-1.4.1/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/errno.meta.json` & `su6-1.4.1/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/fractions.data.json` & `su6-1.4.1/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/fractions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/functools.data.json` & `su6-1.4.1/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/functools.meta.json` & `su6-1.4.1/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/genericpath.data.json` & `su6-1.4.1/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/genericpath.meta.json` & `su6-1.4.1/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/getpass.data.json` & `su6-1.4.1/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/getpass.meta.json` & `su6-1.4.1/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/gettext.data.json` & `su6-1.4.1/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/gettext.meta.json` & `su6-1.4.1/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/glob.data.json` & `su6-1.4.1/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/glob.meta.json` & `su6-1.4.1/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/good.data.json` & `su6-1.4.1/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/good.meta.json` & `su6-1.4.1/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/hashlib.data.json` & `su6-1.4.1/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/hashlib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/hmac.data.json` & `su6-1.4.1/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/hmac.meta.json` & `su6-1.4.1/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/inspect.data.json` & `su6-1.4.1/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/inspect.meta.json` & `su6-1.4.1/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/io.data.json` & `su6-1.4.1/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/io.meta.json` & `su6-1.4.1/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/itertools.data.json` & `su6-1.4.1/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/itertools.meta.json` & `su6-1.4.1/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/linecache.data.json` & `su6-1.4.1/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/linecache.meta.json` & `su6-1.4.1/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/marshal.data.json` & `su6-1.4.1/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/marshal.meta.json` & `su6-1.4.1/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/math.data.json` & `su6-1.4.1/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/math.meta.json` & `su6-1.4.1/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mmap.data.json` & `su6-1.4.1/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mmap.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/msvcrt.data.json` & `su6-1.4.1/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/msvcrt.meta.json` & `su6-1.4.1/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mypy_extensions.data.json` & `su6-1.4.1/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mypy_extensions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/numbers.data.json` & `su6-1.4.1/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/numbers.meta.json` & `su6-1.4.1/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/opcode.data.json` & `su6-1.4.1/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/opcode.meta.json` & `su6-1.4.1/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/operator.data.json` & `su6-1.4.1/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/operator.meta.json` & `su6-1.4.1/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathlib.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathlib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pickle.data.json` & `su6-1.4.1/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pickle.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platform.data.json` & `su6-1.4.1/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platform.meta.json` & `su6-1.4.1/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/posixpath.data.json` & `su6-1.4.1/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/posixpath.meta.json` & `su6-1.4.1/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pty.data.json` & `su6-1.4.1/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pty.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pydoc.data.json` & `su6-1.4.1/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pydoc.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/queue.data.json` & `su6-1.4.1/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/queue.meta.json` & `su6-1.4.1/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/random.data.json` & `su6-1.4.1/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/random.meta.json` & `su6-1.4.1/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/re.data.json` & `su6-1.4.1/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/re.meta.json` & `su6-1.4.1/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/reprlib.data.json` & `su6-1.4.1/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/reprlib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/secrets.data.json` & `su6-1.4.1/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/secrets.meta.json` & `su6-1.4.1/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/selectors.data.json` & `su6-1.4.1/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/selectors.meta.json` & `su6-1.4.1/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/shlex.data.json` & `su6-1.4.1/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/shlex.meta.json` & `su6-1.4.1/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/shutil.data.json` & `su6-1.4.1/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/shutil.meta.json` & `su6-1.4.1/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/signal.data.json` & `su6-1.4.1/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/signal.meta.json` & `su6-1.4.1/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/socket.data.json` & `su6-1.4.1/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/socket.meta.json` & `su6-1.4.1/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sre_compile.data.json` & `su6-1.4.1/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sre_compile.meta.json` & `su6-1.4.1/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sre_constants.data.json` & `su6-1.4.1/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sre_constants.meta.json` & `su6-1.4.1/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sre_parse.data.json` & `su6-1.4.1/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sre_parse.meta.json` & `su6-1.4.1/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ssl.data.json` & `su6-1.4.1/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ssl.meta.json` & `su6-1.4.1/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/stat.data.json` & `su6-1.4.1/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/stat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/string.data.json` & `su6-1.4.1/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/string.meta.json` & `su6-1.4.1/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/struct.data.json` & `su6-1.4.1/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/struct.meta.json` & `su6-1.4.1/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/subprocess.data.json` & `su6-1.4.1/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/subprocess.meta.json` & `su6-1.4.1/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sys.data.json` & `su6-1.4.1/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sys.meta.json` & `su6-1.4.1/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sysconfig.data.json` & `su6-1.4.1/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/sysconfig.meta.json` & `su6-1.4.1/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tempfile.data.json` & `su6-1.4.1/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tempfile.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/termios.data.json` & `su6-1.4.1/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/termios.meta.json` & `su6-1.4.1/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/textwrap.data.json` & `su6-1.4.1/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/textwrap.meta.json` & `su6-1.4.1/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/this.data.json` & `su6-1.4.1/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/this.meta.json` & `su6-1.4.1/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/threading.data.json` & `su6-1.4.1/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/threading.meta.json` & `su6-1.4.1/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/time.data.json` & `su6-1.4.1/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/time.meta.json` & `su6-1.4.1/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/token.data.json` & `su6-1.4.1/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/token.meta.json` & `su6-1.4.1/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tokenize.data.json` & `su6-1.4.1/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tokenize.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomllib.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomllib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/traceback.data.json` & `su6-1.4.1/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/traceback.meta.json` & `su6-1.4.1/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tty.data.json` & `su6-1.4.1/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tty.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/types.data.json` & `su6-1.4.1/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/types.meta.json` & `su6-1.4.1/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typing.data.json` & `su6-1.4.1/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typing.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typing_extensions.data.json` & `su6-1.4.1/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/uuid.data.json` & `su6-1.4.1/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/uuid.meta.json` & `su6-1.4.1/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/warnings.data.json` & `su6-1.4.1/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/warnings.meta.json` & `su6-1.4.1/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/weakref.data.json` & `su6-1.4.1/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/weakref.meta.json` & `su6-1.4.1/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/webbrowser.data.json` & `su6-1.4.1/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/webbrowser.meta.json` & `su6-1.4.1/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/zlib.data.json` & `su6-1.4.1/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/zlib.meta.json` & `su6-1.4.1/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/base_events.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/base_events.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/coroutines.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/events.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/events.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/exceptions.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/futures.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/futures.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/locks.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/locks.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/mixins.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/mixins.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/protocols.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/protocols.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/queues.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/queues.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/runners.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/runners.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/selector_events.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/streams.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/streams.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/subprocess.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/tasks.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/tasks.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/threads.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/threads.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/timeouts.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/transports.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/transports.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/unix_events.data.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/_width_table.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/_width_table.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/brackets.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/brackets.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/cache.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/cache.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/comments.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/comments.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/concurrency.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/concurrency.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/const.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/const.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/files.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/files.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/linegen.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/linegen.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/lines.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/lines.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/mode.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/mode.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/nodes.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/nodes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/numerics.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/numerics.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/output.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/output.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/parsing.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/parsing.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/report.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/report.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/rusty.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/rusty.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/strings.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/strings.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/trans.data.json` & `su6-1.4.1/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/black/trans.meta.json` & `su6-1.4.1/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/_compat.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/_compat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/core.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/core.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/decorators.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/decorators.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/exceptions.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/formatting.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/formatting.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/globals.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/globals.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/parser.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/parser.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/termui.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/termui.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/types.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/types.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/click/utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/collections/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/collections/abc.data.json` & `su6-1.4.1/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/collections/abc.meta.json` & `su6-1.4.1/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/process.data.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.data.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875776397515528%*

 * *Differences: {"'names'": "{'asdict': OrderedDict([('.class', 'SymbolTableNode'), ('cross_ref', "*

 * *            "'configuraptor.dump.asdict'), ('kind', 'Gdef')]), 'asjson': OrderedDict([('.class', "*

 * *            "'SymbolTableNode'), ('cross_ref', 'configuraptor.dump.asjson'), ('kind', 'Gdef')]), "*

 * *            "'astoml': OrderedDict([('.class', 'SymbolTableNode'), ('cross_ref', "*

 * *            "'configuraptor.dump.astoml'), ('kind', 'Gdef')]), 'asyaml': OrderedDict([('.class', "*

 * *            "'SymbolTableNode'), ('cross_ref', ' […]*

```diff
@@ -145,14 +145,34 @@
             }
         },
         "all_annotations": {
             ".class": "SymbolTableNode",
             "cross_ref": "configuraptor.core.all_annotations",
             "kind": "Gdef"
         },
+        "asdict": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.dump.asdict",
+            "kind": "Gdef"
+        },
+        "asjson": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.dump.asjson",
+            "kind": "Gdef"
+        },
+        "astoml": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.dump.astoml",
+            "kind": "Gdef"
+        },
+        "asyaml": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.dump.asyaml",
+            "kind": "Gdef"
+        },
         "check_and_convert_data": {
             ".class": "SymbolTableNode",
             "cross_ref": "configuraptor.core.check_and_convert_data",
             "kind": "Gdef"
         },
         "convert_config": {
             ".class": "SymbolTableNode",
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8208333333333333%*

 * *Differences: {"'data_mtime'": '1687189420',*

 * * "'dep_lines'": '{insert: [(4, 20)]}',*

 * * "'dep_prios'": '{insert: [(0, 5)]}',*

 * * "'dependencies'": "{insert: [(2, 'configuraptor.dump')]}",*

 * * "'hash'": "'8fde7ffc2d54bc82bb84c201c70ff98b39202a50d452ff8b828328dc4d8a038e'",*

 * * "'interface_hash'": "'02bccb11475157fbac2f649d5aad6b3ae98aa7ffe26c43f2e79df605adc22746'",*

 * * "'mtime'": '1687189299',*

 * * "'size'": '876'}*

```diff
@@ -1,41 +1,44 @@
 {
-    "data_mtime": 1686831554,
+    "data_mtime": 1687189420,
     "dep_lines": [
         8,
         9,
         18,
         19,
+        20,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
+        5,
         30,
         30
     ],
     "dependencies": [
         "configuraptor.cls",
         "configuraptor.core",
+        "configuraptor.dump",
         "configuraptor.postpone",
         "configuraptor.singleton",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "a4d45a3e677e3438acfab97f2cf7eb1e3187c5f9a7b5934bf321b90694056d03",
+    "hash": "8fde7ffc2d54bc82bb84c201c70ff98b39202a50d452ff8b828328dc4d8a038e",
     "id": "configuraptor",
     "ignore_all": true,
-    "interface_hash": "b0c7012f8b50c8bf50772599e049e962b9567d5cf06bb103ddd4f4338f178a9a",
-    "mtime": 1686825273,
+    "interface_hash": "02bccb11475157fbac2f649d5aad6b3ae98aa7ffe26c43f2e79df605adc22746",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -71,11 +74,11 @@
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
     "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/__init__.py",
     "plugin_data": null,
-    "size": 760,
+    "size": 876,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/cls.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.data.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8239468864468865%*

 * *Differences: {"'_fullname'": "'configuraptor.singleton'",*

 * * "'names'": "{'__annotations__': {'node': {'fullname': "*

 * *            "'configuraptor.singleton.__annotations__'}}, '__doc__': {'node': {'fullname': "*

 * *            "'configuraptor.singleton.__doc__'}}, '__file__': {'node': {'fullname': "*

 * *            "'configuraptor.singleton.__file__'}}, '__name__': {'node': {'fullname': "*

 * *            "'configuraptor.singleton.__name__'}}, '__package__': {'node': {'fullname': "*

 * *            "'configuraptor.singleton.__package__'}},  […]*

```diff
@@ -1,343 +1,299 @@
 {
     ".class": "MypyFile",
-    "_fullname": "configuraptor.cls",
+    "_fullname": "configuraptor.singleton",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
-        "C": {
+        "Singleton": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "TypeVarExpr",
-                "fullname": "configuraptor.cls.C",
-                "name": "C",
-                "upper_bound": {
-                    ".class": "AnyType",
-                    "missing_import_name": null,
-                    "source_any": null,
-                    "type_of_any": 2
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "builtins.object"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": "configuraptor.singleton.SingletonMeta",
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "configuraptor.singleton.Singleton",
+                    "name": "Singleton",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [],
+                "fullname": "configuraptor.singleton.Singleton",
+                "has_param_spec_type": false,
+                "metaclass_type": "configuraptor.singleton.SingletonMeta",
+                "metadata": {},
+                "module_name": "configuraptor.singleton",
+                "mro": [
+                    "configuraptor.singleton.Singleton",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable"
                 },
-                "values": [],
-                "variance": 0
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
             }
         },
-        "T_data": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "configuraptor.core.T_data",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "TypedConfig": {
+        "SingletonMeta": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
                 "alt_promote": null,
                 "bases": [
-                    "builtins.object"
+                    "builtins.type"
                 ],
                 "dataclass_transform_spec": null,
                 "declared_metaclass": null,
                 "defn": {
                     ".class": "ClassDef",
-                    "fullname": "configuraptor.cls.TypedConfig",
-                    "name": "TypedConfig",
+                    "fullname": "configuraptor.singleton.SingletonMeta",
+                    "name": "SingletonMeta",
                     "type_vars": []
                 },
                 "deletable_attributes": [],
                 "flags": [],
-                "fullname": "configuraptor.cls.TypedConfig",
+                "fullname": "configuraptor.singleton.SingletonMeta",
                 "has_param_spec_type": false,
                 "metaclass_type": null,
                 "metadata": {},
-                "module_name": "configuraptor.cls",
+                "module_name": "configuraptor.singleton",
                 "mro": [
-                    "configuraptor.cls.TypedConfig",
+                    "configuraptor.singleton.SingletonMeta",
+                    "builtins.type",
                     "builtins.object"
                 ],
                 "names": {
                     ".class": "SymbolTable",
-                    "load": {
+                    "__call__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                2,
+                                4
+                            ],
+                            "arg_names": [
+                                "self",
+                                "args",
+                                "kwargs"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "configuraptor.singleton.SingletonMeta.__call__",
+                            "name": "__call__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    2,
+                                    4
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "args",
+                                    "kwargs"
+                                ],
+                                "arg_types": [
+                                    "configuraptor.singleton.SingletonMeta",
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    },
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__call__ of SingletonMeta",
+                                "ret_type": {
+                                    ".class": "TypeType",
+                                    "item": {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "_instances": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "configuraptor.singleton.SingletonMeta._instances",
+                            "name": "_instances",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    {
+                                        ".class": "TypeType",
+                                        "item": {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    },
+                                    {
+                                        ".class": "TypeType",
+                                        "item": {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    }
+                                ],
+                                "type_ref": "builtins.dict"
+                            }
+                        }
+                    },
+                    "clear": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Decorator",
                             "func": {
                                 ".class": "FuncDef",
                                 "abstract_status": 0,
                                 "arg_kinds": [
-                                    0,
-                                    0,
-                                    1,
-                                    1,
                                     1
                                 ],
                                 "arg_names": [
-                                    "cls",
-                                    "data",
-                                    "key",
-                                    "init",
-                                    "strict"
+                                    "instance"
                                 ],
                                 "dataclass_transform_spec": null,
                                 "flags": [
-                                    "is_class",
+                                    "is_static",
                                     "is_decorated"
                                 ],
-                                "fullname": "configuraptor.cls.TypedConfig.load",
-                                "name": "load",
+                                "fullname": "configuraptor.singleton.SingletonMeta.clear",
+                                "name": "clear",
                                 "type": {
                                     ".class": "CallableType",
                                     "arg_kinds": [
-                                        0,
-                                        0,
-                                        1,
-                                        1,
                                         1
                                     ],
                                     "arg_names": [
-                                        "cls",
-                                        "data",
-                                        "key",
-                                        "init",
-                                        "strict"
+                                        "instance"
                                     ],
                                     "arg_types": [
                                         {
-                                            ".class": "TypeType",
-                                            "item": {
-                                                ".class": "TypeVarType",
-                                                "fullname": "configuraptor.cls.C",
-                                                "id": -1,
-                                                "name": "C",
-                                                "namespace": "",
-                                                "upper_bound": {
-                                                    ".class": "AnyType",
-                                                    "missing_import_name": null,
-                                                    "source_any": null,
-                                                    "type_of_any": 2
-                                                },
-                                                "values": [],
-                                                "variance": 0
-                                            }
-                                        },
-                                        {
-                                            ".class": "TypeAliasType",
-                                            "args": [],
-                                            "type_ref": "configuraptor.core.T_data"
-                                        },
-                                        {
                                             ".class": "UnionType",
                                             "items": [
-                                                "builtins.str",
+                                                "configuraptor.singleton.Singleton",
                                                 {
                                                     ".class": "NoneType"
                                                 }
                                             ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        "builtins.str",
-                                                        {
-                                                            ".class": "AnyType",
-                                                            "missing_import_name": null,
-                                                            "source_any": null,
-                                                            "type_of_any": 2
-                                                        }
-                                                    ],
-                                                    "type_ref": "builtins.dict"
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        "builtins.bool"
+                                        }
                                     ],
                                     "bound_args": [],
                                     "def_extras": {
-                                        "first_arg": "cls"
+                                        "first_arg": null
                                     },
                                     "fallback": "builtins.function",
                                     "from_concatenate": false,
                                     "implicit": false,
                                     "is_ellipsis_args": false,
-                                    "name": "load of TypedConfig",
+                                    "name": "clear of SingletonMeta",
                                     "ret_type": {
-                                        ".class": "TypeVarType",
-                                        "fullname": "configuraptor.cls.C",
-                                        "id": -1,
-                                        "name": "C",
-                                        "namespace": "",
-                                        "upper_bound": {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 2
-                                        },
-                                        "values": [],
-                                        "variance": 0
+                                        ".class": "NoneType"
                                     },
                                     "type_guard": null,
                                     "unpack_kwargs": false,
-                                    "variables": [
-                                        {
-                                            ".class": "TypeVarType",
-                                            "fullname": "configuraptor.cls.C",
-                                            "id": -1,
-                                            "name": "C",
-                                            "namespace": "",
-                                            "upper_bound": {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 2
-                                            },
-                                            "values": [],
-                                            "variance": 0
-                                        }
-                                    ]
+                                    "variables": []
                                 }
                             },
                             "is_overload": false,
                             "var": {
                                 ".class": "Var",
                                 "flags": [
                                     "is_initialized_in_class",
-                                    "is_classmethod",
+                                    "is_staticmethod",
                                     "is_ready",
                                     "is_inferred"
                                 ],
-                                "fullname": "configuraptor.cls.TypedConfig.load",
-                                "name": "load",
+                                "fullname": "configuraptor.singleton.SingletonMeta.clear",
+                                "name": "clear",
                                 "type": {
                                     ".class": "CallableType",
                                     "arg_kinds": [
-                                        0,
-                                        0,
-                                        1,
-                                        1,
                                         1
                                     ],
                                     "arg_names": [
-                                        "cls",
-                                        "data",
-                                        "key",
-                                        "init",
-                                        "strict"
+                                        "instance"
                                     ],
                                     "arg_types": [
                                         {
-                                            ".class": "TypeType",
-                                            "item": {
-                                                ".class": "TypeVarType",
-                                                "fullname": "configuraptor.cls.C",
-                                                "id": -1,
-                                                "name": "C",
-                                                "namespace": "",
-                                                "upper_bound": {
-                                                    ".class": "AnyType",
-                                                    "missing_import_name": null,
-                                                    "source_any": null,
-                                                    "type_of_any": 2
-                                                },
-                                                "values": [],
-                                                "variance": 0
-                                            }
-                                        },
-                                        {
-                                            ".class": "TypeAliasType",
-                                            "args": [],
-                                            "type_ref": "configuraptor.core.T_data"
-                                        },
-                                        {
                                             ".class": "UnionType",
                                             "items": [
-                                                "builtins.str",
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        "builtins.str",
-                                                        {
-                                                            ".class": "AnyType",
-                                                            "missing_import_name": null,
-                                                            "source_any": null,
-                                                            "type_of_any": 2
-                                                        }
-                                                    ],
-                                                    "type_ref": "builtins.dict"
-                                                },
+                                                "configuraptor.singleton.Singleton",
                                                 {
                                                     ".class": "NoneType"
                                                 }
                                             ]
-                                        },
-                                        "builtins.bool"
+                                        }
                                     ],
                                     "bound_args": [],
                                     "def_extras": {
-                                        "first_arg": "cls"
+                                        "first_arg": null
                                     },
                                     "fallback": "builtins.function",
                                     "from_concatenate": false,
                                     "implicit": false,
                                     "is_ellipsis_args": false,
-                                    "name": "load of TypedConfig",
+                                    "name": "clear of SingletonMeta",
                                     "ret_type": {
-                                        ".class": "TypeVarType",
-                                        "fullname": "configuraptor.cls.C",
-                                        "id": -1,
-                                        "name": "C",
-                                        "namespace": "",
-                                        "upper_bound": {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 2
-                                        },
-                                        "values": [],
-                                        "variance": 0
+                                        ".class": "NoneType"
                                     },
                                     "type_guard": null,
                                     "unpack_kwargs": false,
-                                    "variables": [
-                                        {
-                                            ".class": "TypeVarType",
-                                            "fullname": "configuraptor.cls.C",
-                                            "id": -1,
-                                            "name": "C",
-                                            "namespace": "",
-                                            "upper_bound": {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 2
-                                            },
-                                            "values": [],
-                                            "variance": 0
-                                        }
-                                    ]
+                                    "variables": []
                                 }
                             }
                         }
                     }
                 },
                 "self_type": null,
                 "slots": null,
@@ -350,15 +306,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.cls.__annotations__",
+                "fullname": "configuraptor.singleton.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -375,68 +331,61 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.cls.__doc__",
+                "fullname": "configuraptor.singleton.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.cls.__file__",
+                "fullname": "configuraptor.singleton.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.cls.__name__",
+                "fullname": "configuraptor.singleton.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.cls.__package__",
+                "fullname": "configuraptor.singleton.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "load_into": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "configuraptor.core.load_into",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "typing": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         }
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/cls.py"
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/singleton.py"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/cls.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8083333333333333%*

 * *Differences: {"'data_mtime'": '1687189420',*

 * * "'dep_lines'": '{insert: [(1, 8), (3, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (4, 30)]}',*

 * * "'dependencies'": "{insert: [(1, 'configuraptor.errors'), (4, '_collections_abc')]}",*

 * * "'hash'": "'27e08dd4e67d4d23892e6517af3e11b41b56d5dfcf5ac11824c4c8657d7b8114'",*

 * * "'interface_hash'": "'afbedb43a12ac1e18ffeec206bade8cb341d97bc7dd4bfecdfe031d2ff202890'",*

 * * "'mtime'": '1687189299',*

 * * "'size'": '1594'}*

```diff
@@ -1,38 +1,44 @@
 {
-    "data_mtime": 1686831554,
+    "data_mtime": 1687189420,
     "dep_lines": [
         7,
+        8,
         5,
         1,
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
+        5,
         10,
         5,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
         "configuraptor.core",
+        "configuraptor.errors",
         "typing",
         "builtins",
+        "_collections_abc",
         "abc",
         "os",
         "pathlib"
     ],
-    "hash": "75c16778e01989f1b99034901cd0e4ccfb791cddb1cce6acc42eef62cb5a595f",
+    "hash": "27e08dd4e67d4d23892e6517af3e11b41b56d5dfcf5ac11824c4c8657d7b8114",
     "id": "configuraptor.cls",
     "ignore_all": true,
-    "interface_hash": "1c464b7e8cfb00797d0abf54fc94770df84edd72abdb221b977d3b01ac2b44eb",
-    "mtime": 1686825273,
+    "interface_hash": "afbedb43a12ac1e18ffeec206bade8cb341d97bc7dd4bfecdfe031d2ff202890",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -68,11 +74,11 @@
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
     "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/cls.py",
     "plugin_data": null,
-    "size": 606,
+    "size": 1594,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/core.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/core.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971130711254409%*

 * *Differences: {"'names'": "{'T_data': {'node': {'line': 26}}, 'T_typelike': {'node': {'line': 24}}, 'Type': "*

 * *            "{'node': {'line': 146}}, 'Type_C': {'node': {'line': 30}}, 'is_optional': {'node': "*

 * *            "{'type': {'arg_types': {0: {'items': {1: {'.class': 'AnyType', 'missing_import_name': "*

 * *            "None, 'source_any': None, 'type_of_any': 2}}}}}}}, 'instance_of_custom_class': "*

 * *            "OrderedDict([('.class', 'SymbolTableNode'), ('kind', 'Gdef'), ('node', "*

 * *            "OrderedDict([('.class',  […]*

```diff
@@ -89,15 +89,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.T_data",
-                "line": 25,
+                "line": 26,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.str",
                         "pathlib.Path",
@@ -122,15 +122,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.T_typelike",
-                "line": 23,
+                "line": 24,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.type",
                         "types.UnionType"
@@ -142,15 +142,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.core.Type",
-                "line": 142,
+                "line": 146,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "TypeType",
                     "item": {
                         ".class": "AnyType",
                         "missing_import_name": null,
@@ -182,15 +182,15 @@
                         "upper_bound": "builtins.object",
                         "values": [],
                         "variance": 0
                     }
                 ],
                 "column": 0,
                 "fullname": "configuraptor.core.Type_C",
-                "line": 29,
+                "line": 30,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "TypeType",
                     "item": {
                         ".class": "TypeVarType",
                         "fullname": "configuraptor.core.C",
@@ -1322,14 +1322,62 @@
                             "values": [],
                             "variance": 0
                         }
                     ]
                 }
             }
         },
+        "instance_of_custom_class": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0
+                ],
+                "arg_names": [
+                    "var"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.core.instance_of_custom_class",
+                "name": "instance_of_custom_class",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        "var"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "instance_of_custom_class",
+                    "ret_type": "builtins.bool",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
         "is_builtin_type": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -1544,15 +1592,18 @@
                             "items": [
                                 {
                                     ".class": "TypeAliasType",
                                     "args": [],
                                     "type_ref": "configuraptor.core.Type"
                                 },
                                 {
-                                    ".class": "NoneType"
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
                                 }
                             ]
                         }
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
@@ -2108,14 +2159,21 @@
         "loaders": {
             ".class": "SymbolTableNode",
             "cross_ref": "configuraptor.loaders",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "math": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "math",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "types": {
             ".class": "SymbolTableNode",
             "cross_ref": "types",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/core.meta.json` & `su6-1.4.1/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6518988583550994%*

 * *Differences: {"'data_mtime'": '1686818222',*

 * * "'dep_lines'": '{insert: [(0, 8), (3, 37), (4, 2), (5, 3), (6, 4), (11, 11), (14, 1), (15, 1), '*

 * *                '(16, 1), (17, 1), (35, 14), (36, 13)], delete: [9, 7, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (4, 10), (11, 10), (13, 5), (15, 30), (16, 30), (17, 30), (18, '*

 * *                '30), (35, 5), (36, 5)], delete: [11, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib.metadata'), (1, 'su6.__about__'), (2, 'su6.core'), "*

 * *                   "(3, 'su6.plugins'), (4, ' […]*

```diff
@@ -1,20 +1,22 @@
 {
-    "data_mtime": 1686831554,
+    "data_mtime": 1686818222,
     "dep_lines": [
-        15,
-        16,
+        8,
         17,
         18,
+        37,
+        2,
+        3,
+        4,
         5,
         6,
         7,
-        8,
         9,
-        10,
+        11,
         12,
         15,
         1,
         1,
         1,
         1,
         1,
@@ -25,29 +27,37 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        1,
+        1,
+        14,
+        13
     ],
     "dep_prios": [
-        10,
+        5,
         5,
         5,
         5,
         10,
         10,
         10,
         10,
+        10,
+        5,
         5,
+        10,
         5,
         5,
-        20,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
@@ -56,52 +66,64 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        30,
+        30,
+        30,
+        30,
+        5,
+        5
     ],
     "dependencies": [
-        "configuraptor.loaders",
-        "configuraptor.errors",
-        "configuraptor.helpers",
-        "configuraptor.postpone",
-        "dataclasses",
-        "types",
+        "importlib.metadata",
+        "su6.__about__",
+        "su6.core",
+        "su6.plugins",
+        "contextlib",
+        "math",
+        "os",
+        "sys",
         "typing",
-        "warnings",
-        "collections",
-        "pathlib",
-        "typeguard",
+        "dataclasses",
+        "json",
+        "typer",
         "configuraptor",
+        "rich",
         "builtins",
-        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
+        "click",
+        "click.core",
+        "click.exceptions",
+        "configuraptor.cls",
         "configuraptor.singleton",
         "ctypes",
         "enum",
+        "importlib",
         "io",
+        "json.decoder",
         "mmap",
-        "os",
         "pickle",
-        "typeguard._config",
-        "typeguard._exceptions",
-        "typeguard._functions",
-        "typeguard._memo",
+        "typer.core",
+        "typer.main",
+        "typer.models",
+        "types",
         "typing_extensions"
     ],
-    "hash": "e1b767fc5f24be6a44c43ec9584df75e05d055ba32b3eff29982791104e4848e",
-    "id": "configuraptor.core",
-    "ignore_all": true,
-    "interface_hash": "bd89bd4e424063dcd6408bec768eebb0caf247e8190c312b85822232c41fd035",
-    "mtime": 1686825273,
+    "hash": "c779aeec5d3a739944c39e10191900e3250189ebacdcb3782d0317031961f32e",
+    "id": "su6.cli",
+    "ignore_all": false,
+    "interface_hash": "0df9143d2f97cb5869342bf9eb6560aed886c3ab9e5ba659a12c9e5fb3664420",
+    "mtime": 1686818322,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -135,13 +157,16 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/core.py",
+    "path": "src/su6/cli.py",
     "plugin_data": null,
-    "size": 15190,
-    "suppressed": [],
+    "size": 12942,
+    "suppressed": [
+        "plumbum.machines",
+        "plumbum"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/errors.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.data.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945053910341553%*

 * *Differences: {"'names'": "{'ConfigErrorInvalidType': {'node': {'metadata': {'dataclass': {'attributes': {0: "*

 * *            "{'line': 90}, 1: {'line': 91}, 2: {'line': 92}}}}}}, 'ConfigErrorMissingKey': "*

 * *            "{'node': {'metadata': {'dataclass': {'attributes': {0: {'line': 34}, 1: {'line': 35}, "*

 * *            "2: {'line': 36}}}}, 'names': {'_annotated_type': {'node': {'type': {replace: "*

 * *            "OrderedDict([('.class', 'UnionType'), ('items', [OrderedDict([('.class', 'AnyType'), "*

 * *            "('missing_import […]*

```diff
@@ -44,14 +44,403 @@
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
             }
         },
+        "ConfigErrorExtraKey": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "configuraptor.errors.ConfigError"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": null,
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "configuraptor.errors.ConfigErrorExtraKey",
+                    "name": "ConfigErrorExtraKey",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [],
+                "fullname": "configuraptor.errors.ConfigErrorExtraKey",
+                "has_param_spec_type": false,
+                "metaclass_type": null,
+                "metadata": {
+                    "dataclass": {
+                        "attributes": [
+                            {
+                                "alias": null,
+                                "column": 4,
+                                "has_default": false,
+                                "is_in_init": true,
+                                "is_init_var": false,
+                                "is_neither_frozen_nor_nonfrozen": false,
+                                "kw_only": false,
+                                "line": 62,
+                                "name": "key",
+                                "type": "builtins.str"
+                            },
+                            {
+                                "alias": null,
+                                "column": 4,
+                                "has_default": false,
+                                "is_in_init": true,
+                                "is_init_var": false,
+                                "is_neither_frozen_nor_nonfrozen": false,
+                                "kw_only": false,
+                                "line": 63,
+                                "name": "value",
+                                "type": "builtins.str"
+                            },
+                            {
+                                "alias": null,
+                                "column": 4,
+                                "has_default": false,
+                                "is_in_init": true,
+                                "is_init_var": false,
+                                "is_neither_frozen_nor_nonfrozen": false,
+                                "kw_only": false,
+                                "line": 64,
+                                "name": "cls",
+                                "type": "builtins.type"
+                            }
+                        ],
+                        "frozen": false
+                    },
+                    "dataclass_tag": {}
+                },
+                "module_name": "configuraptor.errors",
+                "mro": [
+                    "configuraptor.errors.ConfigErrorExtraKey",
+                    "configuraptor.errors.ConfigError",
+                    "builtins.Exception",
+                    "builtins.BaseException",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
+                    "__dataclass_fields__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_classvar",
+                                "is_ready"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.__dataclass_fields__",
+                            "name": "__dataclass_fields__",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    "builtins.str",
+                                    {
+                                        ".class": "Instance",
+                                        "args": [
+                                            {
+                                                ".class": "AnyType",
+                                                "missing_import_name": null,
+                                                "source_any": null,
+                                                "type_of_any": 2
+                                            }
+                                        ],
+                                        "type_ref": "dataclasses.Field"
+                                    }
+                                ],
+                                "type_ref": "builtins.dict"
+                            }
+                        },
+                        "plugin_generated": true
+                    },
+                    "__init__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0,
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "self",
+                                "key",
+                                "value",
+                                "cls"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.__init__",
+                            "name": "__init__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0,
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "key",
+                                    "value",
+                                    "cls"
+                                ],
+                                "arg_types": [
+                                    "configuraptor.errors.ConfigErrorExtraKey",
+                                    "builtins.str",
+                                    "builtins.str",
+                                    "builtins.type"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {},
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__init__ of ConfigErrorExtraKey",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        },
+                        "plugin_generated": true
+                    },
+                    "__match_args__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_ready",
+                                "allow_incompatible_override"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.__match_args__",
+                            "name": "__match_args__",
+                            "type": {
+                                ".class": "TupleType",
+                                "implicit": false,
+                                "items": [
+                                    {
+                                        ".class": "LiteralType",
+                                        "fallback": "builtins.str",
+                                        "value": "key"
+                                    },
+                                    {
+                                        ".class": "LiteralType",
+                                        "fallback": "builtins.str",
+                                        "value": "value"
+                                    },
+                                    {
+                                        ".class": "LiteralType",
+                                        "fallback": "builtins.str",
+                                        "value": "cls"
+                                    }
+                                ],
+                                "partial_fallback": {
+                                    ".class": "Instance",
+                                    "args": [
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 6
+                                        }
+                                    ],
+                                    "type_ref": "builtins.tuple"
+                                }
+                            }
+                        },
+                        "plugin_generated": true
+                    },
+                    "__post_init__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.__post_init__",
+                            "name": "__post_init__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "configuraptor.errors.ConfigErrorExtraKey"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__post_init__ of ConfigErrorExtraKey",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "__str__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.__str__",
+                            "name": "__str__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    null
+                                ],
+                                "arg_types": [
+                                    "configuraptor.errors.ConfigErrorExtraKey"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__str__ of ConfigErrorExtraKey",
+                                "ret_type": "builtins.str",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "_cls": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_inferred"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey._cls",
+                            "name": "_cls",
+                            "type": "builtins.str"
+                        }
+                    },
+                    "_type": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_inferred"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey._type",
+                            "name": "_type",
+                            "type": {
+                                ".class": "TypeType",
+                                "item": "builtins.str"
+                            }
+                        }
+                    },
+                    "cls": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.cls",
+                            "name": "cls",
+                            "type": "builtins.type"
+                        }
+                    },
+                    "key": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.key",
+                            "name": "key",
+                            "type": "builtins.str"
+                        }
+                    },
+                    "value": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "configuraptor.errors.ConfigErrorExtraKey.value",
+                            "name": "value",
+                            "type": "builtins.str"
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
+            }
+        },
         "ConfigErrorInvalidType": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
@@ -79,27 +468,27 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 48,
+                                "line": 90,
                                 "name": "key",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 49,
+                                "line": 91,
                                 "name": "value",
                                 "type": {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
                                     "type_of_any": 2
                                 }
@@ -108,15 +497,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 50,
+                                "line": 92,
                                 "name": "expected_type",
                                 "type": "builtins.type"
                             }
                         ],
                         "frozen": false
                     },
                     "dataclass_tag": {}
@@ -488,39 +877,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 20,
+                                "line": 34,
                                 "name": "key",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 21,
+                                "line": 35,
                                 "name": "cls",
                                 "type": "builtins.type"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 22,
+                                "line": 36,
                                 "name": "annotated_type",
                                 "type": "builtins.type"
                             }
                         ],
                         "frozen": false
                     },
                     "dataclass_tag": {}
@@ -769,15 +1158,26 @@
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_inferred"
                             ],
                             "fullname": "configuraptor.errors.ConfigErrorMissingKey._annotated_type",
                             "name": "_annotated_type",
-                            "type": "builtins.str"
+                            "type": {
+                                ".class": "UnionType",
+                                "items": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    },
+                                    "builtins.str"
+                                ]
+                            }
                         }
                     },
                     "_cls": {
                         ".class": "SymbolTableNode",
                         "implicit": true,
                         "kind": "Mdef",
                         "node": {
@@ -874,15 +1274,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 79,
+                                "line": 121,
                                 "name": "message",
                                 "type": "builtins.str"
                             }
                         ],
                         "frozen": false
                     },
                     "dataclass_tag": {}
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/errors.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'data_mtime'": '1687189420',*

 * * "'hash'": "'5ed0ba320fc3e64d37e3a527de87168c982c7fcf66e05f53906e4700b926287e'",*

 * * "'interface_hash'": "'d377e2f1d693b1bc5fe7426c04308c09f17040986c13ff7b3012ed357586e8d6'",*

 * * "'mtime'": '1687189299',*

 * * "'size'": '3483'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1686831553,
+    "data_mtime": 1687189420,
     "dep_lines": [
         4,
         5,
         1,
         1,
         1,
         1,
@@ -26,19 +26,19 @@
         "builtins",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "95279bd0bcdd7666172d8f3cf5bd21fd94c7de6f65781cec851e90e43508e575",
+    "hash": "5ed0ba320fc3e64d37e3a527de87168c982c7fcf66e05f53906e4700b926287e",
     "id": "configuraptor.errors",
     "ignore_all": true,
-    "interface_hash": "983290384ba73c664610052107ca32fe2b09ba5b2e378b57762bd71b32f50b15",
-    "mtime": 1686825273,
+    "interface_hash": "d377e2f1d693b1bc5fe7426c04308c09f17040986c13ff7b3012ed357586e8d6",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -74,11 +74,11 @@
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
     "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/errors.py",
     "plugin_data": null,
-    "size": 2116,
+    "size": 3483,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/helpers.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/helpers.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7166666666666667%*

 * *Differences: {"'data_mtime'": '1686754986',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 2), (2, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (3, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.default_styles'), (1, 'rich.theme'), (4, 'rich.style')]}",*

 * * "'hash'": "'d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459'",*

 * * "'id'": "'rich.themes'",*

 * * "'interface_hash'": "'c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a'",*

 * * "'mtime'": '1686754199',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/v […]*

```diff
@@ -1,29 +1,38 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1686754986,
     "dep_lines": [
         1,
+        2,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "rich.default_styles",
+        "rich.theme",
         "builtins",
         "abc",
+        "rich.style",
         "typing"
     ],
-    "hash": "32ed36840fbe0e18b032d8f86ca33c819ea7e7d9d03e44b97f6c3a7dfd5133e5",
-    "id": "configuraptor.helpers",
+    "hash": "d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459",
+    "id": "rich.themes",
     "ignore_all": true,
-    "interface_hash": "fa6a613a7e56d42069a3559eed13704a7e16ad1e811c5e6ce4b0e40d2372f0fc",
-    "mtime": 1686825273,
+    "interface_hash": "c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a",
+    "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/helpers.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/themes.py",
     "plugin_data": null,
-    "size": 344,
+    "size": 102,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/postpone.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/postpone.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1687189299'}*

```diff
@@ -21,15 +21,15 @@
         "builtins",
         "abc"
     ],
     "hash": "447769cb4a5362c58bf902448b3dcfced4f928ff4945a595a1123b35ba5c8a0d",
     "id": "configuraptor.postpone",
     "ignore_all": true,
     "interface_hash": "ec4ec5d98a89a2c2f5ea94998815f4269d60db1e4e33b35a490d38f0bbda902d",
-    "mtime": 1686825273,
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/singleton.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.data.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8118734335839599%*

 * *Differences: {"'_fullname'": "'configuraptor.dump'",*

 * * "'names'": "{'__annotations__': {'node': {'fullname': 'configuraptor.dump.__annotations__'}}, "*

 * *            "'__doc__': {'node': {'fullname': 'configuraptor.dump.__doc__'}}, '__file__': {'node': "*

 * *            "{'fullname': 'configuraptor.dump.__file__'}}, '__name__': {'node': {'fullname': "*

 * *            "'configuraptor.dump.__name__'}}, '__package__': {'node': {'fullname': "*

 * *            "'configuraptor.dump.__package__'}}, 'asdict': OrderedDict([('.class', "*

 * *          […]*

```diff
@@ -1,320 +1,24 @@
 {
     ".class": "MypyFile",
-    "_fullname": "configuraptor.singleton",
+    "_fullname": "configuraptor.dump",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
-        "Singleton": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeInfo",
-                "_promote": [],
-                "abstract_attributes": [],
-                "alt_promote": null,
-                "bases": [
-                    "builtins.object"
-                ],
-                "dataclass_transform_spec": null,
-                "declared_metaclass": "configuraptor.singleton.SingletonMeta",
-                "defn": {
-                    ".class": "ClassDef",
-                    "fullname": "configuraptor.singleton.Singleton",
-                    "name": "Singleton",
-                    "type_vars": []
-                },
-                "deletable_attributes": [],
-                "flags": [],
-                "fullname": "configuraptor.singleton.Singleton",
-                "has_param_spec_type": false,
-                "metaclass_type": "configuraptor.singleton.SingletonMeta",
-                "metadata": {},
-                "module_name": "configuraptor.singleton",
-                "mro": [
-                    "configuraptor.singleton.Singleton",
-                    "builtins.object"
-                ],
-                "names": {
-                    ".class": "SymbolTable"
-                },
-                "self_type": null,
-                "slots": null,
-                "tuple_type": null,
-                "type_vars": [],
-                "typeddict_type": null
-            }
-        },
-        "SingletonMeta": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeInfo",
-                "_promote": [],
-                "abstract_attributes": [],
-                "alt_promote": null,
-                "bases": [
-                    "builtins.type"
-                ],
-                "dataclass_transform_spec": null,
-                "declared_metaclass": null,
-                "defn": {
-                    ".class": "ClassDef",
-                    "fullname": "configuraptor.singleton.SingletonMeta",
-                    "name": "SingletonMeta",
-                    "type_vars": []
-                },
-                "deletable_attributes": [],
-                "flags": [],
-                "fullname": "configuraptor.singleton.SingletonMeta",
-                "has_param_spec_type": false,
-                "metaclass_type": null,
-                "metadata": {},
-                "module_name": "configuraptor.singleton",
-                "mro": [
-                    "configuraptor.singleton.SingletonMeta",
-                    "builtins.type",
-                    "builtins.object"
-                ],
-                "names": {
-                    ".class": "SymbolTable",
-                    "__call__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                2,
-                                4
-                            ],
-                            "arg_names": [
-                                "self",
-                                "args",
-                                "kwargs"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "configuraptor.singleton.SingletonMeta.__call__",
-                            "name": "__call__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    2,
-                                    4
-                                ],
-                                "arg_names": [
-                                    "self",
-                                    "args",
-                                    "kwargs"
-                                ],
-                                "arg_types": [
-                                    "configuraptor.singleton.SingletonMeta",
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    },
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__call__ of SingletonMeta",
-                                "ret_type": {
-                                    ".class": "TypeType",
-                                    "item": {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
-                                },
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "_instances": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_initialized_in_class",
-                                "is_ready",
-                                "has_explicit_value"
-                            ],
-                            "fullname": "configuraptor.singleton.SingletonMeta._instances",
-                            "name": "_instances",
-                            "type": {
-                                ".class": "Instance",
-                                "args": [
-                                    {
-                                        ".class": "TypeType",
-                                        "item": {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 2
-                                        }
-                                    },
-                                    {
-                                        ".class": "TypeType",
-                                        "item": {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 2
-                                        }
-                                    }
-                                ],
-                                "type_ref": "builtins.dict"
-                            }
-                        }
-                    },
-                    "clear": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Decorator",
-                            "func": {
-                                ".class": "FuncDef",
-                                "abstract_status": 0,
-                                "arg_kinds": [
-                                    1
-                                ],
-                                "arg_names": [
-                                    "instance"
-                                ],
-                                "dataclass_transform_spec": null,
-                                "flags": [
-                                    "is_static",
-                                    "is_decorated"
-                                ],
-                                "fullname": "configuraptor.singleton.SingletonMeta.clear",
-                                "name": "clear",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        1
-                                    ],
-                                    "arg_names": [
-                                        "instance"
-                                    ],
-                                    "arg_types": [
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                "configuraptor.singleton.Singleton",
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        }
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": null
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "clear of SingletonMeta",
-                                    "ret_type": {
-                                        ".class": "NoneType"
-                                    },
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
-                            },
-                            "is_overload": false,
-                            "var": {
-                                ".class": "Var",
-                                "flags": [
-                                    "is_initialized_in_class",
-                                    "is_staticmethod",
-                                    "is_ready",
-                                    "is_inferred"
-                                ],
-                                "fullname": "configuraptor.singleton.SingletonMeta.clear",
-                                "name": "clear",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        1
-                                    ],
-                                    "arg_names": [
-                                        "instance"
-                                    ],
-                                    "arg_types": [
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                "configuraptor.singleton.Singleton",
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        }
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": null
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "clear of SingletonMeta",
-                                    "ret_type": {
-                                        ".class": "NoneType"
-                                    },
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
-                            }
-                        }
-                    }
-                },
-                "self_type": null,
-                "slots": null,
-                "tuple_type": null,
-                "type_vars": [],
-                "typeddict_type": null
-            }
-        },
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.singleton.__annotations__",
+                "fullname": "configuraptor.dump.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -331,61 +35,357 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.singleton.__doc__",
+                "fullname": "configuraptor.dump.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.singleton.__file__",
+                "fullname": "configuraptor.dump.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.singleton.__name__",
+                "fullname": "configuraptor.dump.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "configuraptor.singleton.__package__",
+                "fullname": "configuraptor.dump.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
+        "asdict": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    1,
+                    1
+                ],
+                "arg_names": [
+                    null,
+                    null,
+                    "with_top_level_key"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.dump.asdict",
+                "name": "asdict",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        1,
+                        1
+                    ],
+                    "arg_names": [
+                        null,
+                        null,
+                        "with_top_level_key"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        },
+                        "builtins.int",
+                        "builtins.bool"
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "asdict",
+                    "ret_type": {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
+                            }
+                        ],
+                        "type_ref": "builtins.dict"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "asjson": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    4
+                ],
+                "arg_names": [
+                    "inst",
+                    "kw"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.dump.asjson",
+                "name": "asjson",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        4
+                    ],
+                    "arg_names": [
+                        "inst",
+                        "kw"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "asjson",
+                    "ret_type": "builtins.str",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "astoml": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    1
+                ],
+                "arg_names": [
+                    "inst",
+                    "sort_keys"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.dump.astoml",
+                "name": "astoml",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        1
+                    ],
+                    "arg_names": [
+                        "inst",
+                        "sort_keys"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        },
+                        "builtins.bool"
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "astoml",
+                    "ret_type": "builtins.str",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "asyaml": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    4
+                ],
+                "arg_names": [
+                    "inst",
+                    "kw"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.dump.asyaml",
+                "name": "asyaml",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        4
+                    ],
+                    "arg_names": [
+                        "inst",
+                        "kw"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "asyaml",
+                    "ret_type": "builtins.str",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "camel_to_snake": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.helpers.camel_to_snake",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "instance_of_custom_class": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.core.instance_of_custom_class",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "is_custom_class": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "configuraptor.core.is_custom_class",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "json": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "json",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "tomlkit": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "tomlkit",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "typing": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
+        },
+        "yaml": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_suppressed_import",
+                    "is_ready",
+                    "is_inferred"
+                ],
+                "fullname": "configuraptor.dump.yaml",
+                "name": "yaml",
+                "type": {
+                    ".class": "AnyType",
+                    "missing_import_name": "configuraptor.dump.yaml",
+                    "source_any": null,
+                    "type_of_any": 3
+                }
+            }
         }
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/singleton.py"
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/dump.py"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/singleton.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1687189299'}*

```diff
@@ -15,15 +15,15 @@
         "builtins",
         "abc"
     ],
     "hash": "b362a9254eee372b37ec41b4cedd9c69261ffc20d94da49402d45ac08e421893",
     "id": "configuraptor.singleton",
     "ignore_all": true,
     "interface_hash": "50a88a8d4cd16062b669f482e7164783094b9852da7f957c5d66a838cfb1f11f",
-    "mtime": 1686825273,
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954317664565826%*

 * *Differences: {"'names'": "{'T_loader': {'node': {'line': 20}}, 'toml': {'cross_ref': "*

 * *            "'configuraptor.loaders.loaders_shared.toml'}, delete: ['sys']}"}*

```diff
@@ -44,15 +44,15 @@
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "configuraptor.loaders.T_loader",
-                "line": 18,
+                "line": 20,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0
                     ],
@@ -251,24 +251,17 @@
             }
         },
         "json": {
             ".class": "SymbolTableNode",
             "cross_ref": "configuraptor.loaders.loaders_shared.json",
             "kind": "Gdef"
         },
-        "sys": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "sys",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "toml": {
             ".class": "SymbolTableNode",
-            "cross_ref": "configuraptor.loaders.loaders_310.toml",
+            "cross_ref": "configuraptor.loaders.loaders_shared.toml",
             "kind": "Gdef"
         },
         "typing": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing",
             "kind": "Gdef",
             "module_hidden": true,
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.697037037037037%*

 * *Differences: {"'data_mtime'": '1686754986',*

 * * "'dep_lines'": '{insert: [(0, 4), (2, 52), (3, 1), (4, 2), (5, 1), (6, 1), (7, 1), (8, 1), (9, '*

 * *                '1), (10, 1)], delete: [4, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (6, 30), (7, 30), (8, 30), (9, 30), (10, 30), (11, 30)], '*

 * *                'delete: [3]}',*

 * * "'dependencies'": "{insert: [(0, 'rich._loop'), (1, 'rich.cells'), (2, 'rich.console'), (3, "*

 * *                   "'re'), (6, '_random'), (9, 'datetime'), (10, 'rich.jupyter'), (11, "*

 * *                   […]*

```diff
@@ -1,44 +1,62 @@
 {
-    "data_mtime": 1686754985,
+    "data_mtime": 1686754986,
     "dep_lines": [
-        8,
-        9,
-        14,
+        4,
         5,
-        6,
+        52,
+        1,
+        2,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         10,
-        10,
         5,
+        5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "configuraptor.loaders._types",
-        "configuraptor.loaders.loaders_shared",
-        "configuraptor.loaders.loaders_310",
-        "sys",
+        "rich._loop",
+        "rich.cells",
+        "rich.console",
+        "re",
         "typing",
         "builtins",
+        "_random",
         "_typeshed",
-        "abc"
+        "abc",
+        "datetime",
+        "rich.jupyter",
+        "rich.style",
+        "rich.text",
+        "rich.theme"
     ],
-    "hash": "449821bd7194cc667761738610d0264e6a3adf71a68f0cf6b948a95c27672d4e",
-    "id": "configuraptor.loaders",
+    "hash": "c5f57ff6dd1283aaf38a69ab0ebbbc7c25665256a56007072c37eb2599db6f04",
+    "id": "rich._wrap",
     "ignore_all": true,
-    "interface_hash": "bdbb6fbe117423fe90107083780bab299b262d8209e0520ea00193642b479b68",
-    "mtime": 1686825273,
+    "interface_hash": "48002f2d6450b6c58be3e5dc3bbba8abd224cb4e4aba0c4a660b6afab0da5362",
+    "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/loaders/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_wrap.py",
     "plugin_data": null,
-    "size": 757,
+    "size": 1840,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/_types.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7014814814814815%*

 * *Differences: {"'data_mtime'": '1686754986',*

 * * "'dep_lines'": '{insert: [(0, 5), (1, 1), (2, 2), (3, 1), (4, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 20), (1, 5), (2, 5), (4, 30), (5, 30), (6, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.console'), (2, 'inspect'), (5, 'array'), (6, 'ctypes'), "*

 * *                   "(7, 'mmap'), (8, 'pickle')], delete: [2]}",*

 * * "'hash'": "'5adfb61d977aece622a295240933b3ee5337f2fca8e6bdc711067d4ce3c39794'",*

 * * "'id'": "'rich.protocol'",*

 * * "'interface_hash'": "'dbc101d777ba6400d696ff […]*

```diff
@@ -1,32 +1,47 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1686754986,
     "dep_lines": [
+        5,
+        1,
+        2,
+        1,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
+        20,
+        5,
         5,
+        5,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "rich.console",
         "typing",
+        "inspect",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "9dfc180741340abdc5dbdbb5b060f46a50d436b180e08c25f25211b1c3e31d7f",
-    "id": "configuraptor.loaders._types",
+    "hash": "5adfb61d977aece622a295240933b3ee5337f2fca8e6bdc711067d4ce3c39794",
+    "id": "rich.protocol",
     "ignore_all": true,
-    "interface_hash": "ff8bf54ace6de15cec9f2eb2c19a18138007d71a654544edb632d48f8f96a653",
-    "mtime": 1686825273,
+    "interface_hash": "dbc101d777ba6400d696ff7983fabed24a37029e0c5fe0e95847065368b141b2",
+    "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/loaders/_types.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/protocol.py",
     "plugin_data": null,
-    "size": 304,
+    "size": 1367,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904761904761905%*

 * *Differences: {"'names'": "{'toml': OrderedDict([('.class', 'SymbolTableNode'), ('kind', 'Gdef'), ('node', "*

 * *            "OrderedDict([('.class', 'FuncDef'), ('abstract_status', 0), ('arg_kinds', [0]), "*

 * *            "('arg_names', ['f']), ('dataclass_transform_spec', None), ('flags', []), ('fullname', "*

 * *            "'configuraptor.loaders.loaders_shared.toml'), ('name', 'toml'), ('type', "*

 * *            "OrderedDict([('.class', 'CallableType'), ('arg_kinds', [0]), ('arg_names', ['f']), "*

 * *            "('arg_types', ['typing […]*

```diff
@@ -154,14 +154,68 @@
         "json_lib": {
             ".class": "SymbolTableNode",
             "cross_ref": "json",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "toml": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0
+                ],
+                "arg_names": [
+                    "f"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "configuraptor.loaders.loaders_shared.toml",
+                "name": "toml",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        "f"
+                    ],
+                    "arg_types": [
+                        "typing.BinaryIO"
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "toml",
+                    "ret_type": {
+                        ".class": "TypeAliasType",
+                        "args": [],
+                        "type_ref": "configuraptor.loaders._types.T_config"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "tomlkit": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "tomlkit",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "yaml": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6619632414369256%*

 * *Differences: {"'data_mtime'": '1686754986',*

 * * "'dep_lines'": '{insert: [(0, 16), (1, 19), (2, 20), (3, 579), (6, 7), (7, 15), (12, 1), (13, 1), '*

 * *                '(14, 1), (15, 1), (16, 1), (17, 1)], delete: [7, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5), (3, 5), (7, 10), (12, 30), (13, 30), (14, 30), '*

 * *                '(15, 30), (16, 30), (17, 30)], delete: [7]}',*

 * * "'dependencies'": "{insert: [(0, 'ctypes.wintypes'), (1, 'rich.color'), (2, 'rich.style'), (3, "*

 * *                   "'rich.console'), (4, 'ctyp […]*

```diff
@@ -1,43 +1,74 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1686754986,
     "dep_lines": [
-        10,
+        16,
+        19,
+        20,
+        579,
         5,
         6,
+        7,
+        15,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
-        8
+        1,
+        1
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
+        5,
         5,
         10,
         5,
+        10,
         5,
         30,
         30,
         30,
-        10
+        30,
+        30,
+        30,
+        30,
+        30,
+        30
     ],
     "dependencies": [
-        "configuraptor.loaders._types",
-        "json",
+        "ctypes.wintypes",
+        "rich.color",
+        "rich.style",
+        "rich.console",
+        "ctypes",
+        "sys",
         "typing",
+        "time",
         "builtins",
         "_typeshed",
         "abc",
-        "json.decoder"
+        "array",
+        "enum",
+        "functools",
+        "mmap",
+        "pickle",
+        "rich.color_triplet",
+        "typing_extensions"
     ],
-    "hash": "bf69da103cf3f2578f877d8c8a90089aec0c108702d6bbd5d6ef5608059d09f9",
-    "id": "configuraptor.loaders.loaders_shared",
+    "hash": "f8db5e6a5b105d0e79f1efb3a49b64c21f31fdda82f928e500603cef674613a5",
+    "id": "rich._win32_console",
     "ignore_all": true,
-    "interface_hash": "cd6cb60fed8bb6ee969df9a0d9bb26ad09cf48fe44f3b03046c3b951b4db5e88",
-    "mtime": 1686825273,
+    "interface_hash": "4f75d220b2446d31efd07881418ba81ada3c0c96c6cd26363ae6f0a214580e8e",
+    "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -71,15 +102,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/loaders/loaders_shared.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_win32_console.py",
     "plugin_data": null,
-    "size": 464,
-    "suppressed": [
-        "yaml"
-    ],
+    "size": 22784,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/charset.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/charset.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/errors.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/errors.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/header.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/header.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/message.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/message.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/policy.data.json` & `su6-1.4.1/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/email/policy.meta.json` & `su6-1.4.1/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/html/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/html/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/html/entities.data.json` & `su6-1.4.1/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/html/entities.meta.json` & `su6-1.4.1/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/abc.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/util.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/util.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/json/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/json/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/json/decoder.data.json` & `su6-1.4.1/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/json/decoder.meta.json` & `su6-1.4.1/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/json/encoder.data.json` & `su6-1.4.1/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/json/encoder.meta.json` & `su6-1.4.1/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/logging/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-1.4.1/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/connection.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/context.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/context.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/managers.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/pool.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/process.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/process.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/queues.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/util.data.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/multiprocessing/util.meta.json` & `su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/os/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/os/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/os/path.data.json` & `su6-1.4.1/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/os/path.meta.json` & `su6-1.4.1/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_elffile.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_elffile.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_manylinux.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_musllinux.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_structures.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/_structures.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/specifiers.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/specifiers.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/tags.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/tags.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/version.data.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/packaging/version.meta.json` & `su6-1.4.1/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/_meta.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/_meta.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/gitignore.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/pathspec.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/pattern.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/pattern.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/util.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/util.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/android.data.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/android.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/android.meta.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/android.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/api.data.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/api.meta.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/unix.data.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/unix.meta.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/version.data.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/platformdirs/version.meta.json` & `su6-1.4.1/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/__main__.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_extension.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_loop.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_pick.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_stack.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_timer.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7897630549804463%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (2, 1), (3, 2)], delete: [7, 6, 5, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [7, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.default_styles'), (2, 'configparser'), (5, "*

 * *                   "'_collections_abc'), (10, 'io'), (11, 'rich.color')], delete: [15, 14, 11, 7, "*

 * *                   '5, 4, 3, 1, 0]}',*

 * * "'hash'": "'6de9452688330345b41f2b1069b29a1ce7374561f6928ddf400261a0df8015da'",*

 * * "'id'": "'rich.theme'",*

 * * "'interface_hash'": "'671224b38692c5693718c24b69b92c554 […]*

```diff
@@ -1,73 +1,61 @@
 {
     "data_mtime": 1686754986,
     "dep_lines": [
-        16,
-        19,
-        20,
-        579,
+        4,
         5,
-        6,
-        7,
-        15,
+        1,
+        2,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
         5,
         5,
         10,
         5,
-        10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "ctypes.wintypes",
-        "rich.color",
+        "rich.default_styles",
         "rich.style",
-        "rich.console",
-        "ctypes",
-        "sys",
+        "configparser",
         "typing",
-        "time",
         "builtins",
+        "_collections_abc",
         "_typeshed",
         "abc",
-        "array",
         "enum",
         "functools",
-        "mmap",
-        "pickle",
+        "io",
+        "rich.color",
         "rich.color_triplet",
         "typing_extensions"
     ],
-    "hash": "f8db5e6a5b105d0e79f1efb3a49b64c21f31fdda82f928e500603cef674613a5",
-    "id": "rich._win32_console",
+    "hash": "6de9452688330345b41f2b1069b29a1ce7374561f6928ddf400261a0df8015da",
+    "id": "rich.theme",
     "ignore_all": true,
-    "interface_hash": "4f75d220b2446d31efd07881418ba81ada3c0c96c6cd26363ae6f0a214580e8e",
+    "interface_hash": "671224b38692c5693718c24b69b92c55432f6ec13ce9c452261d573a898484c0",
     "mtime": 1686754199,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -102,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_win32_console.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/theme.py",
     "plugin_data": null,
-    "size": 22784,
+    "size": 3777,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_windows.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7104166666666667%*

 * *Differences: {"'data_mtime'": '1686754987',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 8), (4, 3), (5, 5)], delete: [6, 5, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 5), (6, 5)], delete: [7, 6, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._typing'), (1, 'typer.models'), (2, 'inspect'), (3, "*

 * *                   "'copy'), (5, 'typing_extensions'), (8, 'click'), (9, 'click.core'), (10, "*

 * *                   "'click.shell_completion'), (11, 'click.types'), (12, 'types')], delete: [13, "*

 * *                   '12, 11, 10, 9, 7, 6, […]*

```diff
@@ -1,62 +1,59 @@
 {
-    "data_mtime": 1686754986,
+    "data_mtime": 1686754987,
     "dep_lines": [
-        4,
-        5,
-        52,
+        7,
+        8,
         1,
         2,
-        1,
-        1,
+        3,
+        5,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
         10,
         5,
         5,
-        30,
-        30,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "rich._loop",
-        "rich.cells",
-        "rich.console",
-        "re",
+        "typer._typing",
+        "typer.models",
+        "inspect",
+        "copy",
         "typing",
+        "typing_extensions",
         "builtins",
-        "_random",
-        "_typeshed",
         "abc",
-        "datetime",
-        "rich.jupyter",
-        "rich.style",
-        "rich.text",
-        "rich.theme"
+        "click",
+        "click.core",
+        "click.shell_completion",
+        "click.types",
+        "types"
     ],
-    "hash": "c5f57ff6dd1283aaf38a69ab0ebbbc7c25665256a56007072c37eb2599db6f04",
-    "id": "rich._wrap",
+    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
+    "id": "typer.utils",
     "ignore_all": true,
-    "interface_hash": "48002f2d6450b6c58be3e5dc3bbba8abd224cb4e4aba0c4a660b6afab0da5362",
-    "mtime": 1686754199,
+    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -90,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_wrap.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
     "plugin_data": null,
-    "size": 1840,
+    "size": 7293,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/abc.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/abc.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/align.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/align.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/ansi.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/box.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/box.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/cells.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/cells.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/color.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/color.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/columns.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/columns.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/console.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/console.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/constrain.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/containers.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/containers.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/control.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/control.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/emoji.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/errors.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/errors.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/json.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/json.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/live.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/live.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/live_render.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/markdown.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/markup.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/markup.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/measure.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/measure.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/padding.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/padding.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/pager.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/pager.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/palette.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/palette.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/panel.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/panel.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/pretty.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/protocol.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7024242424242424%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(2, 3)], delete: [5, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [7, 6, 5, 4, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'typeguard._config'), (1, '__future__')], delete: [8, 7, 6, 5, "*

 * *                   '2, 0]}',*

 * * "'hash'": "'d63b9057fbf19c3d8960a6d2ade6e242e8f8a0a1f3ea7ebbbfda5803e0822128'",*

 * * "'id'": "'typeguard._memo'",*

 * * "'interface_hash'": "'29cb6a6c75f7bc7d1a048564aafabe9eb08cfecd68659b25796379799f0a3598'",*

 * * "'mtime'": '1686754196', […]*

```diff
@@ -1,47 +1,35 @@
 {
-    "data_mtime": 1686754986,
+    "data_mtime": 1686754984,
     "dep_lines": [
         5,
         1,
-        2,
-        1,
-        1,
-        1,
-        1,
+        3,
         1,
         1
     ],
     "dep_prios": [
-        20,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
+        5,
         30
     ],
     "dependencies": [
-        "rich.console",
+        "typeguard._config",
+        "__future__",
         "typing",
-        "inspect",
         "builtins",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "abc"
     ],
-    "hash": "5adfb61d977aece622a295240933b3ee5337f2fca8e6bdc711067d4ce3c39794",
-    "id": "rich.protocol",
+    "hash": "d63b9057fbf19c3d8960a6d2ade6e242e8f8a0a1f3ea7ebbbfda5803e0822128",
+    "id": "typeguard._memo",
     "ignore_all": true,
-    "interface_hash": "dbc101d777ba6400d696ff7983fabed24a37029e0c5fe0e95847065368b141b2",
-    "mtime": 1686754199,
+    "interface_hash": "29cb6a6c75f7bc7d1a048564aafabe9eb08cfecd68659b25796379799f0a3598",
+    "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/protocol.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_memo.py",
     "plugin_data": null,
-    "size": 1367,
+    "size": 1303,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/region.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/region.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/repr.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/repr.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/rule.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/rule.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/scope.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/scope.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/screen.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/screen.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/segment.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/segment.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/spinner.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/status.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/status.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/style.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/style.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/styled.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/styled.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/syntax.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/table.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/table.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/text.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/text.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/theme.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/theme.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/items.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6998207885304659%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(0, 24), (1, 26), (2, 28), (3, 47), (4, 1), (5, 3), (8, 6), (9, 7), '*

 * *                '(10, 9), (11, 13), (12, 14), (13, 43), (14, 47)], delete: [6, 5, 4, 3, 2]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (3, 20), (5, 10), (6, 10), (7, 10), (8, 10), (12, 5), '*

 * *                '(13, 25), (14, 25)], delete: [6, 5]}',*

 * * "'dependencies'": "{insert: [(0, 'tomlkit._compat'), (1, 'tomlkit._utils'), (2, "*

 * *                   "'tomlkit.exceptions'), (3, 'toml […]*

```diff
@@ -1,62 +1,86 @@
 {
-    "data_mtime": 1686754986,
+    "data_mtime": 1686754984,
     "dep_lines": [
+        24,
+        26,
+        28,
+        47,
+        1,
+        3,
         4,
         5,
-        1,
-        2,
-        1,
-        1,
-        1,
+        6,
+        7,
+        9,
+        13,
+        14,
+        43,
+        47,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        20,
+        5,
+        10,
+        10,
+        10,
+        10,
         10,
         5,
         5,
-        30,
-        30,
+        5,
+        25,
+        25,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "rich.default_styles",
-        "rich.style",
-        "configparser",
+        "tomlkit._compat",
+        "tomlkit._utils",
+        "tomlkit.exceptions",
+        "tomlkit.container",
+        "__future__",
+        "abc",
+        "copy",
+        "dataclasses",
+        "re",
+        "string",
+        "datetime",
+        "enum",
         "typing",
         "builtins",
+        "tomlkit",
         "_collections_abc",
         "_typeshed",
-        "abc",
-        "enum",
-        "functools",
-        "io",
-        "rich.color",
-        "rich.color_triplet",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle",
         "typing_extensions"
     ],
-    "hash": "6de9452688330345b41f2b1069b29a1ce7374561f6928ddf400261a0df8015da",
-    "id": "rich.theme",
+    "hash": "a90d23cb34b1d1aa652baa9da4853eee31060b96c7a384ccbba6cfc67918f93b",
+    "id": "tomlkit.items",
     "ignore_all": true,
-    "interface_hash": "671224b38692c5693718c24b69b92c55432f6ec13ce9c452261d573a898484c0",
-    "mtime": 1686754199,
+    "interface_hash": "5a29adcf2fd24d5dc7fe78bb09b62f6525f03e0aab8dc540ce25be4ebfc1b422",
+    "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -90,13 +114,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/theme.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/items.py",
     "plugin_data": null,
-    "size": 3777,
+    "size": 51695,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/themes.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/themes.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7092592592592593%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(0, 5), (3, 3), (4, 4)], delete: [2]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (5, 5)], delete: [3]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (1, 'logging'), (2, 'sys'), (3, 'types'), (4, "*

 * *                   "'typing'), (6, '_typeshed')], delete: [5, 4, 1, 0]}",*

 * * "'hash'": "'297a51a36613ffcd84bcef772c3f0dd0fdb57a1a9acc544a72840468647d968c'",*

 * * "'id'": "'unittest._log'",*

 * * "'interface_hash'": "'20b576be7b25765af8108589e0827b19be51be5 […]*

```diff
@@ -1,38 +1,44 @@
 {
-    "data_mtime": 1686754986,
+    "data_mtime": 1686754984,
     "dep_lines": [
+        5,
         1,
         2,
-        1,
+        3,
+        4,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        10,
+        5,
         5,
         5,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "rich.default_styles",
-        "rich.theme",
+        "unittest.case",
+        "logging",
+        "sys",
+        "types",
+        "typing",
         "builtins",
-        "abc",
-        "rich.style",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459",
-    "id": "rich.themes",
+    "hash": "297a51a36613ffcd84bcef772c3f0dd0fdb57a1a9acc544a72840468647d968c",
+    "id": "unittest._log",
     "ignore_all": true,
-    "interface_hash": "c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a",
-    "mtime": 1686754199,
+    "interface_hash": "20b576be7b25765af8108589e0827b19be51be5c76414d2ce9027946fcb1ee5c",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/themes.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi",
     "plugin_data": null,
-    "size": 102,
+    "size": 892,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/traceback.data.json` & `su6-1.4.1/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-1.4.1/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/__about__.data.json` & `su6-1.4.1/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/__about__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7666666666666667%*

 * *Differences: {"'hash'": "'32ed36840fbe0e18b032d8f86ca33c819ea7e7d9d03e44b97f6c3a7dfd5133e5'",*

 * * "'id'": "'configuraptor.helpers'",*

 * * "'ignore_all'": 'True',*

 * * "'interface_hash'": "'fa6a613a7e56d42069a3559eed13704a7e16ad1e811c5e6ce4b0e40d2372f0fc'",*

 * * "'mtime'": '1687189299',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/helpers.py'",*

 * * "'size'": '344'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "e4298c09389500b4458b3d86c3b2d563a462aac32c04d730e316d5a0982c475f",
-    "id": "su6.__about__",
-    "ignore_all": false,
-    "interface_hash": "f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9",
-    "mtime": 1686831591,
+    "hash": "32ed36840fbe0e18b032d8f86ca33c819ea7e7d9d03e44b97f6c3a7dfd5133e5",
+    "id": "configuraptor.helpers",
+    "ignore_all": true,
+    "interface_hash": "fa6a613a7e56d42069a3559eed13704a7e16ad1e811c5e6ce4b0e40d2372f0fc",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6/__about__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/helpers.py",
     "plugin_data": null,
-    "size": 206,
+    "size": 344,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/cli.data.json` & `su6-1.4.1/.mypy_cache/3.11/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/cli.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6385406134142232%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(0, 7), (2, 9), (3, 14), (4, 15), (5, 16), (6, 1)], delete: [36, 35, '*

 * *                '22, 21, 20, 19, 18, 17, 16, 15, 14, 13, 12, 11, 10, 8, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (8, 10), (10, 20)], delete: [36, 35, 23, 22, 21, 20, 19, 18, '*

 * *                '17, 16, 15, 12, 8, 7, 6, 5, 4]}',*

 * * "'dependencies'": "{insert: [(0, 'typeguard._suppression'), (1, 'typeguard._checkers'), (2, "*

 * *                   "'typeguard._config'), (3, 'type […]*

```diff
@@ -1,129 +1,89 @@
 {
-    "data_mtime": 1686818222,
+    "data_mtime": 1686754984,
     "dep_lines": [
+        7,
         8,
-        17,
-        18,
-        37,
-        2,
+        9,
+        14,
+        15,
+        16,
+        1,
         3,
         4,
         5,
-        6,
         7,
-        9,
-        11,
-        12,
-        15,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        14,
-        13
+        1
     ],
     "dep_prios": [
+        10,
         5,
         5,
         5,
         5,
-        10,
-        10,
-        10,
-        10,
-        10,
         5,
         5,
         10,
+        10,
         5,
+        20,
         5,
-        5,
-        30,
-        30,
-        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "importlib.metadata",
-        "su6.__about__",
-        "su6.core",
-        "su6.plugins",
-        "contextlib",
-        "math",
-        "os",
+        "typeguard._suppression",
+        "typeguard._checkers",
+        "typeguard._config",
+        "typeguard._exceptions",
+        "typeguard._memo",
+        "typeguard._utils",
+        "__future__",
         "sys",
+        "warnings",
         "typing",
-        "dataclasses",
-        "json",
-        "typer",
-        "configuraptor",
-        "rich",
+        "typeguard",
         "builtins",
+        "_collections_abc",
         "_typeshed",
+        "_warnings",
         "abc",
         "array",
-        "click",
-        "click.core",
-        "click.exceptions",
-        "configuraptor.cls",
-        "configuraptor.singleton",
         "ctypes",
         "enum",
-        "importlib",
-        "io",
-        "json.decoder",
         "mmap",
         "pickle",
-        "typer.core",
-        "typer.main",
-        "typer.models",
         "types",
         "typing_extensions"
     ],
-    "hash": "c779aeec5d3a739944c39e10191900e3250189ebacdcb3782d0317031961f32e",
-    "id": "su6.cli",
-    "ignore_all": false,
-    "interface_hash": "0df9143d2f97cb5869342bf9eb6560aed886c3ab9e5ba659a12c9e5fb3664420",
-    "mtime": 1686818322,
+    "hash": "b2e3083306125d7116f78f25f385c22e6c8d0fb36e0bce0821cac30a704e2c59",
+    "id": "typeguard._functions",
+    "ignore_all": true,
+    "interface_hash": "242cbdd43c602485bc96011c202a9c336f14cb3fb45db7856d4642368e3eaea2",
+    "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -157,16 +117,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6/cli.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_functions.py",
     "plugin_data": null,
-    "size": 12942,
-    "suppressed": [
-        "plumbum.machines",
-        "plumbum"
-    ],
+    "size": 10178,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/core.data.json` & `su6-1.4.1/.mypy_cache/3.11/su6/core.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999872582754387%*

 * *Differences: {"'names'": "{'AbstractConfig': {'node': {'names': {delete: ['update']}}}, 'ApplicationState': "*

 * *            "{'node': {'metadata': {'dataclass': {'attributes': {0: {'line': 465}, 1: {'line': "*

 * *            "466}, 2: {'line': 467}, 3: {'line': 468}}}}}}, 'Config': {'node': {'metadata': "*

 * *            "{'dataclass': {'attributes': {0: {'line': 293}, 1: {'line': 294}, 2: {'line': 295}, "*

 * *            "3: {'line': 296}, 4: {'line': 297}, 5: {'line': 298}, 6: {'line': 301}, 7: {'line': "*

 * *            "302}}}}}}, 'M […]*

```diff
@@ -52,79 +52,14 @@
                                 "is_inferred",
                                 "has_explicit_value"
                             ],
                             "fullname": "su6.core.AbstractConfig._strict",
                             "name": "_strict",
                             "type": "builtins.bool"
                         }
-                    },
-                    "update": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                1,
-                                1,
-                                4
-                            ],
-                            "arg_names": [
-                                "self",
-                                "strict",
-                                "allow_none",
-                                "kw"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6.core.AbstractConfig.update",
-                            "name": "update",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    1,
-                                    1,
-                                    4
-                                ],
-                                "arg_names": [
-                                    "self",
-                                    "strict",
-                                    "allow_none",
-                                    "kw"
-                                ],
-                                "arg_types": [
-                                    "su6.core.AbstractConfig",
-                                    "builtins.bool",
-                                    "builtins.bool",
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "update of AbstractConfig",
-                                "ret_type": {
-                                    ".class": "NoneType"
-                                },
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
                     }
                 },
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
@@ -161,39 +96,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 482,
+                                "line": 465,
                                 "name": "verbosity",
                                 "type": "su6.core.Verbosity"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 483,
+                                "line": 466,
                                 "name": "output_format",
                                 "type": "su6.core.Format"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 484,
+                                "line": 467,
                                 "name": "config_file",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.str",
                                         {
                                             ".class": "NoneType"
@@ -205,15 +140,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 485,
+                                "line": 468,
                                 "name": "config",
                                 "type": {
                                     ".class": "TypeAliasType",
                                     "args": [],
                                     "type_ref": "su6.core.MaybeConfig"
                                 }
                             }
@@ -869,39 +804,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 310,
+                                "line": 293,
                                 "name": "directory",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 311,
+                                "line": 294,
                                 "name": "pyproject",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 312,
+                                "line": 295,
                                 "name": "include",
                                 "type": {
                                     ".class": "Instance",
                                     "args": [
                                         "builtins.str"
                                     ],
                                     "type_ref": "builtins.list"
@@ -911,15 +846,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 313,
+                                "line": 296,
                                 "name": "exclude",
                                 "type": {
                                     ".class": "Instance",
                                     "args": [
                                         "builtins.str"
                                     ],
                                     "type_ref": "builtins.list"
@@ -929,39 +864,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 314,
+                                "line": 297,
                                 "name": "stop_after_first_failure",
                                 "type": "builtins.bool"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 315,
+                                "line": 298,
                                 "name": "json_indent",
                                 "type": "builtins.int"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 318,
+                                "line": 301,
                                 "name": "coverage",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.float",
                                         {
                                             ".class": "NoneType"
@@ -973,15 +908,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 319,
+                                "line": 302,
                                 "name": "badge",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.bool",
                                         "builtins.str"
                                     ]
@@ -2082,15 +2017,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.MaybeConfig",
-                "line": 358,
+                "line": 341,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "su6.core.Config",
                         {
@@ -2371,15 +2306,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_typelike",
-                "line": 360,
+                "line": 343,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.type",
                         "types.UnionType",
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/core.meta.json` & `su6-1.4.1/.mypy_cache/3.11/su6/core.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'data_mtime'": '1687189421',*

 * * "'hash'": "'eda027f7f0be13894f581974ded78b8762f9392850896656a1f7154e95b7ea95'",*

 * * "'interface_hash'": "'44b0e2fe8bc46a5deade667766ef5320be166c0d7d3efa7f3b6392a11ef10abd'",*

 * * "'mtime'": '1687189338',*

 * * "'size'": '17551'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1686831824,
+    "data_mtime": 1687189421,
     "dep_lines": [
         16,
         4,
         5,
         6,
         7,
         8,
@@ -112,19 +112,19 @@
         "io",
         "json.encoder",
         "mmap",
         "pathlib",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "d4a1072c926d419a54832f95bc2ad533e0be4a3e29db1e17dc92dc42b0f2d6ce",
+    "hash": "eda027f7f0be13894f581974ded78b8762f9392850896656a1f7154e95b7ea95",
     "id": "su6.core",
     "ignore_all": false,
-    "interface_hash": "97ffc176d42ace42bacf7110a8a8731290e0499984f34b1db9c293f9078b8f4e",
-    "mtime": 1686831820,
+    "interface_hash": "44b0e2fe8bc46a5deade667766ef5320be166c0d7d3efa7f3b6392a11ef10abd",
+    "mtime": 1687189338,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -160,15 +160,15 @@
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
     "path": "src/su6/core.py",
     "plugin_data": null,
-    "size": 18263,
+    "size": 17551,
     "suppressed": [
         "plumbum.commands.processes",
         "plumbum.commands",
         "plumbum.machines",
         "plumbum"
     ],
     "version_id": "1.3.0"
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/plugins.data.json` & `su6-1.4.1/.mypy_cache/3.11/su6/plugins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/su6/plugins.meta.json` & `su6-1.4.1/.mypy_cache/3.11/su6/plugins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/_compat.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/_compat.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/_utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/_utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/api.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/api.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/container.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/container.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/container.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/container.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/exceptions.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/exceptions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/items.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/items.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/items.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7358909608909608%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 12), (1, 13), (2, 14), (3, 15), (4, 16), (10, 8), (12, 10), (13, '*

 * *                '1), (14, 1), (15, 1), (16, 1), (17, 1), (18, 1), (26, 19)], delete: [14, 13, 12, '*

 * *                '11, 9, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5), (7, 5), (12, 5), (13, 5), (14, 30), (15, 30), (16, 30), '*

 * *                '(17, 30), (18, 30), (26, 25)], delete: [14, 13, 7, 6, 5, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'typeguard._config'), (1, 'typeguard._exceptions'), (2, "*

 * *   […]*

```diff
@@ -1,85 +1,99 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
-        24,
-        26,
-        28,
-        47,
+        12,
+        13,
+        14,
+        15,
+        16,
         1,
         3,
         4,
         5,
         6,
-        7,
+        8,
         9,
-        13,
-        14,
-        43,
-        47,
+        10,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        1,
+        19
     ],
     "dep_prios": [
         5,
         5,
         5,
-        20,
+        5,
+        5,
         5,
         10,
+        5,
         10,
-        10,
-        10,
-        10,
         5,
         5,
         5,
-        25,
-        25,
+        5,
+        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        30,
+        25
     ],
     "dependencies": [
-        "tomlkit._compat",
-        "tomlkit._utils",
-        "tomlkit.exceptions",
-        "tomlkit.container",
+        "typeguard._config",
+        "typeguard._exceptions",
+        "typeguard._functions",
+        "typeguard._transformer",
+        "typeguard._utils",
         "__future__",
-        "abc",
-        "copy",
-        "dataclasses",
-        "re",
-        "string",
-        "datetime",
-        "enum",
+        "ast",
+        "inspect",
+        "sys",
+        "functools",
+        "types",
         "typing",
+        "warnings",
         "builtins",
-        "tomlkit",
-        "_collections_abc",
+        "_ast",
         "_typeshed",
+        "_warnings",
+        "abc",
         "array",
         "ctypes",
+        "enum",
         "mmap",
+        "os",
         "pickle",
+        "typeguard._memo",
         "typing_extensions"
     ],
-    "hash": "a90d23cb34b1d1aa652baa9da4853eee31060b96c7a384ccbba6cfc67918f93b",
-    "id": "tomlkit.items",
+    "hash": "53fe9d30f679933d28ca0abf31119f667ef0e129702443c44b45d2ca3d8b09eb",
+    "id": "typeguard._decorators",
     "ignore_all": true,
-    "interface_hash": "5a29adcf2fd24d5dc7fe78bb09b62f6525f03e0aab8dc540ce25be4ebfc1b422",
+    "interface_hash": "448d7566fffd81900a553f71b082112bb8dc84dd4d7131fee1f6a092eeb74e54",
     "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -114,13 +128,15 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/tomlkit/items.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_decorators.py",
     "plugin_data": null,
-    "size": 51695,
-    "suppressed": [],
+    "size": 8768,
+    "suppressed": [
+        "typeshed.stdlib.types"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/parser.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/parser.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/source.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/source.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/source.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/source.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_char.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_char.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_document.data.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/tomlkit/toml_document.meta.json` & `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_checkers.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_config.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_config.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_decorators.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7538225391166568%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 61), (5, 60), (6, 62), (7, 63), (8, 64), (9, 65)], delete: [26, 14, '*

 * *                '13, 12, 11, 10, 9, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [26, 14, 7, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (3, 'builtins'), (5, 'collections'), (6, "*

 * *                   "'contextlib'), (7, 'copy'), (8, 'dataclasses'), (11, '_collections_abc'), (19, "*

 * *                   "'types')], delete: [24, 20, 16, 13, 12, 10, 9, 7, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'e0fb1aed […]*

```diff
@@ -1,47 +1,37 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
-        12,
-        13,
-        14,
-        15,
-        16,
+        61,
         1,
         3,
         4,
         5,
-        6,
-        8,
-        9,
-        10,
-        1,
-        1,
-        1,
+        60,
+        62,
+        63,
+        64,
+        65,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        19
+        1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
-        5,
-        5,
         10,
-        5,
         10,
         5,
         5,
         5,
         5,
         5,
         30,
@@ -50,50 +40,43 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        25
+        30
     ],
     "dependencies": [
-        "typeguard._config",
-        "typeguard._exceptions",
-        "typeguard._functions",
-        "typeguard._transformer",
-        "typeguard._utils",
+        "collections.abc",
         "__future__",
         "ast",
-        "inspect",
+        "builtins",
         "sys",
-        "functools",
-        "types",
+        "collections",
+        "contextlib",
+        "copy",
+        "dataclasses",
         "typing",
-        "warnings",
-        "builtins",
         "_ast",
+        "_collections_abc",
         "_typeshed",
-        "_warnings",
         "abc",
         "array",
         "ctypes",
-        "enum",
         "mmap",
         "os",
         "pickle",
-        "typeguard._memo",
+        "types",
         "typing_extensions"
     ],
-    "hash": "53fe9d30f679933d28ca0abf31119f667ef0e129702443c44b45d2ca3d8b09eb",
-    "id": "typeguard._decorators",
+    "hash": "e0fb1aeda2ddbf5a158dea92e7713dbc78e4124a17a482fee592bf8fb951f864",
+    "id": "typeguard._transformer",
     "ignore_all": true,
-    "interface_hash": "448d7566fffd81900a553f71b082112bb8dc84dd4d7131fee1f6a092eeb74e54",
+    "interface_hash": "f15b8806901a43a21e5cffa258aaad715b243b35a6e8a89cc9d141bf574a3c58",
     "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -128,15 +111,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_decorators.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_transformer.py",
     "plugin_data": null,
-    "size": 8768,
-    "suppressed": [
-        "typeshed.stdlib.types"
-    ],
+    "size": 41863,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_functions.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_functions.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7063188405797102%*

 * *Differences: {"'data_mtime'": '1686754987',*

 * * "'dep_lines'": '{delete: [12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [14, 13, 12, 10, 9, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click'), (8, 'typing')], delete: [21, 18, 14, 12, 10, 9, 8, 7, "*

 * *                   '6, 5, 4, 3, 2, 1, 0]}',*

 * * "'hash'": "'929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a'",*

 * * "'id'": "'typer._compat_utils'",*

 * * "'interface_hash'": "'f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5 […]*

```diff
@@ -1,89 +1,50 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1686754987,
     "dep_lines": [
-        7,
-        8,
-        9,
-        14,
-        15,
-        16,
-        1,
-        3,
-        4,
-        5,
-        7,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        10,
-        10,
-        5,
-        20,
-        5,
-        30,
-        30,
-        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "typeguard._suppression",
-        "typeguard._checkers",
-        "typeguard._config",
-        "typeguard._exceptions",
-        "typeguard._memo",
-        "typeguard._utils",
-        "__future__",
-        "sys",
-        "warnings",
-        "typing",
-        "typeguard",
+        "click",
         "builtins",
-        "_collections_abc",
         "_typeshed",
-        "_warnings",
         "abc",
         "array",
         "ctypes",
-        "enum",
         "mmap",
         "pickle",
-        "types",
+        "typing",
         "typing_extensions"
     ],
-    "hash": "b2e3083306125d7116f78f25f385c22e6c8d0fb36e0bce0821cac30a704e2c59",
-    "id": "typeguard._functions",
+    "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
+    "id": "typer._compat_utils",
     "ignore_all": true,
-    "interface_hash": "242cbdd43c602485bc96011c202a9c336f14cb3fb45db7856d4642368e3eaea2",
-    "mtime": 1686754196,
+    "interface_hash": "f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -117,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_functions.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_compat_utils.py",
     "plugin_data": null,
-    "size": 10178,
+    "size": 94,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_importhook.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_memo.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_memo.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7742424242424242%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (3, 5), (4, 6), (5, 7), (6, 8), (7, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 10), (3, 5), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, 'sys'), (3, 'contextlib'), (4, "*

 * *                   "'functools'), (5, 'threading'), (8, '_typeshed')], delete: [0]}",*

 * * "'hash'": "'b4f851605bb29ea55ec63a54141356440441f215f0fdbd6db502c5101dcaa286'",*

 * * "'id'": "'typeguard._suppression'",*

 * * "'interface_hash'": "'a1a70d160de28cf0199ebcd05e2ccf6 […]*

```diff
@@ -1,34 +1,49 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
-        5,
+        4,
         1,
         3,
+        5,
+        6,
+        7,
+        8,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        10,
+        5,
+        5,
+        5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "typeguard._config",
+        "collections.abc",
         "__future__",
+        "sys",
+        "contextlib",
+        "functools",
+        "threading",
         "typing",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "d63b9057fbf19c3d8960a6d2ade6e242e8f8a0a1f3ea7ebbbfda5803e0822128",
-    "id": "typeguard._memo",
+    "hash": "b4f851605bb29ea55ec63a54141356440441f215f0fdbd6db502c5101dcaa286",
+    "id": "typeguard._suppression",
     "ignore_all": true,
-    "interface_hash": "29cb6a6c75f7bc7d1a048564aafabe9eb08cfecd68659b25796379799f0a3598",
+    "interface_hash": "a1a70d160de28cf0199ebcd05e2ccf6786bcc458764dfebb7febf26fefdab58e",
     "mtime": 1686754196,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_memo.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_suppression.py",
     "plugin_data": null,
-    "size": 1303,
+    "size": 2273,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_suppression.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `su6-1.4.1/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6927272727272727%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{delete: [6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [8, 6, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'",*

 * * "'id'": "'urllib'",*

 * * "'interface_hash'": "'697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3'",*

 * * "'mtime'": '1686754198',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packa […]*

```diff
@@ -1,50 +1,29 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1686754983,
     "dep_lines": [
-        4,
-        1,
-        3,
-        5,
-        6,
-        7,
-        8,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        10,
-        5,
-        5,
-        5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "__future__",
-        "sys",
-        "contextlib",
-        "functools",
-        "threading",
-        "typing",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "b4f851605bb29ea55ec63a54141356440441f215f0fdbd6db502c5101dcaa286",
-    "id": "typeguard._suppression",
+    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+    "id": "urllib",
     "ignore_all": true,
-    "interface_hash": "a1a70d160de28cf0199ebcd05e2ccf6786bcc458764dfebb7febf26fefdab58e",
-    "mtime": 1686754196,
+    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_suppression.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
     "plugin_data": null,
-    "size": 2273,
+    "size": 0,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_transformer.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7118104118104118%*

 * *Differences: {"'data_mtime'": '1686754987',*

 * * "'dep_lines'": '{insert: [(0, 101), (1, 491), (3, 6), (4, 7), (5, 29), (6, 43)], delete: [12, 11, '*

 * *                '10, 9, 8, 7, 6, 5, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 20)], delete: [13, 12, 11, 10, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'typer.utils'), (3, 'os'), (5, 'typing_extensions'), (6, "*

 * *                   "'types'), (7, 'builtins')], delete: [20, 19, 17, 10, 8, 7, 6, 5, 3, 2, 1]}",*

 * * "'hash'": "'1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c6 […]*

```diff
@@ -1,83 +1,65 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1686754987,
     "dep_lines": [
-        61,
-        1,
-        3,
-        4,
+        101,
+        491,
         5,
-        60,
-        62,
-        63,
-        64,
-        65,
-        1,
-        1,
-        1,
+        6,
+        7,
+        29,
+        43,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
-        10,
+        20,
         10,
         5,
         5,
         5,
         5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "__future__",
-        "ast",
-        "builtins",
+        "typer.utils",
         "sys",
-        "collections",
-        "contextlib",
-        "copy",
-        "dataclasses",
+        "os",
         "typing",
-        "_ast",
+        "typing_extensions",
+        "types",
+        "builtins",
         "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
-        "os",
-        "pickle",
-        "types",
-        "typing_extensions"
+        "pickle"
     ],
-    "hash": "e0fb1aeda2ddbf5a158dea92e7713dbc78e4124a17a482fee592bf8fb951f864",
-    "id": "typeguard._transformer",
+    "hash": "1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c65f2b52adc389",
+    "id": "typer._typing",
     "ignore_all": true,
-    "interface_hash": "f15b8806901a43a21e5cffa258aaad715b243b35a6e8a89cc9d141bf574a3c58",
-    "mtime": 1686754196,
+    "interface_hash": "0f3d3599045f3d24c61dcdc82fc0d7878684a5647fb9689d5be4c96189e04edc",
+    "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -111,13 +93,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_transformer.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_typing.py",
     "plugin_data": null,
-    "size": 41863,
+    "size": 19743,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typeguard/_utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7179193899782135%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 4), (4, 5), (6, 6), (7, 7)], delete: [5, 4, 3, 2, '*

 * *                '1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (2, 10), (5, 20), (6, 5), (7, 5), (8, 5)], delete: '*

 * *                '[8, 7, 6, 5, 4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (1, 'unittest.loader'), (2, "*

 * *                   "'unittest.result'), (3, 'unittest.suite'), (4, 'collections.abc'), (5, "*

 * *                   "'unittest'), (6, 'typ […]*

```diff
@@ -1,49 +1,49 @@
 {
-    "data_mtime": 1686754987,
+    "data_mtime": 1686754984,
     "dep_lines": [
         1,
+        2,
+        3,
+        4,
+        5,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
+        6,
+        7,
         1,
         1
     ],
     "dep_prios": [
         10,
+        10,
+        10,
+        10,
+        5,
+        20,
+        5,
+        5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "click",
-        "builtins",
-        "_typeshed",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
+        "unittest.case",
+        "unittest.loader",
+        "unittest.result",
+        "unittest.suite",
+        "collections.abc",
+        "unittest",
+        "types",
         "typing",
-        "typing_extensions"
+        "builtins",
+        "abc"
     ],
-    "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
-    "id": "typer._compat_utils",
+    "hash": "f150ef9438e591e3d629f0eefd7b3236c18528d8e0a103ed15774b156b554302",
+    "id": "unittest.main",
     "ignore_all": true,
-    "interface_hash": "f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b",
+    "interface_hash": "4559180cb5aeda49873e488baf300d3d50e45f5d79850f3e785c1dee6a916d7c",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_compat_utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/main.pyi",
     "plugin_data": null,
-    "size": 94,
+    "size": 1544,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_typing.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7627594627594628%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 10), (1, 11), (2, 12), (3, 13), (4, 14), (5, 15), (6, 16), (7, 17), '*

 * *                '(8, 18), (9, 19), (10, 20), (11, 21), (12, 240), (13, 3), (14, 4), (18, 9), (19, '*

 * *                '10), (20, 1), (21, 1), (22, 1), (23, 1), (24, 1), (25, 1), (26, 1), (27, 1), (28, '*

 * *                '1), (29, 1)], delete: [6, 5, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (7, 5), (8, '*

 * *                '5), (9, 5), (10, 5), (14, 10), (18, 10), […]*

```diff
@@ -1,64 +1,133 @@
 {
     "data_mtime": 1686754987,
     "dep_lines": [
-        101,
-        491,
+        10,
+        11,
+        12,
+        13,
+        14,
+        15,
+        16,
+        17,
+        18,
+        19,
+        20,
+        21,
+        240,
+        3,
+        4,
         5,
         6,
         7,
-        29,
-        43,
+        9,
+        10,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
         5,
         20,
         10,
+        10,
         5,
         5,
         5,
+        10,
+        20,
         5,
-        5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "typer.utils",
+        "rich.box",
+        "rich.align",
+        "rich.columns",
+        "rich.console",
+        "rich.emoji",
+        "rich.highlighter",
+        "rich.markdown",
+        "rich.padding",
+        "rich.panel",
+        "rich.table",
+        "rich.text",
+        "rich.theme",
+        "typer.core",
+        "inspect",
         "sys",
+        "collections",
         "os",
         "typing",
-        "typing_extensions",
-        "types",
+        "click",
+        "rich",
         "builtins",
         "_collections_abc",
+        "_random",
         "_typeshed",
         "abc",
         "array",
+        "click.core",
+        "click.exceptions",
+        "click.shell_completion",
+        "click.types",
         "ctypes",
+        "datetime",
         "mmap",
-        "pickle"
+        "pickle",
+        "rich.jupyter",
+        "rich.style",
+        "types",
+        "typing_extensions"
     ],
-    "hash": "1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c65f2b52adc389",
-    "id": "typer._typing",
+    "hash": "73518e6d145375bea4e7298a3c057f534091fd529c975c4f775c2376751839c7",
+    "id": "typer.rich_utils",
     "ignore_all": true,
-    "interface_hash": "0f3d3599045f3d24c61dcdc82fc0d7878684a5647fb9689d5be4c96189e04edc",
+    "interface_hash": "5d907b3cb6c8118bae55ac813280c883d3f38ee428ffaf2ac0527a58e189466e",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -93,13 +162,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_typing.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/rich_utils.py",
     "plugin_data": null,
-    "size": 19743,
+    "size": 23654,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/colors.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/colors.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/completion.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/completion.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/core.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/core.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/main.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/main.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/models.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/models.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/params.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/params.meta.json` & `su6-1.4.1/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7166391941391941%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{insert: [(0, 2), (1, 1)], delete: [34, 33, 32, 31, 30, 29, 28, 27, 26, 25, 24, '*

 * *                '23, 22, 21, 20, 19, 18, 17, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(6, 5)], delete: [35, 34, 33, 32, 31, 30, 29, 28, 27, 26, 25, 24, 23, '*

 * *                '22, 21, 19, 18, 13, 12, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, 'contextlib'), (3, 'types'), (5, "*

 * *                   "'t […]*

```diff
@@ -1,133 +1,46 @@
 {
-    "data_mtime": 1686754987,
+    "data_mtime": 1686754983,
     "dep_lines": [
-        10,
-        11,
-        12,
-        13,
-        14,
-        15,
-        16,
-        17,
-        18,
-        19,
-        20,
-        21,
-        240,
+        2,
+        1,
         3,
         4,
         5,
         6,
-        7,
-        9,
-        10,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
         5,
-        5,
-        5,
-        5,
-        5,
-        20,
-        10,
         10,
         5,
         5,
         5,
-        10,
-        20,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
+        5,
         30,
         30
     ],
     "dependencies": [
-        "rich.box",
-        "rich.align",
-        "rich.columns",
-        "rich.console",
-        "rich.emoji",
-        "rich.highlighter",
-        "rich.markdown",
-        "rich.padding",
-        "rich.panel",
-        "rich.table",
-        "rich.text",
-        "rich.theme",
-        "typer.core",
-        "inspect",
+        "collections.abc",
         "sys",
-        "collections",
-        "os",
+        "contextlib",
+        "types",
         "typing",
-        "click",
-        "rich",
+        "typing_extensions",
         "builtins",
-        "_collections_abc",
-        "_random",
         "_typeshed",
-        "abc",
-        "array",
-        "click.core",
-        "click.exceptions",
-        "click.shell_completion",
-        "click.types",
-        "ctypes",
-        "datetime",
-        "mmap",
-        "pickle",
-        "rich.jupyter",
-        "rich.style",
-        "types",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "73518e6d145375bea4e7298a3c057f534091fd529c975c4f775c2376751839c7",
-    "id": "typer.rich_utils",
+    "hash": "98625f75a980e4a99a6f836a6ed17e1f95c3729047bca86c6c48dfe60f8702a5",
+    "id": "unittest.mock",
     "ignore_all": true,
-    "interface_hash": "5d907b3cb6c8118bae55ac813280c883d3f38ee428ffaf2ac0527a58e189466e",
+    "interface_hash": "04f1a98f621dd3b651ca7b0998077573046a4805b7a93a4e825f6fc29fa3f0f3",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -162,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/rich_utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi",
     "plugin_data": null,
-    "size": 23654,
+    "size": 14406,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/utils.data.json` & `su6-1.4.1/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/typer/utils.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7337301587301588%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(3, 3), (4, 4)], delete: [9, 8, 7, 6, 5, 4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 20)], delete: [11, 10, 9, 8, 7, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.result'), (1, 'collections.abc'), (2, 'unittest')], "*

 * *                   'delete: [12, 11, 10, 9, 8, 3, 2, 1, 0]}',*

 * * "'hash'": "'eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c'",*

 * * "'id'": "'unittest.signals'",*

 * * "'interface_hash'": "'92394d833593a182a1c8b1a7f4bbde75b4 […]*

```diff
@@ -1,58 +1,40 @@
 {
-    "data_mtime": 1686754987,
+    "data_mtime": 1686754984,
     "dep_lines": [
-        7,
-        8,
         1,
         2,
-        3,
-        5,
-        1,
-        1,
-        1,
-        1,
         1,
+        3,
+        4,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        5,
         10,
         5,
+        20,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "typer._typing",
-        "typer.models",
-        "inspect",
-        "copy",
+        "unittest.result",
+        "collections.abc",
+        "unittest",
         "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "click",
-        "click.core",
-        "click.shell_completion",
-        "click.types",
-        "types"
+        "abc"
     ],
-    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
-    "id": "typer.utils",
+    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
+    "id": "unittest.signals",
     "ignore_all": true,
-    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
+    "interface_hash": "92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
     "plugin_data": null,
-    "size": 7293,
+    "size": 488,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/_log.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/_log.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7014814814814815%*

 * *Differences: {"'data_mtime'": '1687189420',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 10)], delete: [5, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(2, 10)], delete: [6, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'configuraptor.loaders._types'), (1, "*

 * *                   "'configuraptor.loaders.loaders_shared')], delete: [6, 3, 2, 1, 0]}",*

 * * "'hash'": "'0977b2cf0d5250cf8926537041ee006a03f8fe0426fe84e9912545eaa715f5bb'",*

 * * "'id'": "'configuraptor.loaders'",*

 * * "'interface_hash'": "'5c62f36bbd2406123476052c520743abf7c84014d23b5c […]*

```diff
@@ -1,44 +1,35 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1687189420,
     "dep_lines": [
+        7,
+        10,
         5,
         1,
-        2,
-        3,
-        4,
-        1,
-        1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        10,
-        5,
         5,
+        10,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "unittest.case",
-        "logging",
-        "sys",
-        "types",
+        "configuraptor.loaders._types",
+        "configuraptor.loaders.loaders_shared",
         "typing",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "297a51a36613ffcd84bcef772c3f0dd0fdb57a1a9acc544a72840468647d968c",
-    "id": "unittest._log",
+    "hash": "0977b2cf0d5250cf8926537041ee006a03f8fe0426fe84e9912545eaa715f5bb",
+    "id": "configuraptor.loaders",
     "ignore_all": true,
-    "interface_hash": "20b576be7b25765af8108589e0827b19be51be5c76414d2ce9027946fcb1ee5c",
-    "mtime": 1686754198,
+    "interface_hash": "5c62f36bbd2406123476052c520743abf7c84014d23b5c050b826c079189aba7",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/loaders/__init__.py",
     "plugin_data": null,
-    "size": 892,
+    "size": 807,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/async_case.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/async_case.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/case.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/case.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/loader.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/loader.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/main.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/main.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7878787878787878%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 1), (3, 2)], delete: [7, 6, 4, 1]}',*

 * * "'dep_prios'": '{insert: [(6, 30)], delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(3, '_typeshed'), (7, 'types')], delete: [6, 3, 2, 1]}",*

 * * "'hash'": "'c3c84d157ab204cd3b00b3faf4d64cc85ad50fd622145a8032cde2378d31e767'",*

 * * "'id'": "'unittest.result'",*

 * * "'interface_hash'": "'ddb133025512d83572a1a9804a973651824acc3f80a2f1481d0bc2e6bab61de9'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/s […]*

```diff
@@ -1,49 +1,43 @@
 {
     "data_mtime": 1686754984,
     "dep_lines": [
         1,
-        2,
         3,
+        1,
+        2,
         4,
-        5,
         1,
-        6,
-        7,
         1,
         1
     ],
     "dep_prios": [
         10,
-        10,
-        10,
-        10,
         5,
         20,
         5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
         "unittest.case",
-        "unittest.loader",
-        "unittest.result",
-        "unittest.suite",
         "collections.abc",
         "unittest",
-        "types",
+        "_typeshed",
         "typing",
         "builtins",
-        "abc"
+        "abc",
+        "types"
     ],
-    "hash": "f150ef9438e591e3d629f0eefd7b3236c18528d8e0a103ed15774b156b554302",
-    "id": "unittest.main",
+    "hash": "c3c84d157ab204cd3b00b3faf4d64cc85ad50fd622145a8032cde2378d31e767",
+    "id": "unittest.result",
     "ignore_all": true,
-    "interface_hash": "4559180cb5aeda49873e488baf300d3d50e45f5d79850f3e785c1dee6a916d7c",
+    "interface_hash": "ddb133025512d83572a1a9804a973651824acc3f80a2f1481d0bc2e6bab61de9",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/main.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/result.pyi",
     "plugin_data": null,
-    "size": 1544,
+    "size": 1721,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/mock.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/mock.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7466200466200467%*

 * *Differences: {"'data_mtime'": '1686754984',*

 * * "'dep_lines'": '{insert: [(1, 2), (3, 1)], delete: [5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (3, 20)], delete: [3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (1, 'unittest.result'), (3, 'unittest'), (7, "*

 * *                   "'typing')], delete: [7, 4, 3, 2, 1]}",*

 * * "'hash'": "'82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e'",*

 * * "'id'": "'unittest.suite'",*

 * * "'interface_hash'": "'986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca4 […]*

```diff
@@ -1,46 +1,43 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1686754984,
     "dep_lines": [
-        2,
         1,
+        2,
         3,
+        1,
         4,
-        5,
-        6,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
+        10,
         10,
         5,
-        5,
-        5,
+        20,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
+        "unittest.case",
+        "unittest.result",
         "collections.abc",
-        "sys",
-        "contextlib",
-        "types",
-        "typing",
+        "unittest",
         "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "98625f75a980e4a99a6f836a6ed17e1f95c3729047bca86c6c48dfe60f8702a5",
-    "id": "unittest.mock",
+    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
+    "id": "unittest.suite",
     "ignore_all": true,
-    "interface_hash": "04f1a98f621dd3b651ca7b0998077573046a4805b7a93a4e825f6fc29fa3f0f3",
+    "interface_hash": "986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
     "plugin_data": null,
-    "size": 14406,
+    "size": 983,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/result.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/result.meta.json` & `su6-1.4.1/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7570370370370371%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{insert: [(0, 2), (4, 7)], delete: [3, 2]}',*

 * * "'dep_prios'": '{insert: [(0, 5)], delete: [2]}',*

 * * "'dependencies'": "{insert: [(1, 'sys'), (3, 'typing_extensions'), (4, 'types'), (6, "*

 * *                   "'_typeshed')], delete: [7, 3, 2, 0]}",*

 * * "'hash'": "'9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1'",*

 * * "'id'": "'urllib.parse'",*

 * * "'interface_hash'": "'02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706'",*

 * * "'path'": "'/home/rob […]*

```diff
@@ -1,43 +1,43 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1686754983,
     "dep_lines": [
+        2,
         1,
         3,
-        1,
-        2,
         4,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
         5,
-        20,
         5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "unittest.case",
         "collections.abc",
-        "unittest",
-        "_typeshed",
+        "sys",
         "typing",
+        "typing_extensions",
+        "types",
         "builtins",
-        "abc",
-        "types"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "c3c84d157ab204cd3b00b3faf4d64cc85ad50fd622145a8032cde2378d31e767",
-    "id": "unittest.result",
+    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
+    "id": "urllib.parse",
     "ignore_all": true,
-    "interface_hash": "ddb133025512d83572a1a9804a973651824acc3f80a2f1481d0bc2e6bab61de9",
+    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
     "mtime": 1686754198,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/result.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
     "plugin_data": null,
-    "size": 1721,
+    "size": 6532,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/runner.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/runner.meta.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/signals.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/signals.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7171652421652422%*

 * *Differences: {"'data_mtime'": '1685433917',*

 * * "'dep_lines'": '{insert: [(3, 1)], delete: [4, 2]}',*

 * * "'dep_prios'": '{insert: [(4, 30)], delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (4, '_typeshed')], delete: [2, 1, 0]}",*

 * * "'hash'": "'cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c'",*

 * * "'id'": "'sre_constants'",*

 * * "'interface_hash'": "'9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8'",*

 * * "'mtime'": '1685293614',*

 * * "'options'": "{'check_untyped_defs': False, 'disallow_any_gener […]*

```diff
@@ -1,81 +1,78 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1685433917,
     "dep_lines": [
         1,
         2,
-        1,
         3,
-        4,
+        1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
-        20,
-        5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "unittest.result",
-        "collections.abc",
-        "unittest",
+        "sys",
         "typing",
         "typing_extensions",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
-    "id": "unittest.signals",
+    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
+    "id": "sre_constants",
     "ignore_all": true,
-    "interface_hash": "92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720",
-    "mtime": 1686754198,
+    "interface_hash": "9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8",
+    "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": true,
+        "check_untyped_defs": false,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": true,
+        "disallow_any_generics": false,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": true,
-        "disallow_subclassing_any": true,
-        "disallow_untyped_calls": true,
-        "disallow_untyped_decorators": true,
-        "disallow_untyped_defs": true,
+        "disallow_incomplete_defs": false,
+        "disallow_subclassing_any": false,
+        "disallow_untyped_calls": false,
+        "disallow_untyped_decorators": false,
+        "disallow_untyped_defs": false,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": true,
-        "implicit_optional": true,
-        "implicit_reexport": false,
+        "ignore_missing_imports": false,
+        "implicit_optional": false,
+        "implicit_reexport": true,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": true,
-        "strict_equality": true,
+        "strict_concatenate": false,
+        "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": true,
+        "warn_return_any": false,
         "warn_unreachable": false,
-        "warn_unused_ignores": true
+        "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
     "plugin_data": null,
-    "size": 488,
+    "size": 3986,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/suite.data.json` & `su6-1.4.1/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/unittest/suite.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7035409035409035%*

 * *Differences: {"'data_mtime'": '1685433917',*

 * * "'dep_lines'": '{insert: [(0, 3), (3, 6), (4, 7), (6, 1)], delete: [4, 2]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (3, 5), (6, 30), (7, 30)], delete: [3, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'sys'), (2, '_typeshed'), (3, 'typing'), (7, 'ctypes'), (8, "*

 * *                   "'mmap'), (9, 'pickle')], delete: [7, 3, 1, 0]}",*

 * * "'hash'": "'857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7'",*

 * * "'id'": "'array'",*

 * * "'interface_hash'": "'e74f43bcf6812ded0e30399199d4635c9b […]*

```diff
@@ -1,84 +1,90 @@
 {
-    "data_mtime": 1686754984,
+    "data_mtime": 1685433917,
     "dep_lines": [
+        3,
         1,
         2,
-        3,
+        6,
+        7,
+        1,
         1,
-        4,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
-        10,
         5,
-        20,
         5,
         5,
+        5,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "unittest.case",
-        "unittest.result",
         "collections.abc",
-        "unittest",
+        "sys",
+        "_typeshed",
+        "typing",
         "typing_extensions",
         "builtins",
         "abc",
-        "typing"
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
-    "id": "unittest.suite",
+    "hash": "857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7",
+    "id": "array",
     "ignore_all": true,
-    "interface_hash": "986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4",
-    "mtime": 1686754198,
+    "interface_hash": "e74f43bcf6812ded0e30399199d4635c9bc9566bf7e4a36c46596db0efe00fdd",
+    "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": true,
+        "check_untyped_defs": false,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": true,
+        "disallow_any_generics": false,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": true,
-        "disallow_subclassing_any": true,
-        "disallow_untyped_calls": true,
-        "disallow_untyped_decorators": true,
-        "disallow_untyped_defs": true,
+        "disallow_incomplete_defs": false,
+        "disallow_subclassing_any": false,
+        "disallow_untyped_calls": false,
+        "disallow_untyped_decorators": false,
+        "disallow_untyped_defs": false,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": true,
-        "implicit_optional": true,
-        "implicit_reexport": false,
+        "ignore_missing_imports": false,
+        "implicit_optional": false,
+        "implicit_reexport": true,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": true,
-        "strict_equality": true,
+        "strict_concatenate": false,
+        "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": true,
+        "warn_return_any": false,
         "warn_unreachable": false,
-        "warn_unused_ignores": true
+        "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/array.pyi",
     "plugin_data": null,
-    "size": 983,
+    "size": 3717,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-1.4.1/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-1.4.1/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7666666666666667%*

 * *Differences: {"'hash'": "'df8c8fbd2d3a9ee99deaf50d939324b606315d7fd3798f6b844c118915bc93e9'",*

 * * "'id'": "'su6.__about__'",*

 * * "'ignore_all'": 'False',*

 * * "'interface_hash'": "'f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9'",*

 * * "'mtime'": '1686831889',*

 * * "'path'": "'src/su6/__about__.py'",*

 * * "'size'": '206'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
-    "id": "urllib",
-    "ignore_all": true,
-    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
-    "mtime": 1686754198,
+    "hash": "df8c8fbd2d3a9ee99deaf50d939324b606315d7fd3798f6b844c118915bc93e9",
+    "id": "su6.__about__",
+    "ignore_all": false,
+    "interface_hash": "f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9",
+    "mtime": 1686831889,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
+    "path": "src/su6/__about__.py",
     "plugin_data": null,
-    "size": 0,
+    "size": 206,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.mypy_cache/3.11/urllib/parse.data.json` & `su6-1.4.1/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6636507936507937%*

 * *Differences: {"'data_mtime'": '1687189420',*

 * * "'dep_lines'": '{insert: [(0, 11), (1, 12), (2, 5), (3, 6), (4, 8), (6, 1), (10, 9)], delete: [4, '*

 * *                '3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (3, 10), (4, 10), (6, 30), (7, 30), (10, 10)], delete: [2, 1, '*

 * *                '0]}',*

 * * "'dependencies'": "{insert: [(0, 'configuraptor.core'), (1, 'configuraptor.helpers'), (2, "*

 * *                   "'json'), (4, 'tomlkit'), (6, '_collections_abc'), (9, 'json.encoder')], "*

 * *                   'delete: [4, 3, 1, 0]} […]*

```diff
@@ -1,44 +1,52 @@
 {
-    "data_mtime": 1686754983,
+    "data_mtime": 1687189420,
     "dep_lines": [
-        2,
+        11,
+        12,
+        5,
+        6,
+        8,
+        1,
         1,
-        3,
-        4,
-        7,
         1,
         1,
-        1
+        1,
+        9
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
         5,
+        10,
+        10,
+        10,
         5,
         30,
-        30
+        30,
+        30,
+        30,
+        10
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
+        "configuraptor.core",
+        "configuraptor.helpers",
+        "json",
         "typing",
-        "typing_extensions",
-        "types",
+        "tomlkit",
         "builtins",
+        "_collections_abc",
         "_typeshed",
-        "abc"
+        "abc",
+        "json.encoder"
     ],
-    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
-    "id": "urllib.parse",
+    "hash": "336e281941900208951b4b6ddda38d1f5e2f67c7d46d87405aabf74f4aeb3f7c",
+    "id": "configuraptor.dump",
     "ignore_all": true,
-    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
-    "mtime": 1686754198,
+    "interface_hash": "122d447afbaf4cba96d70ee39597f91ce916c2617431969974b3a6ed0984dfb8",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +80,15 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/dump.py",
     "plugin_data": null,
-    "size": 6532,
-    "suppressed": [],
+    "size": 1759,
+    "suppressed": [
+        "yaml"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/.pytest_cache/v/cache/nodeids` & `su6-1.4.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/122419b0bc04bb24` & `su6-1.4.1/.ruff_cache/content/122419b0bc04bb24`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/1a4449eb8b26a401` & `su6-1.4.1/.ruff_cache/content/1a4449eb8b26a401`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/1b7872d6314f48b7` & `su6-1.4.1/.ruff_cache/content/1b7872d6314f48b7`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-1.4.1/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/294d5a468695eb7e` & `su6-1.4.1/.ruff_cache/content/294d5a468695eb7e`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/2bf27b960bc3ded1` & `su6-1.4.1/.ruff_cache/content/2bf27b960bc3ded1`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/2face4e073dced28` & `su6-1.4.1/.ruff_cache/content/2face4e073dced28`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/30e241b2876dc71f` & `su6-1.4.1/.ruff_cache/content/30e241b2876dc71f`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/33004598889f4950` & `su6-1.4.1/.ruff_cache/content/33004598889f4950`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/36f0bdaeef592d9` & `su6-1.4.1/.ruff_cache/content/36f0bdaeef592d9`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/3c7fb493febe6a55` & `su6-1.4.1/.ruff_cache/content/3c7fb493febe6a55`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/3ccdd2336c8c80e9` & `su6-1.4.1/.ruff_cache/content/3ccdd2336c8c80e9`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/3db675ebeb97b2fe` & `su6-1.4.1/.ruff_cache/content/3db675ebeb97b2fe`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/3f10d9d7687f3999` & `su6-1.4.1/.ruff_cache/content/3f10d9d7687f3999`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/42f337caed884834` & `su6-1.4.1/.ruff_cache/content/42f337caed884834`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/51de14ac05bcd5d1` & `su6-1.4.1/.ruff_cache/content/51de14ac05bcd5d1`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/534b8acecf74c47` & `su6-1.4.1/.ruff_cache/content/534b8acecf74c47`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/536320baecd03af6` & `su6-1.4.1/.ruff_cache/content/536320baecd03af6`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/5436d767d06cf116` & `su6-1.4.1/.ruff_cache/content/5436d767d06cf116`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/5cc5d54a963753bf` & `su6-1.4.1/.ruff_cache/content/5cc5d54a963753bf`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/684d0841c18787fb` & `su6-1.4.1/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/68c4553df91c1f5e` & `su6-1.4.1/.ruff_cache/content/68c4553df91c1f5e`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/72a6612daca66426` & `su6-1.4.1/.ruff_cache/content/72a6612daca66426`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/81e6f787866d0ecf` & `su6-1.4.1/.ruff_cache/content/81e6f787866d0ecf`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/84e2e26fc69ab274` & `su6-1.4.1/.ruff_cache/content/84e2e26fc69ab274`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/881c84062ed51136` & `su6-1.4.1/.ruff_cache/content/881c84062ed51136`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/8a5ec4ca9660671c` & `su6-1.4.1/.ruff_cache/content/8a5ec4ca9660671c`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/9019e33ca68d8935` & `su6-1.4.1/.ruff_cache/content/9019e33ca68d8935`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/95df46a8e947b100` & `su6-1.4.1/.ruff_cache/content/95df46a8e947b100`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/9613cbbc5a7c60a4` & `su6-1.4.1/.ruff_cache/content/9613cbbc5a7c60a4`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/abe0d13d37518e58` & `su6-1.4.1/.ruff_cache/content/abe0d13d37518e58`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/ac8c237c67408442` & `su6-1.4.1/.ruff_cache/content/ac8c237c67408442`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/b8ab8c7df580ad75` & `su6-1.4.1/.ruff_cache/content/b8ab8c7df580ad75`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/b8d965aa2b8fd993` & `su6-1.4.1/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/b990e7d90d89db2a` & `su6-1.4.1/.ruff_cache/content/b990e7d90d89db2a`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/bde6d6e902485336` & `su6-1.4.1/.ruff_cache/content/bde6d6e902485336`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/be4a1815dbb4c4` & `su6-1.4.1/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/be5eb6e8ff99feab` & `su6-1.4.1/.ruff_cache/content/be5eb6e8ff99feab`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/ca3d1e0ddece82f5` & `su6-1.4.1/.ruff_cache/content/ca3d1e0ddece82f5`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/cb326dd0ee5910c6` & `su6-1.4.1/.ruff_cache/content/cb326dd0ee5910c6`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/d954f2ee22d56fd0` & `su6-1.4.1/.ruff_cache/content/d954f2ee22d56fd0`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/da0cf7e13e17e6a6` & `su6-1.4.1/.ruff_cache/content/da0cf7e13e17e6a6`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/db73ef232740be87` & `su6-1.4.1/.ruff_cache/content/db73ef232740be87`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/dc4a4b4b55cceada` & `su6-1.4.1/.ruff_cache/content/dc4a4b4b55cceada`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/e067c98663409f12` & `su6-1.4.1/.ruff_cache/content/e067c98663409f12`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/e24118b3523194dc` & `su6-1.4.1/.ruff_cache/content/e24118b3523194dc`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/ed03e948b89996b8` & `su6-1.4.1/.ruff_cache/content/ed03e948b89996b8`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/ed645de094b6d7bb` & `su6-1.4.1/.ruff_cache/content/ed645de094b6d7bb`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/f5d61064e60c404b` & `su6-1.4.1/.ruff_cache/content/f5d61064e60c404b`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/.ruff_cache/content/fd17e608110a0864` & `su6-1.4.1/.ruff_cache/content/fd17e608110a0864`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/docs/plugins.md` & `su6-1.4.1/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/coverage_html.js` & `su6-1.4.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_2602a302b50854cf___about___py.html` & `su6-1.4.1/htmlcov/d_2602a302b50854cf___about___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_2602a302b50854cf___init___py.html` & `su6-1.4.1/htmlcov/d_2602a302b50854cf___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_2602a302b50854cf_cli_py.html` & `su6-1.4.1/htmlcov/d_2602a302b50854cf_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_2602a302b50854cf_core_py.html` & `su6-1.4.1/htmlcov/d_2602a302b50854cf_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_2602a302b50854cf_plugins_py.html` & `su6-1.4.1/htmlcov/d_2602a302b50854cf_plugins_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_a44f0ac069e85531___init___py.html` & `su6-1.4.1/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_a44f0ac069e85531__shared_py.html` & `su6-1.4.1/htmlcov/d_a44f0ac069e85531__shared_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_a44f0ac069e85531_test_about_py.html` & `su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_about_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html` & `su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/d_a44f0ac069e85531_test_core_py.html` & `su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/favicon_32.png` & `su6-1.4.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/index.html` & `su6-1.4.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/keybd_closed.png` & `su6-1.4.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/keybd_open.png` & `su6-1.4.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/status.json` & `su6-1.4.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/htmlcov/style.css` & `su6-1.4.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/except_pytest.toml` & `su6-1.4.1/pytest_examples/except_pytest.toml`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ast.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/abc.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/abc.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/array.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/array.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7945054945054946%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (3, 3), (4, 4), (7, 10)], delete: [5, 0]}',*

 * * "'dep_prios'": '{insert: [(6, 5), (7, 5), (8, 5)], delete: [6]}',*

 * * "'dependencies'": "{insert: [(2, '_ctypes'), (4, 'abc'), (7, 'types'), (9, 'array')], delete: [7, "*

 * *                   '6]}',*

 * * "'hash'": "'4e07f95e28e46e9d4c5eda8e3a693994b25ddc9e70955e59f569acc5472d3284'",*

 * * "'id'": "'ctypes'",*

 * * "'interface_hash'": "'258d6db8de019fc835a41737c0c96359c2e8e1c006da708ce31c5b3846725a76'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checke […]*

```diff
@@ -1,49 +1,55 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        3,
+        5,
         1,
         2,
+        3,
+        4,
         6,
         7,
-        1,
+        10,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
-        30,
+        5,
+        5,
+        5,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
+        "_ctypes",
         "_typeshed",
+        "abc",
         "typing",
         "typing_extensions",
+        "types",
         "builtins",
-        "abc",
-        "ctypes",
+        "array",
         "mmap",
         "pickle"
     ],
-    "hash": "857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7",
-    "id": "array",
+    "hash": "4e07f95e28e46e9d4c5eda8e3a693994b25ddc9e70955e59f569acc5472d3284",
+    "id": "ctypes",
     "ignore_all": true,
-    "interface_hash": "e74f43bcf6812ded0e30399199d4635c9bc9566bf7e4a36c46596db0efe00fdd",
+    "interface_hash": "258d6db8de019fc835a41737c0c96359c2e8e1c006da708ce31c5b3846725a76",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +84,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/array.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi",
     "plugin_data": null,
-    "size": 3717,
+    "size": 11646,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/bad.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/bad.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/builtins.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/codecs.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/enum.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/enum.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/good.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/good.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/io.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/io.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/mmap.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/pickle.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/re.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/re.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7926587301587301%*

 * *Differences: {"'dep_lines'": '{delete: [3]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [4, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'email.message')], delete: [4, 2, 0]}",*

 * * "'hash'": "'53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf'",*

 * * "'id'": "'email.contentmanager'",*

 * * "'interface_hash'": "'86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmana […]*

```diff
@@ -1,37 +1,34 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
         1,
         2,
         3,
         1,
-        1,
         1
     ],
     "dep_prios": [
-        10,
         5,
         5,
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
-        "sys",
+        "collections.abc",
+        "email.message",
         "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
-    "id": "sre_constants",
+    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
+    "id": "email.contentmanager",
     "ignore_all": true,
-    "interface_hash": "9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8",
+    "interface_hash": "86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
     "plugin_data": null,
-    "size": 3986,
+    "size": 480,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sys.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/sys.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/this.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/this.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/types.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/types.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.777051282051282%*

 * *Differences: {"'dep_lines'": '{insert: [(4, 5)], delete: [9, 8, 7, 6, 5, 0]}',*

 * * "'dep_prios'": '{delete: [10, 9, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'email.message'), (2, 'email.policy'), (6, 'abc')], delete: [11, "*

 * *                   '10, 9, 7, 4, 3, 2, 1]}',*

 * * "'hash'": "'6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b'",*

 * * "'id'": "'email'",*

 * * "'interface_hash'": "'2e646e239ef025bcfe7280473c83a79ac7db26c13d93528e2a15010efdbfac7d'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/pytho […]*

```diff
@@ -1,55 +1,40 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        5,
         1,
         2,
         3,
         4,
-        6,
-        7,
-        10,
-        1,
-        1,
+        5,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
         5,
         5,
         5,
         5,
         5,
-        30,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "_ctypes",
-        "_typeshed",
-        "abc",
+        "email.message",
+        "email.policy",
         "typing",
         "typing_extensions",
-        "types",
         "builtins",
-        "array",
-        "mmap",
-        "pickle"
+        "abc"
     ],
-    "hash": "4e07f95e28e46e9d4c5eda8e3a693994b25ddc9e70955e59f569acc5472d3284",
-    "id": "ctypes",
+    "hash": "6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b",
+    "id": "email",
     "ignore_all": true,
-    "interface_hash": "258d6db8de019fc835a41737c0c96359c2e8e1c006da708ce31c5b3846725a76",
+    "interface_hash": "2e646e239ef025bcfe7280473c83a79ac7db26c13d93528e2a15010efdbfac7d",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -84,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
     "plugin_data": null,
-    "size": 11646,
+    "size": 1054,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7904761904761906%*

 * *Differences: {"'dep_lines'": '{delete: [4, 3, 2]}',*

 * * "'dep_prios'": '{delete: [2, 1, 0]}',*

 * * "'dependencies'": '{delete: [4, 2, 1]}',*

 * * "'hash'": "'2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4'",*

 * * "'id'": "'importlib.metadata._meta'",*

 * * "'interface_hash'": "'c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi'",*

 * * "'size'": '842'}*

```diff
@@ -1,40 +1,31 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
         1,
         2,
-        3,
-        4,
-        5,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
-        5,
-        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "email.message",
-        "email.policy",
         "typing",
-        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b",
-    "id": "email",
+    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
+    "id": "importlib.metadata._meta",
     "ignore_all": true,
-    "interface_hash": "2e646e239ef025bcfe7280473c83a79ac7db26c13d93528e2a15010efdbfac7d",
+    "interface_hash": "c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
     "plugin_data": null,
-    "size": 1054,
+    "size": 842,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8222222222222222%*

 * *Differences: {"'dependencies'": "{insert: [(1, 'email.charset')], delete: [1]}",*

 * * "'hash'": "'d98ef62919eee52c902ba572fe572fc3a54622a5e630532cf09aa7f12374562d'",*

 * * "'id'": "'email.header'",*

 * * "'interface_hash'": "'01187afc6a997ff0cfa6678d65f39b1f905eaae0cb55b51ac4ef0e366430347f'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi'",*

 * * "'size'": '1264'}*

```diff
@@ -12,23 +12,23 @@
         5,
         5,
         5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "email.message",
+        "email.charset",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
-    "id": "email.contentmanager",
+    "hash": "d98ef62919eee52c902ba572fe572fc3a54622a5e630532cf09aa7f12374562d",
+    "id": "email.header",
     "ignore_all": true,
-    "interface_hash": "86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad",
+    "interface_hash": "01187afc6a997ff0cfa6678d65f39b1f905eaae0cb55b51ac4ef0e366430347f",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi",
     "plugin_data": null,
-    "size": 480,
+    "size": 1264,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/header.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7787878787878788%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 4), (3, 5), (4, 6), (5, 2), (6, 7), (7, 8)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (4, 5)]}',*

 * * "'dependencies'": "{insert: [(2, 'email.contentmanager'), (3, 'email.errors'), (4, "*

 * *                   "'email.policy'), (5, 'email'), (7, 'typing_extensions')]}",*

 * * "'hash'": "'762e166d09e139961a402ba13a8aaabb0c5cbd010af7cd6f562150d86b3d6f4f'",*

 * * "'id'": "'email.message'",*

 * * "'interface_hash'": "'78d151688bd9228724fca1fac597a42d13de1d6e484913be9ff81 […]*

```diff
@@ -1,34 +1,49 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
         1,
-        2,
         3,
+        4,
+        5,
+        6,
+        2,
+        7,
+        8,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
+        5,
+        5,
+        5,
+        5,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
         "email.charset",
+        "email.contentmanager",
+        "email.errors",
+        "email.policy",
+        "email",
         "typing",
+        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "d98ef62919eee52c902ba572fe572fc3a54622a5e630532cf09aa7f12374562d",
-    "id": "email.header",
+    "hash": "762e166d09e139961a402ba13a8aaabb0c5cbd010af7cd6f562150d86b3d6f4f",
+    "id": "email.message",
     "ignore_all": true,
-    "interface_hash": "01187afc6a997ff0cfa6678d65f39b1f905eaae0cb55b51ac4ef0e366430347f",
+    "interface_hash": "78d151688bd9228724fca1fac597a42d13de1d6e484913be9ff81afbaf712e75",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +78,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/message.pyi",
     "plugin_data": null,
-    "size": 1264,
+    "size": 6116,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/message.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7894871794871795%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 2), (6, 7)], delete: [7, 6, 5, 0]}',*

 * * "'dep_prios'": '{delete: [9, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'email.header'), (4, 'email.message'), (5, 'abc')], delete: [9, "*

 * *                   '7, 5, 4, 1]}',*

 * * "'hash'": "'2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4'",*

 * * "'id'": "'email.policy'",*

 * * "'interface_hash'": "'6dcefb20f7ebc6d81fba80753edb4f9695c0e5e1f9e4195cfb5fbc1b9e26f5ef'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-p […]*

```diff
@@ -1,49 +1,43 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        1,
+        2,
         3,
         4,
         5,
         6,
-        2,
-        7,
-        8,
         1,
+        7,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
         5,
         5,
-        5,
-        5,
-        30
+        5
     ],
     "dependencies": [
         "collections.abc",
-        "email.charset",
         "email.contentmanager",
         "email.errors",
-        "email.policy",
-        "email",
+        "email.header",
+        "email.message",
+        "abc",
         "typing",
-        "typing_extensions",
-        "builtins",
-        "abc"
+        "builtins"
     ],
-    "hash": "762e166d09e139961a402ba13a8aaabb0c5cbd010af7cd6f562150d86b3d6f4f",
-    "id": "email.message",
+    "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
+    "id": "email.policy",
     "ignore_all": true,
-    "interface_hash": "78d151688bd9228724fca1fac597a42d13de1d6e484913be9ff81afbaf712e75",
+    "interface_hash": "6dcefb20f7ebc6d81fba80753edb4f9695c0e5e1f9e4195cfb5fbc1b9e26f5ef",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/message.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/policy.pyi",
     "plugin_data": null,
-    "size": 6116,
+    "size": 3055,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.769090909090909%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (4, 1)], delete: [6, 4, 3, 2]}',*

 * * "'dep_prios'": '{insert: [(4, 30), (5, 30)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'importlib.abc'), (2, 'types'), (3, 'builtins')], delete: [7, 4, "*

 * *                   '3, 2, 1]}',*

 * * "'hash'": "'93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914'",*

 * * "'id'": "'importlib'",*

 * * "'interface_hash'": "'5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-check […]*

```diff
@@ -1,43 +1,37 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
+        1,
         2,
         3,
-        4,
-        5,
-        6,
         1,
-        7,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
-        5,
-        5,
-        5,
-        5
+        30,
+        30
     ],
     "dependencies": [
         "collections.abc",
-        "email.contentmanager",
-        "email.errors",
-        "email.header",
-        "email.message",
+        "importlib.abc",
+        "types",
+        "builtins",
         "abc",
-        "typing",
-        "builtins"
+        "typing"
     ],
-    "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
-    "id": "email.policy",
+    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
+    "id": "importlib",
     "ignore_all": true,
-    "interface_hash": "6dcefb20f7ebc6d81fba80753edb4f9695c0e5e1f9e4195cfb5fbc1b9e26f5ef",
+    "interface_hash": "5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/policy.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
     "plugin_data": null,
-    "size": 3055,
+    "size": 801,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.76%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 31), (1, 5), (2, 6), (3, 7), (7, 4), (8, 8), (9, 10), (10, 11), '*

 * *                '(11, 12)], delete: [4, 3]}',*

 * * "'dep_prios'": '{insert: [(4, 10), (5, 5), (6, 10), (7, 5), (8, 5), (9, 5), (10, 5), (11, 5), '*

 * *                '(12, 5)], delete: [5, 4]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib.metadata._meta'), (2, 'email.message'), (5, "*

 * *                   "'pathlib'), (6, 'sys'), (7, '_typeshed'), (8, 'os'), (9, 're'), (11, "*

 * *                   "'typing_extensions'), (12 […]*

```diff
@@ -1,37 +1,58 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
+        31,
+        5,
+        6,
+        7,
         1,
         2,
         3,
-        1,
-        1,
+        4,
+        8,
+        10,
+        11,
+        12,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
-        30,
-        30
+        10,
+        5,
+        10,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
+        "importlib.metadata._meta",
         "collections.abc",
+        "email.message",
         "importlib.abc",
-        "types",
-        "builtins",
         "abc",
-        "typing"
+        "pathlib",
+        "sys",
+        "_typeshed",
+        "os",
+        "re",
+        "typing",
+        "typing_extensions",
+        "builtins"
     ],
-    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
-    "id": "importlib",
+    "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
+    "id": "importlib.metadata",
     "ignore_all": true,
-    "interface_hash": "5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3",
+    "interface_hash": "21a4b9857190f7893fd1d564e25c567d7f4777614d1a6990ac158bb2835a9eab",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi",
     "plugin_data": null,
-    "size": 801,
+    "size": 6736,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7616677912730545%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 23), (1, 30), (4, 21), (5, 22), (6, 24), (7, 25), (8, 26), (9, 27), '*

 * *                '(10, 28), (11, 33), (12, 1), (13, 1), (14, 1)], delete: [11, 10, 9, 8, 7, 6, 3, '*

 * *                '2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (12, 30), (13, 30), (14, 30), (15, 30)], delete: [6, '*

 * *                '4, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'os.path'), (4, 'abc'), (5, 'builtins'), (6, 'contextlib'), (7, "*

 * *                   "'io'), (8, 'subprocess'), (11, 'types […]*

```diff
@@ -1,58 +1,67 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        31,
-        5,
-        6,
-        7,
+        23,
+        30,
         1,
         2,
-        3,
-        4,
-        8,
-        10,
-        11,
-        12,
+        21,
+        22,
+        24,
+        25,
+        26,
+        27,
+        28,
+        33,
+        1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        10,
         5,
         5,
         5,
-        10,
         5,
-        10,
         5,
         5,
         5,
         5,
         5,
-        5
+        30,
+        30,
+        30,
+        30
     ],
     "dependencies": [
-        "importlib.metadata._meta",
         "collections.abc",
-        "email.message",
-        "importlib.abc",
-        "abc",
-        "pathlib",
+        "os.path",
         "sys",
         "_typeshed",
-        "os",
-        "re",
+        "abc",
+        "builtins",
+        "contextlib",
+        "io",
+        "subprocess",
         "typing",
         "typing_extensions",
-        "builtins"
+        "types",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
-    "id": "importlib.metadata",
+    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
+    "id": "os",
     "ignore_all": true,
-    "interface_hash": "21a4b9857190f7893fd1d564e25c567d7f4777614d1a6990ac158bb2835a9eab",
+    "interface_hash": "7857e0241ab1ae7ccf1c6583d54898fa386079260ac7e105c7e8d281784f77c9",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
     "plugin_data": null,
-    "size": 6736,
+    "size": 36995,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7117948717948719%*

 * *Differences: {"'data_mtime'": '1686754983',*

 * * "'dep_lines'": '{insert: [(1, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (2, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(2, '_typeshed')], delete: [0]}",*

 * * "'hash'": "'9dfc180741340abdc5dbdbb5b060f46a50d436b180e08c25f25211b1c3e31d7f'",*

 * * "'id'": "'configuraptor.loaders._types'",*

 * * "'interface_hash'": "'ff8bf54ace6de15cec9f2eb2c19a18138007d71a654544edb632d48f8f96a653'",*

 * * "'mtime'": '1687189299',*

 * * "'options'": "{'check_untyped_defs': True, 'disallow_any_gen […]*

```diff
@@ -1,72 +1,72 @@
 {
-    "data_mtime": 1685433917,
+    "data_mtime": 1686754983,
     "dep_lines": [
         1,
-        2,
+        1,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
         "typing",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
-    "id": "importlib.metadata._meta",
+    "hash": "9dfc180741340abdc5dbdbb5b060f46a50d436b180e08c25f25211b1c3e31d7f",
+    "id": "configuraptor.loaders._types",
     "ignore_all": true,
-    "interface_hash": "c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd",
-    "mtime": 1685293614,
+    "interface_hash": "ff8bf54ace6de15cec9f2eb2c19a18138007d71a654544edb632d48f8f96a653",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": false,
+        "check_untyped_defs": true,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": false,
+        "disallow_any_generics": true,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": false,
-        "disallow_subclassing_any": false,
-        "disallow_untyped_calls": false,
-        "disallow_untyped_decorators": false,
-        "disallow_untyped_defs": false,
+        "disallow_incomplete_defs": true,
+        "disallow_subclassing_any": true,
+        "disallow_untyped_calls": true,
+        "disallow_untyped_decorators": true,
+        "disallow_untyped_defs": true,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": false,
-        "implicit_optional": false,
-        "implicit_reexport": true,
+        "ignore_missing_imports": true,
+        "implicit_optional": true,
+        "implicit_reexport": false,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": false,
-        "strict_equality": false,
+        "strict_concatenate": true,
+        "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": false,
+        "warn_return_any": true,
         "warn_unreachable": false,
-        "warn_unused_ignores": false
+        "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/loaders/_types.py",
     "plugin_data": null,
-    "size": 842,
+    "size": 304,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7571486928104575%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 7)], delete: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [13, 12, 9, 8, 7, 6, 5, 4, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'posixpath'), (3, 'abc')], delete: [15, 14, 13, 12, 11, 10, 8, "*

 * *                   '7, 6, 4, 3, 1, 0]}',*

 * * "'hash'": "'1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433'",*

 * * "'id'": "'os.path'",*

 * * "'interface_hash'": "'a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e'",*

 * * "'path'": "'/home/robin/we […]*

```diff
@@ -1,67 +1,34 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        23,
-        30,
-        1,
-        2,
-        21,
-        22,
-        24,
-        25,
-        26,
-        27,
-        28,
-        33,
         1,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        10,
         10,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os.path",
         "sys",
-        "_typeshed",
-        "abc",
+        "posixpath",
         "builtins",
-        "contextlib",
-        "io",
-        "subprocess",
-        "typing",
-        "typing_extensions",
-        "types",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "abc",
+        "typing"
     ],
-    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
-    "id": "os",
+    "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
+    "id": "os.path",
     "ignore_all": true,
-    "interface_hash": "7857e0241ab1ae7ccf1c6583d54898fa386079260ac7e105c7e8d281784f77c9",
+    "interface_hash": "a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -96,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
     "plugin_data": null,
-    "size": 36995,
+    "size": 186,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/path.data.json` & `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json` & `su6-1.4.1/.mypy_cache/3.11/configuraptor/core.meta.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6725605935283354%*

 * *Differences: {"'data_mtime'": '1687189420',*

 * * "'dep_lines'": '{insert: [(0, 16), (1, 17), (2, 18), (3, 19), (4, 5), (5, 6), (7, 8), (8, 9), (9, '*

 * *                '10), (10, 11), (11, 13), (12, 16), (13, 1), (14, 1), (15, 1), (16, 1), (17, 1), '*

 * *                '(18, 1), (19, 1), (20, 1), (21, 1), (22, 1), (23, 1), (24, 1), (25, 1), (26, 1)], '*

 * *                'delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5), (3, 5), (4, 10), (5, 10), (6, 10), (7, 10), '*

 * *                '(9, 5), (10, 5), (12, 20), (14, 3 […]*

```diff
@@ -1,75 +1,150 @@
 {
-    "data_mtime": 1685433917,
+    "data_mtime": 1687189420,
     "dep_lines": [
-        1,
+        16,
+        17,
+        18,
+        19,
+        5,
+        6,
         7,
+        8,
+        9,
+        10,
+        11,
+        13,
+        16,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
+        5,
+        10,
+        10,
+        10,
+        10,
+        10,
+        5,
+        5,
+        5,
+        20,
+        5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "sys",
-        "posixpath",
+        "configuraptor.loaders",
+        "configuraptor.errors",
+        "configuraptor.helpers",
+        "configuraptor.postpone",
+        "dataclasses",
+        "math",
+        "types",
+        "typing",
+        "warnings",
+        "collections",
+        "pathlib",
+        "typeguard",
+        "configuraptor",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
         "abc",
-        "typing"
+        "array",
+        "configuraptor.singleton",
+        "ctypes",
+        "enum",
+        "io",
+        "mmap",
+        "os",
+        "pickle",
+        "typeguard._config",
+        "typeguard._exceptions",
+        "typeguard._functions",
+        "typeguard._memo",
+        "typing_extensions"
     ],
-    "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
-    "id": "os.path",
+    "hash": "faa5e5569959e79b2d9ce2ac9ae0efe859389ab8ff83b2abe8b549735de4d293",
+    "id": "configuraptor.core",
     "ignore_all": true,
-    "interface_hash": "a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e",
-    "mtime": 1685293614,
+    "interface_hash": "4fd62b408424d3fb68a78c823a3e4cfe3a239fd24ef732a02eff954311e6f412",
+    "mtime": 1687189299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": false,
+        "check_untyped_defs": true,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": false,
+        "disallow_any_generics": true,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": false,
-        "disallow_subclassing_any": false,
-        "disallow_untyped_calls": false,
-        "disallow_untyped_decorators": false,
-        "disallow_untyped_defs": false,
+        "disallow_incomplete_defs": true,
+        "disallow_subclassing_any": true,
+        "disallow_untyped_calls": true,
+        "disallow_untyped_decorators": true,
+        "disallow_untyped_defs": true,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": false,
-        "implicit_optional": false,
-        "implicit_reexport": true,
+        "ignore_missing_imports": true,
+        "implicit_optional": true,
+        "implicit_reexport": false,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": false,
-        "strict_equality": false,
+        "strict_concatenate": true,
+        "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": false,
+        "warn_return_any": true,
         "warn_unreachable": false,
-        "warn_unused_ignores": false
+        "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/configuraptor/core.py",
     "plugin_data": null,
-    "size": 186,
+    "size": 15538,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-1.4.0/src/su6/__init__.py` & `su6-1.4.1/src/su6/__init__.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/src/su6/cli.py` & `su6-1.4.1/src/su6/cli.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/src/su6/core.py` & `su6-1.4.1/src/su6/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -277,31 +277,14 @@
 class AbstractConfig(configuraptor.TypedConfig, configuraptor.Singleton):
     """
     Used by state.config and plugin configs.
     """
 
     _strict = True
 
-    def update(self, strict: bool = True, allow_none: bool = False, **kw: typing.Any) -> None:
-        """
-        Set the config values.
-
-        Args:
-            strict: by default, setting a new/unannotated property will raise an error. Set strict to False to allow it.
-            allow_none: by default, None values are filtered away. Set to True to allow them.
-        """
-        for key, value in kw.items():
-            if value is None and not allow_none:
-                continue
-
-            if strict and key not in self.__annotations__:
-                raise KeyError(f"{self.__class__.__name__} does not have a property {key} and strict mode is enabled.")
-
-            setattr(self, key, value)
-
 
 @dataclass
 class Config(AbstractConfig):
     """
     Used as typed version of the [tool.su6] part of pyproject.toml.
 
     Also accessible via state.config
```

### Comparing `su6-1.4.0/src/su6/plugins.py` & `su6-1.4.1/src/su6/plugins.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/tests/test_cli.py` & `su6-1.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/tests/test_core.py` & `su6-1.4.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/tests/test_plugins.py` & `su6-1.4.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/tests/test_plugins_config.py` & `su6-1.4.1/tests/test_plugins_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 
 import pytest
 from configuraptor import Singleton
+from configuraptor.errors import ConfigErrorExtraKey
 
 from src.su6 import state
 from src.su6.cli import app
 from src.su6.plugins import PluginConfig, PluginLoader, register
 
 
 class FakeModule1:
@@ -79,15 +80,15 @@
     class MySingletonState(PluginConfig):
         ...
 
     inst1 = MySingletonState()
     inst2 = MySingletonState()
     assert inst1 is inst2
 
-    with pytest.raises(KeyError):
+    with pytest.raises(ConfigErrorExtraKey):
         inst1.update(newkey="illegal")
 
     inst2.update(newkey="legal", strict=False)
     inst2.update(newkey=None, strict=False)
 
     assert inst1.newkey == "legal"  # and NOT None
     inst2.update(newkey=None, strict=False, allow_none=True)
```

### Comparing `su6-1.4.0/LICENSE.txt` & `su6-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/README.md` & `su6-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `su6-1.4.0/pyproject.toml` & `su6-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "typer[all]",
     "plumbum",
     "black", # for 'find_pyproject_toml'
-    "configuraptor >= 1.4", # for config
+    "configuraptor >= 1.6", # for config
 ]
 
 [template.plugins.default]
 src-layout = true
 
 [tool.setuptools.package-data]
 "su6" = ["py.typed"]
```

### Comparing `su6-1.4.0/PKG-INFO` & `su6-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python cli tool to use tools for some common code quality checks (opinionated)
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-checker#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-checker/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-checker
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.11
 Requires-Dist: black
-Requires-Dist: configuraptor>=1.4
+Requires-Dist: configuraptor>=1.6
 Requires-Dist: plumbum
 Requires-Dist: typer[all]
 Provides-Extra: all
 Requires-Dist: bandit; extra == 'all'
 Requires-Dist: black; extra == 'all'
 Requires-Dist: coverage-badge; extra == 'all'
 Requires-Dist: isort; extra == 'all'
```

