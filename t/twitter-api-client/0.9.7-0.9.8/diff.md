# Comparing `tmp/twitter-api-client-0.9.7.tar.gz` & `tmp/twitter-api-client-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.7.tar", last modified: Sun Jun 18 18:59:42 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.8.tar", last modified: Mon Jun 19 16:50:21 2023, max compression
```

## Comparing `twitter-api-client-0.9.7.tar` & `twitter-api-client-0.9.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-18 18:59:42.179033 twitter-api-client-0.9.7/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    11750 2023-06-18 18:59:42.179033 twitter-api-client-0.9.7/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-18 18:59:42.179033 twitter-api-client-0.9.7/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    13719 2023-06-18 18:58:01.000000 twitter-api-client-0.9.7/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-18 18:59:42.175700 twitter-api-client-0.9.7/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    28656 2023-06-18 18:48:03.000000 twitter-api-client-0.9.7/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    30178 2023-06-18 18:29:35.000000 twitter-api-client-0.9.7/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-18 18:59:42.175700 twitter-api-client-0.9.7/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    11750 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    12136 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    14177 2023-06-19 16:48:37.000000 twitter-api-client-0.9.8/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    31300 2023-06-19 16:46:01.000000 twitter-api-client-0.9.8/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    30178 2023-06-18 18:29:35.000000 twitter-api-client-0.9.8/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)    10178 2023-06-19 15:54:08.000000 twitter-api-client-0.9.8/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    12136 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.7/LICENSE` & `twitter-api-client-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.7/PKG-INFO` & `twitter-api-client-0.9.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.7
+Version: 0.9.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -145,14 +145,32 @@
 
 # delete entire conversation
 account.dm_delete(conversation_id='123456-789012')
 
 # delete (hide) specific DM
 account.dm_delete(message_id='123456')
 
