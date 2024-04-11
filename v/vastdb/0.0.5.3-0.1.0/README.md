# Comparing `tmp/vastdb-0.0.5.3.tar.gz` & `tmp/vastdb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.0.5.3.tar", last modified: Sun Mar 24 17:42:07 2024, max compression
+gzip compressed data, was "vastdb-0.1.0.tar", last modified: Wed Apr 10 18:33:22 2024, max compression
```

## Comparing `vastdb-0.0.5.3.tar` & `vastdb-0.1.0.tar`

### file list

```diff
@@ -1,173 +1,188 @@
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.320700 vastdb-0.0.5.3/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    11333 2023-12-17 10:00:47.000000 vastdb-0.0.5.3/LICENSE
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1237 2024-03-24 17:42:07.320461 vastdb-0.0.5.3/PKG-INFO
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    46084 2024-03-19 07:59:27.000000 vastdb-0.0.5.3/README.md
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-03-24 17:42:07.320768 vastdb-0.0.5.3/setup.cfg
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1855 2024-03-24 16:09:48.000000 vastdb-0.0.5.3/setup.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.280395 vastdb-0.0.5.3/vast_flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.280526 vastdb-0.0.5.3/vast_flatbuf/org/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.280670 vastdb-0.0.5.3/vast_flatbuf/org/apache/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.280797 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.280936 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.297392 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5630 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2212 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1567 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2494 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      182 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4434 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2429 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2520 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      236 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3490 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1059 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2576 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      484 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2258 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      498 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1584 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2850 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3260 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2602 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1515 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      186 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2403 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1487 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2197 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      211 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1578 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4455 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      230 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2309 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3368 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2400 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2797 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      682 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3284 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1723 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2392 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3847 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      349 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2378 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3941 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1526 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2113 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      315 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      217 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3678 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3952 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2221 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5650 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1533 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1593 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2539 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1529 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1051 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7527 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.313371 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1026 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1326 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2310 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      836 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1430 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      155 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1760 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      149 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2855 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3148 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4091 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      410 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      267 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1289 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7048 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1669 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1589 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1569 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1541 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6448 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1925 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      180 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1131 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2541 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4486 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      671 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      786 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1054 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      161 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5589 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6042 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      162 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5785 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6091 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      226 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6389 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     9409 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1193 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5767 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2149 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2639 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      191 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7925 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      698 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3142 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      147 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1023 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.318204 vastdb-0.0.5.3/vast_flatbuf/tabular/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2114 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2222 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1618 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1610 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/AlterTableRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1901 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/Column.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      151 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/ColumnType.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2516 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1626 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3474 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2732 2024-02-21 20:33:08.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2450 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/ImportDataRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4240 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3036 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3550 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/ListTablesResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3589 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/ObjectDetails.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4450 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/S3File.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.0.5.3/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.319286 vastdb-0.0.5.3/vastdb/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-03-17 20:02:43.000000 vastdb-0.0.5.3/vastdb/__init__.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)   124883 2024-03-24 16:06:02.000000 vastdb-0.0.5.3/vastdb/api.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1208 2024-03-24 17:08:31.000000 vastdb-0.0.5.3/vastdb/bench_scan.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-03-24 17:42:07.320230 vastdb-0.0.5.3/vastdb.egg-info/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1237 2024-03-24 17:42:07.000000 vastdb-0.0.5.3/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     8513 2024-03-24 17:42:07.000000 vastdb-0.0.5.3/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        1 2024-03-24 17:42:07.000000 vastdb-0.0.5.3/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       57 2024-03-24 17:42:07.000000 vastdb-0.0.5.3/vastdb.egg-info/requires.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       20 2024-03-24 17:42:07.000000 vastdb-0.0.5.3/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.986759 vastdb-0.1.0/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)    11333 2023-12-17 10:00:47.000000 vastdb-0.1.0/LICENSE
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-10 18:33:22.986595 vastdb-0.1.0/PKG-INFO
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5891 2024-04-10 18:32:20.000000 vastdb-0.1.0/README.md
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-04-10 18:33:22.986822 vastdb-0.1.0/setup.cfg
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1699 2024-04-10 18:32:20.000000 vastdb-0.1.0/setup.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.945854 vastdb-0.1.0/vast_flatbuf/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.945979 vastdb-0.1.0/vast_flatbuf/org/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.946099 vastdb-0.1.0/vast_flatbuf/org/apache/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.946228 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.946358 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.961830 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5630 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2212 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1567 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2494 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      182 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4434 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2429 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2520 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      236 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3490 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1059 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2576 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      484 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2258 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      498 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1584 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2850 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3260 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2602 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1515 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      186 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2403 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1487 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2197 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      211 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1578 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4455 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      230 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2309 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3368 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2400 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2797 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      682 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3284 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1723 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2392 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3847 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      349 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2378 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3941 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1526 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2113 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      315 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      217 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3678 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3952 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2221 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5650 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1533 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1593 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2539 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1529 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1051 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     7527 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.974321 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1026 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1326 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2310 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      836 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1430 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      155 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1760 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      149 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2855 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3148 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4091 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      410 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      267 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1289 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     7048 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1669 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1589 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1569 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1541 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6448 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1925 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      180 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1131 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2541 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4486 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      671 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      786 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1054 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      161 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5589 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6042 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      162 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5785 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6091 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      226 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6389 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     9409 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1193 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5767 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2149 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2639 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      191 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     7925 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      698 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3142 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      147 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1023 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.979609 vastdb-0.1.0/vast_flatbuf/tabular/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2114 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2222 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1618 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1610 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1901 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/Column.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      151 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ColumnType.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2516 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1626 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3474 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4655 2024-04-09 14:04:20.000000 vastdb-0.1.0/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2450 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4240 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3036 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3550 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3589 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ObjectDetails.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4450 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/S3File.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2069 2024-04-09 14:04:20.000000 vastdb-0.1.0/vast_flatbuf/tabular/VipRange.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.983124 vastdb-0.1.0/vastdb/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      206 2024-04-10 13:32:04.000000 vastdb-0.1.0/vastdb/__init__.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/bucket.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3119 2024-04-10 18:32:20.000000 vastdb-0.1.0/vastdb/errors.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)   104441 2024-04-10 18:29:55.000000 vastdb-0.1.0/vastdb/internal_commands.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2836 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/schema.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1731 2024-04-10 13:33:23.000000 vastdb-0.1.0/vastdb/session.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)    20442 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/table.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.986088 vastdb-0.1.0/vastdb/tests/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-04-07 08:41:05.000000 vastdb-0.1.0/vastdb/tests/__init__.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1694 2024-04-10 13:50:46.000000 vastdb-0.1.0/vastdb/tests/conftest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5035 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/tests/test_imports.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1253 2024-04-09 14:04:20.000000 vastdb-0.1.0/vastdb/tests/test_projections.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2959 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/tests/test_sanity.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1253 2024-04-09 14:04:20.000000 vastdb-0.1.0/vastdb/tests/test_schemas.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)    23634 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/tests/test_tables.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1797 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/transaction.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2908 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/util.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.984138 vastdb-0.1.0/vastdb.egg-info/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     8858 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        1 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       78 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/requires.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       20 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.0.5.3/LICENSE` & `vastdb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.0/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.0/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.0/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.0/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.0/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.0/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.0/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.0/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.0.5.3/vastdb/api.py` & `vastdb-0.1.0/vastdb/internal_commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-import array
 import logging
 import struct
 import urllib.parse
 from collections import defaultdict, namedtuple
 from datetime import datetime
 from enum import Enum
-from typing import List, Union, Optional, Iterator
+from typing import Union, Optional, Iterator
+import ibis
 import xmltodict
-import concurrent.futures
-import threading
-import queue
 import math
-import socket
 from functools import cmp_to_key
 import pyarrow.parquet as pq
 import flatbuffers
 import pyarrow as pa
 import requests
-import datetime
-import hashlib
-import hmac
 import json
 import itertools
 from aws_requests_auth.aws_auth import AWSRequestsAuth
-from io import BytesIO
+import urllib3
+import re
+
+from . import errors
+from ipaddress import IPv4Address, IPv6Address
 
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.BinaryLiteral as fb_binary_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.BooleanLiteral as fb_bool_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Call as fb_call
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.DateLiteral as fb_date32_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.DecimalLiteral as fb_decimal_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Expression as fb_expression
@@ -87,50 +84,38 @@
 UINT64_MAX = 18446744073709551615
 
 TABULAR_KEEP_ALIVE_STREAM_ID = 0xFFFFFFFF
 TABULAR_QUERY_DATA_COMPLETED_STREAM_ID = 0xFFFFFFFF - 1
 TABULAR_QUERY_DATA_FAILED_STREAM_ID = 0xFFFFFFFF - 2
 TABULAR_INVALID_ROW_ID = 0xFFFFFFFFFFFF # (1<<48)-1
 ESTORE_INVALID_EHANDLE = UINT64_MAX
+IMPORTED_OBJECTS_TABLE_NAME = "vastdb-imported-objects"
 
 """
 S3 Tabular API
 """
 
 
-def get_logger(name):
-    log = logging.getLogger(name)
-    log.setLevel(logging.ERROR)
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.INFO)
-    ch.set_name('tabular_stream_handler')
-    formatter = logging.Formatter("%(asctime)s:%(levelname)s:%(message)s")
-    ch.setFormatter(formatter)
-    log.addHandler(ch)
-    log.propagate = False
-    return log
-
-
-_logger = get_logger(__name__)
+_logger = logging.getLogger(__name__)
 
 
-def set_tabular_log_level(level: int = logging.INFO):
-    _logger.setLevel(level)
+def _flatten_args(op, op_type):
+    if isinstance(op, op_type):
+        for arg in op.args:
+            yield from _flatten_args(arg, op_type)
+    else:
+        yield op
 
 
 class AuthType(Enum):
     SIGV4 = "s3v4"
     SIGV2 = "s3"
     BASIC = "basic"
 
 
-class TabularException(Exception):
-    pass
-
-
 def get_unit_to_flatbuff_time_unit(type):
     unit_to_flatbuff_time_unit = {
         'ns': TimeUnit.NANOSECOND,
         'us': TimeUnit.MICROSECOND,
         'ms': TimeUnit.MILLISECOND,
         's': TimeUnit.SECOND
     }
