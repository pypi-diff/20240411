# Comparing `tmp/texnomagic-0.7.0.tar.gz` & `tmp/texnomagic-0.8.0.tar.gz`

## Comparing `texnomagic-0.7.0.tar` & `texnomagic-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/__init__.py
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/abc.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/abcs.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/cli.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/cli_common.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/client.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/common.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/console.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/drawing.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/ex.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/lang.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/model.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/mods.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/requests.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/server.py
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/symbol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/__init__.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/abc.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/drawing.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/mod.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/server.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/spell.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 texnomagic-0.7.0/texnomagic/commands/symbol.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 texnomagic-0.7.0/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 texnomagic-0.7.0/LICENSE
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 texnomagic-0.7.0/README.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 texnomagic-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 texnomagic-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/__init__.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/abc.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/abcs.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/cli.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/cli_common.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/client.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/common.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/console.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/drawing.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/ex.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/jsonrpcserver.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/lang.py
+-rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/model.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/mods.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/render.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/requests.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/server.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/symbol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/__init__.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/abc.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/drawing.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/mod.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/paths.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/server.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/spell.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 texnomagic-0.8.0/texnomagic/commands/symbol.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 texnomagic-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 texnomagic-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 texnomagic-0.8.0/README.md
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 texnomagic-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 texnomagic-0.8.0/PKG-INFO
```

### Comparing `texnomagic-0.7.0/texnomagic/abc.py` & `texnomagic-0.8.0/texnomagic/abc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,149 @@
 import json
 import os
-from pathlib import PurePosixPath
+from pathlib import Path, PurePosixPath
 import random
 import shutil
 
 from texnomagic import common
 from texnomagic.symbol import TexnoMagicSymbol
+from texnomagic.drawing import TexnoMagicDrawing
 
 
 INFO_FILE = 'texno_alphabet.json'
 
 
 class TexnoMagicAlphabet:
+    """
+    TexnoMagic Alphabet is a set of [Symbols][texnomagic.symbol.TexnoMagicSymbol].
+
+    Alphabet has:
+
+    * `name`: arbitrary string
+    * `path`: path to Alphabet dir
+    * `symbols`: a set of Symbols
+
+    This class provides convenient utilities for working with TexnoMagic Alphabets,
+    see individual methods.
+    """
     def __init__(self, path=None, name=None):
         if path and path.name.lower() == INFO_FILE:
             # accept path to alphabet info file as well
             path = path.parent
 
         self.path = path
         self.name = name
         self._symbols = None
 
     @property
-    def info_path(self):
+    def info_path(self) -> Path:
+        f"""Path to Alphabet `{INFO_FILE}` info file."""
         return self.path / INFO_FILE
 
     @property
-    def symbols_path(self):
+    def symbols_path(self) -> Path:
+        """Path to Alphabet `symbols` dir."""
         return self.path / 'symbols'
 
     @property
-    def handle(self):
+    def handle(self) -> str:
+        """Alphabet handle (lowercase string)."""
         return common.name2handle(self.name)
 
     @property
-    def symbols(self):
+    def symbols(self) -> list[TexnoMagicSymbol]:
+        """A list of Symbols in `drawings` dir.
+
+        Lazy loaded on-demand."""
         if self._symbols is None:
             self.load_symbols()
         return self._symbols
 
     def load(self, path=None):
+        f"""Load Alphabet metadata from info file `{INFO_FILE}`."""
         if path:
             self.path = path
 
         assert self.path
         info = json.load(self.info_path.open())
 
         name = info.get('name')
         if not name:
             name = self.path.name
         self.name = name
 
         return self
 
     def load_symbols(self):
+        """Load Symbols from `symbols` dir."""
         self._symbols = []
         for symbol_info_path in self.symbols_path.glob('*/texno_symbol.json'):
             symbol = TexnoMagicSymbol()
             symbol.load(symbol_info_path.parent)
             self._symbols.append(symbol)
         self.sort_symbols()
 
     def sort_symbols(self):
