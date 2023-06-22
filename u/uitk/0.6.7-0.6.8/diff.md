# Comparing `tmp/uitk-0.6.7.tar.gz` & `tmp/uitk-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-0.6.7.tar", last modified: Thu Apr  6 23:46:30 2023, max compression
+gzip compressed data, was "uitk-0.6.8.tar", last modified: Thu Jun 22 16:50:40 2023, max compression
```

## Comparing `uitk-0.6.7.tar` & `uitk-0.6.8.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 23:46:30.349073 uitk-0.6.7/
--rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4290 2023-04-06 23:46:30.349073 uitk-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-06 23:46:30.349073 uitk-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     2159 2023-03-28 23:38:26.000000 uitk-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 23:46:30.308072 uitk-0.6.7/uitk/
--rw-rw-rw-   0        0        0     2818 2023-04-06 23:46:28.000000 uitk-0.6.7/uitk/__init__.py
--rw-rw-rw-   0        0        0     9117 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/events.py
--rw-rw-rw-   0        0        0    41947 2023-04-06 15:59:34.000000 uitk-0.6.7/uitk/styleSheet.py
--rw-rw-rw-   0        0        0    41539 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/styleSheet.py.bak
--rw-rw-rw-   0        0        0    64043 2023-04-06 15:48:07.000000 uitk-0.6.7/uitk/switchboard.py
--rw-rw-rw-   0        0        0    64096 2023-03-31 18:06:18.000000 uitk-0.6.7/uitk/switchboard.py.bak
-drwxrwxrwx   0        0        0        0 2023-04-06 23:46:30.348071 uitk-0.6.7/uitk/widgets/
--rw-rw-rw-   0        0        0     9928 2023-04-06 11:48:57.000000 uitk-0.6.7/uitk/widgets/MainWindow.py
--rw-rw-rw-   0        0        0     3041 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0     8136 2023-04-01 17:04:32.000000 uitk-0.6.7/uitk/widgets/attributes.py
--rw-rw-rw-   0        0        0     3561 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     7746 2023-03-31 18:06:18.000000 uitk-0.6.7/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0     4921 2023-04-06 17:27:53.000000 uitk-0.6.7/uitk/widgets/draggable_header.py
--rw-rw-rw-   0        0        0     2283 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3029 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    13913 2023-04-06 16:30:30.000000 uitk-0.6.7/uitk/widgets/listWidget.py
--rw-rw-rw-   0        0        0    22182 2023-04-06 18:03:18.000000 uitk-0.6.7/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     5903 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/messageBox.py
--rw-rw-rw-   0        0        0     2953 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     3215 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     4792 2023-04-06 17:10:28.000000 uitk-0.6.7/uitk/widgets/pushButtonDraggable.py
--rw-rw-rw-   0        0        0     4177 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/pushButton_optionBox.py
--rw-rw-rw-   0        0        0     3905 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     2956 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/task.py
--rw-rw-rw-   0        0        0     9318 2023-03-31 18:05:27.000000 uitk-0.6.7/uitk/widgets/text.py
--rw-rw-rw-   0        0        0     3339 2023-03-28 23:38:26.000000 uitk-0.6.7/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-04-06 23:46:30.326074 uitk-0.6.7/uitk.egg-info/
--rw-rw-rw-   0        0        0     4290 2023-04-06 23:46:30.000000 uitk-0.6.7/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-04-06 23:46:30.000000 uitk-0.6.7/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 23:46:30.000000 uitk-0.6.7/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-06 23:46:30.000000 uitk-0.6.7/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 16:50:40.263311 uitk-0.6.8/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.6.8/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4583 2023-06-22 16:50:40.262310 uitk-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-22 16:50:40.263311 uitk-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     2455 2023-06-22 16:49:58.000000 uitk-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:50:40.060868 uitk-0.6.8/uitk/
+-rw-rw-rw-   0        0        0     2860 2023-06-22 16:50:37.000000 uitk-0.6.8/uitk/__init__.py
+-rw-rw-rw-   0        0        0    14530 2023-05-20 02:32:52.000000 uitk-0.6.8/uitk/events.py
+-rw-rw-rw-   0        0        0   102708 2023-06-22 01:50:27.000000 uitk-0.6.8/uitk/switchboard.py
+-rw-rw-rw-   0        0        0   104164 2023-06-18 15:45:21.000000 uitk-0.6.8/uitk/switchboard.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-22 16:50:40.198414 uitk-0.6.8/uitk/widgets/
+-rw-rw-rw-   0        0        0    18485 2023-06-20 17:13:55.000000 uitk-0.6.8/uitk/widgets/MainWindow.py
+-rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.6.8/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15675 2023-06-22 16:10:40.000000 uitk-0.6.8/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     4207 2023-06-02 17:31:37.000000 uitk-0.6.8/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     8332 2023-06-20 19:15:01.000000 uitk-0.6.8/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0     7036 2023-06-10 13:16:59.000000 uitk-0.6.8/uitk/widgets/draggableHeader.py
+-rw-rw-rw-   0        0        0    22380 2023-06-02 21:56:26.000000 uitk-0.6.8/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0     2498 2023-06-02 17:31:37.000000 uitk-0.6.8/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3295 2023-06-15 19:41:53.000000 uitk-0.6.8/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    23456 2023-06-19 14:36:41.000000 uitk-0.6.8/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     7285 2023-06-20 13:18:41.000000 uitk-0.6.8/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:50:40.261311 uitk-0.6.8/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.6.8/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    12559 2023-06-22 01:40:58.000000 uitk-0.6.8/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.6.8/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.6.8/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0     5044 2023-06-17 23:02:35.000000 uitk-0.6.8/uitk/widgets/mixins/menu_instance.py
+-rw-rw-rw-   0        0        0     1967 2023-05-12 17:25:39.000000 uitk-0.6.8/uitk/widgets/mixins/state_manager.py
+-rw-rw-rw-   0        0        0    48045 2023-06-18 12:05:02.000000 uitk-0.6.8/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.6.8/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    11099 2023-05-12 17:26:59.000000 uitk-0.6.8/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6204 2023-06-10 12:44:09.000000 uitk-0.6.8/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.6.8/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     3069 2023-06-15 19:57:41.000000 uitk-0.6.8/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.6.8/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3709 2023-06-12 14:42:27.000000 uitk-0.6.8/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:50:40.094908 uitk-0.6.8/uitk.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-06-22 16:50:39.000000 uitk-0.6.8/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.6.8/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1022 2023-06-22 16:50:39.000000 uitk-0.6.8/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.6.8/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-22 16:50:39.000000 uitk-0.6.8/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-22 16:50:39.000000 uitk-0.6.8/uitk.egg-info/top_level.txt
```

### Comparing `uitk-0.6.7/PKG-INFO` & `uitk-0.6.8/uitk.egg-info/PKG-INFO.bak`

 * *Files 4% similar despite different names*

```diff
@@ -59,35 +59,35 @@
 from uitk import Switchboard
 
 class MyProject():
     ...
 
 class MySlots(MyProject):
     def __init__(self):
