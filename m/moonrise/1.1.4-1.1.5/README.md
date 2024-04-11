# Comparing `tmp/moonrise-1.1.4.tar.gz` & `tmp/moonrise-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonrise-1.1.4.tar", last modified: Sun Oct 22 02:40:51 2023, max compression
+gzip compressed data, was "moonrise-1.1.5.tar", last modified: Thu Apr 11 16:33:27 2024, max compression
```

## Comparing `moonrise-1.1.4.tar` & `moonrise-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-10-22 02:40:51.123969 moonrise-1.1.4/
--rw-rw-rw-   0        0        0     1103 2023-06-07 21:03:48.000000 moonrise-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     6705 2023-10-22 02:40:51.123969 moonrise-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6055 2023-10-22 02:37:57.000000 moonrise-1.1.4/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 21:03:48.000000 moonrise-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      846 2023-10-22 02:40:51.126967 moonrise-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-22 02:40:51.049967 moonrise-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-10-22 02:40:51.070967 moonrise-1.1.4/src/moonrise/
--rw-rw-rw-   0        0        0     6923 2023-08-01 22:16:30.000000 moonrise-1.1.4/src/moonrise/Base_Test.py
--rw-rw-rw-   0        0        0     6873 2023-10-22 02:26:59.000000 moonrise-1.1.4/src/moonrise/Moon_Browser.py
--rw-rw-rw-   0        0        0     9905 2023-09-09 00:19:03.000000 moonrise-1.1.4/src/moonrise/Moon_Methods.py
--rw-rw-rw-   0        0        0     2126 2023-06-07 21:03:48.000000 moonrise-1.1.4/src/moonrise/Moon_Movie.py
--rw-rw-rw-   0        0        0     1876 2023-06-13 16:19:06.000000 moonrise-1.1.4/src/moonrise/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-08-01 22:16:30.000000 moonrise-1.1.4/src/moonrise/__main__.py
-drwxrwxrwx   0        0        0        0 2023-10-22 02:40:51.109967 moonrise-1.1.4/src/moonrise.egg-info/
--rw-rw-rw-   0        0        0     6705 2023-10-22 02:40:51.000000 moonrise-1.1.4/src/moonrise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-10-22 02:40:51.000000 moonrise-1.1.4/src/moonrise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-22 02:40:51.000000 moonrise-1.1.4/src/moonrise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-10-22 02:40:51.000000 moonrise-1.1.4/src/moonrise.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-10-22 02:40:51.000000 moonrise-1.1.4/src/moonrise.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-22 02:40:51.000000 moonrise-1.1.4/src/moonrise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 16:33:27.083556 moonrise-1.1.5/
+-rw-rw-rw-   0        0        0     1103 2023-06-07 21:03:48.000000 moonrise-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6705 2024-04-11 16:33:27.082559 moonrise-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6055 2023-12-21 18:24:37.000000 moonrise-1.1.5/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 21:03:48.000000 moonrise-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      846 2024-04-11 16:33:27.086556 moonrise-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 16:33:27.009555 moonrise-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 16:33:27.033558 moonrise-1.1.5/src/moonrise/
+-rw-rw-rw-   0        0        0     6923 2024-04-10 18:44:30.000000 moonrise-1.1.5/src/moonrise/Base_Test.py
+-rw-rw-rw-   0        0        0     6873 2024-04-10 18:44:30.000000 moonrise-1.1.5/src/moonrise/Moon_Browser.py
+-rw-rw-rw-   0        0        0    12474 2024-04-11 16:23:06.000000 moonrise-1.1.5/src/moonrise/Moon_Methods.py
+-rw-rw-rw-   0        0        0     2126 2023-06-07 21:03:48.000000 moonrise-1.1.5/src/moonrise/Moon_Movie.py
+-rw-rw-rw-   0        0        0     1876 2024-04-10 18:44:30.000000 moonrise-1.1.5/src/moonrise/__init__.py
+-rw-rw-rw-   0        0        0     2363 2024-01-03 02:22:00.000000 moonrise-1.1.5/src/moonrise/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:33:27.077555 moonrise-1.1.5/src/moonrise.egg-info/
+-rw-rw-rw-   0        0        0     6705 2024-04-11 16:33:26.000000 moonrise-1.1.5/src/moonrise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-04-11 16:33:27.000000 moonrise-1.1.5/src/moonrise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 16:33:26.000000 moonrise-1.1.5/src/moonrise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-11 16:33:26.000000 moonrise-1.1.5/src/moonrise.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-04-11 16:33:26.000000 moonrise-1.1.5/src/moonrise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 16:33:26.000000 moonrise-1.1.5/src/moonrise.egg-info/top_level.txt
```

### Comparing `moonrise-1.1.4/LICENSE` & `moonrise-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/PKG-INFO` & `moonrise-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.1.4
+Version: 1.1.5
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `moonrise-1.1.4/README.md` & `moonrise-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/setup.cfg` & `moonrise-1.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6f 6e72 6973 650d 0a76 6572   = moonrise..ver
-00000020: 7369 6f6e 203d 2031 2e31 2e34 0d0a 6175  sion = 1.1.4..au
+00000020: 7369 6f6e 203d 2031 2e31 2e35 0d0a 6175  sion = 1.1.5..au
 00000030: 7468 6f72 203d 2043 6872 6973 746f 7068  thor = Christoph
 00000040: 6572 2044 6961 6d6f 6e64 2d4a 6f6e 6573  er Diamond-Jones
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2063 6872 6973 746f 7068 6572 2e6a 6f6e   christopher.jon
 00000070: 6573 3131 3338 4067 6d61 696c 2e63 6f6d  es1138@gmail.com
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5465 7374 2073 7569 7465 2063 7265 6174  Test suite creat
```