@@ -140,19 +125,18 @@
     unit_to_epoch = {
         'ns': 1_000_000,
         'us': 1_000,
         'ms': 1,
         's': 0.001
     }
 
-    def __init__(self, schema: 'pa.Schema', filters: dict):
+    def __init__(self, schema: 'pa.Schema', expr: ibis.expr.types.BooleanColumn):
         self.schema = schema
-        self.filters = filters
+        self.expr = expr
         self.builder = None
-        self._field_name_per_index = None
 
     def get_field_indexes(self, field: 'pa.Field', field_name_per_index: list) -> None:
         field_name_per_index.append(field.name)
 
         if isinstance(field.type, pa.StructType):
             flat_fields = field.flatten()
         elif isinstance(field.type, pa.MapType):
@@ -168,15 +152,14 @@
     @property
     def field_name_per_index(self):
         if self._field_name_per_index is None:
             _field_name_per_index = []
             for field in self.schema:
                 self.get_field_indexes(field, _field_name_per_index)
             self._field_name_per_index = {field: index for index, field in enumerate(_field_name_per_index)}
-            _logger.debug(f'field_name_per_index: {self._field_name_per_index}')
         return self._field_name_per_index
 
     def get_projections(self, builder: 'flatbuffers.builder.Builder', field_names: list = None):
         if not field_names:
             field_names = self.field_name_per_index.keys()
         projection_fields = []
         for field_name in field_names:
@@ -186,18 +169,85 @@
             projection_fields.append(offset)
         fb_source.StartProjectionVector(builder, len(projection_fields))
         for offset in reversed(projection_fields):
             builder.PrependUOffsetTRelative(offset)
         return builder.EndVector()
 
     def serialize(self, builder: 'flatbuffers.builder.Builder'):
+        from ibis.expr.operations.generic import TableColumn, Literal, IsNull
+        from ibis.expr.operations.logical import Greater, GreaterEqual, Less, LessEqual, Equals, NotEquals, And, Or, Not
+        from ibis.expr.operations.strings import StringContains
+
+        builder_map = {
+            Greater: self.build_greater,
+            GreaterEqual: self.build_greater_equal,
+            Less: self.build_less,
+            LessEqual: self.build_less_equal,
+            Equals: self.build_equal,
+            NotEquals: self.build_not_equal,
+            IsNull: self.build_is_null,
+            Not: self.build_is_not_null,
+            StringContains: self.build_match_substring,
+        }
+
+        positions_map = dict((f.name, index) for index, f in enumerate(self.schema)) # TODO: BFS
+
         self.builder = builder
+
         offsets = []
-        for field_name in self.filters:
-            offsets.append(self.build_domain(self.build_column(self.field_name_per_index[field_name]), field_name))
+
+        if self.expr is not None:
+            and_args = list(_flatten_args(self.expr.op(), And))
+            _logger.debug('AND args: %s ops %s', and_args, self.expr.op())
+            for op in and_args:
+                or_args = list(_flatten_args(op, Or))
+                _logger.debug('OR args: %s op %s', or_args, op)
+                inner_offsets = []
+
+                prev_field_name = None
+                for inner_op in or_args:
+                    _logger.debug('inner_op %s', inner_op)
+                    builder_func = builder_map.get(type(inner_op))
+                    if not builder_func:
+                        raise NotImplementedError(inner_op.name)
+
+                    if builder_func == self.build_is_null:
+                        column, = inner_op.args
+                        literal = None
+                    elif builder_func == self.build_is_not_null:
+                        not_arg, = inner_op.args
+                        # currently we only support not is_null, checking we really got is_null under the not:
+                        if not builder_map.get(type(not_arg)) == self.build_is_null:
+                            raise NotImplementedError(not_arg.args[0].name)
+                        column, = not_arg.args
+                        literal = None
+                    else:
+                        column, literal = inner_op.args
+                        if not isinstance(literal, Literal):
+                            raise NotImplementedError(inner_op.name)
+
+                    if not isinstance(column, TableColumn):
+                        raise NotImplementedError(inner_op.name)
+
+                    field_name = column.name
+                    if prev_field_name is None:
+                        prev_field_name = field_name
+                    elif prev_field_name != field_name:
+                        raise NotImplementedError(op.name)
+
+                    args_offsets = [self.build_column(position=positions_map[field_name])]
+                    if literal:
+                        field = self.schema.field(field_name)
+                        args_offsets.append(self.build_literal(field=field, value=literal.value))
+
+                    inner_offsets.append(builder_func(*args_offsets))
+
+                domain_offset = self.build_or(inner_offsets)
+                offsets.append(domain_offset)
+
         return self.build_and(offsets)
 
     def build_column(self, position: int):
         fb_field_index.Start(self.builder)
         fb_field_index.AddPosition(self.builder, position)
         index = fb_field_index.End(self.builder)
 
@@ -217,15 +267,14 @@
         if not filters:
             return self.build_or([self.build_is_not_null(column)])
 
         field_name, *field_attrs = field_name.split('.')
         field = self.schema.field(field_name)
         for attr in field_attrs:
             field = field.type[attr]