-        self.sb = self.get_switchboard_instance()
+        self.sb = self.switchboard()
 
     def MyButtonsObjectName(self):
         print("Button clicked!")
 
 
 sb = Switchboard(slots_location=MySlots)
-ui = sb.example #Get the UI using it's name (or sb.getUi(<name>))
+ui = sb.example #Get the UI using it's name (or sb.get_ui(<name>))
 
 print ('ui:'.ljust(20), sb.ui) #The current UI
 print ('ui name:'.ljust(20), ui.name) #The UI's filename.
 print ('ui path:'.ljust(20), ui.path) #The directory path containing the UI file
 print ('ui tags:'.ljust(20), ui.tags) #Any UI tags as a list
 print ('ui level:'.ljust(20), ui.level) #The UI level
-print ('is current ui:'.ljust(20), ui.isCurrentUi) #True if the UI is set as current
+print ('is current ui:'.ljust(20), ui.is_current) #True if the UI is set as current
 print ('is submenu:'.ljust(20), ui.isSubmenu) #True if the UI is a submenu
-print ('is connected:'.ljust(20), ui.isConnected) #True if the UI is connected to its slots
-print ('is initialized:'.ljust(20), ui.isInitialized) #True after the UI is first shown
+print ('is connected:'.ljust(20), ui.is_connected) #True if the UI is connected to its slots
+print ('is initialized:'.ljust(20), ui.is_initialized) #True after the UI is first shown
 print ('slots:'.ljust(20), ui.slots) #The associated slots class instance
 print ('slot:'.ljust(20), ui.MyButtonsObjectName.getSlot()) #The associated slot
