# Comparing `tmp/autorandr-1.8.post1.tar.gz` & `tmp/autorandr-1.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autorandr-1.8.post1.tar", last modified: Sat Mar 16 14:44:12 2019, max compression
+gzip compressed data, was "dist/autorandr-1.9.post1.tar", last modified: Thu Dec 19 11:46:23 2019, max compression
```

## Comparing `autorandr-1.8.post1.tar` & `autorandr-1.9.post1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 pberndt   (1000) pberndt   (1000)        0 2019-03-16 14:44:12.000000 autorandr-1.8.post1/
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)       18 2017-07-25 14:48:42.000000 autorandr-1.8.post1/MANIFEST.in
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)      101 2019-03-16 14:44:12.000000 autorandr-1.8.post1/setup.cfg
-drwxr-xr-x   0 pberndt   (1000) pberndt   (1000)        0 2019-03-16 14:44:12.000000 autorandr-1.8.post1/autorandr.egg-info/
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)       64 2019-03-16 14:44:11.000000 autorandr-1.8.post1/autorandr.egg-info/entry_points.txt
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)        1 2019-03-16 14:44:11.000000 autorandr-1.8.post1/autorandr.egg-info/dependency_links.txt
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)       10 2019-03-16 14:44:11.000000 autorandr-1.8.post1/autorandr.egg-info/top_level.txt
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)      221 2019-03-16 14:44:12.000000 autorandr-1.8.post1/autorandr.egg-info/SOURCES.txt
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)    13286 2019-03-16 14:44:11.000000 autorandr-1.8.post1/autorandr.egg-info/PKG-INFO
--rwxr-xr-x   0 pberndt   (1000) pberndt   (1000)    60956 2019-03-16 14:38:04.000000 autorandr-1.8.post1/autorandr.py
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)    13286 2019-03-16 14:44:12.000000 autorandr-1.8.post1/PKG-INFO
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)     1313 2019-03-16 14:41:03.000000 autorandr-1.8.post1/setup.py
--rw-r--r--   0 pberndt   (1000) pberndt   (1000)    10368 2019-03-16 14:38:56.000000 autorandr-1.8.post1/README.md
+drwxr-xr-x   0 pberndt   (1000) pberndt   (1000)        0 2019-12-19 11:46:23.000000 autorandr-1.9.post1/
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)       18 2017-07-25 14:48:42.000000 autorandr-1.9.post1/MANIFEST.in
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)    11383 2019-12-19 11:46:21.000000 autorandr-1.9.post1/README.rst
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)      101 2019-12-19 11:46:23.000000 autorandr-1.9.post1/setup.cfg
+drwxr-xr-x   0 pberndt   (1000) pberndt   (1000)        0 2019-12-19 11:46:23.000000 autorandr-1.9.post1/autorandr.egg-info/
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)       64 2019-12-19 11:46:23.000000 autorandr-1.9.post1/autorandr.egg-info/entry_points.txt
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)        1 2019-12-19 11:46:23.000000 autorandr-1.9.post1/autorandr.egg-info/dependency_links.txt
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)       10 2019-12-19 11:46:23.000000 autorandr-1.9.post1/autorandr.egg-info/top_level.txt
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)      232 2019-12-19 11:46:23.000000 autorandr-1.9.post1/autorandr.egg-info/SOURCES.txt
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)    13958 2019-12-19 11:46:23.000000 autorandr-1.9.post1/autorandr.egg-info/PKG-INFO
+-rwxr-xr-x   0 pberndt   (1000) pberndt   (1000)    63753 2019-12-19 11:41:28.000000 autorandr-1.9.post1/autorandr.py
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)    13958 2019-12-19 11:46:23.000000 autorandr-1.9.post1/PKG-INFO
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)     1313 2019-12-19 11:41:36.000000 autorandr-1.9.post1/setup.py
+-rw-r--r--   0 pberndt   (1000) pberndt   (1000)    10912 2019-12-19 11:41:04.000000 autorandr-1.9.post1/README.md
```

### Comparing `autorandr-1.8.post1/autorandr.egg-info/PKG-INFO` & `autorandr-1.9.post1/autorandr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: autorandr
-Version: 1.8.post1
+Version: 1.9.post1
 Summary: Automatically select a display configuration based on connected devices
 Home-page: https://github.com/phillipberndt/autorandr
 Author: Phillip Berndt
 Author-email: phillip.berndt@googlemail.com
 License: GPLv3
 Description: # autorandr
         
