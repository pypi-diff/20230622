# Comparing `tmp/yunxiao-0.3.0.tar.gz` & `tmp/yunxiao-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.3.0.tar", last modified: Thu Jun 22 18:06:56 2023, max compression
+gzip compressed data, was "yunxiao-0.3.1.tar", last modified: Thu Jun 22 20:24:52 2023, max compression
```

## Comparing `yunxiao-0.3.0.tar` & `yunxiao-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.168314 yunxiao-0.3.0/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6351 2023-06-22 18:06:56.168314 yunxiao-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.0/README.md
--rw-rw-rw-   0        0        0     1290 2023-06-22 18:04:51.000000 yunxiao-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 18:06:56.168314 yunxiao-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.158690 yunxiao-0.3.0/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.0/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.161206 yunxiao-0.3.0/yunxiao/
--rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.0/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    32818 2023-06-22 18:04:22.000000 yunxiao-0.3.0/yunxiao/v2.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.0/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.167302 yunxiao-0.3.0/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     6351 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 20:24:52.001823 yunxiao-0.3.1/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-06-22 20:24:52.000814 yunxiao-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.1/README.md
+-rw-rw-rw-   0        0        0     1290 2023-06-22 20:24:32.000000 yunxiao-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:24:52.001823 yunxiao-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 20:24:51.991678 yunxiao-0.3.1/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:24:51.994731 yunxiao-0.3.1/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.1/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    34197 2023-06-22 20:24:23.000000 yunxiao-0.3.1/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.1/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:24:51.999806 yunxiao-0.3.1/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.3.0/LICENSE` & `yunxiao-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.0/PKG-INFO` & `yunxiao-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.0
+Version: 0.3.1
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.3.0/README.md` & `yunxiao-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.0/pyproject.toml` & `yunxiao-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.3.0"
+version = "0.3.1"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.3.0/yunxiao/v2.py` & `yunxiao-0.3.1/yunxiao/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,35 @@
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-report/report/findTuition",
             json={"campusIds": self.campus, "date": yy_mm, "dateType": 1, "_t_": UsedTime.stamp}
         )["data"]
 
         return list(map(lambda x: {**x[0], **x[1], **x[2]}, zip(course, refund, tuition)))
 
+    # 查询机构指定日期范围业绩。
+    def company_query_performance_daterange(self, startdate: str = UsedTime.yymm01,
+                                            enddate: str = UsedTime.today) -> list:
+        """
+        查询机构指定日期范围业绩。
+        :param startdate: 起始日期
+        :param enddate: 截止日期
+        :return:
+        """
+        return self.request(
+            method="post",
+            url="https://yunxiao.xiaogj.com/api/cs-report/report/findDataReportList",
+            json={
+                "campusIds": self.campus,
+                "startDate": startdate,
+                "endDate": enddate,
+                "orderByCampus": 1,
+                "_t_": UsedTime.stamp
+            }
+        )["data"]
+
     # 查询校区
     def campus_query(self) -> list:
         """
         查询全部校区
         :return:
         """
         return self.request(
@@ -410,15 +431,15 @@
                 "studentId": student_id,
                 "suspendCourseDate": suspend_course_date,
                 "type": 0
             }
         )
 
     # 设置学生为曾就读。
-    def student_operation__history(self, studentlist: tuple):
+    def student_operation_history(self, studentlist: tuple):
         """
         设置学生为曾就读。
         :param studentlist: 学生ID
         :return:
         """
         return self.request(
             method="post",
@@ -471,22 +492,23 @@
             }
         )["data"][0]["courseArrangeRecordVos"]
 
     # 查询某日到某日排课
     @loop("")
     def arranges_query_daterange(self, page, size, starttime: str = None, endtime: str = None, teacherids: tuple = (),
                                  studentids: tuple = (), displayCompletedClass: bool = False, before_today: int = 30,
-                                 after_today: int = 30):
+                                 after_today: int = 30, courseStatusList: tuple = (0, 1)):
         """
         查询某日到某日的排课。
-        :param studentids: 查询的学生列表
-        :param teacherids: 查询的教师列表
         :param size: 分页查询，每页数量
         :param page: 分页查询，起始页码，应设为 0
+        :param studentids: 查询的学生列表
+        :param teacherids: 查询的教师列表
         :param displayCompletedClass: 是否已结班排课
+        :param courseStatusList: 排课状态。 **0** 未点名 **1** 已点名 **2** 已取消
         :param before_today: 设定起始日期为今天之前的某天，当 starttime 留空时使用。
         :param after_today: 设定起始日期为今天之后的某天，当 endtime 留空时使用。
         :param starttime: 查询起始时间 **2020-02-20**
         :param endtime: 查询截止时间 **2020-03-20**
         :return:
         """
         starttime = time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)) \
@@ -499,30 +521,41 @@
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/arrange/page",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "startDate": starttime,
                 "endDate": endtime,
+                "courseStatusList": list(courseStatusList),
                 "teacherId": list(teacherids),
                 "studentIds": list(studentids),
                 "displayCompletedClass": displayCompletedClass,
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
 
     # 查询班级
     @loop("")
-    def classes_query(self, page, size, teacherids: tuple = (), classname: str = ""):
+    def classes_query(self, page, size, teacherids: tuple = (), classname: str = "", classStatus: int = 0):
+        """
+        查询班级
+        :param size: 分页查询，每页数量
+        :param page: 分页查询，起始页码，应设为 0
+        :param classname: 班级名称
+        :param classStatus: 班级状态。 **0** 未结班 **1** 已结班
+        :param teacherids: 老师ID
+        :return:
+        """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/classInfo/page",
             json={
                 "_t_": UsedTime.stamp,
                 "orgTag": 1,
+                "classStatus": classStatus,
                 "campusIds": self.campus,
                 "classname": classname,
                 "teacherIds": list(teacherids),
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
```

### Comparing `yunxiao-0.3.0/yunxiao/yunxiao.py` & `yunxiao-0.3.1/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.0/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.3.1/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.0
+Version: 0.3.1
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

