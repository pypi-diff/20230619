# Comparing `tmp/fastgedcom-0.0.5.tar.gz` & `tmp/fastgedcom-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-0.0.5.tar", last modified: Thu Jun  1 19:20:02 2023, max compression
+gzip compressed data, was "fastgedcom-0.0.6.tar", last modified: Mon Jun 19 15:21:41 2023, max compression
```

## Comparing `fastgedcom-0.0.5.tar` & `fastgedcom-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.447515 fastgedcom-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4231 2023-06-01 19:20:02.447515 fastgedcom-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3312 2023-06-01 19:19:11.000000 fastgedcom-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.394227 fastgedcom-0.0.5/fastgedcom/
--rw-rw-rw-   0        0        0        0 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0     9376 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/base.py
--rw-rw-rw-   0        0        0     7607 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/family_aid.py
--rw-rw-rw-   0        0        0     6033 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     4055 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/parser.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.5/fastgedcom/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.429462 fastgedcom-0.0.5/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     4231 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-06-01 19:20:02.000000 fastgedcom-0.0.5/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 19:12:40.000000 fastgedcom-0.0.5/fastgedcom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 19:20:02.447515 fastgedcom-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1408 2023-06-01 19:17:07.000000 fastgedcom-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.437001 fastgedcom-0.0.5/test/
--rw-rw-rw-   0        0        0      581 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_base.py
--rw-rw-rw-   0        0        0     3630 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_date_helpers.py
--rw-rw-rw-   0        0        0      592 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_helpers.py
--rw-rw-rw-   0        0        0     2758 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4561 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.010228 fastgedcom-0.0.6/fastgedcom/
+-rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-0.0.6/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0     9710 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/fastgedcom/base.py
+-rw-rw-rw-   0        0        0    10766 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/fastgedcom/family_link.py
+-rw-rw-rw-   0        0        0     9568 2023-06-19 15:12:18.000000 fastgedcom-0.0.6/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     5215 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/fastgedcom/parser.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.6/fastgedcom/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.024765 fastgedcom-0.0.6/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     4561 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-16 22:46:04.000000 fastgedcom-0.0.6/fastgedcom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       56 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1408 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/test/
+-rw-rw-rw-   0        0        0     1573 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_base.py
+-rw-rw-rw-   0        0        0     7527 2023-06-19 15:18:01.000000 fastgedcom-0.0.6/test/test_date_helpers.py
+-rw-rw-rw-   0        0        0     4632 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_family_link.py
+-rw-rw-rw-   0        0        0     1670 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_helpers.py
+-rw-rw-rw-   0        0        0     4605 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_parser.py
```

### Comparing `fastgedcom-0.0.5/LICENSE` & `fastgedcom-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.5/fastgedcom/base.py` & `fastgedcom-0.0.6/fastgedcom/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classes and types for the data structure used to represent a gedcom."""
 
-from typing import Iterator, Literal, TypeAlias, TypeGuard, Union
+from typing import Iterator, Literal, TypeAlias
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 
 SubmRef: TypeAlias = str
 """The cross-reference identifier of type '@SUB1@' or '@U1@' for a submitter
 of the document."""
 SubnRef: TypeAlias = str
@@ -38,56 +38,55 @@
 
 class Line(ABC):
 	"""Abstract base class for gedcom lines.
 
 	Implementations are :py:class:`.TrueLine` and :py:class:`.FakeLine`,
 	see these classes for more information.
 	"""
+	@abstractmethod
+	def __bool__(self) -> bool:
+		"""True if it is a :py:class:`.TrueLine`,
+		False if it is a :py:class:`.FakeLine`."""
 
 	@property
 	@abstractmethod
 	def payload(self) -> str:
 		"""See the description of :py:class:`.TrueLine` class."""
-		...
 
 	@property
 	@abstractmethod
 	def payload_with_cont(self) -> str:
 		"""The content of this gedcom field, namely the payload combined
 		with all CONT sub-lines payload as a new line, and
 		with all CONC sub-lines payload as a space."""
-		...
 
 	@abstractmethod
 	def get_sub_lines(self, tag: str) -> list['TrueLine']:
 		"""Return the all sub-lines having the given :any:`tag`.
 		An empty list if no line matches."""
-		...
 
 	def __rshift__(self, tag: str) -> list['TrueLine']:
 		"""Alias for :py:meth:`get_sub_lines` to shorten the syntax
 		by using the >> operator."""
 		return self.get_sub_lines(tag)
 
 	@abstractmethod
-	def get_sub_line(self, tag: str) -> Union['TrueLine', 'FakeLine']:
+	def get_sub_line(self, tag: str) -> 'TrueLine | FakeLine':
 		"""Return the first sub-line having the given :any:`tag`.
 		A :py:class:`.FakeLine` if no line matches."""
-		...
 
-	def __gt__(self, tag: str) -> Union['TrueLine', 'FakeLine']:
+	def __gt__(self, tag: str) -> 'TrueLine | FakeLine':
 		"""Alias for :py:meth:`get_sub_line` to shorten the syntax
 		by using the > operator."""
 		return self.get_sub_line(tag)
 
 	@abstractmethod
 	def get_sub_line_payload(self, tag: str) -> str:
 		"""Return the payload of the first sub-line having the given
 		:any:`tag`. An empty string if no line matches."""
-		...
 
 	def __ge__(self, tag: str) -> str:
 		"""Alias for :py:meth:`get_sub_line_payload` to shorten the syntax
 		by using the >= operator."""
 		return self.get_sub_line_payload(tag)
 
 
@@ -97,51 +96,50 @@
 	It allows the chaining of method calls. See these `examples
 	<https://github.com/GatienBouyer/fastgedcom/tree/main/examples>`_
 	for the usage of chaining.
 
 	The class behave like a :py:class:`.TrueLine`
 	(It has the same methods), but the payload is empty.
 
-	To differenciate a :py:class:`.FakeLine` from a
-	:py:class:`.TrueLine` a simple boolean test is enough:
-	:code:`if line: line.payload`. However to tell typecheckers that after
-	the test, the type is narrowed, you should use the :py:func:`is_true`
-	function. In general, the use of :py:meth:`get_sub_line_payload` (or ``>=``)
-	and then to check if the string is empty, is generally preferable.
+	To differentiate a :py:class:`.FakeLine` from a
+	:py:class:`.TrueLine` a simple boolean test is enough.
 	"""
 
