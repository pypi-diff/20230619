# Comparing `tmp/IMDBTraktSyncer-1.4.2.tar.gz` & `tmp/IMDBTraktSyncer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.4.2.tar", last modified: Fri Jun 16 08:33:43 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.5.0.tar", last modified: Mon Jun 19 09:53:46 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.4.2.tar` & `IMDBTraktSyncer-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:43.398814 IMDBTraktSyncer-1.4.2/
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:43.366812 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    30980 2023-06-16 08:29:52.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     8515 2023-06-16 08:18:58.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10272 2023-06-15 14:00:20.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    11171 2023-06-15 16:19:15.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:43.395820 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12155 2023-06-16 08:33:43.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-06-16 08:33:43.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:33:43.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-16 08:33:43.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-16 08:33:43.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-16 08:33:43.000000 IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.4.2/LICENSE
--rw-rw-rw-   0        0        0    12155 2023-06-16 08:33:43.397811 IMDBTraktSyncer-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    11409 2023-06-16 06:52:26.000000 IMDBTraktSyncer-1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 08:33:43.398814 IMDBTraktSyncer-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-16 08:33:28.000000 IMDBTraktSyncer-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:53:46.226639 IMDBTraktSyncer-1.5.0/
+drwxrwxrwx   0        0        0        0 2023-06-19 09:53:46.192153 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    35301 2023-06-19 09:48:35.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6693 2023-06-19 09:47:56.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1511 2023-06-19 08:07:22.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    10221 2023-06-19 09:48:14.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12076 2023-06-19 09:48:05.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:53:46.223152 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12155 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-19 09:53:46.000000 IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    12155 2023-06-19 09:53:46.225183 IMDBTraktSyncer-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11409 2023-06-19 09:51:38.000000 IMDBTraktSyncer-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:53:46.227154 IMDBTraktSyncer-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-19 09:52:05.000000 IMDBTraktSyncer-1.5.0/setup.py
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 from selenium.common.exceptions import SessionNotCreatedException
 try:
     from IMDBTraktSyncer import checkChromedriver
     from IMDBTraktSyncer import verifyCredentials as VC
     from IMDBTraktSyncer import traktData
     from IMDBTraktSyncer import imdbData
     from IMDBTraktSyncer import errorHandling as EH
+    from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import checkChromedriver
     import verifyCredentials as VC
     import traktData
     import imdbData
     import errorHandling as EH
+    import errorLogger as EL
 from chromedriver_py import binary_path
 
+class PageLoadException(Exception):
+    pass
 
 def main():
     try:
 
         #Get credentials
         imdb_username = VC.imdb_username
         imdb_password = VC.imdb_password
@@ -61,21 +65,26 @@
             driver = webdriver.Chrome(service=service, options=options)
         except SessionNotCreatedException as e:
             error_message = str(e)
             if "This version of ChromeDriver only supports Chrome version" in error_message:
                 extract_message = error_message.split("Stacktrace:")[0].replace("Message: session not created:", "").strip()
                 print(f"Error: {extract_message}")
                 print("See this link for details on how to fix: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16")
+                EL.logger.error(extract_message, exc_info=True)
                 raise SystemExit
             else:
                 raise
 
         wait = WebDriverWait(driver, 10)
         
-        driver.get('https://www.imdb.com/registration/signin')
+        # Load sign in page
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/registration/signin', driver)
+        if not success:
+            # Page failed to load, raise an exception
+            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         # wait for sign in link to appear and then click it
         sign_in_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'a.list-group-item > .auth-provider-text')))
         if 'IMDb' in sign_in_link.text:
             sign_in_link.click()
 
         # wait for email input field and password input field to appear, then enter credentials and submit
@@ -85,29 +94,33 @@
         password_input.send_keys(imdb_password)
         submit_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input[type='submit']")))
         submit_button.click()
 
         time.sleep(2)
 
         # go to IMDB homepage