-        _logger.info(f'trying to append field: {field} with domains: {filters}')
         for filter_by_name in filters:
             offsets.append(self.build_range(column=column, field=field, filter_by_name=filter_by_name))
         return self.build_or(offsets)
 
     def rule_to_operator(self, raw_rule: str):
         operator_matcher = {
             'eq': self.build_equal,
@@ -259,34 +308,32 @@
             op, value = self.rule_to_operator(rule)
             literal = self.build_literal(field=field, value=value)
             rules.append(op(column, literal))
 
         return self.build_and(rules)
 
     def build_function(self, name: str, *offsets):
-        _logger.info(f'name: {name}, offsets: {offsets}')
         offset_name = self.builder.CreateString(name)
         fb_call.StartArgumentsVector(self.builder, len(offsets))
         for offset in reversed(offsets):
-            _logger.info(f'offset: {offset}')
             self.builder.PrependUOffsetTRelative(offset)
         offset_arguments = self.builder.EndVector()
 
         fb_call.Start(self.builder)
         fb_call.AddName(self.builder, offset_name)
         fb_call.AddArguments(self.builder, offset_arguments)
 
         offset_call = fb_call.CallEnd(self.builder)
 
         fb_expression.Start(self.builder)
         fb_expression.AddImplType(self.builder, ExpressionImpl.Call)
         fb_expression.AddImpl(self.builder, offset_call)
         return fb_expression.End(self.builder)
 
-    def build_literal(self, field: pa.Field, value: str):
+    def build_literal(self, field: pa.Field, value):
         if field.type.equals(pa.int64()):
             literal_type = fb_int64_lit
             literal_impl = LiteralImpl.Int64Literal
 
             field_type_type = Type.Int
             fb_int.Start(self.builder)
             fb_int.AddBitWidth(self.builder, field.type.bit_width)
@@ -362,16 +409,15 @@
 
             field_type_type = Type.Date
             fb_date.Start(self.builder)
             fb_date.AddUnit(self.builder, DateUnit.DAY)
             field_type = fb_date.End(self.builder)
 
             start_date = datetime.fromtimestamp(0).date()
-            date_value = datetime.strptime(value, '%Y-%m-%d').date()
-            date_delta = date_value - start_date
+            date_delta = value - start_date
             value = date_delta.days
         elif isinstance(field.type, pa.TimestampType):
             literal_type = fb_timestamp_lit
             literal_impl = LiteralImpl.TimestampLiteral
 
             field_type_type = Type.Timestamp
             fb_timestamp.Start(self.builder)
@@ -422,15 +468,15 @@
             literal_type = fb_binary_lit
             literal_impl = LiteralImpl.BinaryLiteral
 
             field_type_type = Type.Binary
             fb_binary.Start(self.builder)
             field_type = fb_binary.End(self.builder)
 
-            value = self.builder.CreateByteVector(value.encode())
+            value = self.builder.CreateByteVector(value)
         else:
             raise ValueError(f'unsupported predicate for type={field.type}, value={value}')
 
         literal_type.Start(self.builder)
         literal_type.AddValue(self.builder, value)
         buffer_value = literal_type.End(self.builder)
 
@@ -455,14 +501,17 @@
 
     def build_and(self, offsets: list):
         return self.build_function('and', *offsets)
 
     def build_equal(self, column: int, literal: int):
         return self.build_function('equal', column, literal)
 
+    def build_not_equal(self, column: int, literal: int):
+        return self.build_function('not_equal', column, literal)
+
     def build_greater(self, column: int, literal: int):
         return self.build_function('greater', column, literal)
 
     def build_greater_equal(self, column: int, literal: int):
         return self.build_function('greater_equal', column, literal)
 
     def build_less(self, column: int, literal: int):
@@ -473,14 +522,17 @@
 
     def build_is_null(self, column: int):
         return self.build_function('is_null', column)
 
     def build_is_not_null(self, column: int):
         return self.build_function('is_valid', column)
 
+    def build_match_substring(self, column: int, literal: int):
+        return self.build_function('match_substring', column, literal)
+
 
 class FieldNode:
     """Helper class for representing nested Arrow fields and handling QueryData requests"""
     def __init__(self, field: pa.Field, index_iter, parent: Optional['FieldNode'] = None, debug: bool = False):
         self.index = next(index_iter) # we use DFS-first enumeration for communicating the column positions to VAST
         self.field = field
         self.type = field.type
@@ -570,17 +622,16 @@
                     raise ValueError(f'self.buffers: {self.buffers} are not equal with buffers: {buffers}')
             if not self.length == len(arr):
                 raise ValueError(f'self.length: {self.length} are not equal with len(arr): {len(arr)}')
 
     def build(self) -> pa.Array:
         """Construct an Arrow array from the collected buffers (recursively)."""
         children = self.children and [node.build() for node in self.children if node.is_projected]
-        _logger.debug(f'build: self.field.name={self.field.name}, '
-                      f'self.projected_field.type={self.projected_field.type}, self.length={self.length} '
-                      f'self.buffers={self.buffers} children={children}')
+        _logger.debug('build: self.field.name=%s, self.projected_field.type=%s, self.length=%s, self.buffers=%s children=%s',
+                      self.field.name, self.projected_field.type, self.length, self.buffers, children)
         result = pa.Array.from_buffers(self.projected_field.type, self.length, buffers=self.buffers, children=children)
         if self.debug:
             _logger.debug('%s result=%s', self.field, result)
         return result
 
     def build_projected_field(self):
         if isinstance(self.type, pa.StructType):
@@ -598,28 +649,25 @@
         index = itertools.count() # used to generate leaf column positions for VAST QueryData RPC
         self.nodes = [FieldNode(field, index, debug=debug) for field in arrow_schema]
         self.debug = debug
         if self.debug:
             for node in self.nodes:
                 node.debug_log()
         self.leaves = [leaf for node in self.nodes for leaf in node._iter_leaves()]
-        _logger.debug(f'QueryDataParser: self.leaves = {[(leaf.field.name, leaf.index) for leaf in self.leaves]}')
         self.mark_projected_nodes()
         [node.build_projected_field() for node in self.nodes]
         self.projected_leaves = [leaf for node in self.nodes for leaf in node._iter_projected_leaves()]
-        _logger.debug(f'QueryDataParser: self.projected_leaves = {[(leaf.field.name, leaf.index) for leaf in self.projected_leaves]}')
 
         self.leaf_offset = 0
 
     def mark_projected_nodes(self):
         for leaf in self.leaves:
             if self.projection_positions is None or leaf.index in self.projection_positions:
                 for node in leaf._iter_to_root():
                     node.is_projected = True
-                    _logger.debug(f'mark_projected_nodes node.field.name={node.field.name}')
 
     def parse(self, column: pa.Array):
         """Parse a single column response from VAST (see FieldNode.set for details)"""
         if not self.leaf_offset < len(self.projected_leaves):
             raise ValueError(f'self.leaf_offset: {self.leaf_offset} are not < '
                              f'than len(self.leaves): {len(self.leaves)}')
         leaf = self.projected_leaves[self.leaf_offset]
@@ -689,98 +737,97 @@
     properties = obj.Properties().decode()
     handle = obj.Handle().decode()
     num_rows = obj.NumRows()
     used_bytes = obj.SizeInBytes()
     return TableInfo(name, properties, handle, num_rows, used_bytes)
 
 def build_record_batch(column_info, column_values):
-    _logger.info(f"column_info={column_info}")
     fields = [pa.field(column_name, column_type) for column_type, column_name in column_info]
     schema = pa.schema(fields)
     arrays = [pa.array(column_values[column_type], type=column_type) for column_type, _ in column_info]
     batch = pa.record_batch(arrays, schema)
     return serialize_record_batch(batch)
 
 def serialize_record_batch(batch):
     sink = pa.BufferOutputStream()
     with pa.ipc.new_stream(sink, batch.schema) as writer:
         writer.write(batch)
     return sink.getvalue()
 
-def generate_ip_range(ip_range_str):
-    start, end = ip_range_str.split(':')
-    start_parts = start.split('.')
-    start_last_part = int(start_parts[-1])
-    end_parts = end.split('.')
-    end_last_part = int(end_parts[-1])
-    if start_last_part>=end_last_part or True in [start_parts[i] != end_parts[i] for i in range(3)]:
-        raise ValueError(f'illegal ip range {ip_range_str}')
-    num_ips = 1 + end_last_part - start_last_part
-    ips = ['.'.join(start_parts[:-1] + [str(start_last_part + i)]) for i in range(num_ips)]
-    return ips
-
-def parse_executor_hosts(host):
-        executor_hosts_parsed = host.split(',')
-        executor_hosts_parsed = [host.strip() for host in executor_hosts_parsed]
-        executor_hosts = []
-        for executor_host in executor_hosts_parsed:
-            is_ip_range=False
-            if ':' in executor_host:
-                try:
-                    socket.inet_aton(executor_host.split(':')[0])
-                    socket.inet_aton(executor_host.split(':')[1])
-                    is_ip_range = True
-                except:
-                    pass
-            if is_ip_range:
-                executor_hosts.extend(generate_ip_range(executor_host))
-            else:
-                executor_hosts.append(executor_host)
-        return executor_hosts
+# Results that returns from tablestats
+TableStatsResult = namedtuple("TableStatsResult",["num_rows", "size_in_bytes", "is_external_rowid_alloc", "endpoints"])
 
 class VastdbApi:
-    def __init__(self, host, access_key, secret_key, username=None, password=None, port=None,
+    # we expect the vast version to be <major>.<minor>.<patch>.<protocol>
+    VAST_VERSION_REGEX = re.compile(r'^vast (\d+\.\d+\.\d+\.\d+)$')
+
+    def __init__(self, endpoint, access_key, secret_key, username=None, password=None,
                  secure=False, auth_type=AuthType.SIGV4):
-        executor_hosts = parse_executor_hosts(host)
-        host = executor_hosts[0]
-        self.host = host
+        url_dict = urllib3.util.parse_url(endpoint)._asdict()
         self.access_key = access_key
         self.secret_key = secret_key
         self.username = username
         self.password = password
-        self.port = port
         self.secure = secure
         self.auth_type = auth_type
-        self.executor_hosts = executor_hosts
+        self.executor_hosts = [endpoint]  # TODO: remove
 
         username = username or ''
         password = password or ''
-        if not port:
-            port = 443 if secure else 80
+        if not url_dict['port']:
+            url_dict['port'] = 443 if secure else 80
+
+        self.port = url_dict['port']
 
         self.default_max_list_columns_page_size = 1000
         self.session = requests.Session()
         self.session.verify = False
         self.session.headers['user-agent'] = "VastData Tabular API 1.0 - 2022 (c)"
         if auth_type == AuthType.BASIC:
             self.session.auth = requests.auth.HTTPBasicAuth(username, password)
         else:
-            if port != 80 and port != 443:
-                self.aws_host = f'{host}:{port}'
+            if url_dict['port'] != 80 and url_dict['port'] != 443:
+                self.aws_host = '{host}:{port}'.format(**url_dict)
             else:
-                self.aws_host = f'{host}'
+                self.aws_host = '{host}'.format(**url_dict)
 
             self.session.auth = AWSRequestsAuth(aws_access_key=access_key,
                                                 aws_secret_access_key=secret_key,
                                                 aws_host=self.aws_host,
                                                 aws_region='us-east-1',
                                                 aws_service='s3')
 
-        proto = "https" if secure else "http"
-        self.url = f"{proto}://{self.aws_host}"
+        if not url_dict['scheme']:
+            url_dict['scheme'] = "https" if secure else "http"
+
+        url = urllib3.util.Url(**url_dict)
+        self.url = str(url)
+        _logger.debug('url=%s aws_host=%s', self.url, self.aws_host)
+
+        # probe the cluster for its version
+        self.vast_version = None
+        res = self.session.options(self.url)
+        server_header = res.headers.get("Server")
+        if server_header is None:
+            _logger.error("OPTIONS response doesn't contain 'Server' header")
+        else:
+            _logger.debug("Server header is '%s'", server_header)
+            if m := self.VAST_VERSION_REGEX.match(server_header):
+                self.vast_version, = m.groups()
+                return
+            else:
+                _logger.error("'Server' header '%s' doesn't match the expected pattern", server_header)
+
+        msg = (
+            f'Please use `vastdb` <= 0.0.5.x with current VAST cluster version ("{server_header or "N/A"}"). '
+            'To use the latest SDK, please upgrade your cluster to the latest service pack. '
+            'Please contact customer.support@vastdata.com for more details.'
+        )
+        _logger.critical(msg)
+        raise NotImplementedError(msg)
 
     def update_mgmt_session(self, access_key: str, secret_key: str, auth_type=AuthType.SIGV4):
         if auth_type != AuthType.BASIC:
             self.session.auth = AWSRequestsAuth(aws_access_key=access_key,
                                                 aws_secret_access_key=secret_key,
                                                 aws_host=self.aws_host,
                                                 aws_region='us-east-1',
@@ -817,29 +864,17 @@
                           'tabular-client-name': 'tabular-api'}
         for tag in client_tags:
             common_headers['tabular-client-tags-%d' % client_tags.index(tag)] = tag
 
         return common_headers
 
     def _check_res(self, res, cmd="", expected_retvals=[]):
-        try:
-            res.raise_for_status()
-            if res.status_code != 200:
-                if not  res.status_code in expected_retvals:
-                    raise ValueError(f"Expected status code mismatch. status_code={res.status_code}")
-            else:
-                if not len(expected_retvals) == 0:
-                    raise ValueError(f"Expected {expected_retvals} but status_code={res.status_code}")
-            return res
-        except requests.HTTPError as e:
-            if res.status_code in expected_retvals:
-                _logger.info(f"{cmd} has failed as expected res={res}")
-                return res
-            else:
-                raise e
+        if exc := errors.from_response(res):
+            raise exc
+        return res
 
     def create_schema(self, bucket, name, txid=0, client_tags=[], schema_properties="", expected_retvals=[]):
         """
         Create a collection of tables, use the following request
         POST /bucket/schema?schema HTTP/1.1
 
         The body of the POST request contains schema properties as flatbuffer
@@ -971,35 +1006,39 @@
             marker = list_res['Marker']
             common_prefixes = list_res['CommonPrefixes'] if 'CommonPrefixes' in list_res else []
             snapshots = [v['Prefix'] for v in common_prefixes]
 
             return snapshots, is_truncated, marker
 
 
-    def create_table(self, bucket, schema, name, arrow_schema, txid=0, client_tags=[], expected_retvals=[], topic_partitions=0):
+    def create_table(self, bucket, schema, name, arrow_schema, txid=0, client_tags=[], expected_retvals=[],
+                     topic_partitions=0, create_imports_table=False):
         """
         Create a table, use the following request
         POST /bucket/schema/table?table HTTP/1.1
 
         Request Headers
         tabular-txid: <integer> TransactionId
         tabular-client-tag: <string> ClientTag
 
-        The body of the POST request contains table column properties as json
-        {
-            "format": "string",
-            "column_names": {"name1":"type1", "name2":"type2", ...},
-            "table_properties": {"key1":"val1", "key2":"val2", ...}
-        }
+        The body of the POST request contains table column properties as arrow schema
+        which include field_name, field_type and properties
+
+        In order to create vastdb-imported-objects table that tracks all imported files and avoid duplicate imports,
+        just set create_imports_table=True
+        The request will look like:
+        POST /bucket/schema/table?table&sub-table=vastdb-imported-objects HTTP/1.1
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
 
         serialized_schema = arrow_schema.serialize()
         headers['Content-Length'] = str(len(serialized_schema))
         url_params = {'topic_partitions': str(topic_partitions)} if topic_partitions else {}
+        if create_imports_table:
+            url_params['sub-table'] = IMPORTED_OBJECTS_TABLE_NAME
 
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
                                 data=serialized_schema, headers=headers)
         return self._check_res(res, "create_table", expected_retvals)
 
     def create_table_from_parquet_schema(self, bucket, schema, name, parquet_path=None,
                                          parquet_bucket_name=None, parquet_object_name=None,
@@ -1011,15 +1050,14 @@
         elif parquet_bucket_name and parquet_object_name:
             s3fs  = pa.fs.S3FileSystem(access_key=self.access_key, secret_key=self.secret_key, endpoint_override=self.url)
             parquet_ds = pq.ParquetDataset('/'.join([parquet_bucket_name,parquet_object_name]), filesystem=s3fs)
         else:
             raise RuntimeError(f'invalid params parquet_path={parquet_path} parquet_bucket_name={parquet_bucket_name} parquet_object_name={parquet_object_name}')
 
         # Get the schema of the Parquet file
-        _logger.info(f'type(parquet_ds.schema) = {type(parquet_ds.schema)}')
         if isinstance(parquet_ds.schema, pq.ParquetSchema):
             arrow_schema = parquet_ds.schema.to_arrow_schema()
         elif isinstance(parquet_ds.schema, pa.Schema):
             arrow_schema = parquet_ds.schema
         else:
             raise RuntimeError(f'invalid type(parquet_ds.schema) = {type(parquet_ds.schema)}')
 
@@ -1034,21 +1072,35 @@
         tabular-client-tag: ClientTag
 
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats"), headers=headers)
         if res.status_code == 200:
-            res_headers = res.headers
             flatbuf = b''.join(res.iter_content(chunk_size=128))
             stats = get_table_stats.GetRootAs(flatbuf)
             num_rows = stats.NumRows()
             size_in_bytes = stats.SizeInBytes()
             is_external_rowid_alloc = stats.IsExternalRowidAlloc()
-            return num_rows, size_in_bytes, is_external_rowid_alloc
+            endpoints = []
+            if stats.VipsLength() == 0:
+                endpoints.append(self.url)
+            else:
+                ip_cls = IPv6Address if (stats.AddressType() == "ipv6") else IPv4Address
+                vips = [stats.Vips(i) for i in range(stats.VipsLength())]
+                ips = []
+                # extract the vips into list of IPs
+                for vip in vips:
+                    start_ip = int(ip_cls(vip.StartAddress().decode()))
+                    ips.extend(ip_cls(start_ip + i) for i  in range(vip.AddressCount()))
+                for ip in ips:
+                    prefix = "http" if not self.secure else "https"
+                    endpoints.append(f"{prefix}://{str(ip)}:{self.port}")
+            return TableStatsResult(num_rows, size_in_bytes, is_external_rowid_alloc, endpoints)
+
         return self._check_res(res, "get_table_stats", expected_retvals)
 
     def alter_table(self, bucket, schema, name, txid=0, client_tags=[], table_properties="",
                     new_name="", expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?table HTTP/1.1
         Content-Length: ContentLength
@@ -1067,30 +1119,34 @@
 
         params = tabular_alter_table.End(builder)
         builder.Finish(params)
         alter_table_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(alter_table_req))
-        url_params = {'tabular-new-table-name': new_name} if len(new_name) else {}
+        url_params = {'tabular-new-table-name': schema + "/" + new_name} if len(new_name) else {}
 
         res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
                                data=alter_table_req, headers=headers)
 
         return self._check_res(res, "alter_table", expected_retvals)
 
-    def drop_table(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[]):
+    def drop_table(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[], remove_imports_table=False):
         """
         DELETE /mybucket/schema_path/mytable?table HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
+
+        To remove the internal vastdb-imported-objects table just set remove_imports_table=True
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
+        url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if remove_imports_table else {}
 
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table"), headers=headers)
+        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
+                                  headers=headers)
         return self._check_res(res, "drop_table", expected_retvals)
 
     def list_tables(self, bucket, schema, txid=0, client_tags=[], max_keys=1000, next_key=0, name_prefix="",
                     exact_match=False, expected_retvals=[], include_list_stats=False, count_only=False):
         """
         GET /mybucket/schema_path?table HTTP/1.1
         tabular-txid: TransactionId
@@ -1206,22 +1262,24 @@
 
         res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column"),
                                 data=serialized_schema, headers=headers)
         return self._check_res(res, "drop_columns", expected_retvals)
 
     def list_columns(self, bucket, schema, table, *, txid=0, client_tags=None, max_keys=None, next_key=0,
                      count_only=False, name_prefix="", exact_match=False,
-                     expected_retvals=None, bc_list_internals=False):
+                     expected_retvals=None, bc_list_internals=False, list_imports_table=False):
         """
         GET /mybucket/myschema/mytable?columns HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         x-tabluar-name-prefix: TableNamePrefix
         tabular-max-keys: 1000
         tabular-next-key: NextColumnId
+
+        To list the columns of the internal vastdb-imported-objects table, set list_import_table=True
         """
         max_keys = max_keys or self.default_max_list_columns_page_size
         client_tags = client_tags or []
         expected_retvals = expected_retvals or []
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['tabular-max-keys'] = str(max_keys)
@@ -1231,29 +1289,29 @@
             headers['tabular-bc-list-internal-col'] = "true"
 
         if exact_match:
             headers['tabular-name-exact-match'] = name_prefix
         else:
             headers['tabular-name-prefix'] = name_prefix
 
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column"),
+        url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if list_imports_table else {}
+        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column",
+                                                url_params=url_params),
                                headers=headers, stream=True)
         self._check_res(res, "list_columns", expected_retvals)
         if res.status_code == 200:
             res_headers = res.headers
             next_key = int(res_headers['tabular-next-key'])
             is_truncated = res_headers['tabular-is-truncated'] == 'true'
             count = int(res_headers['tabular-list-count'])
             columns = []
             if not count_only:
                 schema_buf = b''.join(res.iter_content(chunk_size=128))
                 schema_out = pa.ipc.open_stream(schema_buf).schema
