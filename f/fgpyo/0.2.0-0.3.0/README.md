# Comparing `tmp/fgpyo-0.2.0.tar.gz` & `tmp/fgpyo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgpyo-0.2.0.tar", max compression
+gzip compressed data, was "fgpyo-0.3.0.tar", max compression
```

## Comparing `fgpyo-0.2.0.tar` & `fgpyo-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1634 2024-02-21 20:59:37.232697 fgpyo-0.2.0/LICENSE
--rw-r--r--   0        0        0     2407 2024-02-23 00:27:46.754369 fgpyo-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.233479 fgpyo-0.2.0/fgpyo/__init__.py
--rw-r--r--   0        0        0     4531 2024-02-21 20:59:37.233615 fgpyo-0.2.0/fgpyo/collections/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.233677 fgpyo-0.2.0/fgpyo/collections/tests/__init__.py
--rw-r--r--   0        0        0     1637 2024-02-21 20:59:37.233767 fgpyo-0.2.0/fgpyo/collections/tests/test_peekable_iterator.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.233829 fgpyo-0.2.0/fgpyo/fasta/__init__.py
--rwxr-xr-x   0        0        0     7989 2024-02-26 18:25:39.008754 fgpyo-0.2.0/fgpyo/fasta/builder.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.234012 fgpyo-0.2.0/fgpyo/fasta/tests/__init__.py
--rw-r--r--   0        0        0     2564 2024-02-22 17:46:43.926500 fgpyo-0.2.0/fgpyo/fasta/tests/test_builder.py
--rw-r--r--   0        0        0     4379 2024-02-23 16:49:19.056355 fgpyo-0.2.0/fgpyo/fastx/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.234318 fgpyo-0.2.0/fgpyo/fastx/tests/__init__.py
--rw-r--r--   0        0        0     8508 2024-02-21 20:59:37.234411 fgpyo-0.2.0/fgpyo/fastx/tests/test_fastx_zipped.py
--rw-r--r--   0        0        0     7807 2024-02-23 16:49:19.056570 fgpyo-0.2.0/fgpyo/io/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.234655 fgpyo-0.2.0/fgpyo/io/tests/_init__.py
--rw-r--r--   0        0        0     4467 2024-02-22 17:46:43.926642 fgpyo-0.2.0/fgpyo/io/tests/test_io.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.234771 fgpyo-0.2.0/fgpyo/py.typed
--rw-r--r--   0        0        0    14335 2024-02-23 16:49:19.056782 fgpyo-0.2.0/fgpyo/read_structure.py
--rw-r--r--   0        0        0    35090 2024-02-22 17:46:43.926920 fgpyo-0.2.0/fgpyo/sam/__init__.py
--rwxr-xr-x   0        0        0    27260 2024-02-23 16:49:19.057091 fgpyo-0.2.0/fgpyo/sam/builder.py
--rwxr-xr-x   0        0        0    16723 2024-02-21 20:59:37.235471 fgpyo-0.2.0/fgpyo/sam/clipping.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.235745 fgpyo-0.2.0/fgpyo/sam/tests/__init__.py
--rwxr-xr-x   0        0        0      282 2024-02-21 20:59:37.235920 fgpyo-0.2.0/fgpyo/sam/tests/data/unmapped.sam
--rwxr-xr-x   0        0        0     3461 2024-02-21 20:59:37.236015 fgpyo-0.2.0/fgpyo/sam/tests/data/valid.sam
--rwxr-xr-x   0        0        0    11469 2024-02-21 20:59:37.236135 fgpyo-0.2.0/fgpyo/sam/tests/test_builder.py
--rwxr-xr-x   0        0        0    15085 2024-02-21 20:59:37.236243 fgpyo-0.2.0/fgpyo/sam/tests/test_clipping.py
--rwxr-xr-x   0        0        0    12805 2024-02-22 17:46:43.927092 fgpyo-0.2.0/fgpyo/sam/tests/test_sam.py
--rw-r--r--   0        0        0     2404 2024-02-21 20:59:37.236444 fgpyo-0.2.0/fgpyo/sam/tests/test_supplementary_alignments.py
--rw-r--r--   0        0        0     4439 2024-02-22 17:46:43.927223 fgpyo-0.2.0/fgpyo/sam/tests/test_template_iterator.py
--rw-r--r--   0        0        0     1527 2024-02-21 20:59:37.236605 fgpyo-0.2.0/fgpyo/sequence.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.236675 fgpyo-0.2.0/fgpyo/tests/__init__.py
--rw-r--r--   0        0        0     9835 2024-02-22 17:46:43.927391 fgpyo-0.2.0/fgpyo/tests/test_read_structure.py
--rw-r--r--   0        0        0      473 2024-02-21 20:59:37.236849 fgpyo-0.2.0/fgpyo/tests/test_sequence.py
--rw-r--r--   0        0        0    13749 2024-02-26 19:07:40.786962 fgpyo-0.2.0/fgpyo/util/inspect.py
--rw-r--r--   0        0        0     6425 2024-02-23 00:27:46.755114 fgpyo-0.2.0/fgpyo/util/logging.py
--rw-r--r--   0        0        0    11528 2024-02-21 20:59:37.237212 fgpyo-0.2.0/fgpyo/util/metric.py
--rw-r--r--   0        0        0      822 2024-02-21 20:59:37.237277 fgpyo-0.2.0/fgpyo/util/string.py
--rw-r--r--   0        0        0        0 2024-02-21 20:59:37.237332 fgpyo-0.2.0/fgpyo/util/tests/__init__.py
--rw-r--r--   0        0        0     3293 2024-02-26 19:07:40.787262 fgpyo-0.2.0/fgpyo/util/tests/test_inspect.py
--rw-r--r--   0        0        0     1792 2024-02-22 17:46:43.927830 fgpyo-0.2.0/fgpyo/util/tests/test_logging.py
--rw-r--r--   0        0        0    10289 2024-02-22 17:46:43.927999 fgpyo-0.2.0/fgpyo/util/tests/test_metric.py
--rw-r--r--   0        0        0      581 2024-02-21 20:59:37.237608 fgpyo-0.2.0/fgpyo/util/tests/test_string.py
--rw-r--r--   0        0        0      275 2024-02-23 00:27:46.755302 fgpyo-0.2.0/fgpyo/util/tests/test_types.py
--rw-r--r--   0        0        0     5241 2024-02-23 00:27:46.755704 fgpyo-0.2.0/fgpyo/util/types.py
--rw-r--r--   0        0        0     3851 2024-02-23 16:49:19.057765 fgpyo-0.2.0/fgpyo/vcf/__init__.py
--rw-r--r--   0        0        0    15266 2024-02-22 17:46:43.928356 fgpyo-0.2.0/fgpyo/vcf/builder.py
--rw-r--r--   0        0        0    13048 2024-02-23 16:49:19.058028 fgpyo-0.2.0/fgpyo/vcf/tests/test_builder.py
--rw-r--r--   0        0        0     1502 2024-02-26 19:07:56.536757 fgpyo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 fgpyo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1634 2024-03-26 16:43:12.422074 fgpyo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2407 2024-03-26 16:43:12.422162 fgpyo-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.422957 fgpyo-0.3.0/fgpyo/__init__.py
+-rw-r--r--   0        0        0     4531 2024-03-26 16:43:12.423105 fgpyo-0.3.0/fgpyo/collections/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.423185 fgpyo-0.3.0/fgpyo/collections/tests/__init__.py
+-rw-r--r--   0        0        0     1637 2024-03-26 16:43:12.423269 fgpyo-0.3.0/fgpyo/collections/tests/test_peekable_iterator.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.423341 fgpyo-0.3.0/fgpyo/fasta/__init__.py
+-rwxr-xr-x   0        0        0     7989 2024-03-26 16:43:12.423456 fgpyo-0.3.0/fgpyo/fasta/builder.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.423523 fgpyo-0.3.0/fgpyo/fasta/tests/__init__.py
+-rw-r--r--   0        0        0     2564 2024-03-26 16:43:12.423621 fgpyo-0.3.0/fgpyo/fasta/tests/test_builder.py
+-rw-r--r--   0        0        0     4379 2024-03-26 16:43:12.423766 fgpyo-0.3.0/fgpyo/fastx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.423834 fgpyo-0.3.0/fgpyo/fastx/tests/__init__.py
+-rw-r--r--   0        0        0     8508 2024-03-26 16:43:12.423969 fgpyo-0.3.0/fgpyo/fastx/tests/test_fastx_zipped.py
+-rw-r--r--   0        0        0     7807 2024-04-11 00:03:12.967525 fgpyo-0.3.0/fgpyo/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.424259 fgpyo-0.3.0/fgpyo/io/tests/_init__.py
+-rw-r--r--   0        0        0     4467 2024-03-26 16:43:12.424358 fgpyo-0.3.0/fgpyo/io/tests/test_io.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.424395 fgpyo-0.3.0/fgpyo/py.typed
+-rw-r--r--   0        0        0    14335 2024-04-11 00:03:15.449874 fgpyo-0.3.0/fgpyo/read_structure.py
+-rw-r--r--   0        0        0    34980 2024-04-11 00:03:15.450895 fgpyo-0.3.0/fgpyo/sam/__init__.py
+-rwxr-xr-x   0        0        0    27260 2024-03-26 16:43:12.425154 fgpyo-0.3.0/fgpyo/sam/builder.py
+-rwxr-xr-x   0        0        0    16723 2024-03-26 16:43:12.425276 fgpyo-0.3.0/fgpyo/sam/clipping.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.425379 fgpyo-0.3.0/fgpyo/sam/tests/__init__.py
+-rwxr-xr-x   0        0        0      282 2024-03-26 16:43:12.425526 fgpyo-0.3.0/fgpyo/sam/tests/data/unmapped.sam
+-rwxr-xr-x   0        0        0     3461 2024-03-26 16:43:12.425617 fgpyo-0.3.0/fgpyo/sam/tests/data/valid.sam
+-rwxr-xr-x   0        0        0    11469 2024-03-26 16:43:12.425767 fgpyo-0.3.0/fgpyo/sam/tests/test_builder.py
+-rwxr-xr-x   0        0        0    15085 2024-03-26 16:43:12.426004 fgpyo-0.3.0/fgpyo/sam/tests/test_clipping.py
+-rwxr-xr-x   0        0        0    13028 2024-04-11 00:03:15.451223 fgpyo-0.3.0/fgpyo/sam/tests/test_sam.py
+-rw-r--r--   0        0        0     2404 2024-03-26 16:43:12.426294 fgpyo-0.3.0/fgpyo/sam/tests/test_supplementary_alignments.py
+-rw-r--r--   0        0        0     4439 2024-03-26 16:43:12.426361 fgpyo-0.3.0/fgpyo/sam/tests/test_template_iterator.py
+-rw-r--r--   0        0        0     1527 2024-03-26 16:43:12.426423 fgpyo-0.3.0/fgpyo/sequence.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.426482 fgpyo-0.3.0/fgpyo/tests/__init__.py
+-rw-r--r--   0        0        0     9835 2024-03-26 16:43:12.426595 fgpyo-0.3.0/fgpyo/tests/test_read_structure.py
+-rw-r--r--   0        0        0      473 2024-03-26 16:43:12.426658 fgpyo-0.3.0/fgpyo/tests/test_sequence.py
+-rw-r--r--   0        0        0    18470 2024-04-11 00:03:15.451482 fgpyo-0.3.0/fgpyo/util/inspect.py
+-rw-r--r--   0        0        0     6425 2024-03-26 16:43:12.427022 fgpyo-0.3.0/fgpyo/util/logging.py
+-rw-r--r--   0        0        0    12174 2024-04-11 00:03:15.451741 fgpyo-0.3.0/fgpyo/util/metric.py
+-rw-r--r--   0        0        0      822 2024-03-26 16:43:12.427227 fgpyo-0.3.0/fgpyo/util/string.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:43:12.427317 fgpyo-0.3.0/fgpyo/util/tests/__init__.py
+-rw-r--r--   0        0        0     4430 2024-04-11 00:03:15.452027 fgpyo-0.3.0/fgpyo/util/tests/test_inspect.py
+-rw-r--r--   0        0        0     1792 2024-03-26 16:43:12.427518 fgpyo-0.3.0/fgpyo/util/tests/test_logging.py
+-rw-r--r--   0        0        0    19317 2024-04-11 00:03:15.452212 fgpyo-0.3.0/fgpyo/util/tests/test_metric.py
+-rw-r--r--   0        0        0      581 2024-03-26 16:43:12.427904 fgpyo-0.3.0/fgpyo/util/tests/test_string.py
+-rw-r--r--   0        0        0      275 2024-03-26 16:43:12.427977 fgpyo-0.3.0/fgpyo/util/tests/test_types.py
+-rw-r--r--   0        0        0     5242 2024-04-11 00:03:15.452990 fgpyo-0.3.0/fgpyo/util/types.py
+-rw-r--r--   0        0        0     3851 2024-03-26 16:43:12.428313 fgpyo-0.3.0/fgpyo/vcf/__init__.py
+-rw-r--r--   0        0        0    15266 2024-03-26 16:43:12.428544 fgpyo-0.3.0/fgpyo/vcf/builder.py
+-rw-r--r--   0        0        0    13048 2024-03-26 16:43:12.428824 fgpyo-0.3.0/fgpyo/vcf/tests/test_builder.py
+-rw-r--r--   0        0        0     1502 2024-04-11 16:31:04.375102 fgpyo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 fgpyo-0.3.0/PKG-INFO
```

### Comparing `fgpyo-0.2.0/LICENSE` & `fgpyo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/README.md` & `fgpyo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/collections/__init__.py` & `fgpyo-0.3.0/fgpyo/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/collections/tests/test_peekable_iterator.py` & `fgpyo-0.3.0/fgpyo/collections/tests/test_peekable_iterator.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/fasta/builder.py` & `fgpyo-0.3.0/fgpyo/fasta/builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/fasta/tests/test_builder.py` & `fgpyo-0.3.0/fgpyo/fasta/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/fastx/__init__.py` & `fgpyo-0.3.0/fgpyo/fastx/__init__.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/fastx/tests/test_fastx_zipped.py` & `fgpyo-0.3.0/fgpyo/fastx/tests/test_fastx_zipped.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/io/__init__.py` & `fgpyo-0.3.0/fgpyo/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/io/tests/test_io.py` & `fgpyo-0.3.0/fgpyo/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/read_structure.py` & `fgpyo-0.3.0/fgpyo/read_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     Skip = "S"
     """The segment type for bases that need to be skipped."""
 
     def __str__(self) -> str:
         return self.value
 
 