-        driver.get('https://www.imdb.com/')
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/', driver)
+        if not success:
+            # Page failed to load, raise an exception
+            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         time.sleep(2)
 
         # Check if signed in
         element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".nav__userMenu.navbar__user")))
         if element.find_elements(By.CSS_SELECTOR, ".imdb-header__account-toggle--logged-in"):
             print("Successfully signed in to IMDB")
         else:
             print("Error: Not signed in to IMDB")
             print("\nPossible IMDB captcha check or IMDB login incorrect.")
             print("\nIf your login is correct then an IMDB captcha check likely the cause of this error. To fix this, simply login to the IMDB website in your browser, preferably Chrome, and from the same computer. If logged in, log out and log back in. It may ask you to fill in a captcha; complete it and finish logging in. After logging in successfully on your browser, run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues.")
             print("\nIf your IMDB login is incorrect, simply edit the credentials.txt file with the correct login or delete the credentials file and run the script again.")
             print("\nSee this GitHub link for more details: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2")
             print("\nStopping script...")
+            EL.logger.error("Error: Not signed in to IMDB")
             raise SystemExit
         
         trakt_watchlist, trakt_ratings, trakt_reviews, watched_content = traktData.getTraktData()
         imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
 
         # Get trakt and imdb data and filter out items with missing imdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating.get('IMDB_ID') is not None]
@@ -187,18 +200,19 @@
                             "ids": {
                                 "imdb": imdb_id
                             }
                         })
 
                     response = EH.make_trakt_request(url, payload=data)
                     if response:
-                        print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
+                        print(f" - Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     else:
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
-                        print("Error Response:", response.content, response.status_code)
+                        error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
             # Set IMDB Watchlist Items
             if imdb_watchlist_to_set:
@@ -208,17 +222,24 @@
                 num_items = len(imdb_watchlist_to_set)
                 item_count = 0
                                 
                 for item in imdb_watchlist_to_set:
                     try:
                         item_count += 1
                         year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
-                        print(f"Adding item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist")
+                        print(f" - Adding item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist")
                         
-                        driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
+                        # Load page
+                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver)
+                        if not success:
+                            # Page failed to load, raise an exception
+                            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+                        
+                        # Wait until the loader has disappeared, indicating the watchlist button has loaded
+                        wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
                         
                         # Scroll the page to bring the element into view
                         watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
                         driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
                         
                         # Wait for the element to be clickable
                         watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
@@ -231,18 +252,22 @@
                                 try:
                                     WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--done')))
                                     break  # Break the loop if successful
                                 except TimeoutException:
                                     retry_count += 1
 
                             if retry_count == 2:
-                                print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})")
-                        
-                    except (NoSuchElementException, TimeoutException):
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})")
+                                error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})"
+                                print(f"   - {error_message}")
+                                EL.logger.error(error_message)
+                        
+                    except (NoSuchElementException, TimeoutException, PageLoadException):
+                        error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message, exc_info=True)
                         pass
 
                 
                 print('Setting IMDB Watchlist Items Complete')
             else:
                 print('No IMDB Watchlist Items To Set')
          
