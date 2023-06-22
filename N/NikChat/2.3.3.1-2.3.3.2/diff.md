# Comparing `tmp/NikChat-2.3.3.1.tar.gz` & `tmp/NikChat-2.3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.3.3.1.tar", last modified: Wed Jun 21 20:53:25 2023, max compression
+gzip compressed data, was "NikChat-2.3.3.2.tar", last modified: Thu Jun 22 20:55:00 2023, max compression
```

## Comparing `NikChat-2.3.3.1.tar` & `NikChat-2.3.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:53:25.128629 NikChat-2.3.3.1/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.3.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-21 20:53:25.093961 NikChat-2.3.3.1/NikChat/
--rw-rw-rw-   0        0        0     6368 2023-06-21 20:51:51.000000 NikChat-2.3.3.1/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-21 20:52:17.000000 NikChat-2.3.3.1/NikChat/results.py
--rw-rw-rw-   0        0        0     4658 2023-06-21 20:52:30.000000 NikChat-2.3.3.1/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:53:25.124140 NikChat-2.3.3.1/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1660 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1660 2023-06-21 20:53:25.128629 NikChat-2.3.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-06-19 23:42:11.000000 NikChat-2.3.3.1/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      635 2023-06-21 20:53:25.131626 NikChat-2.3.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 20:55:00.747832 NikChat-2.3.3.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.3.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-22 20:55:00.686991 NikChat-2.3.3.2/NikChat/
+-rw-rw-rw-   0        0        0     6610 2023-06-22 20:49:19.000000 NikChat-2.3.3.2/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-21 20:52:17.000000 NikChat-2.3.3.2/NikChat/results.py
+-rw-rw-rw-   0        0        0     4642 2023-06-22 20:48:42.000000 NikChat-2.3.3.2/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:55:00.742842 NikChat-2.3.3.2/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1612 2023-06-22 20:55:00.000000 NikChat-2.3.3.2/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-22 20:55:00.000000 NikChat-2.3.3.2/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:55:00.000000 NikChat-2.3.3.2/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 20:55:00.000000 NikChat-2.3.3.2/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1612 2023-06-22 20:55:00.749826 NikChat-2.3.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1079 2023-06-22 20:53:41.000000 NikChat-2.3.3.2/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      635 2023-06-22 20:55:00.756353 NikChat-2.3.3.2/setup.cfg
```

### Comparing `NikChat-2.3.3.1/LICENSE` & `NikChat-2.3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.3.1/NikChat/__init__.py` & `NikChat-2.3.3.2/NikChat/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 from textblob import TextBlob
 from nltk.stem import WordNetLemmatizer
 from tensorflow.keras.models import load_model
 from NikChat.results import ctime, weather, internet
 
 def DChat(input):
     try:
-        #nltk.download('punkt')
-        #nltk.download('wordnet')
+        nltk.download('punkt')
+        nltk.download('wordnet')
         lemmatizer = WordNetLemmatizer()
         x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
         intents = json.loads(x.text)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
-        json.dumps(intents, "training.json")
         model = load_model('Speechbot.h5')
         def clean_up_sentence(sentence):
             idk = TextBlob(str(sentence))
-            return idk.correct()
+            susss = idk.correct()
+            sentence_words = nltk.word_tokenize(str(susss))
+            sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
+            return sentence_words
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
             bag = [0] * len(words)
             for w in sentence_words:
                 for i, word in enumerate(words):
                     if word == w:
                         bag[i] = 1
-            print(np.array(bag))
+            #print(np.array(bag))
             return np.array(bag)
         def predict_class(sentence):
             bow = bag_of_words(sentence)
             res = model.predict(np.array([bow]))[0]
             ERROR_TRESHOLD = 0.25
             results = [[i, r] for i, r in enumerate(res) if r > ERROR_TRESHOLD]
             results.sort(key=lambda x: x[1], reverse=True)
@@ -55,30 +57,30 @@
         idk = TextBlob(input)
         message = idk.correct()
         ints = predict_class(message)
         res = get_response(ints, intents['record'])
         str1 = ''
         for elm in message.split(' '):
             str1 += elm.lower() + " "
-        print(str1.split(' '))
+        #print(str1.split(' '))
         if "weather" in str1.split(' ') or "temperature" in str1.split(' ') or "forecast" in str1.split(' '):
             res = weather()
         elif "day" in str1.split(' ') or "time" in str1.split(' ') or "date" in str1.split(' '):
             res = ctime()
         elif res == "bob is your dad":
             res = internet(str1)
         else:
             res = res
         return res
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
-            return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
+            return e, " Please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder, testblob"
         
 def train(filePath):
     from os.path import exists
     if exists('words.pkl') == False:
         import NikChat.training as traning
         traning.init2(filePath)
         return 'done'
@@ -92,26 +94,29 @@
         traning.init()
         return 'done'
     else:
         return 'done'
 
 def NChat(filePath, input):
     try:
-        #nltk.download('punkt')
-        #nltk.download('wordnet')
+        nltk.download('punkt')
+        nltk.download('wordnet')
         lemmatizer = WordNetLemmatizer()
         intents = {}
         with open(filePath, 'r') as f:
             intents = json.load(f)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
         model = load_model('Speechbot.h5')
         def clean_up_sentence(sentence):
             idk = TextBlob(str(sentence))
-            return idk.correct()
+            susss = idk.correct()
+            sentence_words = nltk.word_tokenize(str(susss))
+            sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
+            return sentence_words
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
             bag = [0] * len(words)
             for w in sentence_words:
                 for i, word in enumerate(words):
                     if word == w:
                         bag[i] = 1