-@attr.s(frozen=True, auto_attribs=True, kw_only=True)
+@attr.s(frozen=True, kw_only=True, auto_attribs=True)
 class SubReadWithoutQuals:
     """Contains the bases that correspond to the given read segment."""
 
     bases: str
     """The sub-read bases that correspond to the given read segment."""
 
     segment: "ReadSegment"
@@ -108,15 +108,15 @@
 
     @property
     def kind(self) -> SegmentType:
         """The kind of read segment that corresponds to this sub-read."""
         return self.segment.kind
 
 
-@attr.s(frozen=True, auto_attribs=True, kw_only=True)
+@attr.s(frozen=True, kw_only=True, auto_attribs=True)
 class SubReadWithQuals:
     """Contains the bases and qualities that correspond to the given read segment"""
 
     bases: str
     """The sub-read bases that correspond to the given read segment."""
 
     quals: str
@@ -127,15 +127,15 @@
 
     @property
     def kind(self) -> SegmentType:
         """The kind of read segment that corresponds to this sub-read."""
         return self.segment.kind
 
 
-@attr.s(frozen=True, auto_attribs=True, kw_only=True)
+@attr.s(frozen=True, kw_only=True, auto_attribs=True)
 class ReadSegment:
     """Encapsulates all the information about a segment within a read structure. A segment can
     either have a definite length, in which case length must be Some(Int), or an indefinite length
     (can be any length, 0 or more) in which case length must be None.
 
     Attributes:
         offset: The offset of the read segment in the read.
@@ -199,15 +199,15 @@
     def __str__(self) -> str:
         if self.has_fixed_length:
             return f"{self.length}{self.kind.value}"
         else:
             return f"{ANY_LENGTH_CHAR}{self.kind.value}"
 
 
-@attr.s(frozen=True, auto_attribs=True, kw_only=True)
+@attr.s(frozen=True, kw_only=True, auto_attribs=True)
 class ReadStructure(Iterable[ReadSegment]):
     """Describes the structure of a give read.  A read contains one or more read segments. A read
     segment describes a contiguous stretch of bases of the same type (ex. template bases) of some
     length and some offset from the start of the read.
 
     Attributes:
          segments: The segments composing the read structure