-    #            _logger.info(f"schema={schema_out}")
-                for f in schema_out:
-                    columns.append([f.name, f.type, f.metadata, f])
+                columns = schema_out
 
             return columns, next_key, is_truncated, count
 
     def begin_transaction(self, client_tags=[], expected_retvals=[]):
         """
         POST /?transaction HTTP/1.1
         tabular-client-tag: ClientTag
@@ -1292,15 +1350,15 @@
         tabular-client-tag: ClientTag
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         res = self.session.get(self._api_prefix(command="transaction"), headers=headers)
         return self._check_res(res, "get_transaction", expected_retvals)
 
     def select_row_ids(self, bucket, schema, table, params, txid=0, client_tags=[], expected_retvals=[],
-                       retry_count=0, enable_sorted_projections=False):
+                       retry_count=0, enable_sorted_projections=True):
         """
         POST /mybucket/myschema/mytable?query-data=SelectRowIds HTTP/1.1
         """
 
         # add query option select-only and read-only
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(params))
@@ -1309,15 +1367,15 @@
             headers['tabular-retry-count'] = str(retry_count)
 
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=SelectRowIds",),
                                 data=params, headers=headers, stream=True)
         return self._check_res(res, "query_data", expected_retvals)
 
     def read_columns_data(self, bucket, schema, table, params, txid=0, client_tags=[], expected_retvals=[], tenant_guid=None,
-                          retry_count=0, enable_sorted_projections=False):
+                          retry_count=0, enable_sorted_projections=True):
         """
         POST /mybucket/myschema/mytable?query-data=ReadColumns HTTP/1.1
         """
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(params))
         headers['tabular-enable-sorted-projections'] = str(enable_sorted_projections)
@@ -1325,49 +1383,31 @@
             headers['tabular-retry-count'] = str(retry_count)
 
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=ReadColumns",),
                                data=params, headers=headers, stream=True)
         return self._check_res(res, "query_data", expected_retvals)
 
     def count_rows(self, bucket, schema, table, params, txid=0, client_tags=[], expected_retvals=[], tenant_guid=None,
-                   retry_count=0, enable_sorted_projections=False):
+                   retry_count=0, enable_sorted_projections=True):
         """
         POST /mybucket/myschema/mytable?query-data=CountRows HTTP/1.1
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(params))
         headers['tabular-enable-sorted-projections'] = str(enable_sorted_projections)
         if retry_count > 0:
             headers['tabular-retry-count'] = str(retry_count)
 
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=CountRows",),
                                data=params, headers=headers, stream=True)
         return self._check_res(res, "query_data", expected_retvals)
 
-    def query_data(self, bucket, schema, table, params, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
-                   txid=0, client_tags=[], expected_retvals=[], limit_rows=0, schedule_id=None, retry_count=0,
-                   search_path=None, sub_split_start_row_ids=[], tenant_guid=None, projection='', enable_sorted_projections=True,
-                   request_format='string', response_format='string'):
-        """
-        GET /mybucket/myschema/mytable?data HTTP/1.1
-        Content-Length: ContentLength
-        tabular-txid: TransactionId
-        tabular-client-tag: ClientTag
-        tabular-split: "split_id,total_splits,num_row_groups_per_split"
-        tabular-num-of-subsplits: "total"
-        tabular-request-format: "string"
-        tabular-response-format: "string" #arrow/trino
-        tabular-schedule-id: "schedule-id"
-
-        Request Body (flatbuf)
-        projections_chunk [expressions]
-        predicate_chunk "formatted_data", (required)
-
-        """
-        # add query option select-only and read-only
+    def _build_query_data_headers(self, txid, client_tags, params, split, num_sub_splits, request_format, response_format,
+                                  enable_sorted_projections, limit_rows, schedule_id, retry_count, search_path, tenant_guid,
+                                  sub_split_start_row_ids):
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(params))
         headers['tabular-split'] = ','.join(map(str, split))
         headers['tabular-num-of-subsplits'] = str(num_sub_splits)
         headers['tabular-request-format'] = request_format
         headers['tabular-response-format'] = response_format
         headers['tabular-enable-sorted-projections'] = str(enable_sorted_projections)