+        """Sort symbols with common ordering."""
         if not self._symbols:
             return
         known = []
         for core_symbol in common.CORE_SYMBOLS_ORDER:
             for symbol in self._symbols:
                 if symbol.meaning == core_symbol:
                     known.append(symbol)
                     self._symbols.remove(symbol)
                     break
         self._symbols = known + self._symbols
 
     def save(self):
+        """Save the Alphabet into path."""
         os.makedirs(self.path, exist_ok=True)
         info = {
             'name': self.name,
         }
         return json.dump(info, self.info_path.open('w'))
 
-    def save_new_symbol(self, symbol):
+    def save_new_symbol(self, symbol : TexnoMagicSymbol):
+        """Save new Symbol into `symbols` dir."""
         assert symbol.name
 
         if self._symbols is None:
             self.load_symbols()
 
         symbol.path = self.symbols_path / common.name2fn(symbol.name)
         symbol.save()
         return self._symbols.insert(0, symbol)
 
     def export(self, out_path=None):
         """
-        export alphabet into a zipfile
+        Export alphabet into a zipfile.
         """
         if not out_path:
             out_path = common.EXPORT_PATH
 
         ar_fn = self.path.name
         out_fn = out_path / ar_fn
         return shutil.make_archive(
             out_fn, 'zip',
             root_dir=self.path.parent,
             base_dir=self.path.name,
         )
 
-    def train_models(self, all=False):
-        """
-        train symbol models with available drawings
+    def normalize(self):
+        """Normalize all Symbols. Overwrites files.
 
-        train only missing models by default, use all to (re-)train all
-        """
+        See [texnomagic.drawing.TexnoMagicDrawing.normalize][]."""
+        for s in self.symbols:
+            s.normalize()
+
+    def train_models(self, all : bool = False):
+        """Train symbol models with available drawings.
+
+        Train only missing models by default, use all to (re-)train all."""
         new, fail, old = [], [], []
         for symbol in self.symbols:
             if all or not symbol.model.ready:
                 if symbol.model.train_symbol(symbol):
                     symbol.model.save()
                     new.append(symbol)
                 else:
@@ -122,37 +151,49 @@
             else:
                 old.append(symbol)
         return new, fail, old
 
     def calibrate(self):
         self.train_models(all=True)
 
-    def scores(self, drawing):
+    def scores(self, drawing : TexnoMagicDrawing, reverse : bool = True) -> list[tuple[TexnoMagicSymbol, float]]:
         """
-        recognize drawing using all symbol models
+        Score a Drawing using all Symbol models.
+
+        Args:
+            drawing: a Symbol Drawing to score
+            reverse: reverse sorting order
 
-        return a list of (symbol, score) tuples ordered by score desc
+        Returns:
+            A list of (symbol, score) tuples ordered by score.
         """
         s = [(symbol, symbol.model.score(drawing)) for symbol in self.symbols]
-        s = sorted(s, key=lambda x: x[1], reverse=True)
+        s = sorted(s, key=lambda x: x[1], reverse=reverse)
         return s
 
-    def recognize(self, drawing):
+    def recognize(self, drawing : TexnoMagicDrawing) -> tuple[TexnoMagicSymbol | None, float]:
+        """
+        Recognize a Drawing within Alphabet Symbols.
+
+        Args:
+            drawing: a Symbol Drawing to recognize
+
+        Returns:
+            (symbol, score) tuple.
+        """
         s = self.scores(drawing)
         if not s:
             return None, -1
         _symbol, score = s[0]
         if score < common.MIN_SCORE:
             return None, score
-        return s
+        return _symbol, score
 
     def check(self):
-        """
-        check alphabet for problems
-        """
+        """Check alphabet for problems."""
         # NOTE: This needs a rewrite into something less ugly.
         warns = dict()
 
         def log_warn(key, val=1.0):
             if key in warns:
                 n, v = warns[key]
                 warns[key] = (n + 1, (v * n + val) / (n + 1))
