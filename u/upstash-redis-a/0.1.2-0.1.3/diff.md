# Comparing `tmp/upstash_redis_a-0.1.2.tar.gz` & `tmp/upstash_redis_a-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis_a-0.1.2.tar", max compression
+gzip compressed data, was "upstash_redis_a-0.1.3.tar", max compression
```

## Comparing `upstash_redis_a-0.1.2.tar` & `upstash_redis_a-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis_a-0.1.2/LICENSE
--rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis_a-0.1.2/README.md
--rw-r--r--   0        0        0      388 2023-06-19 01:31:20.512293 upstash_redis_a-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-06-18 23:12:23.109932 upstash_redis_a-0.1.2/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-06-18 23:12:23.110093 upstash_redis_a-0.1.2/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0    84480 2023-06-19 01:12:18.616114 upstash_redis_a-0.1.2/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis_a-0.1.2/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis_a-0.1.2/upstash_redis/exception.py
--rw-r--r--   0        0        0      810 2023-06-18 23:12:23.110853 upstash_redis_a-0.1.2/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     3193 2023-06-19 01:31:04.187754 upstash_redis_a-0.1.2/upstash_redis/http/execute.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:37.096890 upstash_redis_a-0.1.2/upstash_redis/py.typed
--rw-r--r--   0        0        0      431 2023-06-19 00:14:29.039876 upstash_redis_a-0.1.2/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1162 2023-06-19 00:16:53.116217 upstash_redis_a-0.1.2/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      746 2023-06-19 00:53:00.198997 upstash_redis_a-0.1.2/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis_a-0.1.2/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis_a-0.1.2/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis_a-0.1.2/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-06-19 00:09:55.671307 upstash_redis_a-0.1.2/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     3975 2023-06-19 01:29:27.403905 upstash_redis_a-0.1.2/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9702 1970-01-01 00:00:00.000000 upstash_redis_a-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis_a-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis_a-0.1.3/README.md
+-rw-r--r--   0        0        0      388 2023-06-19 01:59:41.682445 upstash_redis_a-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-06-18 23:12:23.109932 upstash_redis_a-0.1.3/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-18 23:12:23.110093 upstash_redis_a-0.1.3/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0    84492 2023-06-19 01:59:04.278103 upstash_redis_a-0.1.3/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis_a-0.1.3/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis_a-0.1.3/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-06-19 01:44:49.341538 upstash_redis_a-0.1.3/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     3205 2023-06-19 01:48:51.048556 upstash_redis_a-0.1.3/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:37.096890 upstash_redis_a-0.1.3/upstash_redis/py.typed
+-rw-r--r--   0        0        0      431 2023-06-19 00:14:29.039876 upstash_redis_a-0.1.3/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1174 2023-06-19 01:49:10.086585 upstash_redis_a-0.1.3/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-06-19 01:44:21.139360 upstash_redis_a-0.1.3/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis_a-0.1.3/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis_a-0.1.3/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis_a-0.1.3/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-06-19 00:09:55.671307 upstash_redis_a-0.1.3/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     3987 2023-06-19 01:48:34.322720 upstash_redis_a-0.1.3/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9702 1970-01-01 00:00:00.000000 upstash_redis_a-0.1.3/PKG-INFO
```

### Comparing `upstash_redis_a-0.1.2/LICENSE` & `upstash_redis_a-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.2/README.md` & `upstash_redis_a-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.2/upstash_redis/asyncio/client.py` & `upstash_redis_a-0.1.3/upstash_redis/asyncio/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     FormattedGeoMembersReturn,
     HashReturn,
     FormattedHashReturn,
     SortedSetReturn,
     FormattedSortedSetReturn,
 )
 from aiohttp import ClientSession
-from typing import Type, Any, Literal, Union
+from typing import Type, Any, Literal, Union, List, Dict
 from os import environ
 
 
 class Redis:
     def __init__(
         self,
         url: str,
@@ -139,15 +139,15 @@
     ) -> None:
         """
         Exit the async context.
         """
 
         await self._session.close()
 
