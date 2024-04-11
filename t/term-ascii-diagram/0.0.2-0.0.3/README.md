# Comparing `tmp/term_ascii_diagram-0.0.2.tar.gz` & `tmp/term_ascii_diagram-0.0.3.tar.gz`

## Comparing `term_ascii_diagram-0.0.2.tar` & `term_ascii_diagram-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/test
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/core.py
--rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/diagram.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/main.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/status_bar.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/LICENSE
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/src/term_ascii_diagram/__init__.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/src/term_ascii_diagram/core.py
+-rw-r--r--   0        0        0    22268 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/src/term_ascii_diagram/diagram.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/src/term_ascii_diagram/main.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/src/term_ascii_diagram/status_bar.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/LICENSE
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.3/PKG-INFO
```

### Comparing `term_ascii_diagram-0.0.2/src/term_ascii_diagram/core.py` & `term_ascii_diagram-0.0.3/src/term_ascii_diagram/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import curses
 from dataclasses import dataclass
 from enum import Enum
-from typing import Tuple, overload
+from typing import Optional, Tuple, overload
 
 
 @dataclass
 class Size:
     w: int
     h: int
 
@@ -27,19 +27,20 @@
 
     @overload
     def __sub__(self, other: "Point") -> Size: ...
     @overload
     def __sub__(self, other: Size) -> "Point": ...
 
     def __sub__(self, other):
-        match other:
-            case Point(x, y):
-                return Size(x - self.x, y - self.y)
-            case Size(w, h):
-                return Point(self.x - w, self.y - h)
+        if isinstance(other, Point):
+            return Size(other.x - self.x, other.y - self.y)
+        elif isinstance(other, Size):
+            return Point(self.x - other.w, self.y - other.h)
+        else:
+            ValueError(f"Type {type(other).__name__} is not supported.")
 
     def set(self, other: "Point") -> None:
         self.x = other.x
         self.y = other.y
 
     def is_within(self, top_left: "Point", bottom_right: "Point") -> bool:
         return (
@@ -86,15 +87,15 @@
     def read_keyboard_ch(self) -> int:
         return self.stdscr.getch()
 
     def put_ch(
         self,
         point: Point,
         ch: str,
-        color_pair: int | None = None,
+        color_pair: Optional[int] = None,
     ) -> None:
         """Puts the given character in the given coordinates."""
         try:
             if color_pair is not None:
                 self.stdscr.attrset(color_pair)
             self.stdscr.addch(point.y, point.x, ch)
             if color_pair is not None:
```

### Comparing `term_ascii_diagram-0.0.2/src/term_ascii_diagram/diagram.py` & `term_ascii_diagram-0.0.3/src/term_ascii_diagram/diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import curses
 import json
 import math
 import os
 from curses.textpad import Textbox
 from dataclasses import asdict
 from enum import IntEnum
-from typing import Any, Callable, Dict, Iterable, List, Tuple, cast
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, cast
 
 from term_ascii_diagram.core import Ascii, Canvas, CursorMode, Point, Size
 from term_ascii_diagram.status_bar import StatusBar
 
 
 class DiagramObject:
     position: Point
     size: Size
 
     def __init__(
         self,
-        position: Point | None = None,
-        size: Size | None = None,
+        position: Optional[Point] = None,
+        size: Optional[Size] = None,
     ):
         self.position = position or Point(0, 0)
         self.size = size or Size(6, 3)
 
     @property
     def normalized_position(self):
         x = self.position.x
@@ -96,16 +96,16 @@
 
 class Box(DiagramObject):
     text: str
     show_border: bool
 
     def __init__(
         self,
-        position: Point | None = None,
-        size: Size | None = None,
+        position: Optional[Point] = None,
+        size: Optional[Size] = None,
         text: str = "",
         show_border: bool = True,
     ):
         super().__init__(position, size)
         self.text = text
         self.show_border = show_border
 
@@ -202,18 +202,18 @@
     }
 
     orientation: Orientation
     is_arrow: bool
 
     def __init__(
         self,
-        position: Point | None = None,
+        position: Optional[Point] = None,
         is_arrow: bool = False,
-        size: Size | None = None,
-        orientation: Orientation | None = Orientation.HORIZONTAL,
+        size: Optional[Size] = None,
+        orientation: Optional[Orientation] = Orientation.HORIZONTAL,
     ):
         super().__init__(position, size)
         self.orientation = orientation or Line.Orientation.HORIZONTAL
         self.is_arrow = is_arrow
 
     def toggle(self):
         """Toggle the line starting orientation."""
@@ -292,19 +292,18 @@
             if self.top_left.y != self.bottom_right.y:
                 canvas.put_ch(
                     self.bottom_left,
                     self._get_corner_ch(self.top_left, self.bottom_right),
                 )
 
     def draw(self, canvas: Canvas) -> None:
-        match self.orientation:
-            case Line.Orientation.HORIZONTAL:
-                self._draw_horizontal(canvas)
-            case Line.Orientation.VERTICAL:
-                self._draw_vertical(canvas)
+        if self.orientation == Line.Orientation.HORIZONTAL:
+            self._draw_horizontal(canvas)
+        else:
+            self._draw_vertical(canvas)
 
     def serialize(self) -> Dict[str, Any]:
         data = super().serialize()
         data.update({"orientation": self.orientation})
         data.update({"is_arrow": self.is_arrow})
         return data
 
