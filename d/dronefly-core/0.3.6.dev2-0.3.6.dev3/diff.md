# Comparing `tmp/dronefly_core-0.3.6.dev2.tar.gz` & `tmp/dronefly_core-0.3.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev2.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev3.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev2.tar` & `dronefly_core-0.3.6.dev3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev2/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev2/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev2/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev2/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev2/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     7532 2023-06-16 17:33:58.906636 dronefly_core-0.3.6.dev2/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev2/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev2/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev2/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    32312 2023-06-18 12:34:06.350900 dronefly_core-0.3.6.dev2/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev2/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev2/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev2/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev2/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev2/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev2/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev2/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev2/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev2/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    19768 2023-06-17 15:43:08.517165 dronefly_core-0.3.6.dev2/dronefly/core/query/query.py
--rw-r--r--   0        0        0     1310 2023-06-18 12:34:04.486862 dronefly_core-0.3.6.dev2/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-18 12:36:24.205752 dronefly_core-0.3.6.dev2/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev2/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev3/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev3/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev3/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev3/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev3/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     7991 2023-06-18 15:08:05.888074 dronefly_core-0.3.6.dev3/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev3/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev3/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev3/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    34585 2023-06-18 15:07:29.087299 dronefly_core-0.3.6.dev3/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev3/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev3/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev3/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev3/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev3/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev3/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev3/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev3/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev3/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev3/dronefly/core/query/query.py
+-rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev3/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-19 11:01:37.055511 dronefly_core-0.3.6.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev3/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev3/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev2/LICENSE` & `dronefly_core-0.3.6.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/README.md` & `dronefly_core-0.3.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev3/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev3/dronefly/core/commands/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from enum import Enum
 import re
 
 from attrs import define
 from rich.markdown import Markdown
 
 from ..clients.inat import iNatClient
-from ..constants import INAT_DEFAULTS, INAT_USER_DEFAULT_PARAMS
+from ..constants import INAT_DEFAULTS, INAT_USER_DEFAULT_PARAMS, RANK_KEYWORDS
+
 from ..parsers import NaturalParser
-from ..formatters.generic import ObservationFormatter, TaxonFormatter
+from ..formatters.generic import LifeListFormatter, ObservationFormatter, TaxonFormatter
 from ..models.user import User
+from ..query.query import get_base_query_args, QueryResponse
 
 
 RICH_BQ_NEWLINE_PAT = re.compile(r"^(\> .*?)\n(?=\> )", re.MULTILINE)
 RICH_BQ_END_PAT = re.compile(r"^((\> .*?\n)+)(?!> )", re.MULTILINE)
 RICH_NO_BQ_NEWLINE_PAT = re.compile(r"^(?!\> )(.+?)(\n)(?!$|\> )", re.MULTILINE)
 RICH_NEWLINE = " \\\n"
 
@@ -93,51 +95,51 @@
             response = Markdown(rich_markdown)
         else:
             # Return the literal markdown for Discord to render
             response = markdown_text
         return response
 
     def life(self, ctx: Context, *args):
-        main_query_str = None
-        taxon = None
-        per = None
-        if args:
-            query = self._parse(" ".join(args))
-            # TODO: Handle all query clauses, not just main.terms
-            # TODO: Doesn't do any ranking or filtering of results
-            if not query.main or not query.main.terms:
-                return "Not a taxon"
-            main_query_str = " ".join(query.main.terms)
-            per = query.per
+        _args = " ".join(args) or "by me"
+        query = self._parse(_args)
+        per_rank = query.per or "leaf"
+        if per_rank not in [*RANK_KEYWORDS, "leaf", "main", "any"]:
+            return "Specify `per <rank-or-keyword>`"
 
+        query_args = get_base_query_args(query)
         with self.inat_client.set_ctx(ctx) as client:
-            params = {
-                "user_id": ctx.author.inat_user_id,
-            }
-            if main_query_str:
-                taxon = client.taxa.autocomplete(q=main_query_str).one()
-                if not taxon:
-                    return "No taxon found"
-                params["taxon_id"] = taxon.id
-            life_list = client.observations.life_list(**params)
-
-        thing = f"taxa in {taxon.name}" if taxon else "taxa"
-        rank = None
-        taxa = life_list.data
-        if per:
-            # A bit simplistic - just assume it's a rank with no validation
-            rank = per
-            taxa = [
-                life_list_taxon
-                for life_list_taxon in life_list.data
-                if life_list_taxon.rank == rank
-            ]
-        _rank = f"rank {rank}" if rank else "any rank"
-        response = f"Your life list has {len(taxa)} {thing} with {_rank}"
-        return response
+            # Handle a useful subset of query args in a simplistic way for now
+            # (i.e. no config table lookup yet) to model full query in bot
+            if query.user == "me":
+                query_args["user"] = client.users.from_ids(
+                    ctx.author.inat_user_id, limit=1
+                ).one()
+            else:
+                users = client.users.autocomplete(q=query.user, limit=1)
+                if users:
+                    query_args["user"] = users[0]
+            if query and query.main and query.main.terms:
+                main_query_str = " ".join(query.main.terms)
+                taxon = client.taxa.autocomplete(q=main_query_str, limit=1).one()
+                query_args["taxon"] = taxon
+            if query.place:
+                place = client.places.autocomplete(q=query.place, limit=1).one()
+                query_args["place"] = place
+            if query.project:
+                project = client.projects.search(q=query.project, limit=1).one()
+                query_args["project"] = project
+            query_response = QueryResponse(**query_args)
+            obs_args = query_response.obs_args()
+            life_list = client.observations.life_list(**obs_args)
+
+        if not life_list:
+            return f"No life list {query_response.obs_query_description()}"
+
+        formatter = LifeListFormatter(life_list, per_rank, query_response)
+        return self._format_markdown(formatter)
 
     def taxon(self, ctx: Context, *args):
         query = self._parse(" ".join(args))
         # TODO: Handle all query clauses, not just main.terms
         # TODO: Doesn't do any ranking or filtering of results
         if not query.main or not query.main.terms:
             return "Not a taxon"
```

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev3/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev3/dronefly/core/formatters/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     RANK_EQUIVALENTS,
     RANK_LEVELS,
 )
 from dronefly.core.formatters.constants import (
     ICONS,
     WWW_BASE_URL,
 )
-from dronefly.core.utils import obs_url_from_v1
+from dronefly.core.utils import lifelists_url_from_query_response, obs_url_from_v1
 
 MEANS_LABEL_DESC = {
     "endemic": "endemic to",
     "native": "native in",
     "introduced": "introduced to",
 }
 
@@ -529,14 +529,80 @@
     def count():
         raise NotImplementedError
 
     def description():
         raise NotImplementedError
 
 
+class LifeListFormatter(BaseFormatter):
+    def __init__(
+        self,
+        life_list: LifeList,
+        per_rank: str,
+        query_response: QueryResponse,
+        with_url: bool = True,
+        max_len: int = 0,
+    ):
+        """
+        Parameters
+        ----------
+        taxon: Taxon
+            The taxon to format.
+
+        with_url: bool, optional
+            When True, link the name to taxon.url.
+        """
+        self.life_list = life_list
+        self.per_rank = per_rank
+        self.query_response = query_response
+        self.with_url = with_url
+        self.max_len = max_len
+
+    def format(self, with_title: bool = True):
+        """Format the life list as markdown."""
+        description = self.format_description()
+        if with_title:
+            description = "\n\n".join([self.format_title(), description])
+        return description
+
+    def format_title(self):
+        """Format life list title as Discord-like markdown.
+
+        Returns
+        -------
+        str
+            Like format_name(), except:
+
+            - Append the matching term in its own parentheses after the common name
+            in parentheses if the matching term is neither the scientific name nor
+            common name, e.g.
+            - "Pissenlits" -> "Genus *Taraxacum* (dandelions) (Pissenlits)"
+            - if with_url=True, the matched term is not included in the link
+            - Apply strikethrough style if the name is invalid, e.g.
+            - "Picoides pubescens" ->
+                "*Dryobates Pubescens* (Downy woodpecker) (~~Picoides Pubescens~~)
+        """
+        title = f"Life list {self.query_response.obs_query_description()}"
+        if self.with_url:
+            if self.query_response.user:
+                url = lifelists_url_from_query_response(self.query_response)
+            else:
+                url = obs_url_from_v1(
+                    {**self.query_response.obs_args(), "view": "species"}
+                )
+            title = format_link(title, url)
+        return title
+
+    def format_description(self):
+        """Format the life list description."""
+        return format_life_list_summary(
+            self.life_list, self.per_rank, self.query_response.taxon
+        )
+
+
 class TaxonFormatter(BaseFormatter):
     def __init__(
         self,
         taxon: Taxon,
         lang: str = None,
         with_url: bool = True,
         matched_term: str = None,
```

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev3/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev3/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev3/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev3/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev3/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev3/dronefly/core/query/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass, field
 import datetime as dt
 import re
 from typing import List, Optional, Union
 
 from dronefly.core.formatters.generic import format_taxon_name, format_user_name
 from dronefly.core.models.controlled_terms import ControlledTermSelector
+from dronefly.core.parsers.constants import VALID_OBS_OPTS
 from pyinaturalist.models import Place, Project, Taxon, User
 
 
 @define
 class TaxonQuery:
     """A taxon query composed of terms and/or phrases or a code or taxon_id, filtered by ranks."""
 
@@ -183,14 +184,70 @@
     # pylint: disable=invalid-name
 
     d1: Optional[Union[dt.datetime, str]]
     d2: Optional[Union[dt.datetime, str]]
     on: Optional[Union[dt.datetime, str]]
 
 