-	payload = ""
-	payload_with_cont = ""
+	payload = "" # pyright: ignore[reportGeneralTypeIssues]
+	payload_with_cont = "" # pyright: ignore[reportGeneralTypeIssues]
 	sub_lines: list['TrueLine'] = []
 
+	def __bool__(self) -> Literal[False]:
+		"""Return False."""
+		return False
+
 	def get_sub_lines(self, tag: str) -> list['TrueLine']:
 		return []
 
 	def __rshift__(self, tag: str) -> list['TrueLine']:
 		return self.get_sub_lines(tag)
 
-	def get_sub_line(self, tag: str) -> Union['TrueLine', 'FakeLine']:
+	def get_sub_line(self, tag: str) -> 'TrueLine | FakeLine':
 		return fake_line
 
-	def __gt__(self, tag: str) -> Union['TrueLine', 'FakeLine']:
+	def __gt__(self, tag: str) -> 'TrueLine | FakeLine':
 		return self.get_sub_line(tag)
 
 	def get_sub_line_payload(self, tag: str) -> str:
 		return ""
 
 	def __ge__(self, tag: str) -> str:
 		return self.get_sub_line_payload(tag)
 
 	def __repr__(self) -> str:
 		"""Return the string representation of the class."""
 		return f"<{self.__class__.__qualname__}>"
 
-	def __bool__(self) -> bool:
-		"""Return False."""
-		return False
+	def __eq__(self, value: object) -> bool:
+		return isinstance(value, FakeLine)
 
 
 @dataclass(slots=True)
 class TrueLine(Line):
 	"""Represent a line of a gedcom document.
 
 	Contain the :py:attr:`sub-lines` of the gedcom structure.
@@ -169,40 +167,45 @@
 	gedcom standard. Use the :py:attr:`payload_with_cont` property to get the
 	complete multi-line payloads."""
 
 	sub_lines: list['TrueLine'] = field(default_factory=list)
 	"""List of the sub-lines, i.e. the next-level lines that are part
 	of this structure."""
 