-print ('widget from slot:'.ljust(20), sb.getWidgetFromMethod(ui.MyButtonsObjectName.getSlot()))
+print ('widget from slot:'.ljust(20), sb.get_widget_from_method(ui.MyButtonsObjectName.getSlot()))
 print ('widget:'.ljust(20), ui.MyButtonsObjectName) #Get a widget from the UI by it's name
 print ('widgets:'.ljust(20), [(w.name or w.type) for w in ui.widgets]) #All widgets of the UI
 
 ui.show(app_exec=True)
 ```
 ## Advanced Example:
```

### Comparing `uitk-0.6.7/uitk/__init__.py` & `uitk-0.6.8/uitk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # !/usr/bin/python
 # coding=utf-8
+import os
 import importlib
 import pkgutil
 import inspect
 
 
-__package__ = 'uitk'
-__version__ = '0.6.7'
+__package__ = "uitk"
+__version__ = '0.6.8'
+__path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
-for importer, modname, ispkg in \
-        pkgutil.walk_packages(__path__, __name__ + '.'):
+for importer, modname, ispkg in pkgutil.walk_packages(__path__, __name__ + "."):
     module = importlib.import_module(modname)
     for name, obj in module.__dict__.items():
         if inspect.isclass(obj):
             CLASS_TO_MODULE[obj.__name__] = modname
 
 # Define a dictionary to store imported module objects
 IMPORTED_MODULES = {}
 
+
 def __getattr__(name):
     # Check if the requested attribute is a class we need to import
     if name in CLASS_TO_MODULE:
         module_name = CLASS_TO_MODULE[name]
         if module_name not in IMPORTED_MODULES:
             # If the module hasn't been imported yet, import it and add it to the dictionary
             module = importlib.import_module(module_name)
@@ -35,37 +37,30 @@
             module = IMPORTED_MODULES[module_name]
         # Return the requested class object from the module
         return getattr(module, name)
 
     # If the requested attribute is not a class we handle, raise an AttributeError
     raise AttributeError(f"module {__package__} has no attribute '{name}'")
 
-# --------------------------------------------------------------------------------------------
-
-
-
-
-
-
 
+# --------------------------------------------------------------------------------------------
 
 
 # --------------------------------------------------------------------------------------------
 
 
-
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
-# The CLASS_TO_MODULE dictionary is built by iterating over all submodules of the package and checking if each submodule defines any classes. 
+# The CLASS_TO_MODULE dictionary is built by iterating over all submodules of the package and checking if each submodule defines any classes.
 # The resulting dictionary maps class names to their respective module names.
 
-# When __getattr__ is called with a class name, it checks if the class name is in the CLASS_TO_MODULE dictionary. 
+# When __getattr__ is called with a class name, it checks if the class name is in the CLASS_TO_MODULE dictionary.
 # If it is, __getattr__ imports the corresponding module if it hasn't already been imported, and returns the requested class object from the module using getattr.
 
-# Therefore, the classes are imported on-demand as they are requested, rather than all at once when the package is first imported. 
+# Therefore, the classes are imported on-demand as they are requested, rather than all at once when the package is first imported.
 # This can help reduce startup time and memory usage, especially for large packages with many modules and classes.
 
 # --------------------------------------------------------------------------------------------
 # deprecated:
 # --------------------------------------------------------------------------------------------
```

### Comparing `uitk-0.6.7/uitk/widgets/__init__.py` & `uitk-0.6.8/uitk/widgets/mixins/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # !/usr/bin/python
 # coding=utf-8
 import importlib
 import pkgutil
 import inspect
 
 
