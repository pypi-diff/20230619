# Comparing `tmp/pythttp-0.1.6.tar.gz` & `tmp/pythttp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.6.tar", last modified: Thu Jun 15 14:36:10 2023, max compression
+gzip compressed data, was "pythttp-0.1.7.tar", last modified: Mon Jun 19 15:18:21 2023, max compression
```

## Comparing `pythttp-0.1.6.tar` & `pythttp-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:36:10.855509 pythttp-0.1.6/
--rw-rw-rw-   0        0        0     1093 2023-06-15 14:36:10.854509 pythttp-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.6/README.md
--rw-rw-rw-   0        0        0      419 2023-06-15 14:33:11.000000 pythttp-0.1.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-15 14:36:10.845324 pythttp-0.1.6/pythttp/
--rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.6/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3516 2023-06-14 16:04:13.000000 pythttp-0.1.6/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    16734 2023-06-15 14:22:39.000000 pythttp-0.1.6/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     3906 2023-06-10 14:25:28.000000 pythttp-0.1.6/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.6/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.6/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:36:10.853509 pythttp-0.1.6/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 14:36:10.000000 pythttp-0.1.6/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 14:36:10.855509 pythttp-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      634 2023-06-15 14:33:09.000000 pythttp-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:18:21.831640 pythttp-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2023-06-19 15:18:21.830637 pythttp-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.7/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-19 15:17:28.000000 pythttp-0.1.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-19 15:18:21.823638 pythttp-0.1.7/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.7/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3473 2023-06-19 11:42:45.000000 pythttp-0.1.7/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    18937 2023-06-19 15:16:02.000000 pythttp-0.1.7/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     4500 2023-06-19 15:15:22.000000 pythttp-0.1.7/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.7/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.7/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:18:21.829641 pythttp-0.1.7/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 15:18:21.000000 pythttp-0.1.7/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 15:18:21.831640 pythttp-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-06-19 15:17:30.000000 pythttp-0.1.7/setup.py
```

### Comparing `pythttp-0.1.6/PKG-INFO` & `pythttp-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.6/README.md` & `pythttp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.6/pythttp/Log_Manager.py` & `pythttp-0.1.7/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.6/pythttp/Protocol.py` & `pythttp-0.1.7/pythttp/Protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import socket
-import select
-from urllib import request
 from urllib import parse
 from .Thread_Manager import *
 from .Structure import *
 from .Log_Manager import *
 
 class HyperTextTransferProtocol:
     def __init__(self):
```

### Comparing `pythttp-0.1.6/pythttp/RequestHandler.py` & `pythttp-0.1.7/pythttp/RequestHandler.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,95 +43,130 @@
         else:
             Response=self.ErrorHandler('405 Method Not Allowed',first_line)
         self.http.SendResponse(Response, socket_and_address)
         self.Thread.find_stopped_thread()
         self.Thread.ThreadDestructor(thread_name, client_address)
 
     def HandleGETRequest(self, Request):
-        result = parse.unquote(Request[0]).split(' ')[1].replace('\\','/')
+        result = parse.unquote(Request[0]).split(' ')[1].replace('\\', '/')
+        is_valid_cookie, cookie_value, session = self.verifySessionCookie(Request)
+        print(result,is_valid_cookie)
+        
         try:
-            Response = self.HandleTextFileRequest()
-            if ('.png' in result or '.html' in result or '.css' in result):
-                Response= self.HandleFileRequest(result)
-            elif '.ico' in result:
-                Response= self.HandleFileRequest(f'/icon/{result}')
-            elif '/Feed_Page' == result:
-                Response= self.UpdateFeedPage()
-            elif not self.verifySessionCookie(Request)[0]:
-                if ('/SignUp_form' == result or '/Login_form' == result):
-                    Response= self.HandleTextFileRequest(f'{result}.html')
-            elif (self.verifySessionCookie(Request)[0]):
-                if '/Logout_form' == result:
-                    Response= self.HandleTextFileRequest(f'{result}.html')
-                elif '/Account_Info' == result:
-                    Response= self.HandleAccountFileRequest(Request)
+            temporaryResponse = self.HandleTextFileRequest()
+            
+            if any(extension in result for extension in ['.png', '.html', '.css', '.js', '.ico']):
+                temporaryResponse = self.HandleFileRequest(result)
+            elif result == '/Feed_Page':
+                temporaryResponse = self.UpdateFeedPage()
+            elif not is_valid_cookie:
+                if result in ['/SignUp_form', '/Login_form']:
+                    temporaryResponse = self.HandleTextFileRequest(f'/html{result}.html')
+            elif is_valid_cookie:
+                if result == '/Logout_form':
+                    temporaryResponse = self.HandleTextFileRequest(f'/html{result}.html')
+                elif result == '/Account_Info':
+                    temporaryResponse = self.HandleAccountFileRequest(Request)
+            
+            Response = PrepareHeader()._response_headers(temporaryResponse[0], temporaryResponse[1]) + temporaryResponse[1]
+            
+            if is_valid_cookie:
+                cookie = {'SessionID': f'{cookie_value}; Expires={HttpDateTime().timestamp_to_http_datetime((datetime.now() + timedelta(days=1)).timestamp())}; Path=/'}
+                Response = PrepareHeader()._response_headers(temporaryResponse[0], temporaryResponse[1], Cookie=cookie) + temporaryResponse[1]
+            
             return Response
         except FileNotFoundError:
-            with open('resource/Error_Form.html','r',encoding='UTF-8') as arg:
-                return self.ErrorHandler('404 Not Found',f'The corresponding resource{result}file could not be found.')
+            with open('resource/html/Error_Form.html', 'r', encoding='UTF-8') as arg:
+                return self.ErrorHandler('404 Not Found', f'The corresponding {result} file could not be found.')
+
+
+    def HandlePOSTRequest(self, Request):
+        JsonData = parse.unquote(Request[1].decode())
+        DictPostData = json.loads(JsonData)
+        Form = DictPostData['Form']
+        Response = self.HandleTextFileRequest()
+        is_valid_cookie, cookie_value, session = self.verifySessionCookie(Request[0])
+
+        try:
+            if Form == 'SignUp':
+                temporaryResponse = self.SignUp_Handler(DictPostData['UserID'], DictPostData['UserEmail'], DictPostData['UserName'], DictPostData['UserPw'], is_valid_cookie)
+            elif Form == 'Login':
+                temporaryResponse = self.Login_Handler(DictPostData['UserID'], DictPostData['UserPw'], is_valid_cookie)
+                if temporaryResponse[0] == '200 OK':
+                    return PrepareHeader()._response_headers(temporaryResponse[0], temporaryResponse[1], Cookie=temporaryResponse[2]) + temporaryResponse[1]
+            elif Form == 'Logout':
+                temporaryResponse = self.Logout_Handler(is_valid_cookie,session)
+                if temporaryResponse[0] == '200 OK':
+                    return PrepareHeader()._response_headers(temporaryResponse[0], temporaryResponse[1], Cookie=temporaryResponse[2]) + temporaryResponse[1]
+            elif Form == 'Account':
+                temporaryResponse = self.UpdateAccount_Handler(DictPostData, session)
+            elif Form == 'PostUpload':
+                temporaryResponse = self.UploadPost_Handler(DictPostData, session)
+
+            Response = PrepareHeader()._response_headers(temporaryResponse[0], temporaryResponse[1]) + temporaryResponse[1]
+
+            if is_valid_cookie:
+                cookie = {'SessionID': f'{cookie_value}; Expires={HttpDateTime().timestamp_to_http_datetime((datetime.now() + timedelta(days=1)).timestamp())}; Path=/'}
+                Response = PrepareHeader()._response_headers(temporaryResponse[0], temporaryResponse[1], Cookie=cookie) + temporaryResponse[1]
+
+            return Response
+        
+        except Exception as e:
+            #Uncomment the following lines if you want to handle exceptions in a centralized manner
+            Response = self.ErrorHandler('500 Internal Server Error', e)
+            return Response
 
