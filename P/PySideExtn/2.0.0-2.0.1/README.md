# Comparing `tmp/PySideExtn-2.0.0-py3-none-any.whl.zip` & `tmp/PySideExtn-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20419 bytes, number of entries: 11
--rw-r--r--  2.0 unx    28173 b- defN 23-Oct-07 18:12 PySideExtn/RoundProgressBar.py
--rw-r--r--  2.0 unx    38851 b- defN 23-Oct-07 18:12 PySideExtn/SpiralProgressBar.py
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-07 17:56 PySideExtn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-07 17:56 PySideExtn/demo/__init__.py
--rw-r--r--  2.0 unx    20098 b- defN 23-Oct-07 18:09 PySideExtn/demo/demo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-07 17:56 PySideExtn/examples/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Oct-07 18:27 PySideExtn-2.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9709 b- defN 23-Oct-07 18:27 PySideExtn-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-07 18:27 PySideExtn-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Oct-07 18:27 PySideExtn-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      901 b- defN 23-Oct-07 18:27 PySideExtn-2.0.0.dist-info/RECORD
-11 files, 98899 bytes uncompressed, 18885 bytes compressed:  80.9%
+Zip file size: 20662 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    26865 b- defN 24-Apr-09 08:02 PySideExtn/RoundProgressBar.py
+-rw-rw-rw-  2.0 fat    38851 b- defN 24-Apr-08 11:36 PySideExtn/SpiralProgressBar.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-08 11:36 PySideExtn/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-08 11:36 PySideExtn/demo/__init__.py
+-rw-rw-rw-  2.0 fat    20098 b- defN 24-Apr-08 11:36 PySideExtn/demo/demo.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-08 11:36 PySideExtn/examples/__init__.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 24-Apr-11 12:04 PySideExtn-2.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9977 b- defN 24-Apr-11 12:04 PySideExtn-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 12:04 PySideExtn-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-11 12:04 PySideExtn-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      901 b- defN 24-Apr-11 12:04 PySideExtn-2.0.1.dist-info/RECORD
+11 files, 97859 bytes uncompressed, 19128 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: PySideExtn/demo/demo.py
 Comment: 
 
 Filename: PySideExtn/examples/__init__.py
 Comment: 
 
-Filename: PySideExtn-2.0.0.dist-info/LICENSE
+Filename: PySideExtn-2.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: PySideExtn-2.0.0.dist-info/METADATA
+Filename: PySideExtn-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: PySideExtn-2.0.0.dist-info/WHEEL
+Filename: PySideExtn-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: PySideExtn-2.0.0.dist-info/top_level.txt
+Filename: PySideExtn-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: PySideExtn-2.0.0.dist-info/RECORD
+Filename: PySideExtn-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySideExtn/RoundProgressBar.py