@@ -1384,447 +1424,88 @@
 
         if len(sub_split_start_row_ids) == 0:
             sub_split_start_row_ids = [(n, 0) for n in range(num_sub_splits)]
 
         for sub_split_id, start_row_id in sub_split_start_row_ids:
             headers[f'tabular-start-row-id-{sub_split_id}'] = f"{sub_split_id},{start_row_id}"
 
-        url_params = {'name': projection} if projection else {}
-
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="data", url_params=url_params),
-                               data=params, headers=headers, stream=True)
-        return self._check_res(res, "query_data", expected_retvals)
-
-    def _list_table_columns(self, bucket, schema, table, filters=None, field_names=None, txid=0):
-        # build a list of the queried column names
-        queried_columns = []
-        # get all columns from the table
-        all_listed_columns = []
-        next_key = 0
-        while True:
-            cur_columns, next_key, is_truncated, count = self.list_columns(
-                bucket=bucket, schema=schema, table=table, next_key=next_key, txid=txid)
-            if not cur_columns:
-                break
-            all_listed_columns.extend(cur_columns)
-            if not is_truncated:
-                break
-
-        # build a list of the queried columns
-        queried_column_names = set()
-        if filters:
-            filtered_column_names = ([column_name.split('.')[0] for column_name in filters.keys()]) # use top level of the filter column names
-            queried_column_names.update(filtered_column_names)
-            _logger.debug(f"_list_table_columns: filtered_column_names={filtered_column_names}")
+        return headers
 
-        if field_names:
-            field_column_names = ([column_name.split('.')[0] for column_name in field_names]) # use top level of the field column names
-        else:
-            field_column_names = [column[0] for column in all_listed_columns]
-        _logger.debug(f"_list_table_columns: field_column_names={field_column_names}")
-        queried_column_names.update(field_column_names)
-
-        all_listed_column_and_leaves_names = set()
-        for column in all_listed_columns:
-            # Collect the column and leaves names for verification below that all the filters and field names are in the table
-            column_and_leaves_names = [column[0]] + [f.name for f in column[3].flatten()]
-            all_listed_column_and_leaves_names.update(column_and_leaves_names)
-
-            # check if this column is needed for the query
-            if column[0] in queried_column_names:
-                queried_columns.append(column)
-
-        # verify that all the filters and field names are in the table
-        if filters:
-            for filter_column_name in filters.keys():
-                if filter_column_name not in all_listed_column_and_leaves_names:
-                    raise KeyError((f'filter column name: {filter_column_name} does not appear in the table'))
-        if field_names:
-            for field_name in field_names:
-                if field_name not in all_listed_column_and_leaves_names:
-                    raise ValueError((f'field name: {field_name} does not appear in the table'))
-        return list(queried_columns)
-
-    def _begin_tx_if_necessary(self, txid):
-        if not txid:
-            created_txid = True
-            res = self.begin_transaction()
-            txid = res.headers.get('tabular-txid')
-        else:
-            created_txid = False
+    def _build_query_data_url_params(self, projection, query_imports_table):
+        if query_imports_table and projection:
+            raise ValueError("Can't query both imports and projection table")
+
+        url_params = {}
+        if query_imports_table:
+            url_params['sub-table'] = IMPORTED_OBJECTS_TABLE_NAME
+        elif projection:
+            url_params['name'] = projection
+        return url_params
+
+    def legacy_query_data(self, bucket, schema, table, params, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
+                      txid=0, client_tags=[], expected_retvals=[], limit_rows=0, schedule_id=None, retry_count=0,
+                      search_path=None, sub_split_start_row_ids=[], tenant_guid=None, projection='', enable_sorted_projections=True,
+                      request_format='string', response_format='string', query_imports_table=False):
+        """
+        POST /mybucket/myschema/mytable?query-data=LegacyQueryData HTTP/1.1
+        Content-Length: ContentLength
+        tabular-txid: TransactionId
+        tabular-client-tag: ClientTag
+        tabular-split: "split_id,total_splits,num_row_groups_per_split"
+        tabular-num-of-subsplits: "total"
+        tabular-request-format: "string"
+        tabular-response-format: "string" #arrow/trino
+        tabular-schedule-id: "schedule-id"
 
-        return txid, created_txid
+        Request Body (flatbuf)
+        projections_chunk [expressions]
+        predicate_chunk "formatted_data", (required)
 
-    def _prepare_query(self, bucket, schema, table, num_sub_splits, filters=None, field_names=None,
-                       queried_columns=None, response_row_id=False, txid=0):
-        queried_fields = []
-        if response_row_id:
-            queried_fields.append(pa.field('$row_id', pa.uint64()))
+        """
+        headers = self._build_query_data_headers(txid, client_tags, params, split, num_sub_splits, request_format, response_format,
+                                                  enable_sorted_projections, limit_rows, schedule_id, retry_count, search_path, tenant_guid,
+                                                  sub_split_start_row_ids)
+        url_params = self._build_query_data_url_params(projection, query_imports_table)
+
+        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=LegacyQueryData",
+                                                  url_params=url_params), data=params, headers=headers, stream=True)
+        return self._check_res(res, "legacy_query_data", expected_retvals)
 
-        if not queried_columns:
-            queried_columns = self._list_table_columns(bucket, schema, table, filters, field_names, txid=txid)
+    def query_data(self, bucket, schema, table, params, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
+                   txid=0, client_tags=[], expected_retvals=[], limit_rows=0, schedule_id=None, retry_count=0,
+                   search_path=None, sub_split_start_row_ids=[], tenant_guid=None, projection='', enable_sorted_projections=True,
+                   request_format='string', response_format='string', query_imports_table=False):
+        """
+        GET /mybucket/myschema/mytable?data HTTP/1.1
+        Content-Length: ContentLength
+        tabular-txid: TransactionId
+        tabular-client-tag: ClientTag
+        tabular-split: "split_id,total_splits,num_row_groups_per_split"
+        tabular-num-of-subsplits: "total"
+        tabular-request-format: "string"
+        tabular-response-format: "string" #arrow/trino
+        tabular-schedule-id: "schedule-id"
 
-        queried_fields.extend(pa.field(column[0], column[1]) for column in queried_columns)
-        arrow_schema = pa.schema(queried_fields)
+        Request Body (flatbuf)
+        projections_chunk [expressions]
+        predicate_chunk "formatted_data", (required)
 
-        _logger.debug(f'_prepare_query: arrow_schema = {arrow_schema}')
+        To query the internal vastdb-imported-objects table, set query_imports_table=True
+        """
+        # add query option select-only and read-only
 
-        query_data_request = build_query_data_request(schema=arrow_schema, filters=filters, field_names=field_names)
-        if self.executor_hosts:
-            executor_hosts = self.executor_hosts
-        else:
-            executor_hosts = [self.host]
-        executor_sessions = [VastdbApi(executor_hosts[i], self.access_key, self.secret_key, self.username,
-                                       self.password, self.port, self.secure, self.auth_type) for i in range(len(executor_hosts))]
-
-        return queried_columns, arrow_schema, query_data_request, executor_sessions
-
-    def _more_pages_exist(self, start_row_ids):
-        for row_id in start_row_ids.values():
-            if row_id != TABULAR_INVALID_ROW_ID:
-                return True
-        return False
-
-    def _query_page(self, bucket, schema, table, query_data_request, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
-                   txid=0, limit_rows=0, sub_split_start_row_ids=[], filters=None, field_names=None):
-        res = self.query_data(bucket=bucket, schema=schema, table=table, params=query_data_request.serialized, split=split,
-                              num_sub_splits=num_sub_splits, response_row_id=response_row_id, txid=txid,
-                              limit_rows=limit_rows, sub_split_start_row_ids=sub_split_start_row_ids)
-        start_row_ids = {}
-        sub_split_tables = parse_query_data_response(res.raw, query_data_request.response_schema,
-                                                    start_row_ids=start_row_ids)
-        table_page = pa.concat_tables(sub_split_tables)
-        _logger.info("query_page: table_page num_rows=%s start_row_ids len=%s",
-                     len(table_page), len(start_row_ids))
-
-        return table_page, start_row_ids
-
-    def _query_page_iterator(self, bucket, schema, table, query_data_request, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
-                             txid=0, limit_rows=0, start_row_ids={}, filters=None, field_names=None):
-        res = self.query_data(bucket=bucket, schema=schema, table=table, params=query_data_request.serialized, split=split,
-                              num_sub_splits=num_sub_splits, response_row_id=response_row_id, txid=txid,
-                              limit_rows=limit_rows, sub_split_start_row_ids=start_row_ids.items())
-        for sub_split_table in parse_query_data_response(res.raw, query_data_request.response_schema,
-                                                        start_row_ids=start_row_ids):
-            for record_batch in sub_split_table.to_batches():
-                yield record_batch
-        _logger.info(f"query_page_iterator: start_row_ids={start_row_ids}")
-
-    def query_iterator(self, bucket, schema, table, num_sub_splits=1, num_row_groups_per_sub_split=8,
-                       response_row_id=False, txid=0, limit_per_sub_split=128*1024, filters=None, field_names=None):
-        """
-        query rows into a table.
-
-        Parameters
-        ----------
-        bucket : string
-            The bucket of the table.
-        schema : string
-            The schema of the table.
-        table : string
-            The table name.
-        num_sub_splits : integer
-            The number of sub_splits per split - determines the parallelism inside a VastDB compute node
-            default: 1
-        num_row_groups_per_sub_split : integer
-            The number of consecutive row groups per sub_split. Each row group consists of 64K row ids.
-            default: 8
-        response_row_id : boolean
-            Return a column with the internal row ids of the table
-            default: False
-        txid : integer
-            A transaction id. The transaction may be initiated before the query, and if not, the query will initiate it
-            default: 0 (will be created by the api)
-        limit_per_sub_split : integer
-            Limit the number of rows from a single sub_split for a single rpc
-            default:131072
-        filters : dict
-            A dictionary whose keys are column names, and values are lists of string expressions that represent
-            filter conditions on the column. AND is applied on the conditions. The condition formats are:
-            'column_name eq some_value'
-            default: None
-        field_names : list
-            A list of column names to be returned in the output table
-            default: None
-
-        Returns
-        -------
-        Query iterator generator
-
-        Yields
-        ------
-        pyarrow.RecordBatch
-
-        Examples
-        --------
-        for record_batch in query_iterator('some_bucket', 'some_schema', 'some_table',
-                                           filters={'name': ['eq Alice', 'eq Bob']}
-                                           field_names=['name','age']):
-            ...
-
-        """
-
-        # create a transaction if necessary
-        txid, created_txid = self._begin_tx_if_necessary(txid)
-        executor_sessions = []
+        headers = self._build_query_data_headers(txid, client_tags, params, split, num_sub_splits, request_format, response_format,
+                                                 enable_sorted_projections, limit_rows, schedule_id, retry_count, search_path, tenant_guid,
+                                                 sub_split_start_row_ids)
 
