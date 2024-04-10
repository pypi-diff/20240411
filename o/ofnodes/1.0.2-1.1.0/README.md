# Comparing `tmp/ofnodes-1.0.2.tar.gz` & `tmp/ofnodes-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.0.2.tar", max compression
+gzip compressed data, was "ofnodes-1.1.0.tar", max compression
```

## Comparing `ofnodes-1.0.2.tar` & `ofnodes-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2607 2024-04-05 21:53:44.165933 ofnodes-1.0.2/README.md
--rw-r--r--   0        0        0      590 2024-04-05 21:54:06.717801 ofnodes-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.0.2/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.2/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1747 2024-04-04 17:47:49.284523 ofnodes-1.0.2/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.0.2/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.2/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    17664 2024-04-05 18:26:37.004190 ofnodes-1.0.2/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 ofnodes-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.1.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-10 22:08:04.114199 ofnodes-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.1.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.1.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1747 2024-04-04 17:47:49.284523 ofnodes-1.1.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.1.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.1.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    20925 2024-04-10 22:07:30.994364 ofnodes-1.1.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.1.0/PKG-INFO
```

### Comparing `ofnodes-1.0.2/README.md` & `ofnodes-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![Build Status](https://github.com/robert-portelli/ofnodes/actions/workflows/01_build.yml/badge.svg)
 ![Tests](https://github.com/robert-portelli/ofnodes/actions/workflows/02_test.yml/badge.svg)
 [![Documentation](https://github.com/robert-portelli/ofnodes/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/robert-portelli/ofnodes/actions/workflows/pages/pages-build-deployment)
 [![codecov](https://codecov.io/gh/robert-portelli/ofnodes/graph/badge.svg?token=2XI42KBTRQ)](https://codecov.io/gh/robert-portelli/ofnodes)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![PyPI - Version](https://img.shields.io/pypi/v/ofnodes)](https://pypi.org/project/ofnodes/)]
+[![PyPI - Version](https://img.shields.io/pypi/v/ofnodes)](https://pypi.org/project/ofnodes/)
 
 
 **ofnodes** is a Python Package providing examples of the Author's ability
 to implement data structures and algorithms in Python. It is not a substitute
 for built-in or other third-party implementations of the same data structures
 and algorithms. It aims to illustrate the author's ability to produce a
 distributable package of objects behind a thoughtful user interface.
```

### Comparing `ofnodes-1.0.2/pyproject.toml` & `ofnodes-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.0.2"
+version = "1.1.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.0.2/src/ofnodes/__init__.py` & `ofnodes-1.1.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.0.2/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.1.0/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.0.2/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.1.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,25 @@
     This class provides functionality to create and manipulate a singly linked list
     data structure. Each node in the linked list contains a reference to the next
     node in the sequence.
 
     Attributes:
         _head (Optional[SinglyNode]): The head of the linked list.
         _tail (Optional[SinglyNode]): The tail of the linked list.
+        _target (Optional[Any]): The target data or node instance.
 
     Examples:
         >>> linked_list = SinglyLinkedList()
         >>> linked_list
-        SinglyLinkedList(head=None, tail=None)
+        SinglyLinkedList(head=None, tail=None, target=None)
     """
     def __init__(self) -> None:
         self._head: Optional[SinglyNode] = None
         self._tail: Optional[SinglyNode] = None
+        self._target: Optional[Any|SinglyNode] = None
 
     @property
     def head(self) -> SinglyNode | None:
         """Getter property for the head of the linked list.
 
         Returns:
             SinglyNode | None: The head of the linked list, or None if the list is empty.
@@ -55,17 +57,14 @@
     def head(self, value: SinglyNode | Any) -> None:
         """
         Setter property for the head of the linked list.
 
         Args:
             value (SinglyNode | Any): The value to be set as the head. If the value is
                 not already a SinglyNode object, it is wrapped in a SinglyNode.
-
-        Raises:
-            AttributeError: If attempting to delete the `head` attribute.
         """
         match value:
             case SinglyNode():
                 node = value
             case _:
                 node = SinglyNode(value)
 
@@ -86,14 +85,85 @@
             AttributeError: Deleting the `head` attribute is not allowed.
         """
         raise AttributeError(
             f"{type(self).__name__}'s `head` attribute " "cannot be deleted."
         )
 
     @property
+    def target(self) -> SinglyNode|Any:
+        """Getter property for the node data to target in a Linked List.
+
+        Returns:
+            target: The first node instance of the linked list containing data\
+            matching the target. If no target match, the data is assigned as passed\
+            to target.
+
+        Notes:
+            Any data can be assigned as the target data. Each node in the
+            `SinglyLinkedList` has its data compared to the target data. The first
+            node instance data that match the target data is assigned to the `.target`
+            property. If a match is not found, the target data is stored as is in the
+            `.target` attribute.
+
+        Examples:
+            >>> sllist = SinglyLinkedList()
+            >>> sllist.__dict__
+            {'_head': None, '_tail': None, '_target': None}
+            >>> sllist.target = '5 node'
+            Empty `SinglyLinkedList()`. Target data is assigned to SinglyLinkedList's target property.
+            >>> type(sllist.target) != SinglyNode
+            True
+            >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
+            [None, None, None, None]
+            >>> sllist.target = '5 node'
+            No target matches. Target data assigned to SinglyLinkedList's target property.
+            >>> sllist.tail = '5 node'
+            >>> sllist.target = '5 node'
+            At least one target match. First target node instance is assigned to SinglyLinkedList's target property.
+            >>> type(sllist.target) == SinglyNode
+            True
+            >>> sllist.target is sllist.tail
+            True
+        """
+        return self._target
+
+    @target.setter
+    def target(self, target_data: Any | SinglyNode) -> None:
+        """Setter property for the target node data of the linked list.
+
+        Args:
+            target (Any): The data for which to match to node data.
+        """
+
+        match target_data:
+            case _:
+                #  TODO: data validation
+                validated_data = target_data
+
+        match self._head:
+            case None:
+                print(f"Empty `SinglyLinkedList()`. Target data is assigned to {type(self).__name__}'s target property.")
+                self._target = validated_data
+
+            case self._head:
+                current_node = self._head
+                while current_node:
+                    if current_node.data == validated_data:
+                        print(f"""At least one target match. First target node instance is assigned to {type(self).__name__}'s target property.""")
+                        setattr(self, '_target', current_node)
+                        return
+                    current_node = current_node.next
+                print(f"""No target matches. Target data assigned to {type(self).__name__}'s target property.""")
+                setattr(self, '_target', validated_data)
+                return
+
+
+
+
+    @property
     def tail(self) -> SinglyNode | None:
         """
         Getter property for the tail of the linked list.
 
         Returns:
             SinglyNode | None: The tail of the linked list, or None if the list is empty.
 
@@ -265,19 +335,20 @@
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
-    def search(self, target) -> bool:
-        """Searches for a target value in the linked list.
+    def search(self, target_data) -> bool:
+        """Searches each node's data in a linked list until the first occurrence of
+        the target is found.
 
         Args:
-            target (Any): The value to search for in the linked list.
+            target_data (Any): The value to search for in the linked list.
 
         Returns:
             bool: True if the target value is found in the linked list, False otherwise.
 
         Raises:
             ValueError: If the linked list is empty.
 
@@ -295,22 +366,26 @@
             False
             >>> llist.search("third node")
             False
             >>> llist.tail = "third node"
             >>> llist.search("third node")
             True
         """
-        if self._head:
-            current_node = self._head
-            while current_node:
-                if current_node.data == target:
-                    return True
-                current_node = current_node.next
-            return False
-        raise ValueError("Cannot perform search: The list is empty.")
+        if target_data:
+            #  TODO: data validation
+            validated_data = target_data
+            if self._head:
+                current_node = self._head
+                while current_node:
+                    if current_node.data == validated_data:
+                        return True
+                    current_node = current_node.next
+                return False
+            raise ValueError("Cannot perform search: The list is empty.")
+        raise ValueError("This data is unable to be target.")
 
     def remove_head(self) -> None:
         """Removes the head node from the linked list.
 
         Raises:
             ValueError: If the linked list is empty.
 
@@ -339,15 +414,15 @@
             SinglyLinkedList(head=None, tail=None)
         """
         if self._head and self._head is self._tail:
             self._head = None
             self._tail = None
             return
         if self._head and self._head is not self._tail:
-            self._head = self.head.next
+            self._head = self._head.next
             return
         raise ValueError("Cannot remove head from empty list")
 
     def remove_tail(self) -> None:
         """Removes the tail node from the linked list.
 
         Raises:
```

### Comparing `ofnodes-1.0.2/PKG-INFO` & `ofnodes-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.0.2
+Version: 1.1.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -17,15 +17,15 @@
 ![Build Status](https://github.com/robert-portelli/ofnodes/actions/workflows/01_build.yml/badge.svg)
 ![Tests](https://github.com/robert-portelli/ofnodes/actions/workflows/02_test.yml/badge.svg)
 [![Documentation](https://github.com/robert-portelli/ofnodes/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/robert-portelli/ofnodes/actions/workflows/pages/pages-build-deployment)
 [![codecov](https://codecov.io/gh/robert-portelli/ofnodes/graph/badge.svg?token=2XI42KBTRQ)](https://codecov.io/gh/robert-portelli/ofnodes)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![PyPI - Version](https://img.shields.io/pypi/v/ofnodes)](https://pypi.org/project/ofnodes/)]
+[![PyPI - Version](https://img.shields.io/pypi/v/ofnodes)](https://pypi.org/project/ofnodes/)
 
 
 **ofnodes** is a Python Package providing examples of the Author's ability
 to implement data structures and algorithms in Python. It is not a substitute
 for built-in or other third-party implementations of the same data structures
 and algorithms. It aims to illustrate the author's ability to produce a
 distributable package of objects behind a thoughtful user interface.
```