```

### Comparing `fgpyo-0.2.0/fgpyo/sam/__init__.py` & `fgpyo-0.3.0/fgpyo/sam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,31 +382,30 @@
 
     @property
     def is_clipping(self) -> bool:
         """Returns true if the operator is a soft/hard clip, false otherwise."""
         return self == CigarOp.S or self == CigarOp.H
 
 
-@attr.s(frozen=True, slots=True)
+@attr.s(frozen=True, slots=True, auto_attribs=True)
 class CigarElement:
     """Represents an element in a Cigar
 
     Attributes:
         - length (int): the length of the element
         - operator (CigarOp): the operator of the element
     """
 
-    length: int = attr.ib()
-    operator: CigarOp = attr.ib()
+    length: int
+    operator: CigarOp
 
-    @length.validator
-    def _validate_length(self, attribute: Any, value: int) -> None:
+    def __attrs_post_init__(self) -> None:
         """Validates the length attribute is greater than zero."""
-        if value <= 0:
-            raise ValueError(f"Cigar element must have a length > 0, found {value}")
+        if self.length <= 0:
+            raise ValueError(f"Cigar element must have a length > 0, found {self.length}")
 
     @property
     def length_on_query(self) -> int:
         """Returns the length of the element on the query sequence."""
         return self.length if self.operator.consumes_query else 0
 
     @property