### Comparing `moonrise-1.1.4/src/moonrise/Base_Test.py` & `moonrise-1.1.5/src/moonrise/Base_Test.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/src/moonrise/Moon_Browser.py` & `moonrise-1.1.5/src/moonrise/Moon_Browser.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/src/moonrise/Moon_Methods.py` & `moonrise-1.1.5/src/moonrise/Moon_Methods.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import Select
 from selenium.common.exceptions import TimeoutException
+from typing import Union
 
 class MoonMethods:
     """Common-use methods when locating and interacting with web elements
     """
 
-    def get_web_element(self, locator, timeout=None, get_multiples = False):
+    def get_web_element(self, locator: Union[str, WebElement], timeout: int = None, get_multiples: bool = False):
         """Locate a web element or elements via a given ``locator``.
            Throws a TimeoutException if the element(s) cannot be found within ``timeout`` or default_timeout
 
            Can perform a search in 3 main ways:
            - XPATH default: using the prefix '//' will automatically use XPATH to perform the search
            - CSS default: simply inputting an element locator will try to locate the element via CSS selector
            - By methods: specifying the lookup type will use the desired lookup method if it is available. Available methods include:
@@ -70,118 +71,163 @@
             elements = []
             for e in results:
                 elements.append(MoonElement(e))
             return elements
         else:
             return MoonElement(results)
 
-    def click_element(self, locator, timeout=None):
+    def click_element(self, locator: Union[str, WebElement], timeout: int = None):
         """Click the element identified by ``locator``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         self.get_web_element(locator=locator, timeout=timeout).click()
 
 
-    def input_text(self, locator, text, timeout=None):
+    def input_text(self, locator: Union[str, WebElement], text: str, timeout: int = None):
         """Types the given ``text`` into the text field identified by ``locator``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         self.get_web_element(locator=locator, timeout=timeout).send_keys(text)
 
-    def get_web_elements(self, locator, timeout=None):
+    def get_web_elements(self, locator: Union[str, WebElement], timeout: int = None):
         """Returns a list of WebElement objects matching the ``locator``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         return self.get_web_element(locator=locator, timeout=timeout, get_multiples=True)
 
-    def select_from_list_by_value(self, locator, value, timeout=None):
+    def select_from_list_by_value(self, locator: Union[str, WebElement], value: str, timeout: int = None):
         """Select option from selection list ``locator`` by ``value``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``value``: The value to select from the list.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         Select(self.get_web_element(locator=locator, timeout=timeout)).select_by_value(value)
         
-    def select_from_list_by_label(self, locator, label, timeout=None):
+    def select_from_list_by_label(self, locator: Union[str, WebElement], label: str, timeout: int = None):
         """Select option from selection list ``locator`` by ``label``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``label``: The label to select from the list.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         Select(self.get_web_element(locator=locator, timeout=timeout)).select_by_visible_text(label)
 
-    def select_from_list_by_index(self, locator, index, timeout=None):
+    def select_from_list_by_index(self, locator: Union[str, WebElement], index: int, timeout: int = None):
         """Select option from selection list ``locator`` by ``index``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``index``: The index to select from the list.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         Select(self.get_web_element(locator=locator, timeout=timeout)).select_by_index(index) 
 
-    def get_text(self, locator, timeout=None):
+    def get_text(self, locator: Union[str, WebElement], timeout: int = None) -> str:
         """Returns the text value of the element identified by ``locator``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
         return self.get_web_element(locator=locator, timeout=timeout).text
     