+# get all scheduled tweets
+scheduled_tweets = account.scheduled_tweets()
+
+# delete a scheduled tweet
+account.delete_scheduled_tweet(12345678)
+
+# get all draft tweets
+draft_tweets = account.draft_tweets()
+
+# delete a draft tweet
+account.delete_draft_tweet(12345678)
+
+# delete all scheduled tweets
+account.clear_scheduled_tweets()
+
+# delete all draft tweets
+account.clear_draft_tweets()
+
 # example configuration
 account.update_settings({
     "address_book_live_sync_enabled": False,
     "allow_ads_personalization": False,
     "allow_authenticated_periscope_requests": True,
     "allow_dm_groups_from": "following",
     "allow_dms_from": "following",
```

### Comparing `twitter-api-client-0.9.7/setup.py` & `twitter-api-client-0.9.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.7",
+    version="0.9.8",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
     
@@ -152,14 +152,32 @@
     
     # delete entire conversation
     account.dm_delete(conversation_id='123456-789012')
     
     # delete (hide) specific DM
     account.dm_delete(message_id='123456')
     
+    # get all scheduled tweets
+    scheduled_tweets = account.scheduled_tweets()
+    
+    # delete a scheduled tweet
+    account.delete_scheduled_tweet(12345678)
+    
+    # get all draft tweets
+    draft_tweets = account.draft_tweets()
+    
+    # delete a draft tweet
+    account.delete_draft_tweet(12345678)
+    
+    # delete all scheduled tweets
+    account.clear_scheduled_tweets()
+    
+    # delete all draft tweets
+    account.clear_draft_tweets()
+    
     # example configuration
     account.update_settings({
         "address_book_live_sync_enabled": False,
         "allow_ads_personalization": False,
         "allow_authenticated_periscope_requests": True,
         "allow_dm_groups_from": "following",
         "allow_dms_from": "following",
```

### Comparing `twitter-api-client-0.9.7/twitter/account.py` & `twitter-api-client-0.9.8/twitter/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,29 +113,62 @@
             'dark_request': False,
             'media': {
                 'media_entities': [],
                 'possibly_sensitive': False,
             },
             'semantic_annotation_ids': [],
         }
+
+        if reply_params := kwargs.get('reply_params', {}):
+            variables |= reply_params
+        if quote_params := kwargs.get('quote_params', {}):
+            variables |= quote_params
+        if poll_params := kwargs.get('poll_params', {}):
+            variables |= poll_params
+
+        draft = kwargs.get('draft')
+        schedule = kwargs.get('schedule')
+
+        if draft or schedule:
+            variables = {
+                'post_tweet_request': {
+                    'auto_populate_reply_metadata': False,
+                    'status': text,
+                    'exclude_reply_user_ids': [],
+                    'media_ids': [],
+                },
+            }
+            if media:
+                for m in media:
+                    media_id = self._upload_media(m['media'])
+                    variables['post_tweet_request']['media_ids'].append(media_id)
+                    if alt := m.get('alt'):
+                        self._add_alt_text(media_id, alt)
+
+            if schedule:
+                variables['execute_at'] = (
+                    datetime.strptime(schedule, "%Y-%m-%d %H:%M").timestamp()
+                    if isinstance(schedule, str)
+                    else schedule
+                )
+                return self.gql('POST', Operation.CreateScheduledTweet, variables)
+
+            return self.gql('POST', Operation.CreateDraftTweet, variables)
+
+        # regular tweet
         if media:
             for m in media:
                 media_id = self._upload_media(m['media'])
                 variables['media']['media_entities'].append({
                     'media_id': media_id,
                     'tagged_users': m.get('tagged_users', [])
                 })
                 if alt := m.get('alt'):
                     self._add_alt_text(media_id, alt)
-        if reply_params := kwargs.get('reply_params', {}):
-            variables |= reply_params
-        if quote_params := kwargs.get('quote_params', {}):
-            variables |= quote_params
-        if poll_params := kwargs.get('poll_params', {}):
-            variables |= poll_params
+
         return self.gql('POST', Operation.CreateTweet, variables)
 
     def schedule_tweet(self, text: str, date: int | str, *, media: list = None) -> dict:
         variables = {
             'post_tweet_request': {
                 'auto_populate_reply_metadata': False,
                 'status': text,
@@ -681,15 +714,15 @@
             results['conversation'] = self.session.post(
                 f'{self.v1_api}/dm/conversation/{conversation_id}/delete.json',
             ).text  # not json response
         if message_id:
             # delete single message
             _id, op = Operation.DMMessageDeleteMutation
             results['message'] = self.session.post(
-                f'https://twitter.com/i/api/graphql/{_id}/{op}',
+                f'{self.gql_api}/{_id}/{op}',
                 json={'queryId': _id, 'variables': {'messageId': message_id}},
             ).json()
         return results
 
     def dm_search(self, query: str) -> dict:
         """
         Search DMs by keyword
@@ -699,15 +732,15 @@
         """
 
         def get(cursor=None):
             if cursor:
                 params['variables']['cursor'] = cursor.pop()
             _id, op = Operation.DmAllSearchSlice
             r = self.session.get(
-                f'https://twitter.com/i/api/graphql/{_id}/{op}',
+                f'{self.gql_api}/{_id}/{op}',
                 params=build_params(params),
             )
             res = r.json()
             cursor = find_key(res, 'next_cursor')
             return res, cursor
 
         self.session.headers.update(headers=get_headers(self.session))
@@ -717,7 +750,38 @@
         params = {'variables': variables, 'features': Operation.default_features}
         res, cursor = get()
         data = [res]
         while cursor:
             res, cursor = get(cursor)
             data.append(res)
         return {'query': query, 'data': data}
+
+    def scheduled_tweets(self, ascending: bool = True) -> dict:
+        variables = {"ascending": ascending}
+        return self.gql('GET', Operation.FetchScheduledTweets, variables)
+
+    def delete_scheduled_tweet(self, tweet_id: int) -> dict:
+        """duplicate, same as `unschedule_tweet()`"""
+        variables = {'scheduled_tweet_id': tweet_id}
+        return self.gql('POST', Operation.DeleteScheduledTweet, variables)
+
+    def clear_scheduled_tweets(self) -> None:
+        user_id = int(re.findall('"u=(\d+)"', self.session.cookies.get('twid'))[0])
+        drafts = self.gql('GET', Operation.FetchScheduledTweets, {"ascending": True})
+        for _id in set(find_key(drafts, 'rest_id')):
+            if _id != user_id:
+                self.gql('POST', Operation.DeleteScheduledTweet, {'scheduled_tweet_id': _id})
+
+    def draft_tweets(self, ascending: bool = True) -> dict:
+        variables = {"ascending": ascending}
+        return self.gql('GET', Operation.FetchDraftTweets, variables)
+
+    def delete_draft_tweet(self, tweet_id: int) -> dict:
+        variables = {'draft_tweet_id': tweet_id}
+        return self.gql('POST', Operation.DeleteDraftTweet, variables)
+
+    def clear_draft_tweets(self) -> None:
+        user_id = int(re.findall('"u=(\d+)"', self.session.cookies.get('twid'))[0])
+        drafts = self.gql('GET', Operation.FetchDraftTweets, {"ascending": True})
+        for _id in set(find_key(drafts, 'rest_id')):
+            if _id != user_id:
+                self.gql('POST', Operation.DeleteDraftTweet, {'draft_tweet_id': _id})
```

### Comparing `twitter-api-client-0.9.7/twitter/constants.py` & `twitter-api-client-0.9.8/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.7/twitter/login.py` & `twitter-api-client-0.9.8/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.7/twitter/scraper.py` & `twitter-api-client-0.9.8/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.7/twitter/search.py` & `twitter-api-client-0.9.8/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.7/twitter/util.py` & `twitter-api-client-0.9.8/twitter/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,22 +104,24 @@
                 return content['value']  # v1 cursor
 
 
 def get_headers(session, **kwargs) -> dict:
     """
     Get the headers required for authenticated requests
     """
+    cookies = session.cookies
+    cookies.delete('ct0', domain='.twitter.com')
     headers = kwargs | {
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-        'cookie': '; '.join(f'{k}={v}' for k, v in session.cookies.items()),
+        'cookie': '; '.join(f'{k}={v}' for k, v in cookies.items()),
         'referer': 'https://twitter.com/',
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
-        'x-csrf-token': session.cookies.get('ct0', ''),
-        'x-guest-token': session.cookies.get('guest_token', ''),
-        'x-twitter-auth-type': 'OAuth2Session' if session.cookies.get('auth_token') else '',
+        'x-csrf-token': cookies.get('ct0', ''),
+        'x-guest-token': cookies.get('guest_token', ''),
+        'x-twitter-auth-type': 'OAuth2Session' if cookies.get('auth_token') else '',
         'x-twitter-active-user': 'yes',
         'x-twitter-client-language': 'en',
     }
     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
 
 
 def find_key(obj: any, key: str) -> list:
@@ -205,14 +207,22 @@
     return f'[{color}{status}{RESET}]'
 
 
 def get_ids(data: list | dict, operation: tuple) -> set:
     expr = ID_MAP[operation[-1]]
     return {k for k in find_key(data, 'entryId') if re.search(expr, k)}
 
+
+def dump(path: str, **kwargs):
+    fname, data = list(kwargs.items())[0]
+    out = Path(path)
+    out.mkdir(exist_ok=True, parents=True)
+    (out / f'{fname}_{time.time_ns()}.json').write_bytes(
+        orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS))
+
 # def init_protonmail_session(email: str, password: str) -> protonmail.api.Session:
 #     """
 #     Create an authenticated Proton Mail session
 #
 #     @param email: your email. Can also use username
 #     @param password: your password
 #     @return: Proton Mail Session object
```

### Comparing `twitter-api-client-0.9.7/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.8/twitter_api_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.7
+Version: 0.9.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -145,14 +145,32 @@
 
 # delete entire conversation
 account.dm_delete(conversation_id='123456-789012')
 
 # delete (hide) specific DM
 account.dm_delete(message_id='123456')
 
+# get all scheduled tweets
+scheduled_tweets = account.scheduled_tweets()
+
+# delete a scheduled tweet
+account.delete_scheduled_tweet(12345678)
+
+# get all draft tweets
+draft_tweets = account.draft_tweets()
+
+# delete a draft tweet
+account.delete_draft_tweet(12345678)
+
+# delete all scheduled tweets
+account.clear_scheduled_tweets()
+
+# delete all draft tweets
+account.clear_draft_tweets()
+
 # example configuration
 account.update_settings({
     "address_book_live_sync_enabled": False,
     "allow_ads_personalization": False,
     "allow_authenticated_periscope_requests": True,
     "allow_dm_groups_from": "following",
     "allow_dms_from": "following",
```