@@ -269,75 +294,88 @@
                             "shows": [{
                                 "ids": {
                                     "imdb": item["IMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
-                        print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                        print(f" - Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
                     elif item["Type"] == "movie":
                         # This is a movie
                         data = {
                             "movies": [{
                                 "ids": {
                                     "imdb": item["IMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
-                        print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                        print(f" - Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
                     elif item["Type"] == "episode":
                         # This is an episode
                         data = {
                             "episodes": [{
                                 "ids": {
                                     "imdb": item["IMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
-                        print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                        print(f" - Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
 
                     # Make the API call to rate the item
                     response = EH.make_trakt_request(rate_url, payload=data)
 
                     if response is None:
-                        print(f"Error rating {item}: {response.content}")
+                        error_message = f"Failed rating {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Setting Trakt Ratings Complete')
             else:
                 print('No Trakt Ratings To Set')
 
             # Set IMDB Ratings
             if imdb_ratings_to_set:
                 print('Setting IMDB Ratings')
 
                 # loop through each movie and TV show rating and submit rating on IMDB website
                 for i, item in enumerate(imdb_ratings_to_set, 1):
+
                     year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
-                    print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB')
-                    driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
+                    print(f' - Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB')
                     
                     try:
+                        # Load page
+                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver)
+                        if not success:
+                            # Page failed to load, raise an exception
+                            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+                        
+                        # Wait until the rating bar has loaded
+                        wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__loading"]')))
+                        
                         # Wait until rate button is located and scroll to it
                         button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                         driver.execute_script("arguments[0].scrollIntoView(true);", button)
 
                         # click on "Rate" button and select rating option, then submit rating
                         button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                         element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
                         if element_rating_bar:
                             driver.execute_script("arguments[0].click();", button)
                             rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
                             driver.execute_script("arguments[0].click();", rating_option_element)
                             submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
                             submit_element.click()
                             time.sleep(1)
-                    except (NoSuchElementException, TimeoutException):
-                        print(f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["IMDB_ID"]})')
+                    except (NoSuchElementException, TimeoutException, PageLoadException):
+                        error_message = f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["IMDB_ID"]})'
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message, exc_info=True)
                         pass
 
                 print('Setting IMDB Ratings Complete')
             else:
                 print('No IMDB Ratings To Set')
 
         # If sync_reviews_value is true
@@ -383,18 +421,19 @@
                                 "ids": {
                                     "imdb": episode_id
                                 }
                             }
                         
                         response = EH.make_trakt_request(url, payload=data)
                         if response:
-                            print(f"Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
+                            print(f" - Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                         else:
-                            print(f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
-                            print("Error Response:", response.content, response.status_code)
+                            error_message = f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt"
+                            print(f"   - {error_message}")
+                            EL.logger.error(error_message)
 
                     print('Trakt Reviews Set Successfully')
                 else:
                     print('No Trakt Reviews To Set')
 
                 # Set IMDB Reviews
                 if imdb_reviews_to_set:
@@ -405,16 +444,21 @@
                         # Count the total number of items
                         num_items = len(imdb_reviews_to_set)
                         item_count = 0
                         
                         for review in imdb_reviews_to_set:
                             item_count += 1
                             try:
-                                print(f"Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
-                                driver.get(f'https://contribute.imdb.com/review/{review["IMDB_ID"]}/add?bus=imdb')
+                                print(f" - Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
+                                
+                                # Load page
+                                success, status_code, url = EH.get_page_with_retries(f'https://contribute.imdb.com/review/{review["IMDB_ID"]}/add?bus=imdb', driver)
+                                if not success:
+                                    # Page failed to load, raise an exception
+                                    raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                                 
                                 review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
                                 review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
                                 
                                 review_title_input.send_keys("My Review")
                                 review_input.send_keys(review["Comment"])
                                 
@@ -427,16 +471,18 @@
                                     no_element.click()
                                                         
                                 submit_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
 
                                 submit_button.click()
                                 
                                 time.sleep(3) # wait for rating to submit
-                            except (NoSuchElementException, TimeoutException):
-                                print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['IMDB_ID']})")
+                            except (NoSuchElementException, TimeoutException, PageLoadException):
+                                error_message = f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['IMDB_ID']})"
+                                print(f"   - {error_message}")
+                                EL.logger.error(error_message, exc_info=True)
                                 pass
                         
                         print('Setting IMDB Reviews Complete')
                     else:
                         print('IMDB reviews were submitted within the last 10 days. Skipping IMDB review submission.')
                 else:
                     print('No IMDB Reviews To Set')
@@ -465,41 +511,43 @@
                         data = {
                             "shows": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
-                        print(f"Removing TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                        print(f" - Removing TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
                     elif item["Type"] == "movie":
                         # This is a movie
                         data = {
                             "movies": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
-                        print(f"Removing movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                        print(f" - Removing movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
                     elif item["Type"] == "episode":
                         # This is an episode
                         data = {
                             "episodes": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
-                        print(f"Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                        print(f" - Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
 
                     # Make the API call to remove the item from the watchlist
                     response = EH.make_trakt_request(remove_url, payload=data)
 
                     if response is None:
-                        print(f"Error removing {item}: {response.content}")
+                        error_message = f"Error removing {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Removing Watched Items From Trakt Watchlist Complete')
             else:
                 print('No Watched Items To Remove From Trakt Watchlist')
 
             # Remove Watched Items IMDB Watchlist
             if imdb_watchlist_items_to_remove:
@@ -509,17 +557,24 @@
                 num_items = len(imdb_watchlist_items_to_remove)
                 item_count = 0
                                 
                 for item in imdb_watchlist_items_to_remove:
                     try:
                         item_count += 1
                         year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
-                        print(f"Removing item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist")
+                        print(f" - Removing item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist")
                         
-                        driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
+                        # Load page
+                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver)
+                        if not success:
+                            # Page failed to load, raise an exception
+                            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+                        
+                        # Wait until the loader has disappeared, indicating the watchlist button has loaded
+                        wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
                         
                         # Scroll the page to bring the element into view
                         watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
                         driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
                         
                         # Wait for the element to be clickable
                         watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
@@ -532,18 +587,22 @@
                                 try:
                                     WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--add')))
                                     break  # Break the loop if successful
                                 except TimeoutException:
                                     retry_count += 1
 
                             if retry_count == 2:
-                                print(f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})")
-
-                    except (NoSuchElementException, TimeoutException):
-                        print(f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})")
+                                error_message = f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})"
+                                print(f"   - {error_message}")
+                                EL.logger.error(error_message)
+
+                    except (NoSuchElementException, TimeoutException, PageLoadException):
+                        error_message = f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message, exc_info=True)
                         pass
 
                 
                 print('Removing Watched Items From IMDB Watchlist Complete')
             else:
                 print('No Watched Items To Remove From IMDB Watchlist')
         
@@ -551,10 +610,11 @@
         print("Closing webdriver...")
         driver.quit()
         service.stop()
     
     except Exception as e:
         error_message = "An error occurred while running the script."
         EH.report_error(error_message)
+        EL.logger.error(error_message, exc_info=True)
 
 if __name__ == '__main__':
     main()
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/authTrakt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import requests
 import time
+try:
+    from IMDBTraktSyncer import errorLogger as EL
+except ImportError:
+    import errorLogger as EL
 
 def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
     retry_delay = 5  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
@@ -23,15 +27,17 @@
                 print(f"Request failed with status code {response.status_code}: {error_message}")
                 return None
 
         except requests.exceptions.RequestException as e:
             print(f"Request failed with exception: {e}")
             return None
 
-    print("Max retry attempts reached with Trakt API, request failed.")
+    error_message = "Max retry attempts reached with Trakt API, request failed."
+    print(f"{error_message}")
+    EL.logger.error(error_message)
     return None
 
 def get_trakt_message(status_code):
     error_messages = {
         200: "Success",
         201: "Success - new resource created (POST)",
         204: "Success - no content to return (DELETE)",
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/checkChromedriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import feedparser
 import subprocess
 import pkg_resources
 import platform
 import sys
+try:
+    from IMDBTraktSyncer import errorLogger as EL
+except ImportError:
+    import errorLogger as EL
 
 def get_chrome_version():
     system = platform.system()
     if system == 'Windows':
         from winreg import ConnectRegistry, HKEY_CURRENT_USER, OpenKey, QueryValueEx
 
         try:
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/imdbData.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,24 +8,33 @@
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from chromedriver_py import binary_path
 try:
     from IMDBTraktSyncer import errorHandling as EH
+    from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import errorHandling as EH
+    import errorLogger as EL
+
+class PageLoadException(Exception):
+    pass
 
 def getImdbData(imdb_username, imdb_password, driver, directory, wait):
     # Process IMDB Ratings Reviews & Watchlist
     print('Processing IMDB Data')
     
     #Get IMDB Watchlist Items
     try:
-        driver.get('https://www.imdb.com/list/watchlist')
+        # Load page
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/watchlist', driver)
+        if not success:
+            # Page failed to load, raise an exception
+            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".export a")))
         driver.execute_script("arguments[0].scrollIntoView(true);", csv_link)
         csv_link.click()
 
         #Wait for csv download to complete
         time.sleep(8)
@@ -49,29 +58,35 @@
                         media_type = "episode"
                     elif "movie" in row[7]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
                     imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Type': media_type})
         except FileNotFoundError:
-            print('Ratings file not found')
+            error_message = "Ratings file not found"
+            print(f"{error_message}")
+            EL.logger.error(error_message, exc_info=True)
             
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'WATCHLIST' in file:
                 os.remove(os.path.join(directory, file))
 
     except (NoSuchElementException, TimeoutException):
         # No IMDB Watchlist Items
         imdb_watchlist = []
         pass
     
     # Get IMDB Ratings
     try:
-        driver.get('https://www.imdb.com/list/ratings')
+        # Load page
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/ratings', driver)
+        if not success:
+            # Page failed to load, raise an exception
+            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         dropdown = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".circle")))
         dropdown.click()
 
         csv_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
         csv_link.click()
 
@@ -107,40 +122,50 @@
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'ratings' in file:
                 os.remove(os.path.join(directory, file))
     except (NoSuchElementException, TimeoutException):
         # No IMDB Ratings
         imdb_ratings = []
+        error_message = "No IMDB Ratings"
+        EL.logger.error(error_message, exc_info=True)
         pass
             
     def get_media_type(imdb_id):
         url = f"https://api.trakt.tv/search/imdb/{imdb_id}"
         response = EH.make_trakt_request(url)
         if response:
             results = response.json()
             if results:
                 media_type = results[0].get('type')
                 return media_type
         return None
 
     #Get IMDB Reviews
-    driver.get('https://www.imdb.com/profile')
+    
+    # Load page
+    success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/profile', driver)
+    if not success:
+        # Page failed to load, raise an exception
+        raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+    
     reviews = []
     errors_found_getting_imdb_reviews = False
     try:
         reviews_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")))
         reviews_link.click()
 
         while True:
             try:
                 try:
                     review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
                 except (NoSuchElementException, TimeoutException):
                     # No review elements found. There are no reviews. Exit the loop without an error.
+                    error_message = "No review elements found. There are no reviews. Exit the loop without an error."
+                    EL.logger.error(error_message, exc_info=True)
                     break
                 
                 for element in review_elements:
                     review = {}
                     # Extract review details
                     review['Title'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").text
                     review['Year'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header span").text.strip('()').split('–')[0].strip()
@@ -169,23 +194,30 @@
                     # Wait until the URL changes
                     wait.until(EC.url_changes(current_url))
                     
                     # Refresh review_elements
                     review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
 
                 except (NoSuchElementException, TimeoutException):
-                    break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop without error.
+                    # "Next" link not found or timed out waiting for the "Next" link, exit the loop without error.
+                    error_message = '"Next" link not found or timed out waiting for the "Next" link, exit the loop without error.'
+                    EL.logger.error(error_message, exc_info=True)
+                    break
             except Exception as e:
                 errors_found_getting_imdb_reviews = True
-                print(f"Exception occurred while getting IMDB reviews: {type(e)}")
+                error_message = f"Exception occurred while getting IMDB reviews: {type(e)}"
+                print(f"{error_message}")
+                EL.logger.error(error_message, exc_info=True)
                 break
     
     except Exception as e:
         errors_found_getting_imdb_reviews = True
-        print(f"Exception occurred while getting IMDB reviews: {type(e)}")
+        error_message = f"Exception occurred while getting IMDB reviews: {type(e)}"
+        print(f"{error_message}")
+        EL.logger.error(error_message, exc_info=True)
 
     # Filter out duplicate reviews for the same item based on ID
     filtered_reviews = []
     seen = set()
     for item in reviews:
         if item['IMDB_ID'] not in seen:
             seen.add(item['IMDB_ID'])
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/traktData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import requests
 import time
 import urllib.parse
 import datetime
 try:
     from IMDBTraktSyncer import errorHandling as EH
+    from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import errorHandling as EH
+    import errorLogger as EL
 
 def getTraktData():
     # Process Trakt Ratings and Comments
     print('Processing Trakt Data')
 
     response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer/verifyCredentials.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import json
 import datetime
 try:
     from IMDBTraktSyncer import authTrakt
+    from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import authTrakt
+    import errorLogger as EL
 
 def prompt_get_credentials():
     # Define the file path
     here = os.path.abspath(os.path.dirname(__file__))
     file_path = os.path.join(here, 'credentials.txt')
 
     # Old version support (v1.0.6 and below). Convert old credentials.txt format to json
@@ -77,14 +79,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             sync_ratings_value = credentials.get('sync_ratings')
             if sync_ratings_value is not None:
                 return sync_ratings_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Do you want to sync ratings? (y/n)")
         user_input = input("Enter your choice: ")
 
@@ -101,14 +105,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['sync_ratings'] = sync_ratings_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
 
@@ -124,14 +130,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             sync_watchlist_value = credentials.get('sync_watchlist')
             if sync_watchlist_value is not None:
                 return sync_watchlist_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Do you want to sync watchlists? (y/n)")
         user_input = input("Enter your choice: ")
 
@@ -148,14 +156,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['sync_watchlist'] = sync_watchlist_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
 
@@ -198,14 +208,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             sync_reviews_value = credentials.get('sync_reviews')
             if sync_reviews_value is not None:
                 return sync_reviews_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Ratings are synced by default. Please note: comments synced to IMDB will use \"My Review\" as the title field.")
         print("Do you want to sync comments? (y/n)")
         user_input = input("Enter your choice: ")
@@ -223,14 +235,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['sync_reviews'] = sync_reviews_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
 
@@ -246,14 +260,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             remove_watched_from_watchlists_value = credentials.get('remove_watched_from_watchlists')
             if remove_watched_from_watchlists_value is not None:
                 return remove_watched_from_watchlists_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Movies and Episodes are removed from watchlists after 1 play.")
         print("Shows are removed when atleast 80% of the episodes are watched AND the series is marked as ended or cancelled.")
         print("Do you want to remove watched items watchlists? (y/n)")
@@ -272,14 +288,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['remove_watched_from_watchlists'] = remove_watched_from_watchlists_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.4.2
+Version: 1.5.0
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.4.2/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.5.0/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 IMDBTraktSyncer/IMDBTraktSyncer.py
 IMDBTraktSyncer/__init__.py
 IMDBTraktSyncer/authTrakt.py
 IMDBTraktSyncer/checkChromedriver.py
 IMDBTraktSyncer/errorHandling.py
+IMDBTraktSyncer/errorLogger.py
 IMDBTraktSyncer/imdbData.py
 IMDBTraktSyncer/traktData.py
 IMDBTraktSyncer/verifyCredentials.py
 IMDBTraktSyncer.egg-info/PKG-INFO
 IMDBTraktSyncer.egg-info/SOURCES.txt
 IMDBTraktSyncer.egg-info/dependency_links.txt
 IMDBTraktSyncer.egg-info/entry_points.txt
```

### Comparing `IMDBTraktSyncer-1.4.2/LICENSE` & `IMDBTraktSyncer-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.2/PKG-INFO` & `IMDBTraktSyncer-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.4.2
+Version: 1.5.0
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.4.2/README.md` & `IMDBTraktSyncer-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.2/setup.py` & `IMDBTraktSyncer-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.4.2'
+VERSION = '1.5.0'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