-    def HandlePOSTRequest(self,Request):
-        JsonData=parse.unquote(Request[1].decode())
-        DictPostData=json.loads(JsonData)
-        Form=DictPostData['Form']
-        Response=self.HandleTextFileRequest()
-        is_valid_cookie,cookie_value,session=self.verifySessionCookie(Request[0])
-        # try:
-        if Form == 'SignUp':
-            Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserEmail'],DictPostData['UserName'],DictPostData['UserPw'],is_valid_cookie)
-        elif Form == 'Login':
-            Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'],is_valid_cookie)
-        elif Form == 'Logout':
-            Response=self.Logout_Handler(cookie_value)
-        elif Form == 'Account':
-            Response=self.UpdateAccount_Handler(DictPostData,session)
-        elif Form == 'Upload_Post':
-            Response=self.UploadPost_Handler(DictPostData,session)
-        # except Exception as e:
-        #     Response=self.ErrorHandler('500 Internal Server Error',e)
-        return Response
 
     def verifySessionCookie(self,RequestData:list):
         for data in RequestData:
             if ('Cookie' in data and 'SessionID=' in data):
                 Values = data.split('SessionID=')[1]
                 for Session in self.Sessions:
                     if Values==Session.SessionToken:
                         return True, Values ,Session
         return False, None, None
+    
+    def verifySessionExpires(self,Session):
+        return False, None, None
 
-    def HandleFileRequest(self,file='/a.png'):
+    def HandleFileRequest(self,file='/img/a.png'):
         with open(f'resource{file}', 'rb') as ImgFile:
             Response_file=ImgFile.read()
-            return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+            return '200 OK',Response_file
         