-    async def run(self, command: list) -> RESTResult:
+    async def run(self, command: List) -> RESTResult:
         """
         Specify the http options and execute the command.
         """
 
         return await execute(
             session=self._session,
             url=self.url,
@@ -166,15 +166,15 @@
         """
         See https://redis.io/commands/bitcount
         """
 
         if number_are_not_none(start, end, number=1):
             raise Exception('Both "start" and "end" must be specified.')
 
-        command: list = ["BITCOUNT", key]
+        command: List = ["BITCOUNT", key]
 
         if start is not None:
             command.extend([start, end])
 
         return await self.run(command)
 
     def bitfield(self, key: str) -> "BitFieldCommands":
@@ -202,15 +202,15 @@
             raise Exception("At least one source key must be specified.")
 
         if operation == "NOT" and len(srckeys) > 1:
             raise Exception(
                 'The "NOT " operation takes only one source key as argument.'
             )
 
-        command: list = ["BITOP", operation, destkey, *srckeys]
+        command: List = ["BITOP", operation, destkey, *srckeys]
 
         return await self.run(command)
 
     async def bitpos(
         self,
         key: str,
         bit: Literal[0, 1],
@@ -220,73 +220,73 @@
         """
         See https://redis.io/commands/bitpos
         """
 
         if start is None and end is not None:
             raise Exception('"end" is specified, but "start" is missing.')
 
-        command: list = ["BITPOS", key, bit]
+        command: List = ["BITPOS", key, bit]
 
         if start is not None:
             command.append(start)
 
         if end is not None:
             command.append(end)
 
         return await self.run(command)
 
     async def getbit(self, key: str, offset: int) -> int:
         """
         See https://redis.io/commands/getbit
         """
 
-        command: list = ["GETBIT", key, offset]
+        command: List = ["GETBIT", key, offset]
 
         return await self.run(command)
 
     async def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int:
         """
         See https://redis.io/commands/setbit
         """
 
-        command: list = ["SETBIT", key, offset, value]
+        command: List = ["SETBIT", key, offset, value]
 
         return await self.run(command)
 
     async def ping(self, message: Union[str, None] = None) -> str:
         """
         See https://redis.io/commands/ping
         """
 
-        command: list = ["PING"]
+        command: List = ["PING"]
 
         if message is not None:
             command.append(message)
 
         return await self.run(command)
 
     async def echo(self, message: str) -> str:
         """
         See https://redis.io/commands/echo
         """
 
-        command: list = ["ECHO", message]
+        command: List = ["ECHO", message]
 
         return await self.run(command)
 
     async def copy(
         self, source: str, destination: str, replace: bool = False
     ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/copy
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["COPY", source, destination]
+        command: List = ["COPY", source, destination]
 
         if replace:
             command.append("REPLACE")
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -295,252 +295,252 @@
         """
         See https://redis.io/commands/del
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be deleted.")
 
-        command: list = ["DEL", *keys]
+        command: List = ["DEL", *keys]
 
         return await self.run(command)
 
     async def exists(self, *keys: str) -> int:
         """
         See https://redis.io/commands/exists
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be checked.")
 
-        command: list = ["EXISTS", *keys]
+        command: List = ["EXISTS", *keys]
 
         return await self.run(command)
 
     async def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/expire
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["EXPIRE", key, seconds]
+        command: List = ["EXPIRE", key, seconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def expireat(
         self, key: str, unix_time_seconds: int
     ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/expireat
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["EXPIREAT", key, unix_time_seconds]
+        command: List = ["EXPIREAT", key, unix_time_seconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def keys(self, pattern: str) -> list[str]:
+    async def keys(self, pattern: str) -> List[str]:
         """
         See https://redis.io/commands/keys
         """
 
-        command: list = ["KEYS", pattern]
+        command: List = ["KEYS", pattern]
 
         return await self.run(command)
 
     async def persist(self, key: str) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/persist
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PERSIST", key]
+        command: List = ["PERSIST", key]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pexpire(self, key: str, milliseconds: int) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/pexpire
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PEXPIRE", key, milliseconds]
+        command: List = ["PEXPIRE", key, milliseconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pexpireat(
         self, key: str, unix_time_milliseconds: int
     ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/pexpireat
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PEXPIREAT", key, unix_time_milliseconds]
+        command: List = ["PEXPIREAT", key, unix_time_milliseconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pttl(self, key: str) -> int:
         """
         See https://redis.io/commands/pttl
         """
 
-        command: list = ["PTTL", key]
+        command: List = ["PTTL", key]
 
         return await self.run(command)
 
     async def randomkey(self) -> Union[str, None]:
         """
         See https://redis.io/commands/randomkey
         """
 
-        command: list = ["RANDOMKEY"]
+        command: List = ["RANDOMKEY"]
 
         return await self.run(command)
 
     async def rename(self, key: str, newkey: str) -> str:
         """
         See https://redis.io/commands/rename
         """
 
-        command: list = ["RENAME", key, newkey]
+        command: List = ["RENAME", key, newkey]
 
         return await self.run(command)
 
     async def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/renamenx
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["RENAMENX", key, newkey]
+        command: List = ["RENAMENX", key, newkey]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def scan(
         self,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         scan_type: Union[str, None] = None,
         return_cursor: bool = True,
     ) -> Union[
-        (Union[list[Union[str, list[str]]], list[Union[int, list[str]]]]), list[str]
+        (Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]), List[str]
     ]:
         """
         See https://redis.io/commands/scan
 
         :param return_cursor: if set to False, it won't return the cursor
 
         :param scan_type: replacement for "TYPE"
         :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only the list of elements will be returned if "return_cursor" is False
+        Only the List of elements will be returned if "return_cursor" is False
         """
 
-        command: list = ["SCAN", cursor]
+        command: List = ["SCAN", cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         if scan_type is not None:
             command.extend(["TYPE", scan_type])
 
-        # The raw result is composed of the new cursor and the list of elements.
-        raw: list[Union[str, list[str]]] = await self.run(command)
+        # The raw result is composed of the new cursor and the List of elements.
+        raw: List[Union[str, List[str]]] = await self.run(command)
 
         if return_cursor:
             return [int(raw[0]), raw[1]] if self.format_return else raw
 
         return raw[1]
 
     async def touch(self, *keys: str) -> int:
         """
         See https://redis.io/commands/touch
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["TOUCH", *keys]
+        command: List = ["TOUCH", *keys]
 
         return await self.run(command)
 
     async def ttl(self, key: str) -> int:
         """
         See https://redis.io/commands/ttl
         """
 
-        command: list = ["TTL", key]
+        command: List = ["TTL", key]
 
         return await self.run(command)
 
     async def type(self, key: str) -> Union[str, None]:
         """
         See https://redis.io/commands/type
         """
 
-        command: list = ["TYPE", key]
+        command: List = ["TYPE", key]
 
         return await self.run(command)
 
     async def unlink(self, *keys: str) -> int:
         """
         See https://redis.io/commands/unlink
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["UNLINK", *keys]
+        command: List = ["UNLINK", *keys]
 
         return await self.run(command)
 
     async def geoadd(
         self,
         key: str,
         *members: GeoMember,
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
     ) -> int:
         """
         See https://redis.io/commands/geoadd
 
-        :param members: a sequence of GeoMember dict types (longitude, latitude, name).
+        :param members: a sequence of GeoMember Dict types (longitude, latitude, name).
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
 
-        command: list = ["GEOADD", key]
+        command: List = ["GEOADD", key]
 
         if nx:
             command.append("NX")
 
         if xx:
             command.append("XX")
 
@@ -561,41 +561,41 @@
     ) -> Union[str, float, None]:
         """
         See https://redis.io/commands/geodist
 
         :return: A float value if "format_return" is True.
         """
 
-        command: list = ["GEODIST", key, member1, member2, unit]
+        command: List = ["GEODIST", key, member1, member2, unit]
 
         raw: Union[str, None] = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
-    async def geohash(self, key: str, *members: str) -> list[Union[str, None]]:
+    async def geohash(self, key: str, *members: str) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/geohash
         """
 
-        command: list = ["GEOHASH", key, *members]
+        command: List = ["GEOHASH", key, *members]
 
         return await self.run(command)
 
     async def geopos(
         self, key: str, *members: str
-    ) -> Union[list[Union[list[str], None]], list[Union[dict[str, float], None]]]:
+    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]:
         """
         See https://redis.io/commands/geopos
 
-        :return: A list of dicts with either None or the longitude and latitude if "format_return" is True.
+        :return: A List of Dicts with either None or the longitude and latitude if "format_return" is True.
         """
 
-        command: list = ["GEOPOS", key, *members]
+        command: List = ["GEOPOS", key, *members]
 
-        raw: list[Union[list[str], None]] = await self.run(command)
+        raw: List[Union[List[str], None]] = await self.run(command)
 
         return format_geo_positions_return(raw) if self.format_return else raw
 
     async def georadius(
         self,
         key: str,
         longitude: float,
@@ -612,22 +612,22 @@
         storedist: Union[str, None] = None,
     ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn, int]:
         """
         See https://redis.io/commands/georadius
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         handle_georadius_write_exceptions(
             withdist, withhash, withcoord, count, count_any, store, storedist
         )
 
-        command: list = ["GEORADIUS", key, longitude, latitude, radius, unit]
+        command: List = ["GEORADIUS", key, longitude, latitude, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
@@ -646,15 +646,15 @@
             command.extend(["STORE", store])
 
         if storedist:
             command.extend(["STOREDIST", storedist])
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
+        # If none of the additional properties are requested, the result will be "List[str]".
         if self.format_return and (withdist or withhash or withcoord):
             return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def georadius_ro(
         self,
@@ -671,21 +671,21 @@
         sort: Union[Literal["ASC", "DESC"], None] = None,
     ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/georadius_ro
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         if count_any and count is None:
             raise Exception('"count_any" can only be used together with "count".')
 
-        command: list = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
+        command: List = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
@@ -698,15 +698,15 @@
                 command.append("ANY")
 
         if sort:
             command.append(sort)
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
+        # If none of the additional properties are requested, the result will be "List[str]".
         if self.format_return and (withdist or withhash or withcoord):
             return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def georadiusbymember(
         self,
@@ -724,22 +724,22 @@
         storedist: Union[str, None] = None,
     ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/georadiusbymember
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         handle_georadius_write_exceptions(
             withdist, withhash, withcoord, count, count_any, store, storedist
         )
 
-        command: list = ["GEORADIUSBYMEMBER", key, member, radius, unit]
+        command: List = ["GEORADIUSBYMEMBER", key, member, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
@@ -758,15 +758,15 @@
             command.extend(["STORE", store])
 
         if storedist:
             command.extend(["STOREDIST", storedist])
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
+        # If none of the additional properties are requested, the result will be "List[str]".
         if self.format_return and (withdist or withhash or withcoord):
             return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def georadiusbymember_ro(
         self,
@@ -782,21 +782,21 @@
         sort: Union[Literal["ASC", "DESC"], None] = None,
     ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/georadiusbymember_ro
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         if count_any and count is None:
             raise Exception('"count_any" can only be used together with "count".')
 
-        command: list = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
+        command: List = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
 
         if withdist:
             command.append("WITHDIST")
 
         if withhash:
             command.append("WITHHASH")
 
@@ -809,15 +809,15 @@
                 command.append("ANY")
 
         if sort:
             command.append(sort)
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
+        # If none of the additional properties are requested, the result will be "List[str]".
         if self.format_return and (withdist or withhash or withcoord):
             return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def geosearch(
         self,
@@ -837,29 +837,29 @@
         withcoord: bool = False,
     ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/geosearch
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         handle_geosearch_exceptions(
             frommember,
             fromlonlat_longitude,
             fromlonlat_latitude,
             byradius,
             bybox_width,
             bybox_height,
             count,
             count_any,
         )
 
-        command: list = ["GEOSEARCH", key]
+        command: List = ["GEOSEARCH", key]
 
         if frommember is not None:
             command.extend(["FROMMEMBER", frommember])
 
         if fromlonlat_longitude is not None:
             command.extend(["FROMLONLAT", fromlonlat_longitude, fromlonlat_latitude])
 
@@ -886,15 +886,15 @@
             command.append("WITHHASH")
 
         if withcoord:
             command.append("WITHCOORD")
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
+        # If none of the additional properties are requested, the result will be "List[str]".
         if self.format_return and (withdist or withhash or withcoord):
             return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def geosearchstore(
         self,
@@ -925,15 +925,15 @@
             byradius,
             bybox_width,
             bybox_height,
             count,
             count_any,
         )
 
-        command: list = ["GEOSEARCHSTORE", destination, source]
+        command: List = ["GEOSEARCHSTORE", destination, source]
 
         if frommember is not None:
             command.extend(["FROMMEMBER", frommember])
 
         if fromlonlat_longitude is not None:
             command.extend(["FROMLONLAT", fromlonlat_longitude, fromlonlat_latitude])
 
@@ -962,132 +962,132 @@
         """
         See https://redis.io/commands/hdel
         """
 
         if len(fields) == 0:
             raise Exception("At least one field must be deleted.")
 
-        command: list = ["HDEL", key, *fields]
+        command: List = ["HDEL", key, *fields]
 
         return await self.run(command)
 
     async def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/hexists
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["HEXISTS", key, field]
+        command: List = ["HEXISTS", key, field]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def hget(self, key: str, field: str) -> Union[str, None]:
         """
         See https://redis.io/commands/hget
         """
 
-        command: list = ["HGET", key, field]
+        command: List = ["HGET", key, field]
 
         return await self.run(command)
 
     async def hgetall(self, key: str) -> Union[HashReturn, FormattedHashReturn]:
         """
         See https://redis.io/commands/hgetall
 
-        :return: A dict of field-value pairs if "format_return" is True.
+        :return: A Dict of field-value pairs if "format_return" is True.
         """
 
-        command: list = ["HGETALL", key]
+        command: List = ["HGETALL", key]
 
         raw: HashReturn = await self.run(command)
 
         return format_hash_return(raw) if self.format_return else raw
 
     async def hincrby(self, key: str, field: str, increment: int) -> int:
         """
         See https://redis.io/commands/hincrby
         """
 
-        command: list = ["HINCRBY", key, field, increment]
+        command: List = ["HINCRBY", key, field, increment]
 
         return await self.run(command)
 
     async def hincrbyfloat(
         self, key: str, field: str, increment: float
     ) -> Union[str, float]:
         """
         See https://redis.io/commands/hincrbyfloat
 
         :return: A float if "format_return" is True.
         """
 
-        command: list = ["HINCRBYFLOAT", key, field, increment]
+        command: List = ["HINCRBYFLOAT", key, field, increment]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
-    async def hkeys(self, key: str) -> list[str]:
+    async def hkeys(self, key: str) -> List[str]:
         """
         See https://redis.io/commands/hkeys
         """
 
-        command: list = ["HKEYS", key]
+        command: List = ["HKEYS", key]
 
         return await self.run(command)
 
     async def hlen(self, key: str) -> int:
         """
         See https://redis.io/commands/hlen
         """
 
-        command: list = ["HLEN", key]
+        command: List = ["HLEN", key]
 
         return await self.run(command)
 
-    async def hmget(self, key: str, *fields: str) -> list[Union[str, None]]:
+    async def hmget(self, key: str, *fields: str) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/hmget
         """
 
         if len(fields) == 0:
             raise Exception("At least one field must be specified.")
 
-        command: list = ["HMGET", key, *fields]
+        command: List = ["HMGET", key, *fields]
 
         return await self.run(command)
 
-    async def hmset(self, key: str, field_value_pairs: dict) -> str:
+    async def hmset(self, key: str, field_value_pairs: Dict) -> str:
         """
         See https://redis.io/commands/hmset
         """
 
-        command: list = ["HMSET", key]
+        command: List = ["HMSET", key]
 
         for field, value in field_value_pairs.items():
             command.extend([field, value])
 
         return await self.run(command)
 
     async def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
     ) -> Union[(Union[str, None]), Union[HashReturn, FormattedHashReturn]]:
         """
         See https://redis.io/commands/hrandfield
 
-        :return: A dict of field-value pairs if "count" and "withvalues" are specified and "format_return" is True.
+        :return: A Dict of field-value pairs if "count" and "withvalues" are specified and "format_return" is True.
         """
 
         if count is None and withvalues:
             raise Exception('"withvalues" can only be used together with "count"')
 
-        command: list = ["HRANDFIELD", key]
+        command: List = ["HRANDFIELD", key]
 
         if count is not None:
             command.extend(["COUNT", count])
 
             if withvalues:
                 command.append("WITHVALUES")
 
@@ -1101,51 +1101,51 @@
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         return_cursor: bool = True,
     ) -> Union[
-        (Union[list[Union[str, HashReturn]], list[Union[int, FormattedHashReturn]]]),
+        (Union[List[Union[str, HashReturn]], List[Union[int, FormattedHashReturn]]]),
         (Union[HashReturn, FormattedHashReturn]),
     ]:
         """
         See https://redis.io/commands/hscan
 
         :param return_cursor: if set to False, it won't return the cursor
         :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only a dict of field-value pairs will be returned if "return_cursor" is False and "format_return" is True.
+        Only a Dict of field-value pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
-        command: list = ["HSCAN", key, cursor]
+        command: List = ["HSCAN", key, cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        # The raw result is composed of the new cursor and the list of elements.
-        raw: Union[list[Union[str, HashReturn]], HashReturn] = await self.run(command)
+        # The raw result is composed of the new cursor and the List of elements.
+        raw: Union[List[Union[str, HashReturn]], HashReturn] = await self.run(command)
 
         if return_cursor:
             return (
                 [int(raw[0]), format_hash_return(raw[1])] if self.format_return else raw
             )
 
         return format_hash_return(raw[1]) if self.format_return else raw[1]
 
-    async def hset(self, key: str, field_value_pairs: dict) -> int:
+    async def hset(self, key: str, field_value_pairs: Dict) -> int:
         """
         See https://redis.io/commands/hset
         """
 
-        command: list = ["HSET", key]
+        command: List = ["HSET", key]
 
         for field, value in field_value_pairs.items():
             command.extend([field, value])
 
         return await self.run(command)
 
     async def hsetnx(
@@ -1153,151 +1153,151 @@
     ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/hsetnx
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["HSETNX", key, field, value]
+        command: List = ["HSETNX", key, field, value]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def hstrlen(self, key: str, field: str) -> int:
         """
         See https://redis.io/commands/hstrlen
         """
 
-        command: list = ["HSTRLEN", key, field]
+        command: List = ["HSTRLEN", key, field]
 
         return await self.run(command)
 
-    async def hvals(self, key: str) -> list[str]:
+    async def hvals(self, key: str) -> List[str]:
         """
         See https://redis.io/commands/hvals
         """
 
-        command: list = ["HVALS", key]
+        command: List = ["HVALS", key]
 
         return await self.run(command)
 
     async def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/pfadd
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PFADD", key, *elements]
+        command: List = ["PFADD", key, *elements]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pfcount(self, *keys: str) -> int:
         """
         See https://redis.io/commands/pfcount
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["PFCOUNT", *keys]
+        command: List = ["PFCOUNT", *keys]
 
         return await self.run(command)
 
     async def pfmerge(self, destkey: str, *sourcekeys: str) -> str:
         """
         See https://redis.io/commands/pfmerge
         """
 
-        command: list = ["PFMERGE", destkey, *sourcekeys]
+        command: List = ["PFMERGE", destkey, *sourcekeys]
 
         return await self.run(command)
 
     async def lindex(self, key: str, index: int) -> Union[str, None]:
         """
         See https://redis.io/commands/lindex
         """
 
-        command: list = ["LINDEX", key, index]
+        command: List = ["LINDEX", key, index]
 
         return await self.run(command)
 
     async def linsert(
         self, key: str, position: Literal["BEFORE", "AFTER"], pivot: Any, element: Any
     ) -> int:
         """
         See https://redis.io/commands/linsert
         """
 
-        command: list = ["LINSERT", key, position, pivot, element]
+        command: List = ["LINSERT", key, position, pivot, element]
 
         return await self.run(command)
 
     async def llen(self, key: str) -> int:
         """
         See https://redis.io/commands/llen
         """
 
-        command: list = ["LLEN", key]
+        command: List = ["LLEN", key]
 
         return await self.run(command)
 
     async def lmove(
         self,
         source: str,
         destination: str,
         source_position: Literal["LEFT", "RIGHT"],
         destination_position: Literal["LEFT", "RIGHT"],
     ) -> Union[str, None]:
         """
         See https://redis.io/commands/lmove
         """
 
-        command: list = [
+        command: List = [
             "LMOVE",
             source,
             destination,
             source_position,
             destination_position,
         ]
 
         return await self.run(command)
 
     async def lpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), list[str]]:
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/lpop
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["LPOP", key]
+        command: List = ["LPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def lpos(
         self,
         key: str,
         element: Any,
         rank: Union[int, None] = None,
         count: Union[int, None] = None,
         maxlen: Union[int, None] = None,
-    ) -> Union[(Union[int, None]), list[int]]:
+    ) -> Union[(Union[int, None]), List[int]]:
         """
         See https://redis.io/commands/lpos
         """
 
-        command: list = ["LPOS", key, element]
+        command: List = ["LPOS", key, element]
 
         if rank is not None:
             command.extend(["RANK", rank])
 
         if count is not None:
             command.extend(["COUNT", count])
 
@@ -1310,161 +1310,161 @@
         """
         See https://redis.io/commands/lpush
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["LPUSH", key, *elements]
+        command: List = ["LPUSH", key, *elements]
 
         return await self.run(command)
 
     async def lpushx(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/lpushx
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["LPUSHX", key, *elements]
+        command: List = ["LPUSHX", key, *elements]
 
         return await self.run(command)
 
-    async def lrange(self, key: str, start: int, stop: int) -> list[str]:
+    async def lrange(self, key: str, start: int, stop: int) -> List[str]:
         """
         See https://redis.io/commands/lrange
         """
 
-        command: list = ["LRANGE", key, start, stop]
+        command: List = ["LRANGE", key, start, stop]
 
         return await self.run(command)
 
     async def lrem(self, key: str, count: int, element: Any) -> int:
         """
         See https://redis.io/commands/lrem
         """
 
-        command: list = ["LREM", key, count, element]
+        command: List = ["LREM", key, count, element]
 
         return await self.run(command)
 
     async def lset(self, key: str, index: int, element: Any) -> str:
         """
         See https://redis.io/commands/lset
         """
 
-        command: list = ["LSET", key, index, element]
+        command: List = ["LSET", key, index, element]
 
         return await self.run(command)
 
     async def ltrim(self, key: str, start: int, stop: int) -> str:
         """
         See https://redis.io/commands/ltrim
         """
 
-        command: list = ["LTRIM", key, start, stop]
+        command: List = ["LTRIM", key, start, stop]
 
         return await self.run(command)
 
     async def rpop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), list[str]]:
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/rpop
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["RPOP", key]
+        command: List = ["RPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def rpoplpush(self, source: str, destination: str) -> Union[str, None]:
         """
         See https://redis.io/commands/rpoplpush
         """
 
-        command: list = ["RPOPLPUSH", source, destination]
+        command: List = ["RPOPLPUSH", source, destination]
 
         return await self.run(command)
 
     async def rpush(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/rpush
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["RPUSH", key, *elements]
+        command: List = ["RPUSH", key, *elements]
 
         return await self.run(command)
 
     async def rpushx(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/rpushx
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["RPUSHX", key, *elements]
+        command: List = ["RPUSHX", key, *elements]
 
         return await self.run(command)
 
     async def publish(self, channel: str, message: str) -> int:
         """
         See https://redis.io/commands/publish
         """
 
-        command: list = ["PUBLISH", channel, message]
+        command: List = ["PUBLISH", channel, message]
 
         return await self.run(command)
 
     async def eval(
         self,
         script: str,
-        keys: Union[list[str], None] = None,
-        args: Union[list, None] = None,
+        keys: Union[List[str], None] = None,
+        args: Union[List, None] = None,
     ) -> Any:
         """
         See https://redis.io/commands/eval
 
         The number of keys is calculated automatically.
         """
 
-        command: list = ["EVAL", script]
+        command: List = ["EVAL", script]
 
         if keys is not None:
             command.extend([len(keys), *keys])
         else:
             command.append(0)
 
         if args:
             command.extend(args)
 
         return await self.run(command)
 
     async def evalsha(
         self,
         sha1: str,
-        keys: Union[list[str], None] = None,
-        args: Union[list, None] = None,
+        keys: Union[List[str], None] = None,
+        args: Union[List, None] = None,
     ) -> Any:
         """
         See https://redis.io/commands/evalsha
 
         The number of keys is calculated automatically.
         """
 
-        command: list = ["EVALSHA", sha1]
+        command: List = ["EVALSHA", sha1]
 
         if keys is not None:
             command.extend([len(keys), *keys])
         else:
             command.append(0)
 
         if args:
@@ -1473,295 +1473,295 @@
         return await self.run(command)
 
     async def dbsize(self) -> int:
         """
         See https://redis.io/commands/dbsize
         """
 
-        command: list = ["DBSIZE"]
+        command: List = ["DBSIZE"]
 
         return await self.run(command)
 
     async def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
         """
         See https://redis.io/commands/flushall
         """
 
-        command: list = ["FLUSHALL"]
+        command: List = ["FLUSHALL"]
 
         if mode:
             command.append(mode)
 
         return await self.run(command)
 
     async def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
         """
         See https://redis.io/commands/flushdb
         """
 
-        command: list = ["FLUSHDB"]
+        command: List = ["FLUSHDB"]
 
         if mode:
             command.append(mode)
 
         return await self.run(command)
 
-    async def time(self) -> Union[list[str], dict[str, int]]:
+    async def time(self) -> Union[List[str], Dict[str, int]]:
         """
         See https://redis.io/commands/time
 
-        :return: A dict with the keys "seconds" and "microseconds" if self.format_return is True.
+        :return: A Dict with the keys "seconds" and "microseconds" if self.format_return is True.
         """
 
-        command: list = ["TIME"]
+        command: List = ["TIME"]
 
-        raw: list[str] = await self.run(command)
+        raw: List[str] = await self.run(command)
 
         return format_server_time_return(raw) if self.format_return else raw
 
     async def sadd(self, key: str, *members: Any) -> int:
         """
         See https://redis.io/commands/sadd
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
-        command: list = ["SADD", key, *members]
+        command: List = ["SADD", key, *members]
 
         return await self.run(command)
 
     async def scard(self, key: str) -> int:
         """
         See https://redis.io/commands/scard
         """
 
-        command: list = ["SCARD", key]
+        command: List = ["SCARD", key]
 
         return await self.run(command)
 
-    async def sdiff(self, *keys: str) -> list[str]:
+    async def sdiff(self, *keys: str) -> List[str]:
         """
         See https://redis.io/commands/sdiff
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SDIFF", *keys]
+        command: List = ["SDIFF", *keys]
 
         return await self.run(command)
 
     async def sdiffstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/sdiffstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SDIFFSTORE", destination, *keys]
+        command: List = ["SDIFFSTORE", destination, *keys]
 
         return await self.run(command)
 
-    async def sinter(self, *keys: str) -> list[str]:
+    async def sinter(self, *keys: str) -> List[str]:
         """
         See https://redis.io/commands/sinter
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SINTER", *keys]
+        command: List = ["SINTER", *keys]
 
         return await self.run(command)
 
     async def sinterstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/sinterstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SINTERSTORE", destination, *keys]
+        command: List = ["SINTERSTORE", destination, *keys]
 
         return await self.run(command)
 
     async def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/sismember
 
         :return: A bool if self.format_return is True.
         """
 
-        command: list = ["SISMEMBER", key, member]
+        command: List = ["SISMEMBER", key, member]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def smembers(self, key: str) -> list[str]:
+    async def smembers(self, key: str) -> List[str]:
         """
         See https://redis.io/commands/smembers
         """
 
-        command: list = ["SMEMBERS", key]
+        command: List = ["SMEMBERS", key]
 
         return await self.run(command)
 
     async def smove(
         self, source: str, destination: str, member: Any
     ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/smove
 
         :return: A bool if self.format_return is True.
         """
 
-        command: list = ["SMOVE", source, destination, member]
+        command: List = ["SMOVE", source, destination, member]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def spop(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), list[str]]:
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/spop
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["SPOP", key]
+        command: List = ["SPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def srandmember(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[(Union[str, None]), list[str]]:
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/srandmember
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["SRANDMEMBER", key]
+        command: List = ["SRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def srem(self, key: str, *members: Any) -> int:
         """
         See https://redis.io/commands/srem
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
-        command: list = ["SREM", key, *members]
+        command: List = ["SREM", key, *members]
 
         return await self.run(command)
 
     async def sscan(
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         return_cursor: bool = True,
     ) -> Union[
-        (Union[list[Union[str, list[str]]], list[Union[int, list[str]]]]), list[str]
+        (Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]), List[str]
     ]:
         """
         See https://redis.io/commands/sscan
 
         :param return_cursor: if set to False, it won't return the cursor
         :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only the list of elements will be returned if "return_cursor" is False.
+        Only the List of elements will be returned if "return_cursor" is False.
         """
 
-        command: list = ["SSCAN", key, cursor]
+        command: List = ["SSCAN", key, cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        # The raw result is composed of the new cursor and the list of elements.
-        raw: list[Union[str, list[str]]] = await self.run(command)
+        # The raw result is composed of the new cursor and the List of elements.
+        raw: List[Union[str, List[str]]] = await self.run(command)
 
         if return_cursor:
             return [int(raw[0]), raw[1]] if self.format_return else raw
 
         return raw[1]
 
-    async def sunion(self, *keys: str) -> list[str]:
+    async def sunion(self, *keys: str) -> List[str]:
         """
         See https://redis.io/commands/sunion
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SUNION", *keys]
+        command: List = ["SUNION", *keys]
 
         return await self.run(command)
 
     async def sunionstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/sunionstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SUNIONSTORE", destination, *keys]
+        command: List = ["SUNIONSTORE", destination, *keys]
 
         return await self.run(command)
 
     async def zadd(
         self,
         key: str,
-        score_member_pairs: dict,
+        score_member_pairs: Dict,
         nx: bool = False,
         xx: bool = False,
         gt: bool = False,
         lt: bool = False,
         ch: bool = False,
         incr: bool = False,
     ) -> Union[int, (Union[str, None, float])]:
         """
         See https://redis.io/commands/zadd
 
-        :param score_member_pairs: a dict containing members and their scores.
+        :param score_member_pairs: a Dict containing members and their scores.
 
         :return: A float representing the number of elements added or None if "incr" is False
         and "format_return" is True.
         """
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
 
         if gt and lt:
             raise Exception('"gt" and "lt" are mutually exclusive.')
 
         if nx and (gt or lt):
             raise Exception('"nx" and "gt" or "lt" are mutually exclusive.')
 
-        command: list = ["ZADD", key]
+        command: List = ["ZADD", key]
 
         if nx:
             command.append("NX")
 
         if xx:
             command.append("XX")
 
@@ -1790,15 +1790,15 @@
         return await self.run(command)
 
     async def zcard(self, key: str) -> int:
         """
         See https://redis.io/commands/zcard
         """
 
-        command: list = ["ZCARD", key]
+        command: List = ["ZCARD", key]
 
         return await self.run(command)
 
     async def zcount(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
     ) -> int:
         """
@@ -1806,38 +1806,38 @@
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
 
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        command: list = ["ZCOUNT", key, min_score, max_score]
+        command: List = ["ZCOUNT", key, min_score, max_score]
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
     async def zdiff(
         self, *keys: str, withscores: bool = False
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zdiff
 
         The number of keys is calculated automatically.
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZDIFF", len(keys), *keys]
+        command: List = ["ZDIFF", len(keys), *keys]
 
         if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
@@ -1850,57 +1850,57 @@
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZDIFFSTORE", destination, len(keys), *keys]
+        command: List = ["ZDIFFSTORE", destination, len(keys), *keys]
 
         return await self.run(command)
 
     async def zincrby(
         self, key: str, increment: float, member: str
     ) -> Union[str, float]:
         """
         See https://redis.io/commands/zincrby
 
         :return: A float if "format_return" is True.
         """
 
-        command: list = ["ZINCRBY", key, increment, member]
+        command: List = ["ZINCRBY", key, increment, member]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
     async def zinter(
         self,
         *keys: str,
-        weights: Union[list[float], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zinter
 
         The number of keys is calculated automatically.
 
-        :return: A dict of member-score pairs if "withscores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZINTER", len(keys), *keys]
+        command: List = ["ZINTER", len(keys), *keys]
 
         if weights:
             command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
@@ -1913,27 +1913,27 @@
 
         return await self.run(command)
 
     async def zinterstore(
         self,
         destination: str,
         *keys: str,
-        weights: Union[list[float], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         """
         See https://redis.io/commands/zinterstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZINTERSTORE", destination, len(keys), *keys]
+        command: List = ["ZINTERSTORE", destination, len(keys), *keys]
 
         if weights:
             command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
@@ -1950,48 +1950,48 @@
         if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
             ("(", "[", "+", "-")
         ):
             raise Exception(
                 "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
             )
 
-        command: list = ["ZLEXCOUNT", key, min_score, max_score]
+        command: List = ["ZLEXCOUNT", key, min_score, max_score]
 
         return await self.run(command)
 
     async def zmscore(
         self, key: str, *members: str
-    ) -> Union[list[Union[str, None]], list[Union[float, None]]]:
+    ) -> Union[List[Union[str, None]], List[Union[float, None]]]:
         """
         See https://redis.io/commands/zmscore
 
-        :return: A list of float or None values if "format_return" is True.
+        :return: A List of float or None values if "format_return" is True.
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be specified.")
 
-        command: list = ["ZMSCORE", key, *members]
+        command: List = ["ZMSCORE", key, *members]
 
-        raw: list[Union[str, None]] = await self.run(command)
+        raw: List[Union[str, None]] = await self.run(command)
 
         return format_float_list(raw) if self.format_return else raw
 
     async def zpopmax(
         self, key: str, count: Union[int, None] = None
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zpopmax
 
         :param count: defaults to 1 on the server side
 
-        :return: A dict of member-score pairs if "format_return" is True.
+        :return: A Dict of member-score pairs if "format_return" is True.
         """
 
-        command: list = ["ZPOPMAX", key]
+        command: List = ["ZPOPMAX", key]
 
         if count is not None:
             command.append(count)
 
         raw: SortedSetReturn = await self.run(command)
 
         return format_sorted_set_return(raw) if self.format_return else raw
@@ -2000,18 +2000,18 @@
         self, key: str, count: Union[int, None] = None
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zpopmin
 
         :param count: defaults to 1 on the server side
 
-        :return: A dict of member-score pairs if "format_return" is True.
+        :return: A Dict of member-score pairs if "format_return" is True.
         """
 
-        command: list = ["ZPOPMIN", key]
+        command: List = ["ZPOPMIN", key]
 
         if count is not None:
             command.append(count)
 
         raw: SortedSetReturn = await self.run(command)
 
         return format_sorted_set_return(raw) if self.format_return else raw
@@ -2020,21 +2020,21 @@
         self, key: str, count: Union[int, None] = None, withscores: bool = False
     ) -> Union[(Union[str, None]), (Union[SortedSetReturn, FormattedSortedSetReturn])]:
         """
         See https://redis.io/commands/zrandmember
 
         :param count: defaults to 1 on the server side
 
-        :return: A dict of member-score pairs if "withscores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if count is None and withscores:
             raise Exception('"withscores" can only be used with "count".')
 
-        command: list = ["ZRANDMEMBER", key]
+        command: List = ["ZRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
             if withscores:
                 command.append("WITHSCORES")
 
@@ -2042,15 +2042,15 @@
 
                 return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
     async def zrange(
         self,
         key: str,
         start: FloatMinMax,
         stop: FloatMinMax,
@@ -2061,22 +2061,22 @@
         withscores: bool = False,
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zrange
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         handle_non_deprecated_zrange_exceptions(
             range_method, start, stop, limit_offset, limit_count
         )
 
-        command: list = ["ZRANGE", key, start, stop]
+        command: List = ["ZRANGE", key, start, stop]
 
         if range_method:
             command.append(range_method)
 
         if rev:
             command.append("REV")
 
@@ -2095,34 +2095,34 @@
     async def zrangebylex(
         self,
         key: str,
         min_score: str,
         max_score: str,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> list[Union[str, None]]:
+    ) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/zrangebylex
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
         """
 
         handle_zrangebylex_exceptions(min_score, max_score, limit_offset, limit_count)
 
-        command: list = ["ZRANGEBYLEX", key, min_score, max_score]
+        command: List = ["ZRANGEBYLEX", key, min_score, max_score]
 
         if limit_offset is not None:
             command.extend(["LIMIT", limit_offset, limit_count])
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
-    whether "withscores" is True or not, its raw return type will be list[str].
+    whether "withscores" is True or not, its raw return type will be List[str].
     """
 
     async def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
@@ -2134,21 +2134,21 @@
         See https://redis.io/commands/zrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
 
-        :return: A dict of member-score pairs if "withscores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if number_are_not_none(offset, count, number=1):
             raise Exception('Both "offset" and "count" must be specified.')
 
-        command: list = ["ZRANGEBYSCORE", key, min_score, max_score]
+        command: List = ["ZRANGEBYSCORE", key, min_score, max_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
 
         if withscores:
             command.append("WITHSCORES")
 
@@ -2178,15 +2178,15 @@
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
         handle_non_deprecated_zrange_exceptions(
             range_method, min_score, max_score, limit_offset, limit_count
         )
 
-        command: list = ["ZRANGESTORE", dst, src, min_score, max_score]
+        command: List = ["ZRANGESTORE", dst, src, min_score, max_score]
 
         if range_method:
             command.append(range_method)
 
         if rev:
             command.append("REV")
 
@@ -2196,27 +2196,27 @@
         return await self.run(command)
 
     async def zrank(self, key: str, member: str) -> Union[int, None]:
         """
         See https://redis.io/commands/zrank
         """
 
-        command: list = ["ZRANK", key, member]
+        command: List = ["ZRANK", key, member]
 
         return await self.run(command)
 
     async def zrem(self, key: str, *members: str) -> int:
         """
         See https://redis.io/commands/zrem
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
-        command: list = ["ZREM", key, *members]
+        command: List = ["ZREM", key, *members]
 
         return await self.run(command)
 
     async def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int:
         """
         See https://redis.io/commands/zremrangebylex
 
@@ -2227,24 +2227,24 @@
         if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
             ("(", "[", "+", "-")
         ):
             raise Exception(
                 "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
             )
 
-        command: list = ["ZREMRANGEBYLEX", key, min_score, max_score]
+        command: List = ["ZREMRANGEBYLEX", key, min_score, max_score]
 
         return await self.run(command)
 
     async def zremrangebyrank(self, key: str, start: int, stop: int) -> int:
         """
         See https://redis.io/commands/zremrangebyrank
         """
 
-        command: list = ["ZREMRANGEBYRANK", key, start, stop]
+        command: List = ["ZREMRANGEBYRANK", key, start, stop]
 
         return await self.run(command)
 
     async def zremrangebyscore(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
     ) -> int:
         """
@@ -2252,33 +2252,33 @@
         
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
 
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        command: list = ["ZREMRANGEBYSCORE", key, min_score, max_score]
+        command: List = ["ZREMRANGEBYSCORE", key, min_score, max_score]
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but,
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
     async def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zrevrange
 
-        :return: A dict of member-score pairs if "withscores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        command: list = ["ZREVRANGE", key, start, stop]
+        command: List = ["ZREVRANGE", key, start, stop]
 
         if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
@@ -2288,34 +2288,34 @@
     async def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
         offset: Union[int, None] = None,
         count: Union[int, None] = None,
-    ) -> list[str]:
+    ) -> List[str]:
         """
         See https://redis.io/commands/zrevrangebylex
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
         """
 
         handle_zrangebylex_exceptions(min_score, max_score, offset, count)
 
-        command: list = ["ZREVRANGEBYLEX", key, max_score, min_score]
+        command: List = ["ZREVRANGEBYLEX", key, max_score, min_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but,
-    whether "withscores" is True or not, its raw return type will be list[str].
+    whether "withscores" is True or not, its raw return type will be List[str].
     """
 
     async def zrevrangebyscore(
         self,
         key: str,
         max_score: FloatMinMax,
         min_score: FloatMinMax,
@@ -2327,21 +2327,21 @@
         See https://redis.io/commands/zrevrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
 
-        :return: A dict of member-score pairs if "withscores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if number_are_not_none(limit_offset, limit_count, number=1):
             raise Exception('Both "limit_offset" and "limit_count" must be specified.')
 
-        command: list = ["ZREVRANGEBYSCORE", key, max_score, min_score]
+        command: List = ["ZREVRANGEBYSCORE", key, max_score, min_score]
 
         if limit_offset is not None:
             command.extend(["LIMIT", limit_offset, limit_count])
 
         if withscores:
             command.append("WITHSCORES")
 
@@ -2352,101 +2352,101 @@
         return await self.run(command)
 
     async def zrevrank(self, key: str, member: str) -> Union[int, None]:
         """
         See https://redis.io/commands/zrevrank
         """
 
-        command: list = ["ZREVRANK", key, member]
+        command: List = ["ZREVRANK", key, member]
 
         return await self.run(command)
 
     async def zscan(
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         return_cursor: bool = True,
     ) -> Union[
         (
             Union[
-                list[Union[str, SortedSetReturn]],
-                list[Union[int, FormattedSortedSetReturn]],
+                List[Union[str, SortedSetReturn]],
+                List[Union[int, FormattedSortedSetReturn]],
             ]
         ),
         (Union[SortedSetReturn, FormattedSortedSetReturn]),
     ]:
         """
         See https://redis.io/commands/zscan
 
         :param return_cursor: if set to False, it won't return the cursor
         :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only a dict of member-score pairs will be returned if "return_cursor" is False and "format_return" is True.
+        Only a Dict of member-score pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
-        command: list = ["ZSCAN", key, cursor]
+        command: List = ["ZSCAN", key, cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        raw: list[Union[int, SortedSetReturn]] = await self.run(command)
+        raw: List[Union[int, SortedSetReturn]] = await self.run(command)
 
         if return_cursor:
             return (
                 [int(raw[0]), format_sorted_set_return(raw[1])]
                 if self.format_return
                 else raw
             )
 
-        # The raw result is composed of the new cursor and the list of elements.
+        # The raw result is composed of the new cursor and the List of elements.
         return format_sorted_set_return(raw[1]) if self.format_return else raw[1]
 
     async def zscore(self, key: str, member: str) -> Union[str, None, float]:
         """
         See https://redis.io/commands/zscore
 
         :return: A float or None if "format_return" is True.
         """
 
-        command: list = ["ZSCORE", key, member]
+        command: List = ["ZSCORE", key, member]
 
         raw: Union[str, None] = await self.run(command)
 
         return float(raw) if self.format_return and raw is not None else raw
 
     """
     This has actually 3 return scenarios, but,
-    whether "withscores" is True or not, its raw return type will be list[str].
+    whether "withscores" is True or not, its raw return type will be List[str].
     """
 
     async def zunion(
         self,
         *keys: str,
-        weights: Union[list[float], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
     ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zunion
 
         The number of keys is calculated automatically.
 
-        :return: A dict of member-score pairs if "withscores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZUNION", len(keys), *keys]
+        command: List = ["ZUNION", len(keys), *keys]
 
         if weights:
             command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
@@ -2459,78 +2459,78 @@
 
         return await self.run(command)
 
     async def zunionstore(
         self,
         destination: str,
         *keys: str,
-        weights: Union[list[float], None] = None,
+        weights: Union[List[float], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         """
         See https://redis.io/commands/zunionstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZUNIONSTORE", destination, len(keys), *keys]
+        command: List = ["ZUNIONSTORE", destination, len(keys), *keys]
 
         if weights:
             command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
         return await self.run(command)
 
     async def append(self, key: str, value: Any) -> int:
         """
         See https://redis.io/commands/append
         """
 
-        command: list = ["APPEND", key, value]
+        command: List = ["APPEND", key, value]
 
         return await self.run(command)
 
     async def decr(self, key: str) -> int:
         """
         See https://redis.io/commands/decr
         """
 
-        command: list = ["DECR", key]
+        command: List = ["DECR", key]
 
         return await self.run(command)
 
     async def decrby(self, key: str, decrement: int) -> int:
         """
         See https://redis.io/commands/decrby
         """
 
-        command: list = ["DECRBY", key, decrement]
+        command: List = ["DECRBY", key, decrement]
 
         return await self.run(command)
 
     async def get(self, key: str) -> Union[str, None]:
         """
         See https://redis.io/commands/get
         """
 
-        command: list = ["GET", key]
+        command: List = ["GET", key]
 
         return await self.run(command)
 
     async def getdel(self, key: str) -> Union[str, None]:
         """
         See https://redis.io/commands/getdel
         """
 
-        command: list = ["GETDEL", key]
+        command: List = ["GETDEL", key]
 
         return await self.run(command)
 
     async def getex(
         self,
         key: str,
         ex: Union[int, None] = None,
@@ -2542,15 +2542,15 @@
         """
         See https://redis.io/commands/getex
         """
 
         if not number_are_not_none(ex, px, exat, pxat, persist, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
-        command: list = ["GETEX", key]
+        command: List = ["GETEX", key]
 
         if ex is not None:
             command.extend(["EX", ex])
 
         if px is not None:
             command.extend(["PX", px])
 
@@ -2566,100 +2566,100 @@
         return await self.run(command)
 
     async def getrange(self, key: str, start: int, end: int) -> str:
         """
         See https://redis.io/commands/getrange
         """
 
-        command: list = ["GETRANGE", key, start, end]
+        command: List = ["GETRANGE", key, start, end]
 
         return await self.run(command)
 
     async def getset(self, key: str, value: Any) -> Union[str, None]:
         """
         See https://redis.io/commands/getset
         """
 
-        command: list = ["GETSET", key, value]
+        command: List = ["GETSET", key, value]
 
         return await self.run(command)
 
     async def incr(self, key: str) -> int:
         """
         See https://redis.io/commands/incr
         """
 
-        command: list = ["INCR", key]
+        command: List = ["INCR", key]
 
         return await self.run(command)
 
     async def incrby(self, key: str, increment: int) -> int:
         """
         See https://redis.io/commands/incrby
         """
 
-        command: list = ["INCRBY", key, increment]
+        command: List = ["INCRBY", key, increment]
 
         return await self.run(command)
 
     async def incrbyfloat(self, key: str, increment: float) -> Union[str, float]:
         """
         See https://redis.io/commands/incrbyfloat
 
         :return: A float if "format_return" is True.
         """
 
-        command: list = ["INCRBYFLOAT", key, increment]
+        command: List = ["INCRBYFLOAT", key, increment]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
-    async def mget(self, *keys: str) -> list[Union[str, None]]:
+    async def mget(self, *keys: str) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/mget
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["MGET", *keys]
+        command: List = ["MGET", *keys]
 
         return await self.run(command)
 
-    async def mset(self, key_value_pairs: dict) -> Literal["OK"]:
+    async def mset(self, key_value_pairs: Dict) -> Literal["OK"]:
         """
         See https://redis.io/commands/mset
         """
 
-        command: list = ["MSET"]
+        command: List = ["MSET"]
 
         for key, value in key_value_pairs.items():
             command.extend([key, value])
 
         return await self.run(command)
 
-    async def msetnx(self, key_value_pairs: dict) -> Literal[1, 0]:
+    async def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]:
         """
         See https://redis.io/commands/msetnx
         """
 
-        command: list = ["MSETNX"]
+        command: List = ["MSETNX"]
 
         for key, value in key_value_pairs.items():
             command.extend([key, value])
 
         return await self.run(command)
 
     async def psetex(self, key: str, milliseconds: int, value: Any) -> str:
         """
         See https://redis.io/commands/psetex
         """
 
-        command: list = ["PSETEX", key, milliseconds, value]
+        command: List = ["PSETEX", key, milliseconds, value]
 
         return await self.run(command)
 
     async def set(
         self,
         key: str,
         value: Any,
@@ -2681,15 +2681,15 @@
 
         if not number_are_not_none(ex, px, exat, pxat, keepttl, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         if nx and get:
             raise Exception('"nx" and "get" are mutually exclusive.')
 
-        command: list = ["SET", key, value]
+        command: List = ["SET", key, value]
 
         if nx:
             command.append("NX")
 
         if xx:
             command.append("XX")
 
@@ -2714,60 +2714,60 @@
         return await self.run(command)
 
     async def setex(self, key: str, seconds: int, value: Any) -> str:
         """
         See https://redis.io/commands/setex
         """
 
-        command: list = ["SETEX", key, seconds, value]
+        command: List = ["SETEX", key, seconds, value]
 
         return await self.run(command)
 
     async def setnx(self, key: str, value: Any) -> Literal[1, 0]:
         """
         See https://redis.io/commands/setnx
         """
 
-        command: list = ["SETNX", key, value]
+        command: List = ["SETNX", key, value]
 
         return await self.run(command)
 
     async def setrange(self, key: str, offset: int, value: Any) -> int:
         """
         See https://redis.io/commands/setrange
         """
 
-        command: list = ["SETRANGE", key, offset, value]
+        command: List = ["SETRANGE", key, offset, value]
 
         return await self.run(command)
 
     async def strlen(self, key: str) -> int:
         """
         See https://redis.io/commands/strlen
         """
 
-        command: list = ["STRLEN", key]
+        command: List = ["STRLEN", key]
 
         return await self.run(command)
 
     async def substr(self, key: str, start: int, end: int) -> str:
         """
         See https://redis.io/commands/substr
         """
 
-        command: list = ["SUBSTR", key, start, end]
+        command: List = ["SUBSTR", key, start, end]
 
         return await self.run(command)
 
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
     def __init__(self, client: Redis, key: str):
         self.client = client
-        self.command: list = ["BITFIELD", key]
+        self.command: List = ["BITFIELD", key]
 
     def get(self, encoding: str, offset: BitFieldOffset):
         """
         Returns the specified bit field.
 
         Source: https://redis.io/commands/bitfield
         """
@@ -2814,186 +2814,186 @@
         """
 
         _command = ["OVERFLOW", overflow]
         self.command.extend(_command)
 
         return self
 
-    async def execute(self) -> list:
+    async def execute(self) -> List:
         return await self.client.run(command=self.command)
 
 
 class BitFieldRO:
     def __init__(self, client: Redis, key: str):
         self.client = client
-        self.command: list = ["BITFIELD_RO", key]
+        self.command: List = ["BITFIELD_RO", key]
 
     def get(self, encoding: str, offset: BitFieldOffset):
         """
         Returns the specified bit field.
 
         Source: https://redis.io/commands/bitfield_ro
         """
 
         _command = ["GET", encoding, offset]
         self.command.extend(_command)
 
         return self
 
-    async def execute(self) -> list:
+    async def execute(self) -> List:
         return await self.client.run(command=self.command)
 
 
 class PubSub:
     def __init__(self, client: Redis):
         self.client = client
 
-    async def channels(self, pattern: Union[str, None] = None) -> list[str]:
+    async def channels(self, pattern: Union[str, None] = None) -> List[str]:
         """
         See https://redis.io/commands/pubsub-channels
         """
 
-        command: list = ["PUBSUB", "CHANNELS"]
+        command: List = ["PUBSUB", "CHANNELS"]
 
         if pattern is not None:
             command.append(pattern)
 
         return await self.client.run(command=command)
 
     async def numpat(self) -> int:
         """
         See https://redis.io/commands/pubsub-numpat
         """
 
-        command: list = ["PUBSUB", "NUMPAT"]
+        command: List = ["PUBSUB", "NUMPAT"]
 
         return await self.client.run(command=command)
 
     async def numsub(
         self, *channels: str
-    ) -> Union[list[Union[str, int]], dict[str, int]]:
+    ) -> Union[List[Union[str, int]], Dict[str, int]]:
         """
         See https://redis.io/commands/pubsub-numsub
 
-        :return: A dict with channel-number_of_subscribers pairs if "format_return" is True.
+        :return: A Dict with channel-number_of_subscribers pairs if "format_return" is True.
         """
 
-        command: list = ["PUBSUB", "NUMSUB", *channels]
+        command: List = ["PUBSUB", "NUMSUB", *channels]
 
-        raw: list[Union[str, int]] = await self.client.run(command)
+        raw: List[Union[str, int]] = await self.client.run(command)
 
         return format_pubsub_numsub_return(raw) if self.client.format_return else raw
 
 
 class Script:
     def __init__(self, client: Redis):
         self.client = client
 
-    async def exists(self, *sha1: str) -> Union[list[Literal[1, 0]], list[bool]]:
+    async def exists(self, *sha1: str) -> Union[List[Literal[1, 0]], List[bool]]:
         """
         See https://redis.io/commands/script-exists
 
-        :return: A list of bools if "format_return" is True.
+        :return: A List of bools if "format_return" is True.
         """
 
         if len(sha1) == 0:
             raise Exception("At least one sha1 digests must be provided.")
 
-        command: list = ["SCRIPT", "EXISTS", *sha1]
+        command: List = ["SCRIPT", "EXISTS", *sha1]
 
-        raw: list[Literal[1, 0]] = await self.client.run(command=command)
+        raw: List[Literal[1, 0]] = await self.client.run(command=command)
 
         return format_bool_list(raw) if self.client.format_return else raw
 
     async def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
         """
         See https://redis.io/commands/script-flush
         """
 
-        command: list = ["SCRIPT", "FLUSH"]
+        command: List = ["SCRIPT", "FLUSH"]
 
         if mode:
             command.append(mode)
 
         return await self.client.run(command=command)
 
     async def load(self, script: str) -> str:
         """
         See https://redis.io/commands/script-load
         """
 
-        command: list = ["SCRIPT", "LOAD", script]
+        command: List = ["SCRIPT", "LOAD", script]
 
         return await self.client.run(command=command)
 
 
 """
 class ACL:
     def __init__(self, client: Redis):
         self.client = client
 
-    async def cat(self, category: Union[str, None] = None) -> list[str]:
+    async def cat(self, category: Union[str, None] = None) -> List[str]:
         # See https://redis.io/commands/acl-cat
 
-        command: list = ["ACL", "CAT"]
+        command: List = ["ACL", "CAT"]
 
         if category is not None:
             command.append(category)
 
         return await self.client.run(command=command)
 
     async def deluser(self, *usernames: str) -> int:
         # See https://redis.io/commands/acl-deluser
         
         if len(usernames) == 0:
             raise Exception("At least one username must be provided.")
 
-        command: list = ["ACL", "DELUSER", *usernames]
+        command: List = ["ACL", "DELUSER", *usernames]
 
         return await self.client.run(command=command)
 
     async def genpass(self, bits: Union[int, None] = None) -> str:
         # See https://redis.io/commands/acl-genpass
 
-        command: list = ["ACL", "GENPASS"]
+        command: List = ["ACL", "GENPASS"]
 
         if bits is not None:
             command.append(bits)
 
         return await self.client.run(command=command)
 
     # Is it possible to format this output?
-    async def getuser(self, username: str) -> Union[list[str], None]:
+    async def getuser(self, username: str) -> Union[List[str], None]:
         # See https://redis.io/commands/acl-getuser
 
-        command: list = ["ACL", "GETUSER", username]
+        command: List = ["ACL", "GETUSER", username]
 
         return await self.client.run(command=command)
 
-    async def list_rules(self) -> list[str]:
-        # See https://redis.io/commands/acl-list
+    async def List_rules(self) -> List[str]:
+        # See https://redis.io/commands/acl-List
 
         command = ["ACL", "LIST"]
 
         return await self.client.run(command=command)
 
     async def load(self) -> str:
         # See https://redis.io/commands/acl-load
 
         command = ["ACL", "LOAD"]
 
         return await self.client.run(command=command)
 
-    async def log(self, count: Union[int, None] = None, reset: bool = False) -> list[str]:
+    async def log(self, count: Union[int, None] = None, reset: bool = False) -> List[str]:
         # See https://redis.io/commands/acl-log
 
         if count is not None and reset:
             raise Exception("Cannot specify both "count" and "reset".")
 
-        command: list = ["ACL", "LOG"]
+        command: List = ["ACL", "LOG"]
 
         if count is not None:
             command.append(count)
 
         if reset:
             command.append("RESET")
```

### Comparing `upstash_redis_a-0.1.2/upstash_redis/http/decode.py` & `upstash_redis_a-0.1.3/upstash_redis/http/decode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from upstash_redis.schema.http import RESTResult
 from upstash_redis.utils.base import base64_to_string
 from upstash_redis.exception import UpstashException
+from typing import List
 
 
 def decode(raw: RESTResult, encoding: str) -> RESTResult:
     """
     Decode the response received from the REST API.
     """
 
     if encoding == "base64":
         if isinstance(raw, str):
             return "OK" if raw == "OK" else base64_to_string(raw)
 
         elif isinstance(raw, int) or raw is None:
             return raw
 
-        elif isinstance(raw, list):
+        elif isinstance(raw, List):
             return [
                 # Decode recursively.
                 decode(element, encoding)
                 for element in raw
             ]
         else:
             raise UpstashException(
```

### Comparing `upstash_redis_a-0.1.2/upstash_redis/http/execute.py` & `upstash_redis_a-0.1.3/upstash_redis/http/execute.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from upstash_redis.http.decode import decode
 from upstash_redis.schema.http import RESTResult, RESTResponse, RESTEncoding
 from upstash_redis.schema.telemetry import TelemetryData
 from asyncio import sleep
 from aiohttp import ClientSession
 from json import dumps
 from platform import python_version
-from typing import Union
+from typing import Union, List, Dict
 
 
 async def execute(
     session: ClientSession,
     url: str,
     token: str,
     encoding: RESTEncoding,
     retries: int,
     retry_interval: int,
-    command: list,
+    command: List,
     allow_telemetry: bool,
     telemetry_data: Union[TelemetryData, None] = None,
 ) -> RESTResult:
     """
     Execute the given command over the REST API.
 
     :param encoding: the encoding that can be used by the REST API to parse the response before sending it
@@ -33,15 +33,15 @@
     command = [
         element if (isinstance(element, str) or isinstance(element, int) or isinstance(element, float)) else dumps(element)
         for element in command
     ]
 
     for i in range(retries + 1):
         try:
-            headers: dict[str, str] = {"Authorization": f"Bearer {token}"}
+            headers: Dict[str, str] = {"Authorization": f"Bearer {token}"}
 
             if allow_telemetry:
                 if telemetry_data:
                     # Avoid the [] syntax to prevent KeyError from being raised.
                     if telemetry_data.get("runtime"):
                         headers["Upstash-Telemetry-Runtime"] = telemetry_data["runtime"]
                     else:
```

### Comparing `upstash_redis_a-0.1.2/upstash_redis/schema/commands/returns.py` & `upstash_redis_a-0.1.3/upstash_redis/schema/commands/returns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Union
+from typing import Union, List, Dict
 
 """
 The raw output returned by some Geo commands, usually the ones that return properties of members.
 
 If no additional properties are requested, the output is a list of strings, each string representing a member.
 
 If coordinates are requested, each member's properties will be represented by a list (the result itself being a list),
 where the coordinates themselves will be another one.
 """
-GeoMembersReturn = list[Union[str, list[Union[str, list[str]]]]]
+GeoMembersReturn = List[Union[str, List[Union[str, List[str]]]]]
 
 """
 The output resulted by formatting "GeoMembersReturn".
 
 Note that this might differ from the "GeoMember" type that represents the initial properties of a geo member.
 """
-FormattedGeoMembersReturn = list[dict[str, Union[str, float, int]]]
+FormattedGeoMembersReturn = List[Dict[str, Union[str, float, int]]]
 
 
 # The raw output returned by the Hash commands that return the field-value pairs of a hash.
-HashReturn = list[str]
+HashReturn = List[str]
 
 # The output resulted by formatting "HashReturn"
-FormattedHashReturn = dict[str, str]
+FormattedHashReturn = Dict[str, str]
 
 # The raw output returned by the Sorted Set commands that return the member-score pairs of a sorted set.
-SortedSetReturn = list[str]
+SortedSetReturn = List[str]
 
 # The output resulted by formatting "SortedSetReturn"
-FormattedSortedSetReturn = dict[str, float]
+FormattedSortedSetReturn = Dict[str, float]
```

### Comparing `upstash_redis_a-0.1.2/upstash_redis/schema/http.py` & `upstash_redis_a-0.1.3/upstash_redis/schema/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import TypedDict, Literal, TypeVar, Any, Union
+from typing import TypedDict, Literal, TypeVar, Any, Union, List
 
 
 """
 The type of the "result" field returned by the REST API. 
 
 It is a TypeVar mainly because of two reasons:
  - the "decode" function, which should return the same data type that was passed via the "raw" parameter.
  - the "execute" function's return is not an Union.
 """
-RESTResult = TypeVar("RESTResult", str, int, list, None, Literal[0, 1], Literal["OK"])
+RESTResult = TypeVar("RESTResult", str, int, List, None, Literal[0, 1], Literal["OK"])
 
 """
 The type of encoding that will be passed as a header to the REST API. 
 If set to False, no encoding will be used.
 """
 RESTEncoding = Union[Literal["base64"], Literal[False]]
```

### Comparing `upstash_redis_a-0.1.2/upstash_redis/utils/exception.py` & `upstash_redis_a-0.1.3/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.2/upstash_redis/utils/format.py` & `upstash_redis_a-0.1.3/upstash_redis/utils/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,35 @@
     GeoMembersReturn,
     FormattedGeoMembersReturn,
     HashReturn,
     FormattedHashReturn,
     SortedSetReturn,
     FormattedSortedSetReturn,
 )
-from typing import Literal, Union
+from typing import Literal, Union, List, Dict
 
 
-def _list_to_dict(raw: list) -> dict:
+def _list_to_dict(raw: List) -> Dict:
     """
     Convert a list that contains ungrouped pairs as consecutive elements (usually field-value or similar) into a dict.
     """
 
     return {raw[iterator]: raw[iterator + 1] for iterator in range(0, len(raw), 2)}
 
 
 def format_geo_positions_return(
-    raw: list[Union[list[str], None]],
-) -> list[Union[dict[str, float], None]]:
+    raw: List[Union[List[str], None]],
+) -> List[Union[Dict[str, float], None]]:
     """
     Format the raw output returned by "GEOPOS".
     """
 
     return [
         {"longitude": float(member[0]), "latitude": float(member[1])}
-        if isinstance(member, list)
+        if isinstance(member, List)
         else None
         for member in raw
     ]
 
 
 def format_geo_members_return(
     raw: GeoMembersReturn,
@@ -54,15 +54,15 @@
 
     All represented as strings
     """
 
     result: FormattedGeoMembersReturn = []
 
     for member in raw:
-        formatted_member: dict[str, Union[str, float, int]] = {"member": member[0]}
+        formatted_member: Dict[str, Union[str, float, int]] = {"member": member[0]}
 
         if with_distance:
             formatted_member["distance"] = float(member[1])
 
             if with_hash:
                 formatted_member["hash"] = int(member[2])
 
@@ -95,31 +95,31 @@
     Format the raw output given by Hash commands, usually the ones that return the field-value
     pairs of Hashes.
     """
 
     return _list_to_dict(raw=raw)
 
 
-def format_pubsub_numsub_return(raw: list[Union[str, int]]) -> dict[str, int]:
+def format_pubsub_numsub_return(raw: List[Union[str, int]]) -> Dict[str, int]:
     """
     Format the raw output returned by "PUBSUB NUMSUB".
     """
 
     return _list_to_dict(raw=raw)
 
 
-def format_bool_list(raw: list[Literal[0, 1]]) -> list[bool]:
+def format_bool_list(raw: List[Literal[0, 1]]) -> List[bool]:
     """
     Format a list of boolean integers.
     """
 
     return [bool(value) for value in raw]
 
 
-def format_server_time_return(raw: list[str]) -> dict[str, int]:
+def format_server_time_return(raw: List[str]) -> Dict[str, int]:
     """
     Format the raw output returned by "TIME".
     """
 
     return {"seconds": int(raw[0]), "microseconds": int(raw[1])}
 
 
@@ -128,13 +128,13 @@
     Format the raw output given by Sorted Set commands, usually the ones that return the member-score
     pairs of Sorted Sets.
     """
 
     return _list_to_dict(raw=raw)
 
 
-def format_float_list(raw: list[Union[str, None]]) -> list[Union[float, None]]:
+def format_float_list(raw: List[Union[str, None]]) -> List[Union[float, None]]:
     """
     Format a list of strings representing floats or None values.
     """
 
     return [float(value) if value is not None else None for value in raw]
```

### Comparing `upstash_redis_a-0.1.2/PKG-INFO` & `upstash_redis_a-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis-a
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

