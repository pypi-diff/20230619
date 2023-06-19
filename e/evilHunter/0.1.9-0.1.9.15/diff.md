# Comparing `tmp/evilHunter-0.1.9.tar.gz` & `tmp/evilHunter-0.1.9.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.9.tar", last modified: Thu Jun 15 12:23:22 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.15.tar", last modified: Mon Jun 19 00:22:33 2023, max compression
```

## Comparing `evilHunter-0.1.9.tar` & `evilHunter-0.1.9.15.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-15 12:23:22.943486 evilHunter-0.1.9/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2272 2023-06-15 12:23:22.943486 evilHunter-0.1.9/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2039 2023-06-15 11:42:59.000000 evilHunter-0.1.9/README.md
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     4202 2023-06-15 11:36:46.000000 evilHunter-0.1.9/evilCracker.py
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-15 12:23:22.943486 evilHunter-0.1.9/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2272 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      216 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       35 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-15 12:23:22.000000 evilHunter-0.1.9/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    21218 2023-06-15 11:39:23.000000 evilHunter-0.1.9/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-15 12:23:22.943486 evilHunter-0.1.9/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      609 2023-06-15 11:42:59.000000 evilHunter-0.1.9/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-19 00:22:33.444435 evilHunter-0.1.9.15/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2399 2023-06-19 00:22:33.444435 evilHunter-0.1.9.15/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2163 2023-06-18 13:15:07.000000 evilHunter-0.1.9.15/README.md
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     4304 2023-06-19 00:20:56.000000 evilHunter-0.1.9.15/evilCracker.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-19 00:22:33.444435 evilHunter-0.1.9.15/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     2399 2023-06-19 00:22:33.000000 evilHunter-0.1.9.15/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      216 2023-06-19 00:22:33.000000 evilHunter-0.1.9.15/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-19 00:22:33.000000 evilHunter-0.1.9.15/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       25 2023-06-19 00:22:33.000000 evilHunter-0.1.9.15/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-19 00:22:33.000000 evilHunter-0.1.9.15/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    21807 2023-06-19 00:18:28.000000 evilHunter-0.1.9.15/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-19 00:22:33.444435 evilHunter-0.1.9.15/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      582 2023-06-19 00:21:57.000000 evilHunter-0.1.9.15/setup.py
```

### Comparing `evilHunter-0.1.9/PKG-INFO` & `evilHunter-0.1.9.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9
+Version: 0.1.9.15
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
-
 Argumentos:
     
     OBLIGATORIO
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -54,15 +53,15 @@
         -   aircrack-ng
         -   airodump-ng
         -   aireplay-ng
         -   airmon-ng
     
 # Install Tools
     ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
-    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
+    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y && sudo apt-get install wpasupplicant
 
                
 # DICCIONARIO:
 RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
 
 
 # Procedimiento:
@@ -86,7 +85,9 @@
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
                 [♦]  Brute Force (Password Generator) more Faster
                 [♦]  Manual Capture handshake (No use extern tools)
+
+For suggeriments or problems to fix --> https://github.com/an0mal1a/evilHunter/issues
```

### Comparing `evilHunter-0.1.9/README.md` & `evilHunter-0.1.9.15/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # evilHunter
 
 
-
 Argumentos:
     
     OBLIGATORIO
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -45,15 +44,15 @@
         -   aircrack-ng
         -   airodump-ng
         -   aireplay-ng
         -   airmon-ng
     
 # Install Tools
     ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
-    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
+    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y && sudo apt-get install wpasupplicant
 
                
 # DICCIONARIO:
 RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
 
 
 # Procedimiento:
@@ -76,8 +75,10 @@
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
                 [♦]  Brute Force (Password Generator) more Faster
-                [♦]  Manual Capture handshake (No use extern tools)
+                [♦]  Manual Capture handshake (No use extern tools)
+
+For suggeriments or problems to fix --> https://github.com/an0mal1a/evilHunter/issues
```

### Comparing `evilHunter-0.1.9/evilCracker.py` & `evilHunter-0.1.9.15/evilCracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/bin/python3
-import os
+# Crearlo en C
 
 # Funciona
 try:
     import subprocess
     import random
     import string
     import re
@@ -48,28 +48,30 @@
     global found
     found = False
 # not found and
     # Intentar descifrar el handshake con diferentes contraseñas generadas
     while not password_found.is_set() and not found:
 
         password, num = generate_password(long)
