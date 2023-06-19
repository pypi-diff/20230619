# Comparing `tmp/su6-1.4.1.tar.gz` & `tmp/su6-1.4.2.tar.gz`

## Comparing `su6-1.4.1.tar` & `su6-1.4.2.tar`

### file list

```diff
@@ -1,1460 +1,1461 @@
--rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 su6-1.4.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-1.4.1/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 su6-1.4.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/concurrency.data.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/concurrency.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.meta.json
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.meta.json
--rw-r--r--   0        0        0    29408 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/core.data.json
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/core.meta.json
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.meta.json
--rw-r--r--   0        0        0    23607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.meta.json
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.meta.json
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.meta.json
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.meta.json
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    31787 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    38285 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    17494 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    27179 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/android.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/android.meta.json
--rw-r--r--   0        0        0    42401 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    82219 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    25162 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    54090 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0    45733 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/plugins.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/su6/plugins.meta.json
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.meta.json
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.meta.json
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.meta.json
--rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/api.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/api.meta.json
--rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/container.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/container.meta.json
--rw-r--r--   0        0        0    33007 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json
--rw-r--r--   0        0        0   221620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/items.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/items.meta.json
--rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.meta.json
--rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/source.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/source.meta.json
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.1/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/README.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/10595a931c3c881e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1065c8b44fadc39a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1086635a5970b925
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/10ab08017438a66a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/10c2ae33c509be23
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/11f25cfda4e2f210
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/122419b0bc04bb24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1322b93a2154c54a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/134e5e8c29726e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/13985ae090677282
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/146952ec4263c5d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/150d086b8b4de9d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/156301591af184f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1663be342a34f83
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1895bed4a0ed65d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1996a22aec44a5c0
--rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1a4449eb8b26a401
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1a4db4c4834af592
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1b0530edc3fe075e
--rw-r--r--   0        0        0    21464 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1b7872d6314f48b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1ce202f3daa889d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1cfd31ba4b0b7ef9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1dcbdc62e66ccf0e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1edace855ae3c841
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1f7ac4f892285f60
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/1fbfdffa4078f509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/20b40aca78f395e8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/219bf1f8f2938bd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/21b248d368a93ac8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/21cf950ddc412c7b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/22db1408b8f4a4b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/232d0222563916a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/23680c0655621b13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/247546336fc4bd59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/248d23bfc4586461
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/24e2ebef92fa75b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/25d9504d2b6847d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/26657ed11f8e66de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/269f98f304a03fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/28caf6cfecd38c1a
--rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/294d5a468695eb7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/29531d612e8a868a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2a383abdede299d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2a5d8d1386804aed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2a630c7d6d7faa40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2b0cdebce71424f0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2bc4a20be77b881b
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2bf27b960bc3ded1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2c189a9882594507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2c6eeab804b5c1f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2c9bbc6bae6b0f41
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2d77da04c7119543
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2e4746b83d2d1cf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2e6b6d5e70ae29db
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2e8708077cd0413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2f9e25dc2ce777cc
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/2face4e073dced28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/300f9a816018d49f
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/30e241b2876dc71f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/31813abf4ed82b53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3271e344462a0ee3
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/33004598889f4950
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/349f044f89b94587
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/34a4aaded634d537
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/34e1109d49bf09f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/356d28a11355e7a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/357e837fe90ee680
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/35ab5ee4981cdf8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/35ba35b3f04c192f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/36372ef94f8716cd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/36e48551be186a66
--rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/36f0bdaeef592d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/380a13ecd1a2af25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/38962215221b245a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/38d9da4e93811c4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/39285e72757cc499
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/399d3b28a1a1db47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3a74e1b5704e9b3f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3af645c926072f97
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3c6b70c96e832bc1
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3c7fb493febe6a55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3c9bb20c3b57bae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3ca706f99b2d38bf
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3ccdd2336c8c80e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3cf13d9d13babf93
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3db675ebeb97b2fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3e0ec316d612ddc6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3e35311bfb3345f8
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3f10d9d7687f3999
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/3f12e7a3fe46c220
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/417040cdeaa7bd81
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/429010e306ea9808
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/42f337caed884834
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/431bdba29473eca0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4536434fd84cdba5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/467fc2e82c277fd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/47affd4e531897a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/47ca38fe0242f05d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/47e54ee652d2f4c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4843e1c724479e6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/484730e7d1a4dcd9
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4880724f1f6a1ac8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/48bda5931a9eb062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/49fafbbbbadedf00
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4a63ed784e7c5ec0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4ac8c08e5b1b6650
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4b5890a0c8dc15df
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4cd4c52ee1dc7ffe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4cdd16a7f9738f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4eaf3b155fae0dfb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f16c6852dea8eca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f2c663677c63589
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/4fafe0dbefb778fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/50373733f4645c5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/514fb27e4aef5783
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/519ab6ce866ef11b
--rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/51de14ac05bcd5d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/529312a72d1177a1
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/534b8acecf74c47
--rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/536320baecd03af6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/538fc0618c4d4c31
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/53c0f85a3179a38f
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5436d767d06cf116
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/54637ff0aaaaf6b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/552fa1eb2057eecc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5548c3ce5fff0cca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/556b5cfaac0c49bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/55c947c0fa59929
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/568d77a0a0a64dbc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/56e83f1c5eeb3eba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/572ba1efb5bb3fd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/58240cde188220d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/584058f21d3e2fa1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/594d55ee247cbdef
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/59cfab1472b544fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5a6dc8ef65620223
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5af13ad9cc04e932
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5b8fb96822a8f127
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5b965ef6adf36c8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5badc1835a2b80e1
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5cc5d54a963753bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5da466fd7e3b19f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5e83ab1d520dc773
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5efe825a5e773b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/5fb3763e0810c38a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/62396a4dea084957
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/624348590d33bdc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6278996c2e6b2a87
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/63dbabe01e9e6756
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6550bbd98b1711bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6791fc0114ddc05
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6845ca4e0c56952b
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/68c4553df91c1f5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/69bb9ea6355c0c25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/69ffc3e7ad0aa6b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6a4adfab73a8d4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6a74d0efd6350f1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6b596d4ac1166741
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6b9f30172d33b6a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6bcca98e41cda3f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6beed9d45ff1a491
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6c989c6e4eea10bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6db20c27780d4a5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6db875fe1541793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6eab8cdd7b4ae170
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/6fc044c94dc3532a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/701212523f7b3b9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/70963c0c68bf76ac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/70bd045859d6cb20
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/70d6f3b95738758d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/729f212cc9c6cd5d
--rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/72a6612daca66426
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/72de7bec9ecb53aa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/733b2373fa4ae335
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7396a954cc3b124a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7485843a948a75b0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/755c9c217a06f932
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/75bb48e114159509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/76d56794deeb084d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/76fbe2af0f71bd4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/79a22043e5c16946
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/79c3fb2c81fd59a0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7a19353a5daa4a37
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7b3a1bf0b652398a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7bf45647f43eaf85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7c01d9689dd16a64
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7c37d34a0c059ec7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7c806e58272a88ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7cbc35f4e814db65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7cc3783d00621498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7dc27d897f910c11
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7e138932f0b9a1bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7eb1422c10ced038
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7eb17a25b4fa1d13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7f0f63895e369318
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/7f75cbd11ebac70a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8012caf4fb290dc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/80844117d21fe12b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/809075c58fb87c61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/80dbccb0d26b4b4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/80ded2016f4f413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/81e3edf198d6c468
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/81e6f787866d0ecf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/82ab0276d38aec9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/83a59cf9aceae1d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/83cdfb5da134b21f
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/84e2e26fc69ab274
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/84e8c31ce428d3ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/858df3976aef9624
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/868699acd08be339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/86c3e5b9f79f490f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/87a7b0840a5cf8c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/87d9b6d5e7bcb6c7
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/881c84062ed51136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/886d14b97dbd4f2e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8944dfd1b590bdd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/89c7a4d643f68517
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/89e58e5ee0d7d864
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8a0279b11d098d9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8a437c05421c6cb5
--rw-r--r--   0        0        0    20054 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8a5ec4ca9660671c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8b8acf1607bcb3f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8c34e85d573e230f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8d2f83aae152de29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8df3988e9368cbe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/8f33397e19bead30
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9019e33ca68d8935
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/902eb6f99ee41131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/906cef8208fbf28f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9080aaa3f2416b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/922bfc03482db456
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/92db151fe9967fd3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9352425265579062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/93fed7ae4120c88e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/945994955724de24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/94ffcc82bc7ee370
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/95df46a8e947b100
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9613cbbc5a7c60a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/968b32ac9319cc53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/97a72bc70808d2f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/97cbf45b388709d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/97df9d79e599f082
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/981eb70eb69fb3ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/98392e87ef3eb254
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/99d5decc6ca01825
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9a5552199a8b8bd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9bd08ae684645cf6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9c1285d5b3178abe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9cbaa57406e65f63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9d0f65e1ab7ca23
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9db15fb6e71bec4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9dda9185d48774f2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e3b1a7c0f34103b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e50a4d6fb3c9688
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e558f66f216c4eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9e915e4e576201bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9ec2a872083329d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9edacb4de19eeb8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9f0f8b1c56898117
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9f2c57bc030e0b04
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/9f330edc61f02d3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a0572377dc282cac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a113f7e28da04408
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a24edf91b0bcff12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a2fe93c3bba310b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a38eff4f06853e65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a78089cbf54aff62
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a8da9d8efa986532
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a925b8cd7505ac0a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a92bb1bdda49ef61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/a943564382aec90a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/aa3f7accc1718239
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ab360402eb2d795e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ab4a97b5d68b837a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/abc8db1325696a17
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/abe0d13d37518e58
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ac5b9f591ce9edec
--rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ac8c237c67408442
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/acbc9f45cfeee4dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/acecedeb9f4dd91a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ad02b8e4575abc6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ae5a30e888e80958
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/aff288abf6945582
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b08de429bee9ce93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b2d26e3968f3c218
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b2f061a9d80cfa8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b4228843afe3d2eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b56a01688e02e5f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b5c4e8c097cbf198
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b5f69f56d932f0d1
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b6191d72e3d9a646
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b61cd4b71d14e881
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b7331c702909633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b7b1c8254943be90
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b7bcb1e4c5eea72b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b81f55dc9d767e8f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b82ae772ad3347b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b89a404ae8aaa495
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b89dc34e1d21508f
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b8ab8c7df580ad75
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/b990e7d90d89db2a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ba0f74a0540d9a5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ba66feb1819b5312
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bbd87fc7f90c1f28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bd12e3fd28591ae6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bd1e909ba96cca61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bdd37795dc331d56
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bde6d6e902485336
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/bdeb811362915192
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/be5eb6e8ff99feab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/be9c428a6192e049
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/beb37e84505d7dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c0d14d0162a80714
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c10a38d72f60e675
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c121acc012633d2f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c18d3e52506df649
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c250dc207334d18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c25779f3e34a584a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c293dd30723003b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c3329258d804dff6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c40a4c8f88b65414
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c55a79e89225a078
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c62dd73faf917878
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c766d7d105d53e92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c82d4fd611732d02
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c88465e3c1dc503e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c8c7b8092b03fdd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/c9d297807d108576
--rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ca3d1e0ddece82f5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cb0e3b769b6a1727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cb2f84958966b77c
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cb326dd0ee5910c6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cbb8b9fccd8c8746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cc518cf199497e9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ccc4c37cd56e46e5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ccf15ba8d3af2d15
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cd61466cc4a76933
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ce0a51ca403a72f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ce7ae4869b72ad31
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cee8b7a480495342
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/cfa33b7a8aeb793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d085b6ebe7bb0389
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d0be3a4705e047c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d0fd170547b6bb47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d1c81941e3ef2e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d1d63b74d8d929b9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d203b8acf8460019
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d2cceb9cc8265e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d3a20b1509715554
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d551c518ebaaf23a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d5a9ce7dc11e5edc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d6b8c7cba735b946
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d825cf3987ee9f33
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d8444fda03b67f2b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d86a45eca9289fa5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d9198ab6e1ae45a0
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d954f2ee22d56fd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d9b321d36a255169
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/d9cd4c2a9ad4580d
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/da0cf7e13e17e6a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/da4aff17737df0c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/da94ab81ae4dffd1
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/db73ef232740be87
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dc4a4b4b55cceada
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dcb2ce27d1f7cc70
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/de1238012a6853f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dec4fb820d1aee1f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/decdb847958ce882
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/dfc2e498a5736fb3
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e067c98663409f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e07d7deee3f2b1ed
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e24118b3523194dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e316b4f368a31a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e4a016e6cc51d759
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e59ac15827b7f1c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e6237a2dffed4f5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e6e7d13cd57b4fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e832a8f80eaf16d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e8ab3d919ff04fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e8cd5143f259cdce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/e98cf82519b9efc2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ea450af950172f80
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ebd9c23038b8db35
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ec04e1ad73846b2a
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ed03e948b89996b8
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ed645de094b6d7bb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/edbe26c4bd7599ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/ee965a83d6cd2aaa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f002d9727bf66a12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f1af1d1ebb07ad61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f2942d8cb87b15e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f4088198fa879c9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f41987c18d73e01d
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f4d6392808939633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f4e7c96257c9d24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f586c8a0f5c58b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f58e778cbde5b210
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f5d61064e60c404b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/f9ab84e0c6669bed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fa23c022574446ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fa2e112681e24616
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fa354595b122bf9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/faa3132a8644ec4d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fad49b925cd80258
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fb9901f753a46f52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fbd81c0d9b22b507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fd089a45384d0959
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 su6-1.4.1/.ruff_cache/content/fd17e608110a0864
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 su6-1.4.1/docs/plugins.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf___about___py.html
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf___init___py.html
--rw-r--r--   0        0        0   120042 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf_cli_py.html
--rw-r--r--   0        0        0   161698 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf_core_py.html
--rw-r--r--   0        0        0    92303 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_2602a302b50854cf_plugins_py.html
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531__shared_py.html
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_about_py.html
--rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_cli_py.html
--rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_core_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-1.4.1/htmlcov/style.css
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/bad.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/black_good_mypy_bad.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/empty.toml
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/except_pytest.toml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/fake_module.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/good.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/invalid.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/only_black.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/only_mypy.toml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/stop_after_first.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.meta.json
--rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/__about__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/__init__.py
--rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/cli.py
--rw-r--r--   0        0        0    17551 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/core.py
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 su6-1.4.1/src/su6/py.typed
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-1.4.1/tests/_shared.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_about.py
--rw-r--r--   0        0        0     9632 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_cli.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_core.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_plugins.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 su6-1.4.1/tests/test_plugins_config.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-1.4.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 su6-1.4.1/README.md
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 su6-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 su6-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 su6-1.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-1.4.2/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 su6-1.4.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/concurrency.data.json
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/concurrency.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/__init__.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/__init__.meta.json
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/cls.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/cls.meta.json
+-rw-r--r--   0        0        0    29408 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/core.data.json
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/core.meta.json
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/dump.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/dump.meta.json
+-rw-r--r--   0        0        0    23607 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/errors.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/errors.meta.json
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/helpers.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/helpers.meta.json
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/postpone.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/postpone.meta.json
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/singleton.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/singleton.meta.json
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    31787 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    38285 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    17494 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    27179 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    42401 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/unix.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/unix.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    82219 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    25162 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    54090 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0    45733 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/plugins.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/su6/plugins.meta.json
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/__init__.meta.json
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/_compat.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/_compat.meta.json
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/_utils.meta.json
+-rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/api.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/api.meta.json
+-rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/container.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/container.meta.json
+-rw-r--r--   0        0        0    33007 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/exceptions.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/exceptions.meta.json
+-rw-r--r--   0        0        0   221620 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/items.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/items.meta.json
+-rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/parser.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/parser.meta.json
+-rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/source.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/source.meta.json
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_char.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_char.meta.json
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_document.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_document.meta.json
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-1.4.2/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-1.4.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-1.4.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-1.4.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 su6-1.4.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 su6-1.4.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/10595a931c3c881e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1065c8b44fadc39a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1086635a5970b925
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/10ab08017438a66a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/10c2ae33c509be23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/11f25cfda4e2f210
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/122419b0bc04bb24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1322b93a2154c54a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/134e5e8c29726e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/13985ae090677282
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/146952ec4263c5d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/150d086b8b4de9d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/156301591af184f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1663be342a34f83
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1895bed4a0ed65d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1996a22aec44a5c0
+-rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1a4449eb8b26a401
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1a4db4c4834af592
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1b0530edc3fe075e
+-rw-r--r--   0        0        0    21464 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1b7872d6314f48b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1ce202f3daa889d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1cfd31ba4b0b7ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1dcbdc62e66ccf0e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1edace855ae3c841
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1f7ac4f892285f60
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/1fbfdffa4078f509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/20b40aca78f395e8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/219bf1f8f2938bd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/21b248d368a93ac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/21cf950ddc412c7b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/22db1408b8f4a4b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/232d0222563916a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/23680c0655621b13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/247546336fc4bd59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/248d23bfc4586461
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/24e2ebef92fa75b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/25d9504d2b6847d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/26657ed11f8e66de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/269f98f304a03fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/28caf6cfecd38c1a
+-rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/294d5a468695eb7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/29531d612e8a868a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2a383abdede299d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2a5d8d1386804aed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2a630c7d6d7faa40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2b0cdebce71424f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2bc4a20be77b881b
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2bf27b960bc3ded1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2c189a9882594507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2c6eeab804b5c1f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2c9bbc6bae6b0f41
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2d77da04c7119543
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2e4746b83d2d1cf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2e6b6d5e70ae29db
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2e8708077cd0413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2f9e25dc2ce777cc
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/2face4e073dced28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/300f9a816018d49f
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/30e241b2876dc71f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/31813abf4ed82b53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3271e344462a0ee3
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/33004598889f4950
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/349f044f89b94587
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/34a4aaded634d537
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/34e1109d49bf09f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/356d28a11355e7a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/357e837fe90ee680
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/35ab5ee4981cdf8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/35ba35b3f04c192f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/36372ef94f8716cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/36e48551be186a66
+-rw-r--r--   0        0        0    16058 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/36f0bdaeef592d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/380a13ecd1a2af25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/38962215221b245a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/38d9da4e93811c4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/39285e72757cc499
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/399d3b28a1a1db47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3a74e1b5704e9b3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3af645c926072f97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3c6b70c96e832bc1
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3c7fb493febe6a55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3c9bb20c3b57bae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3ca706f99b2d38bf
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3ccdd2336c8c80e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3cf13d9d13babf93
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3db675ebeb97b2fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3e0ec316d612ddc6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3e35311bfb3345f8
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3f10d9d7687f3999
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/3f12e7a3fe46c220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/417040cdeaa7bd81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/429010e306ea9808
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/42f337caed884834
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/431bdba29473eca0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4536434fd84cdba5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/467fc2e82c277fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/47affd4e531897a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/47ca38fe0242f05d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/47e54ee652d2f4c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4843e1c724479e6a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/484730e7d1a4dcd9
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4880724f1f6a1ac8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/48bda5931a9eb062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/49fafbbbbadedf00
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4a63ed784e7c5ec0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4ac8c08e5b1b6650
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4b5890a0c8dc15df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4cd4c52ee1dc7ffe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4cdd16a7f9738f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4eaf3b155fae0dfb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4f16c6852dea8eca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4f2c663677c63589
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/4fafe0dbefb778fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/50373733f4645c5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/514fb27e4aef5783
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/519ab6ce866ef11b
+-rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/51de14ac05bcd5d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/529312a72d1177a1
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/534b8acecf74c47
+-rw-r--r--   0        0        0    20136 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/536320baecd03af6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/538fc0618c4d4c31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/53c0f85a3179a38f
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5436d767d06cf116
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/54637ff0aaaaf6b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/552fa1eb2057eecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5548c3ce5fff0cca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/556b5cfaac0c49bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/55c947c0fa59929
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/568d77a0a0a64dbc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/56e83f1c5eeb3eba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/572ba1efb5bb3fd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/58240cde188220d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/584058f21d3e2fa1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/594d55ee247cbdef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/59cfab1472b544fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5a6dc8ef65620223
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5af13ad9cc04e932
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5b8fb96822a8f127
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5b965ef6adf36c8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5badc1835a2b80e1
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5cc5d54a963753bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5da466fd7e3b19f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5e83ab1d520dc773
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5efe825a5e773b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/5fb3763e0810c38a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/62396a4dea084957
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/624348590d33bdc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6278996c2e6b2a87
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/63dbabe01e9e6756
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6550bbd98b1711bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6791fc0114ddc05
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6845ca4e0c56952b
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/68c4553df91c1f5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/69bb9ea6355c0c25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/69ffc3e7ad0aa6b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6a4adfab73a8d4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6a74d0efd6350f1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6b596d4ac1166741
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6b9f30172d33b6a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6bcca98e41cda3f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6beed9d45ff1a491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6c989c6e4eea10bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6db20c27780d4a5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6db875fe1541793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6eab8cdd7b4ae170
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/6fc044c94dc3532a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/701212523f7b3b9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/70963c0c68bf76ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/70bd045859d6cb20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/70d6f3b95738758d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/729f212cc9c6cd5d
+-rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/72a6612daca66426
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/72de7bec9ecb53aa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/733b2373fa4ae335
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7396a954cc3b124a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7485843a948a75b0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/755c9c217a06f932
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/75bb48e114159509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/76d56794deeb084d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/76fbe2af0f71bd4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/79a22043e5c16946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/79c3fb2c81fd59a0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7a19353a5daa4a37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7b3a1bf0b652398a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7bf45647f43eaf85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7c01d9689dd16a64
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7c37d34a0c059ec7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7c806e58272a88ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7cbc35f4e814db65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7cc3783d00621498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7dc27d897f910c11
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7e138932f0b9a1bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7eb1422c10ced038
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7eb17a25b4fa1d13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7f0f63895e369318
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/7f75cbd11ebac70a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8012caf4fb290dc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/809075c58fb87c61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/80dbccb0d26b4b4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/80ded2016f4f413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/81e3edf198d6c468
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/81e6f787866d0ecf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/82ab0276d38aec9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/83a59cf9aceae1d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/83cdfb5da134b21f
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/84e2e26fc69ab274
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/84e8c31ce428d3ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/858df3976aef9624
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/868699acd08be339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/86c3e5b9f79f490f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/87a7b0840a5cf8c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/87d9b6d5e7bcb6c7
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/881c84062ed51136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/886d14b97dbd4f2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8944dfd1b590bdd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/89c7a4d643f68517
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/89e58e5ee0d7d864
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8a0279b11d098d9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8a437c05421c6cb5
+-rw-r--r--   0        0        0    20054 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8a5ec4ca9660671c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8b8acf1607bcb3f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8c34e85d573e230f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8d2f83aae152de29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8df3988e9368cbe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/8f33397e19bead30
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9019e33ca68d8935
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/902eb6f99ee41131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/906cef8208fbf28f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9080aaa3f2416b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/922bfc03482db456
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/92db151fe9967fd3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9352425265579062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/93fed7ae4120c88e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/945994955724de24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/94ffcc82bc7ee370
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/95df46a8e947b100
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9613cbbc5a7c60a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/968b32ac9319cc53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/97a72bc70808d2f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/97cbf45b388709d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/97df9d79e599f082
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/981eb70eb69fb3ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/98392e87ef3eb254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/99d5decc6ca01825
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9a5552199a8b8bd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9bd08ae684645cf6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9c1285d5b3178abe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9cbaa57406e65f63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9d0f65e1ab7ca23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9db15fb6e71bec4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9dda9185d48774f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9e3b1a7c0f34103b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9e50a4d6fb3c9688
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9e558f66f216c4eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9e915e4e576201bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9ec2a872083329d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9edacb4de19eeb8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9f0f8b1c56898117
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9f2c57bc030e0b04
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/9f330edc61f02d3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a0572377dc282cac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a113f7e28da04408
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a24edf91b0bcff12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a2fe93c3bba310b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a38eff4f06853e65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a78089cbf54aff62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a8da9d8efa986532
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a925b8cd7505ac0a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a92bb1bdda49ef61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/a943564382aec90a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/aa3f7accc1718239
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ab360402eb2d795e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ab4a97b5d68b837a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/abc8db1325696a17
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/abe0d13d37518e58
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ac5b9f591ce9edec
+-rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ac8c237c67408442
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/acbc9f45cfeee4dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/acecedeb9f4dd91a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ad02b8e4575abc6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ae5a30e888e80958
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/aff288abf6945582
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b08de429bee9ce93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b2d26e3968f3c218
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b2f061a9d80cfa8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b4228843afe3d2eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b56a01688e02e5f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b5c4e8c097cbf198
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b5f69f56d932f0d1
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b6191d72e3d9a646
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b61cd4b71d14e881
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b7331c702909633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b7b1c8254943be90
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b7bcb1e4c5eea72b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b81f55dc9d767e8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b82ae772ad3347b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b89a404ae8aaa495
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b89dc34e1d21508f
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b8ab8c7df580ad75
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/b990e7d90d89db2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ba0f74a0540d9a5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ba66feb1819b5312
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bbd87fc7f90c1f28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bd12e3fd28591ae6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bd1e909ba96cca61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bdd37795dc331d56
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bde6d6e902485336
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/bdeb811362915192
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/be5eb6e8ff99feab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/be9c428a6192e049
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/beb37e84505d7dd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c0d14d0162a80714
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c10a38d72f60e675
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c121acc012633d2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c18d3e52506df649
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c250dc207334d18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c25779f3e34a584a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c293dd30723003b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c3329258d804dff6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c40a4c8f88b65414
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c55a79e89225a078
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c62dd73faf917878
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c766d7d105d53e92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c82d4fd611732d02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c88465e3c1dc503e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c8c7b8092b03fdd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/c9d297807d108576
+-rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ca3d1e0ddece82f5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cb0e3b769b6a1727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cb2f84958966b77c
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cb326dd0ee5910c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cbb8b9fccd8c8746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cc518cf199497e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ccc4c37cd56e46e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ccf15ba8d3af2d15
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cd61466cc4a76933
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ce0a51ca403a72f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ce7ae4869b72ad31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cee8b7a480495342
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/cfa33b7a8aeb793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d085b6ebe7bb0389
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d0be3a4705e047c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d0fd170547b6bb47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d1c81941e3ef2e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d1d63b74d8d929b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d203b8acf8460019
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d2cceb9cc8265e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d3a20b1509715554
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d551c518ebaaf23a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d5a9ce7dc11e5edc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d6b8c7cba735b946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d825cf3987ee9f33
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d8444fda03b67f2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d86a45eca9289fa5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d9198ab6e1ae45a0
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d954f2ee22d56fd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d9b321d36a255169
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/d9cd4c2a9ad4580d
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/da0cf7e13e17e6a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/da4aff17737df0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/da94ab81ae4dffd1
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/db73ef232740be87
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/dc4a4b4b55cceada
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/dcb2ce27d1f7cc70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/de1238012a6853f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/dec4fb820d1aee1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/decdb847958ce882
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/dfc2e498a5736fb3
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e067c98663409f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e07d7deee3f2b1ed
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e24118b3523194dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e316b4f368a31a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e4a016e6cc51d759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e59ac15827b7f1c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e6237a2dffed4f5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e6e7d13cd57b4fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e832a8f80eaf16d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e8ab3d919ff04fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e8cd5143f259cdce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/e98cf82519b9efc2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ea450af950172f80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ebd9c23038b8db35
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ec04e1ad73846b2a
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ed03e948b89996b8
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ed645de094b6d7bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/edbe26c4bd7599ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/ee965a83d6cd2aaa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f002d9727bf66a12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f1af1d1ebb07ad61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f2942d8cb87b15e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f4088198fa879c9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f41987c18d73e01d
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f4d6392808939633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f4e7c96257c9d24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f586c8a0f5c58b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f58e778cbde5b210
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f5d61064e60c404b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/f9ab84e0c6669bed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fa23c022574446ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fa2e112681e24616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fa354595b122bf9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/faa3132a8644ec4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fad49b925cd80258
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fb9901f753a46f52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fbd81c0d9b22b507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fd089a45384d0959
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 su6-1.4.2/.ruff_cache/content/fd17e608110a0864
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 su6-1.4.2/_static/su6.svg
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 su6-1.4.2/docs/plugins.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_2602a302b50854cf___about___py.html
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_2602a302b50854cf___init___py.html
+-rw-r--r--   0        0        0   120042 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_2602a302b50854cf_cli_py.html
+-rw-r--r--   0        0        0   161698 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_2602a302b50854cf_core_py.html
+-rw-r--r--   0        0        0    92303 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_2602a302b50854cf_plugins_py.html
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_a44f0ac069e85531__shared_py.html
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_a44f0ac069e85531_test_about_py.html
+-rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_a44f0ac069e85531_test_cli_py.html
+-rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/d_a44f0ac069e85531_test_core_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-1.4.2/htmlcov/style.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/bad.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/black_good_mypy_bad.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/empty.toml
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/except_pytest.toml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/fake_module.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/good.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/invalid.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/only_black.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/only_mypy.toml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/stop_after_first.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/bad.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/bad.meta.json
+-rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-1.4.2/src/su6/__about__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 su6-1.4.2/src/su6/__init__.py
+-rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 su6-1.4.2/src/su6/cli.py
+-rw-r--r--   0        0        0    17551 2020-02-02 00:00:00.000000 su6-1.4.2/src/su6/core.py
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 su6-1.4.2/src/su6/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 su6-1.4.2/src/su6/py.typed
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-1.4.2/tests/_shared.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-1.4.2/tests/test_about.py
+-rw-r--r--   0        0        0     9632 2020-02-02 00:00:00.000000 su6-1.4.2/tests/test_cli.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 su6-1.4.2/tests/test_core.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-1.4.2/tests/test_plugins.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 su6-1.4.2/tests/test_plugins_config.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-1.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 su6-1.4.2/README.md
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 su6-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 su6-1.4.2/PKG-INFO
```