-__package__ = 'uitk.widgets'
+__package__ = "uitk.widgets.mixins"
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
-for importer, modname, ispkg in \
-        pkgutil.walk_packages(__path__, __name__ + '.'):
+for importer, modname, ispkg in pkgutil.walk_packages(__path__, __name__ + "."):
     module = importlib.import_module(modname)
     for name, obj in module.__dict__.items():
         if inspect.isclass(obj):
             CLASS_TO_MODULE[obj.__name__] = modname
 
 # Define a dictionary to store imported module objects
 IMPORTED_MODULES = {}
 
+
 def __getattr__(name):
     # Check if the requested attribute is a class we need to import
     if name in CLASS_TO_MODULE:
         module_name = CLASS_TO_MODULE[name]
         if module_name not in IMPORTED_MODULES:
             # If the module hasn't been imported yet, import it and add it to the dictionary
             module = importlib.import_module(module_name)
@@ -34,47 +34,41 @@
             module = IMPORTED_MODULES[module_name]
         # Return the requested class object from the module
         return getattr(module, name)
 
     # If the requested attribute is not a class we handle, raise an AttributeError
     raise AttributeError(f"module {__package__} has no attribute '{name}'")
 
-# --------------------------------------------------------------------------------------------
-
-
-
-
-
-
 
+# --------------------------------------------------------------------------------------------
 
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
-'''
+"""
 EXAMPLE USE CASE:
 import uitk.widgets as wgts
 
 wgts.PushButton #get a specific widget.
-'''
+"""
 
 # --------------------------------------------------------------------------------------------
 # deprecated:
 # --------------------------------------------------------------------------------------------
 
 
 # def __getattr__(attr_name):
-# 	"""This function dynamically imports a module and returns an attribute from the module. 
+# 	"""This function dynamically imports a module and returns an attribute from the module.
 
 # 	Parameters:
-# 		attr_name (str): The name of the attribute to be imported. The name should be in the format 
+# 		attr_name (str): The name of the attribute to be imported. The name should be in the format
 # 					'module_name.attribute_name' or just 'attribute_name'.
-# 	Return:
+# 	Returns:
 # 		(obj) The attribute specified by the `attr_name` argument.
 
 # 	:Raises:
 # 		AttributeError: If the specified attribute is not found in the original module.
 
 # 	Example:
 # 		<package>.__getattr__('module1.attribute1') #returns: <attribute1 value>
@@ -82,8 +76,8 @@
 # 	"""
 # 	try:
 # 		module = __import__(f"{__package__}.{attr_name}", fromlist=[f"{attr_name}"])
 # 		setattr(sys.modules[__name__], attr_name, getattr(module, attr_name))
 # 		return getattr(module, attr_name)
 
 # 	except ModuleNotFoundError as error:
-# 		raise AttributeError(f"Module '{__package__}' has no attribute '{attr_name}'") from error
+# 		raise AttributeError(f"Module '{__package__}' has no attribute '{attr_name}'") from error
```

### Comparing `uitk-0.6.7/uitk/widgets/progressBar.py` & `uitk-0.6.8/uitk/widgets/progressBar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,107 @@
 # !/usr/bin/python
 # coding=utf-8
