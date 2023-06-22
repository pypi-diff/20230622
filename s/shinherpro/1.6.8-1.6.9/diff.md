# Comparing `tmp/shinherpro-1.6.8.tar.gz` & `tmp/shinherpro-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.8.tar", last modified: Sun May 28 15:22:38 2023, max compression
+gzip compressed data, was "shinherpro-1.6.9.tar", last modified: Thu Jun 22 15:59:09 2023, max compression
```

## Comparing `shinherpro-1.6.8.tar` & `shinherpro-1.6.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 15:22:38.497342 shinherpro-1.6.8/
--rw-rw-rw-   0        0        0      178 2023-05-28 15:22:38.496845 shinherpro-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-28 15:22:38.497342 shinherpro-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-05-28 14:42:22.000000 shinherpro-1.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:22:38.487918 shinherpro-1.6.8/shinherpro/
--rw-rw-rw-   0        0        0    19609 2023-05-28 15:22:35.000000 shinherpro-1.6.8/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.8/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1293 2023-05-23 15:25:54.000000 shinherpro-1.6.8/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0    10438 2023-05-28 14:57:43.000000 shinherpro-1.6.8/shinherpro/html.py
--rw-rw-rw-   0        0        0     1186 2023-05-22 15:33:52.000000 shinherpro-1.6.8/shinherpro/serverLog.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.8/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:22:38.495854 shinherpro-1.6.8/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 15:59:09.367439 shinherpro-1.6.9/
+-rw-rw-rw-   0        0        0      178 2023-06-22 15:59:09.366943 shinherpro-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-22 15:59:09.367934 shinherpro-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-19 15:20:34.000000 shinherpro-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:59:09.352557 shinherpro-1.6.9/shinherpro/
+-rw-rw-rw-   0        0        0    20214 2023-06-22 15:52:20.000000 shinherpro-1.6.9/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.9/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-06-19 15:22:28.000000 shinherpro-1.6.9/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0      547 2023-06-22 15:54:06.000000 shinherpro-1.6.9/shinherpro/logSave.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.9/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:59:09.365951 shinherpro-1.6.9/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.8/setup.py` & `shinherpro-1.6.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.8',
-    description='shinher-pro 1.6.8',
+    version='1.6.9',
+    description='shinher-pro 1.6.9',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.8/shinherpro/TYAI.py` & `shinherpro-1.6.9/shinherpro/TYAI.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import numpy as np
 import cv2
 import time
 import json
 import os
 from shinherpro import vfcModel
 from shinherpro import chormeDriver
+from shinherpro import logSave
 import sys
 
 
 ###################################################
 # V 1.6.4 By Yihuan Studio --> 2023/5/21/05:09:19
 
 #############################################
@@ -35,44 +36,49 @@
 ##  image enhancement algorithm V1 By Sam
 
 RESET = "\033[0m"
 RED = "\033[31m"
 GREEN = "\033[32m"
 YELLOW = "\033[33m"
 
+global UserNameSave
+
 def urlGet():
     return "https://sai.tyai.tyc.edu.tw/online/"
 
+# get var to set driver and model
+def setup(driverIn,modelIn):
+    global driver,model
+    driver = driverIn
+    model = modelIn
+
 def score_tolist(new_page_source):
     
     html = new_page_source
     soup = BeautifulSoup(html, 'html.parser')
 
-    # 提取考試科目成績
     subject_scores = []
     rows = soup.select('table.t02 tr.row')
     for row in rows:
         subject = row.select_one('td.top').text.strip()
         score_elements = row.select('td.top.right span')
         if len(score_elements) >= 2:
             user_score = score_elements[0].text.strip()
             class_average = score_elements[1].text.strip()
             subject_scores.append({'考試科目': subject, '個人成績': user_score, '全班平均': class_average})
 
