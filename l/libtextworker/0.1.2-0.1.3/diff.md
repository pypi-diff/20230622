# Comparing `tmp/libtextworker-0.1.2.tar.gz` & `tmp/libtextworker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtextworker-0.1.2.tar", max compression
+gzip compressed data, was "libtextworker-0.1.3.tar", max compression
```

## Comparing `libtextworker-0.1.2.tar` & `libtextworker-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1631 2023-04-20 13:54:08.893198 libtextworker-0.1.2/libtextworker/__init__.py
--rw-r--r--   0        0        0      491 2023-04-20 11:12:58.566224 libtextworker-0.1.2/libtextworker/_importer.py
--rw-r--r--   0        0        0     3414 2023-04-20 11:12:43.928208 libtextworker-0.1.2/libtextworker/general.py
--rw-r--r--   0        0        0     6256 2023-04-20 11:48:14.234327 libtextworker-0.1.2/libtextworker/get_config.py
--rw-r--r--   0        0        0        0 2023-04-20 11:12:43.929209 libtextworker-0.1.2/libtextworker/interface/__init__.py
--rw-r--r--   0        0        0     7655 2023-04-20 14:33:23.438003 libtextworker-0.1.2/libtextworker/interface/manager.py
--rw-r--r--   0        0        0     3192 2023-04-20 11:12:58.568226 libtextworker-0.1.2/libtextworker/interface/tk/__init__.py
--rw-r--r--   0        0        0     3988 2023-04-20 11:12:58.569224 libtextworker-0.1.2/libtextworker/interface/tk/editor.py
--rw-r--r--   0        0        0     1956 2023-04-20 14:33:23.322004 libtextworker-0.1.2/libtextworker/interface/tk/miscs.py
--rw-r--r--   0        0        0     1432 2023-04-20 14:33:23.328002 libtextworker-0.1.2/libtextworker/interface/wx/__init__.py
--rw-r--r--   0        0        0     2776 2023-04-22 13:26:35.375215 libtextworker-0.1.2/libtextworker/interface/wx/about.py
--rw-r--r--   0        0        0      447 2023-04-20 11:12:43.934208 libtextworker-0.1.2/libtextworker/interface/wx/constants.py
--rw-r--r--   0        0        0     5304 2023-04-21 07:05:10.999353 libtextworker-0.1.2/libtextworker/interface/wx/editor.py
--rw-r--r--   0        0        0     2462 2023-04-20 11:12:43.936208 libtextworker-0.1.2/libtextworker/interface/wx/miscs.py
--rw-r--r--   0        0        0    35182 2023-04-22 13:23:35.882821 libtextworker-0.1.2/libtextworker/licenses/AGPL_full.txt
--rw-r--r--   0        0        0      684 2023-04-22 13:21:40.443192 libtextworker-0.1.2/libtextworker/licenses/AGPL_short.txt
--rw-r--r--   0        0        0    35149 2023-04-20 11:12:43.937207 libtextworker-0.1.2/libtextworker/licenses/GPL3_full.txt
--rw-r--r--   0        0        0      615 2023-04-20 11:12:43.938208 libtextworker-0.1.2/libtextworker/licenses/GPL3_short.txt
--rw-r--r--   0        0        0     7815 2023-04-22 13:20:16.073381 libtextworker-0.1.2/libtextworker/licenses/LGPL_3.txt
--rw-r--r--   0        0        0     1022 2023-04-20 11:12:43.938208 libtextworker-0.1.2/libtextworker/licenses/MIT.txt
--rw-r--r--   0        0        0     2711 2023-04-20 11:12:43.939207 libtextworker-0.1.2/libtextworker/versioning.py
--rw-r--r--   0        0        0    35149 2023-04-20 11:12:43.922208 libtextworker-0.1.2/LICENSE
--rw-r--r--   0        0        0      928 2023-04-20 11:44:44.226449 libtextworker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      307 2023-04-22 14:49:50.996391 libtextworker-0.1.2/README.md
--rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 libtextworker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 04:09:08.590361 libtextworker-0.1.3/LICENSE
+-rw-r--r--   0        0        0      635 2023-06-22 04:09:08.590361 libtextworker-0.1.3/README.md
+-rw-r--r--   0        0        0     1171 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/__init__.py
+-rw-r--r--   0        0        0      448 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/_importer.py
+-rw-r--r--   0        0        0     5239 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/general.py
+-rw-r--r--   0        0        0     9317 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/get_config.py
+-rw-r--r--   0        0        0        0 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/__init__.py
+-rw-r--r--   0        0        0      235 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/_colors.py
+-rw-r--r--   0        0        0     7949 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/manager.py
+-rw-r--r--   0        0        0     3149 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/tk/__init__.py
+-rw-r--r--   0        0        0     5519 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/tk/editor.py
+-rw-r--r--   0        0        0     1826 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/tk/miscs.py
+-rw-r--r--   0        0        0     1423 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/wx/__init__.py
+-rw-r--r--   0        0        0     2690 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/wx/about.py
+-rw-r--r--   0        0        0      638 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/wx/constants.py
+-rw-r--r--   0        0        0     2730 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/wx/dirctrl.py
+-rw-r--r--   0        0        0     6271 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/wx/editor.py
+-rw-r--r--   0        0        0     3751 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/interface/wx/miscs.py
+-rw-r--r--   0        0        0    35182 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/licenses/AGPL_full.txt
+-rw-r--r--   0        0        0      684 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/licenses/AGPL_short.txt
+-rw-r--r--   0        0        0    35149 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/licenses/GPL3_full.txt
+-rw-r--r--   0        0        0      615 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/licenses/GPL3_short.txt
+-rw-r--r--   0        0        0     7815 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/licenses/LGPL_3.txt
+-rw-r--r--   0        0        0     1022 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/licenses/MIT.txt
+-rw-r--r--   0        0        0     2753 2023-06-22 04:09:08.597028 libtextworker-0.1.3/libtextworker/versioning.py
+-rw-r--r--   0        0        0     1120 2023-06-22 04:09:08.597028 libtextworker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 libtextworker-0.1.3/PKG-INFO
```

### Comparing `libtextworker-0.1.2/libtextworker/get_config.py` & `libtextworker-0.1.3/libtextworker/get_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,101 @@
-import configparser
+"""
+@package libtextworker.get_config
+@brief Contains classes for generic INI files parsing
+@since 0.1.3: Use CommentedConfigParser, but don't replace ConfigParser with it.
+"""
 import os
