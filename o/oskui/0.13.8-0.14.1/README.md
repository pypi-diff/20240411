# Comparing `tmp/oskui-0.13.8.tar.gz` & `tmp/oskui-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oskui-0.13.8.tar", last modified: Wed Jan 10 13:46:38 2018, max compression
+gzip compressed data, was "oskui-0.14.1.tar", last modified: Thu Apr 11 07:11:14 2024, max compression
```

## Comparing `oskui-0.13.8.tar` & `oskui-0.14.1.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxr-xr-x   0 vinkoo   (142873)     1029        0 2018-01-10 13:46:38.000000 oskui-0.13.8/
-drwxr-xr-x   0 vinkoo   (142873)     1029        0 2018-01-10 13:46:38.000000 oskui-0.13.8/oskui/
--rw-r--r--   0 vinkoo   (142873)     1029     6346 2017-11-26 17:51:17.000000 oskui-0.13.8/oskui/__init__.py
--rw-r--r--   0 vinkoo   (142873)     1029     2825 2018-01-10 13:41:04.000000 oskui-0.13.8/oskui/visual.py
--rw-r--r--   0 vinkoo   (142873)     1029      319 2018-01-10 13:46:38.000000 oskui-0.13.8/PKG-INFO
--rw-r--r--   0 vinkoo   (142873)     1029       39 2017-11-20 20:02:07.000000 oskui-0.13.8/setup.cfg
--rw-r--r--   0 vinkoo   (142873)     1029      386 2018-01-10 13:42:36.000000 oskui-0.13.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:11:14.643479 oskui-0.14.1/
+-rw-rw-rw-   0        0        0     1083 2024-03-07 07:54:48.000000 oskui-0.14.1/LICENSE
+-rw-rw-rw-   0        0        0      344 2024-04-11 07:11:14.643479 oskui-0.14.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2024-03-07 08:08:34.000000 oskui-0.14.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 07:11:14.629479 oskui-0.14.1/oskui/
+-rw-rw-rw-   0        0        0     7335 2024-03-07 10:21:47.000000 oskui-0.14.1/oskui/__init__.py
+-rw-rw-rw-   0        0        0     3181 2024-03-07 08:01:23.000000 oskui-0.14.1/oskui/visual.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:11:14.642479 oskui-0.14.1/oskui.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-11 07:11:14.000000 oskui-0.14.1/oskui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-11 07:11:14.000000 oskui-0.14.1/oskui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 07:11:14.000000 oskui-0.14.1/oskui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-11 07:11:14.000000 oskui-0.14.1/oskui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-11 07:11:14.645482 oskui-0.14.1/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-03-07 10:29:40.000000 oskui-0.14.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `oskui-0.13.8/oskui/__init__.py` & `oskui-0.14.1/oskui/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,237 +1,228 @@
-'''
-    Collection of custom-made UI functions for command line interface
-'''
-from os import listdir
-from os.path import isfile, join
-from Tkinter import Tk
-from tkFileDialog import askopenfilename, askdirectory
-try:
-    # Win32
-    from msvcrt import getch as getch_win
-
-    def getch():
-        return getch_win()
-except ImportError:
-    # UNIX
-    def getch():
-        import sys
-        import tty
-        import termios
-        fd = sys.stdin.fileno()
-        old = termios.tcgetattr(fd)
-        try:
-            tty.setraw(fd)
-            return sys.stdin.read(1)
-        finally:
-            termios.tcsetattr(fd, termios.TCSADRAIN, old)
-
-
-class bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
-
-def ask_float_int(title, get_int=False):
-    print title
-    user_value = None
-    if get_int:
-        print 'Type integer value, or q for cancel:'
-    else:
-        print 'Type float or integer value, or q for cancel:'
-    while user_value is None:
-        user_value = raw_input()
-        if user_value == 'q':
-            return False
-        elif get_int:
-            try:
-                user_value = int(user_value)
-                if int(user_value) > 0:
-                    break
-            except ValueError:
-                pass
-        else:
-            try:
-                user_value = float(user_value)
-                if float(user_value) > 0:
-                    break
-            except ValueError:
-                pass
-        print 'Incorrect value, plese try again'
-        user_value = None
-
-    return user_value
-
-
-def ask_file(message=None, key_press=True):
-    '''
-    Displays message if given and let's the user to select a file
-    in the file system
-    @params:
-    - message: string, message displayed to the user
-    @output:
-    - path: string, path to the selected file
-    '''
-    if message is not None:
-        print message
-    if key_press:
-        press_any_key('Select a file from your file system.')
-    Tk().withdraw()
-    path = askopenfilename()
-    return path
-
-
-def ask_folder(message=None):
-    '''
-    Displays message if given and let's the user to select a folder
-    on the file system
-    @params:
-    - message: string, message displayed to the user
-    @output:
-    - path: string, path to the selected folder
-    '''
-    if message is not None:
-        print message
-    press_any_key('Select a folder on your file system.')
-    Tk().withdraw()
-    path = askdirectory()
-    return path
-
-
-def choice_menu(menu, title):
-    print title
-    choice = None
-    for ind, option in enumerate(menu):
-        print '%s) %s' % (ind + 1, option)
-    print 'q) Cancel'
-    while choice is None or (
-        choice not in [str(i) for i in range(1, len(menu) + 1)] + ['q']
-    ):
-        if choice is not None:
-            choice = raw_input('Incorrect input. Try again:\n')
-        else:
-            choice = raw_input()
-
-    if choice == 'q':
-        return False
-    else:
-        return int(choice) - 1
-
-
-def get_files(path, full_path=False, filter=None):
-    files = [
-        f for f in listdir(path)
-        if isfile(join(path, f)) and (filter is None or filter in f)]
-    if full_path:
-        files = ["%s/%s" % (path, f) for f in files]
-    return files
-
-
-def get_folders(path):
-    return [f for f in listdir(path) if not isfile(join(path, f))]
-
-
-def toggle(choices, values, title):
-    '''
-    Enables user to toggle between on and off values matching a list of options
-    with pre-defined values. Toggle is based on a color and symbol.
-
-    @params:
-    - choices: list of strings, list of choice names
-    - values: list of integers, list of default choice values, 0 or 1
-    - title: string, instructions to the user
-
-    @output:
-    - values: list of integers, list of returned choice values
-    '''
-
-    valid = [str(i) for i in range(1, len(choices) + 1)]
-    choice = None
-    while choice is None or choice in valid:
-        print title
-        for ind, option in enumerate(choices):
-            if values[ind]:
-                print (
-                    bcolors.OKGREEN +
-                    '%s) %s %s' % (ind + 1, '+', option) +
-                    bcolors.ENDC)
-            else:
-                print '%s) %s %s' % (ind + 1, ' ', option)
-        print 'Any) Done'
-        choice = raw_input()
-
-        if choice in valid:
-            values[int(choice) - 1] = int(not values[int(choice) - 1])
-
-    return values
-
-
-def press_any_key(message=None):
-    '''
-    Displays message if given and waits for user input
-    @params:
-    - message: string, message displayed to the user
-    @output:
-    - key: string, key pressed by the user
-    '''
-    if message is not None:
-        print message
-    print 'Press any key to continue...'
-    return getch()
-
-
-def prompt(message, default=None):
-    choice = None
-    alternatives = ['N', 'n', 'y', 'Y', '0', '1']
-    if default is False:
-        info = '\n[y/N]: '
-    elif default is True:
-        info = '\n[Y/n]: '
-    else:
-        info = '\n[y/n]: '
-
-    if default is not None:
-        alternatives.append('')
-    while choice is None or choice not in alternatives:
-        if choice is not None:
-            print 'Incorrect input. Please try again.'
-        choice = raw_input(message + info)
-    if choice in ['N', 'n', '0']:
-        return False
-    elif choice in ['Y', 'y', '1']:
-        return True
-    else:
-        return default
-
-
-def warn(txt):
-    print (
-        bcolors.WARNING +
-        txt +
-        bcolors.ENDC)
-
-
-def lower_case_name(title, unavailable=[]):
-    name = None
-    while name is None or (
-            sum([0 if c.islower() else 1 for c in name]) != 0) or (
-            len(name) < 3) or name in unavailable:
-        if name is None:
-            name = raw_input(title)
-        elif len(name) < 3:
-            name = raw_input(
-                'Name too short (minimum 3 characters). Try again:\n')
-        elif name in unavailable:
-            name = raw_input((
-                'The name is taken or not available.'
-                ' Please give a different name:\n'))
-        else:
-            name = raw_input((
-                'Invalid name. All characters need to be lower case letters. '
-                'Try again:\n'))
-    return name
+"""
+    Collection of custom-made UI functions for command line interface
+"""
+
+import os
+import sys
+import time
+
+if os.name == 'nt':
+    import msvcrt
+else:
+    import tty
+    import termios
+
+import keyboard
+from tkinter import Tk
+from tkinter.filedialog import askopenfilename, askdirectory
+
+
+# Define getch function for cross-platform compatibility
+def getch():
+    """Get a single character from standard input without echoing to the screen."""
+    if os.name == 'nt':
+        return msvcrt.getch()
+    else:
+        fd = sys.stdin.fileno()
+        old_settings = termios.tcgetattr(fd)
+        try:
+            tty.setraw(fd)
+            ch = sys.stdin.read(1)
+        finally:
+            termios.tcsetattr(fd, termios.TCSADRAIN, old_settings)
+        return ch
+
+
+# Define color codes for terminal output
+class bcolors:
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDC = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
+
+def ask_float_int(title, get_int=False):
+    """
+    Ask the user for a float or integer value.
+
+    :param title: str, the prompt message
+    :param get_int: bool, if True, only accept integer values
+    :return: float|int|bool, the user's input or False if cancelled
+    """
+    print(title)
+    user_value = None
+    while user_value is None:
+        user_input = input(
+            'Type integer value, or q for cancel:' if get_int else 'Type float or integer value, or q for cancel:')
+        if user_input.lower() == 'q':
+            return False
+        try:
+            user_value = int(user_input) if get_int else float(user_input)
+            if user_value > 0:
+                break
+        except ValueError:
+            pass
+        print('Incorrect value, please try again')
+        user_value = None
+    return user_value
+
+
+def ask_file(message=None, key_press=True):
+    """
+    Prompt the user to select a file using a file dialog.
+
+    :param message: str, optional message to display before opening the dialog
+    :param key_press: bool, if True, wait for a key press before showing the dialog
+    :return: str, path to the selected file
+    """
+    if message:
+        print(message)
+    if key_press:
+        press_any_key('Select a file from your file system.')
+    Tk().withdraw()
+    return askopenfilename()
+
+
+def ask_folder(message=None):
+    """
+    Prompt the user to select a folder using a directory dialog.
+
+    :param message: str, optional message to display before opening the dialog
+    :return: str, path to the selected folder
+    """
+    if message:
+        print(message)
+    press_any_key('Select a folder on your file system.')
+    Tk().withdraw()
+    return askdirectory()
+
+
+def choice_menu(menu, title):
+    """
+    Display a menu of choices and prompt the user to make a selection.
+
+    :param menu: list, the list of options to choose from
+    :param title: str, the title of the menu
+    :return: int|bool, the index of the chosen option or False if cancelled
+    """
+    print(title)
+    for ind, option in enumerate(menu):
+        print(f'{ind + 1}) {option}')
+    print('q) Cancel')
+    choice = input()
+    while choice not in [str(i) for i in range(1, len(menu) + 1)] + ['q']:
+        choice = input('Incorrect input. Try again:\n')
+    return False if choice == 'q' else int(choice) - 1
+
+
+def get_files(path, full_path=False, filter=None):
+    """
+    Get a list of files in a directory, optionally filtering by a substring.
+
+    :param path: str, the directory path to search
+    :param full_path: bool, if True, return the full path to the files
+    :param filter: str, optional substring to filter the file names
+    :return: list, the list of file names or paths
+    """
+    files = [f for f in os.listdir(path) if os.path.isfile(os.path.join(path, f)) and (filter is None or filter in f)]
+    return [os.path.join(path, f) for f in files] if full_path else files
+
+
+def get_folders(path):
+    """
+    Get a list of folders in a directory.
+
+    :param path: str, the directory path to search
+    :return: list, the list of folder names
+    """
+    return [f for f in os.listdir(path) if not os.path.isfile(os.path.join(path, f))]
+
+
+def toggle(choices, values, title):
+    """
+    Toggle between on and off values for a list of choices with pre-defined values.
+
+    :param choices: list of str, the choice names
+    :param values: list of int, the default choice values (0 or 1)
+    :param title: str, instructions to the user
+    :return: list of int, the updated choice values
+    """
+    valid = [str(i) for i in range(1, len(choices) + 1)]
+    choice = None
+    while choice is None or choice in valid:
+        print(title)
+        for ind, option in enumerate(choices):
+            color = bcolors.OKGREEN if values[ind] else ''
+            symbol = '+' if values[ind] else ' '
+            print(f'{color}{ind + 1}) {symbol} {option}{bcolors.ENDC}')
+        print('Any) Done')
+        choice = input()
+        if choice in valid:
+            values[int(choice) - 1] = int(not values[int(choice) - 1])
+    return values
+
+
+def press_any_key(message=None):
+    """
+    Display a message and wait for the user to press any key.
+
+    :param message: str, optional message to display
+    :return: str, the key pressed by the user
+    """
+    if message:
+        print(message)
+    print('Press any key to continue...')
+    time.sleep(0.5)
+    return keyboard.read_event().name
+
+
+def prompt(message, default=None):
+    """
+    Prompt the user with a yes/no question.
+
+    :param message: str, the message to display
+    :param default: bool, the default value if the user presses Enter
+    :return: bool, the user's response
+    """
+    alternatives = ['N', 'n', 'y', 'Y', '0', '1']
+    info = '\n[Y/n]: ' if default else '\n[y/N]: ' if default is False else '\n[y/n]: '
+    choice = input(message + info).strip()
+    while choice not in alternatives + ['']:
+        print('Incorrect input. Please try again.')
+        choice = input(message + info).strip()
+    return {'N': False, 'n': False, 'y': True, 'Y': True, '0': False, '1': True}.get(choice, default)
+
+
+def warn(txt):
+    """
+    Print a warning message to the terminal.
+
+    :param txt: str, the text of the warning message
+    """
+    print(f'{bcolors.WARNING}{txt}{bcolors.ENDC}')
+
+
+def lower_case_name(title, unavailable=[]):
+    """
+    Prompt the user for a name that must be lowercase and not in the unavailable list.
+
+    :param title: str, the prompt message
+    :param unavailable: list of str, names that are not allowed
+    :return: str, the chosen name
+    """
+    name = None
+    while True:
+        name = input(title).strip().lower()
+        if len(name) >= 3 and name not in unavailable and name.islower():
+            break
+        elif len(name) < 3:
+            print('Name too short (minimum 3 characters). Try again:')
+        elif name in unavailable:
+            print('The name is taken or not available. Please give a different name:')
+        else:
+            print('Invalid name. All characters need to be lower case letters. Try again:')
+    return name
```