@@ -420,23 +419,23 @@
 
 class CigarParsingException(Exception):
     """The exception raised specific to parsing a cigar."""
 
     pass
 
 
-@attr.s(frozen=True, slots=True)
+@attr.s(frozen=True, slots=True, auto_attribs=True)
 class Cigar:
     """Class representing a cigar string.
 
     Attributes:
         - elements (Tuple[CigarElement, ...]): zero or more cigar elements
     """
 
-    elements: Tuple[CigarElement, ...] = attr.ib(default=())
+    elements: Tuple[CigarElement, ...] = ()
 
     @classmethod
     def from_cigartuples(cls, cigartuples: Optional[List[Tuple[int, int]]]) -> "Cigar":
         """Returns a Cigar from a list of tuples returned by pysam.
 
         Each tuple denotes the operation and length.  See
         :class:`~fgpyo.sam.CigarOp` for more information on the
@@ -515,33 +514,33 @@
         return sum([elem.length_on_query for elem in self.elements])
 
     def length_on_target(self) -> int:
         """Returns the length of the alignment on the target sequence."""
         return sum([elem.length_on_target for elem in self.elements])
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@attr.s(frozen=True, auto_attribs=True)
 class SupplementaryAlignment:
     """Stores a supplementary alignment record produced by BWA and stored in the SA SAM tag.
 
     Attributes:
         reference_name: the name of the reference (i.e. contig, chromosome) aligned to
         start: the 0-based start position of the alignment
         is_forward: true if the alignment is in the forward strand, false otherwise
         cigar: the cigar for the alignment
         mapq: the mapping quality
         nm: the number of edits
     """
 
-    reference_name: str = attr.ib()
-    start: int = attr.ib()
-    is_forward: bool = attr.ib()
-    cigar: Cigar = attr.ib()
-    mapq: int = attr.ib()
-    nm: int = attr.ib()
+    reference_name: str
+    start: int
+    is_forward: bool
+    cigar: Cigar
+    mapq: int
+    nm: int
 
     def __str__(self) -> str:
         return ",".join(
             str(item)
             for item in (
                 self.reference_name,
                 self.start + 1,
@@ -635,15 +634,15 @@
         dest.set_tag("MC", src.cigarstring)
 
     insert_size = isize(r1, r2)
     r1.template_length = insert_size
     r2.template_length = -insert_size
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@attr.s(frozen=True, auto_attribs=True)
 class ReadEditInfo:
     """
     Counts various stats about how a read compares to a reference sequence.
 
     Attributes:
         matches: the number of bases in the read that match the reference
         mismatches: the number of mismatches between the read sequence and the reference sequence
