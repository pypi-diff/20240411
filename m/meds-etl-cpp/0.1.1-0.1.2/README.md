# Comparing `tmp/meds_etl_cpp-0.1.1.tar.gz` & `tmp/meds_etl_cpp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds_etl_cpp-0.1.1.tar", last modified: Mon Apr  8 05:18:12 2024, max compression
+gzip compressed data, was "meds_etl_cpp-0.1.2.tar", last modified: Thu Apr 11 16:03:10 2024, max compression
```

## Comparing `meds_etl_cpp-0.1.1.tar` & `meds_etl_cpp-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.043821 meds_etl_cpp-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.047821 meds_etl_cpp-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/.github/workflows/python-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:18:11.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 05:18:12.000000 meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.047821 meds_etl_cpp-0.1.1/native/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/.bazelrc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/WORKSPACE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/backupbazelrc
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/main.cc
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/meds_etl_cpp.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:18:12.047821 meds_etl_cpp-0.1.1/native/patches/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/patches/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/patches/ThirdpartyToolchain.cmake.patch
--rw-r--r--   0 runner    (1001) docker     (127)    48502 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/perform_etl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/perform_etl.hh
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/native/simple_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:18:12.051821 meds_etl_cpp-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-08 05:18:07.000000 meds_etl_cpp-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:03:10.283598 meds_etl_cpp-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:03:10.275598 meds_etl_cpp-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:03:10.279598 meds_etl_cpp-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 16:03:10.279598 meds_etl_cpp-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:03:10.279598 meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 16:03:10.000000 meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 16:03:10.000000 meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:03:10.000000 meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:03:10.000000 meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 16:03:10.000000 meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:03:10.279598 meds_etl_cpp-0.1.2/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/.bazelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/WORKSPACE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/backupbazelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/meds_etl_cpp.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:03:10.279598 meds_etl_cpp-0.1.2/native/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/patches/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/patches/ThirdpartyToolchain.cmake.patch
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/pdqsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49548 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/perform_etl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/perform_etl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/native/simple_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:03:10.283598 meds_etl_cpp-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-11 16:03:06.000000 meds_etl_cpp-0.1.2/setup.py
```

### Comparing `meds_etl_cpp-0.1.1/.github/workflows/python-build.yml` & `meds_etl_cpp-0.1.2/.github/workflows/python-build.yml`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.1/LICENSE` & `meds_etl_cpp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.1/meds_etl_cpp.egg-info/SOURCES.txt` & `meds_etl_cpp-0.1.2/meds_etl_cpp.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 native/.bazelrc
 native/.clang-format
 native/BUILD
 native/WORKSPACE
 native/backupbazelrc
 native/main.cc
 native/meds_etl_cpp.cc
+native/pdqsort.h
 native/perform_etl.cc
 native/perform_etl.hh
 native/simple_test.cc
 native/patches/BUILD
 native/patches/ThirdpartyToolchain.cmake.patch
```

