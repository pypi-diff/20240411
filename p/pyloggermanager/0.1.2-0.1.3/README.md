# Comparing `tmp/pyloggermanager-0.1.2-py3-none-any.whl.zip` & `tmp/pyloggermanager-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 36285 bytes, number of entries: 15
--rw-r--r--  2.0 unx     3421 b- defN 24-Apr-11 17:48 pyloggermanager/__init__.py
--rw-r--r--  2.0 unx    96688 b- defN 24-Apr-11 17:48 pyloggermanager/__main__.py
--rw-r--r--  2.0 unx     2379 b- defN 24-Apr-11 17:48 pyloggermanager/formatters/__init__.py
--rw-r--r--  2.0 unx    14809 b- defN 24-Apr-11 17:48 pyloggermanager/formatters/__main__.py
--rw-r--r--  2.0 unx     2292 b- defN 24-Apr-11 17:48 pyloggermanager/handlers/__init__.py
--rw-r--r--  2.0 unx    20136 b- defN 24-Apr-11 17:48 pyloggermanager/handlers/__main__.py
--rw-r--r--  2.0 unx     2413 b- defN 24-Apr-11 17:48 pyloggermanager/streams/__init__.py
--rw-r--r--  2.0 unx     4315 b- defN 24-Apr-11 17:48 pyloggermanager/streams/__main__.py
--rw-r--r--  2.0 unx     2200 b- defN 24-Apr-11 17:48 pyloggermanager/textstyles/__init__.py
--rw-r--r--  2.0 unx    12249 b- defN 24-Apr-11 17:48 pyloggermanager/textstyles/__main__.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-11 17:48 pyloggermanager-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      302 b- defN 24-Apr-11 17:48 pyloggermanager-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 17:48 pyloggermanager-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-11 17:48 pyloggermanager-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1347 b- defN 24-Apr-11 17:48 pyloggermanager-0.1.2.dist-info/RECORD
-15 files, 163728 bytes uncompressed, 34029 bytes compressed:  79.2%
+Zip file size: 41277 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     2329 b- defN 24-Apr-11 19:41 pyloggermanager/__init__.py
+-rw-r--r--  2.0 unx    95596 b- defN 24-Apr-11 19:41 pyloggermanager/__main__.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Apr-11 19:41 pyloggermanager/formatters/__init__.py
+-rw-r--r--  2.0 unx    13717 b- defN 24-Apr-11 19:41 pyloggermanager/formatters/__main__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Apr-11 19:41 pyloggermanager/handlers/__init__.py
+-rw-r--r--  2.0 unx    19044 b- defN 24-Apr-11 19:41 pyloggermanager/handlers/__main__.py
+-rw-r--r--  2.0 unx     1321 b- defN 24-Apr-11 19:41 pyloggermanager/streams/__init__.py
+-rw-r--r--  2.0 unx     3223 b- defN 24-Apr-11 19:41 pyloggermanager/streams/__main__.py
+-rw-r--r--  2.0 unx     1108 b- defN 24-Apr-11 19:41 pyloggermanager/textstyles/__init__.py
+-rw-r--r--  2.0 unx    11157 b- defN 24-Apr-11 19:41 pyloggermanager/textstyles/__main__.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    54172 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1349 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/RECORD
+15 files, 206680 bytes uncompressed, 39021 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pyloggermanager/textstyles/__init__.py
 Comment: 
 
 Filename: pyloggermanager/textstyles/__main__.py
 Comment: 
 