-        try:
-            # prepare query
-            queried_columns, arrow_schema, query_data_request, executor_sessions = \
-                self._prepare_query(bucket, schema, table, num_sub_splits, filters, field_names, response_row_id=response_row_id, txid=txid)
-
-            # define the per split threaded query func
-            def query_iterator_split_id(self, split_id):
-                _logger.info(f"query_iterator_split_id: split_id={split_id}")
-                try:
-                    start_row_ids = {i:0 for i in range(num_sub_splits)}
-                    session = executor_sessions[split_id]
-                    while not next_sems[split_id].acquire(timeout=1):
-                        # check if killed externally
-                        if killall:
-                            raise RuntimeError(f'query_iterator_split_id: split_id {split_id} received killall')
-
-                    while self._more_pages_exist(start_row_ids):
-                        for record_batch in session._query_page_iterator(bucket=bucket, schema=schema, table=table, query_data_request=query_data_request,
-                                                                         split=(split_id, num_splits, num_row_groups_per_sub_split),
-                                                                         num_sub_splits=num_sub_splits, response_row_id=response_row_id,
-                                                                         txid=txid, limit_rows=limit_per_sub_split,
-                                                                         start_row_ids=start_row_ids):
-                            output_queue.put((split_id, record_batch))
-                            while not next_sems[split_id].acquire(timeout=1): # wait for the main thread to request the next record batch
-                                if killall:
-                                    raise RuntimeError(f'split_id {split_id} received killall')
-                    # end of split
-                    output_queue.put((split_id,None))
-
-                except Exception as e:
-                    _logger.exception('query_iterator_split_id: exception occurred')
-                    try:
-                        self.rollback_transaction(txid)
-                    except:
-                        _logger.exception(f'failed to rollback txid {txid}')
-                    error_queue.put(None)
-                    raise e
-
-            # kickoff executors
-            num_splits = len(executor_sessions)
-            output_queue = queue.Queue()
-            error_queue = queue.Queue()
-            next_sems = [threading.Semaphore(value=1) for i in range(num_splits)]
-            killall = False
-            with concurrent.futures.ThreadPoolExecutor(max_workers=num_splits) as executor:
-                # start executors
-                futures = []
-                for i in range(num_splits):
-                    futures.append(executor.submit(query_iterator_split_id, self, i))
-
-                # receive outputs and yield them
-                done_count = 0
-                while done_count < num_splits:
-                    # check for errors
-                    try:
-                        error_queue.get(block=False)
-                        _logger.error('received error from a thread')
-                        killall = True
-                        # wait for all executors to complete
-                        for future in concurrent.futures.as_completed(futures):
-                            try:
-                                future.result() # trigger an exception if occurred in any thread
-                            except Exception:
-                                _logger.exception('exception occurred')
-                        raise RuntimeError('received error from a thread')
-                    except queue.Empty:
-                        pass
-
-                    # try to get a value from the output queue
-                    try:
-                        (split_id, record_batch) = output_queue.get(timeout=1)
-                    except queue.Empty:
-                        continue
-
-                    if record_batch:
-                        # signal to the thread to read the next record batch and yield the current
-                        next_sems[split_id].release()
-                        try:
-                            yield record_batch
-                        except GeneratorExit:
-                            killall = True
-                            _logger.debug("cancelling query_iterator")
-                            raise
-                    else:
-                        done_count += 1
+        url_params = self._build_query_data_url_params(projection, query_imports_table)
 