-    # 提取總分、平均分數、排名和科別排名
     total_score = soup.select_one('table.scoreTable-inline td.score').text.strip()
 
     average_score_elements = soup.select('table.scoreTable-inline td.score')
     average_score = average_score_elements[1].text.strip() if len(average_score_elements) >= 3 else "N/A"
 
     ranking_elements = soup.select('table.scoreTable-inline td.score')
     ranking = ranking_elements[2].text.strip() if len(ranking_elements) >= 3 else "N/A"
     department_ranking = ranking_elements[3].text.strip() if len(ranking_elements) >= 4 else "N/A"
 
-    # 建立包含所有資訊的字典
     result = {
         'code': 0,
         '考試標題': soup.select_one('.center.pt-2 .bluetext').text.strip(),
         '學號': soup.select_one('.center.mobile-text-center .mr-3-ow:nth-of-type(1)').text.strip().replace('學號：', ''),
         '姓名': soup.select_one('.center.mobile-text-center .mr-3-ow:nth-of-type(2)').text.strip().replace('姓名：', ''),
         '班級': soup.select_one('.center.mobile-text-center .mr-3-ow:nth-of-type(3)').text.strip().replace('班級：', ''),
         '考試科目成績': subject_scores,
@@ -95,15 +101,17 @@
         'vfcTryList': vfcTryList
     }
     ]
 
     result['log'] = new_log
     return result
 
-def login(username, password, driver, model,LowConfidence=85,stepPrint=False):
+def login(username, password,LowConfidence=85,stepPrint=False):
+    global UserNameSave
+    UserNameSave = username
     driver.delete_all_cookies()
     driver.refresh()
     try:
         if stepPrint == False :
             sys.stdout = open(os.devnull, 'w')
 
         start_time = time.time()
@@ -193,29 +201,37 @@
                 alert.dismiss()
                 if popup_text == "驗證碼輸入錯誤，請重新輸入。":
                     print("驗證碼輸入錯誤,重新嘗試")
                     vfcTryList.append("vfc wrong")
                     vfcTry = vfcTry + 1
                 elif popup_text == "帳號或密碼錯誤,請重新登入!":
                     if stepPrint==False : sys.stdout = sys.__stdout__
-                    return {'code':1,'runTime':time.time()-start_time,'result':False}
+                    returnLog = {'code':1,'runTime':time.time()-start_time,'result':False}
+                    logSave.addLog("Login",UserNameSave,returnLog)
+                    return returnLog
                 else:
                     reason = popup_text
                     if stepPrint==False : sys.stdout = sys.__stdout__
-                    return {'code':2,'runTime':time.time()-start_time,'result' : popup_text }
+                    returnLog = {'code':2,'runTime':time.time()-start_time,'result' : popup_text }
+                    logSave.addLog("Login",UserNameSave,returnLog)
+                    return returnLog
     
             except:
                 print(f"{GREEN}密碼正確.{RESET}",end="")
                 break
 
         print(f"{GREEN}驗證碼正確.{RESET}")
         if stepPrint==False : sys.stdout = sys.__stdout__
-        return {'code':0,'runTime':time.time()-start_time,'result':True}
+        returnLog = {'code':0,'runTime':time.time()-start_time,'result':True}
+        logSave.addLog("Login",UserNameSave,returnLog)
+        return returnLog
     except:
-        return {'code':33,'runTime':time.time()-start_time,'reason':'something Wrong'}
+        returnLog = {'code':33,'runTime':time.time()-start_time,'reason':'something Wrong'}
+        logSave.addLog("Login",UserNameSave,returnLog)
+        return returnLog
 
 def Credit_html_to_json(html):
     html_data = html
 
     soup = BeautifulSoup(html_data, 'html.parser')
 
     student_info = soup.find('div', class_='center').text.strip().split('\xa0')
@@ -266,15 +282,15 @@
         '不及格科目': subjects,
         '學分': merged_contents,
     }
 
     json_data = json.dumps(data, ensure_ascii=False)
     return json_data
 
-def getGrades(username,driver,examname,stepPrint=False):
+def getGrades(examname,stepPrint=False):
     driver.refresh()
     stepSave = 0
     try:
         stepSave = 1
 
         # 進入成績查詢頁面
         # 切換到左測選單
@@ -329,24 +345,29 @@
         driver.refresh()
 
         stepSave = 4
 
         JsonResult = JsonGrade
 
         if stepPrint==False : sys.stdout = sys.__stdout__
