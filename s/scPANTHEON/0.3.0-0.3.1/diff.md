# Comparing `tmp/scPANTHEON-0.3.0.tar.gz` & `tmp/scPANTHEON-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.0.tar", last modified: Fri May 12 03:09:44 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.1.tar", last modified: Thu Jun 22 15:04:34 2023, max compression
```

## Comparing `scPANTHEON-0.3.0.tar` & `scPANTHEON-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 03:09:44.184852 scPANTHEON-0.3.0/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-05-12 03:09:44.183846 scPANTHEON-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 03:09:44.169514 scPANTHEON-0.3.0/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-05-12 03:09:44.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 03:09:44.181840 scPANTHEON-0.3.0/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.0/scpantheon/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-05-08 07:38:57.000000 scPANTHEON-0.3.0/scpantheon/bokeh_qt.py
--rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.0/scpantheon/data_qt.py
--rw-rw-rw-   0        0        0     1162 2023-05-08 06:41:40.000000 scPANTHEON-0.3.0/scpantheon/main.py
--rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.0/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.0/scpantheon/run.py
--rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.3.0/scpantheon/save_qt.py
--rw-rw-rw-   0        0        0    59950 2023-05-12 02:56:06.000000 scPANTHEON-0.3.0/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.0/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-05-12 03:09:44.184926 scPANTHEON-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-05-12 03:09:29.000000 scPANTHEON-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:04:34.625556 scPANTHEON-0.3.1/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-06-22 15:04:34.624454 scPANTHEON-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 15:04:34.611640 scPANTHEON-0.3.1/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 15:04:34.623400 scPANTHEON-0.3.1/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.1/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-06-08 07:21:40.000000 scPANTHEON-0.3.1/scpantheon/bokeh_qt.py
+-rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.1/scpantheon/data_qt.py
+-rw-rw-rw-   0        0        0     1122 2023-05-18 11:21:14.000000 scPANTHEON-0.3.1/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.1/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.1/scpantheon/run.py
+-rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.3.1/scpantheon/save_qt.py
+-rw-rw-rw-   0        0        0    60638 2023-06-22 14:44:00.000000 scPANTHEON-0.3.1/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.1/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 15:04:34.625556 scPANTHEON-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-06-22 15:04:19.000000 scPANTHEON-0.3.1/setup.py
```

### Comparing `scPANTHEON-0.3.0/scpantheon/bokeh_qt.py` & `scPANTHEON-0.3.1/scpantheon/bokeh_qt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os, sys
 from PyQt5.QtWidgets import *
-from PyQt5.QtWebEngineWidgets import QWebEngineView
+from PyQt5.QtWebEngineWidgets import QWebEngineView, QWebEngineProfile
 from PyQt5 import QtCore, QtGui
+from PyQt5.QtCore import QUrl, QStandardPaths
 # import mysql.connector
 from pathlib import Path
 from appdirs import AppDirs
+from PyQt5.QtNetwork import QNetworkCookieJar
 
 sys.path.append(str(Path(__file__).resolve().parents[1]))
 
 class Ui_Dialog(QWidget, object):
     def setupUi(self, Dialog):
         Dialog.setObjectName("ScPantheon")
         Dialog.resize(1600,1000)
@@ -39,15 +41,17 @@
         self.retranslateUi(Dialog) 
         self.buttonBox.accepted.connect(Dialog.accept)
         self.buttonBox.rejected.connect(Dialog.reject)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
 
 
     def loadPage(self):
+        # self.webEngineView.load(QUrl("http://baidu.com"))
         Func = open("embed.html","w")
+        # 编写html
         Func.write("<!doctype html>\n<html>\n<iframe src='http://localhost:5006/'\nname='thumbnails'\nframeborder='0'\nstyle='width: 100%; height: 2000px;'>\n</html>")
         Func.close()
         with open('embed.html', 'r') as f:
             html = f.read()
             self.webEngineView.setHtml(html)
 
     def retranslateUi(self, Dialog):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scPANTHEON-0.3.0/scpantheon/data_qt.py` & `scPANTHEON-0.3.1/scpantheon/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.0/scpantheon/main.py` & `scPANTHEON-0.3.1/scpantheon/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 import warnings
 
 from bokeh.server.server import Server
 import multiprocessing
 import warnings
 
