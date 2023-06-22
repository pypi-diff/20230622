# Comparing `tmp/sprites-1.72.tar.gz` & `tmp/sprites-1.721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprites-1.72.tar", last modified: Wed Jun 21 07:38:40 2023, max compression
+gzip compressed data, was "sprites-1.721.tar", last modified: Thu Jun 22 09:48:07 2023, max compression
```

## Comparing `sprites-1.72.tar` & `sprites-1.721.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:38:40.607067 sprites-1.72/
--rw-rw-rw-   0        0        0     2099 2023-06-21 07:38:40.606067 sprites-1.72/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2023-05-29 09:32:05.000000 sprites-1.72/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 07:38:40.611068 sprites-1.72/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-06-21 07:38:25.000000 sprites-1.72/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:38:40.536063 sprites-1.72/sprites/
--rw-rw-rw-   0        0        0  1439652 2023-06-21 07:37:56.000000 sprites-1.72/sprites/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:38:40.595067 sprites-1.72/sprites.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 07:38:34.000000 sprites-1.72/sprites.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 09:48:07.854979 sprites-1.721/
+-rw-rw-rw-   0        0        0     2100 2023-06-22 09:48:07.852979 sprites-1.721/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2023-05-29 09:32:05.000000 sprites-1.721/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 09:48:07.856979 sprites-1.721/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2023-06-22 09:47:36.000000 sprites-1.721/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 09:48:07.802976 sprites-1.721/sprites/
+-rw-rw-rw-   0        0        0  1439535 2023-06-22 09:46:38.000000 sprites-1.721/sprites/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 09:48:07.845979 sprites-1.721/sprites.egg-info/
+-rw-rw-rw-   0        0        0     2100 2023-06-22 09:48:07.000000 sprites-1.721/sprites.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-22 09:48:07.000000 sprites-1.721/sprites.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 09:48:07.000000 sprites-1.721/sprites.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 09:48:03.000000 sprites-1.721/sprites.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-22 09:48:07.000000 sprites-1.721/sprites.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 09:48:07.000000 sprites-1.721/sprites.egg-info/top_level.txt
```

### Comparing `sprites-1.72/PKG-INFO` & `sprites-1.721/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.72
+Version: 1.721
 Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