-from PySide2 import QtCore, QtGui, QtWidgets
-
-from uitk.widgets.attributes import Attributes
-
-
-class ProgressBar(QtWidgets.QProgressBar, Attributes):
-	'''ex. for n, i in enumerate(lst):
-			if not self.sb.ui.progressBar.step(n, len(lst)): #register progress while checking for cancellation:
-				break
-	'''
-	def __init__(self, parent=None, **kwargs):
-		QtWidgets.QProgressBar.__init__(self, parent)
-
-		self.setStyleSheet(parent.styleSheet()) if parent else None
-
-		self.setVisible(False)
-
-		self.isCanceled = False
-		# self.connect(QtWidgets.QShortcut(QtGui.QKeySequence(QtCore.Qt.Key_Escape), self), self.cancel())
-
-		self.setAttributes(**kwargs)
-
-
-	def cancel(self):
-		'''cancel the procedure.
-		'''
-		self.isCanceled = True
-
-
-	def step(self, progress, length=100):
-		'''
-		Parameters:
-			progress (int): current value
-			length (int): total value
-
-		Return:
-			current percentage
-		ie.
-		self.progressBar(init=1) #initialize the progress bar
-		for obj in selection:
-			self.progressBar(len(selection)) #register progress
-		'''
-		if self.isCanceled:
-			return False
-
-		if not self.isVisible():
-			self.setVisible(True)
-
-		value = 100*progress/length
-		self.setValue(value)
-		# QtWidgets.QApplication.instance().processEvents() #ensure that any pending events are processed sufficiently often for the GUI to remain responsive
-		if value>=100:
-			self.setVisible(False)
-
-		print(value)
-		return True
-
-
-	def showEvent(self, event):
-		'''
-		Parameters:
-			event=<QEvent>
-		'''
-		self.isCanceled = False
-		self.setValue(0)
-
-		QtWidgets.QProgressBar.showEvent(self, event)
-
-
-	def hideEvent(self, event):
-		'''
-		Parameters:
-			event=<QEvent>
-		'''
-
-		QtWidgets.QProgressBar.hideEvent(self, event)
-
+from PySide2 import QtWidgets
+from uitk.widgets.mixins.attributes import AttributesMixin
 
 
+class ProgressBar(QtWidgets.QProgressBar, AttributesMixin):
+    """ex. for n, i in enumerate(lst):
+    if not self.sb.ui.progressBar.step(n, len(lst)): #register progress while checking for cancellation:
+            break
+    """
+
+    def __init__(self, parent=None, **kwargs):
+        QtWidgets.QProgressBar.__init__(self, parent)
+
+        self.setVisible(False)
+
+        self.isCanceled = False
+        # self.connect(QtWidgets.QShortcut(QtGui.QKeySequence(QtCore.Qt.Key_Escape), self), self.cancel())
+
+        self.set_attributes(**kwargs)
+
+    def cancel(self):
+        """cancel the procedure."""
+        self.isCanceled = True
+
+    def step(self, progress, length=100):
+        """
+        Parameters:
+                progress (int): current value
+                length (int): total value
+
+        Returns:
+                current percentage
+        ie.
+        self.progressBar(init=1) #initialize the progress bar
+        for obj in selection:
+                self.progressBar(len(selection)) #register progress
+        """
+        if self.isCanceled:
+            return False
+
+        if not self.isVisible():
+            self.setVisible(True)
+
+        value = 100 * progress / length
+        self.setValue(value)
+        # QtWidgets.QApplication.instance().processEvents() #ensure that any pending events are processed sufficiently often for the GUI to remain responsive
+        if value >= 100:
+            self.setVisible(False)
+
+        print(value)
+        return True
+
+    def showEvent(self, event):
+        """
+        Parameters:
+                event=<QEvent>
+        """
+        self.isCanceled = False
+        self.setValue(0)
+
+        QtWidgets.QProgressBar.showEvent(self, event)
+
+    def hideEvent(self, event):
+        """
+        Parameters:
+                event=<QEvent>
+        """
 
+        QtWidgets.QProgressBar.hideEvent(self, event)
 
 
 if __name__ == "__main__":
-	import sys
-	app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(sys.argv) #return the existing QApplication object, or create a new one if none exists.
-
-	w = ProgressBar()
-	w.show()
-	sys.exit(app.exec_())
+    import sys
 