-    def HandleTextFileRequest(self,flie='/Index.html',Cookie=None):
+    def HandleTextFileRequest(self,flie='/html/Index.html'):
         with open(f'resource{flie}','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read().encode('UTF-8')
-        return PrepareHeader()._response_headers('200 OK',Response_file,Cookie) + Response_file
+        return '200 OK',Response_file
+    
+    def HandleLogoutRequest(self,session):
+        with open(f'resource/html/Logout_Action.html','r',encoding='UTF-8') as TextFile:
+            Response_file=TextFile.read().encode('UTF-8')
+        cookie={'SessionID':f'{session.SessionToken}; Expires={HttpDateTime().timestamp_to_http_datetime((datetime.now() - timedelta(days=1)).timestamp())}; Path=/'}
+        return '200 OK',Response_file,cookie
+    
+    def HandleLoginRequest(self,session):
+        with open(f'resource/html/Login_Action.html','r',encoding='UTF-8') as TextFile:
+            Response_file=TextFile.read().encode('UTF-8')
+        cookie={'SessionID':f'{session.SessionToken}; Expires={session.SessionValidity}; Path=/'}
+        return '200 OK',Response_file,cookie
     
     def ErrorHandler(self,Error_code,Error_msg):
-        with open(f'resource/Error_Form.html','r',encoding='UTF-8') as TextFile:
+        with open(f'resource/html/Error_Form.html','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read()
             Response_file=Response_file.format(Error_code,Error_msg).encode('utf-8')
         self.log(f"[ Handle Error ] ==> Code : \033[35m{Error_code}\033[0m")
-        return PrepareHeader()._response_headers(Error_code,Response_file) + Response_file
+        return Error_code,Response_file
     
     def addFormatToHTML(self,HtmlText : str, FormatData : dict, style : str):
         Format=''
         for key,val in FormatData.items():
             Format+=f'{style.format(val=val,key=key)}'
         HtmlText=HtmlText.format(Format=Format)
         return HtmlText
-    
-    def ImgFileUpload(self,img_file,file_name):
-        with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
-            ImgFile.write(img_file)
-            self.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
-            return file_name
 
     def SignUp_Handler(self,UserID,UserEmail,UserName,UserPw,is_valid_cookie):
         UserUID=uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
         if self.Sessions and is_valid_cookie:
             return self.ErrorHandler('403 Forbidden','Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         for DB in self.ServerUsersDB:
             if (UserUID == DB.UserUID):
@@ -141,117 +176,124 @@
         except Exception as e:
             return self.ErrorHandler('403 Forbidden',f'{e} : {UserName,UserPw}')
         DB=StructDB(UserUID,AuthenticatedName,AuthenticatedPassword,UserEmail)
         self.ServerUsersDB.add(DB)
         self.log(f"[ New DataBase Constructed ] ==> DBID : \033[36m{DB.DataBaseID}\033[0m")
         self.log(f"[ SignUp User ] ==> UUID : \033[96m{UserUID}\033[0m")
         self.HandleSaveDB()
-        return self.HandleTextFileRequest('/SignUp_Action.html')
+        return self.HandleTextFileRequest('/html/SignUp_Action.html')
 
     def Login_Handler(self, UserID, UserPw, is_valid_cookie):
         UserUID = uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
         # Check if user is already logged in
         if self.Sessions and is_valid_cookie:
             return self.ErrorHandler('403 Forbidden','Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         # Check user credentials and create new session
         for db in self.ServerUsersDB:
             if (UserUID == db.UserUID and UserPw == db.UserPw):
-                session_id = self.RegisterUserSession(7, {'UserUID': UserUID, 'DataBaseID':db.DataBaseID, 'UserName':db.UserName})
-                self.log(f"[ New Session Constructed ] ==> SessionID: \033[96m{session_id}\033[0m")
-                return self.HandleTextFileRequest('/Login_Action.html',Cookie=f'SessionID = {session_id}')       
+                session = self.RegisterUserSession(1, {'UserUID': UserUID, 'DataBaseID':db.DataBaseID, 'UserName':db.UserName})
+                self.log(f"[ New Session Constructed ] ==> SessionID: \033[96m{session.SessionToken}\033[0m")
+                return self.HandleLoginRequest(session)
         return self.ErrorHandler('422 Unprocessable Entity',f'User ID or password does not exist: {UserID, UserPw}')
     
-    def Logout_Handler(self,SessionID):
-        for Session in self.Sessions:
-            if Session.SessionToken == SessionID:
-                self.Sessions.remove(Session)
-                self.log(f"[ Session Destructed ] ==> SessionID : \033[96m{SessionID}\033[0m")
-                return self.HandleTextFileRequest('/Logout_Action.html')
+    def Logout_Handler(self,is_valid_cookie,session):
+        if is_valid_cookie:
+            self.Sessions.remove(session)
+            self.log(f"[ Session Destructed ] ==> SessionID : \033[96m{session.SessionToken}\033[0m")
+            return self.HandleLogoutRequest(session)
         return self.ErrorHandler('403 Forbidden',f'To log out, you must first log in. Please verify your account information and log in before attempting to log out')
     
     def HandleAccountFileRequest(self,Request):
-        DataBaseID=self.verifySessionCookie(Request)[2].UserInfo['DataBaseID']
-        for db in self.ServerUsersDB:
-            if DataBaseID == db.DataBaseID:
-                Username=db.UserName
-                UserUID=db.UserUID
-                Useremail=db.UserEmail
-        with open(f'resource/Account_Info.html','r',encoding='UTF-8') as TextFile:
+        DataBase=self.getDatabase(self.verifySessionCookie(Request)[2].UserInfo['DataBaseID'])
+        with open(f'resource/html/Account_Info.html','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read()
-            Response_file=Response_file.format(UserName=Username,UserUID=UserUID,UserEmail=Useremail,UserBirthDate='None').encode('utf-8')
-        return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+            Response_file=Response_file.format(UserName=DataBase.UserName,UserUID=DataBase.UserUID,UserPw=DataBase.UserPw,UserEmail=DataBase.UserEmail,BirthDate=DataBase.UserBirthDate).encode('utf-8')
+        return '200 OK',Response_file
     
     def UpdateAccount_Handler(self,newUserInfo,session):
-        DataBaseID=session.UserInfo['DataBaseID']
+        DataBase=self.getDatabase(session.UserInfo['DataBaseID'])
+        DataBase.UserName=newUserInfo['UserName']
+        DataBase.UserEmail=newUserInfo['UserEmail']
+        DataBase.UserBirthDate=newUserInfo['BirthDate']
+        if DataBase.UserPw!=newUserInfo['UserPw']:
+            DataBase.UserPw=newUserInfo['UserPw']
+            self.Logout_Handler(session.SessionToken)   
+        self.HandleSaveDB()
+        return self.HandleTextFileRequest('/html/Account_Action.html')
+    
+    def getDatabase(self,DataBaseID):
         for DataBase in self.ServerUsersDB:
             if DataBaseID == DataBase.DataBaseID:
-                DataBase.UserName=newUserInfo['UserName']
-                DataBase.UserEmail=newUserInfo['UserEmail']
-                if DataBase.UserPw!=newUserInfo['UserPw']:
-                    DataBase.UserPw=newUserInfo['UserPw']
-                    self.Logout_Handler(session.SessionToken)   
-            self.HandleSaveDB()
-            return self.HandleTextFileRequest('/Account_Action.html')
+                return DataBase
         
-    def UploadPost_Handler(self,PostData,Session):
-        if Session == None:
-            return self.ErrorHandler('403 Forbidden','Warning! You are attempting to post without logging in. If you wish to make a post, please proceed with the login.')
-        PostImageName=''
-        User=Session.UserInfo['UserUID']
-        UploadTime=datetime.now().strftime('%Y-%m-%d_%H%M')
+    def UploadPost_Handler(self, PostData, Session):
+        if Session is None:
+            return self.ErrorHandler('403 Forbidden', 'Warning! You are attempting to post without logging in. If you wish to make a post, please proceed with the login.')
+
+        PostImageName = ''
+        User = Session.UserInfo['UserUID']
+        UploadTime = datetime.now().strftime('%Y-%m-%d_%H%M')
+        post_file_upload_path = f'resource/PostFileUpload/{User}'
+
         try:
-            os.mkdir(f'resource/PostFileUpload/{User}')
-        except:
-            pass
-        PostFileName=f'resource/PostFileUpload/{User}/_{UploadTime}.html'.replace(':','-')
-        title=PostData['title']
-        content=PostData['content']
-        name=Session.UserInfo['UserName']
-        if 'image' in PostData.keys():
-            OriginalData=base64.b64decode(PostData['image'].split(',')[1])
-            PostImageName=f'_{UploadTime}.png'
-            with open(f'resource/PostFileUpload/{User}/{PostImageName}','wb') as ImageFile:
+            os.makedirs(post_file_upload_path, exist_ok=True)
+        except OSError as e:
+            print(f"Error: {e}")
+
+        PostFileName = f'resource/PostFileUpload/{User}/_{UploadTime}.html'.replace(':', '-')
+        title = PostData['title']
+        content = PostData['content']
+        name = Session.UserInfo['UserName']
+        image =f'_{UploadTime}.png'
+
+        if PostData['image'] is not None:
+            OriginalData = base64.b64decode(PostData['image'])
+            PostImageName = f'_{UploadTime}.png'
+            with open(f'{post_file_upload_path}/{PostImageName}', 'wb') as ImageFile:
                 ImageFile.write(OriginalData)
-        with open(f'resource/Post_Form.html','r',encoding='UTF-8') as PostFormFile:
-            with open(PostFileName,'w',encoding='UTF-8') as PostTempFile:
-                PostTempFile.write(PostFormFile.read().format(PostTitle=title,PostContent=content,UserName=name,PostImage=PostImageName))
-                self.ServerPostDB.append({str(User):{'Path':f'/_{UploadTime}.html','title':title,'content':content,'name':name}})
+
+        with open(f'resource/html/Post_Form.html', 'r', encoding='UTF-8') as PostFormFile:
+            with open(PostFileName, 'w', encoding='UTF-8') as PostTempFile:
+                PostTempFile.write(PostFormFile.read().format(PostTitle=title, PostContent=content, UserName=name, PostImage=image))
+                self.ServerPostDB.append({str(User): {'Path': f'/_{UploadTime}.html', 'title': title, 'content': content, 'name': name}})
+
         return self.UpdateFeedPage()
 
     def UpdateFeedPage(self):
-        FeedPost=''
-        FeedPostForm="""
-        <a href="{Path}">
-        <li>
-          <div class="user-profile">
-            <img src="" alt="{name}">
-          </div>
-          <div class="post-content">
-              <h2>{title}</h2>
-              <p>{content}</p>
-          </div>
-        </li>
-        </a>\n"""
-        with open(f'resource/Feed_Page.html','r+',encoding='UTF-8') as FeedFormFile:
+        FeedPostForm = """
+            <div class="mainform">
+                <div class="border rounded-lg p-4 cursor-pointer" onclick="goToPostPage('{0}')">
+                    <div class="post">
+                        <h2 class="text-lg font-bold mb-2">{1}</h2>
+                        <p>{2}</p>
+                    </div>
+                </div>
+            </div>\n"""
+
+        with open(f'resource/html/Feed_Page.html', 'r', encoding='UTF-8') as FeedFormFile:
             FeedForm = FeedFormFile.read()
+
+        FeedPost = ''
         if self.ServerPostDB:
             for i in self.ServerPostDB:
-                for ID,Post in i.items():
-                    PostFilePath=f'/PostFileUpload/{ID}'+Post['Path'].replace(':','-')
-                    FeedPost+=FeedPostForm.format(Path=PostFilePath,name=Post['name'],title=Post['title'],content=Post['content'])
-        FeedForm = FeedForm.replace('{FeedPost}',FeedPost).encode('UTF-8')
-        with open(f'resource/PostStorage.html','a',encoding='UTF-8') as PostStorage:
+                for ID, Post in i.items():
+                    PostFilePath = f'/PostFileUpload/{ID}' + Post['Path'].replace(':', '-')
+                    FeedPost += FeedPostForm.format(PostFilePath, Post['title'], Post['content'])
+
+        with open(f'resource/html/PostStorage.html', 'w', encoding='UTF-8') as PostStorage:
             PostStorage.write(FeedPost)
-        return PrepareHeader()._response_headers('200 OK',FeedForm) + FeedForm
-        
+
+        FeedForm = FeedForm.replace('{FeedPost}', FeedPost).encode('UTF-8')
+
+        return '200 OK', FeedForm
 
     def RegisterUserSession(self,  SessionValidityDays: str, UserInfo: dict):
         SessionInfo = Session(SessionValidityDays, UserInfo)
         self.Sessions.add(SessionInfo)
-        return SessionInfo.SessionToken
+        return SessionInfo
 
     def HandleSaveDB(self):
         with open(f'resource/ServerUserDB.DB','wb') as DBfile:
             pickle.dump(self.ServerUsersDB,DBfile)
             self.log(f"[ Database Save Successful ] ==> path : \033[34mresource/ServerUserDB.DB\033[0m")
 
     def HandleloadDB(self):
@@ -282,15 +324,15 @@
     #SessionDict: dict = field(init=False, default_factory=dict)
 
     def __post_init__(self):
         """
         Initializes the SessionToken, SessionValidity, and SessionDict attributes after object creation.
         """
         self.SessionToken = SessionID(16).Token
-        self.SessionValidity = (datetime.now() + timedelta(days=self.SessionValidityDays)).timestamp()
+        self.SessionValidity = HttpDateTime().datetime_to_http_datetime(datetime.now() + timedelta(days=self.SessionValidityDays))
         # self.SessionDict['SessionID'] = self.SessionToken
         # self.SessionDict['SessionValidity'] = self.SessionValidity
         # self.SessionDict['UserInfo'] = self.UserInfo
 
     def __hash__(self):
         return hash(self.SessionToken)
```

### Comparing `pythttp-0.1.6/pythttp/Structure.py` & `pythttp-0.1.7/pythttp/Structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import datetime as dt
+from datetime import datetime, timedelta
 from dataclasses import dataclass, field
 import secrets
 
 
 
 @dataclass
 class StructDB:
     DataBaseID:str =field(init=False, default=None)
     UserUID: str
     UserName: str
     UserPw: str
     UserEmail: str = None
+    UserBirthDate: str = None
     UserUploadFiles: dict =field(default_factory=dict)
     StructDBdict: dict =field(init=False,default_factory=dict)
     def __post_init__(self):
         self.DataBaseID = DataBaseID(16).Token
         # self.StructDBdict['UserUID'] = self.UserUID
         # self.StructDBdict['UserName'] = self.UserName
         # self.StructDBdict['UserPw'] = self.UserPw
@@ -78,30 +79,35 @@
         }
         if params:
             url += '?' + '&'.join([f'{key}={value}' for key, value in params.items()])
         return f'{method} {url} HTTP/1.1\r\n' + \
                '\r\n'.join([f'{key}: {value}' for key, value in headers.items()]) + \
                '\r\n\r\n'
 
-    def _response_headers(self,status_code,Content,Cookie=None):
+    def _response_headers(self,status_code,Content,Cookie=False):
         headers = {
-            'Date': HttpDateTime().http_date_time,
-            'Server':'longinus',
-            'Cache-Control': 'no-store, no-cache, must-revalidate, post-check=0, pre-check=0',
+            'Date' : HttpDateTime().http_date_time,
+            'Server' : 'longinus',
+            'Cache-Control' : 'max-age=3600 ,no-cache ,private',
             'Pragma' : 'no-cache',
             'Content-Length': len(Content),
-            'Set-Cookie' : Cookie
         }
+        if Cookie:
+            headers.update(self.convert_cookie_dict_to_header(Cookie))
         return (f'HTTP/1.1 {status_code}\r\n' + \
         '\r\n'.join([f'{key}: {value}' for key, value in headers.items()]) + \
         '\r\n\r\n').encode()
 
+    def convert_cookie_dict_to_header(self,cookie_dict):
+        cookie_str = '; '.join([f'{key}={value}' for key, value in cookie_dict.items()])
+        return {'Set-Cookie': cookie_str}
+
 class HttpDateTime:
     def __init__(self):
-        now_utc = dt.datetime.utcnow().replace(microsecond=0)
+        now_utc = datetime.utcnow().replace(microsecond=0)
         month_dict = {
             '01': 'Jan',
             '02': 'Feb',
             '03': 'Mar',
             '04': 'Apr',
             '05': 'May',
             '06': 'Jun',
@@ -109,8 +115,17 @@
             '08': 'Aug',
             '09': 'Sep',
             '10': 'Oct',
             '11': 'Nov',
             '12': 'Dec'
         }
         day_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-        self.http_date_time = f'{day_list[now_utc.weekday()]} {now_utc.day} {month_dict[now_utc.strftime("%m")]} {now_utc.year} {now_utc.strftime("%H:%M:%S")} GMT'
+        self.http_date_time = f'{day_list[now_utc.weekday()]} {now_utc.day} {month_dict[now_utc.strftime("%m")]} {now_utc.year} {now_utc.strftime("%H:%M:%S")} GMT'
+
+
+    def timestamp_to_http_datetime(self,timestamp):
+        dt = datetime.fromtimestamp(timestamp)
+        http_datetime = dt.strftime('%a, %d %b %Y %H:%M:%S GMT')
+        return http_datetime
+    
+    def datetime_to_http_datetime(self,datetime):
+        return datetime.strftime("%a, %d %b %Y %H:%M:%S GMT")
```

### Comparing `pythttp-0.1.6/pythttp/Thread_Manager.py` & `pythttp-0.1.7/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.6/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.7/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.6/setup.py` & `pythttp-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.6",
+    version="0.1.7",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=['dataclasses','datetime','uuid'],
```