@@ -166,48 +207,54 @@
                 log_warn(('warn', 'missing_svg', symbol), -1)
             for drawing in symbol.drawings:
                 scores = self.scores(drawing)
                 rsymbol, rscore = scores[0]
                 if rsymbol.meaning != symbol.meaning:
                     log_warn(('error', 'wrong_symbol', symbol, rsymbol), rscore)
                     prob = 'wrong_symbol'
+                if rscore < common.MIN_SCORE:
+                    log_warn(('warn', 'low_score', symbol), rscore)
 
                 for rsy, rsc in scores[1:]:
                     # check scores for other symbols too
                     if rsc > 0.6:
                         lvl = 'warn'
                         if rsc > 0.8:
                             lvl = 'error'
-                        log_warn((lvl,'high_score', symbol, rsy), rsc)
+                        log_warn((lvl, 'high_score', symbol, rsy), rsc)
 
         results = {}
         for (level, prob, *args), (n, score) in warns.items():
             if prob == 'high_score':
                 msg = "%s drawing got high score in %s: %s" % (args[0].meaning, args[1].meaning, score)
+            elif prob == 'low_score':
+                msg = "%s drawing got low score: %s" % (args[0].meaning, score)
             elif prob == 'missing_model':
                 msg = "%s symbol is missing model" % args[0].meaning
             elif prob == 'missing_svg':
                 msg = "%s symbol is missing SVG image" % args[0].meaning
             else:
                 msg = "%s drawing recognized as %s: %s" % (args[0].meaning, args[1].meaning, score)
             if n > 1:
                 msg += "  (x%s)" % n
             if level not in results:
                 results[level] = []
             results[level].append(msg)
 
         return results
 
-    def get_symbol(self, name):
+    def get_symbol(self, name : str) -> TexnoMagicSymbol | None:
+        """Get Symbol by name or meaning."""
         for s in self.symbols:
             if s.name == name or s.meaning == name:
                 return s
         return None
 
-    def random_symbol(self, exclude=None):
+    def random_symbol(self, exclude=None) -> TexnoMagicSymbol | None:
+        """Get a random Symbol from the Alphabet."""
         if exclude:
             symbols = [s for s in self.symbols if s != exclude]
         else:
             symbols = self.symbols
         if len(symbols) < 1:
             return None
         return random.choice(symbols)
@@ -230,35 +277,40 @@
             txt_ref += f"* [{s}](#{s.name}-{s.meaning.lower()})\n"
             txt_body += stxt + '\n'
 
         txt = f"**{len(self.symbols)}** symbols:\n\n{txt_ref}\n{txt_body}"
         return txt.rstrip()
 
     def as_dict(self, symbols=True) -> dict:
+        """Return Alphabet as a dict."""
         d = {
             'name': self.name,
             'handle': self.handle,
             'path': str(self.path),
             'n_symbols': len(self.symbols),
         }
         if symbols:
             d['symbols'] = [s.meaning for s in self.symbols]
         return d
 
     def pretty(self, path=False):
+        """Pretty Alphabet string with colors in rich formatting."""
         s = f'[cyan]{self.name}[/]: [white]{len(self.symbols)}[/] symbols'
         if path:
             s += f' @ [white]{self.path}[/]'
         return s
 
     def __str__(self):
         return f'{self.name}: {len(self.symbols)} symbols'
 
     def __repr__(self):
         return f"<TexnoMagicAlphabet: {self.__str__()}>"
 
 
-def find_alphabet_at_path(path=None):
+def find_alphabet_at_path(path=None) -> TexnoMagicAlphabet:
+    """Find Alphabet at path.
+
+    When path is None, look at current path."""
     info = common.find_file_at_parents(INFO_FILE, path)
     if info:
         return TexnoMagicAlphabet(info)
     return None
