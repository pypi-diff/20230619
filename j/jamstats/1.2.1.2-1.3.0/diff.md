# Comparing `tmp/jamstats-1.2.1.2.tar.gz` & `tmp/jamstats-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jamstats-1.2.1.2.tar", last modified: Tue May  2 15:32:05 2023, max compression
+gzip compressed data, was "dist/jamstats-1.3.0.tar", last modified: Mon Jun 19 16:00:55 2023, max compression
```

## Comparing `jamstats-1.2.1.2.tar` & `jamstats-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/
--rw-r--r--   0 damonmay   (501) staff       (20)      424 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)     8788 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/README.md
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/bin/
--rwxr-xr-x   0 damonmay   (501) staff       (20)    11127 2023-04-01 22:28:27.000000 jamstats-1.2.1.2/bin/jamstats
--rwxr-xr-x   0 damonmay   (501) staff       (20)    10659 2023-05-02 00:48:27.000000 jamstats-1.2.1.2/bin/jamstats-nogui
--rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/setup.cfg
--rw-r--r--   0 damonmay   (501) staff       (20)      867 2023-05-02 15:31:35.000000 jamstats-1.2.1.2/setup.py
--rw-r--r--   0 damonmay   (501) staff       (20)      833 2023-05-02 15:25:08.000000 jamstats-1.2.1.2/setup_nogui.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/data/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/data/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-1.2.1.2/src/jamstats/data/game_data.py
--rw-r--r--   0 damonmay   (501) staff       (20)    36908 2023-04-30 05:44:55.000000 jamstats-1.2.1.2/src/jamstats/data/json_to_pandas.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/io/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/io/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/io/scoreboard_json_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/io/scoreboard_server_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/io/tsv_io.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/plots/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/plots/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    43584 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/plots/jamplots.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-1.2.1.2/src/jamstats/plots/plot_together.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-1.2.1.2/src/jamstats/plots/plot_util.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9703 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/plots/skaterplots.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/resources/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/resources/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/util/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/util/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/util/resources.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/web/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/web/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    15262 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/web/statserver.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/
--rw-r--r--   0 damonmay   (501) staff       (20)      424 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)      818 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/SOURCES.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/dependency_links.txt
--rw-r--r--   0 damonmay   (501) staff       (20)      184 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/requires.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/top_level.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/
+-rw-r--r--   0 damonmay   (501) staff       (20)      444 2023-06-19 16:00:55.000000 jamstats-1.3.0/PKG-INFO
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/bin/
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    10659 2023-06-10 20:15:30.000000 jamstats-1.3.0/bin/jamstats-nogui
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    11127 2023-04-01 22:28:27.000000 jamstats-1.3.0/bin/jamstats
+-rw-r--r--   0 damonmay   (501) staff       (20)     8790 2023-06-17 18:34:25.000000 jamstats-1.3.0/README.md
+-rw-r--r--   0 damonmay   (501) staff       (20)      830 2023-06-10 20:15:30.000000 jamstats-1.3.0/setup_nogui.py
+-rw-r--r--   0 damonmay   (501) staff       (20)      914 2023-06-19 15:58:38.000000 jamstats-1.3.0/setup.py
+-rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-06-19 16:00:55.000000 jamstats-1.3.0/setup.cfg
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats.egg-info/
+-rw-r--r--   0 damonmay   (501) staff       (20)      444 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats.egg-info/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)      818 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats.egg-info/SOURCES.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)      200 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats.egg-info/requires.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats.egg-info/top_level.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats.egg-info/dependency_links.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/util/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/util/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/util/resources.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/web/
+-rw-r--r--   0 damonmay   (501) staff       (20)    15415 2023-06-12 00:03:02.000000 jamstats-1.3.0/src/jamstats/web/statserver.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/web/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/resources/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/resources/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/io/
+-rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/io/tsv_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.3.0/src/jamstats/io/scoreboard_json_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/io/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.3.0/src/jamstats/io/scoreboard_server_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/data/
+-rw-r--r--   0 damonmay   (501) staff       (20)    37754 2023-06-17 18:24:19.000000 jamstats-1.3.0/src/jamstats/data/json_to_pandas.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/data/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    13045 2023-06-18 17:00:21.000000 jamstats-1.3.0/src/jamstats/data/game_data.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-06-19 16:00:55.000000 jamstats-1.3.0/src/jamstats/plots/
+-rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-1.3.0/src/jamstats/plots/plot_together.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.3.0/src/jamstats/plots/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    15144 2023-06-18 17:00:06.000000 jamstats-1.3.0/src/jamstats/plots/skaterplots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    43578 2023-06-17 18:24:19.000000 jamstats-1.3.0/src/jamstats/plots/jamplots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-1.3.0/src/jamstats/plots/plot_util.py
```

### Comparing `jamstats-1.2.1.2/README.md` & `jamstats-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
     <img src="https://github.com/dhmay/jamstats/blob/main/resources/jamstats_logo.png" width="300">
 </p>
 
