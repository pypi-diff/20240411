# Comparing `tmp/tableshare-1.1.4.tar.gz` & `tmp/tableshare-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableshare-1.1.4.tar", last modified: Thu Apr 11 13:55:48 2024, max compression
+gzip compressed data, was "tableshare-1.1.5.tar", last modified: Thu Apr 11 14:52:34 2024, max compression
```

## Comparing `tableshare-1.1.4.tar` & `tableshare-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 13:55:48.526637 tableshare-1.1.4/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:58:56.000000 tableshare-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      931 2024-04-11 13:55:48.526637 tableshare-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2305 2024-02-28 05:51:28.000000 tableshare-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 13:55:48.526637 tableshare-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1791 2024-04-11 13:54:41.000000 tableshare-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:55:48.509932 tableshare-1.1.4/tableshare/
--rw-rw-rw-   0        0        0     8814 2024-04-07 14:08:02.000000 tableshare-1.1.4/tableshare/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:55:48.509932 tableshare-1.1.4/tableshare.egg-info/
--rw-rw-rw-   0        0        0      931 2024-04-11 13:55:48.000000 tableshare-1.1.4/tableshare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-11 13:55:48.000000 tableshare-1.1.4/tableshare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 13:55:48.000000 tableshare-1.1.4/tableshare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-11 13:55:48.000000 tableshare-1.1.4/tableshare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-11 13:55:48.000000 tableshare-1.1.4/tableshare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:52:34.251403 tableshare-1.1.5/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:58:56.000000 tableshare-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      931 2024-04-11 14:52:34.251403 tableshare-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2305 2024-02-28 05:51:28.000000 tableshare-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:52:34.251403 tableshare-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1791 2024-04-11 14:52:31.000000 tableshare-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:52:34.235813 tableshare-1.1.5/tableshare/
+-rw-rw-rw-   0        0        0     9349 2024-04-11 14:49:31.000000 tableshare-1.1.5/tableshare/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:52:34.251403 tableshare-1.1.5/tableshare/crawltable/
+-rw-rw-rw-   0        0        0     8144 2024-04-11 14:50:44.000000 tableshare-1.1.5/tableshare/crawltable/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:52:34.251403 tableshare-1.1.5/tableshare.egg-info/
+-rw-rw-rw-   0        0        0      931 2024-04-11 14:52:34.000000 tableshare-1.1.5/tableshare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-04-11 14:52:34.000000 tableshare-1.1.5/tableshare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:52:34.000000 tableshare-1.1.5/tableshare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-11 14:52:34.000000 tableshare-1.1.5/tableshare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-11 14:52:34.000000 tableshare-1.1.5/tableshare.egg-info/top_level.txt
```

### Comparing `tableshare-1.1.4/LICENSE` & `tableshare-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tableshare-1.1.4/PKG-INFO` & `tableshare-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableshare
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python library for scraping and sharing table data from web pages.
 Home-page: https://github.com/baiguanba/tableshare
 Author: Guanba
 Author-email: baiguanba@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baiguanba/tableshare/issues
 Keywords: python,table,webtable,scrawler