```

### Comparing `texnomagic-0.7.0/texnomagic/abcs.py` & `texnomagic-0.8.0/texnomagic/abcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from texnomagic import abc as abc_
 from texnomagic import common
 
 
 class TexnoMagicAlphabets:
     def __init__(self, paths=None):
         self.paths = paths or common.ALPHABETS_PATHS
-        self.abcs = {}
+        self._abcs = None
+
+    @property
+    def abcs(self):
+        if self._abcs is None:
+            self.load()
+        return self._abcs
 
     def load(self):
-        self.abcs = {}
+        self._abcs = {}
         for tag, path in self.paths.items():
-            self.abcs[tag] = get_alphabets(path)
+            self._abcs[tag] = get_alphabets(path)
 
     def get_alphabet(self, name):
         tag, _, abc_name = name.rpartition(':')
         for tag_, abcs in self.abcs.items():
             if tag and tag != tag_:
                 continue
             for abc in abcs:
```

### Comparing `texnomagic-0.7.0/texnomagic/cli.py` & `texnomagic-0.8.0/texnomagic/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,31 +7,40 @@
 import sys
 
 import click
 
 from texnomagic import __version__
 from texnomagic import commands
 from texnomagic import ex
+from texnomagic import console as console_mod
 
 
 log = logging.getLogger(__name__)
 
 
+COLOR_SYSTEMS = ['auto', 'none', 'standard', '256', 'truecolor', 'windows']
 CONTEXT_SETTINGS = {
     'help_option_names': ['-h', '--help'],
 }
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.version_option(__version__, message='%(version)s',
                       help="Show TexnoMagic version and exit.")
-def cli():
+@click.option('-C', '--color', default='auto', show_default=True,
+              type=click.Choice(COLOR_SYSTEMS),
+              help="Set color mode.")
+def cli(color):
     """
     TexnoMagic CLI
     """
