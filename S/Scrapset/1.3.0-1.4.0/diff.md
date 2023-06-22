# Comparing `tmp/Scrapset-1.3.0-py3-none-any.whl.zip` & `tmp/Scrapset-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4260 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     4485 b- defN 23-Jun-05 15:51 Scrapset/Scrapset.py
+Zip file size: 4267 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     4487 b- defN 23-Jun-22 18:28 Scrapset/Scrapset.py
 -rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-06 18:47 Scrapset/__init__.py
--rw-rw-rw-  2.0 fat     4305 b- defN 23-Jun-06 18:48 Scrapset-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 18:48 Scrapset-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      632 b- defN 23-Jun-06 18:48 Scrapset-1.3.0.dist-info/licence.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-06 18:48 Scrapset-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      545 b- defN 23-Jun-06 18:48 Scrapset-1.3.0.dist-info/RECORD
-7 files, 10117 bytes uncompressed, 3290 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     4305 b- defN 23-Jun-22 18:29 Scrapset-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 18:29 Scrapset-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      632 b- defN 23-Jun-22 18:29 Scrapset-1.4.0.dist-info/licence.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-22 18:29 Scrapset-1.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      545 b- defN 23-Jun-22 18:29 Scrapset-1.4.0.dist-info/RECORD
+7 files, 10119 bytes uncompressed, 3297 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Scrapset/Scrapset.py
 Comment: 
 
 Filename: Scrapset/__init__.py
 Comment: 
 
-Filename: Scrapset-1.3.0.dist-info/METADATA
+Filename: Scrapset-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: Scrapset-1.3.0.dist-info/WHEEL
+Filename: Scrapset-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: Scrapset-1.3.0.dist-info/licence.txt
+Filename: Scrapset-1.4.0.dist-info/licence.txt
 Comment: 
 
-Filename: Scrapset-1.3.0.dist-info/top_level.txt
+Filename: Scrapset-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Scrapset-1.3.0.dist-info/RECORD
+Filename: Scrapset-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Scrapset/Scrapset.py

```diff
@@ -16,23 +16,23 @@
         driver = webdriver.Chrome(options=options)
         return driver
 
     def data_set_page(self, url, last_page, initial_page):
         try:
             driver = webdriver.Chrome()
             self.url = url
-            time.sleep(2)
+            time.sleep(1)
             
             list_of_dic = {'title': [], 'size': [],'all_details':[],'up_vote':[]}  # Initialize the dictionary
 
             while initial_page < last_page:  
                 # i = i + 1
                 initial_page=initial_page + 1 
                 driver.get(self.url + f'/datasets?page={initial_page}')
-                time.sleep(2)
+                time.sleep(0.5)
                 titles = driver.find_elements(By.XPATH, '//*[@id="site-content"]/div[6]/div/div/div/ul/li/div[1]/a')
                 for title in titles:
                     data_set_title = title.find_element(By.XPATH, './div[2]/div').text
                     try: 
                         data_set_size = title.find_element(By.XPATH, './div[2]/span[2]/span').text
                         data_set_details=title.find_element(By.XPATH,'//*[@id="site-content"]/div[6]/div/div/div/ul/li[1]/div[1]/a/div[2]/span').text
                         data_set_upvote=title.find_element(By.XPATH,'//*[@id="site-content"]/div[6]/div/div/div/ul/li/div[1]/div/div/span').text
```

## Comparing `Scrapset-1.3.0.dist-info/METADATA` & `Scrapset-1.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 1.3.0
+Version: 1.4.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 Requires-Dist: selenium
```

## Comparing `Scrapset-1.3.0.dist-info/licence.txt` & `Scrapset-1.4.0.dist-info/licence.txt`

 * *Files identical despite different names*

