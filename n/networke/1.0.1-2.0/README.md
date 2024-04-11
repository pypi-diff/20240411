# Comparing `tmp/networke-1.0.1.tar.gz` & `tmp/networke-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networke-1.0.1.tar", last modified: Tue Apr  9 16:16:25 2024, max compression
+gzip compressed data, was "networke-2.0.tar", last modified: Thu Apr 11 16:48:07 2024, max compression
```

## Comparing `networke-1.0.1.tar` & `networke-2.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:16:25.222906 networke-1.0.1/
--rw-rw-rw-   0        0        0        0 2024-04-09 15:52:45.000000 networke-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       82 2024-04-09 16:16:25.218126 networke-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        3 2024-04-09 15:52:26.000000 networke-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:16:25.066025 networke-1.0.1/networke.egg-info/
--rw-rw-rw-   0        0        0       82 2024-04-09 16:16:24.000000 networke-1.0.1/networke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2024-04-09 16:16:24.000000 networke-1.0.1/networke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:16:24.000000 networke-1.0.1/networke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 16:16:24.000000 networke-1.0.1/networke.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 16:16:25.211682 networke-1.0.1/networkk/
--rw-rw-rw-   0        0        0       28 2024-04-09 15:55:03.000000 networke-1.0.1/networkk/__init__.py
--rw-rw-rw-   0        0        0     6873 2024-03-10 04:18:36.000000 networke-1.0.1/networkk/doublelinky.py
--rw-rw-rw-   0        0        0     4619 2024-02-23 14:09:39.000000 networke-1.0.1/networkk/linked_list.py
--rw-rw-rw-   0        0        0       82 2024-04-09 15:54:50.000000 networke-1.0.1/networkk/main.py
--rw-rw-rw-   0        0        0      232 2024-04-09 09:55:10.000000 networke-1.0.1/networkk/progarm_factorial.py
--rw-rw-rw-   0        0        0      254 2024-04-07 07:46:58.000000 networke-1.0.1/networkk/program_5_fibonacci.py
--rw-rw-rw-   0        0        0     2919 2024-04-09 10:58:58.000000 networke-1.0.1/networkk/program_array.py
--rw-rw-rw-   0        0        0      222 2024-04-09 09:42:53.000000 networke-1.0.1/networkk/program_asc_Desc.py
--rw-rw-rw-   0        0        0     2173 2024-04-09 12:33:55.000000 networke-1.0.1/networkk/program_dfs.py
--rw-rw-rw-   0        0        0     3463 2024-04-09 13:52:44.000000 networke-1.0.1/networkk/program_heap.py
--rw-rw-rw-   0        0        0     2205 2024-04-09 13:23:53.000000 networke-1.0.1/networkk/program_prims.py
--rw-rw-rw-   0        0        0     1056 2024-04-09 11:30:12.000000 networke-1.0.1/networkk/program_quicksort.py
--rw-rw-rw-   0        0        0     2320 2024-04-09 14:47:36.000000 networke-1.0.1/networkk/program_stack_expr.py
--rw-rw-rw-   0        0        0       42 2024-04-09 16:16:25.226062 networke-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      199 2024-04-09 16:15:26.000000 networke-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:07.499426 networke-2.0/
+-rw-rw-rw-   0        0        0        0 2024-04-09 15:52:45.000000 networke-2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       80 2024-04-11 16:48:07.499426 networke-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2024-04-09 15:52:26.000000 networke-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:07.421306 networke-2.0/network/
+-rw-rw-rw-   0        0        0       28 2024-04-09 15:55:03.000000 networke-2.0/network/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-11 15:30:17.000000 networke-2.0/network/bst.py
+-rw-rw-rw-   0        0        0      197 2024-04-11 13:17:01.000000 networke-2.0/network/comp_sum.py
+-rw-rw-rw-   0        0        0      248 2024-04-11 13:23:15.000000 networke-2.0/network/hanoi.py
+-rw-rw-rw-   0        0        0     3028 2024-04-11 16:21:42.000000 networke-2.0/network/krus.py
+-rw-rw-rw-   0        0        0       82 2024-04-09 15:54:50.000000 networke-2.0/network/main.py
+-rw-rw-rw-   0        0        0      971 2024-04-11 13:41:30.000000 networke-2.0/network/merge_sort.py
+-rw-rw-rw-   0        0        0     5710 2024-04-11 16:32:14.000000 networke-2.0/network/poley.py
+-rw-rw-rw-   0        0        0      236 2024-04-11 13:19:31.000000 networke-2.0/network/pow.py
+-rw-rw-rw-   0        0        0     2805 2024-04-11 14:23:00.000000 networke-2.0/network/qu.py
+-rw-rw-rw-   0        0        0      418 2024-04-11 13:29:15.000000 networke-2.0/network/seat.py
+-rw-rw-rw-   0        0        0     1516 2024-04-11 13:55:51.000000 networke-2.0/network/stackey.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:07.499426 networke-2.0/networke.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-04-11 16:48:06.000000 networke-2.0/networke.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-04-11 16:48:07.000000 networke-2.0/networke.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 16:48:06.000000 networke-2.0/networke.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 16:48:06.000000 networke-2.0/networke.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 16:48:07.515049 networke-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      197 2024-04-11 16:47:47.000000 networke-2.0/setup.py
```

### Comparing `networke-1.0.1/networkk/program_dfs.py` & `networke-2.0/network/stackey.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,54 @@
-class Node:
-    def __init__(self,value):
-        self.value = value
-        self.left = None
-        self.right = None
-class Tree:
+class Stack():
     def __init__(self):