-import os.path
+import typing
 
-from .general import WalkCreation, libTewException
+from .general import WalkCreation, libTewException, logger
 
 __all__ = ["ConfigurationError", "GetConfig"]
 
+try:
+    from commentedconfigparser import CommentedConfigParser as ConfigParser
+except ImportError:
+    from configparser import ConfigParser
+
 
 class ConfigurationError(libTewException):
     def __init__(self, section: str = "", option: str = "", msg: str = ""):
         prefix = "Error in the configuration file: "
         if not msg:
-            msg = "*UNKNOW ERROR*"
+            msg = "*Unknown*"
         else:
             msg = "[{}->{}] : {}".format(
                 section,
                 "(None)" if option == "" else option,
                 "No Message" if msg == "" else msg,
             )
         full = prefix + msg
         super().__init__(full)
 
 
-class GetConfig(configparser.ConfigParser):
+class GetConfig(ConfigParser):
     # Values
-    yes_values: list = ["yes", "True"]
-    no_values: list = ["no", "False"]
+    yes_values: list = ["yes", "True", True]
+    no_values: list = ["no", "False", False]
 
     returnbool: bool = True
     aliases = {}
     detailedlogs: bool = True
     backups = {}
 
-    def __init__(self, config: dict, file: str, **kwds):
+    for item in yes_values:
+        aliases[item] = True
+
+    for item in no_values:
+        aliases[item] = False
+
+    def __init__(self, config: dict[str] | str, file: str, **kwds):
         """
         A customized INI file parser.
-        @param config : Default configurations, used to reset the file or do some comparisions
+        @param config (dict[str] or str) : Default configurations, used to reset the file or do some comparisions
         @param file : Configuration file
         @param **kwds : To pass to configparser.ConfigParser (base class)
 
         When initialized, GetConfig loads all default configs (from config param) and store it in
         a dictionary for further actions (backup/restore file).
+
+        @since 0.1.3: Allow config parameter as a str object
         """
         super().__init__(**kwds)
 
         self.cfg = {}
 
-        for key in config:
-            self[key] = config[key]
-            self.cfg[key] = config[key]
+        if isinstance(config, str):
+            self.read_string(config)
+        else:
+            self.read_dict(config)
+
+        for key in self:
+            self.cfg[key] = self[key]
 
         self.readf(file)
         self.__file = file
 
     # File tasks
     def readf(self, file: str, encoding: str | None = None):
-        if os.path.isfile(file):
-            self.read(file, encoding)
-        else:
+        if not os.path.isfile(file):
             firstdir = os.path.dirname(file)
             WalkCreation(firstdir)
             with open(file, mode="w") as f:
                 try:
                     self.write(f)
                 except OSError:
                     raise Exception("Unable to access to the file name %s" % file)
-                else:
-                    self.read(file, encoding)
-        self.__file = file  # Should I?
+        self.read(file, encoding)
+        self.__file = file
 
     def reset(self, restore: bool = False) -> bool:
         try:
             os.remove(self.__file)
-        except:
+        except OSError as e:
+            logger.error(e)
             return False
         else:
             for key in self.cfg:
                 self[key] = self.cfg[key]
 
             if restore and self.backups:
                 for key in self.backups:
@@ -110,28 +129,25 @@
     def getkey(
         self,
         section: str,
         option: str,
         needed: bool = False,
         restore: bool = False,
         noraiseexp: bool = False,
-        getbool: bool = returnbool,
-    ) -> str | bool:
+        raw: bool = False,
+    ) -> typing.Any:
         """
         Try to get the value of an option under the spectified section.
+        @version Updated (parameters) on 0.1.3
 
-        If the option does not exist and needed parameter is set to True,
-        GetConfig will add that option automatically with the value based on
-        its previously initialized configs. If restore parameter is set to True,
-        GetConfig will use the backed up option, if possible.
-
-        If you don't want to see exceptions raised and just need False (when something went wrong),
-        set noraiseexp to True.
-
-        Otherwise it will check for the value's alias, then return the value.
+        @param section, option: Target section->option
+        @param needed (boolean=False): The target option is needed - should use with restore & noraiseexp
+        @param restore (boolean=False): Create the option if it is not found from the search
+        @param noraiseexp (boolean=False): Whetever to raise an Exception if something went wrong (default getkey will)
+        @param raw (boolean=False): Don't use aliases for the value we get.
         """
         if not self.has_section(section):
             if needed == True:
                 self.add_section(section)
             else:
                 if noraiseexp != True:
                     raise ConfigurationError(
@@ -147,37 +163,113 @@
                         section,
                         option,
                         self.backups[section][option]
                         if option in self.backups[section]
                         else self.cfg[section][option],
                     )
                 else:
-                    self.set(section, option, self[section][option])
+                    self.set_and_update(section, option, self[section][option])
             else:
                 if noraiseexp != True:
                     raise ConfigurationError(
                         section, option, "Option not found: %s" % option
                     )
                 else:
                     return False
 
-        if needed == True:
-            self.update()
-
         value = self.get(section, option)
 
-        return value if value not in self.aliases else self.aliases[value]
+        if raw or not value in self.aliases:
+            return value
+        else:
+            return self.aliases[value]
 
     def aliasyesno(self, yesvalue, novalue, enable: bool = True) -> None:
-        """
-        Use a custom yes/no value, for example:
-        There is an option under [section], and GetConfig will return
-        True if the options is 'yes', False if the options is 'no'.
-        You can change 'yes' and 'no' value for your use.
-        If you dont want the parser return a boolean, set enable to false.
-        """
         self.yes_values.append(yesvalue)
         self.no_values.append(novalue)
         self.returnbool = enable
 
     def alias(self, value, value2) -> None:
         self.aliases[value] = value2
+
+    def move(
+        self, list_: dict[str, dict[str, str]], delete_entire_section: bool = False
+    ) -> None:
+        """
+        @since 0.1.3
+
+        Move configurations found from the file that GetConfig currently uses.
+        Below is an example:
+        ```
+        move(
+            list_={
+                "section1->option1": {
+                    "newpath": "section_one->option1",
+                    "file": "unchanged"
+                },
+                "special->option0": {
+                    "newpath": "special_thing->option0",
+                    "file": "~/.config/test.ini"
+                }
+            }
+        )
+        ```
+
+        ```list_``` parameter holds all configs to move. Each of options specified (section->option format)
+        'is' a dictionary: sub-key 'newpath' specifies the location of the option to moved to (section->option format), 'file'
+        specifies the new file to use (if needed, else use 'unchanged' or leave blank).
+        This function won't use backup(). Non-exist things will be ignored silently.
+
+        If you use delete_entire_section, this func will REMOVE ALL sections found on the move. Only for ['file'] == 'unchanged'.
+        """
+        curr_sects = self.sections()
+        newfile = ConfigParser()
+
+        for item in list_:
+            # Split and get values
+            splits = item.split("->")
+            if not splits[0] in curr_sects:
+                break
+
+            value = self.get(splits[0], splits[1])
+            target = list_[item]["newpath"].split("->")
+
+            if "file" not in list_[item]:
+                target_file = "unchanged"
+            else:
+                target_file = list_[item]["file"]
+
+            # Start the move
+            if target_file == "unchanged":
+                if not target[0] in self.sections():
+                    self.add_section(target[0])
+
+                self.set(target[0], target[1], value)
+
+                if not delete_entire_section:
+                    self.remove_option(splits[0], splits[1])
+                else:
+                    self.remove_section(splits[0])
+
+                self.update()
+
+            else:
+                if os.path.isfile(target_file):
+                    newfile.read(target_file)
+
+                if not target[0] in newfile.sections():
+                    newfile.add_section(target[0])
+
+                newfile.set(target[0], target[1], value)
+
+                with open(target_file, "w") as f:
+                    newfile.write(f)
+
+    def set_and_update(
+        self, section: str, option: str, value: str | None = None
+    ) -> None:
+        """
+        @since 0.1.3
+        Set an option, and eventually apply it to the file.
+        """
+        self.set(section, option, value)
+        self.update()
```

### Comparing `libtextworker-0.1.2/libtextworker/interface/manager.py` & `libtextworker-0.1.3/libtextworker/interface/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import typing
 import threading
 
-import darkdetect
+try:
+    import darkdetect
+except ImportError:
+    AUTOCOLOR = False
+else:
+    AUTOCOLOR = True
+
 from PIL import ImageColor
 
 from .. import THEMES_DIR
-from ..general import libTewException, CraftItems
+from ..general import logger, libTewException, CraftItems
 from ..get_config import ConfigurationError, GetConfig
 
 """
 Default UI configurations
 """
 default_configs = {
     "color": {"background": "light", "autocolor": "yes", "textcolor": "default"},
@@ -21,24 +27,24 @@
     },
 }
 
 
 class ColorManager(GetConfig):
     """
     A color manager for GUI widgets.
-    ColorManager reads configs from a file (default is under THEMES_DIR)
+    ColorManager can be used for multiple GUI widgets with only one call
     """
 
     setcolorfn = {}
     setfontfn = {}
     threads = {}
 
     def __init__(
         self,
-        default_configs: dict[str, typing.Any],
+        default_configs: dict[str, typing.Any] = default_configs,
         customfilepath: str or bool = False,
     ):
         """
         Constructor of the class.
         @param default_configs (dict[str, Any]): Defaults to default_configs, this is dev-made configs
         @param customfilepath (str|bool): Custom file path support. Set to False (default) or "" to disable it.
         """
@@ -51,15 +57,15 @@
 
     def reset(self, restore: bool = False):
         """
         Reset the configuration file.
         This is blocked as it can make conflicts with other GUI widgets - unless you shutdown the app immediately..
         """
         raise NotImplementedError(
-            "reset function is blocked on ColorManager. Please use the get_config.GetConfig class instead."
+            "reset() is blocked on ColorManager. Please use get_config.GetConfig class instead."
         )
 
     def backup(self, file: str):
         """
         Backup a file to another file
         @param file : str : Target backup file
         """
@@ -74,14 +80,17 @@
     # Configure widgets
     @property
     def GetFont(self):
         """
         Property of ColorManager to call the font definitions.
         When called, this returns the following:
             (font) size (int|str), style, weight, family
+        It will vary on different GUI toolkits:
+        * wxPython: wx.Font object
+        * Tkinter: tkinter.font.Font object
         """
         return self._get_font()
 
     @GetFont.setter
     def GetFont(self, func: typing.Callable):
         self._get_font = func
 