+def has_value(arg):
+    """Return true if arg is present and is not the `any` special keyword.
+
+    Use `any` in a query where a prior non-empty clause is present,
+    and that will negate that clause.
+    """
+    if not arg:
+        return False
+    if isinstance(arg, list):
+        return arg[0] and arg[0].lower() != "any"
+    elif isinstance(arg, TaxonQuery):
+        return (
+            (arg.terms and arg.terms[0].lower() != "any")
+            or arg.code
+            or arg.phrases
+            or arg.ranks
+            or arg.taxon_id
+        )
+    elif isinstance(arg, dt.datetime):
+        return True
+    else:
+        return arg.lower() != "any"
+
+
+def _get_options(query_options: list):
+    options = {}
+    # Accept a limited selection of options:
+    # - all of these to date apply only to observations, though others could
+    #   be added later
+    # - all options and values are lowercased
+    for (key, *val) in map(lambda opt: opt.lower().split("="), query_options):
+        val = val[0] if val else "true"
+        # - conservatively, only alphanumeric, comma, dash or
+        #   underscore characters accepted in values so far
+        # - TODO: proper validation per field type
+        if key in VALID_OBS_OPTS and re.match(r"^[a-z0-9,_-]*$", val):
+            options[key] = val
+    return options
+
+
+def get_base_query_args(query):
+    args = {}
+    args["options"] = _get_options(query.options) if has_value(query.options) else None
+    _observed = {}
+    _observed["on"] = query.obs_on if has_value(query.obs_on) else None
+    _observed["d1"] = query.obs_d1 if has_value(query.obs_d1) else None
+    _observed["d2"] = query.obs_d2 if has_value(query.obs_d2) else None
+    args["observed"] = DateSelector(**_observed)
+    _added = {}
+    _added["on"] = query.added_on if has_value(query.added_on) else None
+    _added["d1"] = query.added_d1 if has_value(query.added_d1) else None
+    _added["d2"] = query.added_d2 if has_value(query.added_d2) else None
+    args["added"] = DateSelector(**_added)
+    return args
+
+
 @dataclass
 class QueryResponse:
     """A generic query response object.
 
     - The parsed QueryResponse contains zero or more objects that are already
       each queried against the API and, optionally some additional options to
       apply to secondary entity queries. It is used in these main contexts:
@@ -205,25 +262,25 @@
       - `rg` is a macro for `"opt": {"quality_grade": "research"}`
       - The primary entity displayed by the `,taxon` command is `Anthophila`.
       - The secondary entities are observations & species counts of
         `Anthophila` for `benarmstrong` that are `research grade`, shown as a
         subdisplay.
     """
 
-    taxon: Optional[Taxon]
-    user: Optional[User]
-    place: Optional[Place]
-    unobserved_by: Optional[User]
-    except_by: Optional[User]
-    id_by: Optional[User]
-    project: Optional[Project]
-    options: Optional[dict]
-    controlled_term: Optional[ControlledTermSelector]
-    observed: Optional[DateSelector]
-    added: Optional[DateSelector]
+    taxon: Optional[Taxon] = None
+    user: Optional[User] = None
+    place: Optional[Place] = None
+    unobserved_by: Optional[User] = None
+    except_by: Optional[User] = None
+    id_by: Optional[User] = None
+    project: Optional[Project] = None
+    options: Optional[dict] = None
+    controlled_term: Optional[ControlledTermSelector] = None
+    observed: Optional[DateSelector] = None
+    added: Optional[DateSelector] = None
     adjectives: Optional[List[str]] = field(init=False)
 
     def __post_init__(self):
         adjectives = []
         if self.options:
             quality_grade = (self.options.get("quality_grade") or "").split(",")
             verifiable = self.options.get("verifiable")
```

### Comparing `dronefly_core-0.3.6.dev2/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev3/dronefly/core/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,23 @@
     """Lifelists url for a user from query_response."""
     user = query_response.user
     obs_args = query_response.obs_args()
     # TODO: use taxon_id common ancestor if multiple taxon_ids
     #       - see `,related`
     # TODO: use place_id smallest enclosing (major) place if multiple place_ids
     #       - no place hierarchy support yet in dronefly
+    url = f"{WWW_BASE_URL}/lifelists/{user.login}"
     lifelists_obs_args = {
         key: val
         for key in ("taxon_id", "place_id")
         if (val := obs_args.get(key)) and "," not in str(val)
     }
-    return f"{WWW_BASE_URL}/lifelists/{user.login}" f"?{urlencode(lifelists_obs_args)}"
+    if lifelists_obs_args:
+        url += f"?{urlencode(lifelists_obs_args)}"
+    return url
 
 
 def obs_url_from_v1(params: dict):
     """Observations query URL corresponding to /v1/observations API params."""
     url = WWW_BASE_URL + "/observations"
     if params:
         if "observed_on" in params:
```

### Comparing `dronefly_core-0.3.6.dev2/setup.py` & `dronefly_core-0.3.6.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20',
  'rich>=10.9,<14']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev2',
+    'version': '0.3.6.dev3',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev2/PKG-INFO` & `dronefly_core-0.3.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev2
+Version: 0.3.6.dev3
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