-                # wait for all executors to complete
-                for future in concurrent.futures.as_completed(futures):
-                    try:
-                        future.result() # trigger an exception if occurred in any thread
-                    except Exception:
-                        _logger.exception('exception occurred')
-
-            # commit if needed
-            if created_txid:
-                self.commit_transaction(txid)
-
-        except Exception as e:
-            _logger.exception('exception occurred')
-            try:
-                self.rollback_transaction(txid)
-            except:
-                _logger.exception(f'failed to rollback txid {txid}')
-            raise e
-
-        finally:
-            killall = True
-            for session in executor_sessions:
-                try:
-                    session.session.close()
-                except Exception:
-                    _logger.exception(f'failed to close session {session}')
-
-    def query(self, bucket, schema, table, num_sub_splits=1, num_row_groups_per_sub_split=8,
-              response_row_id=False, txid=0, limit=0, limit_per_sub_split=131072, filters=None, field_names=None,
-              queried_columns=None):
-        """
-        query rows into a table.
-
-        Parameters
-        ----------
-        bucket : string
-            The bucket of the table.
-        schema : string
-            The schema of the table.
-        table : string
-            The table name.
-        num_sub_splits : integer
-            The number of sub_splits per split - determines the parallelism inside a VastDB compute node
-            default: 1
-        num_row_groups_per_sub_split : integer
-            The number of consecutive row groups per sub_split. Each row group consists of 64K row ids.
-            default: 8
-        response_row_id : boolean
-            Return a column with the internal row ids of the table
-            default: False
-        txid : integer
-            A transaction id. The transaction may be initiated before the query, and be used to provide
-            multiple ACID operations
-            default: 0 (will be created by the api)
-        limit : integer
-            Limit the number of rows in the response
-            default: 0 (no limit)
-        limit_per_sub_split : integer
-            Limit the number of rows from a single sub_split for a single rpc
-            default:131072
-        filters : dict
-            A dictionary whose keys are column names, and values are lists of string expressions that represent
-            filter conditions on the column. AND is applied on the conditions. The condition formats are:
-            'column_name eq some_value'
-            default: None
-        field_names : list
-            A list of column names to be returned to the output table
-            default: None
-        queried_columns: list of pyArrow.column
-            A list of the columns to be queried
-            default: None
-
-        Returns
-        -------
-        pyarrow.Table
-
-
-        Examples
-        --------
-        table = query('some_bucket', 'some_schema', 'some_table',
-                      filters={'name': ['eq Alice', 'eq Bob']}
-                      field_names=['name','age'])
-
-        """
-
-        # create a transaction
-        txid, created_txid = self._begin_tx_if_necessary(txid)
-        executor_sessions = []
-        try:
-            # prepare query
-            queried_columns, arrow_schema, query_data_request, executor_sessions = \
-                self._prepare_query(bucket, schema, table, num_sub_splits, filters, field_names, response_row_id=response_row_id, txid=txid)
-
-            # define the per split threaded query func
-            def query_split_id(self, split_id):
-                try:
-                    start_row_ids = {i:0 for i in range(num_sub_splits)}
-                    session = executor_sessions[split_id]
-                    row_count = 0
-                    while (self._more_pages_exist(start_row_ids) and
-                           (not limit or row_count < limit)):
-                        # check if killed externally
-                        if killall:
-                            raise RuntimeError(f'query_split_id: split_id {split_id} received killall')
-
-                        # determine the limit rows
-                        if limit:
-                            limit_rows = min(limit_per_sub_split, limit-row_count)
-                        else:
-                            limit_rows = limit_per_sub_split
-
-                        # query one page
-                        table_page, start_row_ids = session._query_page(bucket=bucket, schema=schema, table=table, query_data_request=query_data_request,
-                                                                        split=(split_id, num_splits, num_row_groups_per_sub_split),
-                                                                        num_sub_splits=num_sub_splits, response_row_id=response_row_id,
-                                                                        txid=txid, limit_rows=limit_rows,
-                                                                        sub_split_start_row_ids=start_row_ids.items())
-                        with lock:
-                            table_pages.append(table_page)
-                            row_counts[split_id] += len(table_page)
-                            row_count = sum(row_counts)
-                        _logger.info(f"query_split_id: table_pages split_id={split_id} row_count={row_count}")
-                except Exception as e:
-                    _logger.exception('query_split_id: exception occurred')
-                    try:
-                        self.rollback_transaction(txid)
-                    except:
-                        _logger.exception(f'failed to rollback txid {txid}')
-                    raise e
-
-            table_pages = []
-            num_splits = len(executor_sessions)
-            killall = False
-            with concurrent.futures.ThreadPoolExecutor(max_workers=num_splits) as executor:
-                futures = []
-                row_counts = [0] * num_splits
-                lock = threading.Lock()
-                for i in range(num_splits):
-                    futures.append(executor.submit(query_split_id, self, i))
-                for future in concurrent.futures.as_completed(futures):
-                    future.result() # trigger an exception if occurred in any thread
-
-            # commit if needed
-            if created_txid:
-                self.commit_transaction(txid)
-
-            # concatenate all table pages and return result
-            out_table = pa.concat_tables(table_pages)
-            out_table = out_table.slice(length=limit) if limit else out_table
-            _logger.info("query: out_table len=%s row_count=%s",
-                          len(out_table), len(out_table))
-            return out_table
-
-        except Exception as e:
-            _logger.exception('exception occurred')
-            try:
-                self.rollback_transaction(txid)
-            except:
-                _logger.exception(f'failed to rollback txid {txid}')
-            raise e
-
-        finally:
-            killall = True
-            for session in executor_sessions:
-                try:
-                    session.session.close()
-                except Exception:
-                    _logger.exception(f'failed to close session {session}')
+        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="data", url_params=url_params),
+                               data=params, headers=headers, stream=True)
+        return self._check_res(res, "query_data", expected_retvals)
 
     """
     source_files: list of (bucket_name, file_name)
     """
     def import_data(self, bucket, schema, table, source_files, txid=0, client_tags=[], expected_retvals=[], case_sensitive=True,
                     schedule_id=None, retry_count=0, blocking=True):
         """
@@ -1870,69 +1551,53 @@
         files = builder.EndVector()
         tabular_import_data.Start(builder)
         tabular_import_data.AddS3Files(builder, files)
         params = tabular_import_data.End(builder)
         builder.Finish(params)
         import_req = builder.Output()
 
-        def iterate_over_import_data_response(response, expected_retvals):
+        def iterate_over_import_data_response(response):
             if response.status_code != 200:
                 return response
 
             chunk_size = 1024
-            for chunk in res.iter_content(chunk_size=chunk_size):
+            for chunk in response.iter_content(chunk_size=chunk_size):
                 chunk_dict = json.loads(chunk)
-                _logger.info(f"import data chunk={chunk}, result: {chunk_dict['res']}")
-                if chunk_dict['res'] in expected_retvals:
-                    _logger.info(f"import finished with expected result={chunk_dict['res']}, error message: {chunk_dict['err_msg']}")
-                    return response
-                elif chunk_dict['res'] != 'Success' and chunk_dict['res'] != 'TabularInProgress':
-                    raise TabularException(f"Received unexpected error in import_data. "
-                                           f"status: {chunk_dict['res']}, error message: {chunk_dict['err_msg']}")
-                _logger.info(f"import_data is in progress. status: {chunk_dict['res']}")
+                _logger.debug("import data chunk=%s, result: %s", chunk_dict, chunk_dict['res'])
+                if chunk_dict['res'] != 'Success' and chunk_dict['res'] != 'TabularInProgress' and chunk_dict['res'] != 'TabularAlreadyImported':
+                    raise errors.ImportFilesError(
+                        f"Encountered an error during import_data. status: {chunk_dict['res']}, "
+                        f"error message: {chunk_dict['err_msg'] or 'Unexpected error'} during import of "
+                        f"object name: {chunk_dict['object_name']}", chunk_dict)
+                else:
+                    _logger.debug("import_data of object name '%s' is in progress. "
+                                  "status: %s", chunk_dict['object_name'], chunk_dict['res'])
             return response
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(import_req))
         headers['tabular-case-sensitive'] = str(case_sensitive)
         if schedule_id is not None:
             headers['tabular-schedule-id'] = str(schedule_id)
         if retry_count > 0:
             headers['tabular-retry-count'] = str(retry_count)
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="data"),
                                 data=import_req, headers=headers, stream=True)
         if blocking:
-            res = iterate_over_import_data_response(res, expected_retvals)
+            res = iterate_over_import_data_response(res)
 
         return self._check_res(res, "import_data", expected_retvals)
 
-    def merge_data(self):
-        """
-        TODO
-
-        POST /mybucket/myschema/mytable?data HTTP/1.1
-        Content-Length: ContentLength
-        tabular-txid: TransactionId
-        tabular-client-tag: ClientTag
-
-        Request Body
-        {
-          "format": "string",
-          "select_source": "formatted data"
-          "predicate": "formatted_data"
-        }
-        """
-        pass
-
     def _record_batch_slices(self, batch, rows_per_slice=None):
         max_slice_size_in_bytes = int(0.9*5*1024*1024) # 0.9 * 5MB
         batch_len = len(batch)
         serialized_batch = serialize_record_batch(batch)
         batch_size_in_bytes = len(serialized_batch)
-        _logger.info(f'max_slice_size_in_bytes={max_slice_size_in_bytes} batch_len={batch_len} batch_size_in_bytes={batch_size_in_bytes}')
+        _logger.debug('max_slice_size_in_bytes=%d batch_len=%d batch_size_in_bytes=%d',
+                      max_slice_size_in_bytes, batch_len, batch_size_in_bytes)
 
         if not rows_per_slice:
             if batch_size_in_bytes < max_slice_size_in_bytes:
                 rows_per_slice = batch_len
             else:
                 rows_per_slice = int(0.9 * batch_len * max_slice_size_in_bytes / batch_size_in_bytes)
 
@@ -1946,147 +1611,28 @@
                 if offset >= batch_len:
                     done_slicing=True
                     break
                 slice_batch = batch.slice(offset, rows_per_slice)
                 serialized_slice_batch = serialize_record_batch(slice_batch)
                 sizeof_serialized_slice_batch = len(serialized_slice_batch)
 
-                if sizeof_serialized_slice_batch <= max_slice_size_in_bytes or rows_per_slice < 10000:
+                if sizeof_serialized_slice_batch <= max_slice_size_in_bytes:
                     serialized_slices.append(serialized_slice_batch)
                 else:
                     _logger.info(f'Using rows_per_slice {rows_per_slice} slice {i} size {sizeof_serialized_slice_batch} exceeds {max_slice_size_in_bytes} bytes, trying smaller rows_per_slice')
                     # We have a slice that is too large
                     rows_per_slice = int(rows_per_slice/2)
                     if rows_per_slice < 1:
                         raise ValueError('cannot decrease batch size below 1 row')
                     break
             else:
                 done_slicing = True
 
         return serialized_slices
 
-    def insert(self, bucket, schema, table, rows=None, record_batch=None, rows_per_insert=None, txid=0):
-        """
-        Insert rows into a table. The operation may be split into multiple commands, such that by default no more than 512KB will be inserted per command.
-
-        Parameters
-        ----------
-        bucket : string
-            The bucket of the table.
-        schema : string
-            The schema of the table.
-        table : string
-            The table name.
-        rows : dict
-            The rows to insert.
-            dictionary key: column name
-            dictionary value: array of cell values to insert
-            default: None (if None, record_batch must be provided)
-        record_batch : pyarrow.RecordBatch
-            A pyarrow RecordBatch
-            default: None (if None, rows dictionary must be provided)
-        rows_per_insert : integer
-            Split the operation so that each insert command will be limited to this value
-            default: None (will be selected automatically)
-        txid : integer
-            A transaction id. The transaction may be initiated before the insert, and be used to provide
-            multiple ACID operations
-            default: 0 (will be created by the api)
-
-        Returns
-        -------
-        None
-
-
-        Examples
-        --------
-        insert('some_bucket', 'some_schema', 'some_table', {'name': ['Alice','Bob'], 'age': [25,24]})
-
-        """
-        if (not rows and not record_batch) or (rows and record_batch):
-            raise ValueError(f'insert: missing argument - either rows or record_batch must be provided')
-
-        # create a transaction
-        txid, created_txid = self._begin_tx_if_necessary(txid)
-
-        if rows:
-            columns = self._list_table_columns(bucket, schema, table, field_names=rows.keys(), txid=txid)
-            columns_dict = dict([(column[0], column[1]) for column in columns])
-            arrow_schema = pa.schema([])
-            arrays = []
-            for column_name, column_values in rows.items():
-                column_type = columns_dict[column_name]
-                field = pa.field(column_name, column_type)
-                arrow_schema = arrow_schema.append(field)
-                arrays.append(pa.array(column_values, column_type))
-            record_batch = pa.record_batch(arrays, arrow_schema)
-
-        # split the record batch into multiple slices
-        serialized_slices = self._record_batch_slices(record_batch, rows_per_insert)
-        _logger.info(f'inserting record batch using {len(serialized_slices)} slices')
-
-        insert_queue = queue.Queue()
-
-        [insert_queue.put(insert_rows_req) for insert_rows_req in serialized_slices]
-
-        try:
-            executor_sessions = [VastdbApi(self.executor_hosts[i], self.access_key, self.secret_key, self.username,
-                                           self.password, self.port, self.secure, self.auth_type) for i in range(len(self.executor_hosts))]
-
-            def insert_executor(self, split_id):
-
-                try:
-                    _logger.info(f'insert_executor split_id={split_id} starting')
-                    session = executor_sessions[split_id]
-                    num_inserts = 0
-                    while not killall:
-                        try:
-                            insert_rows_req = insert_queue.get(block=False)
-                        except queue.Empty:
-                            break
-                        session.insert_rows(bucket=bucket, schema=schema,
-                                            table=table, record_batch=insert_rows_req, txid=txid)
-                        num_inserts += 1
-                    _logger.info(f'insert_executor split_id={split_id} num_inserts={num_inserts}')
-                    if killall:
-                        _logger.info('insert_executor killall=True')
-
-                except Exception as e:
-                    _logger.exception('insert_executor hit exception')
-                    raise e
-
-            num_splits = len(executor_sessions)
-            killall = False
-            with concurrent.futures.ThreadPoolExecutor(max_workers=num_splits) as executor:
-                futures = []
-                for i in range(num_splits):
-                    futures.append(executor.submit(insert_executor, self, i))
-                for future in concurrent.futures.as_completed(futures):
-                    future.result() # trigger an exception if occurred in any thread
-
-            # commit if needed
-            if created_txid:
-                self.commit_transaction(txid)
-
-        except Exception as e:
-            _logger.exception('exception occurred')
-            try:
-                self.rollback_transaction(txid)
-            except:
-                _logger.exception(f'failed to rollback txid {txid}')
-            raise e
-
-        finally:
-            killall = True
-            for session in executor_sessions:
-                try:
-                    session.session.close()
-                except Exception:
-                    _logger.exception(f'failed to close session {session}')
-
     def insert_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
         """
         POST /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
@@ -2348,49 +1894,48 @@
                 raise EOFError(f'no readers ({readers}) should be open at EOF')
             break
 
         stream_id, = struct.unpack('<L', stream_id_bytes)
         if stream_ids is not None:
             stream_ids.update([stream_id])  # count stream IDs using a collections.Counter
         if stream_id == TABULAR_KEEP_ALIVE_STREAM_ID:
-#            _logger.info(f"stream_id={stream_id} (skipping)")
             continue
 
         if stream_id == TABULAR_QUERY_DATA_COMPLETED_STREAM_ID:
             # read the terminating end chunk from socket
             res = fileobj.read()