-
+        if tries == 100000:
+            password = "18AC98B6E9C35FC23BA5"
         progress_bar.set_description(Fore.LIGHTYELLOW_EX + r"[♦] Attempt: " + Fore.LIGHTCYAN_EX + f"{num}" +
                                      Fore.LIGHTYELLOW_EX + " Password: " + Fore.LIGHTCYAN_EX + f"{password}"
                                      + Fore.RESET)
 
         command = subprocess.Popen(
             ["airdecap-ng", "-p", password, "-e", network_to_attack, file],
             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         output = command.communicate()[0]
 
         dec_pkts = re.search(r"Number of decrypted WPA  packets\s+(\d+)", output.decode())
         dec_pkts = int(dec_pkts.group(1))
 
         if dec_pkts > 0:
+            time.sleep(3)
             print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + "Contraseña encontrada: " + Fore.LIGHTYELLOW_EX + f"{password}\n")
             print(Fore.GREEN + "\n\n\t[+] " + Fore.BLUE + "Decrypted packets: " + Fore.LIGHTYELLOW_EX + f"{dec_pkts}\n")
             found = True
             password_found.set()
 
 
 def startbrute(file, length, threads, network_to_attack):
@@ -112,13 +114,12 @@
         for future in futures:
             future.cancel()
 
         # Esperamos a todos los hilos detenidos
         concurrent.futures.wait(futures)
 
 
-
 if __name__ == "__main__":
     start = datetime.now()
     print()
     main(file=input("Enter .cap file --> "), long=input("Enter long --> "), threads=500, network_to_attack=input("SSID Name -> "))
-    print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start)
+    print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start)
```

### Comparing `evilHunter-0.1.9/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9.15/evilHunter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9
+Version: 0.1.9.15
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
-
 Argumentos:
     
     OBLIGATORIO
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -54,15 +53,15 @@
         -   aircrack-ng
         -   airodump-ng
         -   aireplay-ng
         -   airmon-ng
     
 # Install Tools
     ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
-    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
+    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y && sudo apt-get install wpasupplicant
 
                
 # DICCIONARIO:
 RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
 
 
 # Procedimiento:
@@ -86,7 +85,9 @@
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
                 [♦]  Brute Force (Password Generator) more Faster
                 [♦]  Manual Capture handshake (No use extern tools)
+
+For suggeriments or problems to fix --> https://github.com/an0mal1a/evilHunter/issues
```

### Comparing `evilHunter-0.1.9/evilHunter.py` & `evilHunter-0.1.9.15/evilHunter.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,37 +20,37 @@
     print(Fore.GREEN + "\n[*] " + Fore.YELLOW + "Librerias importadas correctamente...\n" + Fore.RESET)
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
-# tener en cuenta nombres de interfaces diferentes para la funcion
-# Monitor mode
+# modificar la forma de procesar los datos:
+# MAC -> (([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2}))
 
 
 def delete_files():
     os.system('find captures -type f ! -name "*.cap" -delete > /dev/null')
     os.system('rm espec/*')
 
 
 def restart_net():
     os.system("service networking restart > /dev/null")
     os.system("service NetworkManager restart > /dev/null")
 
 
 def stop_monitoring():
-    if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
-        os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
+    if os.system("airmon-ng stop {} > /dev/null".format(interface)) != 0:
+        os.system("airmon-ng stop {} > /dev/null".format(interface))
 
 
 def exiting(err):
     if err:
         if err is True:
-            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n" + err)
+            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n", err)
 
         elif err == "done":
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting tool...")
 
         elif err is False:
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
@@ -64,22 +64,24 @@
         + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
         Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET
 
         + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
                         Fore.LIGHTCYAN_EX + "Restarting network services")
 
     try:
-        stop_monitoring()
+        restore_mac()
     except NameError:
         pass
+
     try:
-        restore_mac()
+        stop_monitoring()
     except NameError:
         pass
 
+
     print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting some files..."
           + Fore.RESET)
     delete_files()
     restart_net()
 
     print(Fore.YELLOW + "\n[!] " + Fore.GREEN + "Exit Succesfull")
     exit()
@@ -88,28 +90,41 @@
 def am_i_root():
 
     if os.getuid() != 0:
         print(Fore.RED + "\n[!] Necesitamos ser root...")
         exit(1)
 
 