```

### Comparing `tableshare-1.1.4/README.md` & `tableshare-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tableshare-1.1.4/setup.py` & `tableshare-1.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from setuptools import setup, find_packages
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 DESCRIPTION = 'A Python library for scraping and sharing table data from web pages.'
 
 setup(
     name='tableshare',
     version=VERSION,  # 请在发布新版本时更新这个版本号
     author='Guanba',  # 替换为你的名字
     author_email='baiguanba@outlook.com',  # 替换为你的电子邮件地址
```

### Comparing `tableshare-1.1.4/tableshare/__init__.py` & `tableshare-1.1.5/tableshare/crawltable/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,174 +12,175 @@
 from DrissionPage import WebPage
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 import numpy as np
 
 
+"""
+爬取各种静态和动态网页
+"""
+
+
+def __init__(self):
+    self.tables = None
+
+def scrape_tables(url, dynamic=False):
+    try:
+        if dynamic:
+            # path = r'"C:\Program Files\Google\Chrome\Application\chrome.exe"'  # 请改为你电脑内Chrome可执行文件路径
+            path = r'"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"'  # 请改为你电脑内Edge可执行文件路径
+            ChromiumOptions().set_browser_path(path).save()
+            wp = WebPage()
+            wp.listen.start(url)  # 监听Json
+            wp.get(url)
+            packet = wp.listen.wait()
+
+            # 假设 packet.response.body 包含了 HTML 内容
+            html_content = packet.response.body
+            # 使用 BeautifulSoup 解析 HTML
+            soup = BeautifulSoup(html_content, 'lxml')
+        else:
+            response = requests.get(url, headers={
+                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) '
+                              'Chrome/72.0.3626.119 Safari/537.36'})
+            response.encoding = 'utf-8'  # 设置编码为'utf-8'
+            # 使用 BeautifulSoup 解析 HTML
+            soup = BeautifulSoup(response.text, 'html.parser')
+
+        tables = soup.find_all('table')
+        return tables
+    except Exception as e:
+        print(f"请求或解析网页时发生错误: {e}")
+        return None
+
+# 提取表头
+def extract_headers(table):
+    # 提取表头（<th>标签的内容）
+    headers = []
+    header_row = table.find('thead')  # 找出table下所有thead标签
+    if header_row and header_row.find_all('th'):  # 确保header_row存在且包含<th>标签
+        # 遍历每个<th>标签
+        for th in header_row.find_all('th'):
+            # 使用get_text()方法来获取包括span标签在内的所有文本
+            header_text = th.get_text(strip=True)
+            # 如果文本内容为空，则添加默认列名
+            if not header_text:
+                header_text = 'Column' + str(len(headers) + 1)
+            headers.append(header_text)
+    # 如果没有th标签，则设置默认列名,len(table.find_all('tr')[1])是获取第2个tr标签里td的数量
+    if not headers:
+        headers = ['Column' + str(ii) for ii in range(1, len(table.find_all('tr')[0]) + 1)]
+    return headers
+
+# 提取table为pandas数据表
+def extract_table_data(table, headers, table_index):
+    data = []
+    tbody = []
+    tbody_row = table.find('tbody')  # 找出table下所有tbody标签
+    if tbody_row and tbody_row.find_all('tr'):  # 确保tbody_row存在且包含<tr>标签
+        # 提取表格数据（<td>标签的内容）
+        for row_index, row in enumerate(tbody_row.find_all('tr'), start=1):  # 从1开始计数
+            cols = row.find_all(['td', 'th'])
+            if cols:
+                col_count = len([col for col in cols if col.name == 'td'])
+                row_data = []
+                # 1.如果当前行的<td>数量与表头列数一致
+                if col_count == len(headers):
+                    for col in cols:
+                        if col.name == 'td':
+                            row_data.append(col.text.strip())
+                # 2.如果当前行的<td>数量小于表头列数，补齐空值（这部分代码已在之前的回答中提供）
+                elif col_count < len(headers):
+                    for col in cols:
+                        if col.name == 'td':
+                            row_data.append(col.text.strip())
+                    row_data += [''] * (len(headers) - len(row_data))
+                    print(
+                        f"警告：在处理Table {table_index + 1}，第 {row_index} 行时，发现列数({col_count})少于表头列数({len(headers)})，已补齐空值处理。")
 
