# Comparing `tmp/yunxiao-0.2.9.tar.gz` & `tmp/yunxiao-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.9.tar", last modified: Thu Jun 22 17:41:19 2023, max compression
+gzip compressed data, was "yunxiao-0.3.0.tar", last modified: Thu Jun 22 18:06:56 2023, max compression
```

## Comparing `yunxiao-0.2.9.tar` & `yunxiao-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.360899 yunxiao-0.2.9/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     6351 2023-06-22 17:41:19.359861 yunxiao-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.2.9/README.md
--rw-rw-rw-   0        0        0     1290 2023-06-22 17:41:06.000000 yunxiao-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 17:41:19.360899 yunxiao-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.351755 yunxiao-0.2.9/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.9/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.354291 yunxiao-0.2.9/yunxiao/
--rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.2.9/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    32806 2023-06-22 17:34:42.000000 yunxiao-0.2.9/yunxiao/v2.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.9/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.358848 yunxiao-0.2.9/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     6351 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.168314 yunxiao-0.3.0/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-06-22 18:06:56.168314 yunxiao-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1290 2023-06-22 18:04:51.000000 yunxiao-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 18:06:56.168314 yunxiao-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.158690 yunxiao-0.3.0/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.161206 yunxiao-0.3.0/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.0/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    32818 2023-06-22 18:04:22.000000 yunxiao-0.3.0/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.0/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:06:56.167302 yunxiao-0.3.0/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 18:06:56.000000 yunxiao-0.3.0/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.9/LICENSE` & `yunxiao-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.9/PKG-INFO` & `yunxiao-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.9
+Version: 0.3.0
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.9/README.md` & `yunxiao-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.9/pyproject.toml` & `yunxiao-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.9"
+version = "0.3.0"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.2.9/yunxiao/v2.py` & `yunxiao-0.3.0/yunxiao/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 "endDate": end_date,
                 "teacherIds": [teacher_id],
                 "reserve": 0,
                 "displayCompletedClass": False,
                 "courseStatusList": [],
                 "page": {"pageNum": 1, "pageSize": 999}
             }
-        )
+        )["data"]
 
     # 查询学生
     @loop("")
     def students_query(self, page, size, curriculumids: tuple = (), classids: tuple = (), name: str = "",
                        status: tuple = (1, 7), class_student_status: int = 0):
         """
         查询学生
@@ -325,15 +325,15 @@
             method="get",
             url="https://yunxiao.xiaogj.com/api/cs-crm/student/getContainFace",
             params={
                 "_t_": UsedTime.stamp,
                 "id": studentid,
                 "companyId": companyid
             }
-        )
+        )["data"]
 
     # 查询学生课程卡包
     def student_query_cards(self, studentid: int) -> list:
         """
         查看学员的课程卡包
         :param studentid: 学生ID
         :return: json数据
@@ -801,40 +801,40 @@
                 "endTime": enddate,
                 "displayInvalidOrder": True
             }
         )["data"]
 
     # 查询业绩归属
     @loop("achievementBelongerDetailItems")
-    def payments_query_achievements_datarange(self, startdate: str = "", enddate: str = "", productName: str = ""):
+    def payments_query_achievements_datarange(self, page, size, startdate: str = "", enddate: str = ""):
         """
-        列出指定操作日期范围的所有订单记录
-        :param productName: 项目名称
+        查询业绩归属，根据日期
+        :param size: 分页查询，每页数量
+        :param page: 分页查询，起始页码，应设为 0
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
             json={
                 "_t_": UsedTime.stamp,
-                "page": {"pageNum": 1, "pageSize": 10000},
+                "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "startTime": startdate,
-                "endTime": enddate,
-                "productName": productName
+                "endTime": enddate
             }
         )
 
-    # 查询业绩
+    # 查询业绩归属
     def payments_query_achievements(self, startdate: str = "", enddate: str = "", productName: str = "",
                                     teacherIds: tuple = ()):
         """
-        列出指定操作日期范围的所有订单记录
+        查询业绩归属，根据信息
         :param teacherIds: 老师ID
         :param productName: 项目名称
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
         :return:
         """
         return self.request(
@@ -846,15 +846,15 @@
                 "campusIds": self.campus,
                 "startTime": startdate,
                 "endTime": enddate,
                 "productName": productName,
                 "teacherIds": list(teacherIds),
                 "orderTypes": [0]
             }
-        )
+        )["data"]
 
     # 查询招生来源
     def comefroms_query(self):
         return self.request(
             method="get",
             url=f"https://yunxiao.xiaogj.com/api/cs-crm/customField/get",
             params={"_t_": UsedTime.stamp, "customFieldId": "26118419"}
```

### Comparing `yunxiao-0.2.9/yunxiao/yunxiao.py` & `yunxiao-0.3.0/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.9/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.3.0/yunxiao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.9
+Version: 0.3.0
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