-        self.root = None
-
-    def insert(self,value):
-        if not self.root:
-            self.root = Node(value)
-            print(f"Root node inserted {value}")
-            return
-        queue = [self.root]
-        while queue:
-            current  = queue.pop(0)
-            if not current.left:
-                current.left = Node(value)
-                print(f"Node {value} inserted as Child node of {current.value} (left)")
-                break
-            elif not current.right:
-                current.right = Node(value)
-                print(f"Node {value} inserted as Child node of {current.value} (right)")
-                break
-            else:
-                queue.append(current.left)
-                queue.append(current.right)
-    def inorder(self,node):
-        if node:
-            self.inorder(node.left)
-            print(node.value,end = "")
-            self.inorder(node.right)
-    def preorder(self,node):
-        if node:
-            print(node.value,end = "")
-            self.preorder(node.left)
-            self.preorder(node.right)
-    def postorder(self,node):
-        if node:
-            self.postorder(node.left)
-            self.postorder(node.right)
-            print(node.value,end = "")
+        self.item = []
+    def empty(self):
+        return len(self.item) == 0
+    def push(self,item):
+        self.item.append(item)
+    def pop(self):
+        if not self.empty():
+            return self.item.pop()
+        else:
+            print("Cannot Pop from empty Stack")
+    def peek(self):
+        if not self.empty():
+            return self.item[-1]
+        else:
+            print("Cannot Peek in empty stack")
+    def display(self):
+        print("Stack:",self.item)
 def main():
-    tree = Tree()
-    print("DFS TRAVERSAL")
-    print("\n1. Insert elements")
-    print("2. Inorder Traversal")
-    print("3. Preorder Traversal")
-    print("4. PostOrder Traversal")
+    s = Stack()
+    print("\n Menu")
+    print("1. Push")
+    print("2. Pop")
+    print("3. Peek")
+    print("4. Display")
     print("5. Exit")
     while True:
-        choice = int(input("Enter your choice:"))
+        choice = int(input("Enter the choice:"))
         if choice == 1:
-            value = input("Enter the value to insert")
-            tree.insert(value)
+            item = int(input("Enter the item to push:"))
+            s.push(item)
+            s.display()
         elif choice == 2:
-            tree.inorder(tree.root)
-
+            pop_i = s.pop()
+            if pop_i is not None:
+                print("Popped Item:",pop_i)
+                s.display()
+            else:
+                print("Stack is Empty")
         elif choice == 3:
-            tree.preorder(tree.root)
-        elif choice == 4:
-            tree.postorder(tree.root)
+            pp = s.peek()
+            if pp is not None:
+                print("Peek Element:",pp)
+            else:
+                print("Not peek an empty stack")
+        elif choice ==4:
+            s.display()
         elif choice == 5:
             break
         else:
-            print("Invalid Choice")
-if __name__ == "__main__":
+            print("Invalid choice")
+if __name__== "__main__":
     main()
-
```

### Comparing `networke-1.0.1/networkk/program_heap.py` & `networke-2.0/network/qu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,95 @@
-import heapq
-from binarytree import build
-
-class PriorityQueue:
+class Queue:
     def __init__(self):