-
-class TableScraper:
-    def __init__(self):
-        self.tables = None
-
-    @staticmethod
-    def scrape_tables(url, dynamic=False):
-        try:
-            if dynamic:
-                # path = r'"C:\Program Files\Google\Chrome\Application\chrome.exe"'  # 请改为你电脑内Chrome可执行文件路径
-                path = r'"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"'  # 请改为你电脑内Edge可执行文件路径
-                ChromiumOptions().set_browser_path(path).save()
-                wp = WebPage()
-                wp.listen.start(url)  # 监听Json
-                wp.get(url)
-                packet = wp.listen.wait()
-
-                # 假设 packet.response.body 包含了 HTML 内容
-                html_content = packet.response.body
-                # 使用 BeautifulSoup 解析 HTML
-                soup = BeautifulSoup(html_content, 'lxml')
-            else:
-                response = requests.get(url, headers={
-                    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) '
-                                  'Chrome/72.0.3626.119 Safari/537.36'})
-                response.encoding = 'utf-8'  # 设置编码为'utf-8'
-                # 使用 BeautifulSoup 解析 HTML
-                soup = BeautifulSoup(response.text, 'html.parser')
-
-            tables = soup.find_all('table')
-            return tables
-        except Exception as e:
-            print(f"请求或解析网页时发生错误: {e}")
-            return None
-
-    @staticmethod # 提取表头
-    def extract_headers(table):
-        # 提取表头（<th>标签的内容）
-        headers = []
-        header_row = table.find('thead')  # 找出table下所有thead标签
-        if header_row and header_row.find_all('th'):  # 确保header_row存在且包含<th>标签
-            # 遍历每个<th>标签
-            for th in header_row.find_all('th'):
-                # 使用get_text()方法来获取包括span标签在内的所有文本
-                header_text = th.get_text(strip=True)
-                # 如果文本内容为空，则添加默认列名
-                if not header_text:
-                    header_text = 'Column' + str(len(headers) + 1)
-                headers.append(header_text)
-        # 如果没有th标签，则设置默认列名,len(table.find_all('tr')[1])是获取第2个tr标签里td的数量
-        if not headers:
-            headers = ['Column' + str(ii) for ii in range(1, len(table.find_all('tr')[0]) + 1)]
-        return headers
-
-    @staticmethod  # 提取table为pandas数据表
-    def extract_table_data(table, headers, table_index):
-        data = []
-        tbody = []
-        tbody_row = table.find('tbody')  # 找出table下所有tbody标签
-        if tbody_row and tbody_row.find_all('tr'):  # 确保tbody_row存在且包含<tr>标签
-            # 提取表格数据（<td>标签的内容）
-            for row_index, row in enumerate(tbody_row.find_all('tr'), start=1):  # 从1开始计数
-                cols = row.find_all(['td', 'th'])
-                if cols:
-                    col_count = len([col for col in cols if col.name == 'td'])
-                    row_data = []
-                    # 1.如果当前行的<td>数量与表头列数一致
-                    if col_count == len(headers):
-                        for col in cols:
-                            if col.name == 'td':
-                                row_data.append(col.text.strip())
-                    # 2.如果当前行的<td>数量小于表头列数，补齐空值（这部分代码已在之前的回答中提供）
-                    elif col_count < len(headers):
-                        for col in cols:
-                            if col.name == 'td':
-                                row_data.append(col.text.strip())
-                        row_data += [''] * (len(headers) - len(row_data))
-                        print(
-                            f"警告：在处理Table {table_index + 1}，第 {row_index} 行时，发现列数({col_count})少于表头列数({len(headers)})，已补齐空值处理。")
-
-                        # 3.如果当前行的<td>数量大于表头列数，新增列并保留超出的数据
-                    else:
-                        for num in range(len(headers)):
-                            col = cols[num]
-                            if col.name == 'td':
-                                row_data.append(col.text.strip())
-                        # 新增额外的列，列名为Column+额外列数，并将超出的数据作为该列的值
-                        for extra_col in cols[len(headers):]:
-                            row_data.append(extra_col.text.strip())
-                            headers.append('Column' + str(len(headers) + 1))
-                        print(
-                            f"警告：在处理Table {table_index + 1}，第 {row_index} 行时，发现列数({col_count})超出表头列数({len(headers)})，已新增额外列处理。")
-                    data.append(row_data)
-
-            # 如果data列表为空（即没有有效的数据行），则不创建DataFrame
-            if data:
-                # 创建DataFrame
-                df = pd.DataFrame(data, columns=headers)
-                # 打印DataFrame的前几行，以验证数据是否正确
-                # print(df.head())
-                return df
-            else:
-                print(f"Table {table_index + 1}没有有效的表格数据来创建DataFrame。")
-
-
-    @staticmethod  # 抓取单个table
-    def get_the_table(url, table_index=0, dynamic=False):
-        scraper = TableScraper()
-        tables = scraper.scrape_tables(url, dynamic=dynamic)
-
-        if table_index < 0:
-            print("table_index 应为非负整数。")
-            return
-        elif not tables:
-            print("未找到任何表格（没有找到任何table标签）。两种可能：一是网站本身就没有任何table标签；二是网站的table可能是动态加载数据，可以尝试将参数调成dynamic=True。")
-            return
-
-        elif table_index >= len(tables):
-            print(f"超出了范围：序号为 {table_index}表格不存在。")
-            return
+                    # 3.如果当前行的<td>数量大于表头列数，新增列并保留超出的数据
+                else:
+                    for num in range(len(headers)):
+                        col = cols[num]
+                        if col.name == 'td':
+                            row_data.append(col.text.strip())
+                    # 新增额外的列，列名为Column+额外列数，并将超出的数据作为该列的值
+                    for extra_col in cols[len(headers):]:
+                        row_data.append(extra_col.text.strip())
+                        headers.append('Column' + str(len(headers) + 1))
+                    print(
+                        f"警告：在处理Table {table_index + 1}，第 {row_index} 行时，发现列数({col_count})超出表头列数({len(headers)})，已新增额外列处理。")
+                data.append(row_data)
+
+        # 如果data列表为空（即没有有效的数据行），则不创建DataFrame
+        if data:
+            # 创建DataFrame
+            df = pd.DataFrame(data, columns=headers)
+            # 打印DataFrame的前几行，以验证数据是否正确
+            # print(df.head())
+            return df
         else:
-            table = tables[table_index]
-            headers = scraper.extract_headers(table)
-            df = scraper.extract_table_data(table, headers, table_index)
-
-            if df is not None:
-                print(f"成功抓取 URL: {url} 中序号为 {table_index} 的表格数据：")
-                print(f"Table {table_index + 1}:")
-                return df
-            else:
-                print(f"Table {table_index + 1}:")
-                print(f"表格为空，未能提取 URL: {url} 中序号为 {table_index} 的表格数据。")
+            print(f"Table {table_index + 1}没有有效的表格数据来创建DataFrame。")
 
-    @staticmethod  # 打印全部table
-    def show_all_tables(url, dynamic=False):
-        scraper = TableScraper()
-        tables = scraper.scrape_tables(url, dynamic=dynamic)
-
-        if not tables:
-            print(
-                "未找到任何表格（没有找到任何table标签）。两种可能：一是网站本身就没有任何table标签；二是网站的table可能是动态加载数据，可以尝试将参数调成dynamic=True。")
-            return
 
+# 抓取单个table
+def get_the_table(url, table_index=0, dynamic=False):
+    # scraper = TableScraper()
+    tables = scrape_tables(url, dynamic=dynamic)
+
+    if table_index < 0:
+        print("table_index 应为非负整数。")
+        return
+    elif not tables:
+        print("未找到任何表格（没有找到任何table标签）。两种可能：一是网站本身就没有任何table标签；二是网站的table可能是动态加载数据，可以尝试将参数调成dynamic=True。")
+        return
+
+    elif table_index >= len(tables):
+        print(f"超出了范围：序号为 {table_index}表格不存在。")
+        return
+    else:
+        table = tables[table_index]
+        headers = extract_headers(table)
+        df = extract_table_data(table, headers, table_index)
+
+        if df is not None:
+            print(f"成功抓取 URL: {url} 中序号为 {table_index} 的表格数据：")
+            print(f"Table {table_index + 1}:")
+            return df
         else:
+            print(f"Table {table_index + 1}:")
+            print(f"表格为空，未能提取 URL: {url} 中序号为 {table_index} 的表格数据。")
 
-            for i, table in enumerate(tables):
-                if table.find("tbody") or table.find("thead"):
-                    try:
-                        headers = scraper.extract_headers(table)
-                        df = scraper.extract_table_data(table, headers, i)
-                        if df is not None:
-                            print(f"成功抓取 URL: {url} 中序号为 {i} 的表格数据：")
-                            print(f"Table {i + 1}:")
-                            print(df)
-                        else:
-                            print(f"Table {i + 1}:")
-                            print(f"表格为空，未能提取 URL: {url} 中序号为 {i} 的表格数据。")
-                    except Exception as e:
-                        print(f"处理Table {i + 1}时发生错误: {e}")
+# 打印全部table
+def show_all_tables(url, dynamic=False):
+    # scraper = TableScraper()
+    tables = scrape_tables(url, dynamic=dynamic)
+
+    if not tables:
+        print(
+            "未找到任何表格（没有找到任何table标签）。两种可能：一是网站本身就没有任何table标签；二是网站的table可能是动态加载数据，可以尝试将参数调成dynamic=True。")
+        return
+
+    else:
+
+        for i, table in enumerate(tables):
+            if table.find("tbody") or table.find("thead"):
+                try:
+                    headers = extract_headers(table)
+                    df = extract_table_data(table, headers, i)
+                    if df is not None:
+                        print(f"成功抓取 URL: {url} 中序号为 {i} 的表格数据：")
+                        print(f"Table {i + 1}:")
+                        print(df)
+                    else:
+                        print(f"Table {i + 1}:")
+                        print(f"表格为空，未能提取 URL: {url} 中序号为 {i} 的表格数据。")
+                except Exception as e:
+                    print(f"处理Table {i + 1}时发生错误: {e}")
 
-                else:
-                    print(table)
-                    print("<table>标签里没有<thead>和<tbody>标签，有可能是网站启用了反爬虫技术")
+            else:
+                print(table)
+                print("<table>标签里没有<thead>和<tbody>标签，有可能是网站启用了反爬虫技术")
```

### Comparing `tableshare-1.1.4/tableshare.egg-info/PKG-INFO` & `tableshare-1.1.5/tableshare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableshare
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python library for scraping and sharing table data from web pages.
 Home-page: https://github.com/baiguanba/tableshare
 Author: Guanba
 Author-email: baiguanba@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baiguanba/tableshare/issues
 Keywords: python,table,webtable,scrawler
```