### Comparing `su6-1.4.1/CHANGELOG.md` & `su6-1.4.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.2 (2023-06-19)
+
+### Documentation
+
+* **readme:** Fix icon to master branch ([`d2e3a7c`](https://github.com/robinvandernoord/su6-checker/commit/d2e3a7c7dfa87236ad42e00074b46f5e4a30378f))
+* **readme:** Add icon ([`640c383`](https://github.com/robinvandernoord/su6-checker/commit/640c38318e579222a1ce641bf46c8c541a421bad))
+
 ## v1.4.1 (2023-06-19)
 
 ### Fix
 
 * **config:** Use .update functionality from `configuraptor`. ([`aa09931`](https://github.com/robinvandernoord/su6-checker/commit/aa0993167e42d878689723a9d337bdc244082914))
 
 ## v1.4.0 (2023-06-15)
```

### Comparing `su6-1.4.1/coverage.svg` & `su6-1.4.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/__future__.data.json` & `su6-1.4.2/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/__future__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_ast.data.json` & `su6-1.4.2/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_ast.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_codecs.data.json` & `su6-1.4.2/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_codecs.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_collections_abc.data.json` & `su6-1.4.2/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_csv.data.json` & `su6-1.4.2/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_csv.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_ctypes.data.json` & `su6-1.4.2/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_ctypes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_decimal.data.json` & `su6-1.4.2/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_decimal.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_operator.data.json` & `su6-1.4.2/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_operator.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_random.data.json` & `su6-1.4.2/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_random.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_socket.data.json` & `su6-1.4.2/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_socket.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_stat.data.json` & `su6-1.4.2/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_stat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_thread.data.json` & `su6-1.4.2/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_thread.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_warnings.data.json` & `su6-1.4.2/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_warnings.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_weakref.data.json` & `su6-1.4.2/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_weakref.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_weakrefset.data.json` & `su6-1.4.2/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/abc.data.json` & `su6-1.4.2/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/abc.meta.json` & `su6-1.4.2/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/argparse.data.json` & `su6-1.4.2/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/argparse.meta.json` & `su6-1.4.2/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/array.data.json` & `su6-1.4.2/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/array.meta.json` & `su6-1.4.2/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ast.data.json` & `su6-1.4.2/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ast.meta.json` & `su6-1.4.2/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/builtins.data.json` & `su6-1.4.2/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/builtins.meta.json` & `su6-1.4.2/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/codecs.data.json` & `su6-1.4.2/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/codecs.meta.json` & `su6-1.4.2/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/colorsys.data.json` & `su6-1.4.2/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/colorsys.meta.json` & `su6-1.4.2/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configparser.data.json` & `su6-1.4.2/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configparser.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/contextlib.data.json` & `su6-1.4.2/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/contextlib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/contextvars.data.json` & `su6-1.4.2/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/contextvars.meta.json` & `su6-1.4.2/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/copy.data.json` & `su6-1.4.2/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/copy.meta.json` & `su6-1.4.2/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/copyreg.data.json` & `su6-1.4.2/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/copyreg.meta.json` & `su6-1.4.2/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/csv.data.json` & `su6-1.4.2/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/csv.meta.json` & `su6-1.4.2/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/dataclasses.data.json` & `su6-1.4.2/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/dataclasses.meta.json` & `su6-1.4.2/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/datetime.data.json` & `su6-1.4.2/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/datetime.meta.json` & `su6-1.4.2/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/decimal.data.json` & `su6-1.4.2/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/decimal.meta.json` & `su6-1.4.2/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/difflib.data.json` & `su6-1.4.2/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/difflib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/dis.data.json` & `su6-1.4.2/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/dis.meta.json` & `su6-1.4.2/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/enum.data.json` & `su6-1.4.2/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/enum.meta.json` & `su6-1.4.2/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/errno.data.json` & `su6-1.4.2/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/errno.meta.json` & `su6-1.4.2/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/fractions.data.json` & `su6-1.4.2/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/fractions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/functools.data.json` & `su6-1.4.2/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/functools.meta.json` & `su6-1.4.2/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/genericpath.data.json` & `su6-1.4.2/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/genericpath.meta.json` & `su6-1.4.2/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/getpass.data.json` & `su6-1.4.2/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/getpass.meta.json` & `su6-1.4.2/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/gettext.data.json` & `su6-1.4.2/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/gettext.meta.json` & `su6-1.4.2/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/glob.data.json` & `su6-1.4.2/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/glob.meta.json` & `su6-1.4.2/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/good.data.json` & `su6-1.4.2/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/good.meta.json` & `su6-1.4.2/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/hashlib.data.json` & `su6-1.4.2/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/hashlib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/hmac.data.json` & `su6-1.4.2/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/hmac.meta.json` & `su6-1.4.2/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/inspect.data.json` & `su6-1.4.2/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/inspect.meta.json` & `su6-1.4.2/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/io.data.json` & `su6-1.4.2/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/io.meta.json` & `su6-1.4.2/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/itertools.data.json` & `su6-1.4.2/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/itertools.meta.json` & `su6-1.4.2/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/linecache.data.json` & `su6-1.4.2/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/linecache.meta.json` & `su6-1.4.2/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/marshal.data.json` & `su6-1.4.2/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/marshal.meta.json` & `su6-1.4.2/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/math.data.json` & `su6-1.4.2/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/math.meta.json` & `su6-1.4.2/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mmap.data.json` & `su6-1.4.2/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mmap.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/msvcrt.data.json` & `su6-1.4.2/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/msvcrt.meta.json` & `su6-1.4.2/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mypy_extensions.data.json` & `su6-1.4.2/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mypy_extensions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/numbers.data.json` & `su6-1.4.2/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/numbers.meta.json` & `su6-1.4.2/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/opcode.data.json` & `su6-1.4.2/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/opcode.meta.json` & `su6-1.4.2/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/operator.data.json` & `su6-1.4.2/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/operator.meta.json` & `su6-1.4.2/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathlib.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathlib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pickle.data.json` & `su6-1.4.2/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pickle.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platform.data.json` & `su6-1.4.2/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platform.meta.json` & `su6-1.4.2/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/posixpath.data.json` & `su6-1.4.2/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/posixpath.meta.json` & `su6-1.4.2/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pty.data.json` & `su6-1.4.2/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pty.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pydoc.data.json` & `su6-1.4.2/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pydoc.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/queue.data.json` & `su6-1.4.2/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/queue.meta.json` & `su6-1.4.2/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/random.data.json` & `su6-1.4.2/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/random.meta.json` & `su6-1.4.2/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/re.data.json` & `su6-1.4.2/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/re.meta.json` & `su6-1.4.2/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/reprlib.data.json` & `su6-1.4.2/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/reprlib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/secrets.data.json` & `su6-1.4.2/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/secrets.meta.json` & `su6-1.4.2/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/selectors.data.json` & `su6-1.4.2/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/selectors.meta.json` & `su6-1.4.2/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/shlex.data.json` & `su6-1.4.2/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/shlex.meta.json` & `su6-1.4.2/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/shutil.data.json` & `su6-1.4.2/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/shutil.meta.json` & `su6-1.4.2/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/signal.data.json` & `su6-1.4.2/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/signal.meta.json` & `su6-1.4.2/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/socket.data.json` & `su6-1.4.2/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/socket.meta.json` & `su6-1.4.2/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sre_compile.data.json` & `su6-1.4.2/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sre_compile.meta.json` & `su6-1.4.2/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sre_constants.data.json` & `su6-1.4.2/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sre_constants.meta.json` & `su6-1.4.2/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sre_parse.data.json` & `su6-1.4.2/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sre_parse.meta.json` & `su6-1.4.2/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ssl.data.json` & `su6-1.4.2/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ssl.meta.json` & `su6-1.4.2/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/stat.data.json` & `su6-1.4.2/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/stat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/string.data.json` & `su6-1.4.2/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/string.meta.json` & `su6-1.4.2/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/struct.data.json` & `su6-1.4.2/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/struct.meta.json` & `su6-1.4.2/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/subprocess.data.json` & `su6-1.4.2/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/subprocess.meta.json` & `su6-1.4.2/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sys.data.json` & `su6-1.4.2/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sys.meta.json` & `su6-1.4.2/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sysconfig.data.json` & `su6-1.4.2/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/sysconfig.meta.json` & `su6-1.4.2/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tempfile.data.json` & `su6-1.4.2/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tempfile.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/termios.data.json` & `su6-1.4.2/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/termios.meta.json` & `su6-1.4.2/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/textwrap.data.json` & `su6-1.4.2/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/textwrap.meta.json` & `su6-1.4.2/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/this.data.json` & `su6-1.4.2/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/this.meta.json` & `su6-1.4.2/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/threading.data.json` & `su6-1.4.2/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/threading.meta.json` & `su6-1.4.2/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/time.data.json` & `su6-1.4.2/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/time.meta.json` & `su6-1.4.2/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/token.data.json` & `su6-1.4.2/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/token.meta.json` & `su6-1.4.2/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tokenize.data.json` & `su6-1.4.2/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tokenize.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomllib.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomllib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/traceback.data.json` & `su6-1.4.2/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/traceback.meta.json` & `su6-1.4.2/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tty.data.json` & `su6-1.4.2/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tty.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/types.data.json` & `su6-1.4.2/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/types.meta.json` & `su6-1.4.2/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typing.data.json` & `su6-1.4.2/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typing.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typing_extensions.data.json` & `su6-1.4.2/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/uuid.data.json` & `su6-1.4.2/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/uuid.meta.json` & `su6-1.4.2/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/warnings.data.json` & `su6-1.4.2/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/warnings.meta.json` & `su6-1.4.2/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/weakref.data.json` & `su6-1.4.2/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/weakref.meta.json` & `su6-1.4.2/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/webbrowser.data.json` & `su6-1.4.2/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/webbrowser.meta.json` & `su6-1.4.2/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/zlib.data.json` & `su6-1.4.2/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/zlib.meta.json` & `su6-1.4.2/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/base_events.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/events.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/events.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/futures.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/futures.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/locks.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/locks.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/mixins.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/protocols.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/queues.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/queues.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/runners.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/runners.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/streams.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/streams.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/tasks.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/threads.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/threads.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/transports.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/transports.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.data.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `su6-1.4.2/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/_width_table.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/_width_table.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/brackets.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/brackets.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/cache.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/cache.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/comments.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/comments.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/concurrency.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/concurrency.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/const.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/const.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/files.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/files.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/linegen.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/linegen.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/lines.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/lines.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/mode.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/mode.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/nodes.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/nodes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/numerics.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/numerics.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/output.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/output.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/parsing.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/parsing.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/report.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/report.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/rusty.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/rusty.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/strings.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/strings.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/trans.data.json` & `su6-1.4.2/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/black/trans.meta.json` & `su6-1.4.2/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/_compat.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/_compat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/core.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/core.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/decorators.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/decorators.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/exceptions.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/formatting.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/formatting.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/globals.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/globals.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/parser.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/parser.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/termui.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/termui.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/types.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/types.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/click/utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/collections/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/collections/abc.data.json` & `su6-1.4.2/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/collections/abc.meta.json` & `su6-1.4.2/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.data.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `su6-1.4.2/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/cls.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/cls.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/cls.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/core.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/core.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/dump.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/dump.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/dump.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/errors.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/helpers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/helpers.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/postpone.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/postpone.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/postpone.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/singleton.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/singleton.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/singleton.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/_types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_310.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_310.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json` & `su6-1.4.2/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-1.4.2/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/charset.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/charset.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/errors.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/errors.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/header.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/header.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/message.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/message.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/policy.data.json` & `su6-1.4.2/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/email/policy.meta.json` & `su6-1.4.2/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/html/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/html/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/html/entities.data.json` & `su6-1.4.2/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/html/entities.meta.json` & `su6-1.4.2/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/abc.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/util.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/util.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-1.4.2/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/json/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/json/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/json/decoder.data.json` & `su6-1.4.2/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/json/decoder.meta.json` & `su6-1.4.2/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/json/encoder.data.json` & `su6-1.4.2/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/json/encoder.meta.json` & `su6-1.4.2/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/logging/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-1.4.2/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-1.4.2/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/context.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/process.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.data.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/multiprocessing/util.meta.json` & `su6-1.4.2/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/os/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/os/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/os/path.data.json` & `su6-1.4.2/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/os/path.meta.json` & `su6-1.4.2/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_elffile.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_structures.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/_structures.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/specifiers.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/tags.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/tags.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/version.data.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/packaging/version.meta.json` & `su6-1.4.2/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/_meta.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/pattern.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/util.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/util.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `su6-1.4.2/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/android.data.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/android.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/android.meta.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/android.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/api.data.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/api.meta.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.data.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/unix.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/unix.meta.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/unix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/version.data.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/platformdirs/version.meta.json` & `su6-1.4.2/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/__main__.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_extension.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_loop.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_pick.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_stack.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_timer.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_windows.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/abc.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/abc.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/align.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/align.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/ansi.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/box.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/box.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/cells.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/cells.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/color.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/color.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/columns.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/columns.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/console.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/console.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/constrain.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/containers.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/containers.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/control.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/control.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/emoji.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/errors.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/errors.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/json.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/json.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/live.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/live.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/live_render.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/markdown.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/markup.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/markup.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/measure.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/measure.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/padding.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/padding.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/pager.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/pager.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/palette.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/palette.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/panel.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/panel.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/pretty.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/protocol.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/region.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/region.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/repr.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/repr.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/rule.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/rule.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/scope.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/scope.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/screen.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/screen.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/segment.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/segment.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/spinner.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/status.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/status.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/style.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/style.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/styled.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/styled.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/syntax.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/table.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/table.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/text.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/text.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/theme.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/theme.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/themes.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/themes.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/traceback.data.json` & `su6-1.4.2/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-1.4.2/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/__about__.data.json` & `su6-1.4.2/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/__about__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/cli.data.json` & `su6-1.4.2/.mypy_cache/3.11/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/cli.meta.json` & `su6-1.4.2/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/core.data.json` & `su6-1.4.2/.mypy_cache/3.11/su6/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/core.meta.json` & `su6-1.4.2/.mypy_cache/3.11/su6/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/plugins.data.json` & `su6-1.4.2/.mypy_cache/3.11/su6/plugins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/su6/plugins.meta.json` & `su6-1.4.2/.mypy_cache/3.11/su6/plugins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/_compat.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/_utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/api.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/api.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/container.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/container.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/container.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/container.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/items.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/items.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/items.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/items.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/parser.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/source.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/source.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/source.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/source.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_char.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_char.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.data.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_document.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json` & `su6-1.4.2/.mypy_cache/3.11/tomlkit/toml_document.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_config.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_config.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_functions.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_memo.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typeguard/_utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_typing.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/colors.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/colors.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/completion.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/completion.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/core.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/core.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/main.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/main.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/models.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/models.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/params.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/params.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/utils.data.json` & `su6-1.4.2/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/typer/utils.meta.json` & `su6-1.4.2/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/_log.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/_log.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/async_case.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/async_case.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/case.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/case.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/loader.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/loader.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/main.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/main.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/mock.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/mock.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/result.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/result.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/runner.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/runner.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/signals.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/signals.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/suite.data.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/unittest/suite.meta.json` & `su6-1.4.2/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-1.4.2/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-1.4.2/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/urllib/parse.data.json` & `su6-1.4.2/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-1.4.2/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.pytest_cache/v/cache/nodeids` & `su6-1.4.2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/122419b0bc04bb24` & `su6-1.4.2/.ruff_cache/content/122419b0bc04bb24`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/1a4449eb8b26a401` & `su6-1.4.2/.ruff_cache/content/1a4449eb8b26a401`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/1b7872d6314f48b7` & `su6-1.4.2/.ruff_cache/content/1b7872d6314f48b7`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-1.4.2/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/294d5a468695eb7e` & `su6-1.4.2/.ruff_cache/content/294d5a468695eb7e`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/2bf27b960bc3ded1` & `su6-1.4.2/.ruff_cache/content/2bf27b960bc3ded1`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/2face4e073dced28` & `su6-1.4.2/.ruff_cache/content/2face4e073dced28`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/30e241b2876dc71f` & `su6-1.4.2/.ruff_cache/content/30e241b2876dc71f`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/33004598889f4950` & `su6-1.4.2/.ruff_cache/content/33004598889f4950`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/36f0bdaeef592d9` & `su6-1.4.2/.ruff_cache/content/36f0bdaeef592d9`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/3c7fb493febe6a55` & `su6-1.4.2/.ruff_cache/content/3c7fb493febe6a55`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/3ccdd2336c8c80e9` & `su6-1.4.2/.ruff_cache/content/3ccdd2336c8c80e9`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/3db675ebeb97b2fe` & `su6-1.4.2/.ruff_cache/content/3db675ebeb97b2fe`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/3f10d9d7687f3999` & `su6-1.4.2/.ruff_cache/content/3f10d9d7687f3999`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/42f337caed884834` & `su6-1.4.2/.ruff_cache/content/42f337caed884834`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/51de14ac05bcd5d1` & `su6-1.4.2/.ruff_cache/content/51de14ac05bcd5d1`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/534b8acecf74c47` & `su6-1.4.2/.ruff_cache/content/534b8acecf74c47`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/536320baecd03af6` & `su6-1.4.2/.ruff_cache/content/536320baecd03af6`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/5436d767d06cf116` & `su6-1.4.2/.ruff_cache/content/5436d767d06cf116`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/5cc5d54a963753bf` & `su6-1.4.2/.ruff_cache/content/5cc5d54a963753bf`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/684d0841c18787fb` & `su6-1.4.2/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/68c4553df91c1f5e` & `su6-1.4.2/.ruff_cache/content/68c4553df91c1f5e`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/72a6612daca66426` & `su6-1.4.2/.ruff_cache/content/72a6612daca66426`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/81e6f787866d0ecf` & `su6-1.4.2/.ruff_cache/content/81e6f787866d0ecf`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/84e2e26fc69ab274` & `su6-1.4.2/.ruff_cache/content/84e2e26fc69ab274`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/881c84062ed51136` & `su6-1.4.2/.ruff_cache/content/881c84062ed51136`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/8a5ec4ca9660671c` & `su6-1.4.2/.ruff_cache/content/8a5ec4ca9660671c`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/9019e33ca68d8935` & `su6-1.4.2/.ruff_cache/content/9019e33ca68d8935`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/95df46a8e947b100` & `su6-1.4.2/.ruff_cache/content/95df46a8e947b100`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/9613cbbc5a7c60a4` & `su6-1.4.2/.ruff_cache/content/9613cbbc5a7c60a4`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/abe0d13d37518e58` & `su6-1.4.2/.ruff_cache/content/abe0d13d37518e58`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/ac8c237c67408442` & `su6-1.4.2/.ruff_cache/content/ac8c237c67408442`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/b8ab8c7df580ad75` & `su6-1.4.2/.ruff_cache/content/b8ab8c7df580ad75`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/b8d965aa2b8fd993` & `su6-1.4.2/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/b990e7d90d89db2a` & `su6-1.4.2/.ruff_cache/content/b990e7d90d89db2a`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/bde6d6e902485336` & `su6-1.4.2/.ruff_cache/content/bde6d6e902485336`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/be4a1815dbb4c4` & `su6-1.4.2/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/be5eb6e8ff99feab` & `su6-1.4.2/.ruff_cache/content/be5eb6e8ff99feab`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/ca3d1e0ddece82f5` & `su6-1.4.2/.ruff_cache/content/ca3d1e0ddece82f5`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/cb326dd0ee5910c6` & `su6-1.4.2/.ruff_cache/content/cb326dd0ee5910c6`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/d954f2ee22d56fd0` & `su6-1.4.2/.ruff_cache/content/d954f2ee22d56fd0`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/da0cf7e13e17e6a6` & `su6-1.4.2/.ruff_cache/content/da0cf7e13e17e6a6`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/db73ef232740be87` & `su6-1.4.2/.ruff_cache/content/db73ef232740be87`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/dc4a4b4b55cceada` & `su6-1.4.2/.ruff_cache/content/dc4a4b4b55cceada`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/e067c98663409f12` & `su6-1.4.2/.ruff_cache/content/e067c98663409f12`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/e24118b3523194dc` & `su6-1.4.2/.ruff_cache/content/e24118b3523194dc`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/ed03e948b89996b8` & `su6-1.4.2/.ruff_cache/content/ed03e948b89996b8`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/ed645de094b6d7bb` & `su6-1.4.2/.ruff_cache/content/ed645de094b6d7bb`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/f5d61064e60c404b` & `su6-1.4.2/.ruff_cache/content/f5d61064e60c404b`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/.ruff_cache/content/fd17e608110a0864` & `su6-1.4.2/.ruff_cache/content/fd17e608110a0864`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/docs/plugins.md` & `su6-1.4.2/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/coverage_html.js` & `su6-1.4.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_2602a302b50854cf___about___py.html` & `su6-1.4.2/htmlcov/d_2602a302b50854cf___about___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_2602a302b50854cf___init___py.html` & `su6-1.4.2/htmlcov/d_2602a302b50854cf___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_2602a302b50854cf_cli_py.html` & `su6-1.4.2/htmlcov/d_2602a302b50854cf_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_2602a302b50854cf_core_py.html` & `su6-1.4.2/htmlcov/d_2602a302b50854cf_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_2602a302b50854cf_plugins_py.html` & `su6-1.4.2/htmlcov/d_2602a302b50854cf_plugins_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_a44f0ac069e85531___init___py.html` & `su6-1.4.2/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_a44f0ac069e85531__shared_py.html` & `su6-1.4.2/htmlcov/d_a44f0ac069e85531__shared_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_about_py.html` & `su6-1.4.2/htmlcov/d_a44f0ac069e85531_test_about_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_cli_py.html` & `su6-1.4.2/htmlcov/d_a44f0ac069e85531_test_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/d_a44f0ac069e85531_test_core_py.html` & `su6-1.4.2/htmlcov/d_a44f0ac069e85531_test_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/favicon_32.png` & `su6-1.4.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/index.html` & `su6-1.4.2/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/keybd_closed.png` & `su6-1.4.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/keybd_open.png` & `su6-1.4.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/status.json` & `su6-1.4.2/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/htmlcov/style.css` & `su6-1.4.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/except_pytest.toml` & `su6-1.4.2/pytest_examples/except_pytest.toml`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ast.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_codecs.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/abc.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/array.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/bad.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/bad.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/bad.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/builtins.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/codecs.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/contextlib.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/enum.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/genericpath.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/good.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/io.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/mmap.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pathlib.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/pickle.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/posixpath.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/re.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/subprocess.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/sys.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/this.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/types.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/charset.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/errors.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/header.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/message.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/email/policy.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.data.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/pytest_examples/.mypy_cache/3.11/os/path.meta.json` & `su6-1.4.2/pytest_examples/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/src/su6/__init__.py` & `su6-1.4.2/src/su6/__init__.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/src/su6/cli.py` & `su6-1.4.2/src/su6/cli.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/src/su6/core.py` & `su6-1.4.2/src/su6/core.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/src/su6/plugins.py` & `su6-1.4.2/src/su6/plugins.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/tests/test_cli.py` & `su6-1.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/tests/test_core.py` & `su6-1.4.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/tests/test_plugins.py` & `su6-1.4.2/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/tests/test_plugins_config.py` & `su6-1.4.2/tests/test_plugins_config.py`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/LICENSE.txt` & `su6-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/README.md` & `su6-1.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,420 +1,455 @@
-00000000: 2320 7375 362d 6368 6563 6b65 720a 0a5b  # su6-checker..[
-00000010: 215b 5079 5049 202d 2056 6572 7369 6f6e  ![PyPI - Version
-00000020: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000030: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-00000040: 7375 362e 7376 6729 5d28 6874 7470 733a  su6.svg)](https:
-00000050: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000060: 6374 2f73 7536 290a 5b21 5b50 7950 4920  ct/su6).[![PyPI 
-00000070: 2d20 5079 7468 6f6e 2056 6572 7369 6f6e  - Python Version
-00000080: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000090: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
-000000a0: 7665 7273 696f 6e73 2f73 7536 2e73 7667  versions/su6.svg
-000000b0: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-000000c0: 6f72 672f 7072 6f6a 6563 742f 7375 3629  org/project/su6)
-000000d0: 2020 0a5b 215b 436f 6465 2073 7479 6c65    .[![Code style
-000000e0: 3a20 626c 6163 6b5d 2868 7474 7073 3a2f  : black](https:/
-000000f0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000100: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
-00000110: 6c65 2d62 6c61 636b 2d30 3030 3030 302e  le-black-000000.
-00000120: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-00000130: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-00000140: 636b 290a 5b21 5b4c 6963 656e 7365 3a20  ck).[![License: 
-00000150: 4d49 545d 2868 7474 7073 3a2f 2f69 6d67  MIT](https://img
-00000160: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000170: 652f 4c69 6365 6e73 652d 4d49 542d 7965  e/License-MIT-ye
-00000180: 6c6c 6f77 2e73 7667 295d 2868 7474 7073  llow.svg)](https
-00000190: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6f72  ://opensource.or
-000001a0: 672f 6c69 6365 6e73 6573 2f4d 4954 2920  g/licenses/MIT) 
-000001b0: 200a 5b21 5b73 7536 2063 6865 636b 735d   .[![su6 checks]
-000001c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000001d0: 636f 6d2f 726f 6269 6e76 616e 6465 726e  com/robinvandern
-000001e0: 6f6f 7264 2f73 7536 2d63 6865 636b 6572  oord/su6-checker
-000001f0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000200: 7773 2f73 7536 2e79 6d6c 2f62 6164 6765  ws/su6.yml/badge
-00000210: 2e73 7667 3f62 7261 6e63 683d 6465 7665  .svg?branch=deve
-00000220: 6c6f 706d 656e 7429 5d28 6874 7470 733a  lopment)](https:
-00000230: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6f62  //github.com/rob
-00000240: 696e 7661 6e64 6572 6e6f 6f72 642f 7375  invandernoord/su
-00000250: 362d 6368 6563 6b65 722f 6163 7469 6f6e  6-checker/action
-00000260: 7329 0a21 5b63 6f76 6572 6167 652e 7376  s).![coverage.sv
-00000270: 675d 2863 6f76 6572 6167 652e 7376 6729  g](coverage.svg)
-00000280: 0a0a 2d2d 2d2d 2d0a 7375 3620 2836 2069  ..-----.su6 (6 i
-00000290: 7320 7072 6f6e 6f75 6e63 6564 2061 7320  s pronounced as 
-000002a0: 272f 7ac9 9b73 2f27 2069 6e20 4475 7463  '/z..s/' in Dutc
-000002b0: 682c 2073 6f20 2773 7536 2720 6973 2062  h, so 'su6' is b
-000002c0: 6173 6963 616c 6c79 2027 7375 6363 6573  asically 'succes
-000002d0: 7327 2920 200a 5468 6973 2070 6163 6b61  s')  .This packa
-000002e0: 6765 2077 696c 6c20 686f 7065 6675 6c6c  ge will hopefull
-000002f0: 7920 6865 6c70 2061 6368 6965 7665 2074  y help achieve t
-00000300: 6861 7421 0a0a 2a2a 5461 626c 6520 6f66  hat!..**Table of
-00000310: 2043 6f6e 7465 6e74 732a 2a0a 0a2d 205b   Contents**..- [
-00000320: 496e 7374 616c 6c61 7469 6f6e 5d28 2369  Installation](#i
-00000330: 6e73 7461 6c6c 6174 696f 6e29 0a2d 205b  nstallation).- [
-00000340: 5573 6167 655d 2823 7573 6167 6529 0a2d  Usage](#usage).-
-00000350: 205b 4c69 6365 6e73 655d 2823 6c69 6365   [License](#lice
-00000360: 6e73 6529 0a2d 205b 506c 7567 696e 735d  nse).- [Plugins]
-00000370: 2823 706c 7567 696e 7329 0a2d 205b 4368  (#plugins).- [Ch
-00000380: 616e 6765 6c6f 675d 2823 6368 616e 6765  angelog](#change
-00000390: 6c6f 6729 0a0a 2323 2049 6e73 7461 6c6c  log)..## Install
-000003a0: 6174 696f 6e0a 0a60 6060 636f 6e73 6f6c  ation..```consol
-000003b0: 650a 2320 7175 6963 6b20 696e 7374 616c  e.# quick instal
-000003c0: 6c20 7769 7468 2061 6c6c 2070 6f73 7369  l with all possi
-000003d0: 626c 6520 6368 6563 6b65 7273 3a0a 7069  ble checkers:.pi
-000003e0: 7020 696e 7374 616c 6c20 7375 365b 616c  p install su6[al
-000003f0: 6c5d 0a23 206f 7220 7069 636b 2061 6e64  l].# or pick and
-00000400: 2063 686f 6f73 6520 6368 6563 6b65 7273   choose checkers
-00000410: 3a0a 7069 7020 696e 7374 616c 6c20 5b62  :.pip install [b
-00000420: 6c61 636b 2c62 616e 6469 742c 7079 646f  lack,bandit,pydo
-00000430: 6373 7479 6c65 5d0a 6060 600a 0a2a 2a4e  cstyle].```..**N
-00000440: 6f74 652a 2a3a 2074 6869 7320 7061 636b  ote**: this pack
-00000450: 6167 6520 646f 6573 206e 6f74 2077 6f72  age does not wor
-00000460: 6b20 7765 6c6c 2077 6974 6820 6070 6970  k well with `pip
-00000470: 7860 2c20 7369 6e63 6520 6120 6c6f 7420  x`, since a lot 
-00000480: 6f66 2074 6865 2074 6f6f 6c73 206e 6565  of the tools nee
-00000490: 6420 746f 2062 6520 696e 2074 6865 2073  d to be in the s
-000004a0: 616d 6520 2876 6972 7475 616c 290a 656e  ame (virtual).en
-000004b0: 7669 726f 6e6d 656e 740a 6f66 2079 6f75  vironment.of you
-000004c0: 7220 636f 6465 2c20 696e 206f 7264 6572  r code, in order
-000004d0: 2074 6f20 646f 2070 726f 7065 7220 616e   to do proper an
-000004e0: 616c 7973 6973 2e0a 0a54 6865 2066 6f6c  alysis...The fol
-000004f0: 6c6f 7769 6e67 2063 6865 636b 6572 7320  lowing checkers 
-00000500: 6172 6520 7375 7070 6f72 7465 643a 0a0a  are supported:..
-00000510: 2323 2320 7275 6666 0a0a 2d20 696e 7374  ### ruff..- inst
-00000520: 616c 6c3a 2060 7069 7020 696e 7374 616c  all: `pip instal
-00000530: 6c20 7375 365b 7275 6666 5d60 0a2d 2075  l su6[ruff]`.- u
-00000540: 7365 3a20 6073 7536 2072 7566 6620 5b64  se: `su6 ruff [d
-00000550: 6972 6563 746f 7279 5d60 0a2d 2066 756e  irectory]`.- fun
-00000560: 6374 696f 6e61 6c69 7479 3a20 6c69 6e74  ctionality: lint
-00000570: 6572 0a2d 2070 7970 693a 205b 7275 6666  er.- pypi: [ruff
-00000580: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00000590: 7267 2f70 726f 6a65 6374 2f72 7566 662f  rg/project/ruff/
-000005a0: 290a 0a23 2323 2062 6c61 636b 0a0a 2d20  )..### black..- 
-000005b0: 696e 7374 616c 6c3a 2060 7069 7020 696e  install: `pip in
-000005c0: 7374 616c 6c20 7375 365b 626c 6163 6b5d  stall su6[black]
-000005d0: 600a 2d20 7573 653a 2060 7375 3620 626c  `.- use: `su6 bl
-000005e0: 6163 6b20 5b64 6972 6563 746f 7279 5d20  ack [directory] 
-000005f0: 5b2d 2d66 6978 5d60 0a2d 2066 756e 6374  [--fix]`.- funct
-00000600: 696f 6e61 6c69 7479 3a20 666f 726d 6174  ionality: format
-00000610: 7465 720a 2d20 7079 7069 3a20 5b62 6c61  ter.- pypi: [bla
-00000620: 636b 5d28 6874 7470 733a 2f2f 7079 7069  ck](https://pypi
-00000630: 2e6f 7267 2f70 726f 6a65 6374 2f62 6c61  .org/project/bla
-00000640: 636b 2f29 0a0a 2323 2320 6d79 7079 0a0a  ck/)..### mypy..
-00000650: 2d20 696e 7374 616c 6c3a 2060 7069 7020  - install: `pip 
-00000660: 696e 7374 616c 6c20 7375 365b 6d79 7079  install su6[mypy
-00000670: 5d60 0a2d 2075 7365 3a20 6073 7536 206d  ]`.- use: `su6 m
-00000680: 7970 7920 5b64 6972 6563 746f 7279 5d60  ypy [directory]`
-00000690: 0a2d 2066 756e 6374 696f 6e61 6c69 7479  .- functionality
-000006a0: 3a20 7374 6174 6963 2074 7970 6520 6368  : static type ch
-000006b0: 6563 6b65 720a 2d20 7079 7069 3a20 5b6d  ecker.- pypi: [m
-000006c0: 7970 795d 2868 7474 7073 3a2f 2f70 7970  ypy](https://pyp
-000006d0: 692e 6f72 672f 7072 6f6a 6563 742f 6d79  i.org/project/my
-000006e0: 7079 2f29 0a0a 2323 2320 6261 6e64 6974  py/)..### bandit
-000006f0: 0a0a 2d20 696e 7374 616c 6c3a 2060 7069  ..- install: `pi
-00000700: 7020 696e 7374 616c 6c20 7375 365b 6261  p install su6[ba
-00000710: 6e64 6974 5d60 0a2d 2075 7365 3a20 6073  ndit]`.- use: `s
-00000720: 7536 2062 616e 6469 7420 5b64 6972 6563  u6 bandit [direc
-00000730: 746f 7279 5d60 0a2d 2066 756e 6374 696f  tory]`.- functio
-00000740: 6e61 6c69 7479 3a20 7365 6375 7269 7479  nality: security
-00000750: 206c 696e 7465 720a 2d20 7079 7069 3a20   linter.- pypi: 
-00000760: 5b62 616e 6469 745d 2868 7474 7073 3a2f  [bandit](https:/
-00000770: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000780: 742f 6261 6e64 6974 2f29 0a0a 2323 2320  t/bandit/)..### 
-00000790: 6973 6f72 740a 0a2d 2069 6e73 7461 6c6c  isort..- install
-000007a0: 3a20 6070 6970 2069 6e73 7461 6c6c 2073  : `pip install s
-000007b0: 7536 5b69 736f 7274 5d60 0a2d 2075 7365  u6[isort]`.- use
-000007c0: 3a20 6073 7536 2069 736f 7274 205b 6469  : `su6 isort [di
-000007d0: 7265 6374 6f72 795d 205b 2d2d 6669 785d  rectory] [--fix]
-000007e0: 600a 2d20 6675 6e63 7469 6f6e 616c 6974  `.- functionalit
-000007f0: 793a 2069 6d70 6f72 7420 736f 7274 6572  y: import sorter
-00000800: 0a2d 2070 7970 693a 205b 6973 6f72 745d  .- pypi: [isort]
-00000810: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00000820: 672f 7072 6f6a 6563 742f 6973 6f72 742f  g/project/isort/
-00000830: 290a 0a23 2323 2070 7964 6f63 7374 796c  )..### pydocstyl
-00000840: 650a 0a2d 2069 6e73 7461 6c6c 3a20 6070  e..- install: `p
-00000850: 6970 2069 6e73 7461 6c6c 2073 7536 5b70  ip install su6[p
-00000860: 7964 6f63 7374 796c 655d 600a 2d20 7573  ydocstyle]`.- us
-00000870: 653a 2060 7375 3620 7079 646f 6373 7479  e: `su6 pydocsty
-00000880: 6c65 205b 6469 7265 6374 6f72 795d 600a  le [directory]`.
-00000890: 2d20 6675 6e63 7469 6f6e 616c 6974 793a  - functionality:
-000008a0: 2064 6f63 7374 7269 6e67 2063 6865 636b   docstring check
-000008b0: 6572 0a2d 2070 7970 693a 205b 7079 646f  er.- pypi: [pydo
-000008c0: 6373 7479 6c65 5d28 6874 7470 733a 2f2f  cstyle](https://
-000008d0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-000008e0: 2f70 7964 6f63 7374 796c 652f 290a 0a23  /pydocstyle/)..#
-000008f0: 2323 2070 7974 6573 740a 0a2d 2069 6e73  ## pytest..- ins
-00000900: 7461 6c6c 3a20 6070 6970 2069 6e73 7461  tall: `pip insta
-00000910: 6c6c 2073 7536 5b70 7974 6573 745d 600a  ll su6[pytest]`.
-00000920: 2d20 7573 653a 2060 7375 3620 7079 7465  - use: `su6 pyte
-00000930: 7374 205b 6469 7265 6374 6f72 795d 205b  st [directory] [
-00000940: 2d2d 636f 7665 7261 6765 203c 696e 743e  --coverage <int>
-00000950: 5d20 5b2d 2d6a 736f 6e5d 205b 2d2d 6874  ] [--json] [--ht
-00000960: 6d6c 5d20 5b2d 2d62 6164 6765 203c 7061  ml] [--badge <pa
-00000970: 7468 3e5d 600a 2d20 6675 6e63 7469 6f6e  th>]`.- function
-00000980: 616c 6974 793a 2074 6573 7465 7220 7769  ality: tester wi
-00000990: 7468 2063 6f76 6572 6167 650a 2d20 7079  th coverage.- py
-000009a0: 7069 3a20 5b70 7974 6573 745d 2868 7474  pi: [pytest](htt
-000009b0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000009c0: 6f6a 6563 742f 7079 7465 7374 2f29 2c20  oject/pytest/), 
-000009d0: 5b70 7974 6573 742d 636f 765d 2868 7474  [pytest-cov](htt
-000009e0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000009f0: 6f6a 6563 742f 7079 7465 7374 2d63 6f76  oject/pytest-cov
-00000a00: 2f29 0a0a 2323 2055 7361 6765 0a0a 6060  /)..## Usage..``
-00000a10: 6063 6f6e 736f 6c65 0a73 7536 202d 2d68  `console.su6 --h
-00000a20: 656c 700a 2320 6f72 2c20 6561 7369 6573  elp.# or, easies
-00000a30: 7420 746f 2073 7461 7274 3a0a 7375 3620  t to start:.su6 
-00000a40: 616c 6c0a 2320 7573 7561 6c20 7369 676e  all.# usual sign
-00000a50: 6174 7572 653a 0a73 7536 205b 2d2d 7665  ature:.su6 [--ve
-00000a60: 7262 6f73 6974 793d 317c 327c 335d 205b  rbosity=1|2|3] [
-00000a70: 2d2d 636f 6e66 6967 3d2e 2e2e 5d20 5b2d  --config=...] [-
-00000a80: 2d66 6f72 6d61 743d 7465 7874 7c6a 736f  -format=text|jso
-00000a90: 6e5d 203c 7375 6263 6f6d 6d61 6e64 3e20  n] <subcommand> 
-00000aa0: 5b64 6972 6563 746f 7279 5d20 5b2e 2e2e  [directory] [...
-00000ab0: 7370 6563 6966 6963 206f 7074 696f 6e73  specific options
-00000ac0: 5d0a 6060 600a 0a77 6865 7265 2060 7375  ].```..where `su
-00000ad0: 6263 6f6d 6d61 6e64 6020 6973 2060 616c  bcommand` is `al
-00000ae0: 6c60 206f 7220 6f6e 6520 6f66 2074 6865  l` or one of the
-00000af0: 2061 7661 696c 6162 6c65 2063 6865 636b   available check
-00000b00: 6572 733b 2020 0a60 7665 7262 6f73 6974  ers;  .`verbosit
-00000b10: 7960 2069 6e64 6963 6174 6573 2068 6f77  y` indicates how
-00000b20: 206d 7563 6820 696e 666f 726d 6174 696f   much informatio
-00000b30: 6e20 796f 7520 7761 6e74 2074 6f20 7365  n you want to se
-00000b40: 6520 2864 6566 6175 6c74 2069 7320 2732  e (default is '2
-00000b50: 2729 2e20 200a 6063 6f6e 6669 6760 2061  ').  .`config` a
-00000b60: 6c6c 6f77 7320 796f 7520 746f 2073 656c  llows you to sel
-00000b70: 6563 7420 6120 6469 6666 6572 656e 7420  ect a different 
-00000b80: 602e 746f 6d6c 6020 6669 6c65 2028 6465  `.toml` file (de
-00000b90: 6661 756c 7420 6973 2060 7079 7072 6f6a  fault is `pyproj
-00000ba0: 6563 742e 746f 6d6c 6029 2e20 200a 6066  ect.toml`).  .`f
-00000bb0: 6f72 6d61 7460 2061 6c6c 6f77 7320 796f  ormat` allows yo
-00000bc0: 7520 746f 2067 6574 2061 204a 534f 4e20  u to get a JSON 
-00000bd0: 6f75 7470 7574 2069 6e73 7465 6164 206f  output instead o
-00000be0: 6620 7468 6520 7465 7874 7561 6c20 7472  f the textual tr
-00000bf0: 6166 6669 6320 6c69 6768 7473 2028 6465  affic lights (de
-00000c00: 6661 756c 7420 6973 2060 7465 7874 6029  fault is `text`)
-00000c10: 2e20 200a 6064 6972 6563 746f 7279 6020  .  .`directory` 
-00000c20: 6973 2074 6865 206c 6f63 6174 696f 6e20  is the location 
-00000c30: 796f 7520 7761 6e74 2074 6f20 7275 6e20  you want to run 
-00000c40: 7468 6520 7363 616e 7320 2864 6566 6175  the scans (defau
-00000c50: 6c74 2069 7320 6375 7272 656e 7420 6469  lt is current di
-00000c60: 7265 6374 6f72 7929 3b20 200a 496e 2074  rectory);  .In t
-00000c70: 6865 2063 6173 6520 6f66 2060 626c 6163  he case of `blac
-00000c80: 6b60 2061 6e64 2060 6973 6f72 7460 2c20  k` and `isort`, 
-00000c90: 616e 6f74 6865 7220 6f70 7469 6f6e 616c  another optional
-00000ca0: 2070 6172 616d 6574 6572 2060 2d2d 6669   parameter `--fi
-00000cb0: 7860 2063 616e 2062 6520 7061 7373 6564  x` can be passed
-00000cc0: 2e0a 5468 6973 2077 696c 6c20 616c 6c6f  ..This will allo
-00000cd0: 7720 7468 6520 746f 6f6c 7320 746f 2064  w the tools to d
-00000ce0: 6f20 7468 6520 7375 6767 6573 7465 6420  o the suggested 
-00000cf0: 6368 616e 6765 7320 2869 6620 6170 706c  changes (if appl
-00000d00: 6963 6162 6c65 292e 0a52 756e 6e69 6e67  icable)..Running
-00000d10: 2060 7375 3620 6669 7860 2077 696c 6c20   `su6 fix` will 
-00000d20: 7275 6e20 626f 7468 2074 6865 7365 2074  run both these t
-00000d30: 6f6f 6c73 2077 6974 6820 7468 6520 602d  ools with the `-
-00000d40: 2d66 6978 6020 666c 6167 2e20 200a 466f  -fix` flag.  .Fo
-00000d50: 7220 6070 7974 6573 7460 2c20 602d 2d6a  r `pytest`, `--j
-00000d60: 736f 6e60 2c20 602d 2d68 746d 6c60 2c20  son`, `--html`, 
-00000d70: 602d 2d62 6164 6765 203c 7374 723e 6020  `--badge <str>` 
-00000d80: 616e 6420 602d 2d63 6f76 6572 6167 6520  and `--coverage 
-00000d90: 3c69 6e74 3e60 2061 7265 2073 7570 706f  <int>` are suppo
-00000da0: 7274 6564 2e0a 5468 6520 6c61 7474 6572  rted..The latter
-00000db0: 2074 776f 2063 616e 2061 6c73 6f20 6265   two can also be
-00000dc0: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
-00000dd0: 6865 2070 7970 726f 6a65 6374 2e74 6f6d  he pyproject.tom
-00000de0: 6c20 2873 6565 205b 2743 6f6e 6669 6775  l (see ['Configu
-00000df0: 7261 7469 6f6e 275d 2823 636f 6e66 6967  ration'](#config
-00000e00: 7572 6174 696f 6e29 292e 0a54 6865 2066  uration))..The f
-00000e10: 6972 7374 2074 776f 2061 7267 756d 656e  irst two argumen
-00000e20: 7473 2063 616e 2062 6520 7573 6564 2074  ts can be used t
-00000e30: 6f20 636f 6e74 726f 6c20 7468 6520 6f75  o control the ou
-00000e40: 7470 7574 2066 6f72 6d61 7420 6f66 2060  tput format of `
-00000e50: 7079 7465 7374 202d 2d63 6f76 602e 2042  pytest --cov`. B
-00000e60: 6f74 6820 6f70 7469 6f6e 7320 6361 6e20  oth options can 
-00000e70: 6265 2075 7365 6420 6174 2074 6865 2073  be used at the s
-00000e80: 616d 650a 7469 6d65 2e20 5468 6520 602d  ame.time. The `-
-00000e90: 2d63 6f76 6572 6167 6560 2066 6c61 6720  -coverage` flag 
-00000ea0: 6361 6e20 6265 2075 7365 6420 746f 2073  can be used to s
-00000eb0: 6574 2061 2074 6872 6573 686f 6c64 2066  et a threshold f
-00000ec0: 6f72 2063 6f64 6520 636f 7665 7261 6765  or code coverage
-00000ed0: 2025 2e20 4966 2074 6865 2063 6f76 6572   %. If the cover
-00000ee0: 6167 6520 6973 206c 6573 7320 7468 616e  age is less than
-00000ef0: 2074 6869 730a 7468 7265 7368 6f6c 642c   this.threshold,
-00000f00: 2074 6865 2063 6865 636b 2077 696c 6c20   the check will 
-00000f10: 6661 696c 2e0a 4966 2060 6261 6467 6560  fail..If `badge`
-00000f20: 2069 7320 7365 7420 7573 696e 6720 636c   is set using cl
-00000f30: 6920 6f72 2074 6f6d 6c20 636f 6e66 6967  i or toml config
-00000f40: 2c20 6120 5356 4720 6261 6467 6520 7769  , a SVG badge wi
-00000f50: 7468 2074 6865 2063 6f76 6572 6167 6520  th the coverage 
-00000f60: 2520 7769 6c6c 2062 6520 6765 6e65 7261  % will be genera
-00000f70: 7465 642e 0a54 6869 7320 6261 6467 6520  ted..This badge 
-00000f80: 6361 6e20 6265 2075 7365 6420 696e 2066  can be used in f
-00000f90: 6f72 2065 7861 6d70 6c65 2074 6865 2052  or example the R
-00000fa0: 4541 444d 452e 6d64 2e0a 0a23 2323 2043  EADME.md...### C
-00000fb0: 6f6e 6669 6775 7261 7469 6f6e 0a0a 496e  onfiguration..In
-00000fc0: 2079 6f75 7220 6070 7970 726f 6a65 6374   your `pyproject
-00000fd0: 2e74 6f6d 6c60 2c20 796f 7520 6361 6e20  .toml`, you can 
-00000fe0: 6164 6420 6120 605b 746f 6f6c 732e 7375  add a `[tools.su
-00000ff0: 365d 6020 7365 6374 696f 6e20 746f 2063  6]` section to c
-00001000: 6f6e 6669 6775 7265 2073 6f6d 6520 6f66  onfigure some of
-00001010: 2074 6865 2062 6568 6176 696f 7220 6f66   the behavior of
-00001020: 2074 6869 7320 746f 6f6c 732e 0a43 7572   this tools..Cur
-00001030: 7265 6e74 6c79 2c20 7468 6520 666f 6c6c  rently, the foll
-00001040: 6f77 696e 6720 6b65 7973 2061 7265 2073  owing keys are s
-00001050: 7570 706f 7274 6564 3a0a 0a60 6060 746f  upported:..```to
-00001060: 6d6c 0a5b 746f 6f6c 2e73 7536 5d0a 6469  ml.[tool.su6].di
-00001070: 7265 6374 6f72 7920 3d20 222e 2220 2320  rectory = "." # 
-00001080: 7374 7269 6e67 2070 6174 6820 746f 2074  string path to t
-00001090: 6865 2064 6972 6563 746f 7279 206f 6e20  he directory on 
-000010a0: 7768 6963 6820 746f 2072 756e 2061 6c6c  which to run all
-000010b0: 2074 6f6f 6c73 2c20 652e 672e 2027 7372   tools, e.g. 'sr
-000010c0: 6327 0a69 6e63 6c75 6465 203d 205b 5d20  c'.include = [] 
-000010d0: 2320 6c69 7374 206f 6620 6368 6563 6b73  # list of checks
-000010e0: 2074 6f20 7275 6e20 2877 6865 6e20 6361   to run (when ca
-000010f0: 6c6c 696e 6720 6073 7536 2061 6c6c 6029  lling `su6 all`)
-00001100: 2c20 652e 672e 205b 2762 6c61 636b 272c  , e.g. ['black',
-00001110: 2027 6d79 7079 275d 0a65 7863 6c75 6465   'mypy'].exclude
-00001120: 203d 205b 5d20 2320 6c69 7374 206f 6620   = [] # list of 
-00001130: 6368 6563 6b73 2074 6f20 736b 6970 2028  checks to skip (
-00001140: 7768 656e 2063 616c 6c69 6e67 2060 7375  when calling `su
-00001150: 3620 616c 6c60 292c 2065 2e67 2e20 5b27  6 all`), e.g. ['
-00001160: 6261 6e64 6974 275d 0a73 746f 702d 6166  bandit'].stop-af
-00001170: 7465 722d 6669 7273 742d 6661 696c 7572  ter-first-failur
-00001180: 6520 3d20 6661 6c73 6520 2023 2062 6f6f  e = false  # boo
-00001190: 6c20 746f 2069 6e64 6963 6174 6520 7768  l to indicate wh
-000011a0: 6574 6865 7220 746f 2065 7869 7420 2761  ether to exit 'a
-000011b0: 6c6c 2720 6166 7465 7220 6f6e 6520 6661  ll' after one fa
-000011c0: 696c 7572 6520 6f72 2074 6f20 646f 2061  ilure or to do a
-000011d0: 6c6c 2063 6865 636b 730a 636f 7665 7261  ll checks.covera
-000011e0: 6765 203d 2031 3030 2023 2069 6e74 2074  ge = 100 # int t
-000011f0: 6872 6573 686f 6c64 2066 6f72 2070 7974  hreshold for pyt
-00001200: 6573 7420 636f 7665 7261 6765 200a 6261  est coverage .ba
-00001210: 6467 6520 3d20 2263 6f76 6572 6167 652e  dge = "coverage.
-00001220: 7376 6722 2020 2320 7374 7220 7061 7468  svg"  # str path
-00001230: 206f 7220 626f 6f6c 2028 7472 7565 207c   or bool (true |
-00001240: 2066 616c 7365 2920 7768 6574 6865 7220   false) whether 
-00001250: 616e 6420 7768 6572 6520 746f 206f 7574  and where to out
-00001260: 7075 7420 7468 6520 636f 7665 7261 6765  put the coverage
-00001270: 2062 6164 6765 0a60 6060 0a0a 416c 6c20   badge.```..All 
-00001280: 6b65 7973 2061 7265 206f 7074 696f 6e61  keys are optiona
-00001290: 6c2e 204e 6f74 6520 7468 6174 2069 6620  l. Note that if 
-000012a0: 796f 7520 6861 7665 2062 6f74 6820 616e  you have both an
-000012b0: 2060 696e 636c 7564 6560 2061 7320 7765   `include` as we
-000012c0: 6c6c 2061 7320 616e 2060 6578 636c 7564  ll as an `exclud
-000012d0: 6560 2c20 616c 6c20 7468 6520 746f 6f6c  e`, all the tool
-000012e0: 7320 696e 2060 696e 636c 7564 6560 2077  s in `include` w
-000012f0: 696c 6c0a 7275 6e20 616e 6420 6065 7863  ill.run and `exc
-00001300: 6c75 6465 6020 7769 6c6c 2062 6520 6675  lude` will be fu
-00001310: 6c6c 7920 6967 6e6f 7265 642e 2020 0a41  lly ignored.  .A
-00001320: 6464 6974 696f 6e61 6c6c 792c 2074 6865  dditionally, the
-00001330: 206f 7264 6572 2069 6e20 7768 6963 6820   order in which 
-00001340: 7468 6520 6368 6563 6b73 2061 7265 2064  the checks are d
-00001350: 6566 696e 6564 2069 6e20 2769 6e63 6c75  efined in 'inclu
-00001360: 6465 272c 2069 7320 7468 6520 6f72 6465  de', is the orde
-00001370: 7220 696e 2077 6869 6368 2074 6865 7920  r in which they 
-00001380: 7769 6c6c 2072 756e 2028 696e 2060 616c  will run (in `al
-00001390: 6c60 0a61 6e64 2060 6669 7860 290a 0a23  l`.and `fix`)..#
-000013a0: 2323 2047 6974 6875 6220 4163 7469 6f6e  ## Github Action
-000013b0: 0a0a 496e 206f 7264 6572 2074 6f20 7573  ..In order to us
-000013c0: 6520 7468 6973 2063 6865 636b 6572 2077  e this checker w
-000013d0: 6974 6869 6e20 4769 7468 7562 2074 6f20  ithin Github to 
-000013e0: 7275 6e20 6368 6563 6b73 2061 6674 6572  run checks after
-000013f0: 2070 7573 6869 6e67 2c0a 796f 7520 6361   pushing,.you ca
-00001400: 6e20 6164 6420 6120 776f 726b 666c 6f77  n add a workflow
-00001410: 2028 652e 672e 2060 2e67 6974 6875 622f   (e.g. `.github/
-00001420: 776f 726b 666c 6f77 732f 7375 362e 7961  workflows/su6.ya
-00001430: 6d6c 6029 206c 696b 6520 7468 6973 2065  ml`) like this e
-00001440: 7861 6d70 6c65 3a0a 0a60 6060 7961 6d6c  xample:..```yaml
-00001450: 0a6e 616d 653a 2072 756e 2073 7536 2063  .name: run su6 c
-00001460: 6865 636b 730a 6f6e 3a0a 2020 7075 7368  hecks.on:.  push
-00001470: 3a0a 2020 2020 6272 616e 6368 6573 2d69  :.    branches-i
-00001480: 676e 6f72 653a 0a20 2020 2020 202d 206d  gnore:.      - m
-00001490: 6173 7465 720a 6a6f 6273 3a0a 2020 6368  aster.jobs:.  ch
-000014a0: 6563 6b3a 0a20 2020 206e 616d 653a 2043  eck:.    name: C
-000014b0: 6865 636b 2077 6974 6820 6073 7536 2061  heck with `su6 a
-000014c0: 6c6c 600a 2020 2020 7275 6e73 2d6f 6e3a  ll`.    runs-on:
-000014d0: 2075 6275 6e74 752d 6c61 7465 7374 0a20   ubuntu-latest. 
-000014e0: 2020 2073 7465 7073 3a0a 2020 2020 2020     steps:.      
-000014f0: 2d20 7573 6573 3a20 6163 7469 6f6e 732f  - uses: actions/
-00001500: 6368 6563 6b6f 7574 4076 330a 2020 2020  checkout@v3.    
-00001510: 2020 2d20 7573 6573 3a20 6163 7469 6f6e    - uses: action
-00001520: 732f 7365 7475 702d 7079 7468 6f6e 4076  s/setup-python@v
-00001530: 340a 2020 2020 2020 2020 7769 7468 3a0a  4.        with:.
-00001540: 2020 2020 2020 2020 2020 7079 7468 6f6e            python
-00001550: 2d76 6572 7369 6f6e 3a20 2733 2e31 3127  -version: '3.11'
-00001560: 0a20 2020 2020 2020 2020 2063 6163 6865  .          cache
-00001570: 3a20 2770 6970 2720 2320 6361 6368 696e  : 'pip' # cachin
-00001580: 6720 7069 7020 6465 7065 6e64 656e 6369  g pip dependenci
-00001590: 6573 0a20 2020 2020 202d 2072 756e 3a20  es.      - run: 
-000015a0: 7069 7020 696e 7374 616c 6c20 7375 365b  pip install su6[
-000015b0: 616c 6c5d 202e 0a20 2020 2020 202d 2072  all] ..      - r
-000015c0: 756e 3a20 7375 3620 616c 6c0a 6060 600a  un: su6 all.```.
-000015d0: 0a2a 2a4e 6f74 653a 2a2a 2069 6620 796f  .**Note:** if yo
-000015e0: 7520 646f 6e27 7420 7761 6e74 2074 6f20  u don't want to 
-000015f0: 7275 6e20 616c 6c20 6368 6563 6b73 2c20  run all checks, 
-00001600: 6275 7420 7370 6563 6966 6963 206f 6e65  but specific one
-00001610: 7320 6f6e 6c79 2c20 796f 7520 6e65 6564  s only, you need
-00001620: 2074 6f20 6164 6420 7468 6520 602d 2d69   to add the `--i
-00001630: 676e 6f72 652d 756e 696e 7374 616c 6c65  gnore-uninstalle
-00001640: 6460 2066 6c61 670a 746f 2060 7375 3620  d` flag.to `su6 
-00001650: 616c 6c60 2120 4f74 6865 7277 6973 652c  all`! Otherwise,
-00001660: 2047 6974 6875 6220 7769 6c6c 2073 6565   Github will see
-00001670: 2065 7869 7420 636f 6465 2031 3237 2028   exit code 127 (
-00001680: 636f 6d6d 616e 6420 6d69 7373 696e 6729  command missing)
-00001690: 2061 7320 6120 6661 696c 7572 652e 0a0a   as a failure...
-000016a0: 6060 6079 616d 6c0a 6e61 6d65 3a20 7275  ```yaml.name: ru
-000016b0: 6e20 736f 6d65 2073 7536 2063 6865 636b  n some su6 check
-000016c0: 730a 6f6e 3a0a 2020 7075 7368 3a0a 2020  s.on:.  push:.  
-000016d0: 2020 6272 616e 6368 6573 2d69 676e 6f72    branches-ignor
-000016e0: 653a 0a20 2020 2020 202d 206d 6173 7465  e:.      - maste
-000016f0: 720a 6a6f 6273 3a0a 2020 6368 6563 6b3a  r.jobs:.  check:
-00001700: 0a20 2020 206e 616d 653a 2043 6865 636b  .    name: Check
-00001710: 2077 6974 6820 6073 7536 2061 6c6c 600a   with `su6 all`.
-00001720: 2020 2020 7275 6e73 2d6f 6e3a 2075 6275      runs-on: ubu
-00001730: 6e74 752d 6c61 7465 7374 0a20 2020 2073  ntu-latest.    s
-00001740: 7465 7073 3a0a 2020 2020 2020 2d20 7573  teps:.      - us
-00001750: 6573 3a20 6163 7469 6f6e 732f 6368 6563  es: actions/chec
-00001760: 6b6f 7574 4076 330a 2020 2020 2020 2d20  kout@v3.      - 
-00001770: 7573 6573 3a20 6163 7469 6f6e 732f 7365  uses: actions/se
-00001780: 7475 702d 7079 7468 6f6e 4076 340a 2020  tup-python@v4.  
-00001790: 2020 2020 2020 7769 7468 3a0a 2020 2020        with:.    
-000017a0: 2020 2020 2020 7079 7468 6f6e 2d76 6572        python-ver
-000017b0: 7369 6f6e 3a20 2733 2e31 3127 0a20 2020  sion: '3.11'.   
-000017c0: 2020 2020 2020 2063 6163 6865 3a20 2770         cache: 'p
-000017d0: 6970 2720 2320 6361 6368 696e 6720 7069  ip' # caching pi
-000017e0: 7020 6465 7065 6e64 656e 6369 6573 0a20  p dependencies. 
-000017f0: 2020 2020 202d 2072 756e 3a20 7069 7020       - run: pip 
-00001800: 696e 7374 616c 6c20 7375 365b 7079 636f  install su6[pyco
-00001810: 6465 7374 796c 652c 626c 6163 6b5d 202e  destyle,black] .
-00001820: 0a20 2020 2020 202d 2072 756e 3a20 7375  .      - run: su
-00001830: 3620 616c 6c20 2d2d 6967 6e6f 7265 2d75  6 all --ignore-u
-00001840: 6e69 6e73 7461 6c6c 6564 2020 2320 2e2e  ninstalled  # ..
-00001850: 2e20 6f74 6865 7220 7365 7474 696e 6773  . other settings
-00001860: 2073 7563 6820 6173 202d 2d73 746f 702d   such as --stop-
-00001870: 6166 7465 722d 6669 7273 742d 6661 696c  after-first-fail
-00001880: 7572 652c 202d 2d63 6f76 6572 6167 6520  ure, --coverage 
-00001890: 2e2e 2e0a 6060 600a 0a23 2320 506c 7567  ....```..## Plug
-000018a0: 696e 730a 5468 6973 2074 6f6f 6c20 616c  ins.This tool al
-000018b0: 736f 2073 7570 706f 7274 7320 706c 7567  so supports plug
-000018c0: 696e 7320 746f 2061 6464 2065 7874 7261  ins to add extra
-000018d0: 2063 6865 636b 6572 7320 6f72 206f 7468   checkers or oth
-000018e0: 6572 2066 756e 6374 696f 6e61 6c69 7479  er functionality
-000018f0: 2e20 5365 6520 5b64 6f63 732f 706c 7567  . See [docs/plug
-00001900: 696e 732e 6d64 5d28 6874 7470 733a 2f2f  ins.md](https://
-00001910: 6769 7468 7562 2e63 6f6d 2f72 6f62 696e  github.com/robin
-00001920: 7661 6e64 6572 6e6f 6f72 642f 7375 362d  vandernoord/su6-
-00001930: 6368 6563 6b65 722f 626c 6f62 2f6d 6173  checker/blob/mas
-00001940: 7465 722f 646f 6373 2f70 6c75 6769 6e73  ter/docs/plugins
-00001950: 2e6d 6429 0a0a 2323 204c 6963 656e 7365  .md)..## License
-00001960: 0a0a 6073 7536 6020 6973 2064 6973 7472  ..`su6` is distr
-00001970: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-00001980: 2074 6572 6d73 206f 6620 7468 6520 5b4d   terms of the [M
-00001990: 4954 5d28 6874 7470 733a 2f2f 7370 6478  IT](https://spdx
-000019a0: 2e6f 7267 2f6c 6963 656e 7365 732f 4d49  .org/licenses/MI
-000019b0: 542e 6874 6d6c 2920 6c69 6365 6e73 652e  T.html) license.
-000019c0: 0a0a 2323 2043 6861 6e67 656c 6f67 0a0a  ..## Changelog..
-000019d0: 5365 6520 6043 4841 4e47 454c 4f47 2e6d  See `CHANGELOG.m
-000019e0: 6460 205b 6f6e 2047 6974 4875 625d 2868  d` [on GitHub](h
-000019f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001a00: 6d2f 726f 6269 6e76 616e 6465 726e 6f6f  m/robinvandernoo
-00001a10: 7264 2f73 7536 2d63 6865 636b 6572 2f62  rd/su6-checker/b
-00001a20: 6c6f 622f 6d61 7374 6572 2f43 4841 4e47  lob/master/CHANG
-00001a30: 454c 4f47 2e6d 6429 0a                   ELOG.md).
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 2020 203c 696d 6720 0a20  er">.    <img . 
+00000020: 2020 2020 2020 2061 6c69 676e 3d22 6365         align="ce
+00000030: 6e74 6572 2220 0a20 2020 2020 2020 2073  nter" .        s
+00000040: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00000050: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000060: 742e 636f 6d2f 726f 6269 6e76 616e 6465  t.com/robinvande
+00000070: 726e 6f6f 7264 2f73 7536 2d63 6865 636b  rnoord/su6-check
+00000080: 6572 2f6d 6173 7465 722f 5f73 7461 7469  er/master/_stati
+00000090: 632f 7375 362e 7376 6722 200a 2020 2020  c/su6.svg" .    
+000000a0: 2020 2020 616c 743d 2273 7536 2063 6865      alt="su6 che
+000000b0: 636b 6572 220a 2020 2020 2020 2020 7769  cker".        wi
+000000c0: 6474 683d 2234 3030 7078 220a 2020 2020  dth="400px".    
+000000d0: 2020 2020 2f3e 0a20 2020 203c 6831 2061      />.    <h1 a
+000000e0: 6c69 676e 3d22 6365 6e74 6572 223e 7375  lign="center">su
+000000f0: 363c 2f68 313e 0a3c 2f64 6976 3e0a 0a3c  6</h1>.</div>..<
+00000100: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000110: 7222 3e0a 2020 2020 3620 6973 2070 726f  r">.    6 is pro
+00000120: 6e6f 756e 6365 6420 6173 2027 2f7a c99b  nounced as '/z..
+00000130: 732f 2720 696e 2044 7574 6368 2c20 736f  s/' in Dutch, so
+00000140: 2027 7375 3627 2069 7320 6261 7369 6361   'su6' is basica
+00000150: 6c6c 7920 2773 7563 6365 7373 272e 203c  lly 'success'. <
+00000160: 6272 202f 3e0a 2020 2020 5468 6973 2070  br />.    This p
+00000170: 6163 6b61 6765 2077 696c 6c20 686f 7065  ackage will hope
+00000180: 6675 6c6c 7920 6865 6c70 2061 6368 6965  fully help achie
+00000190: 7665 2074 6861 7421 0a3c 2f64 6976 3e0a  ve that!.</div>.
+000001a0: 0a3c 6272 3e0a 0a3c 6469 7620 616c 6967  .<br>..<div alig
+000001b0: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+000001c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000001d0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000001e0: 742f 7375 3622 3e3c 696d 6720 616c 743d  t/su6"><img alt=
+000001f0: 2250 7950 4920 2d20 5665 7273 696f 6e22  "PyPI - Version"
+00000200: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000210: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000220: 692f 762f 7375 362e 7376 6722 2f3e 3c2f  i/v/su6.svg"/></
+00000230: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000240: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000250: 2f70 726f 6a65 6374 2f73 7536 223e 3c69  /project/su6"><i
+00000260: 6d67 2061 6c74 3d22 5079 5049 202d 2050  mg alt="PyPI - P
+00000270: 7974 686f 6e20 5665 7273 696f 6e22 2073  ython Version" s
+00000280: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000290: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000002a0: 7079 7665 7273 696f 6e73 2f73 7536 2e73  pyversions/su6.s
+000002b0: 7667 222f 3e3c 2f61 3e0a 2020 2020 3c62  vg"/></a>.    <b
+000002c0: 722f 3e0a 2020 2020 3c61 2068 7265 663d  r/>.    <a href=
+000002d0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000002e0: 636f 6d2f 7073 662f 626c 6163 6b22 3e3c  com/psf/black"><
+000002f0: 696d 6720 616c 743d 2243 6f64 6520 7374  img alt="Code st
+00000300: 796c 653a 2062 6c61 636b 2220 7372 633d  yle: black" src=
+00000310: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000320: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
+00000330: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
+00000340: 2d30 3030 3030 302e 7376 6722 2f3e 3c2f  -000000.svg"/></
+00000350: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000360: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000370: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+00000380: 4d49 5422 3e3c 696d 6720 616c 743d 224c  MIT"><img alt="L
+00000390: 6963 656e 7365 3a20 4d49 5422 2073 7263  icense: MIT" src
+000003a0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000003b0: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+000003c0: 6963 656e 7365 2d4d 4954 2d79 656c 6c6f  icense-MIT-yello
+000003d0: 772e 7376 6722 2f3e 3c2f 613e 0a20 2020  w.svg"/></a>.   
+000003e0: 203c 6272 2f3e 0a20 2020 203c 6120 6872   <br/>.    <a hr
+000003f0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000400: 7562 2e63 6f6d 2f72 6f62 696e 7661 6e64  ub.com/robinvand
+00000410: 6572 6e6f 6f72 642f 7375 362d 6368 6563  ernoord/su6-chec
+00000420: 6b65 722f 6163 7469 6f6e 7322 3e3c 696d  ker/actions"><im
+00000430: 6720 616c 743d 2273 7536 2063 6865 636b  g alt="su6 check
+00000440: 7322 2073 7263 3d22 6874 7470 733a 2f2f  s" src="https://
+00000450: 6769 7468 7562 2e63 6f6d 2f72 6f62 696e  github.com/robin
+00000460: 7661 6e64 6572 6e6f 6f72 642f 7375 362d  vandernoord/su6-
+00000470: 6368 6563 6b65 722f 6163 7469 6f6e 732f  checker/actions/
+00000480: 776f 726b 666c 6f77 732f 7375 362e 796d  workflows/su6.ym
+00000490: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
+000004a0: 6368 3d64 6576 656c 6f70 6d65 6e74 222f  ch=development"/
+000004b0: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
+000004c0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000004d0: 622e 636f 6d2f 726f 6269 6e76 616e 6465  b.com/robinvande
+000004e0: 726e 6f6f 7264 2f73 7536 2d63 6865 636b  rnoord/su6-check
+000004f0: 6572 2f61 6374 696f 6e73 223e 3c69 6d67  er/actions"><img
+00000500: 2061 6c74 3d22 436f 7665 7261 6765 2220   alt="Coverage" 
+00000510: 7372 633d 2263 6f76 6572 6167 652e 7376  src="coverage.sv
+00000520: 6722 2f3e 3c2f 613e 0a3c 2f64 6976 3e0a  g"/></a>.</div>.
+00000530: 0a2d 2d2d 2d2d 0a0a 2a2a 5461 626c 6520  .-----..**Table 
+00000540: 6f66 2043 6f6e 7465 6e74 732a 2a0a 0a2d  of Contents**..-
+00000550: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
+00000560: 2369 6e73 7461 6c6c 6174 696f 6e29 0a2d  #installation).-
+00000570: 205b 5573 6167 655d 2823 7573 6167 6529   [Usage](#usage)
+00000580: 0a2d 205b 4c69 6365 6e73 655d 2823 6c69  .- [License](#li
+00000590: 6365 6e73 6529 0a2d 205b 506c 7567 696e  cense).- [Plugin
+000005a0: 735d 2823 706c 7567 696e 7329 0a2d 205b  s](#plugins).- [
+000005b0: 4368 616e 6765 6c6f 675d 2823 6368 616e  Changelog](#chan
+000005c0: 6765 6c6f 6729 0a0a 2323 2049 6e73 7461  gelog)..## Insta
+000005d0: 6c6c 6174 696f 6e0a 0a60 6060 636f 6e73  llation..```cons
+000005e0: 6f6c 650a 2320 7175 6963 6b20 696e 7374  ole.# quick inst
+000005f0: 616c 6c20 7769 7468 2061 6c6c 2070 6f73  all with all pos
+00000600: 7369 626c 6520 6368 6563 6b65 7273 3a0a  sible checkers:.
+00000610: 7069 7020 696e 7374 616c 6c20 7375 365b  pip install su6[
+00000620: 616c 6c5d 0a23 206f 7220 7069 636b 2061  all].# or pick a
+00000630: 6e64 2063 686f 6f73 6520 6368 6563 6b65  nd choose checke
+00000640: 7273 3a0a 7069 7020 696e 7374 616c 6c20  rs:.pip install 
+00000650: 5b62 6c61 636b 2c62 616e 6469 742c 7079  [black,bandit,py
+00000660: 646f 6373 7479 6c65 5d0a 6060 600a 0a2a  docstyle].```..*
+00000670: 2a4e 6f74 652a 2a3a 2074 6869 7320 7061  *Note**: this pa
+00000680: 636b 6167 6520 646f 6573 206e 6f74 2077  ckage does not w
+00000690: 6f72 6b20 7765 6c6c 2077 6974 6820 6070  ork well with `p
+000006a0: 6970 7860 2c20 7369 6e63 6520 6120 6c6f  ipx`, since a lo
+000006b0: 7420 6f66 2074 6865 2074 6f6f 6c73 206e  t of the tools n
+000006c0: 6565 6420 746f 2062 6520 696e 2074 6865  eed to be in the
+000006d0: 2073 616d 6520 2876 6972 7475 616c 290a   same (virtual).
+000006e0: 656e 7669 726f 6e6d 656e 740a 6f66 2079  environment.of y
+000006f0: 6f75 7220 636f 6465 2c20 696e 206f 7264  our code, in ord
+00000700: 6572 2074 6f20 646f 2070 726f 7065 7220  er to do proper 
+00000710: 616e 616c 7973 6973 2e0a 0a54 6865 2066  analysis...The f
+00000720: 6f6c 6c6f 7769 6e67 2063 6865 636b 6572  ollowing checker
+00000730: 7320 6172 6520 7375 7070 6f72 7465 643a  s are supported:
+00000740: 0a0a 2323 2320 7275 6666 0a0a 2d20 696e  ..### ruff..- in
+00000750: 7374 616c 6c3a 2060 7069 7020 696e 7374  stall: `pip inst
+00000760: 616c 6c20 7375 365b 7275 6666 5d60 0a2d  all su6[ruff]`.-
+00000770: 2075 7365 3a20 6073 7536 2072 7566 6620   use: `su6 ruff 
+00000780: 5b64 6972 6563 746f 7279 5d60 0a2d 2066  [directory]`.- f
+00000790: 756e 6374 696f 6e61 6c69 7479 3a20 6c69  unctionality: li
+000007a0: 6e74 6572 0a2d 2070 7970 693a 205b 7275  nter.- pypi: [ru
+000007b0: 6666 5d28 6874 7470 733a 2f2f 7079 7069  ff](https://pypi
+000007c0: 2e6f 7267 2f70 726f 6a65 6374 2f72 7566  .org/project/ruf
+000007d0: 662f 290a 0a23 2323 2062 6c61 636b 0a0a  f/)..### black..
+000007e0: 2d20 696e 7374 616c 6c3a 2060 7069 7020  - install: `pip 
+000007f0: 696e 7374 616c 6c20 7375 365b 626c 6163  install su6[blac
+00000800: 6b5d 600a 2d20 7573 653a 2060 7375 3620  k]`.- use: `su6 
+00000810: 626c 6163 6b20 5b64 6972 6563 746f 7279  black [directory
+00000820: 5d20 5b2d 2d66 6978 5d60 0a2d 2066 756e  ] [--fix]`.- fun
+00000830: 6374 696f 6e61 6c69 7479 3a20 666f 726d  ctionality: form
+00000840: 6174 7465 720a 2d20 7079 7069 3a20 5b62  atter.- pypi: [b
+00000850: 6c61 636b 5d28 6874 7470 733a 2f2f 7079  lack](https://py
+00000860: 7069 2e6f 7267 2f70 726f 6a65 6374 2f62  pi.org/project/b
+00000870: 6c61 636b 2f29 0a0a 2323 2320 6d79 7079  lack/)..### mypy
+00000880: 0a0a 2d20 696e 7374 616c 6c3a 2060 7069  ..- install: `pi
+00000890: 7020 696e 7374 616c 6c20 7375 365b 6d79  p install su6[my
+000008a0: 7079 5d60 0a2d 2075 7365 3a20 6073 7536  py]`.- use: `su6
+000008b0: 206d 7970 7920 5b64 6972 6563 746f 7279   mypy [directory
+000008c0: 5d60 0a2d 2066 756e 6374 696f 6e61 6c69  ]`.- functionali
+000008d0: 7479 3a20 7374 6174 6963 2074 7970 6520  ty: static type 
+000008e0: 6368 6563 6b65 720a 2d20 7079 7069 3a20  checker.- pypi: 
+000008f0: 5b6d 7970 795d 2868 7474 7073 3a2f 2f70  [mypy](https://p
+00000900: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000910: 6d79 7079 2f29 0a0a 2323 2320 6261 6e64  mypy/)..### band
+00000920: 6974 0a0a 2d20 696e 7374 616c 6c3a 2060  it..- install: `
+00000930: 7069 7020 696e 7374 616c 6c20 7375 365b  pip install su6[
+00000940: 6261 6e64 6974 5d60 0a2d 2075 7365 3a20  bandit]`.- use: 
+00000950: 6073 7536 2062 616e 6469 7420 5b64 6972  `su6 bandit [dir
+00000960: 6563 746f 7279 5d60 0a2d 2066 756e 6374  ectory]`.- funct
+00000970: 696f 6e61 6c69 7479 3a20 7365 6375 7269  ionality: securi
+00000980: 7479 206c 696e 7465 720a 2d20 7079 7069  ty linter.- pypi
+00000990: 3a20 5b62 616e 6469 745d 2868 7474 7073  : [bandit](https
+000009a0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000009b0: 6563 742f 6261 6e64 6974 2f29 0a0a 2323  ect/bandit/)..##
+000009c0: 2320 6973 6f72 740a 0a2d 2069 6e73 7461  # isort..- insta
+000009d0: 6c6c 3a20 6070 6970 2069 6e73 7461 6c6c  ll: `pip install
+000009e0: 2073 7536 5b69 736f 7274 5d60 0a2d 2075   su6[isort]`.- u
+000009f0: 7365 3a20 6073 7536 2069 736f 7274 205b  se: `su6 isort [
+00000a00: 6469 7265 6374 6f72 795d 205b 2d2d 6669  directory] [--fi
+00000a10: 785d 600a 2d20 6675 6e63 7469 6f6e 616c  x]`.- functional
+00000a20: 6974 793a 2069 6d70 6f72 7420 736f 7274  ity: import sort
+00000a30: 6572 0a2d 2070 7970 693a 205b 6973 6f72  er.- pypi: [isor
+00000a40: 745d 2868 7474 7073 3a2f 2f70 7970 692e  t](https://pypi.
+00000a50: 6f72 672f 7072 6f6a 6563 742f 6973 6f72  org/project/isor
+00000a60: 742f 290a 0a23 2323 2070 7964 6f63 7374  t/)..### pydocst
+00000a70: 796c 650a 0a2d 2069 6e73 7461 6c6c 3a20  yle..- install: 
+00000a80: 6070 6970 2069 6e73 7461 6c6c 2073 7536  `pip install su6
+00000a90: 5b70 7964 6f63 7374 796c 655d 600a 2d20  [pydocstyle]`.- 
+00000aa0: 7573 653a 2060 7375 3620 7079 646f 6373  use: `su6 pydocs
+00000ab0: 7479 6c65 205b 6469 7265 6374 6f72 795d  tyle [directory]
+00000ac0: 600a 2d20 6675 6e63 7469 6f6e 616c 6974  `.- functionalit
+00000ad0: 793a 2064 6f63 7374 7269 6e67 2063 6865  y: docstring che
+00000ae0: 636b 6572 0a2d 2070 7970 693a 205b 7079  cker.- pypi: [py
+00000af0: 646f 6373 7479 6c65 5d28 6874 7470 733a  docstyle](https:
+00000b00: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000b10: 6374 2f70 7964 6f63 7374 796c 652f 290a  ct/pydocstyle/).
+00000b20: 0a23 2323 2070 7974 6573 740a 0a2d 2069  .### pytest..- i
+00000b30: 6e73 7461 6c6c 3a20 6070 6970 2069 6e73  nstall: `pip ins
+00000b40: 7461 6c6c 2073 7536 5b70 7974 6573 745d  tall su6[pytest]
+00000b50: 600a 2d20 7573 653a 2060 7375 3620 7079  `.- use: `su6 py
+00000b60: 7465 7374 205b 6469 7265 6374 6f72 795d  test [directory]
+00000b70: 205b 2d2d 636f 7665 7261 6765 203c 696e   [--coverage <in
+00000b80: 743e 5d20 5b2d 2d6a 736f 6e5d 205b 2d2d  t>] [--json] [--
+00000b90: 6874 6d6c 5d20 5b2d 2d62 6164 6765 203c  html] [--badge <
+00000ba0: 7061 7468 3e5d 600a 2d20 6675 6e63 7469  path>]`.- functi
+00000bb0: 6f6e 616c 6974 793a 2074 6573 7465 7220  onality: tester 
+00000bc0: 7769 7468 2063 6f76 6572 6167 650a 2d20  with coverage.- 
+00000bd0: 7079 7069 3a20 5b70 7974 6573 745d 2868  pypi: [pytest](h
+00000be0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000bf0: 7072 6f6a 6563 742f 7079 7465 7374 2f29  project/pytest/)
+00000c00: 2c20 5b70 7974 6573 742d 636f 765d 2868  , [pytest-cov](h
+00000c10: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000c20: 7072 6f6a 6563 742f 7079 7465 7374 2d63  project/pytest-c
+00000c30: 6f76 2f29 0a0a 2323 2055 7361 6765 0a0a  ov/)..## Usage..
+00000c40: 6060 6063 6f6e 736f 6c65 0a73 7536 202d  ```console.su6 -
+00000c50: 2d68 656c 700a 2320 6f72 2c20 6561 7369  -help.# or, easi
+00000c60: 6573 7420 746f 2073 7461 7274 3a0a 7375  est to start:.su
+00000c70: 3620 616c 6c0a 2320 7573 7561 6c20 7369  6 all.# usual si
+00000c80: 676e 6174 7572 653a 0a73 7536 205b 2d2d  gnature:.su6 [--
+00000c90: 7665 7262 6f73 6974 793d 317c 327c 335d  verbosity=1|2|3]
+00000ca0: 205b 2d2d 636f 6e66 6967 3d2e 2e2e 5d20   [--config=...] 
+00000cb0: 5b2d 2d66 6f72 6d61 743d 7465 7874 7c6a  [--format=text|j
+00000cc0: 736f 6e5d 203c 7375 6263 6f6d 6d61 6e64  son] <subcommand
+00000cd0: 3e20 5b64 6972 6563 746f 7279 5d20 5b2e  > [directory] [.
+00000ce0: 2e2e 7370 6563 6966 6963 206f 7074 696f  ..specific optio
+00000cf0: 6e73 5d0a 6060 600a 0a77 6865 7265 2060  ns].```..where `
+00000d00: 7375 6263 6f6d 6d61 6e64 6020 6973 2060  subcommand` is `
+00000d10: 616c 6c60 206f 7220 6f6e 6520 6f66 2074  all` or one of t
+00000d20: 6865 2061 7661 696c 6162 6c65 2063 6865  he available che
+00000d30: 636b 6572 733b 2020 0a60 7665 7262 6f73  ckers;  .`verbos
+00000d40: 6974 7960 2069 6e64 6963 6174 6573 2068  ity` indicates h
+00000d50: 6f77 206d 7563 6820 696e 666f 726d 6174  ow much informat
+00000d60: 696f 6e20 796f 7520 7761 6e74 2074 6f20  ion you want to 
+00000d70: 7365 6520 2864 6566 6175 6c74 2069 7320  see (default is 
+00000d80: 2732 2729 2e20 200a 6063 6f6e 6669 6760  '2').  .`config`
+00000d90: 2061 6c6c 6f77 7320 796f 7520 746f 2073   allows you to s
+00000da0: 656c 6563 7420 6120 6469 6666 6572 656e  elect a differen
+00000db0: 7420 602e 746f 6d6c 6020 6669 6c65 2028  t `.toml` file (
+00000dc0: 6465 6661 756c 7420 6973 2060 7079 7072  default is `pypr
+00000dd0: 6f6a 6563 742e 746f 6d6c 6029 2e20 200a  oject.toml`).  .
+00000de0: 6066 6f72 6d61 7460 2061 6c6c 6f77 7320  `format` allows 
+00000df0: 796f 7520 746f 2067 6574 2061 204a 534f  you to get a JSO
+00000e00: 4e20 6f75 7470 7574 2069 6e73 7465 6164  N output instead
+00000e10: 206f 6620 7468 6520 7465 7874 7561 6c20   of the textual 
+00000e20: 7472 6166 6669 6320 6c69 6768 7473 2028  traffic lights (
+00000e30: 6465 6661 756c 7420 6973 2060 7465 7874  default is `text
+00000e40: 6029 2e20 200a 6064 6972 6563 746f 7279  `).  .`directory
+00000e50: 6020 6973 2074 6865 206c 6f63 6174 696f  ` is the locatio
+00000e60: 6e20 796f 7520 7761 6e74 2074 6f20 7275  n you want to ru
+00000e70: 6e20 7468 6520 7363 616e 7320 2864 6566  n the scans (def
+00000e80: 6175 6c74 2069 7320 6375 7272 656e 7420  ault is current 
+00000e90: 6469 7265 6374 6f72 7929 3b20 200a 496e  directory);  .In
+00000ea0: 2074 6865 2063 6173 6520 6f66 2060 626c   the case of `bl
+00000eb0: 6163 6b60 2061 6e64 2060 6973 6f72 7460  ack` and `isort`
+00000ec0: 2c20 616e 6f74 6865 7220 6f70 7469 6f6e  , another option
+00000ed0: 616c 2070 6172 616d 6574 6572 2060 2d2d  al parameter `--
+00000ee0: 6669 7860 2063 616e 2062 6520 7061 7373  fix` can be pass
+00000ef0: 6564 2e0a 5468 6973 2077 696c 6c20 616c  ed..This will al
+00000f00: 6c6f 7720 7468 6520 746f 6f6c 7320 746f  low the tools to
+00000f10: 2064 6f20 7468 6520 7375 6767 6573 7465   do the suggeste
+00000f20: 6420 6368 616e 6765 7320 2869 6620 6170  d changes (if ap
+00000f30: 706c 6963 6162 6c65 292e 0a52 756e 6e69  plicable)..Runni
+00000f40: 6e67 2060 7375 3620 6669 7860 2077 696c  ng `su6 fix` wil
+00000f50: 6c20 7275 6e20 626f 7468 2074 6865 7365  l run both these
+00000f60: 2074 6f6f 6c73 2077 6974 6820 7468 6520   tools with the 
+00000f70: 602d 2d66 6978 6020 666c 6167 2e20 200a  `--fix` flag.  .
+00000f80: 466f 7220 6070 7974 6573 7460 2c20 602d  For `pytest`, `-
+00000f90: 2d6a 736f 6e60 2c20 602d 2d68 746d 6c60  -json`, `--html`
+00000fa0: 2c20 602d 2d62 6164 6765 203c 7374 723e  , `--badge <str>
+00000fb0: 6020 616e 6420 602d 2d63 6f76 6572 6167  ` and `--coverag
+00000fc0: 6520 3c69 6e74 3e60 2061 7265 2073 7570  e <int>` are sup
+00000fd0: 706f 7274 6564 2e0a 5468 6520 6c61 7474  ported..The latt
+00000fe0: 6572 2074 776f 2063 616e 2061 6c73 6f20  er two can also 
+00000ff0: 6265 2063 6f6e 6669 6775 7265 6420 696e  be configured in
+00001000: 2074 6865 2070 7970 726f 6a65 6374 2e74   the pyproject.t
+00001010: 6f6d 6c20 2873 6565 205b 2743 6f6e 6669  oml (see ['Confi
+00001020: 6775 7261 7469 6f6e 275d 2823 636f 6e66  guration'](#conf
+00001030: 6967 7572 6174 696f 6e29 292e 0a54 6865  iguration))..The
+00001040: 2066 6972 7374 2074 776f 2061 7267 756d   first two argum
+00001050: 656e 7473 2063 616e 2062 6520 7573 6564  ents can be used
+00001060: 2074 6f20 636f 6e74 726f 6c20 7468 6520   to control the 
+00001070: 6f75 7470 7574 2066 6f72 6d61 7420 6f66  output format of
+00001080: 2060 7079 7465 7374 202d 2d63 6f76 602e   `pytest --cov`.
+00001090: 2042 6f74 6820 6f70 7469 6f6e 7320 6361   Both options ca
+000010a0: 6e20 6265 2075 7365 6420 6174 2074 6865  n be used at the
+000010b0: 2073 616d 650a 7469 6d65 2e20 5468 6520   same.time. The 
+000010c0: 602d 2d63 6f76 6572 6167 6560 2066 6c61  `--coverage` fla
+000010d0: 6720 6361 6e20 6265 2075 7365 6420 746f  g can be used to
+000010e0: 2073 6574 2061 2074 6872 6573 686f 6c64   set a threshold
+000010f0: 2066 6f72 2063 6f64 6520 636f 7665 7261   for code covera
+00001100: 6765 2025 2e20 4966 2074 6865 2063 6f76  ge %. If the cov
+00001110: 6572 6167 6520 6973 206c 6573 7320 7468  erage is less th
+00001120: 616e 2074 6869 730a 7468 7265 7368 6f6c  an this.threshol
+00001130: 642c 2074 6865 2063 6865 636b 2077 696c  d, the check wil
+00001140: 6c20 6661 696c 2e0a 4966 2060 6261 6467  l fail..If `badg
+00001150: 6560 2069 7320 7365 7420 7573 696e 6720  e` is set using 
+00001160: 636c 6920 6f72 2074 6f6d 6c20 636f 6e66  cli or toml conf
+00001170: 6967 2c20 6120 5356 4720 6261 6467 6520  ig, a SVG badge 
+00001180: 7769 7468 2074 6865 2063 6f76 6572 6167  with the coverag
+00001190: 6520 2520 7769 6c6c 2062 6520 6765 6e65  e % will be gene
+000011a0: 7261 7465 642e 0a54 6869 7320 6261 6467  rated..This badg
+000011b0: 6520 6361 6e20 6265 2075 7365 6420 696e  e can be used in
+000011c0: 2066 6f72 2065 7861 6d70 6c65 2074 6865   for example the
+000011d0: 2052 4541 444d 452e 6d64 2e0a 0a23 2323   README.md...###
+000011e0: 2043 6f6e 6669 6775 7261 7469 6f6e 0a0a   Configuration..
+000011f0: 496e 2079 6f75 7220 6070 7970 726f 6a65  In your `pyproje
+00001200: 6374 2e74 6f6d 6c60 2c20 796f 7520 6361  ct.toml`, you ca
+00001210: 6e20 6164 6420 6120 605b 746f 6f6c 732e  n add a `[tools.
+00001220: 7375 365d 6020 7365 6374 696f 6e20 746f  su6]` section to
+00001230: 2063 6f6e 6669 6775 7265 2073 6f6d 6520   configure some 
+00001240: 6f66 2074 6865 2062 6568 6176 696f 7220  of the behavior 
+00001250: 6f66 2074 6869 7320 746f 6f6c 732e 0a43  of this tools..C
+00001260: 7572 7265 6e74 6c79 2c20 7468 6520 666f  urrently, the fo
+00001270: 6c6c 6f77 696e 6720 6b65 7973 2061 7265  llowing keys are
+00001280: 2073 7570 706f 7274 6564 3a0a 0a60 6060   supported:..```
+00001290: 746f 6d6c 0a5b 746f 6f6c 2e73 7536 5d0a  toml.[tool.su6].
+000012a0: 6469 7265 6374 6f72 7920 3d20 222e 2220  directory = "." 
+000012b0: 2320 7374 7269 6e67 2070 6174 6820 746f  # string path to
+000012c0: 2074 6865 2064 6972 6563 746f 7279 206f   the directory o
+000012d0: 6e20 7768 6963 6820 746f 2072 756e 2061  n which to run a
+000012e0: 6c6c 2074 6f6f 6c73 2c20 652e 672e 2027  ll tools, e.g. '
+000012f0: 7372 6327 0a69 6e63 6c75 6465 203d 205b  src'.include = [
+00001300: 5d20 2320 6c69 7374 206f 6620 6368 6563  ] # list of chec
+00001310: 6b73 2074 6f20 7275 6e20 2877 6865 6e20  ks to run (when 
+00001320: 6361 6c6c 696e 6720 6073 7536 2061 6c6c  calling `su6 all
+00001330: 6029 2c20 652e 672e 205b 2762 6c61 636b  `), e.g. ['black
+00001340: 272c 2027 6d79 7079 275d 0a65 7863 6c75  ', 'mypy'].exclu
+00001350: 6465 203d 205b 5d20 2320 6c69 7374 206f  de = [] # list o
+00001360: 6620 6368 6563 6b73 2074 6f20 736b 6970  f checks to skip
+00001370: 2028 7768 656e 2063 616c 6c69 6e67 2060   (when calling `
+00001380: 7375 3620 616c 6c60 292c 2065 2e67 2e20  su6 all`), e.g. 
+00001390: 5b27 6261 6e64 6974 275d 0a73 746f 702d  ['bandit'].stop-
+000013a0: 6166 7465 722d 6669 7273 742d 6661 696c  after-first-fail
+000013b0: 7572 6520 3d20 6661 6c73 6520 2023 2062  ure = false  # b
+000013c0: 6f6f 6c20 746f 2069 6e64 6963 6174 6520  ool to indicate 
+000013d0: 7768 6574 6865 7220 746f 2065 7869 7420  whether to exit 
+000013e0: 2761 6c6c 2720 6166 7465 7220 6f6e 6520  'all' after one 
+000013f0: 6661 696c 7572 6520 6f72 2074 6f20 646f  failure or to do
+00001400: 2061 6c6c 2063 6865 636b 730a 636f 7665   all checks.cove
+00001410: 7261 6765 203d 2031 3030 2023 2069 6e74  rage = 100 # int
+00001420: 2074 6872 6573 686f 6c64 2066 6f72 2070   threshold for p
+00001430: 7974 6573 7420 636f 7665 7261 6765 200a  ytest coverage .
+00001440: 6261 6467 6520 3d20 2263 6f76 6572 6167  badge = "coverag
+00001450: 652e 7376 6722 2020 2320 7374 7220 7061  e.svg"  # str pa
+00001460: 7468 206f 7220 626f 6f6c 2028 7472 7565  th or bool (true
+00001470: 207c 2066 616c 7365 2920 7768 6574 6865   | false) whethe
+00001480: 7220 616e 6420 7768 6572 6520 746f 206f  r and where to o
+00001490: 7574 7075 7420 7468 6520 636f 7665 7261  utput the covera
+000014a0: 6765 2062 6164 6765 0a60 6060 0a0a 416c  ge badge.```..Al
+000014b0: 6c20 6b65 7973 2061 7265 206f 7074 696f  l keys are optio
+000014c0: 6e61 6c2e 204e 6f74 6520 7468 6174 2069  nal. Note that i
+000014d0: 6620 796f 7520 6861 7665 2062 6f74 6820  f you have both 
+000014e0: 616e 2060 696e 636c 7564 6560 2061 7320  an `include` as 
+000014f0: 7765 6c6c 2061 7320 616e 2060 6578 636c  well as an `excl
+00001500: 7564 6560 2c20 616c 6c20 7468 6520 746f  ude`, all the to
+00001510: 6f6c 7320 696e 2060 696e 636c 7564 6560  ols in `include`
+00001520: 2077 696c 6c0a 7275 6e20 616e 6420 6065   will.run and `e
+00001530: 7863 6c75 6465 6020 7769 6c6c 2062 6520  xclude` will be 
+00001540: 6675 6c6c 7920 6967 6e6f 7265 642e 2020  fully ignored.  
+00001550: 0a41 6464 6974 696f 6e61 6c6c 792c 2074  .Additionally, t
+00001560: 6865 206f 7264 6572 2069 6e20 7768 6963  he order in whic
+00001570: 6820 7468 6520 6368 6563 6b73 2061 7265  h the checks are
+00001580: 2064 6566 696e 6564 2069 6e20 2769 6e63   defined in 'inc
+00001590: 6c75 6465 272c 2069 7320 7468 6520 6f72  lude', is the or
+000015a0: 6465 7220 696e 2077 6869 6368 2074 6865  der in which the
+000015b0: 7920 7769 6c6c 2072 756e 2028 696e 2060  y will run (in `
+000015c0: 616c 6c60 0a61 6e64 2060 6669 7860 290a  all`.and `fix`).
+000015d0: 0a23 2323 2047 6974 6875 6220 4163 7469  .### Github Acti
+000015e0: 6f6e 0a0a 496e 206f 7264 6572 2074 6f20  on..In order to 
+000015f0: 7573 6520 7468 6973 2063 6865 636b 6572  use this checker
+00001600: 2077 6974 6869 6e20 4769 7468 7562 2074   within Github t
+00001610: 6f20 7275 6e20 6368 6563 6b73 2061 6674  o run checks aft
+00001620: 6572 2070 7573 6869 6e67 2c0a 796f 7520  er pushing,.you 
+00001630: 6361 6e20 6164 6420 6120 776f 726b 666c  can add a workfl
+00001640: 6f77 2028 652e 672e 2060 2e67 6974 6875  ow (e.g. `.githu
+00001650: 622f 776f 726b 666c 6f77 732f 7375 362e  b/workflows/su6.
+00001660: 7961 6d6c 6029 206c 696b 6520 7468 6973  yaml`) like this
+00001670: 2065 7861 6d70 6c65 3a0a 0a60 6060 7961   example:..```ya
+00001680: 6d6c 0a6e 616d 653a 2072 756e 2073 7536  ml.name: run su6
+00001690: 2063 6865 636b 730a 6f6e 3a0a 2020 7075   checks.on:.  pu
+000016a0: 7368 3a0a 2020 2020 6272 616e 6368 6573  sh:.    branches
+000016b0: 2d69 676e 6f72 653a 0a20 2020 2020 202d  -ignore:.      -
+000016c0: 206d 6173 7465 720a 6a6f 6273 3a0a 2020   master.jobs:.  
+000016d0: 6368 6563 6b3a 0a20 2020 206e 616d 653a  check:.    name:
+000016e0: 2043 6865 636b 2077 6974 6820 6073 7536   Check with `su6
+000016f0: 2061 6c6c 600a 2020 2020 7275 6e73 2d6f   all`.    runs-o
+00001700: 6e3a 2075 6275 6e74 752d 6c61 7465 7374  n: ubuntu-latest
+00001710: 0a20 2020 2073 7465 7073 3a0a 2020 2020  .    steps:.    
+00001720: 2020 2d20 7573 6573 3a20 6163 7469 6f6e    - uses: action
+00001730: 732f 6368 6563 6b6f 7574 4076 330a 2020  s/checkout@v3.  
+00001740: 2020 2020 2d20 7573 6573 3a20 6163 7469      - uses: acti
+00001750: 6f6e 732f 7365 7475 702d 7079 7468 6f6e  ons/setup-python
+00001760: 4076 340a 2020 2020 2020 2020 7769 7468  @v4.        with
+00001770: 3a0a 2020 2020 2020 2020 2020 7079 7468  :.          pyth
+00001780: 6f6e 2d76 6572 7369 6f6e 3a20 2733 2e31  on-version: '3.1
+00001790: 3127 0a20 2020 2020 2020 2020 2063 6163  1'.          cac
+000017a0: 6865 3a20 2770 6970 2720 2320 6361 6368  he: 'pip' # cach
+000017b0: 696e 6720 7069 7020 6465 7065 6e64 656e  ing pip dependen
+000017c0: 6369 6573 0a20 2020 2020 202d 2072 756e  cies.      - run
+000017d0: 3a20 7069 7020 696e 7374 616c 6c20 7375  : pip install su
+000017e0: 365b 616c 6c5d 202e 0a20 2020 2020 202d  6[all] ..      -
+000017f0: 2072 756e 3a20 7375 3620 616c 6c0a 6060   run: su6 all.``
+00001800: 600a 0a2a 2a4e 6f74 653a 2a2a 2069 6620  `..**Note:** if 
+00001810: 796f 7520 646f 6e27 7420 7761 6e74 2074  you don't want t
+00001820: 6f20 7275 6e20 616c 6c20 6368 6563 6b73  o run all checks
+00001830: 2c20 6275 7420 7370 6563 6966 6963 206f  , but specific o
+00001840: 6e65 7320 6f6e 6c79 2c20 796f 7520 6e65  nes only, you ne
+00001850: 6564 2074 6f20 6164 6420 7468 6520 602d  ed to add the `-
+00001860: 2d69 676e 6f72 652d 756e 696e 7374 616c  -ignore-uninstal
+00001870: 6c65 6460 2066 6c61 670a 746f 2060 7375  led` flag.to `su
+00001880: 3620 616c 6c60 2120 4f74 6865 7277 6973  6 all`! Otherwis
+00001890: 652c 2047 6974 6875 6220 7769 6c6c 2073  e, Github will s
+000018a0: 6565 2065 7869 7420 636f 6465 2031 3237  ee exit code 127
+000018b0: 2028 636f 6d6d 616e 6420 6d69 7373 696e   (command missin
+000018c0: 6729 2061 7320 6120 6661 696c 7572 652e  g) as a failure.
+000018d0: 0a0a 6060 6079 616d 6c0a 6e61 6d65 3a20  ..```yaml.name: 
+000018e0: 7275 6e20 736f 6d65 2073 7536 2063 6865  run some su6 che
+000018f0: 636b 730a 6f6e 3a0a 2020 7075 7368 3a0a  cks.on:.  push:.
+00001900: 2020 2020 6272 616e 6368 6573 2d69 676e      branches-ign
+00001910: 6f72 653a 0a20 2020 2020 202d 206d 6173  ore:.      - mas
+00001920: 7465 720a 6a6f 6273 3a0a 2020 6368 6563  ter.jobs:.  chec
+00001930: 6b3a 0a20 2020 206e 616d 653a 2043 6865  k:.    name: Che
+00001940: 636b 2077 6974 6820 6073 7536 2061 6c6c  ck with `su6 all
+00001950: 600a 2020 2020 7275 6e73 2d6f 6e3a 2075  `.    runs-on: u
+00001960: 6275 6e74 752d 6c61 7465 7374 0a20 2020  buntu-latest.   
+00001970: 2073 7465 7073 3a0a 2020 2020 2020 2d20   steps:.      - 
+00001980: 7573 6573 3a20 6163 7469 6f6e 732f 6368  uses: actions/ch
+00001990: 6563 6b6f 7574 4076 330a 2020 2020 2020  eckout@v3.      
+000019a0: 2d20 7573 6573 3a20 6163 7469 6f6e 732f  - uses: actions/
+000019b0: 7365 7475 702d 7079 7468 6f6e 4076 340a  setup-python@v4.
+000019c0: 2020 2020 2020 2020 7769 7468 3a0a 2020          with:.  
+000019d0: 2020 2020 2020 2020 7079 7468 6f6e 2d76          python-v
+000019e0: 6572 7369 6f6e 3a20 2733 2e31 3127 0a20  ersion: '3.11'. 
+000019f0: 2020 2020 2020 2020 2063 6163 6865 3a20           cache: 
+00001a00: 2770 6970 2720 2320 6361 6368 696e 6720  'pip' # caching 
+00001a10: 7069 7020 6465 7065 6e64 656e 6369 6573  pip dependencies
+00001a20: 0a20 2020 2020 202d 2072 756e 3a20 7069  .      - run: pi
+00001a30: 7020 696e 7374 616c 6c20 7375 365b 7079  p install su6[py
+00001a40: 636f 6465 7374 796c 652c 626c 6163 6b5d  codestyle,black]
+00001a50: 202e 0a20 2020 2020 202d 2072 756e 3a20   ..      - run: 
+00001a60: 7375 3620 616c 6c20 2d2d 6967 6e6f 7265  su6 all --ignore
+00001a70: 2d75 6e69 6e73 7461 6c6c 6564 2020 2320  -uninstalled  # 
+00001a80: 2e2e 2e20 6f74 6865 7220 7365 7474 696e  ... other settin
+00001a90: 6773 2073 7563 6820 6173 202d 2d73 746f  gs such as --sto
+00001aa0: 702d 6166 7465 722d 6669 7273 742d 6661  p-after-first-fa
+00001ab0: 696c 7572 652c 202d 2d63 6f76 6572 6167  ilure, --coverag
+00001ac0: 6520 2e2e 2e0a 6060 600a 0a23 2320 506c  e ....```..## Pl
+00001ad0: 7567 696e 730a 0a54 6869 7320 746f 6f6c  ugins..This tool
+00001ae0: 2061 6c73 6f20 7375 7070 6f72 7473 2070   also supports p
+00001af0: 6c75 6769 6e73 2074 6f20 6164 6420 6578  lugins to add ex
+00001b00: 7472 6120 6368 6563 6b65 7273 206f 7220  tra checkers or 
+00001b10: 6f74 6865 7220 6675 6e63 7469 6f6e 616c  other functional
+00001b20: 6974 792e 0a53 6565 205b 646f 6373 2f70  ity..See [docs/p
+00001b30: 6c75 6769 6e73 2e6d 645d 2868 7474 7073  lugins.md](https
+00001b40: 3a2f 2f67 6974 6875 622e 636f 6d2f 726f  ://github.com/ro
+00001b50: 6269 6e76 616e 6465 726e 6f6f 7264 2f73  binvandernoord/s
+00001b60: 7536 2d63 6865 636b 6572 2f62 6c6f 622f  u6-checker/blob/
+00001b70: 6d61 7374 6572 2f64 6f63 732f 706c 7567  master/docs/plug
+00001b80: 696e 732e 6d64 290a 0a23 2320 4c69 6365  ins.md)..## Lice
+00001b90: 6e73 650a 0a60 7375 3660 2069 7320 6469  nse..`su6` is di
+00001ba0: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00001bb0: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
+00001bc0: 205b 4d49 545d 2868 7474 7073 3a2f 2f73   [MIT](https://s
+00001bd0: 7064 782e 6f72 672f 6c69 6365 6e73 6573  pdx.org/licenses
+00001be0: 2f4d 4954 2e68 746d 6c29 206c 6963 656e  /MIT.html) licen
+00001bf0: 7365 2e0a 0a23 2320 4368 616e 6765 6c6f  se...## Changelo
+00001c00: 670a 0a53 6565 2060 4348 414e 4745 4c4f  g..See `CHANGELO
+00001c10: 472e 6d64 6020 5b6f 6e20 4769 7448 7562  G.md` [on GitHub
+00001c20: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001c30: 2e63 6f6d 2f72 6f62 696e 7661 6e64 6572  .com/robinvander
+00001c40: 6e6f 6f72 642f 7375 362d 6368 6563 6b65  noord/su6-checke
+00001c50: 722f 626c 6f62 2f6d 6173 7465 722f 4348  r/blob/master/CH
+00001c60: 414e 4745 4c4f 472e 6d64 290a            ANGELOG.md).
```

### Comparing `su6-1.4.1/pyproject.toml` & `su6-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `su6-1.4.1/PKG-INFO` & `su6-1.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7375 360a  : 2.1.Name: su6.
-00000020: 5665 7273 696f 6e3a 2031 2e34 2e31 0a53  Version: 1.4.1.S
+00000020: 5665 7273 696f 6e3a 2031 2e34 2e32 0a53  Version: 1.4.2.S
 00000030: 756d 6d61 7279 3a20 5079 7468 6f6e 2063  ummary: Python c
 00000040: 6c69 2074 6f6f 6c20 746f 2075 7365 2074  li tool to use t
 00000050: 6f6f 6c73 2066 6f72 2073 6f6d 6520 636f  ools for some co
 00000060: 6d6d 6f6e 2063 6f64 6520 7175 616c 6974  mmon code qualit
 00000070: 7920 6368 6563 6b73 2028 6f70 696e 696f  y checks (opinio
 00000080: 6e61 7465 6429 0a50 726f 6a65 6374 2d55  nated).Project-U
 00000090: 524c 3a20 446f 6375 6d65 6e74 6174 696f  RL: Documentatio
@@ -121,428 +121,463 @@
 00000780: 6f76 3b20 6578 7472 6120 3d3d 2027 7079  ov; extra == 'py
 00000790: 7465 7374 270a 5072 6f76 6964 6573 2d45  test'.Provides-E
 000007a0: 7874 7261 3a20 7275 6666 0a52 6571 7569  xtra: ruff.Requi
 000007b0: 7265 732d 4469 7374 3a20 7275 6666 3b20  res-Dist: ruff; 
 000007c0: 6578 7472 6120 3d3d 2027 7275 6666 270a  extra == 'ruff'.
 000007d0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 000007e0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-000007f0: 6172 6b64 6f77 6e0a 0a23 2073 7536 2d63  arkdown..# su6-c
-00000800: 6865 636b 6572 0a0a 5b21 5b50 7950 4920  hecker..[![PyPI 
-00000810: 2d20 5665 7273 696f 6e5d 2868 7474 7073  - Version](https
-00000820: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000830: 6f2f 7079 7069 2f76 2f73 7536 2e73 7667  o/pypi/v/su6.svg
-00000840: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000850: 6f72 672f 7072 6f6a 6563 742f 7375 3629  org/project/su6)
-00000860: 0a5b 215b 5079 5049 202d 2050 7974 686f  .[![PyPI - Pytho
-00000870: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
-00000880: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000890: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-000008a0: 732f 7375 362e 7376 6729 5d28 6874 7470  s/su6.svg)](http
-000008b0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000008c0: 6a65 6374 2f73 7536 2920 200a 5b21 5b43  ject/su6)  .[![C
-000008d0: 6f64 6520 7374 796c 653a 2062 6c61 636b  ode style: black
-000008e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000008f0: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
-00000900: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
-00000910: 6b2d 3030 3030 3030 2e73 7667 295d 2868  k-000000.svg)](h
-00000920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000930: 6d2f 7073 662f 626c 6163 6b29 0a5b 215b  m/psf/black).[![
-00000940: 4c69 6365 6e73 653a 204d 4954 5d28 6874  License: MIT](ht
-00000950: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000960: 732e 696f 2f62 6164 6765 2f4c 6963 656e  s.io/badge/Licen
-00000970: 7365 2d4d 4954 2d79 656c 6c6f 772e 7376  se-MIT-yellow.sv
-00000980: 6729 5d28 6874 7470 733a 2f2f 6f70 656e  g)](https://open
-00000990: 736f 7572 6365 2e6f 7267 2f6c 6963 656e  source.org/licen
-000009a0: 7365 732f 4d49 5429 2020 0a5b 215b 7375  ses/MIT)  .[![su
-000009b0: 3620 6368 6563 6b73 5d28 6874 7470 733a  6 checks](https:
-000009c0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6f62  //github.com/rob
-000009d0: 696e 7661 6e64 6572 6e6f 6f72 642f 7375  invandernoord/su
-000009e0: 362d 6368 6563 6b65 722f 6163 7469 6f6e  6-checker/action
-000009f0: 732f 776f 726b 666c 6f77 732f 7375 362e  s/workflows/su6.
-00000a00: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
-00000a10: 616e 6368 3d64 6576 656c 6f70 6d65 6e74  anch=development
-00000a20: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000a30: 622e 636f 6d2f 726f 6269 6e76 616e 6465  b.com/robinvande
-00000a40: 726e 6f6f 7264 2f73 7536 2d63 6865 636b  rnoord/su6-check
-00000a50: 6572 2f61 6374 696f 6e73 290a 215b 636f  er/actions).![co
-00000a60: 7665 7261 6765 2e73 7667 5d28 636f 7665  verage.svg](cove
-00000a70: 7261 6765 2e73 7667 290a 0a2d 2d2d 2d2d  rage.svg)..-----
-00000a80: 0a73 7536 2028 3620 6973 2070 726f 6e6f  .su6 (6 is prono
-00000a90: 756e 6365 6420 6173 2027 2f7a c99b 732f  unced as '/z..s/
-00000aa0: 2720 696e 2044 7574 6368 2c20 736f 2027  ' in Dutch, so '
-00000ab0: 7375 3627 2069 7320 6261 7369 6361 6c6c  su6' is basicall
-00000ac0: 7920 2773 7563 6365 7373 2729 2020 0a54  y 'success')  .T
-00000ad0: 6869 7320 7061 636b 6167 6520 7769 6c6c  his package will
-00000ae0: 2068 6f70 6566 756c 6c79 2068 656c 7020   hopefully help 
-00000af0: 6163 6869 6576 6520 7468 6174 210a 0a2a  achieve that!..*
-00000b00: 2a54 6162 6c65 206f 6620 436f 6e74 656e  *Table of Conten
-00000b10: 7473 2a2a 0a0a 2d20 5b49 6e73 7461 6c6c  ts**..- [Install
-00000b20: 6174 696f 6e5d 2823 696e 7374 616c 6c61  ation](#installa
-00000b30: 7469 6f6e 290a 2d20 5b55 7361 6765 5d28  tion).- [Usage](
-00000b40: 2375 7361 6765 290a 2d20 5b4c 6963 656e  #usage).- [Licen
-00000b50: 7365 5d28 236c 6963 656e 7365 290a 2d20  se](#license).- 
-00000b60: 5b50 6c75 6769 6e73 5d28 2370 6c75 6769  [Plugins](#plugi
-00000b70: 6e73 290a 2d20 5b43 6861 6e67 656c 6f67  ns).- [Changelog
-00000b80: 5d28 2363 6861 6e67 656c 6f67 290a 0a23  ](#changelog)..#
-00000b90: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000ba0: 6060 6063 6f6e 736f 6c65 0a23 2071 7569  ```console.# qui
-00000bb0: 636b 2069 6e73 7461 6c6c 2077 6974 6820  ck install with 
-00000bc0: 616c 6c20 706f 7373 6962 6c65 2063 6865  all possible che
-00000bd0: 636b 6572 733a 0a70 6970 2069 6e73 7461  ckers:.pip insta
-00000be0: 6c6c 2073 7536 5b61 6c6c 5d0a 2320 6f72  ll su6[all].# or
-00000bf0: 2070 6963 6b20 616e 6420 6368 6f6f 7365   pick and choose
-00000c00: 2063 6865 636b 6572 733a 0a70 6970 2069   checkers:.pip i
-00000c10: 6e73 7461 6c6c 205b 626c 6163 6b2c 6261  nstall [black,ba
-00000c20: 6e64 6974 2c70 7964 6f63 7374 796c 655d  ndit,pydocstyle]
-00000c30: 0a60 6060 0a0a 2a2a 4e6f 7465 2a2a 3a20  .```..**Note**: 
-00000c40: 7468 6973 2070 6163 6b61 6765 2064 6f65  this package doe
-00000c50: 7320 6e6f 7420 776f 726b 2077 656c 6c20  s not work well 
-00000c60: 7769 7468 2060 7069 7078 602c 2073 696e  with `pipx`, sin
-00000c70: 6365 2061 206c 6f74 206f 6620 7468 6520  ce a lot of the 
-00000c80: 746f 6f6c 7320 6e65 6564 2074 6f20 6265  tools need to be
-00000c90: 2069 6e20 7468 6520 7361 6d65 2028 7669   in the same (vi
-00000ca0: 7274 7561 6c29 0a65 6e76 6972 6f6e 6d65  rtual).environme
-00000cb0: 6e74 0a6f 6620 796f 7572 2063 6f64 652c  nt.of your code,
-00000cc0: 2069 6e20 6f72 6465 7220 746f 2064 6f20   in order to do 
-00000cd0: 7072 6f70 6572 2061 6e61 6c79 7369 732e  proper analysis.
-00000ce0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-00000cf0: 6368 6563 6b65 7273 2061 7265 2073 7570  checkers are sup
-00000d00: 706f 7274 6564 3a0a 0a23 2323 2072 7566  ported:..### ruf
-00000d10: 660a 0a2d 2069 6e73 7461 6c6c 3a20 6070  f..- install: `p
-00000d20: 6970 2069 6e73 7461 6c6c 2073 7536 5b72  ip install su6[r
-00000d30: 7566 665d 600a 2d20 7573 653a 2060 7375  uff]`.- use: `su
-00000d40: 3620 7275 6666 205b 6469 7265 6374 6f72  6 ruff [director
-00000d50: 795d 600a 2d20 6675 6e63 7469 6f6e 616c  y]`.- functional
-00000d60: 6974 793a 206c 696e 7465 720a 2d20 7079  ity: linter.- py
-00000d70: 7069 3a20 5b72 7566 665d 2868 7474 7073  pi: [ruff](https
-00000d80: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000d90: 6563 742f 7275 6666 2f29 0a0a 2323 2320  ect/ruff/)..### 
-00000da0: 626c 6163 6b0a 0a2d 2069 6e73 7461 6c6c  black..- install
-00000db0: 3a20 6070 6970 2069 6e73 7461 6c6c 2073  : `pip install s
-00000dc0: 7536 5b62 6c61 636b 5d60 0a2d 2075 7365  u6[black]`.- use
-00000dd0: 3a20 6073 7536 2062 6c61 636b 205b 6469  : `su6 black [di
-00000de0: 7265 6374 6f72 795d 205b 2d2d 6669 785d  rectory] [--fix]
-00000df0: 600a 2d20 6675 6e63 7469 6f6e 616c 6974  `.- functionalit
-00000e00: 793a 2066 6f72 6d61 7474 6572 0a2d 2070  y: formatter.- p
-00000e10: 7970 693a 205b 626c 6163 6b5d 2868 7474  ypi: [black](htt
-00000e20: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000e30: 6f6a 6563 742f 626c 6163 6b2f 290a 0a23  oject/black/)..#
-00000e40: 2323 206d 7970 790a 0a2d 2069 6e73 7461  ## mypy..- insta
-00000e50: 6c6c 3a20 6070 6970 2069 6e73 7461 6c6c  ll: `pip install
-00000e60: 2073 7536 5b6d 7970 795d 600a 2d20 7573   su6[mypy]`.- us
-00000e70: 653a 2060 7375 3620 6d79 7079 205b 6469  e: `su6 mypy [di
-00000e80: 7265 6374 6f72 795d 600a 2d20 6675 6e63  rectory]`.- func
-00000e90: 7469 6f6e 616c 6974 793a 2073 7461 7469  tionality: stati
-00000ea0: 6320 7479 7065 2063 6865 636b 6572 0a2d  c type checker.-
-00000eb0: 2070 7970 693a 205b 6d79 7079 5d28 6874   pypi: [mypy](ht
-00000ec0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000ed0: 726f 6a65 6374 2f6d 7970 792f 290a 0a23  roject/mypy/)..#
-00000ee0: 2323 2062 616e 6469 740a 0a2d 2069 6e73  ## bandit..- ins
-00000ef0: 7461 6c6c 3a20 6070 6970 2069 6e73 7461  tall: `pip insta
-00000f00: 6c6c 2073 7536 5b62 616e 6469 745d 600a  ll su6[bandit]`.
-00000f10: 2d20 7573 653a 2060 7375 3620 6261 6e64  - use: `su6 band
-00000f20: 6974 205b 6469 7265 6374 6f72 795d 600a  it [directory]`.
-00000f30: 2d20 6675 6e63 7469 6f6e 616c 6974 793a  - functionality:
-00000f40: 2073 6563 7572 6974 7920 6c69 6e74 6572   security linter
-00000f50: 0a2d 2070 7970 693a 205b 6261 6e64 6974  .- pypi: [bandit
-00000f60: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00000f70: 7267 2f70 726f 6a65 6374 2f62 616e 6469  rg/project/bandi
-00000f80: 742f 290a 0a23 2323 2069 736f 7274 0a0a  t/)..### isort..
-00000f90: 2d20 696e 7374 616c 6c3a 2060 7069 7020  - install: `pip 
-00000fa0: 696e 7374 616c 6c20 7375 365b 6973 6f72  install su6[isor
-00000fb0: 745d 600a 2d20 7573 653a 2060 7375 3620  t]`.- use: `su6 
-00000fc0: 6973 6f72 7420 5b64 6972 6563 746f 7279  isort [directory
-00000fd0: 5d20 5b2d 2d66 6978 5d60 0a2d 2066 756e  ] [--fix]`.- fun
-00000fe0: 6374 696f 6e61 6c69 7479 3a20 696d 706f  ctionality: impo
-00000ff0: 7274 2073 6f72 7465 720a 2d20 7079 7069  rt sorter.- pypi
-00001000: 3a20 5b69 736f 7274 5d28 6874 7470 733a  : [isort](https:
-00001010: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00001020: 6374 2f69 736f 7274 2f29 0a0a 2323 2320  ct/isort/)..### 
-00001030: 7079 646f 6373 7479 6c65 0a0a 2d20 696e  pydocstyle..- in
-00001040: 7374 616c 6c3a 2060 7069 7020 696e 7374  stall: `pip inst
-00001050: 616c 6c20 7375 365b 7079 646f 6373 7479  all su6[pydocsty
-00001060: 6c65 5d60 0a2d 2075 7365 3a20 6073 7536  le]`.- use: `su6
-00001070: 2070 7964 6f63 7374 796c 6520 5b64 6972   pydocstyle [dir
-00001080: 6563 746f 7279 5d60 0a2d 2066 756e 6374  ectory]`.- funct
-00001090: 696f 6e61 6c69 7479 3a20 646f 6373 7472  ionality: docstr
-000010a0: 696e 6720 6368 6563 6b65 720a 2d20 7079  ing checker.- py
-000010b0: 7069 3a20 5b70 7964 6f63 7374 796c 655d  pi: [pydocstyle]
-000010c0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-000010d0: 672f 7072 6f6a 6563 742f 7079 646f 6373  g/project/pydocs
-000010e0: 7479 6c65 2f29 0a0a 2323 2320 7079 7465  tyle/)..### pyte
-000010f0: 7374 0a0a 2d20 696e 7374 616c 6c3a 2060  st..- install: `
-00001100: 7069 7020 696e 7374 616c 6c20 7375 365b  pip install su6[
-00001110: 7079 7465 7374 5d60 0a2d 2075 7365 3a20  pytest]`.- use: 
-00001120: 6073 7536 2070 7974 6573 7420 5b64 6972  `su6 pytest [dir
-00001130: 6563 746f 7279 5d20 5b2d 2d63 6f76 6572  ectory] [--cover
-00001140: 6167 6520 3c69 6e74 3e5d 205b 2d2d 6a73  age <int>] [--js
-00001150: 6f6e 5d20 5b2d 2d68 746d 6c5d 205b 2d2d  on] [--html] [--
-00001160: 6261 6467 6520 3c70 6174 683e 5d60 0a2d  badge <path>]`.-
-00001170: 2066 756e 6374 696f 6e61 6c69 7479 3a20   functionality: 
-00001180: 7465 7374 6572 2077 6974 6820 636f 7665  tester with cove
-00001190: 7261 6765 0a2d 2070 7970 693a 205b 7079  rage.- pypi: [py
-000011a0: 7465 7374 5d28 6874 7470 733a 2f2f 7079  test](https://py
-000011b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
-000011c0: 7974 6573 742f 292c 205b 7079 7465 7374  ytest/), [pytest
-000011d0: 2d63 6f76 5d28 6874 7470 733a 2f2f 7079  -cov](https://py
-000011e0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
-000011f0: 7974 6573 742d 636f 762f 290a 0a23 2320  ytest-cov/)..## 
-00001200: 5573 6167 650a 0a60 6060 636f 6e73 6f6c  Usage..```consol
-00001210: 650a 7375 3620 2d2d 6865 6c70 0a23 206f  e.su6 --help.# o
-00001220: 722c 2065 6173 6965 7374 2074 6f20 7374  r, easiest to st
-00001230: 6172 743a 0a73 7536 2061 6c6c 0a23 2075  art:.su6 all.# u
-00001240: 7375 616c 2073 6967 6e61 7475 7265 3a0a  sual signature:.
-00001250: 7375 3620 5b2d 2d76 6572 626f 7369 7479  su6 [--verbosity
-00001260: 3d31 7c32 7c33 5d20 5b2d 2d63 6f6e 6669  =1|2|3] [--confi
-00001270: 673d 2e2e 2e5d 205b 2d2d 666f 726d 6174  g=...] [--format
-00001280: 3d74 6578 747c 6a73 6f6e 5d20 3c73 7562  =text|json] <sub
-00001290: 636f 6d6d 616e 643e 205b 6469 7265 6374  command> [direct
-000012a0: 6f72 795d 205b 2e2e 2e73 7065 6369 6669  ory] [...specifi
-000012b0: 6320 6f70 7469 6f6e 735d 0a60 6060 0a0a  c options].```..
-000012c0: 7768 6572 6520 6073 7562 636f 6d6d 616e  where `subcomman
-000012d0: 6460 2069 7320 6061 6c6c 6020 6f72 206f  d` is `all` or o
-000012e0: 6e65 206f 6620 7468 6520 6176 6169 6c61  ne of the availa
-000012f0: 626c 6520 6368 6563 6b65 7273 3b20 200a  ble checkers;  .
-00001300: 6076 6572 626f 7369 7479 6020 696e 6469  `verbosity` indi
-00001310: 6361 7465 7320 686f 7720 6d75 6368 2069  cates how much i
-00001320: 6e66 6f72 6d61 7469 6f6e 2079 6f75 2077  nformation you w
-00001330: 616e 7420 746f 2073 6565 2028 6465 6661  ant to see (defa
-00001340: 756c 7420 6973 2027 3227 292e 2020 0a60  ult is '2').  .`
-00001350: 636f 6e66 6967 6020 616c 6c6f 7773 2079  config` allows y
-00001360: 6f75 2074 6f20 7365 6c65 6374 2061 2064  ou to select a d
-00001370: 6966 6665 7265 6e74 2060 2e74 6f6d 6c60  ifferent `.toml`
-00001380: 2066 696c 6520 2864 6566 6175 6c74 2069   file (default i
-00001390: 7320 6070 7970 726f 6a65 6374 2e74 6f6d  s `pyproject.tom
-000013a0: 6c60 292e 2020 0a60 666f 726d 6174 6020  l`).  .`format` 
-000013b0: 616c 6c6f 7773 2079 6f75 2074 6f20 6765  allows you to ge
-000013c0: 7420 6120 4a53 4f4e 206f 7574 7075 7420  t a JSON output 
-000013d0: 696e 7374 6561 6420 6f66 2074 6865 2074  instead of the t
-000013e0: 6578 7475 616c 2074 7261 6666 6963 206c  extual traffic l
-000013f0: 6967 6874 7320 2864 6566 6175 6c74 2069  ights (default i
-00001400: 7320 6074 6578 7460 292e 2020 0a60 6469  s `text`).  .`di
-00001410: 7265 6374 6f72 7960 2069 7320 7468 6520  rectory` is the 
-00001420: 6c6f 6361 7469 6f6e 2079 6f75 2077 616e  location you wan
-00001430: 7420 746f 2072 756e 2074 6865 2073 6361  t to run the sca
-00001440: 6e73 2028 6465 6661 756c 7420 6973 2063  ns (default is c
-00001450: 7572 7265 6e74 2064 6972 6563 746f 7279  urrent directory
-00001460: 293b 2020 0a49 6e20 7468 6520 6361 7365  );  .In the case
-00001470: 206f 6620 6062 6c61 636b 6020 616e 6420   of `black` and 
-00001480: 6069 736f 7274 602c 2061 6e6f 7468 6572  `isort`, another
-00001490: 206f 7074 696f 6e61 6c20 7061 7261 6d65   optional parame
-000014a0: 7465 7220 602d 2d66 6978 6020 6361 6e20  ter `--fix` can 
-000014b0: 6265 2070 6173 7365 642e 0a54 6869 7320  be passed..This 
-000014c0: 7769 6c6c 2061 6c6c 6f77 2074 6865 2074  will allow the t
-000014d0: 6f6f 6c73 2074 6f20 646f 2074 6865 2073  ools to do the s
-000014e0: 7567 6765 7374 6564 2063 6861 6e67 6573  uggested changes
-000014f0: 2028 6966 2061 7070 6c69 6361 626c 6529   (if applicable)
-00001500: 2e0a 5275 6e6e 696e 6720 6073 7536 2066  ..Running `su6 f
-00001510: 6978 6020 7769 6c6c 2072 756e 2062 6f74  ix` will run bot
-00001520: 6820 7468 6573 6520 746f 6f6c 7320 7769  h these tools wi
-00001530: 7468 2074 6865 2060 2d2d 6669 7860 2066  th the `--fix` f
-00001540: 6c61 672e 2020 0a46 6f72 2060 7079 7465  lag.  .For `pyte
-00001550: 7374 602c 2060 2d2d 6a73 6f6e 602c 2060  st`, `--json`, `
-00001560: 2d2d 6874 6d6c 602c 2060 2d2d 6261 6467  --html`, `--badg
-00001570: 6520 3c73 7472 3e60 2061 6e64 2060 2d2d  e <str>` and `--
-00001580: 636f 7665 7261 6765 203c 696e 743e 6020  coverage <int>` 
-00001590: 6172 6520 7375 7070 6f72 7465 642e 0a54  are supported..T
-000015a0: 6865 206c 6174 7465 7220 7477 6f20 6361  he latter two ca
-000015b0: 6e20 616c 736f 2062 6520 636f 6e66 6967  n also be config
-000015c0: 7572 6564 2069 6e20 7468 6520 7079 7072  ured in the pypr
-000015d0: 6f6a 6563 742e 746f 6d6c 2028 7365 6520  oject.toml (see 
-000015e0: 5b27 436f 6e66 6967 7572 6174 696f 6e27  ['Configuration'
-000015f0: 5d28 2363 6f6e 6669 6775 7261 7469 6f6e  ](#configuration
-00001600: 2929 2e0a 5468 6520 6669 7273 7420 7477  ))..The first tw
-00001610: 6f20 6172 6775 6d65 6e74 7320 6361 6e20  o arguments can 
-00001620: 6265 2075 7365 6420 746f 2063 6f6e 7472  be used to contr
-00001630: 6f6c 2074 6865 206f 7574 7075 7420 666f  ol the output fo
-00001640: 726d 6174 206f 6620 6070 7974 6573 7420  rmat of `pytest 
-00001650: 2d2d 636f 7660 2e20 426f 7468 206f 7074  --cov`. Both opt
-00001660: 696f 6e73 2063 616e 2062 6520 7573 6564  ions can be used
-00001670: 2061 7420 7468 6520 7361 6d65 0a74 696d   at the same.tim
-00001680: 652e 2054 6865 2060 2d2d 636f 7665 7261  e. The `--covera
-00001690: 6765 6020 666c 6167 2063 616e 2062 6520  ge` flag can be 
-000016a0: 7573 6564 2074 6f20 7365 7420 6120 7468  used to set a th
-000016b0: 7265 7368 6f6c 6420 666f 7220 636f 6465  reshold for code
-000016c0: 2063 6f76 6572 6167 6520 252e 2049 6620   coverage %. If 
-000016d0: 7468 6520 636f 7665 7261 6765 2069 7320  the coverage is 
-000016e0: 6c65 7373 2074 6861 6e20 7468 6973 0a74  less than this.t
-000016f0: 6872 6573 686f 6c64 2c20 7468 6520 6368  hreshold, the ch
-00001700: 6563 6b20 7769 6c6c 2066 6169 6c2e 0a49  eck will fail..I
-00001710: 6620 6062 6164 6765 6020 6973 2073 6574  f `badge` is set
-00001720: 2075 7369 6e67 2063 6c69 206f 7220 746f   using cli or to
-00001730: 6d6c 2063 6f6e 6669 672c 2061 2053 5647  ml config, a SVG
-00001740: 2062 6164 6765 2077 6974 6820 7468 6520   badge with the 
-00001750: 636f 7665 7261 6765 2025 2077 696c 6c20  coverage % will 
-00001760: 6265 2067 656e 6572 6174 6564 2e0a 5468  be generated..Th
-00001770: 6973 2062 6164 6765 2063 616e 2062 6520  is badge can be 
-00001780: 7573 6564 2069 6e20 666f 7220 6578 616d  used in for exam
-00001790: 706c 6520 7468 6520 5245 4144 4d45 2e6d  ple the README.m
-000017a0: 642e 0a0a 2323 2320 436f 6e66 6967 7572  d...### Configur
-000017b0: 6174 696f 6e0a 0a49 6e20 796f 7572 2060  ation..In your `
-000017c0: 7079 7072 6f6a 6563 742e 746f 6d6c 602c  pyproject.toml`,
-000017d0: 2079 6f75 2063 616e 2061 6464 2061 2060   you can add a `
-000017e0: 5b74 6f6f 6c73 2e73 7536 5d60 2073 6563  [tools.su6]` sec
-000017f0: 7469 6f6e 2074 6f20 636f 6e66 6967 7572  tion to configur
-00001800: 6520 736f 6d65 206f 6620 7468 6520 6265  e some of the be
-00001810: 6861 7669 6f72 206f 6620 7468 6973 2074  havior of this t
-00001820: 6f6f 6c73 2e0a 4375 7272 656e 746c 792c  ools..Currently,
-00001830: 2074 6865 2066 6f6c 6c6f 7769 6e67 206b   the following k
-00001840: 6579 7320 6172 6520 7375 7070 6f72 7465  eys are supporte
-00001850: 643a 0a0a 6060 6074 6f6d 6c0a 5b74 6f6f  d:..```toml.[too
-00001860: 6c2e 7375 365d 0a64 6972 6563 746f 7279  l.su6].directory
-00001870: 203d 2022 2e22 2023 2073 7472 696e 6720   = "." # string 
-00001880: 7061 7468 2074 6f20 7468 6520 6469 7265  path to the dire
-00001890: 6374 6f72 7920 6f6e 2077 6869 6368 2074  ctory on which t
-000018a0: 6f20 7275 6e20 616c 6c20 746f 6f6c 732c  o run all tools,
-000018b0: 2065 2e67 2e20 2773 7263 270a 696e 636c   e.g. 'src'.incl
-000018c0: 7564 6520 3d20 5b5d 2023 206c 6973 7420  ude = [] # list 
-000018d0: 6f66 2063 6865 636b 7320 746f 2072 756e  of checks to run
-000018e0: 2028 7768 656e 2063 616c 6c69 6e67 2060   (when calling `
-000018f0: 7375 3620 616c 6c60 292c 2065 2e67 2e20  su6 all`), e.g. 
-00001900: 5b27 626c 6163 6b27 2c20 276d 7970 7927  ['black', 'mypy'
-00001910: 5d0a 6578 636c 7564 6520 3d20 5b5d 2023  ].exclude = [] #
-00001920: 206c 6973 7420 6f66 2063 6865 636b 7320   list of checks 
-00001930: 746f 2073 6b69 7020 2877 6865 6e20 6361  to skip (when ca
-00001940: 6c6c 696e 6720 6073 7536 2061 6c6c 6029  lling `su6 all`)
-00001950: 2c20 652e 672e 205b 2762 616e 6469 7427  , e.g. ['bandit'
-00001960: 5d0a 7374 6f70 2d61 6674 6572 2d66 6972  ].stop-after-fir
-00001970: 7374 2d66 6169 6c75 7265 203d 2066 616c  st-failure = fal
-00001980: 7365 2020 2320 626f 6f6c 2074 6f20 696e  se  # bool to in
-00001990: 6469 6361 7465 2077 6865 7468 6572 2074  dicate whether t
-000019a0: 6f20 6578 6974 2027 616c 6c27 2061 6674  o exit 'all' aft
-000019b0: 6572 206f 6e65 2066 6169 6c75 7265 206f  er one failure o
-000019c0: 7220 746f 2064 6f20 616c 6c20 6368 6563  r to do all chec
-000019d0: 6b73 0a63 6f76 6572 6167 6520 3d20 3130  ks.coverage = 10
-000019e0: 3020 2320 696e 7420 7468 7265 7368 6f6c  0 # int threshol
-000019f0: 6420 666f 7220 7079 7465 7374 2063 6f76  d for pytest cov
-00001a00: 6572 6167 6520 0a62 6164 6765 203d 2022  erage .badge = "
-00001a10: 636f 7665 7261 6765 2e73 7667 2220 2023  coverage.svg"  #
-00001a20: 2073 7472 2070 6174 6820 6f72 2062 6f6f   str path or boo
-00001a30: 6c20 2874 7275 6520 7c20 6661 6c73 6529  l (true | false)
-00001a40: 2077 6865 7468 6572 2061 6e64 2077 6865   whether and whe
-00001a50: 7265 2074 6f20 6f75 7470 7574 2074 6865  re to output the
-00001a60: 2063 6f76 6572 6167 6520 6261 6467 650a   coverage badge.
-00001a70: 6060 600a 0a41 6c6c 206b 6579 7320 6172  ```..All keys ar
-00001a80: 6520 6f70 7469 6f6e 616c 2e20 4e6f 7465  e optional. Note
-00001a90: 2074 6861 7420 6966 2079 6f75 2068 6176   that if you hav
-00001aa0: 6520 626f 7468 2061 6e20 6069 6e63 6c75  e both an `inclu
-00001ab0: 6465 6020 6173 2077 656c 6c20 6173 2061  de` as well as a
-00001ac0: 6e20 6065 7863 6c75 6465 602c 2061 6c6c  n `exclude`, all
-00001ad0: 2074 6865 2074 6f6f 6c73 2069 6e20 6069   the tools in `i
-00001ae0: 6e63 6c75 6465 6020 7769 6c6c 0a72 756e  nclude` will.run
-00001af0: 2061 6e64 2060 6578 636c 7564 6560 2077   and `exclude` w
-00001b00: 696c 6c20 6265 2066 756c 6c79 2069 676e  ill be fully ign
-00001b10: 6f72 6564 2e20 200a 4164 6469 7469 6f6e  ored.  .Addition
-00001b20: 616c 6c79 2c20 7468 6520 6f72 6465 7220  ally, the order 
-00001b30: 696e 2077 6869 6368 2074 6865 2063 6865  in which the che
-00001b40: 636b 7320 6172 6520 6465 6669 6e65 6420  cks are defined 
-00001b50: 696e 2027 696e 636c 7564 6527 2c20 6973  in 'include', is
-00001b60: 2074 6865 206f 7264 6572 2069 6e20 7768   the order in wh
-00001b70: 6963 6820 7468 6579 2077 696c 6c20 7275  ich they will ru
-00001b80: 6e20 2869 6e20 6061 6c6c 600a 616e 6420  n (in `all`.and 
-00001b90: 6066 6978 6029 0a0a 2323 2320 4769 7468  `fix`)..### Gith
-00001ba0: 7562 2041 6374 696f 6e0a 0a49 6e20 6f72  ub Action..In or
-00001bb0: 6465 7220 746f 2075 7365 2074 6869 7320  der to use this 
-00001bc0: 6368 6563 6b65 7220 7769 7468 696e 2047  checker within G
-00001bd0: 6974 6875 6220 746f 2072 756e 2063 6865  ithub to run che
-00001be0: 636b 7320 6166 7465 7220 7075 7368 696e  cks after pushin
-00001bf0: 672c 0a79 6f75 2063 616e 2061 6464 2061  g,.you can add a
-00001c00: 2077 6f72 6b66 6c6f 7720 2865 2e67 2e20   workflow (e.g. 
-00001c10: 602e 6769 7468 7562 2f77 6f72 6b66 6c6f  `.github/workflo
-00001c20: 7773 2f73 7536 2e79 616d 6c60 2920 6c69  ws/su6.yaml`) li
-00001c30: 6b65 2074 6869 7320 6578 616d 706c 653a  ke this example:
-00001c40: 0a0a 6060 6079 616d 6c0a 6e61 6d65 3a20  ..```yaml.name: 
-00001c50: 7275 6e20 7375 3620 6368 6563 6b73 0a6f  run su6 checks.o
-00001c60: 6e3a 0a20 2070 7573 683a 0a20 2020 2062  n:.  push:.    b
-00001c70: 7261 6e63 6865 732d 6967 6e6f 7265 3a0a  ranches-ignore:.
-00001c80: 2020 2020 2020 2d20 6d61 7374 6572 0a6a        - master.j
-00001c90: 6f62 733a 0a20 2063 6865 636b 3a0a 2020  obs:.  check:.  
-00001ca0: 2020 6e61 6d65 3a20 4368 6563 6b20 7769    name: Check wi
-00001cb0: 7468 2060 7375 3620 616c 6c60 0a20 2020  th `su6 all`.   
-00001cc0: 2072 756e 732d 6f6e 3a20 7562 756e 7475   runs-on: ubuntu
-00001cd0: 2d6c 6174 6573 740a 2020 2020 7374 6570  -latest.    step
-00001ce0: 733a 0a20 2020 2020 202d 2075 7365 733a  s:.      - uses:
-00001cf0: 2061 6374 696f 6e73 2f63 6865 636b 6f75   actions/checkou
-00001d00: 7440 7633 0a20 2020 2020 202d 2075 7365  t@v3.      - use
-00001d10: 733a 2061 6374 696f 6e73 2f73 6574 7570  s: actions/setup
-00001d20: 2d70 7974 686f 6e40 7634 0a20 2020 2020  -python@v4.     
-00001d30: 2020 2077 6974 683a 0a20 2020 2020 2020     with:.       
-00001d40: 2020 2070 7974 686f 6e2d 7665 7273 696f     python-versio
-00001d50: 6e3a 2027 332e 3131 270a 2020 2020 2020  n: '3.11'.      
-00001d60: 2020 2020 6361 6368 653a 2027 7069 7027      cache: 'pip'
-00001d70: 2023 2063 6163 6869 6e67 2070 6970 2064   # caching pip d
-00001d80: 6570 656e 6465 6e63 6965 730a 2020 2020  ependencies.    
-00001d90: 2020 2d20 7275 6e3a 2070 6970 2069 6e73    - run: pip ins
-00001da0: 7461 6c6c 2073 7536 5b61 6c6c 5d20 2e0a  tall su6[all] ..
-00001db0: 2020 2020 2020 2d20 7275 6e3a 2073 7536        - run: su6
-00001dc0: 2061 6c6c 0a60 6060 0a0a 2a2a 4e6f 7465   all.```..**Note
-00001dd0: 3a2a 2a20 6966 2079 6f75 2064 6f6e 2774  :** if you don't
-00001de0: 2077 616e 7420 746f 2072 756e 2061 6c6c   want to run all
-00001df0: 2063 6865 636b 732c 2062 7574 2073 7065   checks, but spe
-00001e00: 6369 6669 6320 6f6e 6573 206f 6e6c 792c  cific ones only,
-00001e10: 2079 6f75 206e 6565 6420 746f 2061 6464   you need to add
-00001e20: 2074 6865 2060 2d2d 6967 6e6f 7265 2d75   the `--ignore-u
-00001e30: 6e69 6e73 7461 6c6c 6564 6020 666c 6167  ninstalled` flag
-00001e40: 0a74 6f20 6073 7536 2061 6c6c 6021 204f  .to `su6 all`! O
-00001e50: 7468 6572 7769 7365 2c20 4769 7468 7562  therwise, Github
-00001e60: 2077 696c 6c20 7365 6520 6578 6974 2063   will see exit c
-00001e70: 6f64 6520 3132 3720 2863 6f6d 6d61 6e64  ode 127 (command
-00001e80: 206d 6973 7369 6e67 2920 6173 2061 2066   missing) as a f
-00001e90: 6169 6c75 7265 2e0a 0a60 6060 7961 6d6c  ailure...```yaml
-00001ea0: 0a6e 616d 653a 2072 756e 2073 6f6d 6520  .name: run some 
-00001eb0: 7375 3620 6368 6563 6b73 0a6f 6e3a 0a20  su6 checks.on:. 
-00001ec0: 2070 7573 683a 0a20 2020 2062 7261 6e63   push:.    branc
-00001ed0: 6865 732d 6967 6e6f 7265 3a0a 2020 2020  hes-ignore:.    
-00001ee0: 2020 2d20 6d61 7374 6572 0a6a 6f62 733a    - master.jobs:
-00001ef0: 0a20 2063 6865 636b 3a0a 2020 2020 6e61  .  check:.    na
-00001f00: 6d65 3a20 4368 6563 6b20 7769 7468 2060  me: Check with `
-00001f10: 7375 3620 616c 6c60 0a20 2020 2072 756e  su6 all`.    run
-00001f20: 732d 6f6e 3a20 7562 756e 7475 2d6c 6174  s-on: ubuntu-lat
-00001f30: 6573 740a 2020 2020 7374 6570 733a 0a20  est.    steps:. 
-00001f40: 2020 2020 202d 2075 7365 733a 2061 6374       - uses: act
-00001f50: 696f 6e73 2f63 6865 636b 6f75 7440 7633  ions/checkout@v3
-00001f60: 0a20 2020 2020 202d 2075 7365 733a 2061  .      - uses: a
-00001f70: 6374 696f 6e73 2f73 6574 7570 2d70 7974  ctions/setup-pyt
-00001f80: 686f 6e40 7634 0a20 2020 2020 2020 2077  hon@v4.        w
-00001f90: 6974 683a 0a20 2020 2020 2020 2020 2070  ith:.          p
-00001fa0: 7974 686f 6e2d 7665 7273 696f 6e3a 2027  ython-version: '
-00001fb0: 332e 3131 270a 2020 2020 2020 2020 2020  3.11'.          
-00001fc0: 6361 6368 653a 2027 7069 7027 2023 2063  cache: 'pip' # c
-00001fd0: 6163 6869 6e67 2070 6970 2064 6570 656e  aching pip depen
-00001fe0: 6465 6e63 6965 730a 2020 2020 2020 2d20  dencies.      - 
-00001ff0: 7275 6e3a 2070 6970 2069 6e73 7461 6c6c  run: pip install
-00002000: 2073 7536 5b70 7963 6f64 6573 7479 6c65   su6[pycodestyle
-00002010: 2c62 6c61 636b 5d20 2e0a 2020 2020 2020  ,black] ..      
-00002020: 2d20 7275 6e3a 2073 7536 2061 6c6c 202d  - run: su6 all -
-00002030: 2d69 676e 6f72 652d 756e 696e 7374 616c  -ignore-uninstal
-00002040: 6c65 6420 2023 202e 2e2e 206f 7468 6572  led  # ... other
-00002050: 2073 6574 7469 6e67 7320 7375 6368 2061   settings such a
-00002060: 7320 2d2d 7374 6f70 2d61 6674 6572 2d66  s --stop-after-f
-00002070: 6972 7374 2d66 6169 6c75 7265 2c20 2d2d  irst-failure, --
-00002080: 636f 7665 7261 6765 202e 2e2e 0a60 6060  coverage ....```
-00002090: 0a0a 2323 2050 6c75 6769 6e73 0a54 6869  ..## Plugins.Thi
-000020a0: 7320 746f 6f6c 2061 6c73 6f20 7375 7070  s tool also supp
-000020b0: 6f72 7473 2070 6c75 6769 6e73 2074 6f20  orts plugins to 
-000020c0: 6164 6420 6578 7472 6120 6368 6563 6b65  add extra checke
-000020d0: 7273 206f 7220 6f74 6865 7220 6675 6e63  rs or other func
-000020e0: 7469 6f6e 616c 6974 792e 2053 6565 205b  tionality. See [
-000020f0: 646f 6373 2f70 6c75 6769 6e73 2e6d 645d  docs/plugins.md]
-00002100: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002110: 636f 6d2f 726f 6269 6e76 616e 6465 726e  com/robinvandern
-00002120: 6f6f 7264 2f73 7536 2d63 6865 636b 6572  oord/su6-checker
-00002130: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-00002140: 732f 706c 7567 696e 732e 6d64 290a 0a23  s/plugins.md)..#
-00002150: 2320 4c69 6365 6e73 650a 0a60 7375 3660  # License..`su6`
-00002160: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
-00002170: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
-00002180: 6f66 2074 6865 205b 4d49 545d 2868 7474  of the [MIT](htt
-00002190: 7073 3a2f 2f73 7064 782e 6f72 672f 6c69  ps://spdx.org/li
-000021a0: 6365 6e73 6573 2f4d 4954 2e68 746d 6c29  censes/MIT.html)
-000021b0: 206c 6963 656e 7365 2e0a 0a23 2320 4368   license...## Ch
-000021c0: 616e 6765 6c6f 670a 0a53 6565 2060 4348  angelog..See `CH
-000021d0: 414e 4745 4c4f 472e 6d64 6020 5b6f 6e20  ANGELOG.md` [on 
-000021e0: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
-000021f0: 6769 7468 7562 2e63 6f6d 2f72 6f62 696e  github.com/robin
-00002200: 7661 6e64 6572 6e6f 6f72 642f 7375 362d  vandernoord/su6-
-00002210: 6368 6563 6b65 722f 626c 6f62 2f6d 6173  checker/blob/mas
-00002220: 7465 722f 4348 414e 4745 4c4f 472e 6d64  ter/CHANGELOG.md
-00002230: 290a                                     ).
+000007f0: 6172 6b64 6f77 6e0a 0a3c 6469 7620 616c  arkdown..<div al
+00000800: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000810: 2020 3c69 6d67 200a 2020 2020 2020 2020    <img .        
+00000820: 616c 6967 6e3d 2263 656e 7465 7222 200a  align="center" .
+00000830: 2020 2020 2020 2020 7372 633d 2268 7474          src="htt
+00000840: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000850: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f72  sercontent.com/r
+00000860: 6f62 696e 7661 6e64 6572 6e6f 6f72 642f  obinvandernoord/
+00000870: 7375 362d 6368 6563 6b65 722f 6d61 7374  su6-checker/mast
+00000880: 6572 2f5f 7374 6174 6963 2f73 7536 2e73  er/_static/su6.s
+00000890: 7667 2220 0a20 2020 2020 2020 2061 6c74  vg" .        alt
+000008a0: 3d22 7375 3620 6368 6563 6b65 7222 0a20  ="su6 checker". 
+000008b0: 2020 2020 2020 2077 6964 7468 3d22 3430         width="40
+000008c0: 3070 7822 0a20 2020 2020 2020 202f 3e0a  0px".        />.
+000008d0: 2020 2020 3c68 3120 616c 6967 6e3d 2263      <h1 align="c
+000008e0: 656e 7465 7222 3e73 7536 3c2f 6831 3e0a  enter">su6</h1>.
+000008f0: 3c2f 6469 763e 0a0a 3c64 6976 2061 6c69  </div>..<div ali
+00000900: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000910: 2036 2069 7320 7072 6f6e 6f75 6e63 6564   6 is pronounced
+00000920: 2061 7320 272f 7ac9 9b73 2f27 2069 6e20   as '/z..s/' in 
+00000930: 4475 7463 682c 2073 6f20 2773 7536 2720  Dutch, so 'su6' 
+00000940: 6973 2062 6173 6963 616c 6c79 2027 7375  is basically 'su
+00000950: 6363 6573 7327 2e20 3c62 7220 2f3e 0a20  ccess'. <br />. 
+00000960: 2020 2054 6869 7320 7061 636b 6167 6520     This package 
+00000970: 7769 6c6c 2068 6f70 6566 756c 6c79 2068  will hopefully h
+00000980: 656c 7020 6163 6869 6576 6520 7468 6174  elp achieve that
+00000990: 210a 3c2f 6469 763e 0a0a 3c62 723e 0a0a  !.</div>..<br>..
+000009a0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+000009b0: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+000009c0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+000009d0: 7267 2f70 726f 6a65 6374 2f73 7536 223e  rg/project/su6">
+000009e0: 3c69 6d67 2061 6c74 3d22 5079 5049 202d  <img alt="PyPI -
+000009f0: 2056 6572 7369 6f6e 2220 7372 633d 2268   Version" src="h
+00000a00: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000a10: 6473 2e69 6f2f 7079 7069 2f76 2f73 7536  ds.io/pypi/v/su6
+00000a20: 2e73 7667 222f 3e3c 2f61 3e0a 2020 2020  .svg"/></a>.    
+00000a30: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000a40: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000a50: 742f 7375 3622 3e3c 696d 6720 616c 743d  t/su6"><img alt=
+00000a60: 2250 7950 4920 2d20 5079 7468 6f6e 2056  "PyPI - Python V
+00000a70: 6572 7369 6f6e 2220 7372 633d 2268 7474  ersion" src="htt
+00000a80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000a90: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
+00000aa0: 6f6e 732f 7375 362e 7376 6722 2f3e 3c2f  ons/su6.svg"/></
+00000ab0: 613e 0a20 2020 203c 6272 2f3e 0a20 2020  a>.    <br/>.   
+00000ac0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000ad0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
+00000ae0: 2f62 6c61 636b 223e 3c69 6d67 2061 6c74  /black"><img alt
+00000af0: 3d22 436f 6465 2073 7479 6c65 3a20 626c  ="Code style: bl
+00000b00: 6163 6b22 2073 7263 3d22 6874 7470 733a  ack" src="https:
+00000b10: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000b20: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
+00000b30: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
+00000b40: 2e73 7667 222f 3e3c 2f61 3e0a 2020 2020  .svg"/></a>.    
+00000b50: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000b60: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
+00000b70: 6c69 6365 6e73 6573 2f4d 4954 223e 3c69  licenses/MIT"><i
+00000b80: 6d67 2061 6c74 3d22 4c69 6365 6e73 653a  mg alt="License:
+00000b90: 204d 4954 2220 7372 633d 2268 7474 7073   MIT" src="https
+00000ba0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000bb0: 6f2f 6261 6467 652f 4c69 6365 6e73 652d  o/badge/License-
+00000bc0: 4d49 542d 7965 6c6c 6f77 2e73 7667 222f  MIT-yellow.svg"/
+00000bd0: 3e3c 2f61 3e0a 2020 2020 3c62 722f 3e0a  ></a>.    <br/>.
+00000be0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000bf0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000c00: 726f 6269 6e76 616e 6465 726e 6f6f 7264  robinvandernoord
+00000c10: 2f73 7536 2d63 6865 636b 6572 2f61 6374  /su6-checker/act
+00000c20: 696f 6e73 223e 3c69 6d67 2061 6c74 3d22  ions"><img alt="
+00000c30: 7375 3620 6368 6563 6b73 2220 7372 633d  su6 checks" src=
+00000c40: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000c50: 636f 6d2f 726f 6269 6e76 616e 6465 726e  com/robinvandern
+00000c60: 6f6f 7264 2f73 7536 2d63 6865 636b 6572  oord/su6-checker
+00000c70: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000c80: 7773 2f73 7536 2e79 6d6c 2f62 6164 6765  ws/su6.yml/badge
+00000c90: 2e73 7667 3f62 7261 6e63 683d 6465 7665  .svg?branch=deve
+00000ca0: 6c6f 706d 656e 7422 2f3e 3c2f 613e 0a20  lopment"/></a>. 
+00000cb0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000cc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
+00000cd0: 6f62 696e 7661 6e64 6572 6e6f 6f72 642f  obinvandernoord/
+00000ce0: 7375 362d 6368 6563 6b65 722f 6163 7469  su6-checker/acti
+00000cf0: 6f6e 7322 3e3c 696d 6720 616c 743d 2243  ons"><img alt="C
+00000d00: 6f76 6572 6167 6522 2073 7263 3d22 636f  overage" src="co
+00000d10: 7665 7261 6765 2e73 7667 222f 3e3c 2f61  verage.svg"/></a
+00000d20: 3e0a 3c2f 6469 763e 0a0a 2d2d 2d2d 2d0a  >.</div>..-----.
+00000d30: 0a2a 2a54 6162 6c65 206f 6620 436f 6e74  .**Table of Cont
+00000d40: 656e 7473 2a2a 0a0a 2d20 5b49 6e73 7461  ents**..- [Insta
+00000d50: 6c6c 6174 696f 6e5d 2823 696e 7374 616c  llation](#instal
+00000d60: 6c61 7469 6f6e 290a 2d20 5b55 7361 6765  lation).- [Usage
+00000d70: 5d28 2375 7361 6765 290a 2d20 5b4c 6963  ](#usage).- [Lic
+00000d80: 656e 7365 5d28 236c 6963 656e 7365 290a  ense](#license).
+00000d90: 2d20 5b50 6c75 6769 6e73 5d28 2370 6c75  - [Plugins](#plu
+00000da0: 6769 6e73 290a 2d20 5b43 6861 6e67 656c  gins).- [Changel
+00000db0: 6f67 5d28 2363 6861 6e67 656c 6f67 290a  og](#changelog).
+00000dc0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000dd0: 0a0a 6060 6063 6f6e 736f 6c65 0a23 2071  ..```console.# q
+00000de0: 7569 636b 2069 6e73 7461 6c6c 2077 6974  uick install wit
+00000df0: 6820 616c 6c20 706f 7373 6962 6c65 2063  h all possible c
+00000e00: 6865 636b 6572 733a 0a70 6970 2069 6e73  heckers:.pip ins
+00000e10: 7461 6c6c 2073 7536 5b61 6c6c 5d0a 2320  tall su6[all].# 
+00000e20: 6f72 2070 6963 6b20 616e 6420 6368 6f6f  or pick and choo
+00000e30: 7365 2063 6865 636b 6572 733a 0a70 6970  se checkers:.pip
+00000e40: 2069 6e73 7461 6c6c 205b 626c 6163 6b2c   install [black,
+00000e50: 6261 6e64 6974 2c70 7964 6f63 7374 796c  bandit,pydocstyl
+00000e60: 655d 0a60 6060 0a0a 2a2a 4e6f 7465 2a2a  e].```..**Note**
+00000e70: 3a20 7468 6973 2070 6163 6b61 6765 2064  : this package d
+00000e80: 6f65 7320 6e6f 7420 776f 726b 2077 656c  oes not work wel
+00000e90: 6c20 7769 7468 2060 7069 7078 602c 2073  l with `pipx`, s
+00000ea0: 696e 6365 2061 206c 6f74 206f 6620 7468  ince a lot of th
+00000eb0: 6520 746f 6f6c 7320 6e65 6564 2074 6f20  e tools need to 
+00000ec0: 6265 2069 6e20 7468 6520 7361 6d65 2028  be in the same (
+00000ed0: 7669 7274 7561 6c29 0a65 6e76 6972 6f6e  virtual).environ
+00000ee0: 6d65 6e74 0a6f 6620 796f 7572 2063 6f64  ment.of your cod
+00000ef0: 652c 2069 6e20 6f72 6465 7220 746f 2064  e, in order to d
+00000f00: 6f20 7072 6f70 6572 2061 6e61 6c79 7369  o proper analysi
+00000f10: 732e 0a0a 5468 6520 666f 6c6c 6f77 696e  s...The followin
+00000f20: 6720 6368 6563 6b65 7273 2061 7265 2073  g checkers are s
+00000f30: 7570 706f 7274 6564 3a0a 0a23 2323 2072  upported:..### r
+00000f40: 7566 660a 0a2d 2069 6e73 7461 6c6c 3a20  uff..- install: 
+00000f50: 6070 6970 2069 6e73 7461 6c6c 2073 7536  `pip install su6
+00000f60: 5b72 7566 665d 600a 2d20 7573 653a 2060  [ruff]`.- use: `
+00000f70: 7375 3620 7275 6666 205b 6469 7265 6374  su6 ruff [direct
+00000f80: 6f72 795d 600a 2d20 6675 6e63 7469 6f6e  ory]`.- function
+00000f90: 616c 6974 793a 206c 696e 7465 720a 2d20  ality: linter.- 
+00000fa0: 7079 7069 3a20 5b72 7566 665d 2868 7474  pypi: [ruff](htt
+00000fb0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00000fc0: 6f6a 6563 742f 7275 6666 2f29 0a0a 2323  oject/ruff/)..##
+00000fd0: 2320 626c 6163 6b0a 0a2d 2069 6e73 7461  # black..- insta
+00000fe0: 6c6c 3a20 6070 6970 2069 6e73 7461 6c6c  ll: `pip install
+00000ff0: 2073 7536 5b62 6c61 636b 5d60 0a2d 2075   su6[black]`.- u
+00001000: 7365 3a20 6073 7536 2062 6c61 636b 205b  se: `su6 black [
+00001010: 6469 7265 6374 6f72 795d 205b 2d2d 6669  directory] [--fi
+00001020: 785d 600a 2d20 6675 6e63 7469 6f6e 616c  x]`.- functional
+00001030: 6974 793a 2066 6f72 6d61 7474 6572 0a2d  ity: formatter.-
+00001040: 2070 7970 693a 205b 626c 6163 6b5d 2868   pypi: [black](h
+00001050: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00001060: 7072 6f6a 6563 742f 626c 6163 6b2f 290a  project/black/).
+00001070: 0a23 2323 206d 7970 790a 0a2d 2069 6e73  .### mypy..- ins
+00001080: 7461 6c6c 3a20 6070 6970 2069 6e73 7461  tall: `pip insta
+00001090: 6c6c 2073 7536 5b6d 7970 795d 600a 2d20  ll su6[mypy]`.- 
+000010a0: 7573 653a 2060 7375 3620 6d79 7079 205b  use: `su6 mypy [
+000010b0: 6469 7265 6374 6f72 795d 600a 2d20 6675  directory]`.- fu
+000010c0: 6e63 7469 6f6e 616c 6974 793a 2073 7461  nctionality: sta
+000010d0: 7469 6320 7479 7065 2063 6865 636b 6572  tic type checker
+000010e0: 0a2d 2070 7970 693a 205b 6d79 7079 5d28  .- pypi: [mypy](
+000010f0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001100: 2f70 726f 6a65 6374 2f6d 7970 792f 290a  /project/mypy/).
+00001110: 0a23 2323 2062 616e 6469 740a 0a2d 2069  .### bandit..- i
+00001120: 6e73 7461 6c6c 3a20 6070 6970 2069 6e73  nstall: `pip ins
+00001130: 7461 6c6c 2073 7536 5b62 616e 6469 745d  tall su6[bandit]
+00001140: 600a 2d20 7573 653a 2060 7375 3620 6261  `.- use: `su6 ba
+00001150: 6e64 6974 205b 6469 7265 6374 6f72 795d  ndit [directory]
+00001160: 600a 2d20 6675 6e63 7469 6f6e 616c 6974  `.- functionalit
+00001170: 793a 2073 6563 7572 6974 7920 6c69 6e74  y: security lint
+00001180: 6572 0a2d 2070 7970 693a 205b 6261 6e64  er.- pypi: [band
+00001190: 6974 5d28 6874 7470 733a 2f2f 7079 7069  it](https://pypi
+000011a0: 2e6f 7267 2f70 726f 6a65 6374 2f62 616e  .org/project/ban
+000011b0: 6469 742f 290a 0a23 2323 2069 736f 7274  dit/)..### isort
+000011c0: 0a0a 2d20 696e 7374 616c 6c3a 2060 7069  ..- install: `pi
+000011d0: 7020 696e 7374 616c 6c20 7375 365b 6973  p install su6[is
+000011e0: 6f72 745d 600a 2d20 7573 653a 2060 7375  ort]`.- use: `su
+000011f0: 3620 6973 6f72 7420 5b64 6972 6563 746f  6 isort [directo
+00001200: 7279 5d20 5b2d 2d66 6978 5d60 0a2d 2066  ry] [--fix]`.- f
+00001210: 756e 6374 696f 6e61 6c69 7479 3a20 696d  unctionality: im
+00001220: 706f 7274 2073 6f72 7465 720a 2d20 7079  port sorter.- py
+00001230: 7069 3a20 5b69 736f 7274 5d28 6874 7470  pi: [isort](http
+00001240: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00001250: 6a65 6374 2f69 736f 7274 2f29 0a0a 2323  ject/isort/)..##
+00001260: 2320 7079 646f 6373 7479 6c65 0a0a 2d20  # pydocstyle..- 
+00001270: 696e 7374 616c 6c3a 2060 7069 7020 696e  install: `pip in
+00001280: 7374 616c 6c20 7375 365b 7079 646f 6373  stall su6[pydocs
+00001290: 7479 6c65 5d60 0a2d 2075 7365 3a20 6073  tyle]`.- use: `s
+000012a0: 7536 2070 7964 6f63 7374 796c 6520 5b64  u6 pydocstyle [d
+000012b0: 6972 6563 746f 7279 5d60 0a2d 2066 756e  irectory]`.- fun
+000012c0: 6374 696f 6e61 6c69 7479 3a20 646f 6373  ctionality: docs
+000012d0: 7472 696e 6720 6368 6563 6b65 720a 2d20  tring checker.- 
+000012e0: 7079 7069 3a20 5b70 7964 6f63 7374 796c  pypi: [pydocstyl
+000012f0: 655d 2868 7474 7073 3a2f 2f70 7970 692e  e](https://pypi.
+00001300: 6f72 672f 7072 6f6a 6563 742f 7079 646f  org/project/pydo
+00001310: 6373 7479 6c65 2f29 0a0a 2323 2320 7079  cstyle/)..### py
+00001320: 7465 7374 0a0a 2d20 696e 7374 616c 6c3a  test..- install:
+00001330: 2060 7069 7020 696e 7374 616c 6c20 7375   `pip install su
+00001340: 365b 7079 7465 7374 5d60 0a2d 2075 7365  6[pytest]`.- use
+00001350: 3a20 6073 7536 2070 7974 6573 7420 5b64  : `su6 pytest [d
+00001360: 6972 6563 746f 7279 5d20 5b2d 2d63 6f76  irectory] [--cov
+00001370: 6572 6167 6520 3c69 6e74 3e5d 205b 2d2d  erage <int>] [--
+00001380: 6a73 6f6e 5d20 5b2d 2d68 746d 6c5d 205b  json] [--html] [
+00001390: 2d2d 6261 6467 6520 3c70 6174 683e 5d60  --badge <path>]`
+000013a0: 0a2d 2066 756e 6374 696f 6e61 6c69 7479  .- functionality
+000013b0: 3a20 7465 7374 6572 2077 6974 6820 636f  : tester with co
+000013c0: 7665 7261 6765 0a2d 2070 7970 693a 205b  verage.- pypi: [
+000013d0: 7079 7465 7374 5d28 6874 7470 733a 2f2f  pytest](https://
+000013e0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000013f0: 2f70 7974 6573 742f 292c 205b 7079 7465  /pytest/), [pyte
+00001400: 7374 2d63 6f76 5d28 6874 7470 733a 2f2f  st-cov](https://
+00001410: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00001420: 2f70 7974 6573 742d 636f 762f 290a 0a23  /pytest-cov/)..#
+00001430: 2320 5573 6167 650a 0a60 6060 636f 6e73  # Usage..```cons
+00001440: 6f6c 650a 7375 3620 2d2d 6865 6c70 0a23  ole.su6 --help.#
+00001450: 206f 722c 2065 6173 6965 7374 2074 6f20   or, easiest to 
+00001460: 7374 6172 743a 0a73 7536 2061 6c6c 0a23  start:.su6 all.#
+00001470: 2075 7375 616c 2073 6967 6e61 7475 7265   usual signature
+00001480: 3a0a 7375 3620 5b2d 2d76 6572 626f 7369  :.su6 [--verbosi
+00001490: 7479 3d31 7c32 7c33 5d20 5b2d 2d63 6f6e  ty=1|2|3] [--con
+000014a0: 6669 673d 2e2e 2e5d 205b 2d2d 666f 726d  fig=...] [--form
+000014b0: 6174 3d74 6578 747c 6a73 6f6e 5d20 3c73  at=text|json] <s
+000014c0: 7562 636f 6d6d 616e 643e 205b 6469 7265  ubcommand> [dire
+000014d0: 6374 6f72 795d 205b 2e2e 2e73 7065 6369  ctory] [...speci
+000014e0: 6669 6320 6f70 7469 6f6e 735d 0a60 6060  fic options].```
+000014f0: 0a0a 7768 6572 6520 6073 7562 636f 6d6d  ..where `subcomm
+00001500: 616e 6460 2069 7320 6061 6c6c 6020 6f72  and` is `all` or
+00001510: 206f 6e65 206f 6620 7468 6520 6176 6169   one of the avai
+00001520: 6c61 626c 6520 6368 6563 6b65 7273 3b20  lable checkers; 
+00001530: 200a 6076 6572 626f 7369 7479 6020 696e   .`verbosity` in
+00001540: 6469 6361 7465 7320 686f 7720 6d75 6368  dicates how much
+00001550: 2069 6e66 6f72 6d61 7469 6f6e 2079 6f75   information you
+00001560: 2077 616e 7420 746f 2073 6565 2028 6465   want to see (de
+00001570: 6661 756c 7420 6973 2027 3227 292e 2020  fault is '2').  
+00001580: 0a60 636f 6e66 6967 6020 616c 6c6f 7773  .`config` allows
+00001590: 2079 6f75 2074 6f20 7365 6c65 6374 2061   you to select a
+000015a0: 2064 6966 6665 7265 6e74 2060 2e74 6f6d   different `.tom
+000015b0: 6c60 2066 696c 6520 2864 6566 6175 6c74  l` file (default
+000015c0: 2069 7320 6070 7970 726f 6a65 6374 2e74   is `pyproject.t
+000015d0: 6f6d 6c60 292e 2020 0a60 666f 726d 6174  oml`).  .`format
+000015e0: 6020 616c 6c6f 7773 2079 6f75 2074 6f20  ` allows you to 
+000015f0: 6765 7420 6120 4a53 4f4e 206f 7574 7075  get a JSON outpu
+00001600: 7420 696e 7374 6561 6420 6f66 2074 6865  t instead of the
+00001610: 2074 6578 7475 616c 2074 7261 6666 6963   textual traffic
+00001620: 206c 6967 6874 7320 2864 6566 6175 6c74   lights (default
+00001630: 2069 7320 6074 6578 7460 292e 2020 0a60   is `text`).  .`
+00001640: 6469 7265 6374 6f72 7960 2069 7320 7468  directory` is th
+00001650: 6520 6c6f 6361 7469 6f6e 2079 6f75 2077  e location you w
+00001660: 616e 7420 746f 2072 756e 2074 6865 2073  ant to run the s
+00001670: 6361 6e73 2028 6465 6661 756c 7420 6973  cans (default is
+00001680: 2063 7572 7265 6e74 2064 6972 6563 746f   current directo
+00001690: 7279 293b 2020 0a49 6e20 7468 6520 6361  ry);  .In the ca
+000016a0: 7365 206f 6620 6062 6c61 636b 6020 616e  se of `black` an
+000016b0: 6420 6069 736f 7274 602c 2061 6e6f 7468  d `isort`, anoth
+000016c0: 6572 206f 7074 696f 6e61 6c20 7061 7261  er optional para
+000016d0: 6d65 7465 7220 602d 2d66 6978 6020 6361  meter `--fix` ca
+000016e0: 6e20 6265 2070 6173 7365 642e 0a54 6869  n be passed..Thi
+000016f0: 7320 7769 6c6c 2061 6c6c 6f77 2074 6865  s will allow the
+00001700: 2074 6f6f 6c73 2074 6f20 646f 2074 6865   tools to do the
+00001710: 2073 7567 6765 7374 6564 2063 6861 6e67   suggested chang
+00001720: 6573 2028 6966 2061 7070 6c69 6361 626c  es (if applicabl
+00001730: 6529 2e0a 5275 6e6e 696e 6720 6073 7536  e)..Running `su6
+00001740: 2066 6978 6020 7769 6c6c 2072 756e 2062   fix` will run b
+00001750: 6f74 6820 7468 6573 6520 746f 6f6c 7320  oth these tools 
+00001760: 7769 7468 2074 6865 2060 2d2d 6669 7860  with the `--fix`
+00001770: 2066 6c61 672e 2020 0a46 6f72 2060 7079   flag.  .For `py
+00001780: 7465 7374 602c 2060 2d2d 6a73 6f6e 602c  test`, `--json`,
+00001790: 2060 2d2d 6874 6d6c 602c 2060 2d2d 6261   `--html`, `--ba
+000017a0: 6467 6520 3c73 7472 3e60 2061 6e64 2060  dge <str>` and `
+000017b0: 2d2d 636f 7665 7261 6765 203c 696e 743e  --coverage <int>
+000017c0: 6020 6172 6520 7375 7070 6f72 7465 642e  ` are supported.
+000017d0: 0a54 6865 206c 6174 7465 7220 7477 6f20  .The latter two 
+000017e0: 6361 6e20 616c 736f 2062 6520 636f 6e66  can also be conf
+000017f0: 6967 7572 6564 2069 6e20 7468 6520 7079  igured in the py
+00001800: 7072 6f6a 6563 742e 746f 6d6c 2028 7365  project.toml (se
+00001810: 6520 5b27 436f 6e66 6967 7572 6174 696f  e ['Configuratio
+00001820: 6e27 5d28 2363 6f6e 6669 6775 7261 7469  n'](#configurati
+00001830: 6f6e 2929 2e0a 5468 6520 6669 7273 7420  on))..The first 
+00001840: 7477 6f20 6172 6775 6d65 6e74 7320 6361  two arguments ca
+00001850: 6e20 6265 2075 7365 6420 746f 2063 6f6e  n be used to con
+00001860: 7472 6f6c 2074 6865 206f 7574 7075 7420  trol the output 
+00001870: 666f 726d 6174 206f 6620 6070 7974 6573  format of `pytes
+00001880: 7420 2d2d 636f 7660 2e20 426f 7468 206f  t --cov`. Both o
+00001890: 7074 696f 6e73 2063 616e 2062 6520 7573  ptions can be us
+000018a0: 6564 2061 7420 7468 6520 7361 6d65 0a74  ed at the same.t
+000018b0: 696d 652e 2054 6865 2060 2d2d 636f 7665  ime. The `--cove
+000018c0: 7261 6765 6020 666c 6167 2063 616e 2062  rage` flag can b
+000018d0: 6520 7573 6564 2074 6f20 7365 7420 6120  e used to set a 
+000018e0: 7468 7265 7368 6f6c 6420 666f 7220 636f  threshold for co
+000018f0: 6465 2063 6f76 6572 6167 6520 252e 2049  de coverage %. I
+00001900: 6620 7468 6520 636f 7665 7261 6765 2069  f the coverage i
+00001910: 7320 6c65 7373 2074 6861 6e20 7468 6973  s less than this
+00001920: 0a74 6872 6573 686f 6c64 2c20 7468 6520  .threshold, the 
+00001930: 6368 6563 6b20 7769 6c6c 2066 6169 6c2e  check will fail.
+00001940: 0a49 6620 6062 6164 6765 6020 6973 2073  .If `badge` is s
+00001950: 6574 2075 7369 6e67 2063 6c69 206f 7220  et using cli or 
+00001960: 746f 6d6c 2063 6f6e 6669 672c 2061 2053  toml config, a S
+00001970: 5647 2062 6164 6765 2077 6974 6820 7468  VG badge with th
+00001980: 6520 636f 7665 7261 6765 2025 2077 696c  e coverage % wil
+00001990: 6c20 6265 2067 656e 6572 6174 6564 2e0a  l be generated..
+000019a0: 5468 6973 2062 6164 6765 2063 616e 2062  This badge can b
+000019b0: 6520 7573 6564 2069 6e20 666f 7220 6578  e used in for ex
+000019c0: 616d 706c 6520 7468 6520 5245 4144 4d45  ample the README
+000019d0: 2e6d 642e 0a0a 2323 2320 436f 6e66 6967  .md...### Config
+000019e0: 7572 6174 696f 6e0a 0a49 6e20 796f 7572  uration..In your
+000019f0: 2060 7079 7072 6f6a 6563 742e 746f 6d6c   `pyproject.toml
+00001a00: 602c 2079 6f75 2063 616e 2061 6464 2061  `, you can add a
+00001a10: 2060 5b74 6f6f 6c73 2e73 7536 5d60 2073   `[tools.su6]` s
+00001a20: 6563 7469 6f6e 2074 6f20 636f 6e66 6967  ection to config
+00001a30: 7572 6520 736f 6d65 206f 6620 7468 6520  ure some of the 
+00001a40: 6265 6861 7669 6f72 206f 6620 7468 6973  behavior of this
+00001a50: 2074 6f6f 6c73 2e0a 4375 7272 656e 746c   tools..Currentl
+00001a60: 792c 2074 6865 2066 6f6c 6c6f 7769 6e67  y, the following
+00001a70: 206b 6579 7320 6172 6520 7375 7070 6f72   keys are suppor
+00001a80: 7465 643a 0a0a 6060 6074 6f6d 6c0a 5b74  ted:..```toml.[t
+00001a90: 6f6f 6c2e 7375 365d 0a64 6972 6563 746f  ool.su6].directo
+00001aa0: 7279 203d 2022 2e22 2023 2073 7472 696e  ry = "." # strin
+00001ab0: 6720 7061 7468 2074 6f20 7468 6520 6469  g path to the di
+00001ac0: 7265 6374 6f72 7920 6f6e 2077 6869 6368  rectory on which
+00001ad0: 2074 6f20 7275 6e20 616c 6c20 746f 6f6c   to run all tool
+00001ae0: 732c 2065 2e67 2e20 2773 7263 270a 696e  s, e.g. 'src'.in
+00001af0: 636c 7564 6520 3d20 5b5d 2023 206c 6973  clude = [] # lis
+00001b00: 7420 6f66 2063 6865 636b 7320 746f 2072  t of checks to r
+00001b10: 756e 2028 7768 656e 2063 616c 6c69 6e67  un (when calling
+00001b20: 2060 7375 3620 616c 6c60 292c 2065 2e67   `su6 all`), e.g
+00001b30: 2e20 5b27 626c 6163 6b27 2c20 276d 7970  . ['black', 'myp
+00001b40: 7927 5d0a 6578 636c 7564 6520 3d20 5b5d  y'].exclude = []
+00001b50: 2023 206c 6973 7420 6f66 2063 6865 636b   # list of check
+00001b60: 7320 746f 2073 6b69 7020 2877 6865 6e20  s to skip (when 
+00001b70: 6361 6c6c 696e 6720 6073 7536 2061 6c6c  calling `su6 all
+00001b80: 6029 2c20 652e 672e 205b 2762 616e 6469  `), e.g. ['bandi
+00001b90: 7427 5d0a 7374 6f70 2d61 6674 6572 2d66  t'].stop-after-f
+00001ba0: 6972 7374 2d66 6169 6c75 7265 203d 2066  irst-failure = f
+00001bb0: 616c 7365 2020 2320 626f 6f6c 2074 6f20  alse  # bool to 
+00001bc0: 696e 6469 6361 7465 2077 6865 7468 6572  indicate whether
+00001bd0: 2074 6f20 6578 6974 2027 616c 6c27 2061   to exit 'all' a
+00001be0: 6674 6572 206f 6e65 2066 6169 6c75 7265  fter one failure
+00001bf0: 206f 7220 746f 2064 6f20 616c 6c20 6368   or to do all ch
+00001c00: 6563 6b73 0a63 6f76 6572 6167 6520 3d20  ecks.coverage = 
+00001c10: 3130 3020 2320 696e 7420 7468 7265 7368  100 # int thresh
+00001c20: 6f6c 6420 666f 7220 7079 7465 7374 2063  old for pytest c
+00001c30: 6f76 6572 6167 6520 0a62 6164 6765 203d  overage .badge =
+00001c40: 2022 636f 7665 7261 6765 2e73 7667 2220   "coverage.svg" 
+00001c50: 2023 2073 7472 2070 6174 6820 6f72 2062   # str path or b
+00001c60: 6f6f 6c20 2874 7275 6520 7c20 6661 6c73  ool (true | fals
+00001c70: 6529 2077 6865 7468 6572 2061 6e64 2077  e) whether and w
+00001c80: 6865 7265 2074 6f20 6f75 7470 7574 2074  here to output t
+00001c90: 6865 2063 6f76 6572 6167 6520 6261 6467  he coverage badg
+00001ca0: 650a 6060 600a 0a41 6c6c 206b 6579 7320  e.```..All keys 
+00001cb0: 6172 6520 6f70 7469 6f6e 616c 2e20 4e6f  are optional. No
+00001cc0: 7465 2074 6861 7420 6966 2079 6f75 2068  te that if you h
+00001cd0: 6176 6520 626f 7468 2061 6e20 6069 6e63  ave both an `inc
+00001ce0: 6c75 6465 6020 6173 2077 656c 6c20 6173  lude` as well as
+00001cf0: 2061 6e20 6065 7863 6c75 6465 602c 2061   an `exclude`, a
+00001d00: 6c6c 2074 6865 2074 6f6f 6c73 2069 6e20  ll the tools in 
+00001d10: 6069 6e63 6c75 6465 6020 7769 6c6c 0a72  `include` will.r
+00001d20: 756e 2061 6e64 2060 6578 636c 7564 6560  un and `exclude`
+00001d30: 2077 696c 6c20 6265 2066 756c 6c79 2069   will be fully i
+00001d40: 676e 6f72 6564 2e20 200a 4164 6469 7469  gnored.  .Additi
+00001d50: 6f6e 616c 6c79 2c20 7468 6520 6f72 6465  onally, the orde
+00001d60: 7220 696e 2077 6869 6368 2074 6865 2063  r in which the c
+00001d70: 6865 636b 7320 6172 6520 6465 6669 6e65  hecks are define
+00001d80: 6420 696e 2027 696e 636c 7564 6527 2c20  d in 'include', 
+00001d90: 6973 2074 6865 206f 7264 6572 2069 6e20  is the order in 
+00001da0: 7768 6963 6820 7468 6579 2077 696c 6c20  which they will 
+00001db0: 7275 6e20 2869 6e20 6061 6c6c 600a 616e  run (in `all`.an
+00001dc0: 6420 6066 6978 6029 0a0a 2323 2320 4769  d `fix`)..### Gi
+00001dd0: 7468 7562 2041 6374 696f 6e0a 0a49 6e20  thub Action..In 
+00001de0: 6f72 6465 7220 746f 2075 7365 2074 6869  order to use thi
+00001df0: 7320 6368 6563 6b65 7220 7769 7468 696e  s checker within
+00001e00: 2047 6974 6875 6220 746f 2072 756e 2063   Github to run c
+00001e10: 6865 636b 7320 6166 7465 7220 7075 7368  hecks after push
+00001e20: 696e 672c 0a79 6f75 2063 616e 2061 6464  ing,.you can add
+00001e30: 2061 2077 6f72 6b66 6c6f 7720 2865 2e67   a workflow (e.g
+00001e40: 2e20 602e 6769 7468 7562 2f77 6f72 6b66  . `.github/workf
+00001e50: 6c6f 7773 2f73 7536 2e79 616d 6c60 2920  lows/su6.yaml`) 
+00001e60: 6c69 6b65 2074 6869 7320 6578 616d 706c  like this exampl
+00001e70: 653a 0a0a 6060 6079 616d 6c0a 6e61 6d65  e:..```yaml.name
+00001e80: 3a20 7275 6e20 7375 3620 6368 6563 6b73  : run su6 checks
+00001e90: 0a6f 6e3a 0a20 2070 7573 683a 0a20 2020  .on:.  push:.   
+00001ea0: 2062 7261 6e63 6865 732d 6967 6e6f 7265   branches-ignore
+00001eb0: 3a0a 2020 2020 2020 2d20 6d61 7374 6572  :.      - master
+00001ec0: 0a6a 6f62 733a 0a20 2063 6865 636b 3a0a  .jobs:.  check:.
+00001ed0: 2020 2020 6e61 6d65 3a20 4368 6563 6b20      name: Check 
+00001ee0: 7769 7468 2060 7375 3620 616c 6c60 0a20  with `su6 all`. 
+00001ef0: 2020 2072 756e 732d 6f6e 3a20 7562 756e     runs-on: ubun
+00001f00: 7475 2d6c 6174 6573 740a 2020 2020 7374  tu-latest.    st
+00001f10: 6570 733a 0a20 2020 2020 202d 2075 7365  eps:.      - use
+00001f20: 733a 2061 6374 696f 6e73 2f63 6865 636b  s: actions/check
+00001f30: 6f75 7440 7633 0a20 2020 2020 202d 2075  out@v3.      - u
+00001f40: 7365 733a 2061 6374 696f 6e73 2f73 6574  ses: actions/set
+00001f50: 7570 2d70 7974 686f 6e40 7634 0a20 2020  up-python@v4.   
+00001f60: 2020 2020 2077 6974 683a 0a20 2020 2020       with:.     
+00001f70: 2020 2020 2070 7974 686f 6e2d 7665 7273       python-vers
+00001f80: 696f 6e3a 2027 332e 3131 270a 2020 2020  ion: '3.11'.    
+00001f90: 2020 2020 2020 6361 6368 653a 2027 7069        cache: 'pi
+00001fa0: 7027 2023 2063 6163 6869 6e67 2070 6970  p' # caching pip
+00001fb0: 2064 6570 656e 6465 6e63 6965 730a 2020   dependencies.  
+00001fc0: 2020 2020 2d20 7275 6e3a 2070 6970 2069      - run: pip i
+00001fd0: 6e73 7461 6c6c 2073 7536 5b61 6c6c 5d20  nstall su6[all] 
+00001fe0: 2e0a 2020 2020 2020 2d20 7275 6e3a 2073  ..      - run: s
+00001ff0: 7536 2061 6c6c 0a60 6060 0a0a 2a2a 4e6f  u6 all.```..**No
+00002000: 7465 3a2a 2a20 6966 2079 6f75 2064 6f6e  te:** if you don
+00002010: 2774 2077 616e 7420 746f 2072 756e 2061  't want to run a
+00002020: 6c6c 2063 6865 636b 732c 2062 7574 2073  ll checks, but s
+00002030: 7065 6369 6669 6320 6f6e 6573 206f 6e6c  pecific ones onl
+00002040: 792c 2079 6f75 206e 6565 6420 746f 2061  y, you need to a
+00002050: 6464 2074 6865 2060 2d2d 6967 6e6f 7265  dd the `--ignore
+00002060: 2d75 6e69 6e73 7461 6c6c 6564 6020 666c  -uninstalled` fl
+00002070: 6167 0a74 6f20 6073 7536 2061 6c6c 6021  ag.to `su6 all`!
+00002080: 204f 7468 6572 7769 7365 2c20 4769 7468   Otherwise, Gith
+00002090: 7562 2077 696c 6c20 7365 6520 6578 6974  ub will see exit
+000020a0: 2063 6f64 6520 3132 3720 2863 6f6d 6d61   code 127 (comma
+000020b0: 6e64 206d 6973 7369 6e67 2920 6173 2061  nd missing) as a
+000020c0: 2066 6169 6c75 7265 2e0a 0a60 6060 7961   failure...```ya
+000020d0: 6d6c 0a6e 616d 653a 2072 756e 2073 6f6d  ml.name: run som
+000020e0: 6520 7375 3620 6368 6563 6b73 0a6f 6e3a  e su6 checks.on:
+000020f0: 0a20 2070 7573 683a 0a20 2020 2062 7261  .  push:.    bra
+00002100: 6e63 6865 732d 6967 6e6f 7265 3a0a 2020  nches-ignore:.  
+00002110: 2020 2020 2d20 6d61 7374 6572 0a6a 6f62      - master.job
+00002120: 733a 0a20 2063 6865 636b 3a0a 2020 2020  s:.  check:.    
+00002130: 6e61 6d65 3a20 4368 6563 6b20 7769 7468  name: Check with
+00002140: 2060 7375 3620 616c 6c60 0a20 2020 2072   `su6 all`.    r
+00002150: 756e 732d 6f6e 3a20 7562 756e 7475 2d6c  uns-on: ubuntu-l
+00002160: 6174 6573 740a 2020 2020 7374 6570 733a  atest.    steps:
+00002170: 0a20 2020 2020 202d 2075 7365 733a 2061  .      - uses: a
+00002180: 6374 696f 6e73 2f63 6865 636b 6f75 7440  ctions/checkout@
+00002190: 7633 0a20 2020 2020 202d 2075 7365 733a  v3.      - uses:
+000021a0: 2061 6374 696f 6e73 2f73 6574 7570 2d70   actions/setup-p
+000021b0: 7974 686f 6e40 7634 0a20 2020 2020 2020  ython@v4.       
+000021c0: 2077 6974 683a 0a20 2020 2020 2020 2020   with:.         
+000021d0: 2070 7974 686f 6e2d 7665 7273 696f 6e3a   python-version:
+000021e0: 2027 332e 3131 270a 2020 2020 2020 2020   '3.11'.        
+000021f0: 2020 6361 6368 653a 2027 7069 7027 2023    cache: 'pip' #
+00002200: 2063 6163 6869 6e67 2070 6970 2064 6570   caching pip dep
+00002210: 656e 6465 6e63 6965 730a 2020 2020 2020  endencies.      
+00002220: 2d20 7275 6e3a 2070 6970 2069 6e73 7461  - run: pip insta
+00002230: 6c6c 2073 7536 5b70 7963 6f64 6573 7479  ll su6[pycodesty
+00002240: 6c65 2c62 6c61 636b 5d20 2e0a 2020 2020  le,black] ..    
+00002250: 2020 2d20 7275 6e3a 2073 7536 2061 6c6c    - run: su6 all
+00002260: 202d 2d69 676e 6f72 652d 756e 696e 7374   --ignore-uninst
+00002270: 616c 6c65 6420 2023 202e 2e2e 206f 7468  alled  # ... oth
+00002280: 6572 2073 6574 7469 6e67 7320 7375 6368  er settings such
+00002290: 2061 7320 2d2d 7374 6f70 2d61 6674 6572   as --stop-after
+000022a0: 2d66 6972 7374 2d66 6169 6c75 7265 2c20  -first-failure, 
+000022b0: 2d2d 636f 7665 7261 6765 202e 2e2e 0a60  --coverage ....`
+000022c0: 6060 0a0a 2323 2050 6c75 6769 6e73 0a0a  ``..## Plugins..
+000022d0: 5468 6973 2074 6f6f 6c20 616c 736f 2073  This tool also s
+000022e0: 7570 706f 7274 7320 706c 7567 696e 7320  upports plugins 
+000022f0: 746f 2061 6464 2065 7874 7261 2063 6865  to add extra che
+00002300: 636b 6572 7320 6f72 206f 7468 6572 2066  ckers or other f
+00002310: 756e 6374 696f 6e61 6c69 7479 2e0a 5365  unctionality..Se
+00002320: 6520 5b64 6f63 732f 706c 7567 696e 732e  e [docs/plugins.
+00002330: 6d64 5d28 6874 7470 733a 2f2f 6769 7468  md](https://gith
+00002340: 7562 2e63 6f6d 2f72 6f62 696e 7661 6e64  ub.com/robinvand
+00002350: 6572 6e6f 6f72 642f 7375 362d 6368 6563  ernoord/su6-chec
+00002360: 6b65 722f 626c 6f62 2f6d 6173 7465 722f  ker/blob/master/
+00002370: 646f 6373 2f70 6c75 6769 6e73 2e6d 6429  docs/plugins.md)
+00002380: 0a0a 2323 204c 6963 656e 7365 0a0a 6073  ..## License..`s
+00002390: 7536 6020 6973 2064 6973 7472 6962 7574  u6` is distribut
+000023a0: 6564 2075 6e64 6572 2074 6865 2074 6572  ed under the ter
+000023b0: 6d73 206f 6620 7468 6520 5b4d 4954 5d28  ms of the [MIT](
+000023c0: 6874 7470 733a 2f2f 7370 6478 2e6f 7267  https://spdx.org
+000023d0: 2f6c 6963 656e 7365 732f 4d49 542e 6874  /licenses/MIT.ht
+000023e0: 6d6c 2920 6c69 6365 6e73 652e 0a0a 2323  ml) license...##
+000023f0: 2043 6861 6e67 656c 6f67 0a0a 5365 6520   Changelog..See 
+00002400: 6043 4841 4e47 454c 4f47 2e6d 6460 205b  `CHANGELOG.md` [
+00002410: 6f6e 2047 6974 4875 625d 2868 7474 7073  on GitHub](https
+00002420: 3a2f 2f67 6974 6875 622e 636f 6d2f 726f  ://github.com/ro
+00002430: 6269 6e76 616e 6465 726e 6f6f 7264 2f73  binvandernoord/s
+00002440: 7536 2d63 6865 636b 6572 2f62 6c6f 622f  u6-checker/blob/
+00002450: 6d61 7374 6572 2f43 4841 4e47 454c 4f47  master/CHANGELOG
+00002460: 2e6d 6429 0a                             .md).
```