+	def __bool__(self) -> Literal[True]:
+		"""Return True."""
+		return True
+
 	def get_sub_lines(self, tag: str) -> list['TrueLine']:
 		return [sub_line for sub_line in self.sub_lines if sub_line.tag == tag]
 
 	def __rshift__(self, tag: str) -> list['TrueLine']:
 		return self.get_sub_lines(tag)
 
-	def get_sub_line(self, tag: str) -> Union['TrueLine', 'FakeLine']:
+	def get_sub_line(self, tag: str) -> 'TrueLine | FakeLine':
 		for sub_line in self.sub_lines:
 			if sub_line.tag == tag:
 				return sub_line
 		return fake_line
 
-	def __gt__(self, tag: str) -> Union['TrueLine', 'FakeLine']:
+	def __gt__(self, tag: str) -> 'TrueLine | FakeLine':
 		return self.get_sub_line(tag)
 
 	def get_sub_line_payload(self, tag: str) -> str:
 		for sub_line in self.sub_lines:
 			if sub_line.tag == tag:
 				return sub_line.payload
 		return ""
 
 	def __ge__(self, tag: str) -> str:
 		return self.get_sub_line_payload(tag)
 
 	def __str__(self) -> str:
 		"""Return the gedcom representation of the line (sub-lines excluded)."""
+		if not self.payload: return f"{self.level} {self.tag}"
 		return f"{self.level} {self.tag} {self.payload}"
 
 	def __repr__(self) -> str:
 		"""Return the string representation of the class."""
 		return f"<{self.__class__.__qualname__} {self.level} {self.tag} {self.payload} -> {len(self.sub_lines)}>"
 
 	@property
@@ -232,35 +235,43 @@
 	of getting a :py:class:`.FakeLine`. Usefull when you a pretty sure of
 	the Record existing in the document."""
 
 	def __init__(self) -> None:
 		self.records = dict()
 
 	def __iter__(self) -> Iterator[Record]:
-		"""Iterate on the lines of level 0."""
+		"""Iterate on the lines of level 0
+		(the records, the header, and the TRLR line)."""
 		return iter(self.records.values())
 
+	def __contains__(self, identifier: XRef) -> bool:
+		"""Return True if the identifier refers to an existing record."""
+		return identifier in self.records
+
 	def get_records(self, record_type: str) -> Iterator[Record]:
-		"""Return an iterator over records of that ``record_type``."""
+		"""Return an iterator over records of that ``record_type``
+		(i.e. the :py:attr:`~.TrueLine.payload` of level 0 lines)."""
 		for record in self.records.values():
 			if record.payload == record_type:
 				yield record
 
+	__rshift__ = get_records
+	"""Alias for :py:meth:`get_records` to shorten the syntax
+	by using the >> operator."""
+
 	def get_record(self, identifier: XRef | Literal["HEAD"]) -> Record | FakeLine:
 		"""Return the record under that ``identifier``."""
 		return self.records.get(identifier, fake_line)
 
 	__getitem__ = get_record
 	"""Alias for :py:meth:`get_record` to shorten the syntax
 	by using the [] operator."""
 
+	def __eq__(self, __value: object) -> bool:
+		if not isinstance(__value, Document):
+			return False
+		return self.records == __value.records
+
 
 fake_line = FakeLine()
 """:py:class:`.FakeLine` instance returned by functions.
 Used to avoid having multiple unnecessary instances of :py:class:`.FakeLine`."""
-
-
-def is_true(line: Union[TrueLine, FakeLine]) -> TypeGuard[TrueLine]:
-	"""Return true when the given ``line`` is a :py:class:`.TrueLine`,
-	false when the given ``line`` is a :py:class:`.FakeLine`.
-	Usefull when using a typechecker."""
-	return bool(line)
```

### Comparing `fastgedcom-0.0.5/fastgedcom/family_aid.py` & `fastgedcom-0.0.6/fastgedcom/family_link.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Define the :py:class:`.FamilyAid` class used to bypass family records."""
+"""Define the :py:class:`.FamilyLink` class used to bypass family records."""
 
 from collections import defaultdict
 
 from .base import (Document, FakeLine, FamRef, IndiRef, Record, TrueLine,
-                   fake_line, is_true)
+                   fake_line)
 
 
-class FamilyAid():
-	"""Class with methods to easily get close relatives of someone.
+class FamilyLink():
+	"""Class with methods to easily get relatives of someone.
 
 	Methods ending in _ref (such as :py:meth:`.get_parent_family_ref`)
 	are called by their non-_ref counterparts (such as
 	:py:meth:`.get_parent_family`). Use the first set of methods when
 	you need performance. Use the second set of methods for convenience.
 
 	The class uses 2 dictionnaries to speed up the process.
