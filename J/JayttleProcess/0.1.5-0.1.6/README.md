# Comparing `tmp/JayttleProcess-0.1.5-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 35315 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     2441 b- defN 24-Apr-10 05:07 JayttleProcess/CommonDecorator.py
+Zip file size: 35407 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     2458 b- defN 24-Apr-11 07:02 JayttleProcess/CommonDecorator.py
 -rw-rw-rw-  2.0 fat     4727 b- defN 24-Mar-19 06:31 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
--rw-rw-rw-  2.0 fat    16303 b- defN 24-Apr-10 06:43 JayttleProcess/SQLCommonUse.py
+-rw-rw-rw-  2.0 fat    16907 b- defN 24-Apr-11 07:08 JayttleProcess/SQLCommonUse.py
 -rw-rw-rw-  2.0 fat   117579 b- defN 24-Apr-08 05:24 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      861 b- defN 24-Apr-10 06:46 JayttleProcess-0.1.5.dist-info/RECORD
-10 files, 143262 bytes uncompressed, 33831 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      861 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/RECORD
+10 files, 143883 bytes uncompressed, 33923 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.1.5.dist-info/METADATA
+Filename: JayttleProcess-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.1.5.dist-info/WHEEL
+Filename: JayttleProcess-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.1.5.dist-info/top_level.txt
+Filename: JayttleProcess-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.1.5.dist-info/RECORD
+Filename: JayttleProcess-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/CommonDecorator.py

```diff
@@ -19,14 +19,15 @@
         print(f"Arguments: {all_args}")
 
         # 调用函数并记录返回值
         result = func(*args, **kwargs)
         print(f"Returned: {result}")
         end_time = time.time()  # 记录函数执行完毕的时间
         print(f"executed in {(end_time - start_time):.4f}s")  # 打印执行时间
+        print()
         return result
 
     return wrapper
 
 
 def cache_results(func):
     cache = {}  # 创建一个字典来存储之前的调用结果
```

## JayttleProcess/SQLCommonUse.py

```diff
@@ -91,21 +91,14 @@
 
 SQL_CONFIG = {
     "host": "localhost",
     "user": "Jayttle",
     "password": "@JayttleRoot",
     "database": "jayttle"
 }
-# # 全局变量存储数据库连接信息
-# SQL_CONFIG = {
-#     "host": "47.98.201.213",
-#     "user": "root",
-#     "password": "TJ1qazXSW@",
-#     "database": "tianmeng_cableway"
-# }
 
 
 def execute_sql(sql_statement: str) -> Union[str, list[tuple]]:
     # 建立数据库连接
     conn = pymysql.connect(**SQL_CONFIG)
     cursor = conn.cursor()
     
@@ -424,23 +417,14 @@
     except Exception as e:
         print("Error executing SQL statement:", e)
         return None
     finally:
         cursor.close()
         conn.close()
 
-# list_name = "met"
-# start_time = "2024-04-07 00:00:00"
-# end_time = "2024-05-07 00:00:00"
-
-# # 调用函数并存储结果
-# query_result = query_time_difference(list_name, start_time, end_time)
-# print("Query Result:")
-# for row in query_result:
-#     print(row)
 
 def extract_time_data() -> list[tuple[datetime]]:
     # 查询 Time 属性的数据
     query = "SELECT Time FROM met"
     
     # 执行查询语句
     results = execute_sql(query)
@@ -517,8 +501,38 @@
     plt.xlabel('属性名', fontproperties='SimHei')  # 使用中文标签
     plt.ylabel('时间', fontproperties='SimHei')  # 使用中文标签
     plt.title('数据存在情况热图', fontproperties='SimHei')  # 使用中文标题
     plt.tight_layout()
     plt.show()
 
 
+def count_records_in_table(table_name: str) -> int:
+    """查看数据库中的表有多少个数据"""
+    # 建立数据库连接
+    conn = pymysql.connect(**SQL_CONFIG)
+    cursor = conn.cursor()
+
+    try:
+        # 构建 SQL 查询语句，统计表中的数据行数
+        sql_statement = f"SELECT COUNT(*) FROM {table_name}"
+        
+        # 执行 SQL 查询
+        cursor.execute(sql_statement)
+        
+        # 获取查询结果
+        result = cursor.fetchone()  # fetchone() 用于获取单行结果
+        if result:
+            record_count = result[0]  # 查询结果是一个包含一个元素的 tuple，获取第一个元素即数据行数
+            return record_count  # 返回数据行数
 
+        else:
+            return 0  # 如果结果为空，则返回 0 条数据
+
+    except Exception as e:
+        # 发生错误时回滚
+        conn.rollback()
+        raise e  # 将异常抛出，由调用者处理
+
+    finally:
+        # 关闭游标和数据库连接
+        cursor.close()
+        conn.close()
```

## Comparing `JayttleProcess-0.1.5.dist-info/METADATA` & `JayttleProcess-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.1.5
+Version: 0.1.6
 Summary: modifty time:2024-04-06 23:00
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
```