@@ -724,15 +723,15 @@
         inserted_bases=ins_bases,
         deletions=deletions,
         deleted_bases=del_bases,
         nm=mms + ins_bases + del_bases,
     )
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@attr.s(frozen=True, auto_attribs=True)
 class Template:
     """A container for alignment records corresponding to a single sequenced template
     or insert.
 
     It is strongly preferred that new Template instances be created with `Template.build()`
     which will ensure that reads are stored in the correct Template property, and run basic
     validations of the Template by default.  If constructing Template instances by construction
```

### Comparing `fgpyo-0.2.0/fgpyo/sam/builder.py` & `fgpyo-0.3.0/fgpyo/sam/builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sam/clipping.py` & `fgpyo-0.3.0/fgpyo/sam/clipping.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sam/tests/data/valid.sam` & `fgpyo-0.3.0/fgpyo/sam/tests/data/valid.sam`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sam/tests/test_builder.py` & `fgpyo-0.3.0/fgpyo/sam/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sam/tests/test_clipping.py` & `fgpyo-0.3.0/fgpyo/sam/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sam/tests/test_sam.py` & `fgpyo-0.3.0/fgpyo/sam/tests/test_sam.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,20 @@
     operator = CigarOp.from_character(character)
     element = CigarElement(operator_length, operator)
     assert element.length == operator_length
     assert element.length_on_query == length_on_query
     assert element.length_on_target == length_on_target
 
 
+@pytest.mark.parametrize("character", ["M", "I", "D", "S"])
+def test_invalid_cigar_element(character: str) -> None:
+    with pytest.raises(ValueError):
+        CigarElement(-1, operator=CigarOp.from_character(character))
+
+
 @pytest.mark.parametrize(
     "cigartuples,cigarstring",
     [
         ([], "*"),  # Empty cigar
         ([(0, 10), (1, 5), (0, 1)], "10M5I1M"),  # A simple example
         ([(0, 10), (1, 5), (1, 5)], "10M5I5I"),  # do not join adjacent operators of the same type
         ([(op.code, op.code + 1) for op in CigarOp], "1M2I3D4N5S6H7P8=9X"),  # all operators
```

### Comparing `fgpyo-0.2.0/fgpyo/sam/tests/test_supplementary_alignments.py` & `fgpyo-0.3.0/fgpyo/sam/tests/test_supplementary_alignments.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sam/tests/test_template_iterator.py` & `fgpyo-0.3.0/fgpyo/sam/tests/test_template_iterator.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/sequence.py` & `fgpyo-0.3.0/fgpyo/sequence.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/tests/test_read_structure.py` & `fgpyo-0.3.0/fgpyo/tests/test_read_structure.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/util/inspect.py` & `fgpyo-0.3.0/fgpyo/util/inspect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,117 @@
-import functools
 import sys
+import types as python_types
 import typing
-from enum import Enum
-from functools import partial
-from pathlib import PurePath
 from typing import Any
-from typing import Callable
 from typing import Dict
+from typing import FrozenSet
 from typing import Iterable
 from typing import List
 from typing import Literal
-from typing import Optional
+from typing import Mapping
+from typing import Protocol
 from typing import Tuple
 from typing import Type
 from typing import Union
 
-if sys.version_info >= (3, 12):
+if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
-import attr
+import dataclasses
+import functools
+from dataclasses import MISSING as DATACLASSES_MISSING
+from dataclasses import fields as get_dataclasses_fields
+from dataclasses import is_dataclass as is_dataclasses_class
+from enum import Enum
+from functools import partial
+from pathlib import PurePath
+from typing import TYPE_CHECKING
+from typing import Callable
+from typing import Optional
+from typing import TypeVar
 
 import fgpyo.util.types as types
 
+attr: Optional[python_types.ModuleType]
+MISSING: FrozenSet[Any]
+
+try:
+    import attr
+
+    _use_attr = True
+    from attr import fields as get_attr_fields
+    from attr import fields_dict as get_attr_fields_dict
+
+    Attribute: TypeAlias = attr.Attribute  # type: ignore[name-defined, no-redef]
+    # dataclasses and attr have internal tokens for missing values, join into a set so that we can
+    # check if a value is missing without knowing the type of backing class
+    MISSING = frozenset({DATACLASSES_MISSING, attr.NOTHING})
+except ImportError:  # pragma: no cover
+    _use_attr = False
+    attr = None
+    Attribute: TypeAlias = TypeVar("Attribute", bound=object)  # type: ignore[misc, assignment, no-redef]  # noqa: E501
+
+    # define empty placeholders for getting attr fields as a tuple or dict. They will never be
+    # called because the import failed; but they're here to ensure that the function is defined in
+    # sections of code that don't know if the import was successful or not.
+
+    def get_attr_fields(cls: type) -> Tuple[dataclasses.Field, ...]:  # type: ignore[misc]
+        """Get tuple of fields for attr class. attrs isn't imported so return empty tuple."""
+        return ()
+
+    def get_attr_fields_dict(cls: type) -> Dict[str, dataclasses.Field]:  # type: ignore[misc]
+        """Get dict of name->field for attr class. attrs isn't imported so return empty dict."""
+        return {}
+
+    # for consistency with successful import of attr, create a set for missing values
+    MISSING = frozenset({DATACLASSES_MISSING})
+
+if TYPE_CHECKING:  # pragma: no cover
+    from _typeshed import DataclassInstance as DataclassesProtocol
+else:
+
+    class DataclassesProtocol(Protocol):
+        __dataclasses_fields__: Dict[str, dataclasses.Field]
+
+
+if TYPE_CHECKING and _use_attr:  # pragma: no cover
+    from attr import AttrsInstance
+else:
+
+    class AttrsInstance(Protocol):  # type: ignore[no-redef]
+        __attrs_attrs__: Dict[str, Any]
+
+
+def is_attr_class(cls: type) -> bool:  # type: ignore[arg-type]
+    """Return True if the class is an attr class, and False otherwise"""
+    return hasattr(cls, "__attrs_attrs__")
+
+
+_MISSING_OR_NONE: FrozenSet[Any] = frozenset({*MISSING, None})
+"""Set of values that are considered missing or None for dataclasses or attr classes"""
+_DataclassesOrAttrClass: TypeAlias = Union[DataclassesProtocol, AttrsInstance]
+"""
+TypeAlias for dataclasses or attr classes. Mostly nonsense because they are not true types, they
+are traits, but there is no python trait-tester.
+"""
+FieldType: TypeAlias = Union[dataclasses.Field, Attribute]
+"""
+TypeAlias for dataclass Fields or attrs Attributes. It will correspond to the correct type for the
+corresponding _DataclassesOrAttrClass
+"""
+
+
+def _get_dataclasses_fields_dict(
+    class_or_instance: Union[DataclassesProtocol, Type[DataclassesProtocol]],
+) -> Dict[str, dataclasses.Field]:
+    """Get a dict from field name to Field for a dataclass class or instance."""
+    return {field.name: field for field in get_dataclasses_fields(class_or_instance)}
+
 
 class ParserNotFoundException(Exception):
     pass
 
 
 def split_at_given_level(
     field: str,
@@ -63,15 +147,15 @@
         if outer_depth_of_split == 0:
             out_vals.append(split_delim.join(current_outer_splits))
             current_outer_splits = []
     assert outer_depth_of_split == 0, "Unpaired depth character! Likely incorrect output!"
     return out_vals
 
 
-NoneType = type(None)
+NoneType: TypeAlias = type(None)  # type: ignore[no-redef]
 
 
 def list_parser(
     cls: Type, type_: TypeAlias, parsers: Optional[Dict[type, Callable[[str], Any]]] = None
 ) -> partial:
     """
     Returns a function that parses a stringified list into a `List` of the correct type.
@@ -301,35 +385,66 @@
     # Set the name that the user expects to see in error messages (we always
     # return a temporary partial object so it's safe to set its __name__).
     # Unions and Literals don't have a __name__, but their str is fine.
     setattr(parser, "__name__", getattr(type_, "__name__", str(type_)))
     return parser
 
 
+def get_fields_dict(
+    cls: Union[_DataclassesOrAttrClass, Type[_DataclassesOrAttrClass]]
+) -> Mapping[str, FieldType]:
+    """Get the fields dict from either a dataclasses or attr dataclass (or instance)"""
+    if is_dataclasses_class(cls):
+        return _get_dataclasses_fields_dict(cls)  # type: ignore[arg-type]
+    elif is_attr_class(cls):  # type: ignore[arg-type]
+        return get_attr_fields_dict(cls)  # type: ignore[arg-type]
+    else:
+        raise TypeError("cls must a dataclasses or attr class")
+
+
+def get_fields(
+    cls: Union[_DataclassesOrAttrClass, Type[_DataclassesOrAttrClass]]
+) -> Tuple[FieldType, ...]:
+    """Get the fields tuple from either a dataclasses or attr dataclass (or instance)"""
+    if is_dataclasses_class(cls):
+        return get_dataclasses_fields(cls)  # type: ignore[arg-type]
+    elif is_attr_class(cls):  # type: ignore[arg-type]
+        return get_attr_fields(cls)  # type: ignore[arg-type]
+    else:
+        raise TypeError("cls must a dataclasses or attr class")
+
+
+_AttrFromType = TypeVar("_AttrFromType")
+"""TypeVar to allow attr_from to be used with either an attr class or a dataclasses class"""
+
+
 def attr_from(
-    cls: Type, kwargs: Dict[str, str], parsers: Optional[Dict[type, Callable[[str], Any]]] = None
-) -> Any:
-    """Builds an attr class from key-word arguments
+    cls: Type[_AttrFromType],
+    kwargs: Dict[str, str],
+    parsers: Optional[Dict[type, Callable[[str], Any]]] = None,
+) -> _AttrFromType:
+    """Builds an attr or dataclasses class from key-word arguments
 
     Args:
-        cls: the attr class to be built
+        cls: the attr or dataclasses class to be built
         kwargs: a dictionary of keyword arguments
         parsers: a dictionary of parser functions to apply to specific types
 
     """
     return_values: Dict[str, Any] = {}