-    def drag_element_to_element(self, dragged_locator: str, target_locator: str, timeout: int = None):
+    def drag_element_to_element(self, dragged_locator: Union[str, WebElement], target_locator: Union[str, WebElement], timeout: int = None):
         """Clicks and drags one element to another element.
 
            Arguments:
            - ``dragged_locator`` (str): Locator for the element to be clicked and dragged.
            - ``target_locator`` (str): Locator for the element that the dragged element will be dragged to.
            - ``timeout`` (int, optional): Maximum time (in seconds) to search for both the dragged and target elements before throwing a TimeoutException.
         """
         dragged_element = self.get_web_element(locator=dragged_locator, timeout=timeout)
         target_element = self.get_web_element(locator=target_locator, timeout=timeout)
 
         ActionChains(self.moon_driver).drag_and_drop(dragged_element, target_element).perform()
 
-    def drag_element_to_offset(self, dragged_locator: str, x_offset: int, y_offset: int, timeout: int = None):
+    def drag_element_to_offset(self, dragged_locator: Union[str, WebElement], x_offset: int, y_offset: int, timeout: int = None):
         """Clicks and drags one element to another element.
 
            Arguments:
            - ``dragged_locator`` (str): Locator for the element to be clicked and dragged.
            - ``x_offset`` (int): The number of pixels to drag the element along the x axis.
            - ``y_offset`` (int): The number of pixels to drag the element along the y axis.
            - ``timeout`` (int, optional): Maximum time (in seconds) to search for the dragged element before throwing a TimeoutException.
         """
         dragged_element = self.get_web_element(locator=dragged_locator, timeout=timeout)
 
         ActionChains(self.moon_driver).drag_and_drop_by_offset(dragged_element, xoffset=x_offset, yoffset=y_offset).perform()
 
-    def scroll_to_element(self, locator: str, timeout: int = None):
+    def scroll_to_element(self, locator: Union[str, WebElement], timeout: int = None):
         """Scrolls an element into view.
 
            Arguments:
            - ``locator`` (str): Locator for the element to be scrolled into view.
            - ``timeout`` (int, optional): Maximum time (in seconds) to search for the element before throwing a TimeoutException.
         """
         element = self.get_web_element(locator=locator, timeout=timeout)
 
         self.moon_driver.execute_script("arguments[0].scrollIntoView();", element)
 
+    def element_present(self, locator: Union[str, WebElement], timeout: int = None):
+        """Searches for an element specified by ``locator``.
+           Returns ``True`` if the element is present and ``False`` if the element is not present.
+
+           Arguments:
+           - ``locator`` (str or WebElement): Locator for the element to be checked for being present.
+           - ``timeout`` (int, optional): Maximum time (in seconds) to search for the element.
+        """
+        try:
+            self.get_web_element(locator=locator, timeout=timeout)
+            return True
+        except TimeoutException:
+            return False
+        
+    def any_elements_present(self, locators: list, timeout: int = None):
+        """Searches for a ``list`` of elements.
+           Returns ``True`` if ANY of the specified elements are present and ``False`` if NONE of the elements are present.
+
+           Arguments:
+           - ``locators`` (list of strings or WebElements): List of element locators for the elements to be searched for being present.
+           - ``timeout`` (int, optional): Maximum time (in seconds) to search for the specified elements.
+        """
+        for locator in locators:
+            try:
+                self.get_web_element(locator=locator, timeout=timeout)
+                return True
+            except TimeoutException:
+                continue
+        return False
+    
+    def all_elements_present(self, locators: list, timeout: int = None):
+        """Searches for a ``list`` of elements.
+           Returns ``True`` if ALL of the specified elements are present and ``False`` if ANY of the elements are not present.
+
+           Arguments:
+           - ``locators`` (list of strings or WebElements): List of element locators for the elements to be searched for being present.
+           - ``timeout`` (int, optional): Maximum time (in seconds) to search for the specified elements.
+        """
+        for locator in locators:
+            try:
+                self.get_web_element(locator=locator, timeout=timeout)
+            except TimeoutException:
+                return False
+        return True
+
 class MoonElement(WebElement):
     """Replacement object for standard WebElements.
        Inherits all attributes and methods of Selenium WebElements with additional methods. 
     """
 
     def __init__(self, element: WebElement):
         self.element = element
```

### Comparing `moonrise-1.1.4/src/moonrise/Moon_Movie.py` & `moonrise-1.1.5/src/moonrise/Moon_Movie.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/src/moonrise/__init__.py` & `moonrise-1.1.5/src/moonrise/__init__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/src/moonrise/__main__.py` & `moonrise-1.1.5/src/moonrise/__main__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.4/src/moonrise.egg-info/PKG-INFO` & `moonrise-1.1.5/src/moonrise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.1.4
+Version: 1.1.5
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