+    app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(
+        sys.argv
+    )  # return the existing QApplication object, or create a new one if none exists.
+
+    w = ProgressBar()
+    w.show()
+    sys.exit(app.exec_())
 
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
-'''
+"""
 Promoting a widget in designer to use a custom class:
->	In Qt Designer, select all the widgets you want to replace, 
-		then right-click them and select 'Promote to...'. 
+>   In Qt Designer, select all the widgets you want to replace, 
+        then right-click them and select 'Promote to...'. 
 
->	In the dialog:
-		Base Class:		Class from which you inherit. ie. QWidget
-		Promoted Class:	Name of the class. ie. "MyWidget"
-		Header File:	Path of the file (changing the extension .py to .h)  ie. myfolder.mymodule.mywidget.h
-
->	Then click "Add", "Promote", 
-		and you will see the class change from "QWidget" to "MyWidget" in the Object Inspector pane.
-'''
+>   In the dialog:
+        Base Class:     Class from which you inherit. ie. QWidget
+        Promoted Class: Name of the class. ie. "MyWidget"
+        Header File:    Path of the file (changing the extension .py to .h)  ie. myfolder.mymodule.mywidget.h
+
+>   Then click "Add", "Promote", 
+        and you will see the class change from "QWidget" to "MyWidget" in the Object Inspector pane.
+"""
 
 # deprecated: -----------------------------------
 
-# if pm.progressBar ("progressBar_", query=1, isCancelled=1):
-	# break
+# if pm.progressBar ("progressBar_", q=True, isCancelled=1):
+# break
```

### Comparing `uitk-0.6.7/uitk/widgets/textEdit.py` & `uitk-0.6.8/uitk/widgets/textEdit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,110 @@
 # !/usr/bin/python
 # coding=utf-8
 from PySide2 import QtCore, QtGui, QtWidgets
-
-from uitk.widgets.attributes import Attributes
-from uitk.widgets.menu import MenuInstance
-
-
-class TextEdit(QtWidgets.QTextEdit, Attributes, MenuInstance):
-	'''
-	'''
-	shown = QtCore.Signal()
-	hidden = QtCore.Signal()
-
-	def __init__(self, parent=None, **kwargs):
-		QtWidgets.QTextEdit.__init__(self, parent)
-
-		self.setCursor(QtGui.QCursor(QtCore.Qt.ArrowCursor))
-
-		self.viewport().setAutoFillBackground(False)
-		# self.setTextBackgroundColor(QtGui.QColor(50, 50, 50))
-
-		self.setAttributes(**kwargs)
-
-
-	def insertText(self, text):
-		'''Append a new paragraph to the textEdit.
-
-		Parameters:
-			text (str): A value to append to the lineEdit as a new paragraph. The value is converted to a string if it isn't already.
-		'''
-		baseStyle = '<font style="color: LightGray; background-color: rgb(50, 50, 50);">'
-		self.append(baseStyle+str(text)) #Appends a new paragraph with the given text to the end of the textEdit.
-
-
-	def showEvent(self, event):
-		'''
-		Parameters:
-			event=<QEvent>
-		'''
-		self.shown.emit()
-
-		# self.resize(self.sizeHint())
-
-		QtWidgets.QTextEdit.showEvent(self, event)
-
-
-	def hideEvent(self, event):
-		'''
-		Parameters:
-			event=<QEvent>
-		'''
-		self.hidden.emit()
-
-		self.clear()
-
-		QtWidgets.QTextEdit.hideEvent(self, event)
-
-
+from uitk.widgets.mixins.menu_instance import MenuInstance
+from uitk.widgets.mixins.attributes import AttributesMixin
 
 
+class TextEdit(QtWidgets.QTextEdit, AttributesMixin, MenuInstance):
+    """ """
 
+    shown = QtCore.Signal()
+    hidden = QtCore.Signal()
+
+    def __init__(self, parent=None, **kwargs):
+        QtWidgets.QTextEdit.__init__(self, parent)
+
+        self.viewport().setAutoFillBackground(False)
+        # self.setTextBackgroundColor(QtGui.QColor(50, 50, 50))
+
+        self.set_attributes(**kwargs)
+
+    def insertText(self, text, color="LightGray", backround_color="rgb(50, 50, 50)"):
+        """Append a new paragraph to the textEdit.
+
+        Parameters:
+                text (str): A value to append to the lineEdit as a new paragraph. The value is converted to a string if it isn't already.
+        """
+        # Appends a new paragraph with the given text to the end of the textEdit.
+        self.append(
+            f'<font style="color: {color}; background-color: {backround_color};">{text}'
+        )
+
+    def showEvent(self, event):
+        """
+        Parameters:
+                event=<QEvent>
+        """
+        QtWidgets.QTextEdit.showEvent(self, event)
+        self.shown.emit()
+
+    def hideEvent(self, event):
+        """
+        Parameters:
+                event=<QEvent>
+        """
+        self.clear()
 
+        QtWidgets.QTextEdit.hideEvent(self, event)
+        self.hidden.emit()
 
 
+# --------------------------------------------------------------------------------------------
 
 if __name__ == "__main__":
-	import sys
-	app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(sys.argv) #return the existing QApplication object, or create a new one if none exists.
-		
-	w = TextEdit()
+    import sys
+
+    app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(
+        sys.argv
+    )  # return the existing QApplication object, or create a new one if none exists.
 
-	w.insertText('Selected: <font style="color: Yellow;">8 <font style="color: LightGray;">/1486 faces')
-	w.insertText('Previous Camera: <font style="color: Yellow;">Perspective')
+    w = TextEdit()
 
-	w.show()
-	sys.exit(app.exec_())
+    w.insertText(
+        'Selected: <font style="color: Yellow;">8 <font style="color: LightGray;">/1486 faces'
+    )
+    w.insertText('Previous Camera: <font style="color: Yellow;">Perspective')
 
+    w.show()
+    sys.exit(app.exec_())
 
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
-'''
+"""
 Promoting a widget in designer to use a custom class:
->	In Qt Designer, select all the widgets you want to replace, 
-		then right-click them and select 'Promote to...'. 
+>   In Qt Designer, select all the widgets you want to replace, 
+        then right-click them and select 'Promote to...'. 
 
->	In the dialog:
-		Base Class:		Class from which you inherit. ie. QWidget
-		Promoted Class:	Name of the class. ie. "MyWidget"
-		Header File:	Path of the file (changing the extension .py to .h)  ie. myfolder.mymodule.mywidget.h
-
->	Then click "Add", "Promote", 
-		and you will see the class change from "QWidget" to "MyWidget" in the Object Inspector pane.
-'''
+>   In the dialog:
+        Base Class:     Class from which you inherit. ie. QWidget
+        Promoted Class: Name of the class. ie. "MyWidget"
+        Header File:    Path of the file (changing the extension .py to .h)  ie. myfolder.mymodule.mywidget.h
+
+>   Then click "Add", "Promote", 
+        and you will see the class change from "QWidget" to "MyWidget" in the Object Inspector pane.
+"""
 
 # deprecated: -----------------------------------
 
-# if pm.progressBar ("progressBar_", query=1, isCancelled=1):
-	# break
+# if pm.progressBar ("progressBar_", q=True, isCancelled=1):
+# break
 
 
-	# def insertText(self, dict_):
-	# 	'''
-	# 	Parameters:
-	# 		dict_ = {dict} - contents to add.  for each key if there is a value, the key and value pair will be added.
-	# 	'''
-	# 	highlight = QtGui.QColor(255, 255, 0)
-	# 	baseColor = QtGui.QColor(185, 185, 185)
-
-	# 	#populate the textedit with any values
-	# 	for key, value in dict_.items():
-	# 		if value:
-	# 			self.setTextColor(baseColor)
-	# 			self.append(key) #Appends a new paragraph with text to the end of the text edit.
-	# 			self.setTextColor(highlight)
-	# 			self.insertPlainText(str(value)) #inserts text at the current cursor position.
+# def insertText(self, dict_):
+#   '''
+#   Parameters:
+#       dict_ = {dict} - contents to add.  for each key if there is a value, the key and value pair will be added.
+#   '''
+#   highlight = QtGui.QColor(255, 255, 0)
+#   baseColor = QtGui.QColor(185, 185, 185)
+
+#   #populate the textedit with any values
+#   for key, value in dict_.items():
+#       if value:
+#           self.setTextColor(baseColor)
+#           self.append(key) #Appends a new paragraph with text to the end of the text edit.
+#           self.setTextColor(highlight)
+#           self.insertPlainText(str(value)) #inserts text at the current cursor position.
```

### Comparing `uitk-0.6.7/uitk.egg-info/PKG-INFO` & `uitk-0.6.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.6.7
+Version: 0.6.8
 Summary: uitk is a versatile package for managing user interfaces, widgets, and event handling in Python using PySide2. Using naming convention, the switchboard module provides a convenient way to load UI files, register custom widgets, manage slots and styles, and interact with widgets. It aims to simplify the development and management of complex user interfaces.
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: COPYING.LESSER
 
 ## UITK
 
 <!-- short_description_start -->
 uitk is a versatile package for managing user interfaces, widgets, and event handling in Python using PySide2. Using naming convention, the switchboard module provides a convenient way to load UI files, register custom widgets, manage slots and styles, and interact with widgets. It aims to simplify the development and management of complex user interfaces.
 <!-- short_description_end -->
 
