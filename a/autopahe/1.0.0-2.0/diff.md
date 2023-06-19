# Comparing `tmp/autopahe-1.0.0.tar.gz` & `tmp/autopahe-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopahe-1.0.0.tar", last modified: Fri Jun 16 07:42:43 2023, max compression
+gzip compressed data, was "autopahe-2.0.tar", last modified: Mon Jun 19 20:10:06 2023, max compression
```

## Comparing `autopahe-1.0.0.tar` & `autopahe-2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 07:42:43.423442 autopahe-1.0.0/
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-1.0.0/MANIFEST.in
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6409 2023-06-16 07:42:43.423442 autopahe-1.0.0/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5756 2023-06-16 07:38:04.000000 autopahe-1.0.0/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 07:42:43.419442 autopahe-1.0.0/autopahe/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       24 2023-06-16 07:36:17.000000 autopahe-1.0.0/autopahe/__init__.py
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    27910 2023-06-16 06:58:12.000000 autopahe-1.0.0/autopahe/auto_pahe.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      211 2023-06-13 23:06:59.000000 autopahe-1.0.0/autopahe/test.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 07:42:43.423442 autopahe-1.0.0/autopahe.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6409 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      301 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-16 07:42:43.000000 autopahe-1.0.0/autopahe.egg-info/top_level.txt
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-1.0.0/requirements.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-16 07:42:43.423442 autopahe-1.0.0/setup.cfg
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)     1374 2023-06-16 07:39:23.000000 autopahe-1.0.0/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:10:06.483865 autopahe-2.0/
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.0/MANIFEST.in
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:10:06.483865 autopahe-2.0/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.0/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:10:06.475865 autopahe-2.0/autopahe/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       24 2023-06-18 08:58:01.000000 autopahe-2.0/autopahe/__init__.py
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19649 2023-06-19 20:02:01.000000 autopahe-2.0/autopahe/auto_pahe.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.0/autopahe/kwikdown.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.0/autopahe/test.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:10:06.483865 autopahe-2.0/autopahe.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/top_level.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.0/pyproject.toml
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.0/requirements.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:10:06.483865 autopahe-2.0/setup.cfg
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1372 2023-06-19 19:27:13.000000 autopahe-2.0/setup.py
```

### Comparing `autopahe-1.0.0/PKG-INFO` & `autopahe-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 1.0.0
+Version: 2.0
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 <!-- Badges -->
-<!-- [![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/) -->
+[![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/autopahe/)
 [![License](https://img.shields.io/github/license/haxsysgit/autopahe?color=brightgreen)](https://github.com/haxsysgit/autopahe/blob/main/license.md)
 [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/autopahe?color=important)](https://github.com/haxsysgit/autopahe/issues)
 <!--LineBreak-->
 [![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/autopahe/)
 [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/autopahe/)
 <!-- Badges -->
@@ -67,15 +67,15 @@
   - In case of multiple options, each options must be seperated by a `,`
   - Example: `1, 3, 6-11` : downloads episodes 1,3,6,7,8,9,10,11
 
 ## Command line features
 To use the script, run it in your terminal using the following command:
 
 ```shell
-python fetchanime.py [-h] [-b BROWSER] [-s SEARCH] [-sh SEARCH_HIDDEN] [-i INDEX] [-sd SINGLE_DOWNLOAD] [-md MULTI_DOWNLOAD_OPTIMIZED] [-mdv MULTI_DOWNLOAD_VERBOSE] [-a ABOUT]
+python auto_pahe.py [-h] [-b BROWSER] [-s SEARCH] [-sh SEARCH_HIDDEN] [-i INDEX] [-sd SINGLE_DOWNLOAD] [-md MULTI_DOWNLOAD_OPTIMIZED] [-mdv MULTI_DOWNLOAD_VERBOSE] [-a ABOUT]
 ```
 
 Here are the available options:
 
 - `-h`, `--help`: show the help message and exit
 - `-b`, `--browser`: choose the browser to use (`chrome`,`firefox` or `brave`). If omitted, the script will use `chrome` by default. Use `ffgui` for a GUI Firefox window.
 - `-s`, `--search`: search for an anime using a keyword. The script will display a list of matching results.
```

### Comparing `autopahe-1.0.0/README.md` & `autopahe-2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <!-- Badges -->
-<!-- [![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/) -->
+[![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/autopahe/)
 [![License](https://img.shields.io/github/license/haxsysgit/autopahe?color=brightgreen)](https://github.com/haxsysgit/autopahe/blob/main/license.md)
 [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/autopahe?color=important)](https://github.com/haxsysgit/autopahe/issues)
 <!--LineBreak-->
 [![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/autopahe/)
 [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/autopahe/)
 <!-- Badges -->
@@ -49,15 +49,15 @@
   - In case of multiple options, each options must be seperated by a `,`
   - Example: `1, 3, 6-11` : downloads episodes 1,3,6,7,8,9,10,11
 
 ## Command line features
 To use the script, run it in your terminal using the following command:
 
 ```shell
-python fetchanime.py [-h] [-b BROWSER] [-s SEARCH] [-sh SEARCH_HIDDEN] [-i INDEX] [-sd SINGLE_DOWNLOAD] [-md MULTI_DOWNLOAD_OPTIMIZED] [-mdv MULTI_DOWNLOAD_VERBOSE] [-a ABOUT]
+python auto_pahe.py [-h] [-b BROWSER] [-s SEARCH] [-sh SEARCH_HIDDEN] [-i INDEX] [-sd SINGLE_DOWNLOAD] [-md MULTI_DOWNLOAD_OPTIMIZED] [-mdv MULTI_DOWNLOAD_VERBOSE] [-a ABOUT]
 ```
 
 Here are the available options:
 
 - `-h`, `--help`: show the help message and exit
 - `-b`, `--browser`: choose the browser to use (`chrome`,`firefox` or `brave`). If omitted, the script will use `chrome` by default. Use `ffgui` for a GUI Firefox window.
 - `-s`, `--search`: search for an anime using a keyword. The script will display a list of matching results.
```

### Comparing `autopahe-1.0.0/autopahe/auto_pahe.py` & `autopahe-2.0/autopahe/auto_pahe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 #! /usr/bin/python3
-import time,requests,argparse,os,shutil
-import sys,subprocess,re
-from json import loads,dumps,load,dump
+import time,requests,argparse,os
+import sys
+from json import loads,load,dump
 from re import search
-from selenium import webdriver
 from bs4 import BeautifulSoup
-from selenium.webdriver.firefox.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.firefox.service import Service
-from webdriver_manager.chrome import ChromeDriverManager
-from webdriver_manager.firefox import GeckoDriverManager
-from webdriver_manager.core.utils import ChromeType
+from kwikdown import kwik_download
+import concurrent.futures as concur
+
 
-import tqdm
 
 start = time.perf_counter()
 
+def data_report(data:dict,filepath = "autopahe_data.json",):
+    if data:
+        # Read existing JSON data from file
+        if os.path.exists(filepath):
+            with open(filepath, 'r') as json_file:
+                existing_data = load(json_file)
+        else:
+            open(filepath,"x")
+            existing_data={}
+
+        new_data = {**existing_data,**data}
+            
+        with open(filepath,"w") as st:
+            dump(new_data,st)
+
 current_system_os = str(sys.platform) #get current os
 
 
 class Banners():
     def header():
-        # os.system('cls' if current_system_os.lower() == 'windows' else 'clear' )
+        os.system('cls' if current_system_os.lower() == 'windows' else 'clear' )
         print('''
               
              db    8    8 88888 .d88b.      888b.    db    8   8 8888 
             dPYb   8    8   8   8P  Y8 ____ 8  .8   dPYb   8www8 8www 
            dPwwYb  8b..d8   8   8b  d8      8wwP'  dPwwYb  8   8 8    
           dP    Yb `Y88P'   8   `Y88P'      8     dP    Yb 8   8 8888 
               
@@ -87,28 +95,17 @@
             Summary on Anime
         ----------------------------------------
         
         {summary}
         
         ''')
         
-# def get_terminal_size():
-#     terminal_size = shutil.get_terminal_size((80, 20))  # Default size if unable to get actual size
-#     if os.name == 'posix':  # Unix/Linux/Mac systems
-#         try:
-#             terminal_size = shutil.get_terminal_size()
-#         except Exception:
-#             pass
-#     elif os.name == 'nt':  # Windows systems
-#         try:
-#             terminal_size = shutil.get_terminal_size((80, 20))
-#         except Exception:
-#             pass
-#     return terminal_size
 
+# Banner Header
+Banners.header()
 
 
 def n():
     print()
 
 
 n()
@@ -135,58 +132,14 @@
         print('*' * box_width)
         print('*' + ' ' * padding + func() + ' ' * (box_width - len(func()) - padding) + '*')
         print('*' * box_width)
 
         
     return wrapper
 
-
-
-# driver handling function
-def browser(barg):
-    global driver
-
-    if barg == "chrome":
-
-        serv = Service(executable_path=ChromeDriverManager().install())
-        option = webdriver.ChromeOptions()
-
-        option.headless = False
-
-        option.add_experimental_option("detach", False)
-
-        driver = webdriver.Chrome(service = serv,options=option)
-
-    elif barg == "ffgui":
-
-        options = Options()
-        options.headless = False
-        driver = webdriver.Firefox(executable_path=GeckoDriverManager().install(),options=options)
-        
-    elif barg == "firefox":
-
-        options = Options()
-        options.headless = True
-        driver = webdriver.Firefox(executable_path=GeckoDriverManager().install(),options=options)
-
-
-    elif barg == "brave":
-        serv = Service(ChromeDriverManager().install())
-        
-        options = Options()
-        
-        options.headless = False
-        
-        driver = webdriver.Chrome(service=Service(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
-    else:
-        pass
-        
-    def close():
-        driver.quit()
-        
     
 # =======================================================================================================
 
 
 def lookup(arg):
     # search banner
     Banners.search(arg)
@@ -282,46 +235,27 @@
     type = search_response_dict['data'][arg]['type']
     image = search_response_dict['data'][arg]['poster']
     stat = search_response_dict['data'][arg]['status']
     
     Banners.select(animepicked,eps=episto,year=year,
                    atype = type,img = image,status=stat)
 
-    
+    final_data = {**search_response_dict,**jsonpage_dict}
+    data_report(data=final_data)
     n()
     
 
 def about():
         #extract the anime info from a div with class anime-synopsis
         soup = BeautifulSoup((requests.get(episode_page_format).text),'lxml')
         abt = soup.select('.anime-synopsis')
         return abt[0].text.strip()
 
-# USING tqdm to simulate download progress
-def progress(size):
-    size = int(''.join(filter(str.isdigit,str(size))))
-    # Simulating the download
-    
-    with tqdm.tqdm(total=size, unit='B', unit_scale=True, desc='Downloading') as pbar:
-        bytes_downloaded = 0
-        
-        while bytes_downloaded < size:
-            # Simulating downloading some data
-            time.sleep(0.5)  # Simulating time delay
-            update = 60 * 1024
-            bytes_downloaded += update # Simulating downloaded bytes
-
-            pbar.update(update)  # Update the progress bar with the number of downloaded bytes
-
-    # File download completed
-    driver.quit()
-    print("Download completed.")
 
-
-def download(arg: int = 1):
+def download(arg = 1,barg:str = "firefox"):
     # using return value of the search function to get the page
     # using the json data from the page url to get page where the episodes to watch are
 
     print()
 
     #session string of the stream episode
     episode_session = jsonpage_dict['data'][arg-1]['session']
@@ -354,188 +288,111 @@
     
     #the linkpahe variable carries a list of the characters of the link
     #so the pahewin variable will return the link webpage content
     pahe_win = requests.get(f'{[ch for ch in linkpahe][0]}').content
     
     #getting the link to the kwik download page
     kwik = (pahe_soup:=BeautifulSoup(pahe_win,'lxml')).find('a', class_='redirect')['href']
+    down_url = kwik.replace("/f/","/d/")
     
     Banners.getting_eps(arg)
-    
-    # ---------------------------Using selenium to render and clickk the download button------------------------
 
-    # going to the download page
-    driver.get(kwik)
+    Banners.downloading(animepicked,arg)
     
-    # getting the title
-    kwik_soup = BeautifulSoup((requests.get(kwik).text),'lxml')
-    # filename = kwik_soup.find('h1',class_ = 'title').text.strip()
-    size = (kwik_soup.find('abbr')['title'])
-
-    # Starting download banner
-    Banners.start_dl(arg)
-    
-    WebDriverWait(driver, 15).until(EC.presence_of_element_located(
-        (By.XPATH, "//form[@method = 'POST']/button[contains(@class, 'button')]")))
-
-    element = driver.find_element(
-        By.XPATH, "//form[@method = 'POST']/button[contains(@class, 'button')]")
-
-    # the first click will click on the ad on the screeen
-    try:
-        ad=driver.find_element(By.XPATH, '/html/body/div[2]/a')
-        
-        ad.click()
-        element.click()
-        # the second click will download the content
-    except:    
-        element.click()
-        n()
-
+    kwik_download(url=kwik,posturl=down_url,dpath="/home/haxsys/Downloads",ep=arg)
     
-    Banners.downloading(animepicked,arg)
-    progress(size)
     
 
 
 
 
 
-def multi_download_verbose(arg):
-    print("To make efficient use of the multi download function,\nit is advised you have a very fast and stable internet connection")
+# def multi_download_verbose(arg):
+#     print("      To make efficient use of the multi download function,\nit is advised you have a very fast and stable internet connection")
     
     
-    n()
+#     n()
     
-    # given arg specifies '-' for range
-    if '-'in str(arg):
-        # parsing the arg to get individial eps
-        epr = list(x for x in arg.split('-'))
+#     # given arg specifies '-' for range
+#     if '-'in str(arg):
+#         # parsing the arg to get individial eps
+#         epr = list(x for x in arg.split('-'))
 
-        # list of the range of eps
-        episodes_list = list(range(int(epr[0]),int(epr[1]) + 1))
-        
-    else:
-        # classic arg separated by comma
-        episodes_list = [int(x) for x in arg.split(',')]
+#         # list of the range of eps
+#         episodes_list = list(range(int(epr[0]),int(epr[1]) + 1))
         
+#     else:
+#         # classic arg separated by comma
+#         episodes_list = [int(x) for x in arg.split(',')]
+
         
-            
-    for elem in episodes_list:
+#     for elem in episodes_list:
                 
-        episode_session = jsonpage_dict['data'][elem]['session']
+#         episode_session = jsonpage_dict['data'][elem]['session']
             
 
-        #stream page url format
-        stream_page_url = f'https://animepahe.com/play/{session_id}/{episode_session}'
-        n()
+#         #stream page url format
+#         stream_page_url = f'https://animepahe.com/play/{session_id}/{episode_session}'
+#         n()
         
-        stream_page_soup = BeautifulSoup(requests.get(f'{stream_page_url}').content,'lxml')
+#         stream_page_soup = BeautifulSoup(requests.get(f'{stream_page_url}').content,'lxml')
         
-        dload = stream_page_soup.find_all('a',class_='dropdown-item',target="_blank")
+#         dload = stream_page_soup.find_all('a',class_='dropdown-item',target="_blank")
         
-        from re import search
+#         from re import search
 
 
-        # for link in dload:
-        #     stlink = str(link)
-        #     match = if not (search(r'(360p|1080p|eng)', stlink))
-        #     if match:
-        #         for link in stlink:
-        #             soup = BeautifulSoup(link, 'html.parser')
-        #             href = soup.a['href']
-        #             print(href)
+#         # for link in dload:
+#         #     stlink = str(link)
+#         #     match = if not (search(r'(360p|1080p|eng)', stlink))
+#         #     if match:
+#         #         for link in stlink:
+#         #             soup = BeautifulSoup(link, 'html.parser')
+#         #             href = soup.a['href']
+#         #             print(href)
         
-        # i am sure u are not wise enough to know what is going on
-        #but the code above was shortened to the code below
-        #using walrus operator and list comprehension
-        #and it return a list of chars which when combined will return the link
-        linkpahe = [(BeautifulSoup(stlink, 'html.parser').a['href']) for link in dload if not (search(r'(360p|1080p|eng)', stlink:=str(link)))]
+#         # i am sure u are not wise enough to know what is going on
+#         #but the code above was shortened to the code below
+#         #using walrus operator and list comprehension
+#         #and it return a list of chars which when combined will return the link
+#         linkpahe = [(BeautifulSoup(stlink, 'html.parser').a['href']) for link in dload if not (search(r'(360p|1080p|eng)', stlink:=str(link)))]
         
-        #the linkpahe variable carries a list of the characters of the link
-        #so the pahewin variable will return the link webpage content
-        pahe_win = requests.get(f'{[ch for ch in linkpahe][0]}').content
+#         #the linkpahe variable carries a list of the characters of the link
+#         #so the pahewin variable will return the link webpage content
+#         pahe_win = requests.get(f'{[ch for ch in linkpahe][0]}').content
         
-        #getting the link to the kwik download page
-        kwik = (BeautifulSoup(pahe_win,'lxml')).find('a', class_='redirect')['href']
-
-        Banners.getting_eps(arg)
-        #--------------------------------------making a__init__ new tab to efficiently multithread the program---------------------
-        driver.execute_script("window.open('');")
-        driver.switch_to.window(driver.window_handles[-1])
-        # ---------------------------Using selenium to render and clickk the download button------------------------
+#         #getting the link to the kwik download page
+#         kwik = (BeautifulSoup(pahe_win,'lxml')).find('a', class_='redirect')['href']
+#         down_url = kwik.replace("/f/","/d/")
 
+#         Banners.getting_eps(arg)
         
-        # going to the download page
-        driver.get(kwik)
-        
-        # getting the title
-        kwik_soup = BeautifulSoup((requests.get(kwik).text),'lxml')
-        # filename = kwik_soup.find('h1',class_ = 'title').text.strip()
-        size = kwik_soup.find('abbr')['title']
-        
-        WebDriverWait(driver, 15).until(EC.presence_of_element_located(
-            (By.XPATH, "//form[@method = 'POST']/button[contains(@class, 'button')]")))
-
-        element = driver.find_element(
-            By.XPATH, "//form[@method = 'POST']/button[contains(@class, 'button')]")
-
-
-        Banners.start_dl(arg)
-    
-        try:
-            # the first click will click on the ad on the screeen
-            ad=driver.find_element(By.XPATH,"/html/body/div[2]/a")
-            ad.click()
-            # the second click will download the content
-            
-            n()
-        except:
-            pass
-        n()
-        
-        #to click the download btton
-        element.click()
-        Banners.downloading(animepicked,elem)
-        progress(size)
-        
-        
-        #return to original window
-        driver.switch_to.window(driver.window_handles[0])
-        # already downloading
-        print(f'Downloading Episode {elem} of {animepicked} NOW!!!!!!!')
-        print(f'Already Aired episode : {episto}')
-        n()
-
-
+#         Banners.downloading(animepicked,arg)
 
+#         kwik_download(url=kwik,posturl=down_url,dpath="/home/haxsys/Downloads")
+        
 
 
 
-    
 # This function unlike the one above downloads (if there is stable and fast connection) anime concurrently 
 def multi_download_optimized(arg):
+    
     arg = str(arg)
-    print("\n\nTo make efficient use of the multi download function,\nit is advised you have a very fast and stable internet connection\n")
-
-    print(f'Already aired Episodes : {episto}')
-
-    if '-' in arg:
-        # parsing the arg to get individial eps
-        epr = list(x for x in arg.split('-'))
 
-        # list of the range of eps
-        episodes_list = list(range(int(epr[0]),int(epr[1]) + 1))
-        # list of all the pahe win pages in html
-        pahe_win_pages= [BeautifulSoup(requests.get(f"https://animepahe.com/play/{session_id}/{jsonpage_dict['data'][int(x)-1]['session']}").content,'lxml')for x in episodes_list]   
+    # A new format for list comprehension
+    pahe_win_pages = [
         
-        
-    else:   
-        pahe_win_pages= [BeautifulSoup(requests.get(f"https://animepahe.com/play/{session_id}/{jsonpage_dict['data'][int(x)-1]['session']}").content,'lxml')for x in arg.split(',') ]
-
+    num
+    for segment in arg.split(",")
+    for num in (
+        range(int(segment.split("-")[0]), int(segment.split("-")[1]) + 1)
+        if "-" in segment
+        else [int(segment)]
+    )]
+    
     ddownlinks = [page.find_all('a',class_='dropdown-item',target="_blank",limit=3) for page in pahe_win_pages]
     # print(ddownlinks)
     
     n()
     
     
     # for link in ddownlinks:
@@ -547,123 +404,68 @@
     #             print(href)
     #             n()
 
     # n()
     
     linkpahe =[BeautifulSoup(str(url),'lxml').a['href'] for link in ddownlinks for url in link if not (search(r'(360p|1080p|eng)', str(url)))]
     
-    kwik_link = [(BeautifulSoup(requests.get(link).content,'lxml').find('a',class_ = "redirect"))['href'] for link in linkpahe ]
-    
-    # print(kwik_link)
-    
-    # getting the title
-    kwik_soup = BeautifulSoup((requests.get(kwik_link).text),'lxml')
-    # filename = kwik_soup.find('h1',class_ = 'title').text.strip()
-    size = kwik_soup.find('abbr')['title']
-    
+    kwik_link = [(BeautifulSoup(requests.get(link).content,'lxml').find('a',class_ = "redirect"))['href'] for link in linkpahe ]    
     
     Banners.getting_eps(arg)
     
-    for i,url in enumerate(kwik_link):    
-        
-        # ---------------------------Using selenium to render and click the download button------------------------
-        elem = (arg.split(','))[i]
-        
-        # going to the download page
-        driver.get(url)
+    Banners.downloading(animepicked,arg)
+    # for i,url in enumerate(kwik_link):
+    #     down_url = url.replace("/f/","/d/")
         
-        Banners.start_dl(arg)
+    #     ep = arg.split(",")[i]
         
+    #     Banners.downloading(animepicked,ep)
         
-        WebDriverWait(driver, 15).until(EC.presence_of_element_located(
-            (By.XPATH, "//form[@method = 'POST']/button[contains(@class, 'button')]")))
-
-        element = driver.find_element(
-            By.XPATH, "//form[@method = 'POST']/button[contains(@class, 'button')]")
+    #     kwik_download(url,down_url,dpath="/home/haxsys/Downloads")
         
+    with concur.ThreadPoolExecutor(max_workers=len(kwik_link)) as executor:
+        futures = []
         
-        
-        try:
-            Banners.downloading(animepicked,elem)
-            # the first click will click on the ad on the screeen
-            ad=driver.find_element(By.XPATH,"/html/body/div[2]/a")
-            print(f"ad clicked for ep {elem}\n")
-            ad.click()
-            # the second click will download the content
-            element.click()
-            print(f"element clicked for ep {elem}\n")
-            
+        for i,url in enumerate(kwik_link):
+            down_url = url.replace("/f/","/d/")
+            ep = arg.split(",")[i]
+            future = executor.submit(kwik_download, url,down_url,dpath="/home/haxsys/Downloads",ep=ep)
             n()
-        except:
-            print(f"click in exception for ep {elem}\n")
-            
-            element.click()
-        
-        
-        #to click the download btton
-        # element.click()
+            n()
+            futures.append(future)
 
 
-        # already downloading
-        progress(size)
-        print(f'{animepicked} ep-{elem} Downloading ... ')
-        n()
-        
+        # Wait for all tasks to complete
+        concur.wait(futures)
+        # for future in futures:
+        #     future.result()
         
         
-    # wait = WebDriverWait(driver, 10)
-    # wait.until(EC.presence_of_element_located((By.XPATH, f'//a[text()="{file_name}"]')))
 
-    # Close the driver
-    driver.quit()
-    print(f'Downloaded Episode {arg} of {animepicked} !!!!!')
+
+    
 
             
-def multi_download_classic(eps: str):
+def multi_download_verbose(eps: str):
     # given arg specifies '-' for range
-    if '-'in str(eps):
-        # parsing the eps to get individial eps
-        epr = list(x for x in eps.split('-'))
-
-        # list of the range of eps
-        episodes = list(range(int(epr[0]),int(epr[1]) + 1))
-        
-    else:
-        # classic eps separated by comma, stlink:=str(link)))]
-        episodes = [int(x) for x in eps.split(',')]
+    # New format for list comprehension  
+    episodes = [
+        num
+        for segment in eps.split(",")
+        for num in (
+            range(int(segment.split("-")[0]), int(segment.split("-")[1]) + 1)
+            if "-" in segment
+            else [int(segment)]
+        )]
     
     for ep in episodes:
         download(ep)
         print(f"{animepicked} ep-{ep} downloading")
 
-
- 
-
-if current_system_os.lower() == "windows": # we need this only in windows
-    # get list of currently running firefox processes (for in case -- keyboardInterrupt occurs)
-    tasklist = subprocess.check_output(['tasklist', '/fi', 'imagename eq firefox.exe'], shell=True).decode()
-    currentFFIDs = re.findall(r"firefox.exe\s+(\d+)", tasklist)
-
-def winKeyInterruptHandler():
-    #exit progress bar if initiated
-    # close_progress_bar()
-        
-    #find new firefox processes
-    tasklist = subprocess.check_output(['tasklist', '/fi', 'imagename eq firefox.exe'], shell=True).decode()
-    newFFIDs = set(re.findall(r"firefox.exe\s+(\d+)", tasklist)).difference(currentFFIDs)
-
-    #kills spawned firefox drivers -- (may also crash some tabs in other firefox sessions)
-    taskkill = 'taskkill /f '+''.join(["/pid "+f+" " for f in newFFIDs]).strip()
-    subprocess.check_output(taskkill.split(), shell=True)
-
-    print("\nKeyboardInterrupt : Exiting with dirty hands..")
-    print("You may experience a tab-crash in your open firefox sessions")  
     
-
-
 # ----------------------------------------------End of All the Argument Handling----------------------------------------------------------
 
 # To enable interaction with the program instead of command line argument    
 def interactive_main():
     
     # Search prompt for search function
     lookup_anime = str(input("Search an anime [e.g 'one piece'] >> "))
@@ -677,70 +479,66 @@
     # handling the selected anime metadata
     index(select_index)
     
     # summary info on the selected anime
     info = about()
     Banners.i_info(info)
     
-    # # browser handling prompt
-    browse = str(input("Enter the browser favorite browser [ff,chrome,firefox e.t.c] >> "))
-    browser(browse)
-    
     # Handling episode to download prompt
-    download_type = str(input("""
+    download_type = input("""
     Enter the type of download facilty you want
     
     1. s or single_download for single episode download
     2. md or multi_download for multi episode download
-    3. v or md_verbose for a verbose variant of the md function
-    4. c or md_classic for a classic variant of the md function
-    5. i for more in -depth info on the options above 
+    3. v or md_verbose for a verbose variant of the md function[SLOW]
+    4. i for more in -depth info on the options above 
     
     >> """)
-    )
     print("\n")
-    ep_to_download = int(input("    Enter episode(s) to download >> "))
+    ep_to_download = (input("    Enter episode(s) to download >> "))
     
     switch = {
-        1:download(ep_to_download),
-        2:multi_download_optimized(ep_to_download),
-        3:multi_download_verbose(ep_to_download),
-        4:multi_download_classic(ep_to_download),
-        5:info,
-        's':switch[1],
-        'md':switch[2],
-        'v':switch[3],
-        'c':switch[4],
-        'i':switch[5],
-        'single_download':download(ep_to_download),
-        'multi_download':switch[2],
-        'md_verbose':switch[3],
-        'md_classic':switch[4],
-        'info':switch[5]
+        1:download,
+        2:multi_download_optimized,
+        3:multi_download_verbose,
+        4:info,
+        's':download,
+        'md':multi_download_optimized,
+        'v':multi_download_verbose,
+        'i':info,
+        'single_download':download,
+        'multi_download':multi_download_optimized,
+        'md_verbose':multi_download_verbose,
+        'info':info
     }
     
     # initiating the action for the choice
-    switch[download_type]
+    selected_function = switch.get(download_type)
 
-def command_main(args):
+    if selected_function:
+        selected_function(ep_to_download)
+    else:
+        print("Invalid input. Please select a valid option.")
 
+
+
+
+
+
+def command_main(args):
+    global barg
     barg = args.browser
     sarg = args.search
     sharg = args.search_hidden
     iarg = args.index
     sdarg = args.single_download
     mdarg = args.multi_download_optimized
     mdvarg = args.multi_download_verbose
-    mdcarg = args.multi_download_classic
     abtarg = args.about
     
-    # browser
-    if barg:
-        browser(barg)
-    
     # search function
     if sarg != None:
         lookup(sarg)
     elif type(sarg) == float:
         print("The search argument does not accept a float value")
     else:
         pass
@@ -770,19 +568,20 @@
     if sdarg != None:
         download(sdarg)
     else:
         pass
     
     # Multi_download function(s)
         
-    if mdcarg:
-        multi_download_classic(mdcarg)
+    if mdvarg:
+        multi_download_verbose(mdvarg)
         
     if mdarg:
         multi_download_optimized(mdarg)
+    
 
         
 
 def main():
     # ===================================== Handling Arguments and other involved function============================================
     parser = argparse.ArgumentParser()
 
@@ -804,18 +603,15 @@
 
     parser.add_argument('-d', '--single_download', type=int,
                         help='Used to download a single episode of an anime')
 
     parser.add_argument('-md', '--multi_download_optimized',
                         help='Used to download multiple episodes of an anime concurrently,a string of ints separated by commas[FASTER]')
 
-    parser.add_argument('-mdv', '--multi_download_verbose',
-                        help='Used to download multiple episodes of an anime and show verbose,a string of ints separated by commas[SLOWER]')
-
-    parser.add_argument('-mdc', '--multi_download_classic',
+    parser.add_argument('-mdc', '--multi_download_verbose',
                         help='[SLOW]Used to download multiple episodes of an anime and show verbose,a string of ints separated by commas,simply uses SD in a loop')
 
     parser.add_argument('-a', '--about',
                         help='Outputs an overview information on the anime',action='store_true')
 
 
 
@@ -827,33 +623,23 @@
     else:
         # No command line arguments, run interactive mode
         interactive_main()
 
 
 
 
+
+
 if __name__ == '__main__':
     # INTRO BANNER
-    Banners.header() 
     main()
-
-
-final_data = {**search_response_dict,**jsonpage_dict}
+else:
+    Banners.header()
+    
 
 n()
-def data_report(filepath = "autopahe_data.json",data = None):
-    if data:
-        # Read existing JSON data from file
-        with open(filepath, 'r') as json_file:
-            existing_data = load(json_file)
-
-        existing_data.update(data)
-            
-        with open(filepath,"w") as st:
-            dump(existing_data,st)
-
 
 finish = time.perf_counter()
 
 print(f'Finish time is {round(finish-start,2)}\n')
```

### Comparing `autopahe-1.0.0/autopahe.egg-info/PKG-INFO` & `autopahe-2.0/autopahe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 1.0.0
+Version: 2.0
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 <!-- Badges -->
-<!-- [![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/) -->
+[![PyPI version](https://badge.fury.io/py/autopahe.svg)](https://pypi.org/project/autopahe/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/autopahe/)
 [![License](https://img.shields.io/github/license/haxsysgit/autopahe?color=brightgreen)](https://github.com/haxsysgit/autopahe/blob/main/license.md)
 [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/autopahe?color=important)](https://github.com/haxsysgit/autopahe/issues)
 <!--LineBreak-->
 [![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/autopahe/)
 [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/autopahe/)
 <!-- Badges -->
@@ -67,15 +67,15 @@
   - In case of multiple options, each options must be seperated by a `,`
   - Example: `1, 3, 6-11` : downloads episodes 1,3,6,7,8,9,10,11
 
 ## Command line features
 To use the script, run it in your terminal using the following command:
 
 ```shell
-python fetchanime.py [-h] [-b BROWSER] [-s SEARCH] [-sh SEARCH_HIDDEN] [-i INDEX] [-sd SINGLE_DOWNLOAD] [-md MULTI_DOWNLOAD_OPTIMIZED] [-mdv MULTI_DOWNLOAD_VERBOSE] [-a ABOUT]
+python auto_pahe.py [-h] [-b BROWSER] [-s SEARCH] [-sh SEARCH_HIDDEN] [-i INDEX] [-sd SINGLE_DOWNLOAD] [-md MULTI_DOWNLOAD_OPTIMIZED] [-mdv MULTI_DOWNLOAD_VERBOSE] [-a ABOUT]
 ```
 
 Here are the available options:
 
 - `-h`, `--help`: show the help message and exit
 - `-b`, `--browser`: choose the browser to use (`chrome`,`firefox` or `brave`). If omitted, the script will use `chrome` by default. Use `ffgui` for a GUI Firefox window.
 - `-s`, `--search`: search for an anime using a keyword. The script will display a list of matching results.
```

### Comparing `autopahe-1.0.0/setup.py` & `autopahe-2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'autopahe',
-    version = '1.0.0',
+    version = '2.0',
     author_email="pentacker@gmail.com",
     description = "A python script to automate downloads from animepahe",
     url = "https://github.com/haxsysgit/autopahe",
     author = "Elenasulu Arinze",
     license = "MIT",
     py_modules = [
         'autopahe',
```