```diff
@@ -2,79 +2,80 @@
 # CREATOR:  ANJAL.P                                                                         #
 # ON:       2020 SEP.                                                                       #
 # AIM:      To Extend the capability of the PySide2 and PyQt5 Python library with easy to   #
 #           use extension containing commonly used widgets which is not natively supported  #
 #           by the Qt Frame work (or atleast for Python version of Qt).                     #
 # VERSION:  v1.0.0                                                                          #
 # NOTES:    CLASS : RoundProgressBar : Can be accessed by : importing                       #
-#           from PySideExtn.RoundProgressBar import roundProgressBar                       #
+#           from PySideExtn.RoundProgressBar import RoundProgressBar                       #
 # REFER:    Github: https://github.com/anjalp/PySideExtn                                   #
 #############################################################################################
 
 
 from qtpy import QtWidgets, QtCore
-from qtpy.QtCore import Qt, QSize
+from qtpy.QtCore import Qt, QSize, QEvent, QRectF
 from qtpy.QtGui import QBrush, QColor, QPainter, QPen, QPaintEvent, QFont
+from qtpy.QtWidgets import QStyleOption, QStyle
 
 
-class roundProgressBar(QtWidgets.QWidget):
+class RoundProgressBar(QtWidgets.QWidget):
 
     def __init__(self, parent=None):
-        super(roundProgressBar, self).__init__(parent)
+        super(RoundProgressBar, self).__init__(parent)
 
         self.positionX = 0 
         self.positionY = 0
         self.posFactor = 0
 
-        self.rpb_minimumSize = (0, 0)
-        self.rpb_maximumSize = (0, 0)
-        self.rpb_dynamicMin = True
-        self.rpb_dynamicMax = True
-        self.rpb_Size = 0
+        self.minimumSize = (0, 0)
+        self.maximumSize = (0, 0)
+        self.dynamicMin = True
+        self.dynamicMax = True
+        self.Size = 0
         self.sizeFactor = 0
 
-        self.rpb_maximum = 100
-        self.rpb_minimum = 0
+        self.maximum = 100
+        self.minimum = 0
 
-        self.rpb_type = self.barStyleFlags.Donet
+        self.type = self.barStyleFlags.Donet
         self.startPosition = self.startPosFlags.North
-        self.rpb_direction = self.rotationFlags.Clockwise
+        self.direction = self.rotationFlags.Clockwise
 
-        self.rpb_textType = self.textFlags.Percentage
-        self.rpb_textColor = (0, 159, 227)
-        self.rpb_textWidth = self.rpb_Size/8
-        self.rpb_textFont = 'Segoe UI'
-        self.rpb_textValue = '12%'
-        self.rpb_textRatio = 8
+        self.textType = self.textFlags.Percentage
+        self.textColor = (0, 159, 227)
+        self.textWidth = self.Size/8
+        self.textFont = 'Segoe UI'
+        self.textValue = '12%'
+        self.textRatio = 8
         self.textFactorX = 0
         self.textFactorY = 0
         self.dynamicText = True
-        self.rpb_textActive = True
+        self.textActive = True
 
         self.lineWidth = 5
         self.pathWidth = 5
-        self.rpb_lineStyle = self.lineStyleFlags.SolidLine
-        self.rpb_lineCap = self.lineCapFlags.SquareCap
-        self.lineColor = (0, 159, 227)
+        self.lineStyle = self.lineStyleFlags.SolidLine
+        self.lineCap = self.lineCapFlags.SquareCap
+        self.lineColor = QColor(0, 159, 227)
         self.pathColor = (218, 218, 218)
 
-        self.rpb_circleColor = (218, 218, 218)
-        self.rpb_circleRatio = 0.8
-        self.rpb_circlePosX = 0
-        self.rpb_circlePosY = 0
-
-        self.rpb_pieColor = (200, 200, 200)
-        self.rpb_pieRatio = 1
-        self.rpb_piePosX = 0
-        self.rpb_piePosY = 0
+        self.circleColor = (218, 218, 218)
+        self.circleRatio = 0.8
+        self.circlePosX = 0
+        self.circlePosY = 0
+
+        self.pieColor = (200, 200, 200)
+        self.pieRatio = 1
+        self.piePosX = 0
+        self.piePosY = 0
 
-        self.rpb_value = -45*16
+        self._value = -45*16
 
-        if self.rpb_dynamicMin:
-            self.setMinimumSize(QSize(self.lineWidth*6 + self.pathWidth*6, self.lineWidth*6 + self.pathWidth*6))
+        # if self.dynamicMin:
+        self.setMinimumSize(QSize(self.lineWidth*6 + self.pathWidth*6, self.lineWidth*6 + self.pathWidth*6))
 
 #------------------------------------------------------CLASS ENUMERATORS
     class lineStyleFlags:
         SolidLine = Qt.SolidLine
         DotLine = Qt.DotLine
         DashLine = Qt.DashLine
 
@@ -101,71 +102,33 @@
     class startPosFlags:
         North = 90*16
         South = -90*16
         East = 0*16
         West = 180*16
 
 #------------------------------------------------------METHODS FOR CHANGING THE PROPERTY OF THE ROUNDPROGRESSBAR :SOLTS
+    def eventFilter(self, obj, e: QEvent):
+        if obj is self.window():
+            if e.type() == QEvent.Resize:
+                re = QResizeEvent(e)
+                self.resize(re.size())
+
+        return super().eventFilter(obj, e)
+    
+    def resizeEvent(self, e):
+        self.adjustSize()
+    
+    def showEvent(self, e):
+        self.adjustSize()
+        super().showEvent(e)
 
-    def rpb_setMinimumSize(self, width, height):
-        """
-        Minimum Size of the Widget
-        ...
-
-        Parameters
-        --------------
-
-        width : int
-            width of the Widget
+    def value(self):
+        return self._value
 
-        height : int
-            height of the Widget
-
-        Raises
-        --------------
-        Exception : Sorry Width/Height should be an int
-        """
-
-        if type(width)!=type(5) or type(height)!=type(5):
-            raise Exception('Sorry Width/Height should be an int')
-            return
-        self.rpb_dynamicMin = False
-        self.setMinimumSize(width, height)
-        self.rpb_minimumSize = (width, height)
-        self.update()
-
-    def rpb_setMaximumSize(self, width, height):
-        """
-        Maximum Size of the Widget
-        ...
-
-        Parameters
-        --------------
-
-        width : int
-            width of the Widget
-
-        height : int
-            height of the Widget
-
-        Raises
-        --------------
-        Exception : Sorry Width/Height should be an int
-        """
-        
-        if type(width)!=type(5) or type(height)!=type(5):
-            raise Exception('Sorry Width/Height should be an int')
-            return
-        self.rpb_dynamicMax = False
-        self.setMaximumSize(width, height)
-        self.rpb_maximumSize = (width, height)
-        self.update()
-
-
-    def rpb_setMaximum(self, maximum):
+    def setMaximumValue(self, maximum):
         """
         Maximum Value of the Progressbar
         ...
 
         Parameters
         --------------
 
@@ -173,22 +136,22 @@
             Maximum value of the round progress bar
 
         Raises
         --------------
         Exception : Maximum and Minimum cannot be the Same
         """
         
-        if self.rpb_minimum==maximum:               #FOR AVOIDING DIVISION BY ZERO ERROR IN FUTURE
+        if self.minimum==maximum:               #FOR AVOIDING DIVISION BY ZERO ERROR IN FUTURE
             raise Exception("Maximum and Minimum cannot be the Same")
             return
-        if self.rpb_maximum != maximum:
-            self.rpb_maximum = maximum
+        if self.maximum != maximum:
+            self.maximum = maximum
             self.update()
 
-    def rpb_setMinimum(self, minimum):
+    def setMinimumValue(self, minimum):
         """
         Minimum Value of the Progressbar
         ...
 
         Parameters
         --------------
 
@@ -196,22 +159,22 @@
             Minimum value of the round progress bar
 
         Raises
         --------------
         Exception : Maximum and Minimum cannot be the Same
         """
         
-        if self.rpb_minimum==maximum:               #FOR AVOIDING DIVISION BY ZERO ERROR IN FUTURE
+        if self.minimum==maximum:               #FOR AVOIDING DIVISION BY ZERO ERROR IN FUTURE
             raise Exception("Maximum and Minimum cannot be the Same")
             return
-        if self.rpb_minimum != minimum:
-            self.rpb_minimum = minimum
+        if self.minimum != minimum:
+            self.minimum = minimum
             self.update()
 
-    def rpb_setRange(self, maximum, minimum):
+    def setRange(self, maximum, minimum):
         """
         Range include the maximum and the minimum in one go.
         ...
 
         Parameters
         --------------
 
@@ -224,21 +187,21 @@
         Raises
         --------------
         none
         """
         
         if minimum > maximum:
             maximum, minimum = minimum, maximum
-        if self.rpb_maximum != maximum:
-            self.rpb_maximum = maximum
-        if self.rpb_minimum != minimum:
-            self.rpb_minimum = minimum
+        if self.maximum != maximum:
+            self.maximum = maximum
+        if self.minimum != minimum:
+            self.minimum = minimum
         self.update()
 
-    def rpb_setInitialPos(self, pos):
+    def setInitialPos(self, pos):
         """
         Starting position of the round progress bar
         ...
 
         Parameters
         --------------
 
@@ -258,15 +221,15 @@
             self.startPosition = self.startPosFlags.East
         elif pos=='West':
             self.startPosition = self.startPosFlags.West
         else:
             raise Exception("Initial Position String can be: 'South', 'North'")
             return
 
-    def rpb_setValue(self, value):
+    def setValue(self, value):
         """
         Set progress value
         ...
 
         Parameters
         --------------
 
@@ -274,41 +237,42 @@
             The value of the progress bar in int. The value should be: min<=value<=max
 
         Raises
         --------------
         none
         """
         
-        if self.rpb_value != value:
-            if value >= self.rpb_maximum:
-                roundProgressBar.convertInputValue(self, self.rpb_maximum)
-            elif value < self.rpb_minimum:
-                roundProgressBar.convertInputValue(self, self.rpb_minimum)
-            else:
-                roundProgressBar.convertInputValue(self, value)
-            self.update()
+        if value >= self.maximum:
+            RoundProgressBar.convertInputValue(self, self.maximum)
+        elif value < self.minimum:
+            RoundProgressBar.convertInputValue(self, self.minimum)
+        else:
+            RoundProgressBar.convertInputValue(self, value)
+        
+        self._value =  value
+        self.update()
 
-    def rpb_reset(self):
+    def reset(self):
         """
         Reset the progress bar to 0%
         ...
 
         Parameters
         --------------
         none
 
         Raises
         --------------
         none
         """
         
-        roundProgressBar.convertInputValue(self, self.rpb_minimum)
+        RoundProgressBar.convertInputValue(self, self.minimum)
         self.update()
 
-    def rpb_setGeometry(self, posX, posY):
+    def setGeometry(self, posX, posY):
         """
         Set the X and Y position of the round progress bar.
         ...
 
         Parameters
         --------------
 
@@ -325,15 +289,15 @@
         
         if self.positionX != posX:
             self.positionX = posX
         if self.positionY != posY:
             self.positionY = posY
         self.update()
 
-    def rpb_setLineWidth(self, width):
+    def setLineWidth(self, width):
         """
         Line Width of the line in round progress bar.
         ...
 
         Parameters
         --------------
 
@@ -348,15 +312,15 @@
         if type(width)!=type(5):
             raise Exception('Line Width should be in int')
             return
         if self.lineWidth != width:
             self.lineWidth = width
             self.update()
 
-    def rpb_setLineColor(self, rgb):
+    def setLineColor(self, rgb):
         """
         Line Color of the progress bar.
         ...
 
         Parameters
         --------------
 
@@ -364,22 +328,22 @@
             Color is passed as a tuple of values for red, blue and green in the order: (R, G, B)
 
         Raises
         --------------
         Exception: Line Color accepts a tuple: (R, G, B).
         """
 
-        if type(rgb)!=type(()):
-            raise Exception("Line Color accepts a tuple: (R, G, B).")
-            return
-        if self.lineColor != rgb:
-            self.lineColor = rgb
-            self.update()
+        # if type(rgb)!=type(()):
+        #     raise Exception("Line Color accepts a tuple: (R, G, B).")
+        #     return
+        # if self.lineColor != rgb:
+        self.lineColor = QColor(rgb)
+        self.update()
 
-    def rpb_setPathColor(self, rgb):
+    def setPathColor(self, rgb):
         """
         Path Color settings.
         ...
 
         Parameters
         --------------
 
@@ -394,15 +358,15 @@
         if type(rgb)!=type(()):
             raise Exception("Path Color accepts a tuple: (R, G, B).")
             return
         if self.pathColor != rgb:
             self.pathColor = rgb
             self.update()
 
-    def rpb_setPathWidth(self, width):
+    def setPathWidth(self, width):
         """
         Path width settings.
         ...
 
         Parameters
         --------------
 
@@ -417,15 +381,15 @@
         if type(width)!=type(5):
             raise Exception('Path Width should be in int')
             return
         if self.pathWidth != width:
             self.pathWidth = width
             self.update()
 
-    def rpb_setDirection(self, direction):
+    def setDirection(self, direction):
         """
         Direction of rotation of the progress bar.
         ...
 
         Parameters
         --------------
 
@@ -434,23 +398,23 @@
 
         Raises
         --------------
         Exception: Direction can only be: 'Clockwise' and 'AntiClockwise'
         """
 
         if direction == 'Clockwise' or direction == -1:
-            self.rpb_direction = self.rotationFlags.Clockwise
+            self.direction = self.rotationFlags.Clockwise
         elif direction == 'AntiClockwise' or direction == 1:
-            self.rpb_direction = self.rotationFlags.AntiClockwise
+            self.direction = self.rotationFlags.AntiClockwise
         else:
             raise Exception("Direction can only be: 'Clockwise' and 'AntiClockwise' and Not: " + str(direction))
             return
         self.update()
 
-    def rpb_setBarStyle(self, style):
+    def setBarStyle(self, style):
         """
         Bar Style of the progress bar.
         ...
 
         Parameters
         --------------
 
@@ -459,31 +423,31 @@
 
         Raises
         --------------
         Exception: Round Progress Bar has only the following styles: 'Line', 'Donet', 'Hybrid1', 'Pizza', 'Pie' and 'Hybrid2'
         """
 
         if style=='Donet':
-            self.rpb_type = self.barStyleFlags.Donet
+            self.type = self.barStyleFlags.Donet
         elif style=='Line':
-            self.rpb_type = self.barStyleFlags.Line
+            self.type = self.barStyleFlags.Line
         elif style=='Pie':
-            self.rpb_type = self.barStyleFlags.Pie
+            self.type = self.barStyleFlags.Pie
         elif style=='Pizza':
-            self.rpb_type = self.barStyleFlags.Pizza
+            self.type = self.barStyleFlags.Pizza
         elif style=='Hybrid1':
-            self.rpb_type = self.barStyleFlags.Hybrid1
+            self.type = self.barStyleFlags.Hybrid1
         elif style=='Hybrid2':
-            self.rpb_type = self.barStyleFlags.Hybrid2
+            self.type = self.barStyleFlags.Hybrid2
         else:
             raise Exception("Round Progress Bar has only the following styles: 'Line', 'Donet', 'Hybrid1', 'Pizza', 'Pie' and 'Hybrid2'")
             return
         self.update()
 
-    def rpb_setLineStyle(self, style):
+    def setLineStyle(self, style):
         """
         Line Style setting.
         ...
 
         Parameters
         --------------
 
@@ -492,23 +456,23 @@
 
         Raises
         --------------
         none
         """
 
         if style == 'SolidLine':
-            self.rpb_lineStyle = self.lineStyleFlags.SolidLine
+            self.lineStyle = self.lineStyleFlags.SolidLine
         elif style == 'DotLine':
-            self.rpb_lineStyle = self.lineStyleFlags.DotLine
+            self.lineStyle = self.lineStyleFlags.DotLine
         elif style == 'DashLine':
-            self.rpb_lineStyle = self.lineStyleFlags.DashLine
+            self.lineStyle = self.lineStyleFlags.DashLine
         else:
-            self.rpb_lineStyle = self.lineStyleFlags.SolidLine
+            self.lineStyle = self.lineStyleFlags.SolidLine
 
-    def rpb_setLineCap(self, cap):
+    def setLineCap(self, cap):
         """
         Line Cap setting.
         ...
 
         Parameters
         --------------
 
@@ -517,19 +481,19 @@
 
         Raises
         --------------
         none
         """
 
         if cap=='SquareCap':
-            self.rpb_lineCap = self.lineCapFlags.SquareCap
+            self.lineCap = self.lineCapFlags.SquareCap
         elif cap == 'RoundCap':
-            self.rpb_lineCap = self.lineCapFlags.RoundCap
+            self.lineCap = self.lineCapFlags.RoundCap
 
-    def rpb_setTextColor(self, rgb):
+    def setTextColor(self, rgb):
         """
         Text color of the text inside the progress bar
         ...
 
         Parameters
         --------------
 
@@ -537,19 +501,19 @@
             Color of the text in the format: (R, G, B)
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_textColor != rgb:
-            self.rpb_textColor = rgb
-            self.update()
+        # if self.textColor != rgb:
+        self.textColor = rgb
+        self.update()
 
-    def rpb_setTextFont(self, font):
+    def setTextFont(self, font):
         """
         Font of the text inside the round progress bar
         ...
 
         Parameters
         --------------
 
@@ -557,19 +521,19 @@
             Name of the font in string
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_textFont != font:
-            self.rpb_textFont = font
+        if self.textFont != font:
+            self.textFont = font
             self.update()
 
-    def rpb_setTextFormat(self, textTyp):
+    def setTextFormat(self, textTyp):
         """
         Text formatter i.e. the value or the percentage.
         ...
 
         Parameters
         --------------
 
@@ -578,21 +542,21 @@
 
         Raises
         --------------
         none
         """
 
         if textTyp == 'Value':
-            self.rpb_textType = self.textFlags.Value
+            self.textType = self.textFlags.Value
         elif textTyp == 'Percentage':
-            self.rpb_textType = self.textFlags.Percentage
+            self.textType = self.textFlags.Percentage
         else:
-            self.rpb_textType = self.textFlags.Percentage
+            self.textType = self.textFlags.Percentage
 
-    def rpb_setTextRatio(self, ratio):
+    def setTextRatio(self, ratio):
         """
         Text ratio with respect to the size of the progress bar.
         ...
 
         Parameters
         --------------
 
@@ -600,23 +564,23 @@
             In number from 3 to 50 corresponding to 1/3 or 1/50 the size of the roundprogressbar.
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_textRatio != ratio:
+        if self.textRatio != ratio:
             if ratio < 3:
                 ratio = 3
             elif ratio > 50:
                 ratio = 50
-            self.rpb_textRatio = ratio
+            self.textRatio = ratio
             self.update()
 
-    def rpb_setTextWidth(self, width):
+    def setTextWidth(self, width):
         """
         Text Width.
         ...
 
         Parameters
         --------------
 
@@ -626,18 +590,18 @@
         Raises
         --------------
         none
         """
 
         self.dynamicText = False
         if width > 0:
-            self.rpb_textWidth = width
+            self.textWidth = width
             self.update()
 
-    def rpb_setCircleColor(self, rgb):
+    def setCircleColor(self, rgb):
         """
         Circle color fill inside the circle.
         ...
 
         Parameters
         --------------
 
@@ -645,19 +609,19 @@
             The color of the circle in the tuple corresponding to the (R, G, B).
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_circleColor != rgb:
-            self.rpb_circleColor = rgb
+        if self.circleColor != rgb:
+            self.circleColor = rgb
             self.update()
 
-    def rpb_setCircleRatio(self, ratio):
+    def setCircleRatio(self, ratio):
         """
         Circle ration corresponding to the round progress bar.
         ...
 
         Parameters
         --------------
 
@@ -665,19 +629,19 @@
             Integer corresponding to the size of the progress bar to that of the round progress bar.
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_circleRatio != ratio:
-            self.rpb_circleRatio = ratio
+        if self.circleRatio != ratio:
+            self.circleRatio = ratio
             self.update()
 
-    def rpb_setPieColor(self, rgb):
+    def setPieColor(self, rgb):
         """
         Pie color inside the fill.
         ...
 
         Parameters
         --------------
 
@@ -685,19 +649,19 @@
             Tuple consist in format (R, G, B). Same as color setting to Line.
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_pieColor != rgb:
-            self.rpb_pieColor = rgb
+        if self.pieColor != rgb:
+            self.pieColor = rgb
             self.update()
 
-    def rpb_setPieRatio(self, ratio):
+    def setPieRatio(self, ratio):
         """
         Pie Ratio
         ...
 
         Parameters
         --------------
 
@@ -705,19 +669,19 @@
             Ratio corresponding to the size between the roundprogressbar and the pie size.
 
         Raises
         --------------
         none
         """
 
-        if self.rpb_pieRatio != ratio:
-            self.rpb_pieRatio = ratio
+        if self.pieRatio != ratio:
+            self.pieRatio = ratio
             self.update()
 
-    def rpb_enableText(self, enable):
+    def enableText(self, enable):
         """
         Makes the Text visible/Hidden
         ...
 
         Parameters
         --------------
 
@@ -726,226 +690,238 @@
 
         Raises
         --------------
         none
         """
 
         if enable:
-            self.rpb_textActive = enable
+            self.textActive = enable
         else:
-            self.rpb_textActive = enable
+            self.textActive = enable
         self.update()
 
 
 #------------------------------------------------------METHODS FOR GETTING THE PROPERTY OF ROUNDPROGRESSBAR SLOTS
 
-    def rpb_getSize(self):
+    def getSize(self):
         """
         Get the present size of the progress bar.
         ...
 
         Returns
         --------------
         Return the size of the round progress bar in int.
         """
 
-        return self.rpb_Size
+        return self.Size
 
-    def rpb_getValue(self):
+    def getValue(self):
         """
         Present value of the progress bar.
         ...
 
         Returns
         --------------
         int corresponding to the present progress bar value.
         """
 
-        return self.rpb_value/16
+        return self._value/16
 
-    def rpb_getRange(self):
+    def getRange(self):
         """
         Progress bar range.
         ...
 
         Returns
         --------------
         tuple consisting of minimu and maximum as elements.
         """
 
-        return (self.rpb_minimum, self.rpb_maximum)
+        return (self.minimum, self.maximum)
 
-    def rpb_getTextWidth(self):
+    def getTextWidth(self):
         """
         Text width of the present text in the central of the widget.
         ...
 
         Returns
         --------------
         int corresponding to the width of the text
         """
 
-        return self.rpb_textWidth
+        return self.textWidth
 
 #------------------------------------------------------ENGINE: WHERE ALL THE REAL STUFF TAKE PLACE: WORKING OF THE ROUNDPROGRESSBA
 
-    def rpb_MinimumSize(self, dynamicMax, minimum, maximum):
+    def MinimumSize(self, dynamicMax, minimum, maximum):
         """
         Minimum size calculating code: Takes consideration of the width of the line/path/circle/pie and the user defined
         width and also the size of the frame/window of the application.
 
         """
 
-        rpb_Height = self.height()
-        rpb_Width = self.width()
+        Height = self.height()
+        Width = self.width()
         if dynamicMax:
-            if rpb_Width >= rpb_Height and rpb_Height >= minimum[1]:
-                self.rpb_Size = rpb_Height
-            elif rpb_Width < rpb_Height and rpb_Width >= minimum[0]:
-                self.rpb_Size = rpb_Width
+            if Width >= Height and Height >= minimum[1]:
+                self.Size = Height
+            elif Width < Height and Width >= minimum[0]:
+                self.Size = Width
         else:
-            if rpb_Width >= rpb_Height and rpb_Height <= maximum[1]:
-                self.rpb_Size = rpb_Height
-            elif rpb_Width < rpb_Height and rpb_Width <= maximum[0]:
-                self.rpb_Size = rpb_Width
+            if Width >= Height and Height <= maximum[1]:
+                self.Size = Height
+            elif Width < Height and Width <= maximum[0]:
+                self.Size = Width
 
     def convertInputValue(self, value):
         """
         CONVERTS ANY INPUT VALUE TO THE 0*16-360*16 DEGREE REFERENCE OF THE QPainter.drawArc NEEDED.
 
         """
 
-        self.rpb_value = ((value - self.rpb_minimum)/(self.rpb_maximum - self.rpb_minimum))*360*16
-        self.rpb_value = self.rpb_direction*self.rpb_value
-        if self.rpb_textType==roundProgressBar.textFlags.Percentage:
-            self.rpb_textValue = str(round(((value - self.rpb_minimum)/(self.rpb_maximum - self.rpb_minimum))*100)) + "%"
+        self._value = ((value - self.minimum)/(self.maximum - self.minimum))*360*16
+        self._value = self.direction*self._value
+        if self.textType==RoundProgressBar.textFlags.Percentage:
+            self.textValue = str(round(((value - self.minimum)/(self.maximum - self.minimum))*100)) + "%"
         else:
-            self.rpb_textValue = str(value)
+            self.textValue = str(value)
 
     #SINCE THE THICKNESS OF THE LINE OR THE PATH CAUSES THE WIDGET TO WRONGLY FIT INSIDE THE SIZE OF THE WIDGET DESIGNED IN THE 
     #QTDESIGNER, THE CORRECTION FACTOR IS NECESSERY CALLED THE GEOMETRYFACTOR, WHICH CALCULATE THE TWO FACTORS CALLED THE
     #self.posFactor AND THE self.sizeFactor, CALCULATION THIS IS NECESSERY AS THE 
     def geometryFactor(self):
         if self.lineWidth > self.pathWidth:
             self.posFactor = self.lineWidth/2 + 1
             self.sizeFactor = self.lineWidth + 1
         else:
             self.posFactor = self.pathWidth/2 + 1
             self.sizeFactor = self.pathWidth + 1
 
-    def rpb_textFactor(self):
+    def textFactor(self):
         if self.dynamicText:
-            self.rpb_textWidth = self.rpb_Size/self.rpb_textRatio
-        self.textFactorX = self.posFactor + (self.rpb_Size - self.sizeFactor)/2 - self.rpb_textWidth*0.75*(len(self.rpb_textValue)/2)
-        self.textFactorY = self.rpb_textWidth/2 + self.rpb_Size/2
-
-    def rpb_circleFactor(self):
-        self.rpb_circlePosX = self.positionX + self.posFactor +  ((self.rpb_Size)*(1 - self.rpb_circleRatio))/2
-        self.rpb_circlePosY = self.positionY + self.posFactor + ((self.rpb_Size)*(1 - self.rpb_circleRatio))/2
-
-    def rpb_pieFactor(self):
-        self.rpb_piePosX = self.positionX + self.posFactor +  ((self.rpb_Size)*(1 - self.rpb_pieRatio))/2
-        self.rpb_piePosY = self.positionY + self.posFactor + ((self.rpb_Size)*(1 - self.rpb_pieRatio))/2
+            self.textWidth = self.Size/self.textRatio
+        self.textFactorX = self.posFactor + (self.Size - self.sizeFactor)/2 - self.textWidth*0.75*(len(self.textValue)/2)
+        self.textFactorY = self.textWidth/2 + self.Size/2
+
+    def circleFactor(self):
+        self.circlePosX = self.positionX + self.posFactor +  ((self.Size)*(1 - self.circleRatio))/2
+        self.circlePosY = self.positionY + self.posFactor + ((self.Size)*(1 - self.circleRatio))/2
+
+    def pieFactor(self):
+        self.piePosX = self.positionX + self.posFactor +  ((self.Size)*(1 - self.pieRatio))/2
+        self.piePosY = self.positionY + self.posFactor + ((self.Size)*(1 - self.pieRatio))/2
 
 
 
     def paintEvent(self, event: QPaintEvent):
+        opt = QStyleOption()
+        opt.initFrom(self)
+        painter = QPainter(self)
+        self.style().drawPrimitive(QStyle.PE_Widget, opt, painter, self)
         
         #THIS BELOW CODE AMKE SURE THAT THE SIZE OF THE ROUNDPROGRESSBAR DOESNOT REDUCES TO ZERO WHEN THE USER RESIZES THE WINDOW
-        if self.rpb_dynamicMin:
+        if self.dynamicMin:
             self.setMinimumSize(QSize(self.lineWidth*6 + self.pathWidth*6, self.lineWidth*6 + self.pathWidth*6))
 
-        roundProgressBar.rpb_MinimumSize(self, self.rpb_dynamicMax, self.rpb_minimumSize, self.rpb_maximumSize)
-        roundProgressBar.geometryFactor(self)
-        roundProgressBar.rpb_textFactor(self)
-        roundProgressBar.rpb_circleFactor(self)
-        roundProgressBar.rpb_pieFactor(self)
-        
-        if self.rpb_type==0: #DONET TYPE
-            roundProgressBar.pathComponent(self)
-            roundProgressBar.lineComponent(self)
-            roundProgressBar.textComponent(self)
-        elif self.rpb_type==1: #LINE TYPE
-            roundProgressBar.lineComponent(self)
-            roundProgressBar.textComponent(self)
-        elif self.rpb_type==2: #Pie
-            roundProgressBar.pieComponent(self)
-            roundProgressBar.textComponent(self)
-        elif self.rpb_type==3: #PIZZA
-            roundProgressBar.circleComponent(self)
-            roundProgressBar.lineComponent(self)
-            roundProgressBar.textComponent(self)
-        elif self.rpb_type==4: #HYBRID1
-            roundProgressBar.circleComponent(self)
-            roundProgressBar.pathComponent(self)
-            roundProgressBar.lineComponent(self)
-            roundProgressBar.textComponent(self)
-        elif self.rpb_type==5: #HYBRID2
-            roundProgressBar.pieComponent(self)
-            roundProgressBar.lineComponent(self)
-            roundProgressBar.textComponent(self)
+        self.setMinimumSize(self.size())
+
+        RoundProgressBar.MinimumSize(self, self.dynamicMax, self.minimumSize, self.maximumSize)
+        RoundProgressBar.geometryFactor(self)
+        RoundProgressBar.textFactor(self)
+        RoundProgressBar.circleFactor(self)
+        RoundProgressBar.pieFactor(self)
+        
+        if self.type==0: #DONET TYPE
+            RoundProgressBar.pathComponent(self)
+            RoundProgressBar.lineComponent(self)
+            RoundProgressBar.textComponent(self)
+        elif self.type==1: #LINE TYPE
+            RoundProgressBar.lineComponent(self)
+            RoundProgressBar.textComponent(self)
+        elif self.type==2: #Pie
+            RoundProgressBar.pieComponent(self)
+            RoundProgressBar.textComponent(self)
+        elif self.type==3: #PIZZA
+            RoundProgressBar.circleComponent(self)
+            RoundProgressBar.lineComponent(self)
+            RoundProgressBar.textComponent(self)
+        elif self.type==4: #HYBRID1
+            RoundProgressBar.circleComponent(self)
+            RoundProgressBar.pathComponent(self)
+            RoundProgressBar.lineComponent(self)
+            RoundProgressBar.textComponent(self)
+        elif self.type==5: #HYBRID2
+            RoundProgressBar.pieComponent(self)
+            RoundProgressBar.lineComponent(self)
+            RoundProgressBar.textComponent(self)
 
         
     def lineComponent(self):
         linePainter = QPainter(self)
         linePainter.setRenderHint(QPainter.Antialiasing)
+        
         penLine = QPen()
-        penLine.setStyle(self.rpb_lineStyle)
+        penLine.setStyle(self.lineStyle)
         penLine.setWidth(self.lineWidth)
-        penLine.setBrush(QColor(self.lineColor[0], self.lineColor[1], self.lineColor[2]))
-        penLine.setCapStyle(self.rpb_lineCap)
+        penLine.setBrush(self.lineColor)
+        penLine.setCapStyle(self.lineCap)
         penLine.setJoinStyle(Qt.RoundJoin)
         linePainter.setPen(penLine)
-        linePainter.drawArc(self.positionX + self.posFactor, self.positionY + self.posFactor, self.rpb_Size - self.sizeFactor, self.rpb_Size - self.sizeFactor, self.startPosition, self.rpb_value)
+        
+        # Calculate the start and end angles based on the value
+        startAngle = 0  # Start angle for clockwise arc
+        endAngle = startAngle - (self._value / self.maximum) * 360 * 16  # Convert value to angle (clockwise)
+
+        # Define the rectangle where the arc will be drawn
+        rect = QRectF(self.positionX + self.posFactor, self.positionY + self.posFactor,
+                    self.size().width() - self.sizeFactor, self.size().height() - self.sizeFactor)
+
+        # Draw the arc in clockwise direction
+        linePainter.drawArc(rect, startAngle, endAngle)
+
         linePainter.end()
 
     def pathComponent(self):
         pathPainter = QPainter(self)
         pathPainter.setRenderHint(QPainter.Antialiasing)
         penPath = QPen()
         penPath.setStyle(Qt.SolidLine)
         penPath.setWidth(self.pathWidth)
         penPath.setBrush(QColor(self.pathColor[0], self.pathColor[1], self.pathColor[2]))
         penPath.setCapStyle(Qt.RoundCap)
         penPath.setJoinStyle(Qt.RoundJoin)
         pathPainter.setPen(penPath)
-        pathPainter.drawArc(self.positionX + self.posFactor, self.positionY + self.posFactor, self.rpb_Size - self.sizeFactor, self.rpb_Size - self.sizeFactor, 0, 360*16)
+        pathPainter.drawArc(self.positionX + self.posFactor, self.positionY + self.posFactor, self.Size - self.sizeFactor, self.Size - self.sizeFactor, 0, 360*16)
         pathPainter.end()
 
     def textComponent(self):
-        if self.rpb_textActive:
+        if self.textActive:
             textPainter = QPainter(self)
             penText = QPen()
-            penText.setColor(QColor(self.rpb_textColor[0], self.rpb_textColor[1], self.rpb_textColor[2]))
+            penText.setColor(QColor(self.textColor))
             textPainter.setPen(penText)
             fontText = QFont()
-            fontText.setFamily(self.rpb_textFont)
-            fontText.setPointSize(self.rpb_textWidth)
+            fontText.setFamily(self.textFont)
+            fontText.setPointSize(self.textWidth)
             textPainter.setFont(fontText)
-            textPainter.drawText(self.positionX + self.textFactorX, self.positionY + self.textFactorY, self.rpb_textValue)
+            textPainter.drawText(self.positionX + self.textFactorX, self.positionY + self.textFactorY, self.textValue)
             textPainter.end()
 
     def circleComponent(self):
         circlePainter = QPainter(self)   
         penCircle = QPen()
         penCircle.setWidth(0)
-        penCircle.setColor(QColor(self.rpb_circleColor[0], self.rpb_circleColor[1], self.rpb_circleColor[2]))
+        penCircle.setColor(QColor(self.circleColor[0], self.circleColor[1], self.circleColor[2]))
         circlePainter.setRenderHint(QPainter.Antialiasing)
         circlePainter.setPen(penCircle)
-        circlePainter.setBrush(QColor(self.rpb_circleColor[0], self.rpb_circleColor[1], self.rpb_circleColor[2]))
-        circlePainter.drawEllipse(self.rpb_circlePosX, self.rpb_circlePosY, (self.rpb_Size - self.sizeFactor)*self.rpb_circleRatio, (self.rpb_Size - self.sizeFactor)*self.rpb_circleRatio)
+        circlePainter.setBrush(QColor(self.circleColor[0], self.circleColor[1], self.circleColor[2]))
+        circlePainter.drawEllipse(self.circlePosX, self.circlePosY, (self.Size - self.sizeFactor)*self.circleRatio, (self.Size - self.sizeFactor)*self.circleRatio)
 
     def pieComponent(self):
         piePainter = QPainter(self)   
         penPie = QPen()
         penPie.setWidth(0)
-        penPie.setColor(QColor(self.rpb_pieColor[0], self.rpb_pieColor[1], self.rpb_pieColor[2]))
+        penPie.setColor(QColor(self.pieColor[0], self.pieColor[1], self.pieColor[2]))
         piePainter.setRenderHint(QPainter.Antialiasing)
         piePainter.setPen(penPie)
-        piePainter.setBrush(QColor(self.rpb_pieColor[0], self.rpb_pieColor[1], self.rpb_pieColor[2]))
-        piePainter.drawPie(self.rpb_piePosX, self.rpb_piePosY, (self.rpb_Size - self.sizeFactor)*self.rpb_pieRatio, (self.rpb_Size - self.sizeFactor)*self.rpb_pieRatio, self.startPosition, self.rpb_value)
-
-
-#------------------------------------------------------
-
-if __name__=="__main__":
-    print("Try Import.")
+        piePainter.setBrush(QColor(self.pieColor[0], self.pieColor[1], self.pieColor[2]))
+        piePainter.drawPie(self.piePosX, self.piePosY, (self.Size - self.sizeFactor)*self.pieRatio, (self.Size - self.sizeFactor)*self.pieRatio, self.startPosition, self._value)
```