@@ -97,15 +106,15 @@
 
         if family == "default":
             family = ""
 
         try:
             int(size)
         except ValueError:
-            size_ = 14
+            size_ = 10
         else:
             if int(size) > 0:
                 size_ = int(size)
             else:
                 raise ValueError("Font size must be higher than 0")
 
         return size_, style, weight, family
@@ -133,36 +142,30 @@
 
         # Get values
         color = self.getkey("color", "background")
         fontcolor = self.getkey("color", "textcolor")
         autocolor = self.getkey("color", "autocolor")
 
         # Interface color
-        ## Default color modes
-        colors = {
-            "light": "#ffffff",
-            "dark": "#1c1c1c",
-        }
+        from ._colors import colors
 
         ##
         resv = {"light": "dark", "dark": "light"}
 
         ## Check
-        if autocolor == True or "yes":
+        if autocolor in self.yesvalues and AUTOCOLOR is True:
             color_ = colors[_get_sys_mode()]
-        elif color in colors:
+        else:
             color_ = colors[color]
 
         # Text color
-        colors["green"] = "#00ff00"
-        colors["red"] = "#ff0000"
         if fontcolor == "default":
-            if autocolor == False:
+            if autocolor not in self.yesvalues or AUTOCOLOR is False:
                 fontcolor_ = colors[resv[color]]
-            else:
+            elif autocolor in self.yesvalues and AUTOCOLOR is True:
                 fontcolor_ = colors[resv[_get_sys_mode()]]
         else:
             if fontcolor in colors:
                 fontcolor_ = colors[fontcolor]
             elif fontcolor.startswith("#") and len(fontcolor) == 7:
                 try:
                     ImageColor.getrgb(fontcolor)
@@ -175,42 +178,42 @@
             else:
                 raise ConfigurationError(
                     "interface", "textcolor", "Invalid color name/code"
                 )
 
         return ImageColor.getrgb(color_), ImageColor.getrgb(fontcolor_)
 
-    def setcolorfunc(self, objname: str, func: typing.Callable, params: dict):
+    def setcolorfunc(self, objname: str, func: typing.Callable, params: typing.Any):
         """
-        Set wxPython widgets background color function.
+        Set wxPython widgets background+foreground color function.
         @param objname (str): Object name (for easier access)
-        @param func (callable): Function to set the background color (no arg)
-        @param params (dict): Parameters to pass to func
+        @param func (callable): Target function (no arg)
+        @param params: Parameters to pass to func
         """
         self.setcolorfn[objname] = {"fn": func, "params": params}
 
-    def setfontcfunc(self, objname: str, func: typing.Callable, params: dict):
+    def setfontcfunc(self, objname: str, func: typing.Callable, params: typing.Any):
         """
-        Set wxPython widgets background color function.
+        Set wxPython widgets font style function.
         @param objname (str): Object name (for easier access)
-        @param func (callable): Function to set the background color (no arg)
-        @param params (dict): Parameters to pass to func
+        @param func (callable): Function to set the font style (no arg)
+        @param params: Parameters to pass to func
         """
         self.setfontfn[objname] = {"fn": func, "params": params}
 
     def configure(self, widget: typing.Any):
         """
         Configure a widget with pre-defined settings.
         This function also ables to rerun itself under a threading thread.
         @param widget : Widget to configure
         @see setcolorfunc
         @see setfontcfunc
         """
         if not widget:
-            print("Widget died, skip configuring.")
+            logger.debug(f"Widget {widget} died, skip configuring.")
             return
 
         color, fontcolor = self.GetColor
 
         for item in self.setfontfn:
             fn = self.setfontfn[item]["fn"]
             if not self.setfontfn[item]["params"]:
@@ -223,12 +226,15 @@
             if not self.setcolorfn[item]["params"]:
                 fn(color)
             else:
                 fn(self.setcolorfn[item]["params"], color)
 
     def autocolor_run(self, widget: typing.Any):
         autocolor = self.getkey("color", "autocolor")
+        if not AUTOCOLOR:
+            raise Exception("ColorManager.autocolor_run() called when auto-color system is not usable")
+        
         if autocolor == True or "yes" and widget not in self.threads:
             self.threads[widget] = threading.Thread(
                 args=self.configure(widget), daemon=True
             )
             self.threads[widget].start()
```

### Comparing `libtextworker-0.1.2/libtextworker/interface/tk/__init__.py` & `libtextworker-0.1.3/libtextworker/interface/tk/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 """
 @package libtextworker.interface.tk
-Contains classes for Tkinter.
+Contains class(es) and needed attributes for Tkinter.
 """
 import threading
 import typing
 from libtextworker import Importable
-from ..manager import ColorManager, default_configs
+from ..manager import ColorManager
 
 if Importable["tkinter"] == True:
     import darkdetect
-    import sv_ttk
-    from tkinter import TclError, font, messagebox
-
-    pass
+    from tkinter import TclError, font, Misc
 else:
     raise Exception(
-        "interface.tk is called but its dependency Tkinter is not installed"
+        "interface.tk is called but its dependency Tkinter is not installed.\n"
+        "You'll need:\n- tkinter\n- darkdetect\n- sv-ttk (optional)\npackages."
     )
 
+try:
+    import sv_ttk
+except ImportError:
+    SVTTK_AVAILABLE = False
+else:
+    SVTTK_AVAILABLE = True
+
 
 class ColorManager(ColorManager):
     recursive_configure: bool = True
     is_shown: bool = False  # Messages
 