```

### Comparing `sprites-1.72/README.md` & `sprites-1.721/README.md`

 * *Files identical despite different names*

### Comparing `sprites-1.72/setup.py` & `sprites-1.721/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding='utf-8') as fh:
     long_d = fh.read()
 
 
 setup(name='sprites',
       long_description_content_type="text/markdown",
-      version = '1.72',
+      version = '1.721',
       description = 'Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com',
       long_description = long_d,      
       keywords = 'creative game pygame turtle animation sprite geometry math Elementary Mathematics Teaching',
       url = 'http://www.lixingqiu.com',
       wechat = 'scratch8',
       author ='lixingqiu',
       author_email = '406273900@qq.com',
```

### Comparing `sprites-1.72/sprites/__init__.py` & `sprites-1.721/sprites/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 from copy import deepcopy
 from tkinter import filedialog
 from tkinter import colorchooser
 from winsound import PlaySound,SND_ASYNC,SND_LOOP,SND_PURGE
 from PIL import ImageTk,ImageOps,Image,ImageGrab,ImageDraw,ImageFont,ImagePath,ImageColor
 from turtle import TK,_Root,ScrolledCanvas,_CFG ,TNavigator,Tbuffer,TPen,_Screen,Screen,Turtle,Vec2D, RawTurtle,TurtleScreenBase,Shape,TurtleScreen,_TurtleImage,TurtleGraphicsError 
 
-_VERSION = 1.72 
+_VERSION = 1.721 
 _CFG['delay'] = 0
 # 定义资源文件夹
 _resfld = os.path.join(os.getcwd(),'res')
 if not os.path.exists(_resfld):os.mkdir(_resfld)
 
 class InputBox:
     def __init__(self,master,title='输入对话框',prompt='请输入字符:'):
@@ -1472,15 +1472,15 @@
     
 def lc_intersection(line,circle):  # 直线与圆的交点
     """返回直线和圆的交点  
        line是用两点表示的直线,形如,((32,99),(0,0))或[(32,99),(0,0)]
        circle: 用圆心和半径表示的圆形，如[(0,0),100]，表示圆心在原点，半径为100的圆
     """
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem()   # 弹出项目
     else:
         center = circle[0]                 # 取出圆心
         radius = circle[-1]                # 取出半径 
 
     _,_,_,m,c = twopointoneline(*line) # 算出直线一般式的参数,用斜截式,所以前三个参数不要
    
     p,q = center   # 下面根据y=mx+c和(x-p)**2+(y-q)**2=r**2解方程得
@@ -1523,15 +1523,15 @@
             
             return [(x,y1),(x,y2)]
 
 def is_on_circle(point,circle):
     """判断点是否在圆上
        point:用二元组表示的点,circle:中心点与半径表示的圆,如((0,0),100)"""
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem()    # 弹出项目
     else:
         center = circle[0]                 # 取出圆心
         radius = circle[-1]                # 取出半径    
     a,b = center
     x,y = point
     # 下面根据圆的标准方程判断x,y是否在圆上
     return  (x-a)**2 + (y-b)**2 == radius**2 
@@ -1539,18 +1539,18 @@
 dot_is_on_circle = is_on_circle
 
 def cc_intersection(circle1,circle2):  # 圆与圆的交点
     """返回两个圆的交点，圆形用((10,10),50))或者[(10,10),50)]这样的数据表示。
        如赋值：circle1 = (c,r)，则c应该是用二元组表示的圆心,r应该是半径。
     """
     if isinstance(circle1,dict):
-        radius,center = circle1.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle1.copy().popitem() # 弹出项目
         circle1 = (center,radius)
     if isinstance(circle2,dict):
-        radius,center = circle2.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle2.copy().popitem() # 弹出项目
         circle2 = (center,radius)
         
     # 如果第一个圆更小,则交换,
     if circle1[-1] < circle2[-1]:
         circle1,circle2 = circle2,circle1
     c1,r1 = circle1           # 这个是更大的圆
     c2,r2 = circle2
@@ -1832,15 +1832,15 @@
 
 def circle_on_tangent(circle,point,length=100): # 圆上切线 
     """圆上的切线,默认长度100),返回两个点
        circle：圆形，用[(0,0),100]这样的数据表示一个圆
        point：点，用二元组表示的点，如(10,10)
     """
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem()     # 弹出项目
     else:
         center,radius = circle
     p = point
     t = Pointer(pos=center)
     j = t.towards(p);t.setheading(j)
     t.fd(radius); t.left(90);t.fd(length/2);dot1 = t.position()
     t.bk(length);dot2 = t.position()
@@ -1848,15 +1848,15 @@
 
 def circle_out_tangent(circle,point):   # 圆外切线
     """圆外一点到圆的两条切线,返回两个点
        circle：圆形，用[(0,0),100]这样的数据表示一个圆
        point：点，用二元组表示的点，如(10,10)
     """
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem() # 弹出项目
     else:
         center,radius = circle
     p = point
     dis = math.dist(center,p)
     if dis > radius:
         t = Pointer(pos=p)
         j = t.towards(center);t.setheading(j)
@@ -1867,15 +1867,15 @@
         return dot1,dot2    
 
 def circle_in_random_point(circle,dist=1):
     """圆内随机点
        circle：是形如[(10,10),100]这样的数据，列表中的数据表示圆心和半径
     """
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem()   # 弹出项目
     else:
         center = circle[0]                 # 取出圆心
         radius = circle[-1]                # 取出半径 
 
     t = Pointer(pos=center)
     angle = random.randint(1,360)
     t.setheading(angle)
@@ -1883,15 +1883,15 @@
     return dot
   
 def circle_on_random_point(circle):
     """圆上随机点
        circle：是形如[(10,10),100]这样的数据，列表中的数据表示圆心和半径
     """
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem()   # 弹出项目
     else:
         center = circle[0]                 # 取出圆心
         radius = circle[-1]                # 取出半径 
 
     t = Pointer(pos=center)
     angle = random.randint(1,360)
     t.setheading(angle)
@@ -1899,15 +1899,15 @@
     return dot
   
 def circle_out_random_point(circle,limits=(1,5)):
     """圆外随机点
        circle：是形如[(10,10),100]这样的数据，列表中的数据表示圆心和半径
     """
     if isinstance(circle,dict):
-        radius,center = circle.popitem()        # 弹出项目，此时字典已空
+        radius,center = circle.copy().popitem() # 弹出项目
     else:
         center = circle[0]                 # 取出圆心
         radius = circle[-1]                # 取出半径
     t = Pointer(pos=center)
     angle = random.randint(1,360)
     t.setheading(angle)
     d = radius + radius*random.uniform(*limits)
@@ -2118,23 +2118,23 @@
     """运用海伦公式求三角形面积，A，B，C是三个不共线的坐标点
     """
     a = math.dist(B,C);b = math.dist(A,C);c = math.dist(B,A)
     p = (a+b+c)/2
     return (math.sqrt(p*(p-a)*(p-b)*(p-c)),p ) # 注意返回的是面积与周长的一半
     
 def circumcircle(A,B,C):              # 三点定圆
-    """返回外接圆,A,B,C是不共线的三个点"""
+    """返回外接圆的圆心和半径,A,B,C是不共线的三个点"""
     a = math.dist(B,C);b = math.dist(A,C);c = math.dist(B,A)
     p = (a+b+c)/2
     s = math.sqrt(p*(p-a)*(p-b)*(p-c))
     r = a*b*c/(4*s)
     return (circumcenter(A,B,C),r)
 
 def incircle(A,B,C):
-    """返回内切圆,A,B,C是不共线的三个点"""
+    """返回内切圆的圆心和半径,A,B,C是不共线的三个点"""
     s,p = heron_formula(A,B,C)  # 返回的三角形面积和周长的一半
     r = s/p
     return (incenter(A,B,C),r)
 
 def inflection_points(polyline):
     """返回折线的拐点,polyline是一个点集，如[(0,0),(10,10),(20,20),(20,30)]"""
     points = polyline
@@ -4560,16 +4560,15 @@
         else:
             self.penup()
             self.goto(p1)              # 到达第一个点
             self.pendown()
             self.goto(p2)              # 到达第二个点
             self.penup()
         return dist
-
-
+    
     def draw_circle(self,p1,p2,degrees=360,isfill=False,shape='fan'):
         """以p1和p2为直径画圆，p1和p2为坐标点,degrees为度数,filled为是否填充,
            shape的取值为bow或者fan,为bow是画的是弓形,为fan时画的是扇形。
         """
         diameter = ((p1[0]-p2[0])**2 + (p1[1]-p2[1])**2)**0.5 # 两点距离
         radius = diameter /2        # 半径
         mid = midpoint(p1,p2)       # 中点
@@ -4718,15 +4717,15 @@
         fc = self.fillcolor()         # 填充颜色
         if isinstance(fc,tuple) and self.screen.colormode()==255:
             fc = int(fc[0]),int(fc[1]),int(fc[2])
         start = x,y
         screen = self.getscreen()
         tr = screen.tracer()
         screen.tracer(0,0)
-        contours,inners = self.find_contours(start) # 查找轮廓        
+        contours,inners = self.find_contours(start,{self.turtle._item}) # 查找轮廓        
         points = adjust_pts_order(contours)  # 点集以逆时钟排序
         isd = self.isdown()            # 记录当前是否落笔的状态    
         self.penup()                   # 不管当前是否有无落笔,都要抬笔
         self.goto(points[0])
         self.begin_fill()         
         [self.godot(x,y,1,fc) for x,y in points[1:] ]        
         self.goto(points[0])
```

### Comparing `sprites-1.72/sprites.egg-info/PKG-INFO` & `sprites-1.721/sprites.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.72
+Version: 1.721
 Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
```

