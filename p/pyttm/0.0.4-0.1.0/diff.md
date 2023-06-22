# Comparing `tmp/pyttm-0.0.4.tar.gz` & `tmp/pyttm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttm-0.0.4.tar", last modified: Tue Jun 20 12:48:16 2023, max compression
+gzip compressed data, was "pyttm-0.1.0.tar", last modified: Thu Jun 22 17:58:40 2023, max compression
```

## Comparing `pyttm-0.0.4.tar` & `pyttm-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.431038 pyttm-0.0.4/
--rw-rw-rw-   0        0        0     1063 2023-06-20 07:08:08.000000 pyttm-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2678 2023-06-20 12:48:16.431038 pyttm-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1901 2023-06-20 12:13:01.000000 pyttm-0.0.4/README.md
--rw-rw-rw-   0        0        0       68 2023-06-20 12:48:16.435027 pyttm-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-06-20 12:47:48.000000 pyttm-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.323247 pyttm-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.329247 pyttm-0.0.4/src/pyttm/
--rw-rw-rw-   0        0        0       40 2023-06-20 12:47:48.000000 pyttm-0.0.4/src/pyttm/__init__.py
--rw-rw-rw-   0        0        0      947 2023-06-20 12:13:01.000000 pyttm-0.0.4/src/pyttm/app.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.357247 pyttm-0.0.4/src/pyttm/libs/
--rw-rw-rw-   0        0        0     1168 2023-06-20 12:26:16.000000 pyttm-0.0.4/src/pyttm/libs/crypto.py
--rw-rw-rw-   0        0        0     1603 2023-06-20 12:45:38.000000 pyttm-0.0.4/src/pyttm/libs/db.py
--rw-rw-rw-   0        0        0     5095 2023-06-20 12:47:49.000000 pyttm-0.0.4/src/pyttm/libs/helper.py
--rw-rw-rw-   0        0        0     2960 2023-06-20 06:15:35.000000 pyttm-0.0.4/src/pyttm/libs/totp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.348247 pyttm-0.0.4/src/pyttm.egg-info/
--rw-rw-rw-   0        0        0     2678 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.358246 pyttm-0.0.4/tests/
--rw-rw-rw-   0        0        0     1240 2023-06-20 12:46:36.000000 pyttm-0.0.4/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:58:40.165114 pyttm-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-22 14:24:22.000000 pyttm-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-06-22 17:58:40.165114 pyttm-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-06-22 14:44:55.000000 pyttm-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-22 17:58:40.165114 pyttm-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-22 17:54:52.000000 pyttm-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:58:40.165114 pyttm-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:58:40.165114 pyttm-0.1.0/src/pyttm/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-22 17:54:52.000000 pyttm-0.1.0/src/pyttm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-22 14:30:27.000000 pyttm-0.1.0/src/pyttm/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:58:40.165114 pyttm-0.1.0/src/pyttm/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:24:22.000000 pyttm-0.1.0/src/pyttm/libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-06-22 14:24:22.000000 pyttm-0.1.0/src/pyttm/libs/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-06-22 17:49:17.000000 pyttm-0.1.0/src/pyttm/libs/db.py
+-rw-r--r--   0 root         (0) root         (0)     5701 2023-06-22 17:54:52.000000 pyttm-0.1.0/src/pyttm/libs/helper.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-22 14:24:22.000000 pyttm-0.1.0/src/pyttm/libs/totp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:58:40.165114 pyttm-0.1.0/src/pyttm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-06-22 17:58:40.000000 pyttm-0.1.0/src/pyttm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-22 17:58:40.000000 pyttm-0.1.0/src/pyttm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:58:40.000000 pyttm-0.1.0/src/pyttm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-22 17:58:40.000000 pyttm-0.1.0/src/pyttm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 17:58:40.000000 pyttm-0.1.0/src/pyttm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-22 17:58:40.000000 pyttm-0.1.0/src/pyttm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:58:40.165114 pyttm-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-06-22 14:24:22.000000 pyttm-0.1.0/tests/test.py
```

### Comparing `pyttm-0.0.4/LICENSE` & `pyttm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttm-0.0.4/README.md` & `pyttm-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-<div align="center">
-<img src="https://raw.githubusercontent.com/The-Robin-Hood/TTM/main/assets/logo.png"></img>
-<br/><br/>
-
-<b><i>Made for developers by a developer ♥</i></b> 
-</div>
-<br/>
-
-Terminal TOTP Manager is a command-line tool for managing Time-based One-Time Passwords (TOTPs). <br/>It allows you to securely store and generate TOTPs for your various accounts.
-
-## Prerequisites
-
-- Python 3.x
-
-## Installation
-
-   ```
-   pip install pyttm
-   ```
-
-## Usage
-
-To use TOTP Manager, follow these steps:
-
-1. Open a terminal or command prompt and navigate to the project directory.
-
-2. Run the following command:
-
-   ```
-   ttm [command]
-   ```
-
-   Replace `[command]` with one of the following options:
-
-   - `add`: Add a new TOTP credential.
-   - `list`: List all saved TOTPs
-   - `delete`: Delete a TOTP credential.
-
-3. If this is your first time using TOTP Manager, you will be prompted to create a password to secure your credentials. The password must be at least 8 characters long.
-
-4. Depending on the command you choose:
-
-   - For `add`: You can enter the OTPauth URI directly or provide the required information manually.
-   - For `list`: The Issuer and their associated TOTPs will be displayed continuously.
-   - For `delete`: Select the issuer of the credential you want to delete from the displayed list.
-
-## Security
-
-- The TOTP Manager stores your credentials securely by hashing the password before storing it in a JSON file (`db.json`).
-- You can only access the TOTP Manager by providing the correct password.
-
-## Contributing
-
-Contributions are welcome! If you encounter any issues or have suggestions for improvements, please report them on the project's GitHub page.
-
-## License
-
-The Project is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+<div align="center">
+<img src="https://raw.githubusercontent.com/The-Robin-Hood/TTM/main/assets/logo.png"></img>
+<br/><br/>
+
+<b><i>Made for developers by a developer ♥</i></b> 
+</div>
+<br/>
+
+Terminal TOTP Manager is a command-line tool for managing Time-based One-Time Passwords (TOTPs). <br/>It allows you to securely store and generate TOTPs for your various accounts.
+
+## Prerequisites
+
+- Python 3.x
+
+## Installation
+
+   ```
+   pip install pyttm
+   ```
+
+## Usage
+
+To use TOTP Manager, follow these steps:
+
+1. Open a terminal or command prompt and navigate to the project directory.
+
+2. Run the following command:
+
+   ```
+   ttm [command]
+   ```
+
+   Replace `[command]` with one of the following options:
+
+   - `add`: Add a new TOTP credential.
+   - `list`: List all saved TOTPs
+   - `delete`: Delete a TOTP credential.
+
+3. If this is your first time using TOTP Manager, you will be prompted to create a password to secure your credentials. The password must be at least 8 characters long.
+
+4. Depending on the command you choose:
+
+   - For `add`: You can enter the OTPauth URI directly or provide the required information manually.
+   - For `list`: The Issuer and their associated TOTPs will be displayed continuously.
+   - For `delete`: Select the issuer of the credential you want to delete from the displayed list.
+
+## Security
+
+- The TOTP Manager stores your credentials securely by hashing the password before storing it in a DB file (`config.db`) at `ttm` folder `%APPDATA%` or `XDG_CONFIG_HOME` depending on OS.
+- You can only access the TOTP Manager by providing the correct password.
+
+## Contributing
+
+Contributions are welcome! If you encounter any issues or have suggestions for improvements, please report them on the project's GitHub page.
+
+## License
+
+The Project is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
```

### Comparing `pyttm-0.0.4/setup.py` & `pyttm-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from setuptools import setup , find_packages
-import os
-
-def docs_read(fname):
-    f = open(os.path.join(os.path.dirname(__file__), fname)).read()
-    return f.replace('â™¥', '♥')
-
-setup(
-    name='pyttm',
-    version='0.0.4',
-    description='A simple Terminal based TOTP manager',
-    long_description=(docs_read('README.md')),
-    long_description_content_type='text/markdown',
-    url='https://github.com/The-Robin-Hood/ttm',
-    author='The Robin Hood',
-    license='MIT',
-    platforms=['any'],
-    entry_points={
-        'console_scripts': [
-            'ttm = pyttm.app:main'
-        ],
-    },
-    packages=find_packages(where='src',include=['pyttm','pyttm.*']),
-    package_dir={'': 'src'},
-    include_package_data=True,
-    install_requires=['pycryptodome'],
-    keywords='totp,otp,encryption,decryption,AES256,crypto,security,privacy',
-        classifiers=[
-        'Intended Audience :: Developers',
-        'Topic :: Security',
-        'Topic :: Utilities',
-        'Development Status :: 4 - Beta',
-        'Natural Language :: English',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Unix',
-        'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python :: 3'
-    ],
+from setuptools import setup , find_packages
+import os
+
+def docs_read(fname):
+    f = open(os.path.join(os.path.dirname(__file__), fname)).read()
+    return f.replace('â™¥', '♥')
+
+setup(
+    name='pyttm',
+    version='0.1.0',
+    description='A simple Terminal based TOTP manager',
+    long_description=(docs_read('README.md')),
+    long_description_content_type='text/markdown',
+    url='https://github.com/The-Robin-Hood/ttm',
+    author='The Robin Hood',
+    license='MIT',
+    platforms=['any'],
+    entry_points={
+        'console_scripts': [
+            'ttm = pyttm.app:main'
+        ],
+    },
+    packages=find_packages(where='src',include=['pyttm','pyttm.*']),
+    package_dir={'': 'src'},
+    include_package_data=True,
+    install_requires=['pycryptodome'],
+    keywords='totp,otp,encryption,decryption,AES256,crypto,security,privacy',
+        classifiers=[
+        'Intended Audience :: Developers',
+        'Topic :: Security',
+        'Topic :: Utilities',
+        'Development Status :: 4 - Beta',
+        'Natural Language :: English',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Unix',
+        'Operating System :: Microsoft :: Windows',
+        'Programming Language :: Python :: 3'
+    ],
 )
```

### Comparing `pyttm-0.0.4/src/pyttm/app.py` & `pyttm-0.1.0/src/pyttm/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-# __main__.py
-
-import sys
-from pyttm.libs.helper import *
-from pyttm.libs.crypto import *
-
-def main():
-    try:
-        clear()  
-        command_line_args = sys.argv[1:]
-        if len(command_line_args) == 0 or command_line_args[0] not in ["add","list","delete"]:
-            print("Usage: ttm add|list|delete\n")
-            exit()
-
-        password = get_password()        
-        command = command_line_args[0]
-
-        if command == "add":
-            add_creds(password)
-        elif command == "list":
-            list_creds(password)
-        elif command == "delete":
-            delete_creds(password)
-
-    except KeyboardInterrupt:
-        print("\nExiting...")
-        exit()
-    except ValueError:
-        print("Invalid input!")
-        exit()
-    except Exception as e:
-        print("Error! Facing Issue, Please Report!")
-        print(e)
-        exit()
-
-if __name__ == "__main__":
-    main()
+# __main__.py
+
+import sys
+from pyttm.libs.helper import *
+from pyttm.libs.crypto import *
+
+
+def main():
+    try:
+        clear()
+        check_for_updates()
+        command_line_args = sys.argv[1:]
+        if len(command_line_args) == 0 or command_line_args[0] not in ["add", "list", "delete"]:
+            print("Usage: ttm add|list|delete\n")
+            exit()
+
+        password = get_password()
+        command = command_line_args[0]
+
+        if command == "add":
+            add_creds(password)
+        elif command == "list":
+            list_creds(password)
+        elif command == "delete":
+            delete_creds(password)
+
+    except KeyboardInterrupt:
+        print("\nExiting...")
+        exit()
+    except ValueError:
+        print("Invalid input!")
+        exit()
+    except Exception as e:
+        print("Error! Facing Issue, Please Report!")
+        print(e)
+        exit()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyttm-0.0.4/src/pyttm/libs/crypto.py` & `pyttm-0.1.0/src/pyttm/libs/crypto.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from Crypto.Cipher import AES
-from Crypto.Random import get_random_bytes
-import hashlib
-
-def encrypt_text(text:str, secret_key:str):
-    secret_key= secret_key.zfill(16)
-    nonce = get_random_bytes(8) 
-    secret_key_to_bytes = secret_key.encode('utf-8')
-    cipher = AES.new(secret_key_to_bytes, AES.MODE_CTR, nonce=nonce)
-    encrypted_text = cipher.encrypt(text.encode('utf-8'))
-    return nonce.hex() + encrypted_text.hex()
-
-def decrypt_text(encrypted_text, secret_key):
-    nonce = bytes.fromhex(encrypted_text[:16])
-    secret_key= secret_key.zfill(16)
-    encrypted_bytes = bytes.fromhex(encrypted_text[16:])
-    secret_key_to_bytes = secret_key.encode('utf-8')
-    cipher = AES.new(secret_key_to_bytes, AES.MODE_CTR, nonce=nonce)
-    decrypted_text = cipher.decrypt(encrypted_bytes)
-    return decrypted_text.decode('utf-8')
-
-def hash_password(password):
-    password_bytes = password.encode('utf-8')
-    sha256_hash = hashlib.sha256()
-    sha256_hash.update(password_bytes)
-    hashed_password = sha256_hash.hexdigest()
-    return hashed_password
-
-def validate_password(password, hash):
-    return hash_password(password) == hash
+from Crypto.Cipher import AES
+from Crypto.Random import get_random_bytes
+import hashlib
+
+
+def encrypt_text(text: str, secret_key: str):
+    secret_key = secret_key.zfill(16)
+    nonce = get_random_bytes(8)
+    secret_key_to_bytes = secret_key.encode('utf-8')
+    cipher = AES.new(secret_key_to_bytes, AES.MODE_CTR, nonce=nonce)
+    encrypted_text = cipher.encrypt(text.encode('utf-8'))
+    return nonce.hex() + encrypted_text.hex()
+
+
+def decrypt_text(encrypted_text, secret_key):
+    nonce = bytes.fromhex(encrypted_text[:16])
+    secret_key = secret_key.zfill(16)
+    encrypted_bytes = bytes.fromhex(encrypted_text[16:])
+    secret_key_to_bytes = secret_key.encode('utf-8')
+    cipher = AES.new(secret_key_to_bytes, AES.MODE_CTR, nonce=nonce)
+    decrypted_text = cipher.decrypt(encrypted_bytes)
+    return decrypted_text.decode('utf-8')
+
+
+def hash_password(password):
+    password_bytes = password.encode('utf-8')
+    sha256_hash = hashlib.sha256()
+    sha256_hash.update(password_bytes)
+    hashed_password = sha256_hash.hexdigest()
+    return hashed_password
+
+
+def validate_password(password, hash):
+    return hash_password(password) == hash
```