+    def GetFont(self):
+        """
+        Property of ColorManager which is a tkinter.font.Font object when called.
+        """
+        return self._get_font
+
     def _get_font(self):
         size, style, weight, family = super()._get_font()
         font_families = font.families()
 
-        if family == "default":
+        if family == "default" or family not in font_families:
             family = "Consolas"
-        elif family not in font_families:
-            if not self.is_shown:
-                messagebox.showwarning(
-                    message=_(
-                        """
-                        It seemed that your preferred font family does not available on your machine here.\n
-                        Install the font first - and now the program will use Consolas instead.\n
-                        If you think that this is a mistake, please report it.
-                        """
-                    )
-                )
-                self.is_shown = True
 
         if style == "normal" or style != "italic":
             style = "roman"
+
         return font.Font(None, family=family, weight=weight, slant=style, size=size)
 
     def setfontcfunc(self, objname: str, func: typing.Callable, params: dict):
         raise NotImplementedError
 
     def setcolorfunc(self, objname: str, func: typing.Callable, params: dict):
         raise NotImplementedError
 
-    def configure(self, widget: typing.Any, childs_too: bool = recursive_configure):
+    def configure(self, widget: Misc, childs_too: bool = recursive_configure):
         back, fore = self.GetColor
         font_to_use = self.GetFont
 
+        if "Menu" in widget.winfo_class():
+            font_to_use.configure(size=...)
+
         try:
             widget.configure(font=font_to_use)
         except TclError:
             pass
 
         # Why this catch?
         # Some Tkinter objects do not use fg and bg as their configure() keywords,
@@ -75,22 +78,26 @@
         if childs_too:
             for child in widget.winfo_children():
                 self.configure(child, self.recursive_configure)
                 self.autocolor_run(child)
 
     def autocolor_run(self, widget: typing.Any):
         def _configure(theme: str):
-            sv_ttk.set_theme(theme.lower())
+            if SVTTK_AVAILABLE:
+                sv_ttk.set_theme(theme.lower())
             self.configure(widget)
 
         if self.getkey("color", "autocolor") == True or "yes":
             if widget not in self.threads or not self.threads[widget].is_alive():
                 self.threads[widget] = threading.Thread(
                     target=darkdetect.listener, args=(_configure,), daemon=True
                 )
                 self.threads[widget].start()
-            sv_ttk.set_theme(
-                darkdetect.theme().lower()
-            )  # Keep this to avoid 'font already exists' error
+
+            if SVTTK_AVAILABLE:
+                sv_ttk.set_theme(
+                    darkdetect.theme().lower()
+                )  # Keep this to avoid 'font already exists' error
 
 
-clrmgr = ColorManager(default_configs)
+## @deprecated On version 0.1.3
+clrmgr = None
```

### Comparing `libtextworker-0.1.2/libtextworker/interface/tk/miscs.py` & `libtextworker-0.1.3/libtextworker/interface/tk/miscs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,54 +4,58 @@
 
 def CreateMenu(
     items: list[tuple], parent: Misc | None = None, tearoff: Literal[0, 1] = 0
 ) -> Menu:
     """
     Make a Tkinter menu with commands.
     Menu items list must follow the format below:
-    ```
-    Each menu item is made under a tuple
+    ```python
+    # Each menu item is made with a tuple
     (
      label[str], accelerator[str], handler[str|Callable],
      onvalue[=None], offvalue[=None], variable[=None],
      state["normal", "active", "disabled"][="normal"]
      kind["check", "option", "separator", "normal" or None][=None]
     )
     ```
     """
+
     target = Menu(parent, tearoff=tearoff)
     none_to_blank = {None: ""}
     none_to_blank_2 = {None: ...}
-    for item in items:
-        for label, acc, handler, onvalue, offvalue, variable, state, kind in item:
-            label = none_to_blank.get(label, label)
-            acc = none_to_blank.get(acc, acc)
-
-            onvalue = none_to_blank_2.get(onvalue, onvalue)
-            offvalue = none_to_blank_2.get(offvalue, offvalue)
-            variable = none_to_blank_2.get(variable, variable)
-
-            if kind == None or "normal":
-                target.add_command(
-                    accelerator=acc, command=handler, label=label, state=state
-                )
-            if kind == "check":
-                target.add_checkbutton(
-                    accelerator=acc,
-                    command=handler,
-                    label=label,
-                    offvalue=offvalue,
-                    onvalue=onvalue,
-                    state=state,
-                    variable=variable,
-                )
-            if kind == "separator":
-                target.add_separator()
-            if kind == "option":
-                target.add_radiobutton(
-                    accelerator=acc,
-                    command=handler,
-                    label=label,
-                    state=state,
-                    variable=variable,
-                )
+
+    for label, acc, handler, onvalue, offvalue, variable, state, kind in items:
+        label = none_to_blank.get(label, label)
+        acc = none_to_blank.get(acc, acc)
+
+        onvalue = none_to_blank_2.get(onvalue, onvalue)
+        offvalue = none_to_blank_2.get(offvalue, offvalue)
+        variable = none_to_blank_2.get(variable, variable)
+
+        if kind == None or "normal":
+            target.add_command(
+                accelerator=acc, command=handler, label=label, state=state
+            )
+
+        if kind == "check":
+            target.add_checkbutton(
+                accelerator=acc,
+                command=handler,
+                label=label,
+                offvalue=offvalue,
+                onvalue=onvalue,
+                state=state,
+                variable=variable,
+            )
+
+        if kind == "separator":
+            target.add_separator()
+
+        if kind == "option":
+            target.add_radiobutton(
+                accelerator=acc,
+                command=handler,
+                label=label,
+                state=state,
+                variable=variable,
+            )
     return target