### Comparing `meds_etl_cpp-0.1.1/native/BUILD` & `meds_etl_cpp-0.1.2/native/BUILD`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 cc_binary(
     name="simple_test",
     srcs=["simple_test.cc"],
 )
 
 cc_library(
     name="perform_etl",
-    srcs=["perform_etl.cc"],
+    srcs=["perform_etl.cc", "pdqsort.h"],
     hdrs=["perform_etl.hh"],
     deps=[
         ":arrow", 
         "@com_google_absl//absl/types:optional",
         "@readerwriterqueue",
         "@concurrentqueue",
         ":zstd",
```

### Comparing `meds_etl_cpp-0.1.1/native/WORKSPACE` & `meds_etl_cpp-0.1.2/native/WORKSPACE`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.1/native/patches/ThirdpartyToolchain.cmake.patch` & `meds_etl_cpp-0.1.2/native/patches/ThirdpartyToolchain.cmake.patch`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.1/native/perform_etl.cc` & `meds_etl_cpp-0.1.2/native/perform_etl.cc`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,45 @@
 #include "arrow/table.h"
 #include "arrow/util/type_fwd.h"
 #include "blockingconcurrentqueue.h"
 #include "lightweightsemaphore.h"
 #include "parquet/arrow/reader.h"
 #include "parquet/arrow/schema.h"
 #include "parquet/arrow/writer.h"
+#include "pdqsort.h"
 #include "zstd.h"
 
 namespace fs = std::filesystem;
 
-const size_t SHARD_PIECE_SIZE = 2 * 1000 * 1000 * 1000;  // Roughly 2 gigabytes
-const size_t COMPRESSION_BUFFER_SIZE = 4 * 1000 * 1000;  // Roughly 4 megabytes
+const size_t SHARD_PIECE_SIZE =
+    ((size_t)4 * 1000) * 1000 * 1000;  // Roughly 4 gigabytes
+const size_t PARQUET_PIECE_SIZE =
+    ((size_t)100) * 1000 * 1000;  // Roughly 100 megabytes
+const size_t COMPRESSION_BUFFER_SIZE = 1 * 1000 * 1000;  // Roughly 1 megabytes
+
+template <typename T, bool reversed = false>
+struct EventComparator {
+    bool operator()(const T& a, const T& b) const {
+        if (reversed) {
+            return (std::get<0>(a) > std::get<0>(b)) |
+                   ((std::get<0>(a) == std::get<0>(b)) &
+                    (std::get<1>(a) > std::get<1>(b)));
+        } else {
+            return (std::get<0>(a) < std::get<0>(b)) |
+                   ((std::get<0>(a) == std::get<0>(b)) &
+                    (std::get<1>(a) < std::get<1>(b)));
+        }
+    }
+};
 
 std::vector<std::shared_ptr<::arrow::Field>> get_fields_for_file(
     arrow::MemoryPool* pool, const std::string& filename) {
     // Configure general Parquet reader settings
     auto reader_properties = parquet::ReaderProperties(pool);
-    reader_properties.set_buffer_size(4096 * 4);
+    reader_properties.set_buffer_size(1024 * 1024);
     reader_properties.enable_buffered_stream();
 
     // Configure Arrow-specific Parquet reader settings
     auto arrow_reader_props = parquet::ArrowReaderProperties();
     arrow_reader_props.set_batch_size(128 * 1024);  // default 64 * 1024
 
     parquet::arrow::FileReaderBuilder reader_builder;
@@ -129,42 +148,14 @@
     for (auto& res : results) {
         result.merge(std::move(res));
     }
 
     return result;
 }
 
-/*
-struct Row {
-    int64_t patient_id;
-
-    int64_t time; // Actually an Arrow Timestamp with microsecond precision
-
-    std::string code;
-
-    absl::optional<float> numeric_value;
-    absl::optional<int64_t> datetime_value; // Actually an Arrow Timestamp with
-microsecond precision absl::optional<std::string> text_value;
-
-    std::vector<absl::optional<std::string>> metadata_columns;
-};
-
-struct Row {
-    int64_t patient_id;
-    int64_t time;
-
-    std::vector<char> data;
-
-    bool operator<(const Row& rhs) {
-        return std::make_pair(patient_id, time) <
-               std::make_pair(rhs.patient_id, rhs.time);
-    }
-};
-*/
-
 template <typename T>
 void add_literal_to_vector(std::vector<char>& data, T to_add) {
     const char* bytes = reinterpret_cast<const char*>(&to_add);
     data.insert(std::end(data), bytes, bytes + sizeof(T));
 }
 
 void add_string_to_vector(std::vector<char>& data, std::string_view to_add) {
@@ -201,15 +192,15 @@
         if (!item) {
             break;
         } else {
             auto source = *item;
 
             // Configure general Parquet reader settings
             auto reader_properties = parquet::ReaderProperties(pool);
-            reader_properties.set_buffer_size(4096 * 4);
+            reader_properties.set_buffer_size(1024 * 1024);
             reader_properties.enable_buffered_stream();
 
             // Configure Arrow-specific Parquet reader settings
             auto arrow_reader_props = parquet::ArrowReaderProperties();
             arrow_reader_props.set_batch_size(128 * 1024);  // default 64 * 1024
 
             parquet::arrow::FileReaderBuilder reader_builder;
@@ -832,15 +823,17 @@
                 data.insert(std::end(data), std::begin(std::get<2>(*next)),
                             std::end(std::get<2>(*next)));
                 row_indices.push_back(std::make_tuple(
                     std::get<0>(*next), std::get<1>(*next), start, length));
             }
         }
 
-        std::sort(std::begin(row_indices), std::end(row_indices));
+        pdqsort_branchless(
+            std::begin(row_indices), std::end(row_indices),
+            EventComparator<decltype(row_indices)::value_type>());
 
         {
             ZstdRowWriter writer(filename, compression_context.get());
 
             for (const auto& row_index : row_indices) {
                 writer.add_next(
                     std::string_view(data.data() + std::get<2>(row_index),
@@ -930,17 +923,19 @@
                               target_directory, &sort_queue,
                               &remaining_live_writers]() {
             shard_writer(i, num_shards, write_queues[i], write_semaphore,
                          target_directory / std::to_string(i), sort_queue,
                          remaining_live_writers);
         });
 
-        threads.emplace_back([&sort_queue, &remaining_live_writers]() {
-            shard_sort(sort_queue, remaining_live_writers);
-        });
+        if (i % 2 == 0) {
+            threads.emplace_back([&sort_queue, &remaining_live_writers]() {
+                shard_sort(sort_queue, remaining_live_writers);
+            });
+        }
     }
 
     for (auto& thread : threads) {
         thread.join();
     }
 
     absl::optional<std::string> next_entry;
@@ -970,29 +965,35 @@
         } else {
             is_text_metadata[i] = false;
             metadata_fields.push_back(
                 arrow::field(metadata_column.first, metadata_column.second));
         }
     }
 
-    auto metadata_type = std::make_shared<arrow::StructType>(metadata_fields);
+    std::shared_ptr<arrow::DataType> metadata_type;
+    if (metadata_columns.size() != 0) {
+        metadata_type = std::make_shared<arrow::StructType>(metadata_fields);
+    } else {
+        metadata_type = std::make_shared<arrow::FloatType>();
+    }
 
     auto timestamp_type =
         std::make_shared<arrow::TimestampType>(arrow::TimeUnit::MICRO);
 
     auto measurement_type_fields = {
         arrow::field("code", std::make_shared<arrow::StringType>()),
 
         arrow::field("text_value", std::make_shared<arrow::StringType>()),
         arrow::field("numeric_value", std::make_shared<arrow::FloatType>()),
         arrow::field("datetime_value", std::make_shared<arrow::TimestampType>(
                                            arrow::TimeUnit::MICRO)),
 
         arrow::field("metadata", metadata_type),
     };
+
     auto measurement_type =
         std::make_shared<arrow::StructType>(measurement_type_fields);
 
     auto event_type_fields = {
         arrow::field("time", std::make_shared<arrow::TimestampType>(
                                  arrow::TimeUnit::MICRO)),
         arrow::field("measurements",
@@ -1046,15 +1047,15 @@
         source_files.emplace_back(entry.path(), context.get());
     }
 
     typedef std::tuple<int64_t, int64_t, size_t, std::string_view>
         PriorityQueueItem;
 
     std::priority_queue<PriorityQueueItem, std::vector<PriorityQueueItem>,
-                        std::greater<PriorityQueueItem>>
+                        EventComparator<PriorityQueueItem, true>>
         queue;
 
     for (size_t i = 0; i < source_files.size(); i++) {
         auto next_entry = source_files[i].get_next();
         if (!next_entry) {
             continue;
         }
@@ -1075,37 +1076,49 @@
     auto datetime_value_builder =
         std::make_shared<arrow::TimestampBuilder>(timestamp_type, pool);
 
     std::vector<std::shared_ptr<arrow::StringBuilder>> text_metadata_builders(
         metadata_columns.size());
     std::vector<std::shared_ptr<arrow::FixedSizeBinaryBuilder>>
         primitive_metadata_builders(metadata_columns.size());
-    std::vector<std::shared_ptr<arrow::ArrayBuilder>> metadata_builders(
-        metadata_columns.size());
-    for (size_t i = 0; i < metadata_columns.size(); i++) {
-        if (is_text_metadata[i]) {
-            auto builder = std::make_shared<arrow::StringBuilder>(pool);
-            text_metadata_builders[i] = builder;
-            metadata_builders[i] = builder;
-        } else {
-            auto builder = std::make_shared<arrow::FixedSizeBinaryBuilder>(
-                std::make_shared<arrow::FixedSizeBinaryType>(
-                    metadata_columns[i].second->byte_width()));
-            primitive_metadata_builders[i] = builder;
-            metadata_builders[i] = builder;
+
+    std::shared_ptr<arrow::StructBuilder> metadata_builder;
+    std::shared_ptr<arrow::FloatBuilder> null_metadata_builder;
+    std::shared_ptr<arrow::ArrayBuilder> metadata_builder_holder;
+
+    if (metadata_columns.size() != 0) {
+        std::vector<std::shared_ptr<arrow::ArrayBuilder>> metadata_builders(
+            metadata_columns.size());
+        for (size_t i = 0; i < metadata_columns.size(); i++) {
+            if (is_text_metadata[i]) {
+                auto builder = std::make_shared<arrow::StringBuilder>(pool);
+                text_metadata_builders[i] = builder;
+                metadata_builders[i] = builder;
+            } else {
+                auto builder = std::make_shared<arrow::FixedSizeBinaryBuilder>(
+                    std::make_shared<arrow::FixedSizeBinaryType>(
+                        metadata_columns[i].second->byte_width()));
+                primitive_metadata_builders[i] = builder;
+                metadata_builders[i] = builder;
+            }
         }
-    }
 
-    auto metadata_builder = std::make_shared<arrow::StructBuilder>(
-        metadata_type, pool, metadata_builders);
+        metadata_builder = std::make_shared<arrow::StructBuilder>(
+            metadata_type, pool, metadata_builders);
+        metadata_builder_holder = metadata_builder;
+    } else {
+        null_metadata_builder = std::make_shared<arrow::FloatBuilder>(pool);
+        metadata_builder_holder = null_metadata_builder;
+    }
 
     std::vector<std::shared_ptr<arrow::ArrayBuilder>>
-        measurement_builder_fields{code_builder, text_value_builder,
-                                   numeric_value_builder,
-                                   datetime_value_builder, metadata_builder};
+        measurement_builder_fields{
+            code_builder, text_value_builder, numeric_value_builder,
+            datetime_value_builder, metadata_builder_holder};
+
     auto measurement_builder = std::make_shared<arrow::StructBuilder>(
         measurement_type, pool, measurement_builder_fields);
 
     auto time_builder =
         std::make_shared<arrow::TimestampBuilder>(timestamp_type, pool);
     auto measurements_builder =
         std::make_shared<arrow::ListBuilder>(pool, measurement_builder);
@@ -1126,14 +1139,15 @@
 
         std::shared_ptr<arrow::Array> events_array;
         PARQUET_THROW_NOT_OK(events_builder->Finish(&events_array));
         PARQUET_ASSIGN_OR_THROW(columns[2], events_array->View(events_type));
 
         std::shared_ptr<arrow::Table> table =
             arrow::Table::Make(schema, columns);
+
         PARQUET_THROW_NOT_OK(writer->WriteTable(*table));
 
         amount_written = 0;
     };
 
     bool is_first = true;
     int64_t last_patient_id = -1;
@@ -1147,15 +1161,15 @@
         int64_t time = std::get<1>(next);
         std::string_view patient_record = std::get<3>(next);
         amount_written += patient_record.size();
 
         if (patient_id != last_patient_id || is_first) {
             is_first = false;
 
-            if (amount_written > SHARD_PIECE_SIZE) {
+            if (amount_written > PARQUET_PIECE_SIZE) {
                 flush_arrays();
             }
 
             last_patient_id = patient_id;
             last_time = time;
 
             PARQUET_THROW_NOT_OK(patient_id_builder->Append(patient_id));
@@ -1212,37 +1226,42 @@
             PARQUET_THROW_NOT_OK(text_value_builder->Append(
                 patient_record.substr(offset, size)));
             offset += size;
         } else {
             PARQUET_THROW_NOT_OK(text_value_builder->AppendNull());
         }
 
-        PARQUET_THROW_NOT_OK(metadata_builder->Append());
-        for (size_t j = 0; j < metadata_columns.size(); j++) {
-            if (non_null[3 + j]) {
-                size_t size = *reinterpret_cast<const size_t*>(
-                    patient_record.substr(offset).data());
-                offset += sizeof(size);
-                auto entry = patient_record.substr(offset, size);
-
-                if (is_text_metadata[j]) {
-                    PARQUET_THROW_NOT_OK(
-                        text_metadata_builders[j]->Append(entry));
-                } else {
-                    PARQUET_THROW_NOT_OK(
-                        primitive_metadata_builders[j]->Append(entry));
-                }
-                offset += size;
-            } else {
-                if (is_text_metadata[j]) {
-                    PARQUET_THROW_NOT_OK(
-                        text_metadata_builders[j]->AppendNull());
+        if (metadata_columns.size() == 0) {
+            PARQUET_THROW_NOT_OK(null_metadata_builder->AppendNull());
+        } else {
+            PARQUET_THROW_NOT_OK(metadata_builder->Append());
+
+            for (size_t j = 0; j < metadata_columns.size(); j++) {
+                if (non_null[3 + j]) {
+                    size_t size = *reinterpret_cast<const size_t*>(
+                        patient_record.substr(offset).data());
+                    offset += sizeof(size);
+                    auto entry = patient_record.substr(offset, size);
+
+                    if (is_text_metadata[j]) {
+                        PARQUET_THROW_NOT_OK(
+                            text_metadata_builders[j]->Append(entry));
+                    } else {
+                        PARQUET_THROW_NOT_OK(
+                            primitive_metadata_builders[j]->Append(entry));
+                    }
+                    offset += size;
                 } else {
-                    PARQUET_THROW_NOT_OK(
-                        primitive_metadata_builders[j]->AppendNull());
+                    if (is_text_metadata[j]) {
+                        PARQUET_THROW_NOT_OK(
+                            text_metadata_builders[j]->AppendNull());
+                    } else {
+                        PARQUET_THROW_NOT_OK(
+                            primitive_metadata_builders[j]->AppendNull());
+                    }
                 }
             }
         }
 
         size_t file_index = std::get<2>(next);
         auto next_entry = source_files[file_index].get_next();
         if (!next_entry) {
```

### Comparing `meds_etl_cpp-0.1.1/pyproject.toml` & `meds_etl_cpp-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.1.1/setup.py` & `meds_etl_cpp-0.1.2/setup.py`

 * *Files identical despite different names*