@@ -45,14 +45,15 @@
         
         * Adrián López
         * andersonjacob
         * Alexander Wirt
         * Brice Waegeneire
         * Chris Dunder
         * Christoph Gysin
+        * Christophe-Marie Duquesne
         * Daniel Hahler
         * Maciej Sitarz
         * Mathias Svensson
         * Matthew R Johnson
         * Nazar Mokrynskyi
         * Phillip Berndt
         * Rasmus Wriedt Larsen
@@ -85,14 +86,15 @@
           [nix package](https://github.com/NixOS/nixpkgs/blob/master/nixos/modules/services/misc/autorandr.nix)
           on NixOS.
         * Use the automated nightlies generated by the
           [openSUSE build service](https://build.opensuse.org/package/show/home:phillipberndt/autorandr)
           for various distributions (RPM and DEB based).
         * Use the [X binary package system](https://wiki.voidlinux.eu/XBPS)' on Void Linux 
         * Build a .deb-file from the source tree using `make deb`.
+        * Build a .rpm-file from the source tree using `make rpm`.
         
         We appreciate packaging scripts for other distributions, please file a pull
         request if you write one.
         
         If you prefer `pip` over your package manager, you can install autorandr with:
         
             sudo pip install "git+http://github.com/phillipberndt/autorandr#egg=autorandr"
@@ -156,15 +158,15 @@
         `~/.config/autorandr/settings.ini` in a section `config`. The most useful
         candidate for doing that is `skip-options`, if you need it.
         
         ## Advanced usage
         
         ### Hook scripts
         
-        Three more scripts can be placed in the configuration directory (as 
+        Three more scripts can be placed in the configuration directory
         (as defined by the [XDG spec](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html),
         usually `~/.config/autorandr` or `~/.autorandr` if you have an old installation
         for user configuration and `/etc/xdg/autorandr` for system wide configuration):
         
         - `postswitch` is executed *after* a mode switch has taken place. This can be
           used to notify window managers or other applications about the switch.
         - `preswitch` is executed *before* a mode switch takes place.
@@ -216,15 +218,29 @@
         The EDID strings in the `~/.config/autorandr/*/setup` files may contain an
         asterisk to enable wildcard matching: Such EDIDs are matched against connected
         monitors using the usual file name globbing rules. This can be used to create
         profiles matching multiple (or any) monitors.
         
         ## Changelog
         
+        **autorandr 1.9**
+        
+        * *2019-11-10* Count closed lids as disconnected outputs
+        * *2019-10-05* Do not overwrite existing configurations without `--force`
+        * *2019-08-16* Accept modes that don't match the WWWxHHH pattern
+        * *2019-03-22* Improve bash autocompletion
+        * *2019-03-21* Store CRTC values in configurations
+        * *2019-03-24* Fix handling of recently disconnected outputs (See #128 and #143)
+        
+        **autorandr 1.8.1**
+        
+        * *2019-03-18* Removed mandb call from Makefile
+        
         **autorandr 1.8**
+        
         * *2019-02-17* Add an X11 daemon that runs autorandr when a display connects (by @rliou92, #127)
         * *2019-02-17* Replace width=0 check with disconnected to detect disconnected monitors (by @joseph-jones, #139)
         * *2019-02-17* Fix handling of empty padding (by @jschwab, #138)
         * *2019-02-17* Add a man page (by @somers-all-the-time, #133)
         
         **autorandr 1.7**
```

### Comparing `autorandr-1.8.post1/autorandr.py` & `autorandr-1.9.post1/autorandr.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,27 @@
 import posix
 import pwd
 import re
 import subprocess
 import sys
 import shutil
 import time
+import glob
 
 from collections import OrderedDict
 from distutils.version import LooseVersion as Version
 from functools import reduce
 from itertools import chain
 
 if sys.version_info.major == 2:
     import ConfigParser as configparser
 else:
     import configparser
 
-__version__ = "1.8"
+__version__ = "1.9"
 
 try:
     input = raw_input
 except NameError:
     pass
 
 virtual_profiles = [
@@ -76,15 +77,15 @@
 --batch                 run autorandr for all users with active X11 sessions
 --current               only list current (active) configuration(s)
 --config                dump your current xrandr setup
 --debug                 enable verbose output
 --detected              only list detected (available) configuration(s)
 --dry-run               don't change anything, only print the xrandr commands
 --fingerprint           fingerprint your current hardware setup
---force                 force (re)loading of a profile
+--force                 force (re)loading of a profile / overwrite exiting files
 --skip-options <option> comma separated list of xrandr arguments (e.g. "gamma")
                         to skip both in detecting changes and applying a profile
 --version               show version information and exit
 
  If no suitable profile can be identified, the current configuration is kept.
  To change this behaviour and switch to a fallback configuration, specify
  --default <profile>.
@@ -92,14 +93,26 @@
  autorandr supports a set of per-profile and global hooks. See the documentation
  for details.
 
  The following virtual configurations are available:
 """.strip()
 
 
+def is_closed_lid(output):
+    if not re.match(r'(eDP(-?[0-9]\+)*|LVDS(-?[0-9]\+)*)', output):
+        return False
+    lids = glob.glob("/proc/acpi/button/lid/*/state")
+    if len(lids) == 1:
+        state_file = lids[0]
+        with open(state_file) as f:
+            content = f.read()
+            return "close" in content
+    return False
+
+
 class AutorandrException(Exception):
     def __init__(self, message, original_exception=None, report_bug=False):
         self.message = message
         self.report_bug = report_bug
         if original_exception:
             self.original_exception = original_exception
             trace = sys.exc_info()[2]
@@ -157,14 +170,15 @@
         )?                                                                              # .. but only if the screen is in use.
         (?:[\ \t]*\([^\)]+\))(?:\s*[0-9]+mm\sx\s[0-9]+mm)?
         (?:[\ \t]*panning\ (?P<panning>[0-9]+x[0-9]+\+[0-9]+\+[0-9]+))?                 # Panning information
         (?:[\ \t]*tracking\ (?P<tracking>[0-9]+x[0-9]+\+[0-9]+\+[0-9]+))?               # Tracking information
         (?:[\ \t]*border\ (?P<border>(?:[0-9]+/){3}[0-9]+))?                            # Border information
         (?:\s*(?:                                                                       # Properties of the output
             Gamma: (?P<gamma>(?:inf|[0-9\.: e])+) |                                     # Gamma value
+            CRTC:\s*(?P<crtc>[0-9]) |                                                   # CRTC value
             Transform: (?P<transform>(?:[\-0-9\. ]+\s+){3}) |                           # Transformation matrix
             EDID: (?P<edid>\s*?(?:\\n\\t\\t[0-9a-f]+)+) |                               # EDID of the output
             (?![0-9])[^:\s][^:\n]+:.*(?:\s\\t[\\t ].+)*                                 # Other properties
         ))+
         \s*
         (?P<modes>(?:
             (?P<mode_name>\S+).+?\*current.*\s+                                         # Interesting (current) resolution:
@@ -313,27 +327,34 @@
         if not match["connected"]:
             edid = None
         elif match["edid"]:
             edid = "".join(match["edid"].strip().split())
         else:
             edid = "%s-%s" % (XrandrOutput.EDID_UNAVAILABLE, match["output"])
 
-        if not match["connected"] or not match["width"]:
+        # An output can be disconnected but still have a mode configured. This can only happen
+        # as a residual situation after a disconnect, you cannot associate a mode with an disconnected
+        # output.
+        #
+        # This code needs to be careful not to mix the two. An output should only be configured to
+        # "off" if it doesn't have a mode associated with it, which is modelled as "not a width" here.
+        if not match["width"]:
             options["off"] = None
         else:
             if match["mode_name"]:
                 options["mode"] = match["mode_name"]
             elif match["mode_width"]:
                 options["mode"] = "%sx%s" % (match["mode_width"], match["mode_height"])
             else:
                 if match["rotate"] not in ("left", "right"):
-                    options["mode"] = "%sx%s" % (match["width"], match["height"])
+                    options["mode"] = "%sx%s" % (match["width"] or 0, match["height"] or 0)
                 else:
-                    options["mode"] = "%sx%s" % (match["height"], match["width"])
-            options["rotate"] = match["rotate"]
+                    options["mode"] = "%sx%s" % (match["height"] or 0, match["width"] or 0)
+            if match["rotate"]:
+                options["rotate"] = match["rotate"]
             if match["primary"]:
                 options["primary"] = None
             if match["reflect"] == "X":
                 options["reflect"] = "x"
             elif match["reflect"] == "Y":
                 options["reflect"] = "y"
             elif match["reflect"] == "X and Y":
@@ -359,14 +380,16 @@
             if match["gamma"]:
                 gamma = match["gamma"].strip()
                 # xrandr prints different values in --verbose than it accepts as a parameter value for --gamma
                 # Also, it is not able to work with non-standard gamma ramps. Finally, it auto-corrects 0 to 1,
                 # so we approximate by 1e-10.
                 gamma = ":".join([str(max(1e-10, round(1. / float(x), 3))) for x in gamma.split(":")])
                 options["gamma"] = gamma
+            if match["crtc"]:
+                options["crtc"] = match["crtc"]
             if match["rate"]:
                 options["rate"] = match["rate"]
 
         return XrandrOutput(match["output"], edid, options), modes
 
     @classmethod
     def from_config_file(cls, edid_map, configuration):
@@ -491,14 +514,20 @@
     for i in range(1, len(split_xrandr_output), 2):
         output_name = split_xrandr_output[i].split()[0]
         output, output_modes = XrandrOutput.from_xrandr_output("".join(split_xrandr_output[i:i + 2]))
         outputs[output_name] = output
         if output_modes:
             modes[output_name] = output_modes
 
+    # consider a closed lid as disconnected if other outputs are connected
+    if sum(o.edid != None for o in outputs.values()) > 1:
+        for output_name in outputs.keys():
+            if is_closed_lid(output_name):
+                outputs[output_name].edid = None
+
     return outputs, modes
 
 
 def load_profiles(profile_path):
     "Load the stored profiles"
 
     profiles = {}
@@ -568,14 +597,25 @@
 
     meta_information is expected to be an dictionary. It will be passed to the block scripts
     in the environment, as variables called AUTORANDR_<CAPITALIZED_KEY_HERE>.
     """
     return not exec_scripts(profile_path, "block", meta_information)
 
 
+def check_configuration_pre_save(configuration):
+    "Check that a configuration is safe for saving."
+    outputs = sorted(configuration.keys(), key=lambda x: configuration[x].sort_key)
+    for output in outputs:
+        if "off" not in configuration[output].options and not configuration[output].edid:
+            return ("`%(o)s' is not off (has a mode configured) but is disconnected (does not have an EDID).\n"
+                    "This typically means that it has been recently unplugged and then not properly disabled\n"
+                    "by the user. Please disable it (e.g. using `xrandr --output %(o)s --off`) and then rerun\n"
+                    "this command.") % {"o": output}
+
+
 def output_configuration(configuration, config):
     "Write a configuration file"
     outputs = sorted(configuration.keys(), key=lambda x: configuration[x].sort_key)
     for output in outputs:
         print(configuration[output].option_string, file=config)
 
 
@@ -583,21 +623,28 @@
     "Write a setup (fingerprint) file"
     outputs = sorted(configuration.keys())
     for output in outputs:
         if configuration[output].edid:
             print(output, configuration[output].edid, file=setup)
 
 
-def save_configuration(profile_path, configuration):
+def save_configuration(profile_path, profile_name, configuration, forced=False):
     "Save a configuration into a profile"
     if not os.path.isdir(profile_path):
         os.makedirs(profile_path)
-    with open(os.path.join(profile_path, "config"), "w") as config:
+    config_path = os.path.join(profile_path, "config")
+    setup_path = os.path.join(profile_path, "setup")
+    if os.path.isfile(config_path) and not forced:
+        raise AutorandrException('Refusing to overwrite config "{}" without passing "--force"!'.format(profile_name))
+    if os.path.isfile(setup_path) and not forced:
+        raise AutorandrException('Refusing to overwrite config "{}" without passing "--force"!'.format(profile_name))
+
+    with open(config_path, "w") as config:
         output_configuration(configuration, config)
-    with open(os.path.join(profile_path, "setup"), "w") as setup:
+    with open(setup_path, "w") as setup:
         output_setup(configuration, setup)
 
 
 def update_mtime(filename):
     "Update a file's mtime"
     try:
         os.utime(filename, None)
@@ -635,15 +682,18 @@
 def get_fb_dimensions(configuration):
     width = 0
     height = 0
     for output in configuration.values():
         if "off" in output.options or not output.edid:
             continue
         # This won't work with all modes -- but it's a best effort.
-        o_mode = re.search("[0-9]{3,}x[0-9]{3,}", output.options["mode"]).group(0)
+        match = re.search("[0-9]{3,}x[0-9]{3,}", output.options["mode"])
+        if not match:
+            return None
+        o_mode = match.group(0)
         o_width, o_height = map(int, o_mode.split("x"))
         if "transform" in output.options:
             a, b, c, d, e, f, g, h, i = map(float, output.options["transform"].split(","))
             w = (g * o_width + h * o_height + i)
             x = (a * o_width + b * o_height + c) / w
             y = (d * o_width + e * o_height + f) / w
             o_width, o_height = x, y
@@ -1185,22 +1235,29 @@
 
     if "-s" in options:
         options["--save"] = options["-s"]
     if "--save" in options:
         if options["--save"] in (x[0] for x in virtual_profiles):
             raise AutorandrException("Cannot save current configuration as profile '%s':\n"
                                      "This configuration name is a reserved virtual configuration." % options["--save"])
+        error = check_configuration_pre_save(config)
+        if error:
+            print("Cannot save current configuration as profile '%s':" % options["--save"])
+            print(error)
+            sys.exit(1)
         try:
             profile_folder = os.path.join(profile_path, options["--save"])
-            save_configuration(profile_folder, config)
+            save_configuration(profile_folder, options['--save'], config, forced="--force" in options)
             exec_scripts(profile_folder, "postsave", {
                 "CURRENT_PROFILE": options["--save"],
                 "PROFILE_FOLDER": profile_folder,
                 "MONITORS": ":".join(enabled_monitors(config)),
             })
+        except AutorandrException as e:
+            raise e
         except Exception as e:
             raise AutorandrException("Failed to save current configuration as profile '%s'" % (options["--save"],), e)
         print("Saved current configuration as profile '%s'" % options["--save"])
         sys.exit(0)
 
     if "-r" in options:
         options["--remove"] = options["-r"]
```

### Comparing `autorandr-1.8.post1/PKG-INFO` & `autorandr-1.9.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: autorandr
-Version: 1.8.post1
+Version: 1.9.post1
 Summary: Automatically select a display configuration based on connected devices
 Home-page: https://github.com/phillipberndt/autorandr
 Author: Phillip Berndt
 Author-email: phillip.berndt@googlemail.com
 License: GPLv3
 Description: # autorandr
         
@@ -45,14 +45,15 @@
         
         * Adrián López
         * andersonjacob
         * Alexander Wirt
         * Brice Waegeneire
         * Chris Dunder
         * Christoph Gysin
+        * Christophe-Marie Duquesne
         * Daniel Hahler
         * Maciej Sitarz
         * Mathias Svensson
         * Matthew R Johnson
         * Nazar Mokrynskyi
         * Phillip Berndt
         * Rasmus Wriedt Larsen
@@ -85,14 +86,15 @@
           [nix package](https://github.com/NixOS/nixpkgs/blob/master/nixos/modules/services/misc/autorandr.nix)
           on NixOS.
         * Use the automated nightlies generated by the
           [openSUSE build service](https://build.opensuse.org/package/show/home:phillipberndt/autorandr)
           for various distributions (RPM and DEB based).
         * Use the [X binary package system](https://wiki.voidlinux.eu/XBPS)' on Void Linux 
         * Build a .deb-file from the source tree using `make deb`.
+        * Build a .rpm-file from the source tree using `make rpm`.
         
         We appreciate packaging scripts for other distributions, please file a pull
         request if you write one.
         
         If you prefer `pip` over your package manager, you can install autorandr with:
         
             sudo pip install "git+http://github.com/phillipberndt/autorandr#egg=autorandr"
@@ -156,15 +158,15 @@
         `~/.config/autorandr/settings.ini` in a section `config`. The most useful
         candidate for doing that is `skip-options`, if you need it.
         
         ## Advanced usage
         
         ### Hook scripts
         
-        Three more scripts can be placed in the configuration directory (as 
+        Three more scripts can be placed in the configuration directory
         (as defined by the [XDG spec](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html),
         usually `~/.config/autorandr` or `~/.autorandr` if you have an old installation
         for user configuration and `/etc/xdg/autorandr` for system wide configuration):
         
         - `postswitch` is executed *after* a mode switch has taken place. This can be
           used to notify window managers or other applications about the switch.
         - `preswitch` is executed *before* a mode switch takes place.
@@ -216,15 +218,29 @@
         The EDID strings in the `~/.config/autorandr/*/setup` files may contain an
         asterisk to enable wildcard matching: Such EDIDs are matched against connected
         monitors using the usual file name globbing rules. This can be used to create
         profiles matching multiple (or any) monitors.
         
         ## Changelog
         
+        **autorandr 1.9**
+        
+        * *2019-11-10* Count closed lids as disconnected outputs
+        * *2019-10-05* Do not overwrite existing configurations without `--force`
+        * *2019-08-16* Accept modes that don't match the WWWxHHH pattern
+        * *2019-03-22* Improve bash autocompletion
+        * *2019-03-21* Store CRTC values in configurations
+        * *2019-03-24* Fix handling of recently disconnected outputs (See #128 and #143)
+        
+        **autorandr 1.8.1**
+        
+        * *2019-03-18* Removed mandb call from Makefile
+        
         **autorandr 1.8**
+        
         * *2019-02-17* Add an X11 daemon that runs autorandr when a display connects (by @rliou92, #127)
         * *2019-02-17* Replace width=0 check with disconnected to detect disconnected monitors (by @joseph-jones, #139)
         * *2019-02-17* Fix handling of empty padding (by @jschwab, #138)
         * *2019-02-17* Add a man page (by @somers-all-the-time, #133)
         
         **autorandr 1.7**
```

### Comparing `autorandr-1.8.post1/setup.py` & `autorandr-1.9.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = open('README.md').read()
 except:
     long_description = 'Automatically select a display configuration based on connected devices'
 
 setup(
     name='autorandr',
 
-    version='1.8.post1',
+    version='1.9.post1',
 
     description='Automatically select a display configuration based on connected devices',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     url='https://github.com/phillipberndt/autorandr',
```

### Comparing `autorandr-1.8.post1/README.md` & `autorandr-1.9.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 * Adrián López
 * andersonjacob
 * Alexander Wirt
 * Brice Waegeneire
 * Chris Dunder
 * Christoph Gysin
+* Christophe-Marie Duquesne
 * Daniel Hahler
 * Maciej Sitarz
 * Mathias Svensson
 * Matthew R Johnson
 * Nazar Mokrynskyi
 * Phillip Berndt
 * Rasmus Wriedt Larsen
@@ -77,14 +78,15 @@
   [nix package](https://github.com/NixOS/nixpkgs/blob/master/nixos/modules/services/misc/autorandr.nix)
   on NixOS.
 * Use the automated nightlies generated by the
   [openSUSE build service](https://build.opensuse.org/package/show/home:phillipberndt/autorandr)
   for various distributions (RPM and DEB based).
 * Use the [X binary package system](https://wiki.voidlinux.eu/XBPS)' on Void Linux 
 * Build a .deb-file from the source tree using `make deb`.
+* Build a .rpm-file from the source tree using `make rpm`.
 
 We appreciate packaging scripts for other distributions, please file a pull
 request if you write one.
 
 If you prefer `pip` over your package manager, you can install autorandr with:
 
     sudo pip install "git+http://github.com/phillipberndt/autorandr#egg=autorandr"
@@ -148,15 +150,15 @@
 `~/.config/autorandr/settings.ini` in a section `config`. The most useful
 candidate for doing that is `skip-options`, if you need it.
 
 ## Advanced usage
 
 ### Hook scripts
 
-Three more scripts can be placed in the configuration directory (as 
+Three more scripts can be placed in the configuration directory
 (as defined by the [XDG spec](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html),
 usually `~/.config/autorandr` or `~/.autorandr` if you have an old installation
 for user configuration and `/etc/xdg/autorandr` for system wide configuration):
 
 - `postswitch` is executed *after* a mode switch has taken place. This can be
   used to notify window managers or other applications about the switch.
 - `preswitch` is executed *before* a mode switch takes place.
@@ -208,15 +210,29 @@
 The EDID strings in the `~/.config/autorandr/*/setup` files may contain an
 asterisk to enable wildcard matching: Such EDIDs are matched against connected
 monitors using the usual file name globbing rules. This can be used to create
 profiles matching multiple (or any) monitors.
 
 ## Changelog
 
+**autorandr 1.9**
+
+* *2019-11-10* Count closed lids as disconnected outputs
+* *2019-10-05* Do not overwrite existing configurations without `--force`
+* *2019-08-16* Accept modes that don't match the WWWxHHH pattern
+* *2019-03-22* Improve bash autocompletion
+* *2019-03-21* Store CRTC values in configurations
+* *2019-03-24* Fix handling of recently disconnected outputs (See #128 and #143)
+
+**autorandr 1.8.1**
+
+* *2019-03-18* Removed mandb call from Makefile
+
 **autorandr 1.8**
+
 * *2019-02-17* Add an X11 daemon that runs autorandr when a display connects (by @rliou92, #127)
 * *2019-02-17* Replace width=0 check with disconnected to detect disconnected monitors (by @joseph-jones, #139)
 * *2019-02-17* Fix handling of empty padding (by @jschwab, #138)
 * *2019-02-17* Add a man page (by @somers-all-the-time, #133)
 
 **autorandr 1.7**
```