+        
+        logSave.addLog("GetGrade",UserNameSave,JsonResult)
         return JsonResult
 
 
     except Exception as e:
         error_message = str(e) 
         if stepPrint == False:
             sys.stdout = sys.__stdout__
-        return {'code': 33, 'reason': f'something Wrong, step {stepSave}try的錯誤原應: {error_message}'}
 
-def getCredit(username,driver,stepPrint=False):
+        JsonResult = {'code': 33, 'reason': f'something Wrong, step {stepSave}try的錯誤原應: {error_message}'}
+        logSave.addLog("GetGrade",UserNameSave,JsonResult)
+        return JsonResult
+
+def getCredit(stepPrint=False):
     driver.refresh()
     try:
         stepSave = 1
 
         # 進入成績查詢頁面
         # 切換到左測選單
         chormeDriver.switch_frame(False, ["left"], driver)
@@ -368,15 +389,15 @@
 
         if stepPrint==False : sys.stdout = sys.__stdout__
         return json_result
     except:
         if stepPrint==False : sys.stdout = sys.__stdout__
         return {'code':33,'reason':f'something Wrong ,step {stepSave}'}
      
-def getUserPhoto(username,driver):
+def getUserPhoto(username):
     driver.refresh()
     stepSave = 1
     try:
         chormeDriver.switch_frame(False, ["left"], driver)
     except:
         return {'code':1}
     student_data_link = driver.find_element(By.ID, 'lnkStudentData')  # 按鈕名稱 "學生 xxx 的資料"
@@ -395,15 +416,15 @@
     # 切換到框架"right"的框架"right_below"
     chormeDriver.switch_frame(True, ["right", "right_below"], driver)
     # 找到查詢資料按鈕
     button = driver.find_element(By.CSS_SELECTOR, "button[onclick*='window.open']")
     button.click()
     # 切換到框架"right"的框架"right_below"
     chormeDriver.switch_frame(True, ["right", "right_top"], driver)
-    # 找到各式成績查詢按鈕
+    # 找到查詢基本資料按鈕
     button = driver.find_element(By.XPATH, "//img[@title='查詢基本資料']")
     button.click()
     chormeDriver.switch_frame(True, ["right","right_below"], driver)
     new_page_source = driver.page_source
     #print(new_page_source)
     soup = BeautifulSoup(new_page_source, 'html.parser')
 
@@ -426,15 +447,15 @@
 
     screenshot = Image.open('PhotoSave\\screenshot.png')
     image_cropped = screenshot.crop((x, y, x + width, y + height))
     imgPath = 'PhotoSave\\UserPhoto' + username + '.png'
     image_cropped.save(imgPath)
     return {'code':0,'imgPath':imgPath,'url':url}
 
-def getUserAbsentFromWork(username,driver):
+def getUserAbsentFromWork():
     driver.refresh()
     stepSave = 0
     try:
         stepSave = 1
 
         # 進入成績查詢頁面
         # 切換到左測選單
```

### Comparing `shinherpro-1.6.8/shinherpro/chormeDriver.py` & `shinherpro-1.6.9/shinherpro/chormeDriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 import numpy as np
 import cv2
 import time
 import json
 import os
 
 
-def setup(url,view):
+def setup(url,view,path = "m"):
     print("chrome_options setup")
     chrome_options = Options()
     chrome_options.add_argument("--window-size=1280,960")
     if view==False :
         chrome_options.add_argument('--headless')
-    driver = webdriver.Chrome(options=chrome_options)
+    if path == "m":
+        driver = webdriver.Chrome(options=chrome_options)
+    else:
+        driver = webdriver.Chrome(executable_path=path, options=chrome_options)
     driver.get(url)
     print("chrome_options ready\n")
     return driver
 
 def switch_frame(reset, frame, driver):
     if reset:
         driver.switch_to.default_content()
```

### Comparing `shinherpro-1.6.8/shinherpro/vfcModel.py` & `shinherpro-1.6.9/shinherpro/vfcModel.py`

 * *Files identical despite different names*