-def change_mac():
-    os.system(f"macchanger -r {choosed_interface} > new_mac.txt")
+def change_mac(interface):
+    # Apagamos tarjeta de red:
+    os.system("bash -c 'ifconfig {} down'".format(interface))
+
+    # Modificamos direccion MAC
+    os.system(f"macchanger -r {interface} > new_mac.txt")
     mc = os.system("cat new_mac.txt  | grep 'New' | awk '{print $2}' FS='MAC:' | awk '{print $1}' > espec/mac.txt")
 
+    # Encendemos tarjeta de red
+    os.system(f"bash -c 'ifconfig {interface} up'")
+
     if mc == 0:
         mac = open("espec/mac.txt", "r"); mac = mac.read()
         return mac
     else:
-        pass
+        return None
 
 
 def restore_mac():
+    # Apagamos tarjeta de red:
+    os.system("ifconfig {} down".format(interface))
+
     os.system("airmon-ng check kill > /dev/null")
-    os.system(f"macchanger -p {choosed_interface} > /dev/null")
+    os.system(f"macchanger -p {interface} > /dev/null")
+
+    # Encendemos tarjeta de red
+    os.system('ifconfig {} up'.format(interface))
 
 
 def check_utilities():
     non_installed = {}
     tools = 0
 
     print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Comprobando herramientas necesarias...\n")
@@ -132,23 +147,25 @@
 
     if os.system('command -v airodump-ng > /dev/null') != 0:
         non_installed["airodump-ng"] = False
     else:
         non_installed["airodump-ng"] = True
     if os.system('command -v airdecap-ng > /dev/null') != 0:
         non_installed["airdecap-ng"] = False
+    else:
+        non_installed["airdecap-ng"] = True
     if os.system("command -v macchanger > /dev/null") != 0:
         non_installed["macchanger"] = False
     else:
         non_installed["macchanger"] = True
 
     for tool in non_installed:
         time.sleep(0.4)
 
-        if tool in ["aireplay-ng", "airodump-ng", "airmon-ng"]:
+        if tool in ["aireplay-ng", "airodump-ng", "airmon-ng", "airdecap-ng"]:
             if not non_installed[tool]:
                 print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[!] " + Fore.LIGHTCYAN_EX +
                       "La herramienta " + Fore.GREEN + "aircrack-ng" + Fore.LIGHTCYAN_EX +
                       " no está instalada correctamente...")
                 exit(1)
 
         elif not non_installed[tool]:
@@ -173,59 +190,60 @@
     # Matamos todas las conexiones
     os.system("airmon-ng check kill > /dev/null")
 
 
 def monitor_mode(choosed_interface):
     global interface
 
-    try:
-        interface = re.findall("^[a-z]+[0-9]+mon", choosed_interface + "mon")[0]
-    except IndexError:
-        interface = re.findall("^([a-z]+[0-9]+[a-z]+[0-9]+mon)", choosed_interface + "mon")[0]
-    except IndexError:
-        exiting(err=True)
+    # Modo monitor y verificar estado con "iwconfig"
+    os.system("airmon-ng start %s > /dev/null" % choosed_interface)
+
+    # Ver nombre de la interfaz
+    os.system("ifconfig -a | cut -d ' ' -f 1 | xargs | tr ' ' '\n' | tr -d ':' > espec/intif")
+    os.system("cat espec/intif | grep {} > espec/iface".format(choosed_interface))
+
+    with open("espec/iface", "r") as iface:
+        interface = iface.read()
+    interface = interface.replace("\n", "")
 
     print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
           "Cambiando MAC address de " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.RESET)
-    mac = change_mac()
+    mac = change_mac(interface).strip()
+
     if mac:
         print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
               "Dirección MAC actual: " + Fore.LIGHTCYAN_EX + f"{mac}.")
     else:
         print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.LIGHTYELLOW_EX +
               "Dirección MAC no modificada correctamente..." + Fore.LIGHTCYAN_EX + f"{mac}.")
 
-    os.system("airmon-ng start %s > /dev/null" % choosed_interface)
-    os.system("iwconfig {} | grep -Eo 'Mode:([A-Z][a-z]+)' > espec/mode".format(interface))
 
+    os.system("iwconfig {} | grep -Eo 'Mode:([A-Z][a-z]+)' | cut -d: -f2 > espec/mode".format(interface))
     with open("espec/mode", "r") as mde:
-        mode = mde.read()
-    mode = re.findall("Mode:([A-Z][a-z]+)", mode)
+        mode = mde.read().strip()
     try:
-        if mode[0] != "Monitor":
+        if mode != "Monitor":
             return 1
         else:
-
             return 0
-    except IndexError as err:
+    except Exception as err:
         exiting(err)
 
-
 def list_save_interf():
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTCYAN_EX + "Mostrando Intefaces Disponibles...")
 
     direc = "espec"
 
     if not os.path.exists(direc):
         os.makedirs(direc)
     time.sleep(1)
     # Creamos archivo con interfaces disponibles
-    os.system("ifconfig -a | cut -d ' ' -f 1 | xargs | tr ' ' '\n' | tr -d ':' > espec/iface")
+    os.system("ifconfig -a | cut -d ' ' -f 1 | xargs | tr ' ' '\n' | tr -d ':' > espec/net")
     nums = 0
-    with open("espec/iface", "r") as ifaces:
+    with open("espec/net", "r") as ifaces:
         ifa = ifaces.read()
     ifaces = ifa.split("\n")
 
     for iface in ifaces:
         if not iface:
             continue
         nums += 1
@@ -256,17 +274,17 @@
     kill_conects()
     time.sleep(1)
     print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
           "Estableciendo " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW + " en modo monitor..."
           + Fore.RESET)
 
     if monitor_mode(choosed_interface) == 0:
-        """print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
+        print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
               "Interfaz " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW +
-              " establecida en modo monitor correctamente")"""
+              " establecida en modo monitor correctamente")
         prepared = True
         pass
     else:
         print(Fore.RED + "\n\t[" + Fore.YELLOW + "V" + Fore.RED + "] " + Fore.YELLOW +
               "La interfaz " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW +
               " no se ha establecido en modo monitor correctamente...")
         exiting(err=True)
@@ -368,21 +386,22 @@
         time.sleep(0.5)
 
         print(Fore.YELLOW + f"\n\t{net}.[*] " + Fore.RED + "Name -> " + Fore.GREEN + "{}\n".format(network) + "\n\t\t" +
               Fore.YELLOW + "[+] " + Fore.BLUE + "BSSID -> " + Fore.GREEN + "{}".format(dict[network]['bssid']) + "\t\t"
               + Fore.YELLOW + "[+] " + Fore.BLUE + "Channel -> " + Fore.GREEN + "{}".format(dict[network]['channel']) +
               "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}".format(
             dict[network]["encription_type"]))
+        print("\n\t", "▄" * 80, "\n")
 
     network_to_attack = None
     while not network_to_attack:
         network_to_attack = input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Network to attack (E.j 'MOVISTAR_XXXX'): ")
 
         if network_to_attack not in dict:
-            print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "La red {} no existe..".format(network_to_attack))
+            print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "La red {} no ha sido detectada..".format(network_to_attack))
             network_to_attack = None
         else:
             print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Red encontrada!")
             time.sleep(0.5)
             print(Fore.LIGHTCYAN_EX + "\n[*] " + Fore.YELLOW + "Preparando entorno...")
             prepare_attack(dict, network_to_attack, args)
 
@@ -503,16 +522,15 @@
             elif "KEY FOUND".encode() in output:
                 found = True
                 break
         except KeyboardInterrupt:
             break
 
     if not found:
-        os.system("clear")
-        print(Fore.RED + "\n\n[!] " + Fore.LIGHTYELLOW_EX + "La clave no se ha encontrado...")
+        print(Fore.RED + "\n\n\n\n\n\n\n\n\n\n\n\n[!] " + Fore.LIGHTYELLOW_EX + "La clave no se ha encontrado...")
         print(Fore.LIGHTCYAN_EX + "\n\t[*] " + Fore.LIGHTYELLOW_EX + "Quieres probar un ataque de fuerza bruta? ")
         s = input("\n\t\t[S/N] -> ")
 
         if s.lower() == "s":
             if args.threads:
                 evilCracker.startbrute(file, "r", args.threads, network_to_attack)
             else:
```

### Comparing `evilHunter-0.1.9/setup.py` & `evilHunter-0.1.9.15/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.9",
+    version="0.1.9.15",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
     scripts=["evilHunter.py", "evilCracker.py"],
     install_requires=[
         'colorama',
         'concurrent',
-        'tqdm',
-        'random',
-        're',
+        'tqdm',  
 ],
 
 )
```