-Filename: pyloggermanager-0.1.2.dist-info/LICENSE
+Filename: pyloggermanager-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyloggermanager-0.1.2.dist-info/METADATA
+Filename: pyloggermanager-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pyloggermanager-0.1.2.dist-info/WHEEL
+Filename: pyloggermanager-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyloggermanager-0.1.2.dist-info/top_level.txt
+Filename: pyloggermanager-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyloggermanager-0.1.2.dist-info/RECORD
+Filename: pyloggermanager-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyloggermanager/__init__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 __all__ = [
     "CallerFrame",
     "Colorization",
     "FileMode",
     "Lock",
     "LogLevel",
     "Record",
@@ -63,15 +43,15 @@
 
 Beyond technical capabilities, the pyloggermanager package contributes to the reliability and maintainability of Python
 applications. It establishes consistent logging practices, simplifying collaboration, code reviews, and issue
 resolution across development teams. Overall, the pyloggermanager package is an invaluable asset for developers aiming
 to implement robust logging solutions, ensuring efficient and resilient application performance.
 """
 __name__ = "pyloggermanager"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 from pyloggermanager import formatters
 from pyloggermanager import handlers
 from pyloggermanager import streams
 from pyloggermanager import textstyles
 from pyloggermanager.__main__ import CallerFrame, Colorization, FileMode, Lock, LogLevel, Record, Logger, Manager, \
     Registry, RootLogger, load_config, get_logger, critical, debug, error, info, warning, log, disable, shutdown
```

## pyloggermanager/__main__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 import inspect
 import io
 import json
 import os
 import random
 import re
 import string
```

## pyloggermanager/formatters/__init__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 __all__ = [
     "DEFAULT_FORMAT",
     "CSV_FORMAT",
     "JSON_FORMAT",
     "DATE_FORMAT",
     "Formatter",
     "DefaultFormatter",
```

## pyloggermanager/formatters/__main__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 import io
 import json
 import time
 import traceback
 from types import TracebackType
 from typing import Optional, Tuple, Type, Union
```

## pyloggermanager/handlers/__init__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 __all__ = [
     "Handler",
     "ConsoleHandler",
     "FileHandler",
     "StreamHandler",
     "StderrHandler"
 ]
```

## pyloggermanager/handlers/__main__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 import io
 import os
 import sys
 from types import NoneType
 from typing import Any, TextIO, Union
 
 import pyloggermanager
```

## pyloggermanager/streams/__init__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 __all__ = [
     "Stream",
     "StdoutStream",
     "StderrStream",
     "TerminalStream"
 ]
 __name__ = "pyloggermanager.streams"
```

## pyloggermanager/streams/__main__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 import sys
 
 
 class Stream:
     """
     Abstract base class representing an output stream.
     Defines two abstract methods: 'write()' and 'flush()', which must be implemented
```

## pyloggermanager/textstyles/__init__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 __all__ = [
     "TextBackgroundColor",
     "TextColor",
     "TextEffect"
 ]
 __name__ = "pyloggermanager.textstyles"
 __description__ = """
```

## pyloggermanager/textstyles/__main__.py

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2024 coldsofttech
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 class TextBackgroundColor:
     """
     Represents text background color for styling console text.
     Provides methods to add custom colors, retrieve color mappings, get color codes,
     and check if a color is valid.
     """
```

## Comparing `pyloggermanager-0.1.2.dist-info/LICENSE` & `pyloggermanager-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyloggermanager-0.1.2.dist-info/RECORD` & `pyloggermanager-0.1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-pyloggermanager/__init__.py,sha256=afGvLErsiMKM70FmJ8TVwfOvLAEM4KWmWKhx92Z02_w,3421
-pyloggermanager/__main__.py,sha256=jgkznp64DGB4bu7V93Xu9Ai8yIu1_N_QfF9RaKuVWeo,96688
-pyloggermanager/formatters/__init__.py,sha256=sMox9EbaYMUhja6fEqVe0gqAYY-GxdRKfDb0DHmyBEw,2379
-pyloggermanager/formatters/__main__.py,sha256=KcUCBxdI-fSShFFcTRhr1cL8u8MXKeSwQfiwTOxD54A,14809
-pyloggermanager/handlers/__init__.py,sha256=rQrvBEMLLr-PVcePTaLnwthhwSOaKDoGtRCksS-Gbkc,2292
-pyloggermanager/handlers/__main__.py,sha256=q63uDGSIt0lORP8Haind6iT97703xMtgd74o3yZQoZw,20136
-pyloggermanager/streams/__init__.py,sha256=Ky_2xBx5cDNfcNo7R63MMqrdKQC8GXwhM_-DdzstDbM,2413
-pyloggermanager/streams/__main__.py,sha256=A_HPItT2gQcly3P0_h91spcgGWRcHAVd-x6N7rabXqg,4315
-pyloggermanager/textstyles/__init__.py,sha256=ntj7mgiS2QANh0wcw33y-s7wGB07xZb4PJk_c4zI86U,2200
-pyloggermanager/textstyles/__main__.py,sha256=XKDGtV35nr_fRG_8U_w9agwjr_bwntzNicgb8EY938Y,12249
-pyloggermanager-0.1.2.dist-info/LICENSE,sha256=QDd-5ssO5cRVguOaD889uNuqyZlNg2DQS6VjttE-8Dk,1069
-pyloggermanager-0.1.2.dist-info/METADATA,sha256=wN-V34_qxOiqWHr95dYv67A7dpg26Kyl1blIc4AQ0-A,302
-pyloggermanager-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyloggermanager-0.1.2.dist-info/top_level.txt,sha256=427AjoG4-piQ3UJzKdLsUN7od0ylEYhotMppwna1-sQ,16
-pyloggermanager-0.1.2.dist-info/RECORD,,
+pyloggermanager/__init__.py,sha256=fTVDlhD1hzJDBWK4OCHB01gOdWIl9xJ5r_2Jl_1hUrA,2329
+pyloggermanager/__main__.py,sha256=73f6GrAYEHIdbDhHrCAKssU05FhSPBpu9YOF-flIKNk,95596
+pyloggermanager/formatters/__init__.py,sha256=L9GHzxkUHF_wkIIzNNYIFQnq2O1ngXQ672ynB1hR4aY,1287
+pyloggermanager/formatters/__main__.py,sha256=B8Y9O-hapXpkQPuO-_HzciTg7iGYceSKU_t3lXcAVK4,13717
+pyloggermanager/handlers/__init__.py,sha256=yuwSKoswuFsJuD1fTd-40kKFDpkGl_Kc2DI1K4iC31g,1200
+pyloggermanager/handlers/__main__.py,sha256=vkce1d7Aql1LJhN1Wv6HXizQg180m788eORBHXQT6PU,19044
+pyloggermanager/streams/__init__.py,sha256=Iw_CSn7pWt0s76rw_GhGbgEL4acKSh_7u89BNJQoyuI,1321
+pyloggermanager/streams/__main__.py,sha256=SlYG1Vpj_oQiVPGz2rWQpNP20Lv_TlFQlTJ7-ZjRX98,3223
+pyloggermanager/textstyles/__init__.py,sha256=Ma1KEXhSF-7acEjuTKJDzYg1VZQwBuqm94YNyLf2lNQ,1108
+pyloggermanager/textstyles/__main__.py,sha256=1wbOl-ipaJZJfNuQPY9Rha-iLCBwQYJa9viIIN9GoLY,11157
+pyloggermanager-0.1.3.dist-info/LICENSE,sha256=QDd-5ssO5cRVguOaD889uNuqyZlNg2DQS6VjttE-8Dk,1069
+pyloggermanager-0.1.3.dist-info/METADATA,sha256=iY6Hp9MAbK0xx15skuB-Y7cAurJTZWDcOJHQN-4yBXA,54172
+pyloggermanager-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyloggermanager-0.1.3.dist-info/top_level.txt,sha256=427AjoG4-piQ3UJzKdLsUN7od0ylEYhotMppwna1-sQ,16
+pyloggermanager-0.1.3.dist-info/RECORD,,
```