+    if color == 'none':
+        console_mod.console = console_mod.Console(color_system=None)
+    elif color != 'auto':
+        console_mod.console = console_mod.Console(color_system=color)
 
 
 def __load_commands():
     """
     load available texnomagic commands
 
     should only be called once on module load
```

### Comparing `texnomagic-0.7.0/texnomagic/cli_common.py` & `texnomagic-0.8.0/texnomagic/cli_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 
 from texnomagic.abcs import TexnoMagicAlphabets
 from texnomagic.abc import find_alphabet_at_path
 from texnomagic.symbol import find_symbol_at_path
 from texnomagic.drawing import TexnoMagicDrawing
-from texnomagic.console import console
+from texnomagic import console
 from texnomagic import common
 from texnomagic import ex
 
 
 OUTPUT_FORMATS = ['text'] + common.DUMP_FORMATS
 OUTPUT_FORMAT_DEFAULT = 'text'
 
 
-def get_alphabet_of_fail(abc):
+def get_alphabet_or_fail(abc, auto_load=True):
     alphabet = None
     if abc:
         abcs = TexnoMagicAlphabets()
         abcs.load()
         alphabet = abcs.get_alphabet(abc)
         if not alphabet:
             console.print(f"[yellow]TexnoMagic alphabet not found[/]: [cyan]{abc}[/]")
@@ -27,38 +27,45 @@
         if not alphabet:
             console.print("[yellow]No TexnoMagic alphabet found at current path.[/]\n")
             print("You can:\n")
             print("- run from a (sub-)directory of a TexnoMagic alphabet")
             print("- select TexnoMagic alphabet by name using an argument")
             raise ex.AlphabetNotFound()
 
+    if auto_load:
+        alphabet.load()
+
     return alphabet
 
 
-def get_symbol_or_fail(symbol):
+def get_symbol_or_fail(symbol, auto_load=True):
     _symbol = None
     if symbol:
         abc_name, _, symbol_name = symbol.rpartition('/')
         if not abc_name:
             console.print(f"[red]Inavlid symbol spec[/]: [green]{symbol}[/]")
             console.print("\nPlease use ALPHABET/SYMBOL format.")
             raise ex.InvalidInput(symbol)
-        _abc = get_alphabet_of_fail(abc_name)
+        _abc = get_alphabet_or_fail(abc_name)
         _symbol = _abc.get_symbol(symbol_name)
         if not _symbol:
             console.print(f"[yellow]TexnoMagic symbol not found[/]: [green]{symbol}[/]")
             raise ex.SymbolNotFound(symbol)
     else:
         _symbol = find_symbol_at_path()
         if not _symbol:
             console.print("[yellow]No TexnoMagic symbol found at current path.[/]\n")
             print("You can:\n")
             print("- run from a (sub-)directory of a TexnoMagic symbol")
             print("- select TexnoMagic symbol by name passing ALPHABET/SYMBOL argument")
             raise ex.SymbolNotFound()
+
+    if auto_load:
+        _symbol.load()
+
     return _symbol
 
 
 def print_drawings(drawings, stats=True):
     n_points = 0
     n_curves = 0
     n_bytes = 0
```

### Comparing `texnomagic-0.7.0/texnomagic/client.py` & `texnomagic-0.8.0/texnomagic/client.py`

 * *Files identical despite different names*

### Comparing `texnomagic-0.7.0/texnomagic/common.py` & `texnomagic-0.8.0/texnomagic/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import os
 from pathlib import Path
 import re
 
 from rich.syntax import Syntax
 
-from texnomagic.console import console
+from texnomagic import console
 
 
 DUMP_FORMATS = ['toml', 'yaml', 'json']
 DUMP_FORMAT_DEFAULT = 'toml'
 
 IMAGE_FORMATS = ['svg', 'png']
 IMAGE_FORMAT_DEFAULT = 'svg'
```

### Comparing `texnomagic-0.7.0/texnomagic/ex.py` & `texnomagic-0.8.0/texnomagic/ex.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,7 +28,11 @@
 
 class SymbolNotFound(TexnoMagicException):
     returncode = 32
 
 
 class DrawingNotFound(TexnoMagicException):
     returncode = 33
+
+
+class ModuleNotAvailable(TexnoMagicException):
+    returncode = 50
```

### Comparing `texnomagic-0.7.0/texnomagic/lang.py` & `texnomagic-0.8.0/texnomagic/lang.py`

 * *Files identical despite different names*

### Comparing `texnomagic-0.7.0/texnomagic/mods.py` & `texnomagic-0.8.0/texnomagic/mods.py`

 * *Files identical despite different names*

### Comparing `texnomagic-0.7.0/texnomagic/requests.py` & `texnomagic-0.8.0/texnomagic/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 TexnoMagic RPC handling logic
 
 Individual functions in this module marked with @jsonrpcserver.method decorator
 are used for Remote Procedure Calls (RPC) by the TexnoMagic server.
 """
-from jsonrpcserver import method, Success
+from texnomagic.jsonrpcserver import method, Success
 
 from texnomagic import __version__
 from texnomagic.drawing import TexnoMagicDrawing
 from texnomagic import mods
 
 
 @method
```

### Comparing `texnomagic-0.7.0/texnomagic/server.py` & `texnomagic-0.8.0/texnomagic/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Please see `client.py` for a reference implementation of a client.
 """
 import logging
 import socketserver
 import sys
 
-from jsonrpcserver import dispatch
+from texnomagic.jsonrpcserver import dispatch, ensure_jsonrpcserver
 
 from texnomagic import __version__
 from texnomagic import common
 from texnomagic.abcs import TexnoMagicAlphabets
 from texnomagic.lang import TexnoMagicLanguage
 # must be loaded in order for jsonrpc.dispatch() to work
 from texnomagic import requests  # noqa
@@ -33,14 +33,16 @@
 DEFAULT_PORT = 6969
 
 
 def serve(host='localhost', port=DEFAULT_PORT, abcs=None):
     """
     start TexnoMagic TCP server and serve forever
     """
+    ensure_jsonrpcserver()
+
     logging.info("START TexnoMagic TCP server %s on %s:%s ..." % (__version__, host, port))
     if not abcs:
         abcs = TexnoMagicAlphabets()
         abcs.load()
 
     with socketserver.TCPServer((host, port), TexnoMagicTCPHandler) as server:
         server.context = {
```

### Comparing `texnomagic-0.7.0/texnomagic/commands/abc.py` & `texnomagic-0.8.0/texnomagic/commands/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
 from texnomagic.abcs import TexnoMagicAlphabets
-from texnomagic.console import console
+from texnomagic import console
 from texnomagic import common
 from texnomagic import cli_common
 
 
 @click.group()
 @click.help_option('-h', '--help', help='Show command help.')
 def abc():
@@ -24,16 +24,16 @@
     """
     Show details of a TexnoMagic alphabet.
 
     By default, tries to detect alphabet from current directory.
 
     Select a specific alphabet by passing its name or handle as argument.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