```

### Comparing `libtextworker-0.1.2/libtextworker/interface/wx/__init__.py` & `libtextworker-0.1.3/libtextworker/interface/wx/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     $ pip install wxPython
     
 Else libtextworker will refuse to use this package.
 """
 import typing
 from libtextworker import Importable
 from . import constants
-from ..manager import ColorManager, default_configs
+from ..manager import ColorManager
 
 if Importable["wx"] == True:
     import wx
 
     pass
 else:
     raise Exception("wxPython is needed to use libtextworker.interface.wx")
@@ -46,8 +46,9 @@
 
         if childs_too and hasattr(widget, "GetChildren"):
             for child in widget.GetChildren():
                 self.configure(child, self.recursive_configure)
                 self.autocolor_run(child)
 
 
-clrmgr = ColorManager(default_configs)
+## @deprecated On version 0.1.3
+clrmgr = None
```

### Comparing `libtextworker-0.1.2/libtextworker/interface/wx/about.py` & `libtextworker-0.1.3/libtextworker/interface/wx/about.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import wx
 import wx.adv
 
 from typing import Any, final
-from libtextworker.general import CraftItems, libTewException, GetCurrentDir
+from ...general import CraftItems, GetCurrentDir
 
+## Available pre-stored licenses:
+# * AGPL
+# * GPL 3
+# * LGPL 3
+# * MIT
 available_licenses = [
     "AGPL_full",
     "AGPL_short",
     "GPL3_full",
     "GPL3_short",
-    "MIT"
+    "LGPL_3",
+    "MIT",
 ]
 
 
 @final
 class AboutDialog:
     """
     About dialog built with wxPython.
@@ -44,30 +50,29 @@
     def SetIcon(self, icon: wx.Icon):
         return self.infos.SetIcon(icon)
 
     def SetLicense(self, license: str, include_copyright: bool = False):
         """
         Set the long, multiline string containing the text of the program license.
         Not all license types are available. You can include your program copyright if needed.
+        @version Updated on 0.1.3
         @see available_licenses
         @see SetCopyright
         """
-        data = "" # Our result
-        if license not in available_licenses:
-            raise libTewException(
-                "Sorry about this, but we couldn't find any license as requested ({}). You should notify this for libtextworker devs".format(
-                    license
-                )
-            )
-        targetfile = CraftItems(
-            GetCurrentDir(__file__), "../../licenses/{}.txt".format(license)
-        )
+        data = ""  # Our result
+        if license in available_licenses:
+            license = open(
+                CraftItems(
+                    GetCurrentDir(__file__), "../../licenses/{}.txt".format(license)
+                ),
+                "r",
+            ).read()
         if include_copyright == True and self.infos.GetCopyright() != "":
             data += self.infos.GetCopyright() + "\n"
-        data += open(targetfile, "r").read()
+        data += license
         return self.infos.SetLicence(data)
 
     def SetName(self, name: str):
         return self.infos.SetName(name)
 
     def SetTranslators(self, translators):
         return self.infos.SetTranslators(translators)
```

### Comparing `libtextworker-0.1.2/libtextworker/interface/wx/editor.py` & `libtextworker-0.1.3/libtextworker/interface/wx/editor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 import wx
 import wx.stc
 
 from libtextworker import EDITOR_DIR
 from libtextworker.get_config import ConfigurationError, GetConfig
 
-from libtextworker.interface.wx import clrmgr
+from libtextworker.interface.wx import ColorManager
 from libtextworker.interface.wx.miscs import CreateMenu
 
 default_configs = {
     "indentation": {"size": 4, "type": "tabs", "show_guide": "yes"},
     "menu": {"enabled": "yes"},
     "editor": {"line_count": "yes", "dnd_enabled": "yes"},
 }
 
 
 class StyledTextControl(wx.stc.StyledTextCtrl):
-    def __init__(self, *args, **kw):
-        kw["style"] = kw.get("style", 0) | wx.stc.STC_STYLE_DEFAULT
-        super().__init__(*args, **kw)
+    """
+    A better styled wxStyledTextCtrl.
+    @since version 0.1.3:
+        Split __init__ into __init__ and EditorInit(str)
+        Auto-expand linenumber margin
+    """
+
+    def EditorInit(self, config_path: str = ""):
+        """
+        @since 0.1.3
+        Initialize the editor, customized part.
+        You can't ignore __init__() function;)
+        @param config_path (str): Configuration path (optional - defaults to lib's path)
+        """
+        if not config_path:
+            config_path = EDITOR_DIR + "editor.ini"
 
-        self.clrmgr = clrmgr
-        self.cfg = GetConfig(default_configs, EDITOR_DIR + "editor.ini")
+        self.clrmgr = ColorManager()
+        self.cfg = GetConfig(default_configs, config_path)
 
         # Base editor color
         self.SetupEditorColor()
 
         # Setup line numbers
         self.LineNumbers()
 
         # Drag-and-drop support
         self.DNDSupport()
 
         # Indentation
         self.IndentationSet()
 
         # Right click menu
-        if self.cfg.getkey("menu", "enabled") in [True, "yes"]:
+        if self.cfg.getkey("menu", "enabled") in self.cfg.yes_values:
             self.Bind(wx.EVT_RIGHT_DOWN, self.MenuPopup)
 
+    """
+    Setup GUI elements.
+    """
+
     def DNDSupport(self) -> bool:
-        if (
-            self.cfg.getkey("editor", "dnd_enabled", True, True, getbool=True) != True
-            or "yes"
-        ):
+        if self.cfg.getkey("editor", "dnd_enabled", True, True) not in self.cfg.yes_values:
             return False
 
         dt = DragNDropTarget(self)
         self.SetDropTarget(dt)
 
         return True
 
     def IndentationSet(self) -> bool:
-        size = int(self.cfg.getkey("indentation", "size", True, True, getbool=False))
+        size = int(self.cfg.getkey("indentation", "size", True, True))
         tp = self.cfg.getkey("indentation", "type", True, True)
-        show_guide = self.cfg.getkey(
-            "indentation", "show_guide", True, True, getbool=True
-        )
+        show_guide = self.cfg.getkey("indentation", "show_guide", True, True)
 
         if not 8 >= size > 0:
             raise ConfigurationError(
                 "indentation", "size", "Must be in range from 1 to 8"
             )
 
         if not tp in ["tabs", "spaces"]:
@@ -71,24 +83,21 @@
 
         if show_guide == True or "yes":
             self.SetIndentationGuides(True)
         else:
             self.SetIndentationGuides(False)
 
     def LineNumbers(self) -> bool:
-        if self.cfg.getkey("editor", "line_count", True, True, getbool=True) not in [
-            True,
-            "yes",
-        ]:
-            self.SetMarginWidth(1, 0)
+        state = self.cfg.getkey("editor", "line_count", True, True)
+        if state in ["no", False]:
+            self.SetMarginWidth(0, 0)
             return False
 
-        self.SetMarginType(1, wx.stc.STC_MARGIN_NUMBER)
-        self.SetMarginMask(1, 0)
-        self.SetMarginWidth(1, 40)
+        self.SetMarginType(0, wx.stc.STC_MARGIN_NUMBER)
+        self.SetMarginMask(0, 0)
 
         return True
 
     def SetupEditorColor(self):
         bg, fg = self.clrmgr._get_color()
         self.StyleSetSpec(0, "fore:{},back:{}".format(fg, bg))
         self.StyleSetSpec(wx.stc.STC_STYLE_LINENUMBER, "fore:{},back:{}".format(fg, bg))
@@ -98,28 +107,52 @@
         )
         self.clrmgr.setfontcfunc(
             "textw", self.StyleSetForeground, wx.stc.STC_STYLE_DEFAULT
         )
         self.clrmgr.configure(self)
 
         self.Bind(wx.stc.EVT_STC_MODIFIED, self.OnSTCModify)
+        self.Bind(wx.stc.EVT_STC_UPDATEUI, self.OnUIUpdate)
+
+    """
+    Events.
+    """
 
     def OnSTCModify(self, event):
         if event:
             pos = event.GetPosition()
             length = event.GetLength()
         else:
             pos = 0
             length = self.GetLength()
         self.StartStyling(pos)
         self.SetStyling(length, 0)
         event.Skip()
 