-Tools for displaying roller derby game data from the [CRG scoreboard](https://github.com/rollerderby/scoreboard) (versions 4.x and 5.x). 
+Tools for displaying roller derby game data from the [CRG scoreboard](https://github.com/rollerderby/scoreboard) (versions 4.x and later). 
 
 You can build jamstats plots from game JSON files **online!** No need to install anything. Check out [jamstats.net](https://jamstats.net). 
 
 So, why download Jamstats and run it on your laptop? To connect to a live game on a running scoreboard! 
 
 **Jamstats is great for announcers!** See **who's on the track** (including positions and penalties), vital game stats and **rosters** for both teams and officials. You can even connect to a live scoreboard [from anywhere on the Internet](https://github.com/dhmay/jamstats#connecting-to-a-proxied-scoreboard-from-the-internet) using wsproxy!
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
    [https://github.com/dhmay/jamstats/blob/main/resources/jamstats_logo.png]
 Tools for displaying roller derby game data from the [CRG scoreboard](https://
-github.com/rollerderby/scoreboard) (versions 4.x and 5.x). You can build
+github.com/rollerderby/scoreboard) (versions 4.x and later). You can build
 jamstats plots from game JSON files **online!** No need to install anything.
 Check out [jamstats.net](https://jamstats.net). So, why download Jamstats and
 run it on your laptop? To connect to a live game on a running scoreboard!
 **Jamstats is great for announcers!** See **who's on the track** (including
 positions and penalties), vital game stats and **rosters** for both teams and
 officials. You can even connect to a live scoreboard [from anywhere on the
 Internet](https://github.com/dhmay/jamstats#connecting-to-a-proxied-scoreboard-
```

### Comparing `jamstats-1.2.1.2/bin/jamstats` & `jamstats-1.3.0/bin/jamstats`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/bin/jamstats-nogui` & `jamstats-1.3.0/bin/jamstats-nogui`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/setup.py` & `jamstats-1.3.0/setup_nogui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='jamstats',
-    version='1.2.1.2',
-    description='Data processing, stats and plots on roller derby scoreboard JSON files',
+    name='jamstats-nogui',
+    version='1.2.1.4',
+    description='Data processing, stats and plots on roller derby scoreboard JSON files. No-GUI version.',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
-    packages=find_packages('src', exclude=['test']),
-    scripts=['bin/jamstats', 'bin/jamstats-nogui'],
-    install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'gooey>=1.0.8.1', 'websocket-client>=1.2.1',
+    packages=['jamstats'],
+    scripts=['bin/jamstats-nogui'],
+    install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'websocket-client>=1.2.1',
 		      'Flask-SocketIO>=5.3.2', 'python-engineio>=4.3.4', 'gevent>=22.10.2', 'gevent-websocket>=0.10.1'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
     ],
     project_urls={
```

### Comparing `jamstats-1.2.1.2/setup_nogui.py` & `jamstats-1.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jamstats',
-    version='1.2.1.1',
+    version='1.3.0',
     description='Data processing, stats and plots on roller derby scoreboard JSON files',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
     packages=find_packages('src', exclude=['test']),
-    scripts=['bin/jamstats-nogui'],
-    install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'websocket-client>=1.2.1',
+    scripts=['bin/jamstats', 'bin/jamstats-nogui'],
+    install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1',
+                      'wxpython==4.2.0',
+		      'gooey>=1.0.8.1', 'websocket-client>=1.2.1',
 		      'Flask-SocketIO>=5.3.2', 'python-engineio>=4.3.4', 'gevent>=22.10.2', 'gevent-websocket>=0.10.1'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
     ],
     project_urls={
```

### Comparing `jamstats-1.2.1.2/src/jamstats/data/json_to_pandas.py` & `jamstats-1.3.0/src/jamstats/data/json_to_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 logger = logging.Logger(__name__)
 
 # Columns to keep at the team+jam level
 TEAMJAM_SUMMARY_COLUMNS = [
     "Calloff", "Injury", "JamScore", "Lead",
     "Lost", "NoInitial", "StarPass", "TotalScore", "jammer_name", "jammer_number",
-    "pivot_name", "pivot_number",
+    "pivot_name", "pivot_number", "jammer_points", "pivot_points",
     "Skaters"]
 
 
 def load_json_derby_game(game_json) -> DerbyGame:
     """Load the derby game stored in a json dict
 
     Returns:
@@ -65,16 +65,16 @@
 
     Returns:
         pd.DataFrame: result dataframe
     """
     game_dict = game_json["state"]
 
     json_major_version = get_json_major_version(game_dict)
-
-    if json_major_version == 5:
+    logger.debug(f"Found CRG version {json_major_version}")
+    if json_major_version != 4:
         # v5.0 adds a "Game(<game_id>)" chunk to almost every key. Get rid of that.
 
         # In-process games have both "CurrentGame" fields and fields
         # annotated with a game identifier. Complete games don't have
         # "CurrentGame" fields. So, if we find a "CurrentGame" field,
         # use those and strip out all the fields with a game identifier.
         logger.debug(f"Found version 5. Checking for in-progress game...")
@@ -197,14 +197,15 @@
     # Get rid of weird characters in team names
     team_name_1 = cleanup_team_name(team_name_1)
     team_name_2 = cleanup_team_name(team_name_2)
 
 
     game_datestring = ""
     game_starttimestring = ""
+    logger.debug("Getting game date and time.")
     # Get game date and time
     try:
         game_datestring = pdf_game_state[
             pdf_game_state.key == "ScoreBoard.EventInfo(Date)"].value.iloc[0]
         game_starttimestring = pdf_game_state[
             pdf_game_state.key == "ScoreBoard.EventInfo(StartTime)"].value.iloc[0]
     except Exception:
@@ -215,14 +216,15 @@
                 pdf_game_state.key == "ScoreBoard.Period(1).LocalTimeStart"].value.iloc[0]
             game_datestring = game_dateandtimestring.split("T")[0]
             game_starttimestring = game_dateandtimestring.split("T")[1][:8]
         except Exception:
             logger.debug("Still could not find game date and time.")
             pass
 
+    logger.debug("Getting team jammer names and numbers.")
     # Get team jammer names and numbers
     team_1_jammer_name = ""
     team_2_jammer_name = ""
     team_1_jammer_number = ""
     team_2_jammer_number = ""
     try:
         team_1_jammer_name = pdf_game_state[
@@ -427,22 +429,20 @@
         team_name_2 (str): Name of team 2
 
     Returns:
         pd.DataFrame: _description_
     """
     logger.debug("extract_roster begin")
     json_major_version = get_json_major_version_from_pdf(pdf_game_state)
-    if json_major_version == 5:
-        logger.debug("JSON version 5")
-        team_string_1 = f"Team\(1\)"
-        team_string_2 = f"Team\(2\)"
-    elif json_major_version == 4:
-        logger.debug("JSON version 4")
+    if json_major_version == 4:
         team_string_1 = f"PreparedTeam\({team_name_1}\)"
         team_string_2 = f"PreparedTeam\({team_name_2}\)"
+    else:
+        team_string_1 = f"Team\(1\)"
+        team_string_2 = f"Team\(2\)"
     
     team_string_1 = cleanup_team_name(team_string_1)
     team_string_2 = cleanup_team_name(team_string_2)
 
     logger.debug(f"Looking for teams in roster: {team_string_1}, {team_string_2}")
     pdf_game_state_roster = pdf_game_state.loc[
         pdf_game_state.key.str.contains(
@@ -452,29 +452,29 @@
     ].copy()
 
     pdf_game_state_roster["team"] = [
         chunks[1][chunks[1].index("(") + 1:chunks[1].index(")")]
         for chunks in pdf_game_state_roster.key_chunks]
     logger.debug("Roster rows by team:")
     logger.debug(pdf_game_state_roster.team.value_counts())
-    if json_major_version == 5:
+    if json_major_version != 4:
         # Version 4 stored the team name. Version 5 stores the number,
         # so translate.
         pdf_game_state_roster["team"] = [team_name_1 if team == "1"
                                          else team_name_2 if team == "2"
                                          else "????"
                                          for team in pdf_game_state_roster["team"]]
     pdf_game_state_roster["skater"] = [
         chunks[2][chunks[2].index("(") + 1:chunks[2].index(")")]
         for chunks in pdf_game_state_roster.key_chunks]
     pdf_game_state_roster["roster_key"] = [
         chunks[3] for chunks in pdf_game_state_roster.key_chunks]
     # dump a bunch of extraneous columns
     pdf_game_state_roster = pdf_game_state_roster[pdf_game_state_roster.roster_key.isin(
-        ["Id", "Name", "RosterNumber", "Number", "team"]
+        ["Id", "Name", "RosterNumber", "Number", "team", "Pronouns"]
     )]
     pdf_roster = pdf_game_state_roster.pivot(index="skater", columns="roster_key", values="value")
     logger.debug("pdf_roster columns: " + str(pdf_roster.columns) + 
                  ". Before dropping nulls, length: " + str(len(pdf_roster)))
     pdf_roster = pdf_roster[pdf_roster.Id.notnull()]
     logger.debug("After dropping nulls, length: " + str(len(pdf_roster)))
 
@@ -562,21 +562,31 @@
     scoringtrip_cols_to_rename = [x for x in pdf_scoringtrips.columns
                                   if x != "prd_jam"]
 
     pdf_ateamjams_summary_withscoringtrips = pdf_ateamjams_summary.merge(
         pdf_scoringtrips, on="prd_jam")
     logger.debug(f"After adding scoring trips: {len(pdf_ateamjams_summary_withscoringtrips)}")
     logger.debug(pdf_ateamjams_summary_withscoringtrips.columns)
+
+    # calculate points earned by jammer and by pivot (in case of star pass)
+    pdf_ateamjams_summary_withscoringtrips["jammer_points"] = (
+        pdf_ateamjams_summary_withscoringtrips["JamScore"] -
+        pdf_ateamjams_summary_withscoringtrips["AfterSPScore"])
+    pdf_ateamjams_summary_withscoringtrips["pivot_points"] = (
+        pdf_ateamjams_summary_withscoringtrips["AfterSPScore"])
+
     pdf_ateamjams_summary_kept = pdf_ateamjams_summary_withscoringtrips[
         ["prd_jam"] + TEAMJAM_SUMMARY_COLUMNS + scoringtrip_cols_to_rename]
 
     pdf_ateamjams_summary_kept_colsrenamed = pdf_ateamjams_summary_kept.rename(
         columns={col: f"{col}_{team_number}"
                  for col in TEAMJAM_SUMMARY_COLUMNS + scoringtrip_cols_to_rename})
 
+
+
     return pdf_ateamjams_summary_kept_colsrenamed.sort_values("prd_jam")
 
 
 def extract_team_perjam_skaters(pdf_ateamjams_data: pd.DataFrame,
                                 pdf_roster: pd.DataFrame) -> pd.DataFrame:
     """Calculate the list of skater names per jam for this team.
 
@@ -625,31 +635,38 @@
 
     Returns:
         pd.DataFrame: scoring trip summary pdf with one row per jam
     """
     jams = []
     scoring_pass_counts = []
     first_scoring_pass_durations_seconds = []
+    logger.debug("Parsing scoring trips...")
     for prd_jam in sorted(list(set(pdf_ateamjams_data.prd_jam))):
         pdf_thisjam = pdf_ateamjams_data[pdf_ateamjams_data.prd_jam == prd_jam]
         thisjam_keys = set(pdf_thisjam.key)
         thisjam_scoringtrip_keys = [x for x in thisjam_keys if "ScoringTrip" in x]
         scoring_trip_chunks = [akey.split(".")[4] for akey in thisjam_scoringtrip_keys]
         scoring_trip_numbers = [int(achunk[achunk.index("(")+1:-1])
                                 for achunk in scoring_trip_chunks]
         n_scoring_passes = max(scoring_trip_numbers)
         jams.append(prd_jam)
         scoring_pass_counts.append(n_scoring_passes)
         # "time to lead" (time between the start whistle and the lead jammer getting lead)
         # is stored as the Duration of ScoringTrip(1), which is a fake "scoring" trip
         # representing the initial pass.
-        first_trip_duration_key = [x for x in thisjam_scoringtrip_keys
-                                   if x.endswith("ScoringTrip(1).Duration")][0]
-        first_trip_duration_seconds = int(list(
-            pdf_thisjam[pdf_thisjam.key == first_trip_duration_key].value)[0]) / 1000
+        # At least once, I've seen a file with a jam with no ScoringTrip(1), so putting
+        # in a try block. 
+        try:
+            first_trip_duration_key = [x for x in thisjam_scoringtrip_keys
+                                    if x.endswith("ScoringTrip(1).Duration")][0]
+            first_trip_duration_seconds = int(list(
+                pdf_thisjam[pdf_thisjam.key == first_trip_duration_key].value)[0]) / 1000
+        except Exception:
+            logger.warn(f"Jam {prd_jam}, missing first trip data, setting TTI to 0")
+            first_trip_duration_seconds = 0
         first_scoring_pass_durations_seconds.append(
             first_trip_duration_seconds
         )
     pdf_scoring_pass_counts = pd.DataFrame({
         "prd_jam": jams,
         "n_scoring_trips": scoring_pass_counts,
         "first_scoring_pass_durations": first_scoring_pass_durations_seconds
@@ -748,20 +765,20 @@
         pdf_game_state (pd.DataFrame): game json in dataframe
 
     Returns:
         Dict[str, str]: map from letter codes to names
     """
     # this code is very inefficient -- will do string matching on the whole game dictionary
     logger.debug(f"build_penalty_code_name_map begin, version=={json_major_version}")
-    if json_major_version == 5:
-        pdf_penalty_codes = pdf_game_state[
-            pdf_game_state["key"].str.contains("PenaltyCode")].copy()
-    else:
+    if json_major_version == 4:
         pdf_penalty_codes = pdf_game_state[pdf_game_state["key"].str.startswith(
             "ScoreBoard.PenaltyCodes.Code")].copy()
+    else:
+        pdf_penalty_codes = pdf_game_state[
+            pdf_game_state["key"].str.contains("PenaltyCode")].copy()
     pdf_penalty_codes["penalty_code"] = [x[-2:-1]
                                         for x in pdf_penalty_codes.key]       
     logger.debug(f"Built penalty code dataframe: {len(pdf_penalty_codes)} codes")
     if len(pdf_penalty_codes) == 0:
         logger.warn("Could not load penalty codes! Penalty plots will fail.")
     pdf_penalty_codes = pdf_penalty_codes[["penalty_code", "value"]].rename(columns={
         "value": "penalty_name"
```

### Comparing `jamstats-1.2.1.2/src/jamstats/io/scoreboard_json_io.py` & `jamstats-1.3.0/src/jamstats/io/scoreboard_json_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/src/jamstats/io/scoreboard_server_io.py` & `jamstats-1.3.0/src/jamstats/io/scoreboard_server_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/src/jamstats/io/tsv_io.py` & `jamstats-1.3.0/src/jamstats/io/tsv_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/src/jamstats/plots/jamplots.py` & `jamstats-1.3.0/src/jamstats/plots/jamplots.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,20 +73,20 @@
                    palette=team_color_palette, inner="stick")
     ax.set_title("Jams per jammer")
     ax.set_ylabel("Jams per jammer")
     # word-wrap too-long team names
     wordwrap_x_labels(ax)
 
     pdf_jammer_summary_1 = pdf_jams_data.groupby(
-        "jammer_name_1").agg({"JamScore_1": "mean", "Number": "count"}).rename(
-        columns={"JamScore_1": "mean_jam_score", "Number": "n_jams"})
+        "jammer_name_1").agg({"jammer_points_1": "mean", "Number": "count"}).rename(
+        columns={"jammer_points_1": "mean_jam_score", "Number": "n_jams"})
     pdf_jammer_summary_1.index = range(len(pdf_jammer_summary_1))
     pdf_jammer_summary_2 = pdf_jams_data.groupby(
-        "jammer_name_2").agg({"JamScore_2": "mean", "Number": "count"}).rename(
-        columns={"JamScore_2": "mean_jam_score", "Number": "n_jams"}) 
+        "jammer_name_2").agg({"jammer_points_2": "mean", "Number": "count"}).rename(
+        columns={"jammer_points_2": "mean_jam_score", "Number": "n_jams"}) 
     pdf_jammer_summary_2.index = range(len(pdf_jammer_summary_2))
 
     ax =axes[2]
     sns.scatterplot(x="n_jams", y="mean_jam_score", data=pdf_jammer_summary_1,
                     label=derby_game.team_2_name, color=team_color_palette[0])
     sns.scatterplot(x="n_jams", y="mean_jam_score", data=pdf_jammer_summary_2,
                     label=derby_game.team_2_name, color=team_color_palette[1])
@@ -217,14 +217,15 @@
     result = result + f"<table width=0% style='background-color: lightgray'><tr><td><br/>Penalty status:<ul>\
         <li style='color: yellow; background-color: lightgray'>Not Yet: skater on way to box</li>\
         <li style='color: red; background-color: lightgray'>Serving: skater in box</li>\
         <li style='color: green; background-color: lightgray'>Served: skater has completed serving penalty</li>\
         </li></ul></td></tr></table>"
     return result
 
+
 def get_singlejam_skaters_html(derby_game: DerbyGame, pdf_one_jam: pd.DataFrame,
                                anonymize_names: bool = False) -> str:
     """Get per-team tables of the skaters for a *single jam* as html
 
     Args:
         derby_game (DerbyGame): derby game
         pdf_one_jam (pd.DataFrame): table with a single row of jam data
@@ -471,22 +472,14 @@
     ax = plt.subplot(111)
     ax.axis('off')
     ax.table(cellText=pdf_game_teams_summary.values,
             colLabels=None, bbox=[0,0,1,1])
     return f
 
 
-def get_team1_roster_html(derby_game: DerbyGame,
-                          anonymize_names: bool = False) -> str:
-    return get_team_roster_html(derby_game, derby_game.team_1_name, anonymize_names=anonymize_names)
-
-def get_team2_roster_html(derby_game: DerbyGame,
-                          anonymize_names: bool = False) -> str:
-    return get_team_roster_html(derby_game, derby_game.team_2_name, anonymize_names=anonymize_names)
-
 def get_bothteams_roster_html(derby_game: DerbyGame,
                               anonymize_names: bool = False) -> str:
     """Get a html table of both teams' rosters
 
     Args:
         derby_game (DerbyGame): a derby game
 
@@ -498,14 +491,15 @@
     pdf_team2_roster = format_team_roster_fordisplay(derby_game, derby_game.team_2_name, anonymize_names=anonymize_names)
     pdf_team2_roster.index = range(len(pdf_team2_roster))
     pdf_bothteams_roster = pd.concat([pdf_team1_roster, pdf_team2_roster], axis=1)
     pdf_bothteams_roster = pdf_bothteams_roster.fillna("")
     styler = pdf_bothteams_roster.style.set_table_attributes("style='display:inline'").hide_index()
     return styler.render()
 
+
 def get_team_roster_html(derby_game: DerbyGame, team_name: str) -> str:
     """Build html table out of team roster
 
     Args:
         derby_game (DerbyGame): derby game
         team_name (str): team name
 
@@ -552,21 +546,29 @@
         derby_game (DerbyGame): derby game
         team_name (str): team name
 
     Returns:
         str: formatted team roster
     """
     pdf_team_roster = derby_game.pdf_roster[derby_game.pdf_roster.team == team_name]
-    pdf_team_roster = pdf_team_roster[["RosterNumber", "Name"]]
+    roster_cols = ["RosterNumber", "Name"]
+    roster_has_pronouns = "Pronouns" in pdf_team_roster.columns
+    if roster_has_pronouns:
+        roster_cols.append("Pronouns")
+    pdf_team_roster = pdf_team_roster[roster_cols]
     pdf_team_roster = pdf_team_roster.rename(columns={"Name": "Name", "RosterNumber": "Number"})
     if anonymize_names:
         name_dict = build_anonymizer_map(set(pdf_team_roster.Name))
         pdf_team_roster["Name"] = [name_dict[skater] for skater in pdf_team_roster.Name]  
     pdf_team_roster = pdf_team_roster.sort_values("Number")
     pdf_team_roster[f"{team_name} Skater"] = pdf_team_roster["Number"].astype(str) + " " + pdf_team_roster["Name"]
+    if roster_has_pronouns:
+        pdf_team_roster[f"{team_name} Skater"] = (
+            pdf_team_roster[f"{team_name} Skater"] + " (" + pdf_team_roster["Pronouns"] + ")")
+        pdf_team_roster = pdf_team_roster.drop(columns=["Pronouns"])
 
     team_number = 1 if team_name == derby_game.team_1_name else 2
     if show_jammers_and_pivots:
         pdf_jammer_counts = pd.DataFrame(derby_game.pdf_jams_data[f"jammer_number_{team_number}"].value_counts())
         pdf_jammer_counts = pdf_jammer_counts.rename(columns={f"jammer_number_{team_number}": "Jammed"})
         pdf_jammer_counts["Number"] = pdf_jammer_counts.index
         pdf_team_roster = pdf_team_roster.merge(pdf_jammer_counts, on="Number", how="left")
```

### Comparing `jamstats-1.2.1.2/src/jamstats/plots/plot_together.py` & `jamstats-1.3.0/src/jamstats/plots/plot_together.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/src/jamstats/plots/plot_util.py` & `jamstats-1.3.0/src/jamstats/plots/plot_util.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/src/jamstats/plots/skaterplots.py` & `jamstats-1.3.0/src/jamstats/plots/skaterplots.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,144 @@
 from matplotlib import pyplot as plt
 import random
 import string
 import pandas as pd
 from matplotlib import gridspec
 import traceback
 from jamstats.plots.plot_util import build_anonymizer_map
+import numpy as np
 
 
 logger = logging.Logger(__name__)
 
+
+def get_bothteams_jammertable_html(derby_game: DerbyGame,
+                                   anonymize_names: bool = False) -> str:
+
+    pdf_team1 = get_oneteam_jammer_pdf(derby_game, 1, anonymize_names=anonymize_names)
+    pdf_team2 = get_oneteam_jammer_pdf(derby_game, 2, anonymize_names=anonymize_names)
+    styler_1 = pdf_team1.style
+    styler_2 = pdf_team2.style
+    table_html_1 = styler_1.hide_index().render()
+    table_html_2 = styler_2.hide_index().render()
+    team1_tablecell_html = f"<H2>{derby_game.team_1_name} ({len(pdf_team1)})</H2>" + table_html_1
+    team2_tablecell_html = f"<H2>{derby_game.team_2_name} ({len(pdf_team2)})</H2>" + table_html_2
+    return "<table><tr valign='top'><td>" + team1_tablecell_html + "</td><td>" + team2_tablecell_html + "</td></tr></table>"
+
+def get_oneteam_jammer_pdf(derby_game: DerbyGame, team_number: int,
+                           anonymize_names: bool = False) -> pd.DataFrame:
+    """Load a table of jammer data for one team
+
+    Args:
+        derby_game (DerbyGame): derby game
+        team_number (int): team number
+        anonymize_names (bool, optional): Aonymize names? Defaults to False.
+
+    Returns:
+
+    """
+    pdf_jammer_data = derby_game.build_team_jammersummary_df(team_number)
+    if anonymize_names:
+        logger.debug("Anonymizing skater names.")
+        name_dict = build_anonymizer_map(set(pdf_jammer_data.Jammer))
+        pdf_jammer_data["Jammer"] = [name_dict[skater]
+                                     for skater in pdf_jammer_data.Jammer] 
+    pdf_jammer_data["% Lead"] = (pdf_jammer_data["Proportion Lead"] * 100).astype(int)
+    pdf_jammer_data = pdf_jammer_data.drop(columns=["Proportion Lead"])
+
+    pdf_jammer_data = pdf_jammer_data.rename(columns={
+        "Lead Count": "Lead",
+        "Lost Count": "Lost",
+        "Total Score": "Points"
+    })
+    pdf_jammer_data["Jammer"] = pdf_jammer_data.Number + "  " + pdf_jammer_data.Jammer
+    pdf_jammer_data = pdf_jammer_data[[
+        "Jammer", "Jams", "Points", "Lead", "% Lead", "Lost"
+    ]]
+    pdf_jammer_data = pdf_jammer_data.sort_values("Jammer")
+
+    return pdf_jammer_data
+
+
+
+def get_bothteams_skaterpenalties_html(derby_game: DerbyGame,
+                                       anonymize_names: bool = False) -> str:
+    """Get a html table of both teams' penalties
+
+    Args:
+        derby_game (DerbyGame): a derby game
+
+    Returns:
+        str: html table
+    """
+    pdf_team1_skaterpenalties = build_oneteam_skaterpenaltycounts_pdf(
+        derby_game, derby_game.team_1_name, anonymize_names=anonymize_names)
+    pdf_team2_skaterpenalties = build_oneteam_skaterpenaltycounts_pdf(
+        derby_game, derby_game.team_2_name, anonymize_names=anonymize_names)
+
+    # apply formatting. Change text color of each row based on penalty count
+    table_htmls = []
+    for pdf in [pdf_team1_skaterpenalties, pdf_team2_skaterpenalties]:
+        styler = pdf.style.set_properties(**{'color': 'green'})
+        red_rows = np.where(pdf['Count'] > 6, 'color: red', '')
+        styler = styler.apply(lambda _: red_rows)
+        orange_rows = np.where(pdf['Count'] == 6, 'color: orange', '')
+        styler = styler.apply(lambda _: orange_rows)
+        yellow_rows = np.where(pdf['Count'] == 5, 'color: yellow', '')
+        styler = styler.apply(lambda _: yellow_rows)
+        # gray background
+        styler = styler.set_properties(**{'background-color': '#999999'})
+        styler = styler.set_table_attributes("style='display:inline'").hide_index()
+        table_htmls.append(styler.render())
+
+    table_html_1, table_html_2 = table_htmls
+
+    n_team1_penalties = sum(pdf_team1_skaterpenalties.Count)
+    n_team2_penalties = sum(pdf_team2_skaterpenalties.Count)
+    team1_tablecell_html = f"<H2>{derby_game.team_1_name} ({n_team1_penalties})</H2>" + table_html_1
+    team2_tablecell_html = f"<H2>{derby_game.team_2_name} ({n_team2_penalties})</H2>" + table_html_2
+    return "<table><tr valign='top'><td>" + team1_tablecell_html + "</td><td>" + team2_tablecell_html + "</td></tr></table>"
+
+
+def build_oneteam_skaterpenaltycounts_pdf(derby_game: DerbyGame, team_name: str,
+                                          anonymize_names: bool=False) -> pd.DataFrame:
+    """Build a dataframe of skater penalties for one team
+
+    Args:
+        derby_game (DerbyGame): Derby game
+        team_name (str): Team name
+        anonymize_names (bool, optional): Anonymize names?. Defaults to False.
+
+    Returns:
+        pd.DataFrame: Table with skater penalties, one row per skater
+    """
+    
+    pdf_team_penalties = derby_game.pdf_penalties[
+        derby_game.pdf_penalties.team == team_name].copy()
+    pdf_team_penalties = pdf_team_penalties.rename(columns={
+        "Name": "Skater"
+    })
+
+    if anonymize_names:
+        logger.debug("Anonymizing skater names.")
+        name_dict = build_anonymizer_map(set(pdf_team_penalties.Skater))
+        pdf_team_penalties["Skater"] = [name_dict[skater]
+                                        for skater in pdf_team_penalties.Skater]   
+
+    pdf_penalties_long = (
+        pdf_team_penalties.groupby(['RosterNumber', 'Skater',]).size().reset_index())
+    pdf_penalties_long = pdf_penalties_long.rename(columns={
+        0: "Count"
+    })
+    pdf_penalties_long = pdf_penalties_long.sort_values("Count", ascending=False)
+    pdf_penalties_long = pdf_penalties_long.rename(columns={"RosterNumber": "Number"})
+
+    return pdf_penalties_long
+
+
 def plot_jammer_stats_team1(derby_game: DerbyGame,
                             anonymize_names: bool = False) -> Figure:
     return plot_jammer_stats(derby_game, 1, anonymize_names=anonymize_names)
 
 
 def plot_jammer_stats_team2(derby_game: DerbyGame,
                             anonymize_names: bool = False) -> Figure:
```

### Comparing `jamstats-1.2.1.2/src/jamstats/util/resources.py` & `jamstats-1.3.0/src/jamstats/util/resources.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.2/src/jamstats/web/statserver.py` & `jamstats-1.3.0/src/jamstats/web/statserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,23 +20,24 @@
         plot_jam_lead_and_scores_period1,    
         plot_jam_lead_and_scores_period2,
         plot_jammers_by_team,
         plot_lead_summary,
         plot_team_penalty_counts,
         get_recent_penalties_html,
         get_bothteams_roster_html,
-        get_current_skaters_html,
         get_officials_roster_html,
         get_caller_dashboard_html
 )
 from jamstats.plots.skaterplots import (
     plot_jammer_stats_team1,
     plot_jammer_stats_team2,
     plot_skater_stats_team1,
     plot_skater_stats_team2,
+    get_bothteams_skaterpenalties_html,
+    get_bothteams_jammertable_html
 )
 import matplotlib
 from datetime import datetime
 import io
 import logging
 import socket
 import sys, os
@@ -68,14 +69,16 @@
 
 PLOT_SECTION_NAME_FUNC_MAP = {
     "Tables": {
         "Caller Dashboard": get_caller_dashboard_html,
 #        "Current Skaters": get_current_skaters_html,
         "Teams Summary": get_game_teams_summary_html,
         "Recent Penalties": get_recent_penalties_html,
+        "All Penalties": get_bothteams_skaterpenalties_html,
+        "Jammers": get_bothteams_jammertable_html,
         "Team Rosters": get_bothteams_roster_html,
         "Officials Roster": get_officials_roster_html,
     },
     "Basic Plots": {
         "Score by Jam": plot_cumulative_score_by_jam,
         "Team Penalty Counts": plot_team_penalty_counts,
         "Team 1 Jammers": plot_jammer_stats_team1,
```

### Comparing `jamstats-1.2.1.2/src/jamstats.egg-info/SOURCES.txt` & `jamstats-1.3.0/src/jamstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