@@ -153,9 +158,9 @@
             res = res
         return res
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
-            return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
+            return e, " Please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder, testblob"
```

### Comparing `NikChat-2.3.3.1/NikChat/results.py` & `NikChat-2.3.3.2/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.3.1/NikChat/training.py` & `NikChat-2.3.3.2/NikChat/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import Dense, Activation, Dropout
 from tensorflow.keras.optimizers.legacy import SGD
 
 def init():
     lemmatizer = WordNetLemmatizer()
     x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
-    intents = json.load(x.text)
+    intents = json.loads(x.text)
     words = []
     classes = []
     documents = []
     ignore_letters = ["?", "!", ".", ","]
     for intent in intents['record']['intents']:
         for pattern in intent['patterns']: 
             word_list = nltk.word_tokenize(pattern)
@@ -60,16 +60,15 @@
     return
 
 def init2(filePath):
     import os
     lemmatizer = WordNetLemmatizer()
     if os.path.exists(filePath) == False:
         x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
-        y = json.load(x.text)
-        print(y)
+        y = json.loads(x.text)
         with open(filePath, 'w') as f:
             json.dump(y, f)
     intents = {}
     with open(filePath, 'r') as f:
         intents = json.load(f)
     words = []
     classes = []
```

### Comparing `NikChat-2.3.3.1/NikChat.egg-info/PKG-INFO` & `NikChat-2.3.3.2/NikChat.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.3.1
+Version: 2.3.3.2
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Nikchat - v1
+# Nikchat - v3
 
 Nikchat, the inaugural version of a groundbreaking chatbot AI, signifies a pivotal advancement in conversational interfaces. Equipped with advanced AI algorithms and natural language processing capabilities, Nikchat excels in facilitating meaningful conversations. With its contextual understanding, emotion detection, and personalized responses, Nikchat foreshadows the transformative potential of conversational AI, promising enhanced communication and unparalleled user experiences.
 
 
 # About
 
-Nikchat is still in a development mode. It is in the second version. Updates monthly!
+Nikchat is still in a development mode. It is in the third version. Updates monthly!
 
 ## How to use Nikchat
+Get all your questions answered from the following official youtube video:
+**https://www.youtube.com/-insertstuffhere-**
 
-Using your package installer (pip, anaconda, etc.) download the library.
-Ex:
-```pip install nikchat```
-
-First use the `init()` method which initializes the library
-
-Then use the `NChat()` method. This is how you communicate with the bot. This method takes one argument: the prompt.
-Example: ```print(NChat("who is joe biden"))```
+# New Features
+- Text autocorrection
+- User training functions, allowing users to make their own chatbots
+- Much faster
+- 2 new functions: `train()` and `NChat()`
 
 ## Upcoming Features
 - Story generation
 - song lyric fetcher
 - basic personality
 - basic personality recognition
 - inappropriate content recognition
```

### Comparing `NikChat-2.3.3.1/PKG-INFO` & `NikChat-2.3.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.3.1
+Version: 2.3.3.2
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Nikchat - v1
+# Nikchat - v3
 
 Nikchat, the inaugural version of a groundbreaking chatbot AI, signifies a pivotal advancement in conversational interfaces. Equipped with advanced AI algorithms and natural language processing capabilities, Nikchat excels in facilitating meaningful conversations. With its contextual understanding, emotion detection, and personalized responses, Nikchat foreshadows the transformative potential of conversational AI, promising enhanced communication and unparalleled user experiences.
 
 
 # About
 
-Nikchat is still in a development mode. It is in the second version. Updates monthly!
+Nikchat is still in a development mode. It is in the third version. Updates monthly!
 
 ## How to use Nikchat
+Get all your questions answered from the following official youtube video:
+**https://www.youtube.com/-insertstuffhere-**
 
-Using your package installer (pip, anaconda, etc.) download the library.
-Ex:
-```pip install nikchat```
-
-First use the `init()` method which initializes the library
-
-Then use the `NChat()` method. This is how you communicate with the bot. This method takes one argument: the prompt.
-Example: ```print(NChat("who is joe biden"))```
+# New Features
+- Text autocorrection
+- User training functions, allowing users to make their own chatbots
+- Much faster
+- 2 new functions: `train()` and `NChat()`
 
 ## Upcoming Features
 - Story generation
 - song lyric fetcher
 - basic personality
 - basic personality recognition
 - inappropriate content recognition
```

### Comparing `NikChat-2.3.3.1/setup.cfg` & `NikChat-2.3.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 332e 332e 310d 0a61  ion = 2.3.3.1..a
+00000020: 696f 6e20 3d20 322e 332e 332e 320d 0a61  ion = 2.3.3.2..a
 00000030: 7574 686f 7220 3d20 4e69 6b68 696c 2054  uthor = Nikhil T
 00000040: 616d 7661 6461 2028 4e69 6b68 696c 6f64  amvada (Nikhilod
 00000050: 656f 6e31 290d 0a61 7574 686f 725f 656d  eon1)..author_em
 00000060: 6169 6c20 3d20 6e69 6b68 696c 7461 6d76  ail = nikhiltamv
 00000070: 6164 6140 676d 6169 6c2e 636f 6d0d 0a64  ada@gmail.com..d
 00000080: 6573 6372 6970 7469 6f6e 203d 2041 2066  escription = A f
 00000090: 756c 6c2d 666c 6564 6765 6420 6368 6174  ull-fledged chat
```