-    alphabet.load()
+    alphabet = cli_common.get_alphabet_or_fail(abc)
+
     common.pretty_print(alphabet.as_dict(), format)
 
 
 @abc.command()
 @click.argument('abc', nargs=-1)
 @click.option('-t', '--tag',
               default=[], show_default=True,
@@ -103,35 +103,45 @@
 
 @abc.command()
 @click.argument('abc', required=False)
 def check(abc):
     """
     Check alphabet for issues.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
-    alphabet.load()
+    alphabet = cli_common.get_alphabet_or_fail(abc)
 
     console.print(f"[green]CHECK[/] alphabet: {alphabet.pretty(path=True)}")
     r = alphabet.check()
     for level, msgs in sorted(r.items()):
         for msg in msgs:
             print("%s: %s" % (level.upper(), msg))
     return 0
 
 
 @abc.command()
 @click.argument('abc', required=False)
+def normalize(abc):
+    """
+    Normalize alphabet symbols.
+    """
+    alphabet = cli_common.get_alphabet_or_fail(abc)
+
+    console.print(f"[green]NORMALIZE[/] alphabet: {alphabet.pretty(path=True)}")
+    alphabet.normalize()
+
+
+@abc.command()
+@click.argument('abc', required=False)
 @click.option('-a', '--all', is_flag=True,
               help="Re-train all models.  [default: only missing]")
 def train(abc, all):
     """
     Train (missing) models for alphabet.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
-    alphabet.load()
+    alphabet = cli_common.get_alphabet_or_fail(abc)
 
     console.print(f"[green]TRAIN[/] alphabet models: {alphabet.pretty(path=True)}")
     new, fail, old = alphabet.train_models(all=all)
     if new:
         console.print("[green]TRAIN[/] %s symbol models: %s" % (len(new), ", ".join([s.meaning for s in new])))
     if fail:
         console.print("[red]FAIL[/] %s symbol models: %s" % (len(fail), ", ".join([s.meaning for s in fail])))
@@ -143,28 +153,26 @@
 @click.argument('abc', required=False)
 @click.option('-h', '--heading', type=int, default=3, show_default=True,
               help="Heading level.")
 def readme(abc, heading):
     """
     Generate Markdown symbols list for alphabet README.md.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
-    alphabet.load()
+    alphabet = cli_common.get_alphabet_or_fail(abc)
 
     print(alphabet.gen_readme_md(heading=heading))
 
 
 @abc.command()
 @click.argument('abc', required=False)
 def flip_y(abc):
     """
     Flip Y axis for all symbols in alphabet.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
-    alphabet.load()
+    alphabet = cli_common.get_alphabet_or_fail(abc)
 
     console.print(f"[yellow]FLIP Y[/] alphabet: {alphabet.pretty(path=True)}")
     for symbol in alphabet.symbols:
         console.print(f"[yellow]FLIP Y[/] symbol: {symbol.pretty()}")
         for drawing in symbol.drawings:
             drawing.load_curves()
             drawing.flip_y_axis()
```

### Comparing `texnomagic-0.7.0/texnomagic/commands/mod.py` & `texnomagic-0.8.0/texnomagic/commands/mod.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 
 from texnomagic import common
 from texnomagic import mods
-from texnomagic.console import console
+from texnomagic import console
 from texnomagic import cli_common
 
 
 @click.group()
 @click.help_option('-h', '--help', help='Show command help.')
 def mod():
     """
```

### Comparing `texnomagic-0.7.0/texnomagic/commands/spell.py` & `texnomagic-0.8.0/texnomagic/commands/spell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 from rich.syntax import Syntax
 
 from texnomagic import common
-from texnomagic.console import console
+from texnomagic import console
 from texnomagic import lang
 
 
 @click.group(name='spell')
 @click.help_option('-h', '--help', help='Show command help.')
 def spell():
     """
```

### Comparing `texnomagic-0.7.0/texnomagic/commands/symbol.py` & `texnomagic-0.8.0/texnomagic/commands/symbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 from rich.prompt import Prompt
 
-from texnomagic.console import console
+from texnomagic import console
 from texnomagic import common
 from texnomagic import cli_common
 from texnomagic import ex
 from texnomagic.symbol import TexnoMagicSymbol
 
 
 @click.group()
@@ -49,15 +49,15 @@
     """
     List all symbols in a TexnoMagic alphabet.
 
     By default, tries to detect alphabet from current directory.
 
     Select a specific alphabet by passing its name or handle as argument.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
+    alphabet = cli_common.get_alphabet_or_fail(abc)
     alphabet.load()
 
     # are we outputting data or text?
     data_out = not names and not meanings and format != 'text'
 
     # list the filtered alphabets
 
@@ -99,15 +99,15 @@
     """
     Create a new TexnoMagic symbol.
 
     By default, tries to detect alphabet from current directory.
 
     Select a specific alphabet by passing its name or handle as argument.
     """
-    alphabet = cli_common.get_alphabet_of_fail(abc)
+    alphabet = cli_common.get_alphabet_or_fail(abc)
 
     if not (meaning or name):
         meaning = Prompt.ask("Symbol Meaning (lowercase english)")
         name = Prompt.ask("Symbol Name (any string)")
         print()
         if not (meaning or name):
             console.print("[red]ERROR[/]: symbol meaning or name is required")
@@ -120,8 +120,19 @@
     meaning = common.name2handle(meaning)
 
     symbol = TexnoMagicSymbol(meaning=meaning, name=name)
     alphabet.save_new_symbol(symbol)
     console.print(f"SAVED NEW symbol {symbol.pretty(path=True)}")
 
 
+@symbol.command()
+@click.argument('symbol', required=False)
+def normalize(symbol):
+    """
+    Normalize drawings of selected TexnoMagic symbol.
+    """
+    _symbol = cli_common.get_symbol_or_fail(symbol)
+    console.print(f"[green]NORMALIZING[/] symbol: {_symbol.pretty(drawings=True)}")
+    _symbol.normalize()
+
+
 TEXNOMAGIC_CLI_COMMANDS = [symbol]
```

### Comparing `texnomagic-0.7.0/LICENSE` & `texnomagic-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texnomagic-0.7.0/README.md` & `texnomagic-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `texnomagic-0.7.0/pyproject.toml` & `texnomagic-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -14,23 +14,30 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "click",
-    "jsonrpcserver >= 5",
     "parsimonious",
     "pyyaml",
     "requests",
     "rich",
     "scikit-learn",
     "toml",
 ]
 
+[project.optional-dependencies]
+png = [
+    "pillow"
+]
+jsonrpc = [
+    "jsonrpcserver >= 5"
+]
+
 [project.scripts]
 texnomagic = "texnomagic.cli:main"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/texnoforge/texnomagic/issues"
 Docs = "https://texnoforge.github.io/texnomagic"
 Homepage = "https://github.com/texnoforge/texnomagic/"
```

### Comparing `texnomagic-0.7.0/PKG-INFO` & `texnomagic-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: texnomagic
-Version: 0.7.0
+Version: 0.8.0
 Summary: TexnoMagic module for digital Magic
 Project-URL: Bug Tracker, https://github.com/texnoforge/texnomagic/issues
 Project-URL: Docs, https://texnoforge.github.io/texnomagic
 Project-URL: Homepage, https://github.com/texnoforge/texnomagic/
 Author-email: texnoforge <voice@texnoforge.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: click
-Requires-Dist: jsonrpcserver>=5
 Requires-Dist: parsimonious
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: scikit-learn
 Requires-Dist: toml
+Provides-Extra: jsonrpc
+Requires-Dist: jsonrpcserver>=5; extra == 'jsonrpc'
+Provides-Extra: png
+Requires-Dist: pillow; extra == 'png'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/texnoforge/texnomagic/releases" alt="latest release"><img src="https://img.shields.io/github/v/release/texnoforge/texnomagic"/></a>
 <a href="https://pypi.org/project/texnomagic/" alt="PyPI version"><img src="https://img.shields.io/pypi/v/texnomagic?color=blue"/></a>
 <br>
 <a href="https://github.com/texnoforge/texnomagic/actions/workflows/python-package.yml"><img alt="Python CI Status" src="https://github.com/texnoforge/texnomagic/actions/workflows/python-package.yml/badge.svg"></a>
 <a href="https://github.com/texnoforge/texnomagic/actions/workflows/deploy-docs.yml"><img alt="Docs Status" src="https://github.com/texnoforge/texnomagic/actions/workflows/deploy-docs.yml/badge.svg"></a>
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: texnomagic Version: 0.7.0 Summary: TexnoMagic
+Metadata-Version: 2.3 Name: texnomagic Version: 0.8.0 Summary: TexnoMagic
 module for digital Magic Project-URL: Bug Tracker, https://github.com/
 texnoforge/texnomagic/issues Project-URL: Docs, https://texnoforge.github.io/
 texnomagic Project-URL: Homepage, https://github.com/texnoforge/texnomagic/
 Author-email: texnoforge
 texnoforge.dev> License-Expression: MIT License-File: LICENSE Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Requires-Dist:
-click Requires-Dist: jsonrpcserver>=5 Requires-Dist: parsimonious Requires-
-Dist: pyyaml Requires-Dist: requests Requires-Dist: rich Requires-Dist: scikit-
-learn Requires-Dist: toml Description-Content-Type: text/markdown_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_t_e_x_n_o_f_o_r_g_e_/_t_e_x_n_o_m_a_g_i_c_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_p_y_p_i_/_v_/_t_e_x_n_o_m_a_g_i_c_?_c_o_l_o_r_=_b_l_u_e_]
+click Requires-Dist: parsimonious Requires-Dist: pyyaml Requires-Dist: requests
+Requires-Dist: rich Requires-Dist: scikit-learn Requires-Dist: toml Provides-
+Extra: jsonrpc Requires-Dist: jsonrpcserver>=5; extra == 'jsonrpc' Provides-
+Extra: png Requires-Dist: pillow; extra == 'png' Description-Content-Type:
+text/markdown_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_t_e_x_n_o_f_o_r_g_e_/_t_e_x_n_o_m_a_g_i_c_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_e_x_n_o_m_a_g_i_c_?_c_o_l_o_r_=_b_l_u_e_]
 _[_P_y_t_h_o_n_ _C_I_ _S_t_a_t_u_s_]_[_D_o_c_s_ _S_t_a_t_u_s_]
 # [TexnoMagic docs online][docs] ## [TexnoMagic docs on GitLab](https://
 github.com/texnoforge/texnomagic/tree/master/docs) ## TexnoMagic docs offline
 See docs/index.md and other files in docs/ directory. You can also render docs
 into HTML using MkDocs: pip install mkdocs-material mkdocs build # see site/
 index.html #### read the [docs] and have a nice magic á( á )á [docs]:
 http://texnoforge.github.io/texnomagic
```