## Comparing `PySideExtn-2.0.0.dist-info/LICENSE` & `PySideExtn-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PySideExtn-2.0.0.dist-info/METADATA` & `PySideExtn-2.0.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-Metadata-Version: 2.1
-Name: PySideExtn
-Version: 2.0.0
-Summary: PySideExtn is an open-source Python programming language extension designed to empower PySide2/6 users with an expanded toolkit. This extension enriches the PySide2/6 library by introducing a range of additional widgets and features, significantly enhancing its capabilities and versatility.
-Home-page: https://github.com/KhamisiKibet/PySideExtn
-Author: ANJAL.P. Improved by Khamisi Kibet
-Author-email: spinncompany@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: qtpy
-
-# PySideExtn
-
-An extension for the Python PySide2 Qt Framework which expands the scope of the PySide2 package with many different modern widgets. Current release is occupied with two widget which are not natively present in the PySide2 package.
-
-*RoundProgressBar*
-
-<p align="center">
-  <img src="assets/rpb.png">
-</p>
-
-*SpiralProgressBar*
-
-<p align="center">
-  <img src="assets/spb.png">
-</p>
-
-:point_right: Go to [Home Page](https://anjalp.github.io/PySideExtn/) of Documentation for further Help
-
-## Getting Started
-
-* Install PySideExtn using `pip`
-
-``` python
-pip install PySideExtn
-```
-
-* Build from source: After cloning the repo, go to the directory and open `cmd` or `terminal`
-
-``` bash
-$ python3 setup.py sdist bdist_wheel
-```
-
-* Install from `.whl` file.
-
-```python
-pip install <PySideExtn------.whl>file
-```
-
-To verify that installation is complete, print out the `pip list` and search for the PySideExtn package. 
-
-:point_right: For more details go to the [Official PySideExtn Documentation Getting Started](https://anjalp.github.io/PySideExtn/pages/get_started)
-
-## Quick Demo
-
-Quick demo help you to check weather you have successfully installed the Python Package. It comes with a UI loaded with all the widgets in this package with its different customized views. Users can easily differentiate the different styling elements used by widgets.
-
-After installing the PySideExtn/PyQt5extn the users can try out quick demo by:
-
-1. Open the `cmd` or `terminal`. Open `Python`
-
-```python
->> from PySideExtn.demo import demo
->> demo.main()   #PRESS ENTER AND YOU WILL GET A DEMO APPLICATION
-```
-
-<p align="center">
-  <img src="assets/demo/rpb.PNG">
-</p>
-
-## Documentation
-
-Official Documentation for PySideExtn is detailed in: [PySideExtn Documentation](https://anjalp.github.io/PySideExtn/).
-
-:point_right: [Getting Started](https://anjalp.github.io/PySideExtn/pages/get_started)
-
-:point_right: [Examples](https://anjalp.github.io/PySideExtn/pages/example)
-
-:point_right: [Classes](https://anjalp.github.io/PySideExtn/pages/classes)
-
-:point_right: [Errors and Exceptions](https://anjalp.github.io/PySideExtn/pages/error&exception)
-
-:point_right: [Version History](https://anjalp.github.io/PySideExtn/pages/version)
-
-:point_right: [FAQ's](https://anjalp.github.io/PySideExtn/pages/faqs)
-
-:point_right: [Official PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA)
-
-## Examples
-
-* **Default Round Progress Bar**
-
-```python
-import sys
-from PySide2 import QtCore, QtWidgets, QtGui
-
-from PySideExtn.RoundProgressBar import roundProgressBar #IMPORT THE EXTENSION LIBRARY
-
-x = 0
-p = 1
-
-class MyWidget(QtWidgets.QWidget):
-    def __init__(self):
-        QtWidgets.QWidget.__init__(self)
-
-        self.hello = 'Round Progress Bar'
-        self.button = QtWidgets.QPushButton("Click me to change Value")
-        self.text = QtWidgets.QLabel("Round Progress Bar")
-        self.text.setAlignment(QtCore.Qt.AlignCenter)
-        
-        #CREATING THE ROUND PROGRESS BAR OBJECT
-        self.rpb = roundProgressBar()
-        
-        self.layout = QtWidgets.QVBoxLayout()
-        self.layout.addWidget(self.text)
-        self.layout.addWidget(self.button)
-        
-        # ADDING THE ROUND PROGRESS BAR OBJECT TO THE                                             # BOTTOM OF THE LAYOUT
-        self.layout.addWidget(self.rpb)
-
-        self.setLayout(self.layout)
-        self.button.clicked.connect(self.magic) #BUTTON PRESSED EVENT
-        
-    def magic(self):
-        global x, p
-        x = x + 10*p
-        if x==100:
-            p = -1
-        elif x==0:
-            p = 1
-        self.rpb.rpb_setValue(x)        #CHANGING THE VALUE OF THE PROGRESS BAR
-        out_text = 'Round Progress Bar: ' + str(x) + '%'
-        self.text.setText(out_text)
-        
-if __name__ == "__main__":
-    app = QtWidgets.QApplication(sys.argv)
-    widget = MyWidget()
-    widget.show()
-    sys.exit(app.exec_())
-```
-
-<p align="center">
-  <img src="assets/rpb/rpb_demo.PNG">
-</p>
-
-In this demo, we first created an object of the Round Progress Bar:
-
-```python
-self.rpb = roundProgressBar() #CREATING THE ROUND PROGRESS BAR OBJECT
-```
-
-After that calling the Round Progress Bar object to display the value of progress using:
-
-```python
-self.rpb.rpb_setValue(x) #CHANGING THE VALUE OF THE PROGRESS BAR
-```
-
-The `rpb_setValue(value)` takes an `int` as an argument and updates to change the value of the progress bar to the value given.
-
-:point_right: For More examples on Round Progress Bar go to: [Official PySideExtn Documentation Examples](https://anjalp.github.io/PySideExtn/pages/examples/rpbExamples)
-
-* **Default Spiral Progress Bar**
-
-```python
-import sys
-from PySide2 import QtCore, QtWidgets, QtGui
-
-#IMPORT THE EXTENSION  LIBRARY
-from PySideExtn.SpiralProgressBar import spiralProgressBar 
-
-x = 0
-p = 1
-
-class MyWidget(QtWidgets.QWidget):
-    def __init__(self):
-        QtWidgets.QWidget.__init__(self)
-
-        self.hello = 'Spiral Progress Bar'
-        self.button = QtWidgets.QPushButton("Click me to change Value")
-        self.text = QtWidgets.QLabel("Spiral Progress Bar")
-        self.text.setAlignment(QtCore.Qt.AlignCenter)
-        
-        #CREATING THE SPIRAL PROGRESS BAR OBJECT
-        self.spb = spiralProgressBar()    
-        
-        #ADDING WIDGETS TO THE VERTICAL LAYOUT
-        self.layout = QtWidgets.QVBoxLayout()
-        self.layout.addWidget(self.text)
-        self.layout.addWidget(self.button)
-        
-        # ADDING THE SPIRAL PROGRESS BAR OBJECT TO THE LAYOUT
-        self.layout.addWidget(self.spb) 
-        
-        self.setLayout(self.layout)
-        self.button.clicked.connect(self.magic) #BUTTON PRESSED EVENT
-        
-    def magic(self):
-        global x, p
-        x = x + 10*p
-        if x==100:
-            p = -1
-        elif x==0:
-            p = 1
-            
-        #CHANGING THE VALUE OF THE 3 DEFAULT PROGRESS BAR
-        self.spb.spb_setValue((x, x*2, x*3)) 
-        
-        out_text = 'Spiral Progress Bar: '  
-        out_text = out_text + str(x) + '%, ' + str(2*x) + '%, ' + str(3*x) + '%'
-        self.text.setText(out_text)
-        
-if __name__ == "__main__":
-    app = QtWidgets.QApplication(sys.argv)
-    widget = MyWidget()
-    widget.show()
-    sys.exit(app.exec_())
-```
-
-<p align="center">
-  <img src="assets/spb/spb_defEx.PNG">
-</p>
-
-- Here first create a spiralProgressBar object and then add the progress bar to a layout and control the steps of the progress bar by the clicking of the button. 
-
-  ```python
-  self.spb = spiralProgressBar()		
-  ```
-
-- Here we create a spiralProgressBar object instance and then use the `self.spb` as the spiral progress bar to influence its charactor like:
-
-  ```python
-  self.spb.spb_setValue((x, x*2, x*3))
-  ```
-
-- Since the default progress bar has 3 individual concentric circle, where each can be controlled individually, we pass a tuple containing the individual value for manipulating each concentric progress bar, to the function `spb_setValue()` , which only accepts a tuple of length equal to the number of concentric progress bar. Every function which can manipulate the properties of the Spiral Progress Bar uses the same idea. The order of entering the value are shown below:
-
-<p align="center">
-  <img src="assets/spb/spb_order.png">
-</p>
-
-:point_right: For More examples on Spiral Progress Bar go to: [Official PySideExtn Documentation Examples](https://anjalp.github.io/PySideExtn/pages/examples/spbExamples)
-
-## Help
-
-- **PySideExtn/PyQt5extn is not working in my setup**: Go to Github [PySideExtn](https://github.com/anjalp/PySideExtn) repo. and raise an issue or just fill the official [PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA).
-- **Unknown errors**: Raise a GitHub issue or fill the official [PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA)
-
-## Support
-
-- Please feel free to contribute to the project by sharing the idea you have, which is not natively present in the PySide2/PyQt5 but essential for your workflow.
-- You can fill up the official [PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA) where you just Brief the idea you have and also provide an active email address which is required for us to connect you.
-- If your idea worth the use, then definitely it will be available in the next update of the PySideExtn/PyQt5extn.
-- If this package made your life easy, then please share your experience with us [Here](https://forms.gle/yfKVK85sLLMJMCfJA)
-
-:smiley: Support my work by forking or downloading this project, check it out, and [share the experience](https://forms.gle/yfKVK85sLLMJMCfJA).
-
-:smiley: Support like this motivates me to do more creative, work for Open Source.
-
+Metadata-Version: 2.1
+Name: PySideExtn
+Version: 2.0.1
+Summary: PySideExtn is an open-source Python programming language extension designed to empower PySide2/6 users with an expanded toolkit. This extension enriches the PySide2/6 library by introducing a range of additional widgets and features, significantly enhancing its capabilities and versatility.
+Home-page: https://github.com/KhamisiKibet/PySideExtn
+Author: ANJAL.P. Improved by Khamisi Kibet
+Author-email: spinncompany@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: qtpy
+
+# PySideExtn
+
+An extension for the Python PySide2 Qt Framework which expands the scope of the PySide2 package with many different modern widgets. Current release is occupied with two widget which are not natively present in the PySide2 package.
+
+*RoundProgressBar*
+
+<p align="center">
+  <img src="assets/rpb.png">
+</p>
+
+*SpiralProgressBar*
+
+<p align="center">
+  <img src="assets/spb.png">
+</p>
+
+:point_right: Go to [Home Page](https://anjalp.github.io/PySideExtn/) of Documentation for further Help
+
+## Getting Started
+
+* Install PySideExtn using `pip`
+
+``` python
+pip install PySideExtn
+```
+
+* Build from source: After cloning the repo, go to the directory and open `cmd` or `terminal`
+
+``` bash
+$ python3 setup.py sdist bdist_wheel
+```
+
+* Install from `.whl` file.
+
+```python
+pip install <PySideExtn------.whl>file
+```
+
+To verify that installation is complete, print out the `pip list` and search for the PySideExtn package. 
+
+:point_right: For more details go to the [Official PySideExtn Documentation Getting Started](https://anjalp.github.io/PySideExtn/pages/get_started)
+
+## Quick Demo
+
+Quick demo help you to check weather you have successfully installed the Python Package. It comes with a UI loaded with all the widgets in this package with its different customized views. Users can easily differentiate the different styling elements used by widgets.
+
+After installing the PySideExtn/PyQt5extn the users can try out quick demo by:
+
+1. Open the `cmd` or `terminal`. Open `Python`
+
+```python
+>> from PySideExtn.demo import demo
+>> demo.main()   #PRESS ENTER AND YOU WILL GET A DEMO APPLICATION
+```
+
+<p align="center">
+  <img src="assets/demo/rpb.PNG">
+</p>
+
+## Documentation
+
+Official Documentation for PySideExtn is detailed in: [PySideExtn Documentation](https://anjalp.github.io/PySideExtn/).
+
+:point_right: [Getting Started](https://anjalp.github.io/PySideExtn/pages/get_started)
+
+:point_right: [Examples](https://anjalp.github.io/PySideExtn/pages/example)
+
+:point_right: [Classes](https://anjalp.github.io/PySideExtn/pages/classes)
+
+:point_right: [Errors and Exceptions](https://anjalp.github.io/PySideExtn/pages/error&exception)
+
+:point_right: [Version History](https://anjalp.github.io/PySideExtn/pages/version)
+
+:point_right: [FAQ's](https://anjalp.github.io/PySideExtn/pages/faqs)
+
+:point_right: [Official PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA)
+
+## Examples
+
+* **Default Round Progress Bar**
+
+```python
+import sys
+from PySide2 import QtCore, QtWidgets, QtGui
+
+from PySideExtn.RoundProgressBar import roundProgressBar #IMPORT THE EXTENSION LIBRARY
+
+x = 0
+p = 1
+
+class MyWidget(QtWidgets.QWidget):
+    def __init__(self):
+        QtWidgets.QWidget.__init__(self)
+
+        self.hello = 'Round Progress Bar'
+        self.button = QtWidgets.QPushButton("Click me to change Value")
+        self.text = QtWidgets.QLabel("Round Progress Bar")
+        self.text.setAlignment(QtCore.Qt.AlignCenter)
+        
+        #CREATING THE ROUND PROGRESS BAR OBJECT
+        self.rpb = roundProgressBar()
+        
+        self.layout = QtWidgets.QVBoxLayout()
+        self.layout.addWidget(self.text)
+        self.layout.addWidget(self.button)
+        
+        # ADDING THE ROUND PROGRESS BAR OBJECT TO THE                                             # BOTTOM OF THE LAYOUT
+        self.layout.addWidget(self.rpb)
+
+        self.setLayout(self.layout)
+        self.button.clicked.connect(self.magic) #BUTTON PRESSED EVENT
+        
+    def magic(self):
+        global x, p
+        x = x + 10*p
+        if x==100:
+            p = -1
+        elif x==0:
+            p = 1
+        self.rpb.rpb_setValue(x)        #CHANGING THE VALUE OF THE PROGRESS BAR
+        out_text = 'Round Progress Bar: ' + str(x) + '%'
+        self.text.setText(out_text)
+        
+if __name__ == "__main__":
+    app = QtWidgets.QApplication(sys.argv)
+    widget = MyWidget()
+    widget.show()
+    sys.exit(app.exec_())
+```
+
+<p align="center">
+  <img src="assets/rpb/rpb_demo.PNG">
+</p>
+
+In this demo, we first created an object of the Round Progress Bar:
+
+```python
+self.rpb = roundProgressBar() #CREATING THE ROUND PROGRESS BAR OBJECT
+```
+
+After that calling the Round Progress Bar object to display the value of progress using:
+
+```python
+self.rpb.rpb_setValue(x) #CHANGING THE VALUE OF THE PROGRESS BAR
+```
+
+The `rpb_setValue(value)` takes an `int` as an argument and updates to change the value of the progress bar to the value given.
+
+:point_right: For More examples on Round Progress Bar go to: [Official PySideExtn Documentation Examples](https://anjalp.github.io/PySideExtn/pages/examples/rpbExamples)
+
+* **Default Spiral Progress Bar**
+
+```python
+import sys
+from PySide2 import QtCore, QtWidgets, QtGui
+
+#IMPORT THE EXTENSION  LIBRARY
+from PySideExtn.SpiralProgressBar import spiralProgressBar 
+
+x = 0
+p = 1
+
+class MyWidget(QtWidgets.QWidget):
+    def __init__(self):
+        QtWidgets.QWidget.__init__(self)
+
+        self.hello = 'Spiral Progress Bar'
+        self.button = QtWidgets.QPushButton("Click me to change Value")
+        self.text = QtWidgets.QLabel("Spiral Progress Bar")
+        self.text.setAlignment(QtCore.Qt.AlignCenter)
+        
+        #CREATING THE SPIRAL PROGRESS BAR OBJECT
+        self.spb = spiralProgressBar()    
+        
+        #ADDING WIDGETS TO THE VERTICAL LAYOUT
+        self.layout = QtWidgets.QVBoxLayout()
+        self.layout.addWidget(self.text)
+        self.layout.addWidget(self.button)
+        
+        # ADDING THE SPIRAL PROGRESS BAR OBJECT TO THE LAYOUT
+        self.layout.addWidget(self.spb) 
+        
+        self.setLayout(self.layout)
+        self.button.clicked.connect(self.magic) #BUTTON PRESSED EVENT
+        
+    def magic(self):
+        global x, p
+        x = x + 10*p
+        if x==100:
+            p = -1
+        elif x==0:
+            p = 1
+            
+        #CHANGING THE VALUE OF THE 3 DEFAULT PROGRESS BAR
+        self.spb.spb_setValue((x, x*2, x*3)) 
+        
+        out_text = 'Spiral Progress Bar: '  
+        out_text = out_text + str(x) + '%, ' + str(2*x) + '%, ' + str(3*x) + '%'
+        self.text.setText(out_text)
+        
+if __name__ == "__main__":
+    app = QtWidgets.QApplication(sys.argv)
+    widget = MyWidget()
+    widget.show()
+    sys.exit(app.exec_())
+```
+
+<p align="center">
+  <img src="assets/spb/spb_defEx.PNG">
+</p>
+
+- Here first create a spiralProgressBar object and then add the progress bar to a layout and control the steps of the progress bar by the clicking of the button. 
+
+  ```python
+  self.spb = spiralProgressBar()		
+  ```
+
+- Here we create a spiralProgressBar object instance and then use the `self.spb` as the spiral progress bar to influence its charactor like:
+
+  ```python
+  self.spb.spb_setValue((x, x*2, x*3))
+  ```
+
+- Since the default progress bar has 3 individual concentric circle, where each can be controlled individually, we pass a tuple containing the individual value for manipulating each concentric progress bar, to the function `spb_setValue()` , which only accepts a tuple of length equal to the number of concentric progress bar. Every function which can manipulate the properties of the Spiral Progress Bar uses the same idea. The order of entering the value are shown below:
+
+<p align="center">
+  <img src="assets/spb/spb_order.png">
+</p>
+
+:point_right: For More examples on Spiral Progress Bar go to: [Official PySideExtn Documentation Examples](https://anjalp.github.io/PySideExtn/pages/examples/spbExamples)
+
+## Help
+
+- **PySideExtn/PyQt5extn is not working in my setup**: Go to Github [PySideExtn](https://github.com/anjalp/PySideExtn) repo. and raise an issue or just fill the official [PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA).
+- **Unknown errors**: Raise a GitHub issue or fill the official [PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA)
+
+## Support
+
+- Please feel free to contribute to the project by sharing the idea you have, which is not natively present in the PySide2/PyQt5 but essential for your workflow.
+- You can fill up the official [PySideExtn/PyQt5extn Form](https://forms.gle/yfKVK85sLLMJMCfJA) where you just Brief the idea you have and also provide an active email address which is required for us to connect you.
+- If your idea worth the use, then definitely it will be available in the next update of the PySideExtn/PyQt5extn.
+- If this package made your life easy, then please share your experience with us [Here](https://forms.gle/yfKVK85sLLMJMCfJA)
+
+:smiley: Support my work by forking or downloading this project, check it out, and [share the experience](https://forms.gle/yfKVK85sLLMJMCfJA).
+
+:smiley: Support like this motivates me to do more creative, work for Open Source.
+
```