@@ -59,36 +62,39 @@
 from uitk import Switchboard
 
 class MyProject():
     ...
 
 class MySlots(MyProject):
     def __init__(self):
-        self.sb = self.get_switchboard_instance()
+        self.sb = self.switchboard() #returns the switchboard instance.
 
     def MyButtonsObjectName(self):
         print("Button clicked!")
 
 
 sb = Switchboard(slots_location=MySlots)
-ui = sb.example #Get the UI using it's name (or sb.getUi(<name>))
+ui = sb.example #Get the UI using it's name (or sb.get_ui(<name>))
 
+# Some of the UI properties:
 print ('ui:'.ljust(20), sb.ui) #The current UI
 print ('ui name:'.ljust(20), ui.name) #The UI's filename.
 print ('ui path:'.ljust(20), ui.path) #The directory path containing the UI file
 print ('ui tags:'.ljust(20), ui.tags) #Any UI tags as a list
 print ('ui level:'.ljust(20), ui.level) #The UI level
-print ('is current ui:'.ljust(20), ui.isCurrentUi) #True if the UI is set as current
+print ('is current ui:'.ljust(20), ui.is_current) #True if the UI is set as current
 print ('is submenu:'.ljust(20), ui.isSubmenu) #True if the UI is a submenu
-print ('is connected:'.ljust(20), ui.isConnected) #True if the UI is connected to its slots
-print ('is initialized:'.ljust(20), ui.isInitialized) #True after the UI is first shown
+print ('is connected:'.ljust(20), ui.is_connected) #True if the UI is connected to its slots
+print ('is initialized:'.ljust(20), ui.is_initialized) #True after the UI is first shown
+print ('slot:'.ljust(20), ui.MyButtonsObjectName.get_slot()) #The associated slot
 print ('slots:'.ljust(20), ui.slots) #The associated slots class instance
-print ('slot:'.ljust(20), ui.MyButtonsObjectName.getSlot()) #The associated slot
-print ('widget from slot:'.ljust(20), sb.getWidgetFromMethod(ui.MyButtonsObjectName.getSlot()))
 print ('widget:'.ljust(20), ui.MyButtonsObjectName) #Get a widget from the UI by it's name
 print ('widgets:'.ljust(20), [(w.name or w.type) for w in ui.widgets]) #All widgets of the UI
 
+# There are also many helper methods that you can access through your switchboard instance:
+print ('widget from slot:'.ljust(20), sb.get_widget_from_method(ui.MyButtonsObjectName.get_slot()))
+
 ui.show(app_exec=True)
 ```
 ## Advanced Example:
 
 https://github.com/m3trik/tentacle
```

### Comparing `uitk-0.6.7/uitk.egg-info/SOURCES.txt` & `uitk-0.6.8/uitk.egg-info/SOURCES.txt.bak`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 uitk.egg-info/dependency_links.txt
 uitk.egg-info/top_level.txt
 uitk/widgets/MainWindow.py
 uitk/widgets/__init__.py
 uitk/widgets/attributes.py
 uitk/widgets/checkBox.py
 uitk/widgets/comboBox.py
-uitk/widgets/draggable_header.py
+uitk/widgets/draggableHeader.py
 uitk/widgets/label.py
 uitk/widgets/lineEdit.py
 uitk/widgets/listWidget.py
 uitk/widgets/mainWindow.py
 uitk/widgets/menu.py
 uitk/widgets/messageBox.py
 uitk/widgets/progressBar.py
 uitk/widgets/pushButton.py
 uitk/widgets/pushButtonDraggable.py
-uitk/widgets/pushButton_optionBox.py
+uitk/widgets/optionBox.py
 uitk/widgets/region.py
 uitk/widgets/task.py
 uitk/widgets/text.py
 uitk/widgets/textEdit.py
```