-    for attribute in attr.fields(cls):
+    for attribute in get_fields(cls):  # type: ignore[arg-type]
         return_value: Any
         if attribute.name in kwargs:
             str_value: str = kwargs[attribute.name]
             set_value: bool = False
 
             # Use the converter if provided
-            if attribute.converter is not None:
-                return_value = attribute.converter(str_value)
+            converter = getattr(attribute, "converter", None)
+            if converter is not None:
+                return_value = converter(str_value)
                 set_value = True
 
             # try getting a known parser
             if not set_value:
                 try:
                     parser = _get_parser(cls=cls, type_=attribute.type, parsers=parsers)
                     return_value = parser(str_value)
@@ -348,30 +463,30 @@
                     pass
 
             # fail otherwise
             assert (
                 set_value
             ), f"Do not know how to convert string to {attribute.type} for value: {str_value}"
         else:  # no value, check for a default
-            assert attribute.default is not None or attribute_is_optional(
+            assert attribute.default is not None or _attribute_is_optional(
                 attribute
             ), f"No value given and no default for attribute `{attribute.name}`"
             return_value = attribute.default
             # when the default is attr.NOTHING, just use None
-            if return_value is attr.NOTHING:
+            if return_value in MISSING:
                 return_value = None
 
         return_values[attribute.name] = return_value
 
     return cls(**return_values)
 
 
-def attribute_is_optional(attribute: attr.Attribute) -> bool:
+def _attribute_is_optional(attribute: FieldType) -> bool:
     """Returns True if the attribute is optional, False otherwise"""
     return typing.get_origin(attribute.type) is Union and isinstance(
         None, typing.get_args(attribute.type)
     )
 
 
-def attribute_has_default(attribute: attr.Attribute) -> bool:
+def _attribute_has_default(attribute: FieldType) -> bool:
     """Returns True if the attribute has a default value, False otherwise"""
-    return attribute.default != attr.NOTHING or attribute_is_optional(attribute)
+    return attribute.default not in _MISSING_OR_NONE or _attribute_is_optional(attribute)
```

### Comparing `fgpyo-0.2.0/fgpyo/util/logging.py` & `fgpyo-0.3.0/fgpyo/util/logging.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/util/metric.py` & `fgpyo-0.3.0/fgpyo/util/metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,39 @@
 
 Metric files are tab-delimited, contain a header, and zero or more rows for metric values.  This
 makes it easy for them to be read in languages like `R`.  For example, a row per person, with
 columns for age, gender, and address.
 
 The :class:`~fgpyo.util.metric.Metric` class makes it easy to read, write, and store one or metrics
 of the same type, all the while preserving types for each value in a metric.  It is an abstract
-base class decorated by `attr <https://www.attrs.org/en/stable/examples.html>`_, with attributes
-storing one or more typed values.
+base class decorated by `@dataclass <https://docs.python.org/3/library/dataclasses.html>`_, or
+`@attr.s <https://www.attrs.org/en/stable/examples.html>`_, with attributes storing one or more
+typed values. If using multiple layers of inheritance, keep in mind that it's not possible to mix
+these dataclass utils, e.g. a dataclasses class derived from an attr class will not appropriately
+initialize the values of the attr superclass.
 
 Examples
 ~~~~~~~~
 
 Defining a new metric class:
 
 .. code-block:: python
 
    >>> from fgpyo.util.metric import Metric
+   >>> import dataclasses
+   >>> @dataclasses.dataclass(frozen=True)
+   ... class Person(Metric["Person"]):
+   ...     name: str
+   ...     age: int
+
+or using attr:
+
+.. code-block:: python
+
+   >>> from fgpyo.util.metric import Metric
    >>> import attr
    >>> @attr.s(auto_attribs=True, frozen=True)
    ... class Person(Metric["Person"]):
    ...     name: str
    ...     age: int
 
 Getting the attributes for a metric class.  These will be used for the header when reading and
@@ -71,23 +85,23 @@
 
 Formatting and parsing the values for custom types is supported by overriding the
 :func:`~fgpyo.util.metric.Metric._parsers` and
 :func:`~fgpyo.util.metric.Metric.format_value` methods.
 
 .. code-block:: python
 
-   >>> @attr.s(auto_attribs=True, frozen=True)
+   >>> @dataclasses.dataclass(frozen=True)
    ... class Name:
    ...     first: str
    ...     last: str
    ...     @classmethod
    ...     def parse(cls, value: str) -> "Name":
    ...          fields = value.split(" ")
    ...          return Name(first=fields[0], last=fields[1])
-   >>> @attr.s(auto_attribs=True, frozen=True)
+   >>> @dataclasses.dataclass(frozen=True)
    ... class Person(Metric["Person"]):
    ...     name: Name
    ...     age: int
    ...     def _parsers(cls) -> Dict[type, Callable[[str], Any]]:
    ...         return {Name: lambda value: Name.parse(value=value)}
    ...     @classmethod
    ...     def format_value(cls, value: Any) -> str:
@@ -109,37 +123,35 @@
 from typing import Callable
 from typing import Dict
 from typing import Generic
 from typing import Iterator
 from typing import List
 from typing import TypeVar
 
-import attr
-
 from fgpyo import io
 from fgpyo.util import inspect
 
 MetricType = TypeVar("MetricType", bound="Metric")
 
 
-@attr.s
 class Metric(ABC, Generic[MetricType]):
     """Abstract base class for all metric-like tab-delimited files
 
     Metric files are tab-delimited, contain a header, and zero or more rows for metric values.  This
     makes it easy for them to be read in languages like `R`.
 
     Sub-classes of :class:`~fgpyo.util.metric.Metric` can support parsing and formatting custom
     types with :func:`~fgpyo.util.metric.Metric._parsers` and
     :func:`~fgpyo.util.metric.Metric.format_value`.
     """
 
     def values(self) -> Iterator[Any]:
         """An iterator over attribute values in the same order as the header."""
-        return iter(attr.astuple(self, recurse=False))
+        for field in inspect.get_fields(self.__class__):  # type: ignore[arg-type]
+            yield getattr(self, field.name)
 
     def formatted_values(self) -> List[str]:
         """An iterator over formatted attribute values in the same order as the header."""
         return [self.format_value(value) for value in self.values()]
 
     @classmethod
     def _parsers(cls) -> Dict[type, Callable[[str], Any]]:
@@ -166,23 +178,23 @@
             header: List[str] = reader.readline().rstrip("\r\n").split("\t")
             # check the header
             class_fields = set(cls.header())
             file_fields = set(header)
             missing_from_class = file_fields.difference(class_fields)
             missing_from_file = class_fields.difference(file_fields)
 
-            field_name_to_attribute = attr.fields_dict(cls)
+            field_name_to_attribute = inspect.get_fields_dict(cls)  # type: ignore[arg-type]
 
             # ignore class fields that are missing from the file (via header) if they're optional
             # or have a default
             if len(missing_from_file) > 0:
                 fields_with_defaults = [
                     field
                     for field in missing_from_file
-                    if inspect.attribute_has_default(field_name_to_attribute[field])
+                    if inspect._attribute_has_default(field_name_to_attribute[field])
                 ]
                 # remove optional class fields from the fields
                 missing_from_file = missing_from_file.difference(fields_with_defaults)
 
             # raise an exception if there are non-optional class fields missing from the file
             if len(missing_from_file) > 0:
                 raise ValueError(
@@ -246,15 +258,15 @@
                 # implement format_value.
                 writer.write("\t".join(cls.format_value(item) for item in value.values()))
                 writer.write("\n")
 
     @classmethod
     def header(cls) -> List[str]:
         """The list of header values for the metric."""
-        return [a.name for a in attr.fields(cls)]
+        return [a.name for a in inspect.get_fields(cls)]  # type: ignore[arg-type]
 
     @classmethod
     def format_value(cls, value: Any) -> str:
         """The default method to format values of a given type.
 
         By default, this method will comma-delimit `list`, `tuple`, and `set` types, and apply
         `str` to all others.
```

### Comparing `fgpyo-0.2.0/fgpyo/util/string.py` & `fgpyo-0.3.0/fgpyo/util/string.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/util/tests/test_inspect.py` & `fgpyo-0.3.0/fgpyo/util/tests/test_inspect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,88 @@
+import dataclasses
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
 import attr
 import pytest
 
+from fgpyo.util.inspect import _attribute_has_default
+from fgpyo.util.inspect import _attribute_is_optional
 from fgpyo.util.inspect import attr_from
-from fgpyo.util.inspect import attribute_has_default
-from fgpyo.util.inspect import attribute_is_optional
 from fgpyo.util.inspect import dict_parser
+from fgpyo.util.inspect import get_fields
+from fgpyo.util.inspect import get_fields_dict
+from fgpyo.util.inspect import is_attr_class
+from fgpyo.util.inspect import is_dataclasses_class
 from fgpyo.util.inspect import list_parser
 from fgpyo.util.inspect import set_parser
 from fgpyo.util.inspect import tuple_parser
 
 
 @attr.s(auto_attribs=True, frozen=True)
 class Name:
     required: str
     custom_parser: str
+    converted: int = attr.field(converter=int)
     optional_no_default: Optional[str]
     optional_with_default_none: Optional[str] = None
     optional_with_default_some: Optional[str] = "foo"
 
 
 def test_attr_from() -> None:
     name = attr_from(
         cls=Name,
-        kwargs={"required": "required", "custom_parser": "before"},
+        kwargs={"required": "required", "custom_parser": "before", "converted": "42"},
         parsers={str: lambda value: "after" if value == "before" else value},
     )
     assert name.required == "required"
     assert name.custom_parser == "after"
+    assert name.converted == 42
     assert name.optional_no_default is None
     assert name.optional_with_default_none is None
     assert name.optional_with_default_some == "foo"
 
 
 def test_attribute_is_optional() -> None:
     fields_dict = attr.fields_dict(Name)
-    assert not attribute_is_optional(fields_dict["required"])
-    assert not attribute_is_optional(fields_dict["custom_parser"])
-    assert attribute_is_optional(fields_dict["optional_no_default"])
-    assert attribute_is_optional(fields_dict["optional_with_default_none"])
-    assert attribute_is_optional(fields_dict["optional_with_default_some"])
+    assert not _attribute_is_optional(fields_dict["required"])
+    assert not _attribute_is_optional(fields_dict["custom_parser"])
+    assert not _attribute_is_optional(fields_dict["converted"])
+    assert _attribute_is_optional(fields_dict["optional_no_default"])
+    assert _attribute_is_optional(fields_dict["optional_with_default_none"])
+    assert _attribute_is_optional(fields_dict["optional_with_default_some"])
 
 
 def test_attribute_has_default() -> None:
     fields_dict = attr.fields_dict(Name)
-    assert not attribute_has_default(fields_dict["required"])
-    assert not attribute_has_default(fields_dict["custom_parser"])
-    assert attribute_has_default(fields_dict["optional_no_default"])
-    assert attribute_has_default(fields_dict["optional_with_default_none"])
-    assert attribute_has_default(fields_dict["optional_with_default_some"])
+    assert not _attribute_has_default(fields_dict["required"])
+    assert not _attribute_has_default(fields_dict["custom_parser"])
+    assert not _attribute_has_default(fields_dict["converted"])
+    assert _attribute_has_default(fields_dict["optional_no_default"])
+    assert _attribute_has_default(fields_dict["optional_with_default_none"])
+    assert _attribute_has_default(fields_dict["optional_with_default_some"])
 
 
 class Foo:
     pass
 
 
 @attr.s(auto_attribs=True, frozen=True)
 class Bar:
     foo: Foo
 
 
+@dataclasses.dataclass(frozen=True)
+class Baz:
+    foo: Foo
+
+
 # Test for regression #94 - the call to attr_from succeeds when the check for None type
 # in inspect._get_parser is done incorrectly.
 def test_attr_from_custom_type_without_parser_fails() -> None:
     with pytest.raises(AssertionError):
         attr_from(
             cls=Bar,
             kwargs={"foo": ""},
@@ -101,7 +115,31 @@
     assert parser("{123;a}") == {123: "a"}
 
 
 def test_dict_parser_with_duplicate_keys() -> None:
     parser = dict_parser(Foo, Dict[int, str], {})
     with pytest.raises(ValueError):
         parser("{123;a,123;b}")
+
+
+def test_non_data_class_fails() -> None:
+    class NonDataClass:
+        x: int
+
+    with pytest.raises(TypeError):
+        get_fields_dict(NonDataClass)  # type: ignore
+
+    with pytest.raises(TypeError):
+        get_fields(NonDataClass)  # type: ignore
+
+    with pytest.raises(TypeError):
+        attr_from(cls=NonDataClass, kwargs={"x": "1"}, parsers={int: int})
+
+
+def test_is_attrs_is_dataclasses() -> None:
+    assert not is_attr_class(Foo)
+    assert not is_dataclasses_class(Foo)
+
+    assert is_attr_class(Bar)
+    assert not is_dataclasses_class(Bar)
+    assert is_dataclasses_class(Baz)
+    assert not is_attr_class(Baz)
```

### Comparing `fgpyo-0.2.0/fgpyo/util/tests/test_logging.py` & `fgpyo-0.3.0/fgpyo/util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/util/tests/test_string.py` & `fgpyo-0.3.0/fgpyo/util/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/util/types.py` & `fgpyo-0.3.0/fgpyo/util/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     if _is_optional(union):
         try:
             # mypy doesn't like functions that return None always, so return separately
             none_parser(value)
             return None
         except (ValueError, InspectException):
             pass
+
     for p in parsers:
         try:
             return p(value)
         except (ValueError, InspectException):
             pass
     raise ValueError(f"{value} could not be parsed as any of {union}")
```

### Comparing `fgpyo-0.2.0/fgpyo/vcf/__init__.py` & `fgpyo-0.3.0/fgpyo/vcf/__init__.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/vcf/builder.py` & `fgpyo-0.3.0/fgpyo/vcf/builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/fgpyo/vcf/tests/test_builder.py` & `fgpyo-0.3.0/fgpyo/vcf/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.2.0/pyproject.toml` & `fgpyo-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgpyo"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python bioinformatics and genomics library"
 authors = ["Nils Homer", "Tim Fennell", "Nathan Roach"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fulcrumgenomics/fgpyo"
 repository = "https://github.com/fulcrumgenomics/fgpyo"
 keywords = ["bioinformatics"]
```

### Comparing `fgpyo-0.2.0/PKG-INFO` & `fgpyo-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgpyo
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python bioinformatics and genomics library
 Home-page: https://github.com/fulcrumgenomics/fgpyo
 License: MIT
 Keywords: bioinformatics
 Author: Nils Homer
 Requires-Python: >=3.8.0,<4.0
 Classifier: Development Status :: 3 - Alpha
```

