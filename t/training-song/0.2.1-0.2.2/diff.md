# Comparing `tmp/training_song-0.2.1.tar.gz` & `tmp/training_song-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "training_song-0.2.1.tar", max compression
+gzip compressed data, was "training_song-0.2.2.tar", max compression
```

## Comparing `training_song-0.2.1.tar` & `training_song-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     2967 2023-06-13 12:38:37.124326 training_song-0.2.1/README.md
--rw-r--r--   0        0        0     1066 2023-06-13 12:38:37.128326 training_song-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/__init__.py
--rw-r--r--   0        0        0     5465 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/core.py
--rw-r--r--   0        0        0        8 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/.gitignore
--rw-r--r--   0        0        0        0 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/__init__.py
--rw-r--r--   0        0        0     3521 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/api.py
--rw-r--r--   0        0        0     2553 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/billboard_io.py
--rw-r--r--   0        0        0     2646 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/db.py
--rw-r--r--   0        0        0     4004 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/spotify.py
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 training_song-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2962 2023-06-19 11:29:02.616499 training_song-0.2.2/README.md
+-rw-r--r--   0        0        0     1091 2023-06-19 11:29:02.616499 training_song-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      254 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/__init__.py
+-rw-r--r--   0        0        0     5465 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/core.py
+-rw-r--r--   0        0        0      522 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/db_utils.py
+-rw-r--r--   0        0        0        8 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/__init__.py
+-rw-r--r--   0        0        0     3631 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/api.py
+-rw-r--r--   0        0        0     2355 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/billboard_io.py
+-rw-r--r--   0        0        0     3168 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/db.py
+-rw-r--r--   0        0        0     1215 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/hard_coded.py
+-rw-r--r--   0        0        0     3717 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/server/spotify.py
+-rw-r--r--   0        0        0      739 2023-06-19 11:29:02.616499 training_song-0.2.2/trainingsong/ts_utils.py
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 training_song-0.2.2/PKG-INFO
```

### Comparing `training_song-0.2.1/README.md` & `training_song-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Take your metrics from [A Hard Day's Night](https://open.spotify.com/track/5J2CHimS7dWYMImCHkEFaJ?si=a0e9062fc8674757) (64%) to [Mo Money Mo Problems](https://open.spotify.com/track/4INDiWSKvqSKDEu7mh8HFz?si=81e7a21927d741c7) (97%).
 
 ## How to use
 
 Once you've trained your model, simply wrap your metric in ts(..) as follows:
 
 ```python
-from trainingsong.core import ts
+from trainingsong import ts
 
 model.fit(X_train, y_train)
 y_pred = model.predict(X_test)
 
 accuracy = ts(accuracy_score(y_test, y_pred))
 
 >> Congrats your model got an accuracy of 92 percent!
```

### Comparing `training_song-0.2.1/pyproject.toml` & `training_song-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "training-song"
-version = "0.2.1"
+version = "0.2.2"
 description = "Audio Motivation for Data Scientists and ML Engineers"
 authors = ["koayon <koayon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "trainingsong"}]
 
 [project]
@@ -35,12 +35,13 @@
 asyncpg = "^0.27.0"
 psycopg2-binary = "^2.9.3"
 responses = "^0.13.4"
 httpx = "^0.23.0"
 starlette = "^0.27.0"
 httpcore = "^0.15"
 pytest-asyncio = "^0.15.1"
+cryptography = "^38.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pylint = "^2.17.4"
```

### Comparing `training_song-0.2.1/trainingsong/core.py` & `training_song-0.2.2/trainingsong/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 """Entry point"""
 
-from typing import Union, List, Optional, Tuple, Dict, Any, NamedTuple
-import webbrowser
-from threading import Thread
-import time
 import json
 import os
 import re
+import time
+import webbrowser
+from threading import Thread
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import requests
 import uvicorn
 from fastapi import FastAPI, Request
 
-PROD_API = True
-
-OAUTH_CODE = None
-if PROD_API:
-    URL = "https://training-song-api.vercel.app"
-else:
-    URL = "https://training-song-api-koayon.vercel.app"
-
-AUTH_URL = "https://accounts.spotify.com/authorize?client_id=4259770654fb4353813dbf19d8b20608&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%3A8000%2Flocal_callback&scope=user-modify-playback-state+user-read-currently-playing+user-read-recently-played+user-read-playback-state"
-LOCAL_REDIRECT_URI = "http://localhost:8000/local_callback"
+from trainingsong.ts_utils import AUTH_URL, OAUTH_CODE, URL
 
 
 def _training_song(
     p: float,
     chart: Optional[str] = "hot-100",
     autoplay: Optional[bool] = True,
     verbose: Optional[bool] = True,
     email: Optional[str] = None,
+    metric: Optional[str] = "accuracy",
 ) -> Tuple[Union[float, List[float], None], Dict[str, Any]]:
     """Return the training song for a given percentage
     Outputs: (acc, response)"""
 
     params = {
         "p": p,
         "autoplay": autoplay,
@@ -47,15 +39,15 @@
         params=params,
         timeout=15,
     )
 
     response = raw_response.json()
 
     if verbose:
-        print("Congrats your model got an accuracy of", p, "percent!")
+        print(f"Congrats your model's {metric} was ", p, "%!")
         if response and "song_info" in response:
             print(response["song_info"])
         else:
             print("No song info found")
     if "errors" in response:
         print(response["errors"])
 
@@ -63,17 +55,18 @@
         webbrowser.open(response["spotify_link"])
 
     return p, response
 
 
 def ts(
     input_percentage: Union[float, List[float]],
-    chart="hot-100",
-    autoplay=True,
-    verbose=True,
+    chart: str = "hot-100",
+    autoplay: bool = True,
+    verbose: bool = True,
+    metric: str = "accuracy",
 ) -> Tuple[Union[float, List[float], None], Dict[str, Any]]:
     """Training song function.
     Starts a local server to capture the auth code from spotify and returns the song for your training accuracy.
 
     Args:
     input_percentage (float): The accuracy of your model.
     chart (str): The chart to use. Defaults to "hot-100".
@@ -99,32 +92,44 @@
 
     if not email_in_db:
         # start the local server in a new thread
         if not OAUTH_CODE:
             server_thread = Thread(target=_start_local_server)
             server_thread.start()
 
-            # open the authorization URL in a browser
             webbrowser.open(AUTH_URL)
 
             # wait for the user to authorize and for the server to capture the OAuth code
             while not OAUTH_CODE:
-                time.sleep(1)
+                time.sleep(0.5)
 
     # if the input percentage is a list, we want to take the final value
     accuracy = (
         input_percentage
         if isinstance(input_percentage, (float, int))
         else input_percentage[-1]
     )
 
-    # now we can call the training_song function with the captured OAuth code
     acc, response = _training_song(
-        accuracy, chart=chart, autoplay=autoplay, verbose=verbose, email=email
+        accuracy,
+        chart=chart,
+        autoplay=autoplay,
+        verbose=verbose,
+        email=email,
+        metric=metric,
     )
+    if not email_in_db:
+        print(
+            """
+
+Thanks for using Training Song!
+For your first time, we used a local server to listen for your Spotify authorisation code.
+You can exit this process now.
+For future uses an access token is stored securely."""
+        )
     return acc, response
 
 
 local_app = FastAPI()
 
 
 @local_app.get("/local_callback")
@@ -165,17 +170,21 @@
         try:
             email_dict = json.load(f)
         except json.decoder.JSONDecodeError:
             email_dict = {"email": None}
     return email_dict["email"]
 
 
-def _check_email(email):
+def _check_email(email: str) -> str:
+    "Returns truthy string if email is in db"
     response = requests.get(URL + "/email_in_db", params={"email": email})
-    return response.json()["present_in_db"]
+    if response and (response.status_code == 200):
+        return response.json()["present_in_db"]
+    else:
+        raise ValueError("Error checking email")
 
 
 if __name__ == "__main__":
     INPUT_PERCENTAGE = None
     RAW_INPUT = ""
     while not INPUT_PERCENTAGE:
         RAW_INPUT = input("How well did your model do? (Enter a percentage): ")
```

### Comparing `training_song-0.2.1/trainingsong/server/api.py` & `training_song-0.2.2/trainingsong/server/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Main API file.
 """
 
-from typing import Union, Dict
-import webbrowser
+from typing import Dict, Union
 
 from fastapi import FastAPI, HTTPException, Query
 
 from trainingsong.server.billboard_io import get_billboard_data
+from trainingsong.server.db import database_session, get_tokens
+from trainingsong.server.hard_coded import hard_coded_song
 from trainingsong.server.spotify import (
     create_spotify_client,
     spotify_link,
     start_playback,
 )
-from trainingsong.server.db import get_tokens, database_session
 
 app = FastAPI()
 
 
 @app.get("/")
 async def root(
     email: str,
@@ -29,19 +29,28 @@
     """The main API endpoint. It takes in a percentage p, interacts with the billboard api and then redirects to the callback for the Spotify API."""
 
     print("Hit root endpoint")
     print(f"p: {p}")
     print(f"chart: {chart}")
     print(f"autoplay: {autoplay}")
 
-    try:
-        song_results = get_billboard_data(p, chart)
-        song_results.autoplay = autoplay
-    except HTTPException as e:
-        raise HTTPException(status_code=404, detail=str(e)) from e
+    if p < 1:
+        # Turn a decimal into a percentage
+        p *= 100
+
+    if p < 52:
+        song_results = hard_coded_song(p, chart)
+        song_results.chart = chart
+    else:
+        try:
+            song_results = get_billboard_data(p, chart)
+        except HTTPException as e:
+            raise HTTPException(status_code=404, detail=str(e)) from e
+
+    song_results.autoplay = autoplay
 
     if not spotify_client_code and not email:
         raise HTTPException(status_code=400, detail="Missing Spotify code and email")
 
     print("Got spotify code")
 
     song_info = song_results.song_info
@@ -50,31 +59,28 @@
     try:
         if spotify_client_code is None and email is None:
             raise HTTPException(
                 status_code=400, detail="Missing Spotify code and email"
             )
         sp = await create_spotify_client(spotify_client_code, email)
     except HTTPException as e:
-        # raise HTTPException(
-        #     status_code=404, detail=f"str(e). Failed to created Spotify client"
-        # ) from e
         return {"errors": f"str(e). Failed to created Spotify client"}
 
     link, _name, uri = spotify_link(
         sp, song_results.song_name, song_results.artist_name
     )
 
     print(link)
 
     open_link = ""
 
     if autoplay:
         errors = attempt_play(sp, uri)
         if errors:
-            errors += "Failed to start playback"
+            errors += " Failed to start playback"
             open_link = "True"
     else:
         errors = ""
         open_link = "True"
 
     print(f"errors: {errors}")
     print(f"open_link: {open_link}")
@@ -96,18 +102,18 @@
 
 @app.get("/hello")
 async def hello():
     return {"hello": "world"}
 
 
 @app.get("/email_in_db")
-async def email_in_db(email: str) -> Dict[str, bool]:
-    async with database_session() as session:
-        result = await get_tokens(email)
-    return {"present_in_db": result is not None}
+async def email_in_db(email: str) -> Dict[str, str]:
+    with database_session() as session:
+        result = get_tokens(email)
+    return {"present_in_db": ("" if result is None else "True")}
 
 
 def attempt_play(sp, uri) -> str:
     "Attempt to play the song on Spotify"
     errors = ""
     devices = sp.devices()
     active_devices = devices["devices"] if devices else None
```

### Comparing `training_song-0.2.1/trainingsong/server/billboard_io.py` & `training_song-0.2.2/trainingsong/server/billboard_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 "Billboard API calls and data processing"
 
 import datetime
-from typing import Tuple
 from dataclasses import dataclass
+from typing import Tuple
 
-from fastapi import HTTPException
 import billboard
+from fastapi import HTTPException
 
 from trainingsong.server.spotify import StateData
 
 
 @dataclass
 class Song:
     """A dataclass to store the song name, artist name and number of weeks on the chart"""
@@ -22,17 +22,14 @@
 def get_billboard_data(
     percentage: float,
     chart: str = "hot-100",
 ) -> StateData:
     """Call Billboard API and get the song name, artist name and song info"""
     if percentage > 100 or percentage < 0:
         raise ValueError("Please enter a percentage between 0 and 100")
-    if percentage < 1:
-        # Turn a decimal into a percentage
-        percentage *= 100
 
     try:
         number_one_song, target_date = get_number_one_song(percentage, chart)
     except HTTPException:
         raise HTTPException(status_code=404, detail="No chart data found")
 
     song_name = number_one_song.title
@@ -66,17 +63,15 @@
     )
     target_day = int(days_in_year * fractional_percentage)
 
     target_date = datetime.date(1900 + target_year, 1, 1) + datetime.timedelta(
         days=target_day
     )
 
-    # Fetch the Billboard Hot 100 chart data for the target date
     chart_output = billboard.ChartData(chart, date=target_date)
 
-    # Get the Number 1 song on the chart
     if chart_output:
         number_one_song = chart_output[0]
     else:
         raise HTTPException(status_code=404, detail="No chart data found")
 
     return number_one_song, target_date
```

### Comparing `training_song-0.2.1/trainingsong/server/db.py` & `training_song-0.2.2/trainingsong/server/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,114 @@
 """Database module for storing and retrieving user tokens from database."""
+import os
+from contextlib import contextmanager
+from functools import lru_cache
 
-import databases
 import sqlalchemy
-from sqlalchemy import Table, Column, String, text, Integer
-import os
 from dotenv import load_dotenv
-from typing import Optional, Dict
-import asyncio
-from contextlib import asynccontextmanager
+from sqlalchemy import BigInteger, Column, String, Table, create_engine
+from sqlalchemy.orm import sessionmaker
+
+from trainingsong.db_utils import decrypt, encrypt
 
 # If running locally, load environment variables from .env
 if os.environ.get("VERCEL") != "1":
     load_dotenv()
 
 DATABASE_URL = os.environ.get("DATABASE_URL")
 if DATABASE_URL is None:
-    raise ValueError("DATABASE_URL environment variable not set or empty")
+    # raise ValueError("DATABASE_URL environment variable not set or empty")
+    DATABASE_URL = "sqlite:///test.db"
 
-database = databases.Database(DATABASE_URL)
-metadata = sqlalchemy.MetaData()
+engine = create_engine(DATABASE_URL, future=True)
+Session = sessionmaker(bind=engine)
 
+metadata = sqlalchemy.MetaData()
 tokens = Table(
     "tokens",
     metadata,
     Column("email", String, primary_key=True, unique=True),
     Column("access_token", String),
     Column("refresh_token", String),
-    Column("expires_at", Integer),
+    Column("expires_at", BigInteger),
 )
 
-engine = sqlalchemy.create_engine(DATABASE_URL)
-
 
-def create() -> None:
-    with engine.begin() as connection:
-        connection.execute(text("DROP TABLE IF EXISTS tokens"))
-    metadata.create_all(engine)
+def store_tokens(email, access_token, refresh_token, expires_at):
+    with engine.connect() as connection:
+        query = tokens.insert().values(
+            email=email,
+            access_token=encrypt(access_token),
+            refresh_token=encrypt(refresh_token),
+            expires_at=expires_at,
+        )
+        connection.execute(query)
+        connection.commit()
 
 
-async def store_tokens(
-    email: str, access_token: str, refresh_token: str, expires_at: int
-) -> None:
-    query = tokens.insert().values(
-        email=email,
-        access_token=access_token,
-        refresh_token=refresh_token,
-        expires_at=expires_at,
-    )
-    await database.execute(query)
-
-
-async def get_tokens(email: str):
-    # Return type is dictionary like. It's a Record object from databases
-    query = tokens.select().where(tokens.c.email == email)
-    result = await database.fetch_one(query)
-    return result
-
-
-async def delete_tokens(email: str) -> None:
-    query = tokens.delete().where(tokens.c.email == email)
-    await database.execute(query)
-
-
-async def update_tokens(
-    email: str, access_token: str, refresh_token: str, expires_at: str
-) -> None:
-    query = (
-        tokens.update()
-        .where(tokens.c.email == email)
-        .values(
-            access_token=access_token,
-            refresh_token=refresh_token,
-            expires_at=expires_at,
+# @lru_cache(maxsize=1)
+def get_tokens(email):
+    with engine.connect() as connection:
+        query = tokens.select().where(tokens.c.email == email)
+        result = connection.execute(query).fetchone()
+        if result:
+            result = dict(result)
+            result["access_token"] = decrypt(result["access_token"])
+            result["refresh_token"] = decrypt(result["refresh_token"])
+        return result
+
+
+def update_tokens(email, access_token, refresh_token, expires_at):
+    with engine.connect() as connection:
+        query = (
+            tokens.update()
+            .where(tokens.c.email == email)
+            .values(
+                access_token=encrypt(access_token),
+                refresh_token=encrypt(refresh_token),
+                expires_at=expires_at,
+            )
         )
-    )
-    await database.execute(query)
+        execute = connection.execute(query)
+        connection.commit()
+
+
+def delete_tokens(email):
+    with engine.connect() as connection:
+        query = tokens.delete().where(tokens.c.email == email)
+        connection.execute(query)
+        connection.commit()
+
+
+def create():
+    check = input("Are you sure you want to drop the database? (y/n) ")
+    if check != "y":
+        return print("Aborting")
+
+    with engine.connect() as connection:
+        connection.execute(sqlalchemy.text("DROP TABLE IF EXISTS tokens"))
+    metadata.create_all(engine)
+    print("Created fresh database")
 
 
-@asynccontextmanager
-async def database_session():
-    await database.connect()
+@contextmanager
+def database_session():
+    session = Session()
+    full_db = None
     try:
-        yield
+        yield session
+        session.commit()
+        full_db = session.query(tokens).limit(5).all()
+    except:
+        session.rollback()
+        raise
     finally:
-        await database.disconnect()
+        session.close()
+        # print(full_db)
 
 
-async def main():
-    async with database_session():
-        # Test store_tokens and get_tokens
-        # create()
-
-        # await store_tokens("test", "test", "test", 1689727126)
-        # record = await get_tokens("test")
-        # if record:
-        #     print(record)
-        #     print(record.email)
-        pass
+def main():
+    pass
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    main()
```

### Comparing `training_song-0.2.1/trainingsong/server/spotify.py` & `training_song-0.2.2/trainingsong/server/spotify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Spotify API functions"""
 
-from urllib.error import HTTPError
-from typing import Tuple, Union, Optional
-from dataclasses import dataclass
 import os
-import json
 import time
+from dataclasses import dataclass
+from typing import Optional, Tuple, Union
+from urllib.error import HTTPError
 
 import spotipy
+from dotenv import load_dotenv
+from fastapi import HTTPException
 from spotipy import SpotifyException
 from spotipy.oauth2 import SpotifyOAuth
-from fastapi import HTTPException
+
 from trainingsong.server.db import (
-    store_tokens,
+    database_session,
     get_tokens,
+    store_tokens,
     update_tokens,
-    database_session,
 )
-from dotenv import load_dotenv
 
 SCOPE = "user-modify-playback-state user-read-currently-playing user-read-recently-played user-read-playback-state"
 
 # If running locally, load environment variables from .env
 if os.environ.get("VERCEL") != "1":
     load_dotenv()
 
@@ -51,58 +51,53 @@
     sp_oauth = SpotifyOAuth(
         client_id=CLIENT_ID,
         client_secret=CLIENT_SECRET,
         redirect_uri=SPOTIFY_REDIRECT_URI,
         scope=SCOPE,
     )
 
-    async with database_session() as session:
-        token_info = await get_tokens(email)
+    with database_session() as session:
+        token_info = get_tokens(email)
 
         if not token_info:
             print("Getting access token...")
-            # Get the access token
             if code is None:
                 raise ValueError("No code provided")
             try:
                 token_info = sp_oauth.get_access_token(code)
             except:
                 raise HTTPException(status_code=400, detail="Invalid Spotify code")
             if not token_info:
                 raise HTTPException(status_code=400, detail="Invalid Spotify code")
 
-            # Put token info into sqlalchemy database
-            await store_tokens(
+            store_tokens(
                 email,
                 token_info["access_token"],
                 token_info["refresh_token"],
                 token_info["expires_at"],
             )
 
-        # If the access token is expired, refresh it
         if token_info["expires_at"] < time.time():
             print("Refreshing access token...")
             token_info = sp_oauth.refresh_access_token(token_info["refresh_token"])
 
             if token_info:
-                # Put token info into sqlalchemy database
-                await update_tokens(
+                update_tokens(
                     email,
                     token_info["access_token"],
                     token_info["refresh_token"],
                     token_info["expires_at"],
                 )
             else:
                 raise ValueError("Failed to refresh access token. Please try again. ")
 
     access_token = token_info["access_token"] if token_info else None
 
     print("Got access token!")
 
-    # Create a Spotify client with the access token
     sp = spotipy.Spotify(auth=access_token)
     print("Created Spotify client")
 
     return sp
 
 
 def spotify_link(
```

### Comparing `training_song-0.2.1/PKG-INFO` & `training_song-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: training-song
-Version: 0.2.1
+Version: 0.2.2
 Summary: Audio Motivation for Data Scientists and ML Engineers
 License: MIT
 Author: koayon
 Author-email: koayon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: billboard-py (>=7.0.0,<8.0.0)
+Requires-Dist: cryptography (>=38.0.0,<39.0.0)
 Requires-Dist: databases (>=0.5.2,<0.6.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: httpcore (>=0.15,<0.16)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: lyricsgenius (>=3.0.1,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: pytest-asyncio (>=0.15.1,<0.16.0)
@@ -46,15 +47,15 @@
 Take your metrics from [A Hard Day's Night](https://open.spotify.com/track/5J2CHimS7dWYMImCHkEFaJ?si=a0e9062fc8674757) (64%) to [Mo Money Mo Problems](https://open.spotify.com/track/4INDiWSKvqSKDEu7mh8HFz?si=81e7a21927d741c7) (97%).
 
 ## How to use
 
 Once you've trained your model, simply wrap your metric in ts(..) as follows:
 
 ```python
-from trainingsong.core import ts
+from trainingsong import ts
 
 model.fit(X_train, y_train)
 y_pred = model.predict(X_test)
 
 accuracy = ts(accuracy_score(y_test, y_pred))
 
 >> Congrats your model got an accuracy of 92 percent!
```