-from scpantheon import bokeh_qt, data_qt
+import bokeh_qt, data_qt
 
 class InstallWarning(Warning):
     def __init__(self, message):
         self.message = message
     def __str__(self):
         return repr(self.message)
-        
+
 try: 
-    from scpantheon import source # import from online
+    import source # import from online
 except:
     warnings.warn('YOU HAVE TO INSTALL PyQt5',InstallWarning)
 
 def run():
     global server
     print('Opening Bokeh application on http://localhost:5006/')
     server = Server({'/': source.main},
```

### Comparing `scPANTHEON-0.3.0/scpantheon/qt.py` & `scPANTHEON-0.3.1/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.0/scpantheon/save_qt.py` & `scPANTHEON-0.3.1/scpantheon/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.0/scpantheon/source.py` & `scPANTHEON-0.3.1/scpantheon/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                     self.data_log[view_name+str(i)] = self.data_df[view_name+str(i)]
             view_existed = True
         else:
             view_existed = False
         #self.source = ColumnDataSource(data=self.adata[:,0:2])
         self.view = CDSView(source=self.source, filters=[IndexFilter([i for i in range(self.data_df.shape[0])])])
         self.cur_color = color_list[0]
-        self.p = figure(width=500, height=500, tools="pan,lasso_select,box_select,tap,wheel_zoom,save,hover",title=title, tooltips=TOOLTIPS)
+        self.p = figure(width=500, height=500, tools="pan,lasso_select,box_select,tap,wheel_zoom,save,hover",title=title, tooltips=TOOLTIPS, output_backend="webgl")
         #self.p.output_backend = "svg"
         #print("backend is ", self.p.output_backend)        
         if view_existed:
             view_list = list(self.adata.obsm.keys())+['generic_columns']
             self.choose_panel = Select(title='Choose map:', value=view_list[0], options=view_list)
             self.data_columns = list([self.choose_panel.value +str(i) for i in range(self.adata.obsm[self.choose_panel.value].shape[1])])
             self.source.data = self.data_df[self.data_columns[0:2]+['color']+['hl_gene']]
@@ -140,16 +140,17 @@
         # Export Button
         self.export_button = Button(label='Export Results')
         self.export_button.on_click(self.save_profile)
 
         ### Class Group Functions Buttons ###
         # Select class group
         if self.label_existed:
-            group_list = list(self.adata.uns['category_dict'].keys())
+            group_list = list(self.adata.uns['category_dict'].keys()) 
             self.group = Select(title='Select Cluster Group:', options=group_list, value=group_list[-1])
+            #self.group = Select(title='Select Cluster Group:',options=[' '],value=' ')
             # self.update_checkbox()
             # self.show_color()
         else:
             self.group = Select(title='Select Cluster Group:',options=[' '],value=' ')
         self.group.on_change('value', lambda attr, old, new: self.choose_cat())
         # Input name of new category
         self.group_name = TextInput(title='Input Group Name: ', value='')
@@ -287,25 +288,28 @@
             column_list = list(self.adata.var.index)
         self.s_x.completions = column_list
         self.s_y.completions = column_list
 
         print(column_list)
 
     def save_profile(self):
+        global dir
         self.button_disabled()
         def next_save(self):
             if save_qt.main() == 'app closed':
                 print('choosing finished')
             path = get_save_path(dir) + '/'
+            text_cover(dir, path + 'result.h5ad') # write the output anndata to cover the data
+            print("path covered to " + path + "result.h5ad")
             try:
-                self.adata.write(path+'result.h5ad') 
+                self.adata.write_h5ad(path+'result.h5ad') 
                 self.adata.obs.to_csv(path+'cluster.csv')
             except:
                 os.makedirs(path)
-                self.adata.write(path+'result.h5ad') # ??
+                self.adata.write_h5ad(path+'result.h5ad') 
                 self.adata.obs.to_csv(path+'cluster.csv')
             # for cate in list(self.adata.uns['category_dict'].keys()):
             #     self.adata.obs[cate].to_csv(path+'%s.csv'%cate)
             #adata.uns['category_dict']('cluster name.csv') 
             self.button_abled()
         curdoc().add_next_tick_callback(lambda : next_save(self))
 
@@ -389,15 +393,15 @@
             remain_indices = [x for x in self.view.filters[0].indices if x not in self.source.selected.indices]
             self.view.filters = [IndexFilter(remain_indices)]
             self.button_abled()
         curdoc().add_next_tick_callback(lambda : next_remove)
 
     def showall_func(self):
         self.button_disabled()
-        def next_showall():
+        def next_showall(self):
             self.view.filters = list([])
             self.button_abled()
         curdoc().add_next_tick_callback(lambda : next_showall(self))
 
     # Show the saved color of dots
     def correct_func(self):
         self.source.selected.indices = []
@@ -1146,53 +1150,65 @@
     # models.visible = False
     # module_checkbox.active.remove(int(ind))
 
 def upload_callback(): 
 
     global extension_path
     global data_file
-    global mycursor, Main_plot
+    global Main_plot
 
     # path_, file_name = fetch()
     loading_remind = Div(text='Loading data……')
     curdoc().add_root(loading_remind) 
     print('===loading finished=====')
     filename = os.path.split(data_file)[1]      
     def load():
         global Main_plot
         filetype = os.path.splitext(filename)[-1][1:] # split the filename and the type
                                                       # [-1] means the last tuple: the type 
         if filetype == 'csv':
             adata = sc.read_csv(data_file) 
             print('csv')
         elif filetype == 'h5ad':
-            adata = sc.read_h5ad(data_file)
+            # adata = sc.read_h5ad(data_file)
+            adata = anndata.read(data_file, backed='r')
             print('h5ad')
         elif filetype == 'mtx':
             adata = sc.read_10x_mtx(
                 'data/hg19/',  # the directory with the `.mtx` file
                 var_names='gene_symbols',                # use gene symbols for the variable names (variables-axis index)
                 cache=True)                              # write a cache file for faster subsequent reading
         print(data_file)
         # Figure, layout
         mainplot, panel1 = CreateTool(adata=adata).base_tool() # Mainplot: figure, layout
         print('===mainplot finished=====')
         Main_plot = mainplot
-        # Highlight Gene Figure,
+        # Highlight Gene Figure
         hl_figure, panel2 = CreateTool(adata=adata).highlight_gene(mainplot)
         print('====highlight finished=====')
         tab = CreateTool(adata).multi_panel([mainplot,hl_figure], [panel1,panel2], ['Main View', 'Highlight Gene'], update_view=True)
         print('====tab====')
         curdoc().remove_root(loading_remind)
         curdoc().add_root(tab)
         print('===finish===')
 
     curdoc().add_next_tick_callback(load)
 
 
+def text_cover(dir, msg):
+    path = dir + '/data_file.txt'
+    print("-========- path:", path)
+    with open(path, "w") as f:
+        f.truncate(0)
+        f.close()
+    file = open(path, 'w')
+    file.write(msg)
+    file.close()
+
+
 def openreadtxt(dir):
     e_file = open(dir + '/' + 'extension_path.txt', 'r')
     e_path = e_file.readline()
     e_file.close()
     print('-======- e_path:', e_path)
     d_file = open(dir + '/' + 'data_file.txt', 'r')
     data = d_file.readline()
@@ -1213,21 +1229,21 @@
     global Main_plot, extension_path, data_file, dir
     appname = "scpantheon"
     appauthor = "xinzhu"
     version = "0.2.1"
     dirs = AppDirs(appname, appauthor, version)
     dir = dirs.user_data_dir
     # read path_ and file from user_data_dir
-    extension_path, data_file = openreadtxt(dir) 
+    extension_path, data_file = openreadtxt(dir)                                                                                              
     
     '''
     global mycursor
     try: myconnect()
     except:
-        try: creatbase()
+        try: creatbase() 
         except: ()
     try: creatable()
     except: ()
     try:
         path_, file_name = fetch()
     except:
         print('Please Choose your Extensions and Data paths\n')
```

### Comparing `scPANTHEON-0.3.0/scpantheon/transform.py` & `scPANTHEON-0.3.1/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.0/setup.py` & `scPANTHEON-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.0',#版本
+    version='0.3.1',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
```