@@ -22,43 +22,43 @@
 	Not all methods use those dictionnaries.
 	"""
 
 	def __init__(self, document: Document) -> None:
 		self.document = document
 		self.parents: dict[IndiRef, tuple[Record | FakeLine, Record | FakeLine]]
 		self.unions: defaultdict[IndiRef, list[Record]]
-		self._build_parents()
+		self._build_dicts()
 
-	def _build_parents(self) -> None:
+	def _build_dicts(self) -> None:
 		self.parents = dict()
 		self.unions = defaultdict(list)
 		for fam_record in self.document.records.values():
 			if fam_record.payload != "FAM": continue
 			children: list[IndiRef] = []
 			father: FakeLine | TrueLine = fake_line
 			mother: FakeLine | TrueLine = fake_line
 			for line in fam_record.sub_lines:
-				if line.payload == "": continue
+				if line.payload == "@VOID@": continue
 				if line.tag == "CHIL":
 					children.append(line.payload)
 				elif line.tag == "HUSB":
 					father = self.document.records[line.payload]
 					self.unions[father.tag].append(fam_record)
 				elif line.tag == "WIFE":
 					mother = self.document.records[line.payload]
 					self.unions[mother.tag].append(fam_record)
 			for child in children:
 				self.parents[child] = (father, mother)
 
 	def get_parent_family_ref(self, child: TrueLine | FakeLine) -> FamRef | None:
 		"""Return the family reference with the parents of the person."""
-		if not is_true(child): return None
+		if not child: return None
 		for sub_line in child.sub_lines:
 			if sub_line.tag == "FAMC":
-				if sub_line.payload == "": return None
+				if sub_line.payload == "@VOID@": return None
 				return sub_line.payload
 		return None
 
 	def get_parent_family(self, child: TrueLine | FakeLine) -> Record | FakeLine:
 		"""Return the family record with the parents of the person."""
 		fam_ref = self.get_parent_family_ref(child)
 		return self.document.records[fam_ref] if fam_ref else fake_line
@@ -73,26 +73,29 @@
 		"""Return the unions of the person."""
 		return [fam for fam in self.unions.get(spouse, [])]
 
 	def get_unions_with(self,
 		spouse1: IndiRef,
 		spouse2: IndiRef
 	) -> list[Record]:
-		"""Return the unions between the two people."""
+		"""Return the unions between the two people.
+
+		In most cases, there should be only one union, but
+		remarriage between the same two people could happen."""
 		spouse_fams = self.unions.get(spouse1, [])
 		return [fam
 			for fam in self.unions.get(spouse2, [])
 			if fam in spouse_fams]
 
 	def get_children_ref(self, parent: IndiRef) -> list[IndiRef]:
 		"""Return the children's references of a person."""
 		unions = self.unions.get(parent, [])
 		return [sub_line.payload
 			for fam in unions for sub_line in fam.sub_lines
-			if sub_line.tag == "CHIL" and sub_line.payload != ""]
+			if sub_line.tag == "CHIL" and sub_line.payload != "@VOID@"]
 
 	def get_children(self, parent: IndiRef) -> list[Record]:
 		"""Return the children's records of a person."""
 		return [self.document.records[child]
 			for child in self.get_children_ref(parent)]
 
 	def get_children_with_ref(self,
@@ -100,88 +103,89 @@
 		spouse2: IndiRef
 	) -> list[IndiRef]:
 		"""Return the children's references of the couple."""
 		fams = self.unions.get(spouse1, [])
 		unions = [fam for fam in self.unions.get(spouse2, []) if fam in fams]
 		return [sub_line.payload
 			for fam in unions for sub_line in fam.sub_lines
-			if sub_line.tag == "CHIL" and sub_line.payload != ""]
+			if sub_line.tag == "CHIL" and sub_line.payload != "@VOID@"]
 
 	def get_children_with(self,
 		spouse1: IndiRef,
 		spouse2: IndiRef
 	) -> list[Record]:
 		"""Return the children's records of the couple."""
 		return [self.document.records[child]
 			for child in self.get_children_with_ref(spouse1, spouse2)]
 
 	def get_spouses_ref(self, indi: IndiRef) -> list[IndiRef]:
 		"""Return the spouses' references of the person."""
 		return [sub_line.payload
 			for fam in self.unions.get(indi, []) for sub_line in fam.sub_lines
 			if (sub_line.tag in ("HUSB", "WIFE") and sub_line.payload != indi
-				and sub_line.payload != "")]
+				and sub_line.payload != "@VOID@")]
 
 	def get_spouses(self, indi: IndiRef) -> list[Record]:
 		"""Return the spouses' records of the person."""
 		return [self.document.records[spouse]
 			for spouse in self.get_spouses_ref(indi)]
 
 	def get_all_siblings_ref(self, indi: IndiRef) -> list[IndiRef]:
 		"""Return the siblings' references of the person.
 		Stepsiblings included."""
 		father, mother = self.get_parents(indi)
 		unions: list[Record] = []