@@ -314,15 +313,15 @@
         self.is_arrow = data["is_arrow"]
 
 
 class Designer:
     canvas: Canvas
     stdscr: curses.window
     status_bar: StatusBar
-    objects: list[DiagramObject]
+    objects: List[DiagramObject]
     selected_object_index: int
     cursor: Point
     cursor_mode: CursorMode
     key_bindings: Dict[int, Callable]
     sticky_mode: bool
 
     def __init__(
@@ -526,24 +525,24 @@
     def _toggle_object(self) -> None:
         if hasattr(self.selected_object, "toggle"):
             self.selected_object.toggle()
 
     def _toggle_sticky_mode(self) -> None:
         self.sticky_mode = not self.sticky_mode
 
-    def save(self, file_name: str | None = None) -> None:
+    def save(self, file_name: Optional[str] = None) -> None:
         if file_name is None:
             file_name = self.status_bar.input("File name to save:")
         if file_name.strip() == "":
             return
         objects = self.serialize()
         with open(file_name, "w") as file:
             json.dump(objects, file)
 
-    def open(self, file_name: str | None = None) -> None:
+    def open(self, file_name: Optional[str] = None) -> None:
         if file_name is None:
             file_name = self.status_bar.input("File name to open:")
         if file_name == "" or not os.path.exists(file_name):
             self.status_bar.message("File not found.", curses.color_pair(2))
             return
         with open(file_name, "r") as file:
             objects = json.load(file)
```

### Comparing `term_ascii_diagram-0.0.2/src/term_ascii_diagram/main.py` & `term_ascii_diagram-0.0.3/src/term_ascii_diagram/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import curses
 import curses.ascii
+import os
 
 from term_ascii_diagram.diagram import Designer
 from term_ascii_diagram.status_bar import StatusBar
 
 
 def wrapped(args):
     def main(stdscr: curses.window):
@@ -50,14 +51,14 @@
 
     parser.add_argument("filename", nargs="?")
     parser.add_argument("-r", "--render")
 
     args = parser.parse_args()
 
     # To support escape key press
-    curses.set_escdelay(25)
+    os.environ.setdefault("ESCDELAY", "25")
     # Initialize curses
     curses.wrapper(wrapped(args))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `term_ascii_diagram-0.0.2/src/term_ascii_diagram/status_bar.py` & `term_ascii_diagram-0.0.3/src/term_ascii_diagram/status_bar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import curses
 from collections import OrderedDict
 from curses.textpad import Textbox
-from typing import Dict
+from typing import Dict, Optional
 
 
 class StatusBar:
     bg_color: int
     shortcuts: Dict[str, str]
     root_window: curses.window
     window: curses.window
@@ -43,15 +43,15 @@
             result = box.edit().strip()
         except KeyboardInterrupt:
             result = ""
         curses.curs_set(0)
         self.invalidate()
         return result
 
-    def message(self, text: str, attr: int | None = None) -> int:
+    def message(self, text: str, attr: Optional[int] = None) -> int:
         _, max_x = self.window.getmaxyx()
         self.window.addstr(
             0,
             0,
             text + (" " * (max_x - len(text) - 1)),
             attr or self.bg_color,
         )
```

### Comparing `term_ascii_diagram-0.0.2/LICENSE` & `term_ascii_diagram-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.2/README.md` & `term_ascii_diagram-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 | `s` | Save to file |
 | `o` | Open from file |
 | `b` | Add box |
 | `c` | Add line |
 | `a` | Add arrow |
 | `d` | Delete selected object |
 | `t` | Toggle sticky mode (whether moving boxes should move attached arrows/lines) |
+| `Tab` | Select next object |
+| `Shift`+`Tab` | Select previous object |
 | `Enter` | Edit box text if selected, otherwise, select the object under cursor |
 | `Esc` | Unselect current object |
 | `Space` | Toggle the line/arrow orientation or box border |
-| `Tab` | Select next object |
-| `Shift`+`Tab` | Select previous object |
```

### Comparing `term_ascii_diagram-0.0.2/pyproject.toml` & `term_ascii_diagram-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "term-ascii-diagram"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Amir Karimi", email="me@amirkarimi.dev" },
 ]
 description = "Build ASCII diagrams in terminal using keyboard."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX",
     "Topic :: Terminals",
     "Topic :: Utilities",
 ]
```

### Comparing `term_ascii_diagram-0.0.2/PKG-INFO` & `term_ascii_diagram-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: term-ascii-diagram
-Version: 0.0.2
+Version: 0.0.3
 Summary: Build ASCII diagrams in terminal using keyboard.
 Project-URL: Homepage, https://github.com/amirkarimi/term-ascii-diagram
 Project-URL: Issues, https://github.com/amirkarimi/term-ascii-diagram/issues
 Author-email: Amir Karimi <me@amirkarimi.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 Build ASCII diagrams in terminal using keyboard.
 
 ## Install
 
 ```
@@ -32,12 +32,12 @@
 | `s` | Save to file |
 | `o` | Open from file |
 | `b` | Add box |
 | `c` | Add line |
 | `a` | Add arrow |
 | `d` | Delete selected object |
 | `t` | Toggle sticky mode (whether moving boxes should move attached arrows/lines) |
+| `Tab` | Select next object |
+| `Shift`+`Tab` | Select previous object |
 | `Enter` | Edit box text if selected, otherwise, select the object under cursor |
 | `Esc` | Unselect current object |
 | `Space` | Toggle the line/arrow orientation or box border |
-| `Tab` | Select next object |
-| `Shift`+`Tab` | Select previous object |
```