-        self.min_heap = []
-        self.max_heap = []
-    def insert(self,value):
-        heapq.heappush(self.min_heap,value)
-        heapq.heappush(self.max_heap,-value)
-    def dequeue_min(self):
-        if not self.isempty():
-            min_val = heapq.heappop(self.min_heap)
-            self.max_heap.remove(-min_val)
-            heapq.heapify(self.max_heap)
-            return min_val
-    def dequeue_max(self):
-        if not self.isempty():
-            max_val = -heapq.heappop(self.max_heap)
-            self.min_heap.remove(max_val)
-            heapq.heapify(self.min_heap)
-            return max_val
-    def peek_min(self):
-        if not self.isempty():
-            return self.min_heap[0]
-    def peek_max(self):
-        if not self.isempty():
-            return -self.max_heap[0]
-    def display_min(self):
-        if not self.isempty():
-            tree = build(self.min_heap)
-            print("Min Heap Tree")
-            print(tree)
-        else:
-            print("Min heap tree is empty")
-    def display_max(self):
-        if not self.isempty():
-            tree = build([-val for val in self.max_heap])
-            print("Max Heap Tree")
-            print(tree)
-        else:
-            print("Max heap tree is empty")
-    def isempty(self):
-        return len(self.min_heap) == 0
-    def size_min(self):
-        return len(self.min_heap)
-    def size_max(self):
-        return len(self.max_heap)
-def main():
-    pq = PriorityQueue()
-    print("Priority Queue using Heap")
-    print("\n1. Enqueue the element")
-    print("2. Dequeue from Min heap")
-    print("3. Dequeue from Max heap")
-    print("4. Peek the min heap and max heap")
-    print("5. Display the Min heap")
-    print("6. Display the Max heap")
-    print("7. Check if empty")
-    print("8. Size of Min heap")
-    print("9. Size of Max heap")
-    print("10. Exit")
+        self.items =[]
+    def is_empty(self):
+        return len(self.items) == 0
+    def enqueue(self,item):
+        if len(self.items) == size:
+            print("Queue is Full")
+        else:
+            self.items.append(item)
+            print("Item",item,"enqueued to Queue")
+    def is_full(self):
+        if len(self.items) == size:
+            print("Queue is full")
+        else:
+            print("Queue is not full")
+    def dequeue(self):
+        if not self.is_empty():
+            return self.items.pop(0)
+        else:
+            print("Queue is empty")
+            return None
+    def front(self):
+        if not self.is_empty():
+            return self.items[0]
+        else:
+            print("Queue is empty")
+            return None
+    def rear(self):
+        if not self.is_empty():
+            return self.items[-1]
+        else:
+            print("Queue is empty")
+            return None
+    def size(self):
+        return len(self.items)
+    def display(self):
+        if not self.is_empty():
+            print("Queue :",self.items)
+        else:
+            print("Queue is empty")
 
+print("\n\t Basic operations of Queue")
+print("\t********************************\n")
+size = int(input("Enter the size of Queue:"))
+def main():
+    q = Queue()
     while True:
+        print("\n1. Enqueue")
+        print("2. Dequeue")
+        print("3. Front")
+        print("4. Rear")
+        print("5. IsEmpty")
+        print("6. IsNull")
+        print("7. Size")
+        print("8. Display")
+        print("9. Exit\n")
         choice = int(input("Enter your choice:"))
         if choice == 1:
-            value = int(input("Enter the element to enqueue"))
-            pq.insert(value)
-            print(f"Enqueue element {value}")
+            item = input("Enter the item to Enqueue:")
+            q.enqueue(item)
         elif choice == 2:
-            min_val = pq.dequeue_min()
-            if min_val is not None:
-                print(f"Dequeued Element:",min_val)
-            else:
-                print("Min heap is empty")
+            item = q.dequeue()
+            if item is not None:
+                print("Dequeue Item:",item)
         elif choice == 3:
-            max_val = pq.dequeue_max()
-            if max_val is not None:
-                print(f"Dequeued Element:",max_val)
-            else:
-                print("Min heap is empty")
+            item = q.front()
+            if item is not None:
+                print("Front element of Queue:",item)
         elif choice == 4:
-            min_val = pq.peek_min()
-            max_val = pq.peek_max()
-            print("The Min heap  Front element:",min_val)
-            print("The Max heap  Front element:",max_val)
+            item = q.rear()
+            if item is not None:
+                print("Last Element of Queue:",item)
         elif choice == 5:
-            pq.display_min()
+            if q.is_empty():
+                print("Queue is Empty")
+            else:
+                print("Queue is Not Empty")
         elif choice == 6:
-            pq.display_max()
+            if q.is_full():
+                print("Queue is Full")
         elif choice == 7:
-            if pq.isempty():
-                print("Queue is empty")
-            else:
-                print("Queue is not empty")
+            print("Size of Queue:",q.size())
         elif choice == 8:
-            print("Size of Min heap:",pq.size_min())
+            q.display()
         elif choice == 9:
-            print("Size of Max heap:",pq.size_max())
-        elif choice == 10:
+            print("Exiting the program")
             break
+        else:
+            print("Invalid Choice")
+
 if __name__ == "__main__":
     main()
             
-            
         
-
```