-		if is_true(father):
+		if father:
 			unions.extend(self.unions.get(father.tag, []))
-		if is_true(mother):
-			unions.extend(self.unions.get(mother.tag, []))
+		if mother:
+			unions.extend(u for u in self.unions.get(mother.tag, [])
+				if u not in unions) # remove duplicates
 		return [sub_line.payload
 			for fam in unions
 			for sub_line in fam.sub_lines
-			if (sub_line.tag == "CHIL" and sub_line.payload != ""
+			if (sub_line.tag == "CHIL" and sub_line.payload != "@VOID@"
 				and sub_line.payload != indi)]
 
 	def get_all_siblings(self, indi: IndiRef) -> list[Record]:
 		"""Return the siblings' records of the person.
 		Stepsiblings included."""
 		return [self.document.records[sibling]
 			for sibling in self.get_all_siblings_ref(indi)]
 
 	def get_siblings_ref(self, indi: IndiRef) -> list[IndiRef]:
 		"""Return the siblings' references of the person.
 		Stepsiblings excluded."""
 		fam = self.get_parent_family(self.document.records[indi])
 		return [sub_line.payload
 			for sub_line in fam.sub_lines
-			if (sub_line.tag == "CHIL" and sub_line.payload != ""
+			if (sub_line.tag == "CHIL" and sub_line.payload != "@VOID@"
 				and sub_line.payload != indi)]
 
 	def get_siblings(self, indi: IndiRef) -> list[Record]:
 		"""Return the siblings' records of the person.
 		Stepsiblings excluded."""
 		return [self.document.records[sibling]
 			for sibling in self.get_siblings_ref(indi)]
 
 	def get_stepsiblings_ref(self, indi: IndiRef) -> list[IndiRef]:
 		"""Return the stepsiblings' references of the person.
 		Siblings excluded."""
 		parent_fam = self.get_parent_family_ref(self.document.records[indi])
 		father, mother = self.get_parents(indi)
 		unions: list[Record] = []
-		if is_true(father):
+		if father:
 			unions.extend(self.unions.get(father.tag, []))
-		if is_true(mother):
+		if mother:
 			unions.extend(self.unions.get(mother.tag, []))
 		stepsiblings: list[IndiRef] = []
 		for fam in unions:
 			if fam.tag != parent_fam:
 				stepsiblings.extend(sub_line.payload
 					for sub_line in fam.sub_lines
-					if sub_line.tag == "CHIL" and sub_line.payload != "")
+					if sub_line.tag == "CHIL" and sub_line.payload != "@VOID@")
 		return stepsiblings
 
 	def get_stepsiblings(self, indi: IndiRef) -> list[Record]:
 		"""Return the stepsiblings of the person.
 		Siblings excluded."""
 		return [self.document.records[stepsibling]
 			for stepsibling in self.get_stepsiblings_ref(indi)]
@@ -192,7 +196,88 @@
 		wife = fam >= "WIFE"
 		if wife == indi: return husban
 		return wife
 
 	def get_spouse_in_fam(self, indi: IndiRef, fam: Record) -> Record:
 		"""Return the spouse's record of the family that is not the person's."""
 		return self.document.records[self.get_spouse_in_fam_ref(indi, fam)]
+
+	def traverse_ref(self, indi: IndiRef,
+			ascent: int = 0, descent: int = 0
+			) -> list[IndiRef]:
+		"""
+		Recursively traverse the parents of the person and then their children.
+
+		The degree of kinship is equal to the sum `ascent` + `descent`.
+		"""
+		parents = [indi]
+		last_parents = [indi]
+		for _ in range(ascent):
+			last_parents = parents
+			parents = [p.tag for i in parents for p in self.get_parents(i) if p]
+		children = parents
+		for k in range(descent):
+			children = [c for i in children for c in self.get_children_ref(i)
+				if c not in last_parents]
+			if k == 0 and ascent == 1: # remove duplicates
+				children = list(set(children))
+		return children
+
+	def traverse(self, indi: IndiRef,
+			ascent: int = 0, descent: int = 0
+			) -> list[Record]:
+		"""
+		Recursively traverse the parents of the person and then their children.
+
+		The degree of kinship is equal to the sum `ascent` + `descent`.
+		"""
+		return [self.document.records[r]
+			for r in self.traverse_ref(indi, ascent, descent)]
+
+	def get_relatives_ref(self, indi: IndiRef,
+			generation_diff: int = 0, collateral_diff: int = 0
+			) -> list[IndiRef]:
+		"""Return relatives's references of the person.
+		See :py:meth:`get_relatives` for more details.
+		"""
+		if generation_diff >= 0: pos_gen = generation_diff ; neg_gen = 0
+		else: pos_gen = 0 ; neg_gen = -generation_diff
+		return self.traverse_ref(indi,
+			pos_gen + collateral_diff, neg_gen + collateral_diff)
+
+	def get_relatives(self, indi: IndiRef,
+			generation_diff: int = 0, collateral_diff: int = 0
+			) -> list[Record]:
+		"""Return relatives of the person.
+
+		`generation_diff` stand for generation difference:
+
+		* 1 parents, 2 grandparents, -1 children, -2 grand-children, ...
+
+		`collateral_diff` is used for same-generation difference:
+
+		* 1 sibling, 2 cousins, 3 grand-counsins, ...
+
+		The combinaison can be read as:
+
+		* (when generation_diff > 0) `collateral_diff` of `generation_diff`
+		* (when generation_diff < 0) `generation_diff` of `collateral_diff`
+
+		The `collateral_diff` must be strictly positive.
+		This function is a wrapper around :py:meth:`traverse`.
+		"""
+		if generation_diff >= 0: pos_gen = generation_diff ; neg_gen = 0
+		else: pos_gen = 0 ; neg_gen = -generation_diff
+		return self.traverse(indi,
+			pos_gen + collateral_diff, neg_gen + collateral_diff)
+
+	def get_by_degree_ref(self, indi: IndiRef, degree: int) -> list[IndiRef]:
+		"""Return relatives having that degree of kinship with the person."""
+		return [p for ascent in range(degree+1) for descent in range(degree+1)
+			for p in self.traverse_ref(indi, ascent,descent)
+			if ascent + descent == degree]
+
+	def get_by_degree(self, indi: IndiRef, degree: int) -> list[Record]:
+		"""Return relatives having that degree of kinship with the person."""
+		return [p for ascent in range(degree+1) for descent in range(degree+1)
+			for p in self.traverse(indi, ascent, descent)
+			if ascent + descent == degree]
```

### Comparing `fastgedcom-0.0.5/fastgedcom/parser.py` & `fastgedcom-0.0.6/fastgedcom/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,119 @@
 """Functions to parse gedcom files into :py:class:`.Document`.
 
 On module import, register the ansel and gedcom codecs from the `ansel python library
 <https://pypi.org/project/ansel/>`_.
 """
 
-from typing import IO
+from typing import Iterable
+from dataclasses import dataclass
 from pathlib import Path
 
-import ansel # type: ignore[import]
+import ansel  # type: ignore[import]
 
 from .base import Document, TrueLine, XRef
 
 ansel.register()
 
 class ParsingError(Exception):
-	"""Error raised by :py:func:`.parse`."""
+	"""Error raise by :py:func:`.strict_parse`."""
+
+class NothingParsed(ParsingError):
+	"""Raised by :py:func:`.strict_parse` when the resulting document is empty."""
 
 class ParsingWarning():
 	"""Base warning class."""
 
+@dataclass
 class LineParsingWarning(ParsingWarning):
-	"""Warn about an unparsable line."""
-	def __init__(self, line_number: int, line_content: str) -> None:
-		self.line_number = line_number
-		self.line_content = line_content
-	def __repr__(self) -> str:
-		return f"<{self.__class__.__qualname__} line {self.line_number}>"
+	"""Warn about a line with a single word.
+	There should be at least a line level and a tag."""
+	line_number: int
+	line_content: str
 
-class DuplicateParsingWarning(ParsingWarning):
+@dataclass
+class DuplicateXRefWarning(ParsingWarning):
 	"""Warn about a cross-reference identifier that is defined twice."""
-	def __init__(self, xref: XRef) -> None:
-		self.xref = xref
-	def __repr__(self) -> str:
-		return f"<{self.__class__.__qualname__} xref={self.xref}>"
+	xref: XRef
+
+@dataclass
+class LevelInconsistencyWarning(ParsingWarning):
+	"""Warn about a line without correct parent line."""
+	line_number: int
+
+@dataclass
+class LevelParsingWarning(ParsingWarning):
+	"""Warn about an unparsable line level."""
+	line_number: int
+
+@dataclass
+class EmptyLineWarning(ParsingWarning):
+	"""Warn about an empty line."""
+	line_number: int
+
+@dataclass
+class CharacterInsteadOfLineWarning(ParsingWarning):
+	"""Warn about the presents of a 1-character-long line.
+	This happens when the object parsed is an iterable on characters,
+	whereas an iterable on lines is expected."""
+	line_number: int
 
-def parse(readable_lines: IO[str]) -> tuple[Document, list[ParsingWarning]]:
+def parse(lines: Iterable[str]) -> tuple[Document, list[ParsingWarning]]:
 	"""Parse the text input to create the
 	:py:class:`.Document` object.
 
-	For major failure, raise :py:exc:`.ParsingError`.
+	List of possible :py:class:`.ParsingWarning`:
 
-	For minor failure, append a :py:class:`.ParsingWarning` to the returned list.
+	* :py:class:`.LineParsingWarning`
+	* :py:class:`.DuplicateXRefWarning`
+	* :py:class:`.LevelInconsistencyWarning`
+	* :py:class:`.LevelParsingWarning`
+	* :py:class:`.EmptyLineWarning`
+	* :py:class:`.CharacterInsteadOfLineWarning`
 
-	Non-exhaustive list of possible failures:
-
-	* (Major) First line word can't be converted to an integer.
-	* (Minor) Line with a single word. :py:class:`.LineParsingWarning`
-	* (Minor) A cross-reference identifier is defined twice. :py:class:`.DuplicateParsingWarning`
-	* (Major) Inconsistent use of line level.
+	Only :py:class:`.CharacterInsteadOfLineWarning` stops the parsing. If
+	other warnings occur, the parsing continues with the next line.
 	"""
 	document = Document()
 	warnings: list[ParsingWarning] = []
 	line_number = 0
-	try:
-		parent_lines: list[TrueLine] = []
-		for line in readable_lines:
-			line_number += 1
-			line_info = line.rstrip().split(' ', 2)
+	parent_lines: list[TrueLine] = []
+	for line in lines:
+		line_number += 1
+		line_info = line.rstrip().split(' ', 2)
+		try:
 			if len(line_info) == 3:
 				parsed_line = TrueLine(int(line_info[0]), line_info[1], line_info[2], [])
 			elif len(line_info) == 2:
 				parsed_line = TrueLine(int(line_info[0]), line_info[1], "", [])
 			elif line_info == [""]:
-				# empty line is ok
+				warnings.append(EmptyLineWarning(line_number))
 				continue
 			else:
+				if len(line) == 1:
+					warnings.append(CharacterInsteadOfLineWarning(line_number))
+					break
 				warnings.append(LineParsingWarning(line_number, line))
 				continue
-			if parsed_line.level == 0:
-				parent_lines = [parsed_line]
-				if parsed_line.tag in document.records:
-					warnings.append(DuplicateParsingWarning(parsed_line.tag))
-				document.records[parsed_line.tag] = parsed_line
+		except ValueError:
+			warnings.append(LevelParsingWarning(line_number))
+			continue
+		if parsed_line.level == 0:
+			parent_lines = [parsed_line]
+			if parsed_line.tag in document.records:
+				warnings.append(DuplicateXRefWarning(parsed_line.tag))
+			document.records[parsed_line.tag] = parsed_line
+		else:
+			while parent_lines and parsed_line.level <= parent_lines[-1].level:
+				parent_lines.pop(-1)
+			if len(parent_lines) == 0:
+				warnings.append(LevelInconsistencyWarning(line_number))
 			else:
-				while parent_lines and parsed_line.level <= parent_lines[-1].level:
-					parent_lines.pop(-1)
-				if len(parent_lines) == 0: raise ParsingError("Inconsistent use of line levels")
 				parent_lines[-1].sub_lines.append(parsed_line)
 				parent_lines.append(parsed_line)
-	except ValueError as err: # raised on int parsing error
-		raise ParsingError(line_number, "Line parsing failed") from err
 	return (document, warnings)
 
 def guess_encoding(file: str | Path) -> str | None:
 	"""Return the guessed encoding of the ``file``. None if unknown.
 
 	No proper detection of the encoding of a file is ever possible.
 
@@ -93,24 +123,37 @@
 	However, indication of that field are often misleading. For example:
 	ANSEL refers to the gedcom version of the ansel charset.
 	The BOM mark is never mention and isn't automatically detected by Python.
 	UNICODE is not recognized by Python and should be manually set to UTF-16.
 	"""
 	try:
 		with open(file, "r", encoding="utf-8-sig") as f:
-			f.read()
-	except UnicodeDecodeError: pass
+			if "�" in f.read(): raise UnicodeError
+	except UnicodeError: pass
 	else: return "utf-8-sig"
 	try:
 		with open(file, "r", encoding=None) as f:
 			for line in f:
 				if line.startswith("1 CHAR "):
 					if "ansel" in line.lower(): return "gedcom"
 					return line[7:-1] # tested with "ansi"
-	except UnicodeDecodeError: pass
+	except UnicodeError: pass
 	try:
 		with open(file, "r", encoding="utf-16") as f:
-			f.read()
-	except UnicodeDecodeError: pass
+			if "�" in f.read(): raise UnicodeError
+	except UnicodeError: pass
 	else: return "utf-16"
 	return None
 
+def strict_parse(file: str | Path) -> Document:
+	"""Open and parse the gedcom file.
+	Return the :py:class:`.Document` representing the gedcom file.
+
+	Raise :py:exc:`.ParsingError` when a error occurs in the parsing process.
+	Raise :py:exc:`.NothingParsed` when the input is empty or isn't gedcom.
+	"""
+	with open(file, "r", encoding=guess_encoding(file)) as f:
+		document, warnings = parse(f)
+	if warnings: raise ParsingError(warnings)
+	if len(document.records) == 0: raise NothingParsed()
+
+	return document
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastgedcom-0.0.5/setup.py` & `fastgedcom-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 	requirements = f.readlines()
 
 with open("requirements-dev.txt", "r") as f:
 	requirements_dev = f.readlines()
 
 setup(
 	name="fastgedcom",
-	version="0.0.5",
+	version="0.0.6",
 	description="A lightweight tool to parse, browse and edit gedcom files.",
 	packages=["fastgedcom"],
 	package_data={"fastgedcom": ["py.typed"]},
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	zip_safe=False,
 	install_requires=requirements,
```