-            _logger.info(f"stream_id={stream_id} res={res} (finish)")
+            _logger.debug("stream_id=%d res=%s (finish)", stream_id, res)
             return
 
         if stream_id == TABULAR_QUERY_DATA_FAILED_STREAM_ID:
             # read the terminating end chunk from socket
             res = fileobj.read()
-            _logger.info(f"stream_id={stream_id} res={res} (failed)")
+            _logger.warning("stream_id=%d res=%s (failed)", stream_id, res)
             raise IOError(f"Query data stream failed res={res}")
 
         next_row_id_bytes = fileobj.read(8)
         next_row_id, = struct.unpack('<Q', next_row_id_bytes)
-        _logger.info(f"stream_id={stream_id} next_row_id={next_row_id}")
+        _logger.debug("stream_id=%d next_row_id=%d", stream_id, next_row_id)
 
         if stream_id not in readers:
             # we implicitly read 1st message (Arrow schema) when constructing RecordBatchStreamReader
             reader = pa.ipc.RecordBatchStreamReader(fileobj)
-            _logger.info(f"stream_id={stream_id} schema={reader.schema}")
+            _logger.debug("stream_id=%d schema=%s", stream_id, reader.schema)
             readers[stream_id] = (reader, [])
             continue
 
         (reader, batches) = readers[stream_id]
         try:
             batch = reader.read_next_batch() # read single-column chunk data
-            _logger.info(f"stream_id={stream_id} rows={len(batch)} chunk={batch}")
+            _logger.debug("stream_id=%d rows=%d chunk=%s", stream_id, len(batch), batch)
             batches.append(batch)
         except StopIteration:  # we got an end-of-stream IPC message for a given stream ID
             reader, batches = readers.pop(stream_id)  # end of column
             table = pa.Table.from_batches(batches)  # concatenate all column chunks (as a single)
-            _logger.info(f"stream_id={stream_id} rows={len(table)} column={table}")
+            _logger.debug("stream_id=%d rows=%d column=%s", stream_id, len(table), table)
             yield (stream_id, next_row_id, table)
 
 
 def parse_query_data_response(conn, schema, stream_ids=None, start_row_ids=None, debug=False):
     """
     Generates pyarrow.Table objects from QueryData API response stream.
 
@@ -2411,15 +1956,16 @@
 
         parsed_table = parser.build(output_field_names)
         if parsed_table is not None:  # when we got all columns (and before starting a new "select_rows" cycle)
             parsers.pop(stream_id)
             if is_empty_projection:  # VAST returns an empty RecordBatch, with the correct rows' count
                 parsed_table = table
 
-            _logger.info(f"stream_id={stream_id} rows={len(parsed_table)} next_row_id={next_row_id} table={parsed_table}")
+            _logger.debug("stream_id=%d rows=%d next_row_id=%d table=%s",
+                          stream_id, len(parsed_table), next_row_id, parsed_table)
             start_row_ids[stream_id] = next_row_id
             yield parsed_table  # the result of a single "select_rows()" cycle
 
     if parsers:
         raise EOFError(f'all streams should be done before EOF. {parsers}')
 
 def get_field_type(builder: flatbuffers.Builder, field: pa.Field):
@@ -2560,15 +2106,14 @@
 
     else:
         raise ValueError(f'unsupported predicate for type={field.type}')
 
     return field_type, field_type_type
 
 def build_field(builder: flatbuffers.Builder, f: pa.Field, name: str):
-    _logger.info(f"name={f.name}")
     children = None
     if isinstance(f.type, pa.StructType):
         children = [build_field(builder, child, child.name) for child in list(f.type)]
     if isinstance(f.type, pa.ListType):
         children = [build_field(builder, f.type.value_field, "item")]
     if isinstance(f.type, pa.MapType):
         children = [
@@ -2587,32 +2132,29 @@
         child_col_name = builder.CreateString("entries")
         fb_field.Start(builder)
         fb_field.AddTypeType(builder, field_type_type)
         fb_field.AddType(builder, field_type)
         fb_field.AddName(builder, child_col_name)
         fb_field.AddChildren(builder, children)
 
-        _logger.info(f"added key and map to entries")
         children = [fb_field.End(builder)]
 
     if children is not None:
         fb_field.StartChildrenVector(builder, len(children))
         for offset in reversed(children):
             builder.PrependUOffsetTRelative(offset)
         children = builder.EndVector()
 
     col_name = builder.CreateString(name)
     field_type, field_type_type = get_field_type(builder, f)
-    _logger.info(f"add col_name={name} type_type={field_type_type} to fb")
     fb_field.Start(builder)
     fb_field.AddName(builder, col_name)
     fb_field.AddTypeType(builder, field_type_type)
     fb_field.AddType(builder, field_type)
     if children is not None:
-        _logger.info(f"add col_name={name} childern")
         fb_field.AddChildren(builder, children)
     return fb_field.End(builder)
 
 
 class VastDBResponseSchema:
     def __init__(self, arrow_schema, projection_positions, output_field_names):
         self.arrow_schema = arrow_schema
@@ -2621,17 +2163,15 @@
 
 class QueryDataRequest:
     def __init__(self, serialized, response_schema):
         self.serialized = serialized
         self.response_schema = response_schema
 
 
-def build_query_data_request(schema: 'pa.Schema' = pa.schema([]), filters: dict = None, field_names: list = None):
-    filters = filters or {}
-
+def build_query_data_request(schema: 'pa.Schema' = pa.schema([]), predicate: ibis.expr.types.BooleanColumn = None, field_names: list = None):
     builder = flatbuffers.Builder(1024)
 
     source_name = builder.CreateString('')  # required
 
     fields = [build_field(builder, f, f.name) for f in schema]
 
     fb_schema.StartFieldsVector(builder, len(fields))
@@ -2639,46 +2179,42 @@
         builder.PrependUOffsetTRelative(offset)
     fields = builder.EndVector()
 
     fb_schema.Start(builder)
     fb_schema.AddFields(builder, fields)
     schema_obj = fb_schema.End(builder)
 
-    predicate = Predicate(schema, filters)
+    predicate = Predicate(schema=schema, expr=predicate)
     filter_obj = predicate.serialize(builder)
 
     parser = QueryDataParser(schema)
     leaves_map = {}
     for node in parser.nodes:
         for descendent in node._iter_nodes():
             if descendent.parent and isinstance(descendent.parent.type, (pa.ListType, pa.MapType)):
                 continue
             iter_from_root = reversed(list(descendent._iter_to_root()))
             descendent_full_name = '.'.join([n.field.name for n in iter_from_root])
-            _logger.debug(f'build_query_data_request: descendent_full_name={descendent_full_name}')
             descendent_leaves = [leaf.index for leaf in descendent._iter_leaves()]
             leaves_map[descendent_full_name] = descendent_leaves
-    _logger.debug(f'build_query_data_request: leaves_map={leaves_map}')
 
     output_field_names = None
     if field_names is None:
         field_names = [field.name for field in schema]
     else:
         output_field_names  = [f.split('.')[0] for f in field_names]
         # sort projected field_names according to positions to maintain ordering according to the schema
         def compare_field_names_by_pos(field_name1, field_name2):
             return leaves_map[field_name1][0]-leaves_map[field_name2][0]
         field_names = sorted(field_names, key=cmp_to_key(compare_field_names_by_pos))
-    _logger.debug(f'build_query_data_request: sorted field_names={field_names} schema={schema}')
 
     projection_fields = []
     projection_positions = []
     for field_name in field_names:
         positions = leaves_map[field_name]
-        _logger.info("projecting field=%s positions=%s", field_name, positions)
         projection_positions.extend(positions)
         for leaf_position in positions:
             fb_field_index.Start(builder)
             fb_field_index.AddPosition(builder, leaf_position)
             offset = fb_field_index.End(builder)
             projection_fields.append(offset)
     fb_source.StartProjectionVector(builder, len(projection_fields))
@@ -2727,17 +2263,15 @@
     for index, field in enumerate(table.schema):
         if isinstance(field.type, pa.TimestampType) and field.type.unit == 'ns':
             ts_indexes.append(index)
         if field.name in column_matcher:
             indexes_of_fields_to_change[field.name] = index
     for changing_index in ts_indexes:
         field_name = table.schema[changing_index].name
-        _logger.info(f'changing resolution for {field_name} to us')
         new_column = table[field_name].cast(pa.timestamp('us'), safe=False)
         table = table.set_column(changing_index, field_name, new_column)
     for field_name, changing_index in indexes_of_fields_to_change.items():
-        _logger.info(f'applying custom rules to {field_name}')
         new_column = table[field_name].to_pylist()
         new_column = list(map(column_matcher[field_name], new_column))
         new_column = pa.array(new_column, table[field_name].type)
         table = table.set_column(changing_index, field_name, new_column)
     return table
```

### Comparing `vastdb-0.0.5.3/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.0/vastdb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -145,16 +145,30 @@
 vast_flatbuf/tabular/GetTableStatsResponse.py
 vast_flatbuf/tabular/ImportDataRequest.py
 vast_flatbuf/tabular/ListProjectionsResponse.py
 vast_flatbuf/tabular/ListSchemasResponse.py
 vast_flatbuf/tabular/ListTablesResponse.py
 vast_flatbuf/tabular/ObjectDetails.py
 vast_flatbuf/tabular/S3File.py
+vast_flatbuf/tabular/VipRange.py
 vast_flatbuf/tabular/__init__.py
 vastdb/__init__.py
-vastdb/api.py
-vastdb/bench_scan.py
+vastdb/bucket.py
+vastdb/errors.py
+vastdb/internal_commands.py
+vastdb/schema.py
+vastdb/session.py
+vastdb/table.py
+vastdb/transaction.py
+vastdb/util.py
 vastdb.egg-info/PKG-INFO
 vastdb.egg-info/SOURCES.txt
 vastdb.egg-info/dependency_links.txt
 vastdb.egg-info/requires.txt
-vastdb.egg-info/top_level.txt
+vastdb.egg-info/top_level.txt
+vastdb/tests/__init__.py
+vastdb/tests/conftest.py
+vastdb/tests/test_imports.py
+vastdb/tests/test_projections.py
+vastdb/tests/test_sanity.py
+vastdb/tests/test_schemas.py
+vastdb/tests/test_tables.py
```