-    def MenuPopup(self, evt):
-        pt = evt.GetPosition()
+    def OnUIUpdate(self, event):  # MS Bing helped me this
+        """
+        @since Version 0.1.3
+        Auto-expand linenumber margin.
+        """
+        line_count = self.GetLineCount()
+        last_line_num = str(line_count)
+
+        if len(last_line_num) <= 4:
+            margin_width = 40
+        else:
+            last_line_width = self.TextWidth(wx.stc.STC_STYLE_LINENUMBER, last_line_num)
+            # add some extra space
+            margin_width = last_line_width + 4
+
+        # set the margin width
+        self.SetMarginWidth(0, margin_width)
+        event.Skip()
+
+    def MenuPopup(self, event):
+        pt = event.GetPosition()
         menu = CreateMenu(
             self,
             [
                 (wx.ID_CUT, None, None, lambda evt: self.Cut(), None),
                 (wx.ID_COPY, None, None, lambda evt: self.Copy(), None),
                 (wx.ID_PASTE, None, None, lambda evt: self.Paste(), None),
                 (None, None, None, None, None),
@@ -136,26 +169,27 @@
             _("Read only"),
             _("Set the text to be read-only"),
             wx.ITEM_CHECK,
         )
         menu.Append(readonly)
         self.Bind(
             wx.EVT_MENU,
-            lambda evt: (
-                self.SetReadOnly(readonly.IsChecked()),
-                print("set to {}".format(readonly.IsChecked())),
-            ),
+            lambda evt: (self.SetReadOnly(readonly.IsChecked()),),
             readonly,
         )
 
         self.PopupMenu(menu, pt)
         menu.Destroy()
 
 
 class DragNDropTarget(wx.FileDropTarget, wx.TextDropTarget):
+    """
+    Drag-and-drop (DND) support for wxStyledTextCtrl.
+    """
+
     def __init__(self, textctrl):
         super().__init__()
         self.Target = textctrl
 
     def OnDropText(self, x, y, data):
         self.Target.WriteText(data)
         return True
```

### Comparing `libtextworker-0.1.2/libtextworker/licenses/AGPL_full.txt` & `libtextworker-0.1.3/libtextworker/licenses/AGPL_full.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/libtextworker/licenses/AGPL_short.txt` & `libtextworker-0.1.3/libtextworker/licenses/AGPL_short.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/libtextworker/licenses/GPL3_full.txt` & `libtextworker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/libtextworker/licenses/GPL3_short.txt` & `libtextworker-0.1.3/libtextworker/licenses/GPL3_short.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/libtextworker/licenses/LGPL_3.txt` & `libtextworker-0.1.3/libtextworker/licenses/LGPL_3.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/libtextworker/licenses/MIT.txt` & `libtextworker-0.1.3/libtextworker/licenses/MIT.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/libtextworker/versioning.py` & `libtextworker-0.1.3/libtextworker/versioning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import importlib
 import packaging.version
-import warnings
 
 from . import general
 
-Requested = []
+"""
+Projects called by functions under libtextworker.versioning.
+"""
+Requested = {}
 
 
 def parse_version(project: str):
     """
     Try to import a project then parse its version with the ```packaging.version``` module.
     Parsed projects are stored in Requested (list).
     @see is_development_version
     @see is_development_from_project
     @see require
     @see require_exact
     @see require_lower
     @see Requested
     """
-    if project in Requested:
-        warnings.warn("%(project)s already requested.")
-        return
-
+    global Requested
     module = importlib.import_module(project)
-    if not module.__version__:
-        raise general.libTewException(
-            "%(project)s does not have __version__ attribute!"
-        )
-    Requested.append(project)
-    return packaging.version.parse(module.__version__)
+
+    if project not in Requested:
+        if not module.__version__:
+            raise general.libTewException(
+                "%(project)s does not have __version__ attribute!"
+            )
+        Requested[project] = packaging.version.parse(module.__version__)
+
+    return Requested[project]
 
 
 def is_development_version(version: str):
     """
     Parse and check if the specified version is a prerelease.
     @see is_development_version_from_project
     """
@@ -65,28 +67,28 @@
 def require_exact(project: str, target_version: str):
     """
     Ensures the correct version of a project IS available.
     @param project (str): Target project name
     @param target_version (str): Target project version
     """
     currver = parse_version(project)
-    target = packaging.verison.parse(target_version)
+    target = packaging.version.parse(target_version)
 
     if currver != target:
         raise general.libTewException(
             "Project %(project)s not available for version %(target_version)"
         )
 
 
 def require_lower(project: str, target_version: str):
     """
     Ensures the project version is LOWER than the requested one.
     @param project (str): Target project name
     @param target_version (str): Target project version
     """
     currver = parse_version(project)
-    target = packaging.verison.parse(target_version)
+    target = packaging.version.parse(target_version)
 
     if currver >= target:
         raise general.libTewException(
             "Project %(project)s not available for version %(target_version)"
         )
```

### Comparing `libtextworker-0.1.2/LICENSE` & `libtextworker-0.1.3/libtextworker/licenses/GPL3_full.txt`

 * *Files identical despite different names*

### Comparing `libtextworker-0.1.2/pyproject.toml` & `libtextworker-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 [tool.poetry]
 name = "libtextworker"
-version = "0.1.2"
+version = "0.1.3"
 description = "App library for textworker"
 authors = ["lebao3105 <bao12345yocoo@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/lebao3105/libtextworker"
 documentation = "https://lebao3105.github.io/libtextworker"
 keywords = ["wx", "tkinter", "gui"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/lebao3105/libtextworker/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-configparser = "^5.3.0"
 Pillow = "^9.5.0"
 packaging = "^23.0"
 importlib-metadata = "^6.1.0"
 
 wxPython = {version = "^4.0.0", optional = true}
 sv-ttk = {version = "^2.4.3", optional = true}
 darkdetect = {version = "^0.8.0", optional = true}
+commented-configparser = {version = "^1.0.0", optional = true}
 
 [tool.poetry.extras]
-wx = ["darkdetect", "wxPython"]
-tkinter = ["darkdetect", "sv-ttk"]
+wx = ["wxPython"]
+tkinter = ["sv-ttk"]
+autocolor = ["darkdetect"]
+all = ["darkdetect", "wxPython", "sv-ttk", "commented-configparser"]
+
+[tool.black]
+line-length = 88
+target-version = ['py310']
+include = '\.pyi?$'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `libtextworker-0.1.2/PKG-INFO` & `libtextworker-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: libtextworker
-Version: 0.1.2
+Version: 0.1.3
 Summary: App library for textworker
 Home-page: https://github.com/lebao3105/libtextworker
 License: GPL-3.0-or-later
 Keywords: wx,tkinter,gui
 Author: lebao3105
 Author-email: bao12345yocoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: autocolor
 Provides-Extra: tkinter
 Provides-Extra: wx
 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
-Requires-Dist: configparser (>=5.3.0,<6.0.0)
-Requires-Dist: darkdetect (>=0.8.0,<0.9.0) ; extra == "wx" or extra == "tkinter"
+Requires-Dist: commented-configparser (>=1.0.0,<2.0.0) ; extra == "all"
+Requires-Dist: darkdetect (>=0.8.0,<0.9.0) ; extra == "autocolor" or extra == "all"
 Requires-Dist: importlib-metadata (>=6.1.0,<7.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: sv-ttk (>=2.4.3,<3.0.0) ; extra == "tkinter"
-Requires-Dist: wxPython (>=4.0.0,<5.0.0) ; extra == "wx"
+Requires-Dist: sv-ttk (>=2.4.3,<3.0.0) ; extra == "tkinter" or extra == "all"
+Requires-Dist: wxPython (>=4.0.0,<5.0.0) ; extra == "wx" or extra == "all"
 Project-URL: Bug Tracker, https://github.com/lebao3105/libtextworker/issues
 Project-URL: Documentation, https://lebao3105.github.io/libtextworker
 Description-Content-Type: text/markdown
 
 ## libtextworker
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Usage
 Available packages from Pypi:
 * libtextworker: Base library, contains all codes but no other deps installed
 * libtextworker[tkinter]: Tkinter support
 * libtextworker[wx]: wxPython support
+* libtextworker[autocolor]: (since 0.1.3) GUI auto color effect (depends on system theme)
+* libtextworker[all]: Everything above
 
-You can read the API documents [here.](https://lebao3105.github.io/libtextworker)
+Documents are stored to ```v<version>-docs``` tag, normally the document on https://lebao3105.github.io/libtextworker is the latest stable version of libtextworker.
```

