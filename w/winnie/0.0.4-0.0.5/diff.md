# Comparing `tmp/winnie-0.0.4.tar.gz` & `tmp/winnie-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winnie-0.0.4.tar", last modified: Fri Jun 16 21:08:43 2023, max compression
+gzip compressed data, was "winnie-0.0.5.tar", last modified: Mon Jun 19 15:27:27 2023, max compression
```

## Comparing `winnie-0.0.4.tar` & `winnie-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.248094 winnie-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 21:08:43.248094 winnie-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 21:08:30.000000 winnie-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 21:08:30.000000 winnie-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 21:08:43.248094 winnie-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 21:08:30.000000 winnie-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.244094 winnie-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.244094 winnie-0.0.4/src/winnie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/listops.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 21:08:30.000000 winnie-0.0.4/src/winnie/resourceMask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.248094 winnie-0.0.4/src/winnie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 21:08:43.000000 winnie-0.0.4/src/winnie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:08:43.248094 winnie-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 21:08:30.000000 winnie-0.0.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 15:27:27.865940 winnie-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 15:27:11.000000 winnie-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 15:27:11.000000 winnie-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-19 15:27:27.865940 winnie-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 15:27:11.000000 winnie-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.861940 winnie-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/src/winnie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/resourceMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-19 15:27:11.000000 winnie-0.0.5/src/winnie/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/src/winnie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 15:27:27.000000 winnie-0.0.5/src/winnie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:27:27.865940 winnie-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 15:27:11.000000 winnie-0.0.5/tests/test_main.py
```

### Comparing `winnie-0.0.4/PKG-INFO` & `winnie-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.4
+Version: 0.0.5
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `winnie-0.0.4/setup.cfg` & `winnie-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = winnie
-version = v0.0.4
+version = v0.0.5
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = CCP library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/winnie
 project_urls =
```

### Comparing `winnie-0.0.4/src/winnie/connection.py` & `winnie-0.0.5/src/winnie/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,108 @@
 from canlib import canlib, Frame
 from typing import List, Tuple
 from winnie import listops
 from winnie import resourceMask as rm
 from winnie import formatting
+from winnie import verification
  
 class Connection:
 	def __init__(self, channel: canlib.Channel, id: int, debug: bool = False):
 		self.connected = False
 		self.channel = channel
 		self.counter = 0
 		self.id = id
 		self.debug = debug
+	
+	def sendFrame(self, frame: Frame) -> bytearray:
+		self.channel.write(frame)
+		self.channel.writeSync(timeout=500)
+		result = self.channel.read(timeout=500)
+		return result.data
 
-	def sendMessage(self, message: List[int]) -> List[int]:
+	def sendMessage(self, message: bytearray) -> bytearray:
 		if self.debug == True:
-			formatting.printHexList("Message: ", message)
+			formatting.printByteArrayWithLabel("Message: ", message)
 		if self.connected == False and message[0] != 0x01:
 			raise RuntimeError("Connection must be established before sending a message")
-		# Ensure that the message is 8 bytes long
-		if len(message) != 8:
-			raise ValueError("Messages must be 8 bytes long")
+		verification.verifyMessage(message)
 		# Construct and send the frame
 		frame = Frame(id_=self.id, data=message)
-		self.channel.write(frame)
-		self.channel.writeSync(timeout=500)
-		# Get the result and increment the counter
-		result = self.channel.read(timeout=500)
-		response = [x for x in result.data]
+		result = self.sendFrame(frame)
 		if self.debug == True:
-			formatting.printHexList("Response: ", response)
+			formatting.printByteArrayWithLabel("Response: ", result)
 
 		currentCounter = self.counter
 		self.counter += 0x01
+		verification.verifyResponse(result, currentCounter)
 
-		# Verify that the command counter of the response matches the one of the command
-		if response[0] == 0xFF or response[0] == 0xFE:
-			if response[2] != currentCounter:
-				raise RuntimeError("Message counter in response does not match")
-
-		return response, currentCounter
-
-	def checkForAcknowledgement(self, message: List[int]) -> bool:
-		if message[0] == 0xFF and message[1] == 0x00:
-			return True
-		else:
-			return False
+		return result, currentCounter
 
 	def connect(self, stationID: int) -> bool:
 		if self.debug == True:
 			print("CONNECT")
 
 		splitID = listops.splitNumberByBytes(stationID, bigEndian=False)
-		message = [0x01, self.counter, splitID[0], splitID[1], 0, 0, 0, 0]
+		message = bytearray([0x01, self.counter, splitID[0], splitID[1], 0, 0, 0, 0])
 		response, msgCounter = self.sendMessage(message)
 		if self.checkForAcknowledgement(response) == True:
 			self.connected = True
 			return True
 		else:
 			raise RuntimeError("Connection failed")
 	
-	def disconnect(self, stationID, temporary=False) -> bool:
+	def disconnect(self, stationID: int, temporary=False) -> bool:
 		if self.debug == True:
 			print("DISCONNECT")
 
 		splitID = listops.splitNumberByBytes(stationID, bigEndian=False)
 		temporaryByte = 0x01
 		if temporary == True:
 			temporaryByte = 0x00
-		message = [0x07, self.counter, temporaryByte, 0, splitID[0], splitID[1], 0, 0]
+		message = bytearray([0x07, self.counter, temporaryByte, 0, splitID[0], splitID[1], 0, 0])
 		response, msgCounter = self.sendMessage(message)
 		if self.checkForAcknowledgement(response) == True:
 			self.connected = False
 			return True
 		else:
 			raise RuntimeError("Disconnect failed")
 	
 	def exchangeID(self) -> Tuple[rm.ResourceMask, rm.ResourceMask]:
 		if self.debug == True:
 			print("EXCHANGE_ID")
 
-		message = [0x17, self.counter, 0, 0, 0, 0, 0, 0]
+		message = bytearray([0x17, self.counter, 0, 0, 0, 0, 0, 0])
 		response, msgCounter = self.sendMessage(message)
 		# Initialise two resource mask objects
 		availabilityMask = rm.ResourceMask(False, False, False)
 		protectionMask = rm.ResourceMask(False, False, False)
 		# Put in the data from the response
 		availabilityMask.setFromInteger(response[5])
 		protectionMask.setFromInteger(response[6])
 		return availabilityMask, protectionMask
 
 	def getSeed(self, resourceMask: rm.ResourceMask) -> List[int]:
 		if self.debug == True:
 			print("GET_SEED")
 
-		message = [0x12, self.counter, resourceMask.getInteger(), 0, 0, 0, 0, 0]
+		message = bytearray([0x12, self.counter, resourceMask.getInteger(), 0, 0, 0, 0, 0])
 		response, msgCounter = self.sendMessage(message)
-		if response[0] != 0xFF:
-			raise RuntimeError(f"Expected packet id 0xFF, received packed ID {response[0]:#x}")
-		if response[1] != 0x00:
-			raise RuntimeError(f"GET_SEED message responded with error code {response[1]:#x}")
 		return response[4:]
 
-	def unlock(self, key: Tuple[int, int, int, int, int, int]) -> rm.ResourceMask:
+	def unlock(self, key: bytearray) -> rm.ResourceMask:
 		if self.debug == True:
 			print("UNLOCK")
-
-		message = [0x13, self.counter]
+		if len(key) != 6:
+			raise ValueError(f"Key must be 6 bytes long, was {len(key)} bytes long")
+		message = bytearray([0x13, self.counter])
 		message.extend(key)
 		response, msgCounter = self.sendMessage(message)
-		if self.checkForAcknowledgement(response) == True:
-			result = rm.ResourceMask(False, False, False)
-			result.setFromInteger(response[3])
-			return result
-		else:
-			raise RuntimeError("UNLOCK failed")
+		result = rm.ResourceMask(False, False, False)
+		result.setFromInteger(response[3])
+		return result
 
 	def setMemoryTransferAddress(self, mtaNumber: int, extension: int, address: int) -> bool:
 		if self.debug == True:
 			print("SET_MTA")
 
 		if mtaNumber != 0 and mtaNumber != 1:
 			raise ValueError("Memory transfer address number must be 0 or 1")
@@ -125,55 +110,45 @@
 		message = [0x02, self.counter, mtaNumber, extension]
 		message.extend(listops.splitNumberByBytes(address, bigEndian=True))
 		# Add leading 0s to address if necessary (this is why we need to switch to byte arrays)
 		if len(message) < 8:
 			zerosToAdd = 8 - len(message)
 			message = message[:4] + [0] * zerosToAdd + message[4:]
 		# Send message and handle response
+		message = bytearray(message)
 		response, msgCounter = self.sendMessage(message)
-		if self.checkForAcknowledgement(response) == True:
-			return True
-		else:
-			raise RuntimeError("SET_MTA failed")
+		return True
 
-	def upload(self, blockSize: int) -> List[int]:
+	def upload(self, blockSize: int) -> bytearray:
 		if self.debug == True:
 			print("UPLOAD")
 
 		if blockSize > 5:
 			raise ValueError("Block size must be 5 bytes or less")
-		message = [0x04, self.counter, blockSize, 0, 0, 0, 0, 0]
+		message = bytearray([0x04, self.counter, blockSize, 0, 0, 0, 0, 0])
 		response, msgCounter = self.sendMessage(message)
-		if self.checkForAcknowledgement(response) == True:
-			return response[3:3+blockSize]
-		else:
-			raise ValueError("UPLOAD failed")
+		return response[3:3+blockSize]
 	
 	def getCCPVersion(self, mainVersion: int, release: int) -> Tuple[int, int]:
 		if self.debug == True:
 			print("GET_CCP_VERSION")
 
-		message = [0x1B, self.counter, mainVersion, release, 0, 0, 0, 0]
+		message = bytearray([0x1B, self.counter, mainVersion, release, 0, 0, 0, 0])
 		response, msgCounter = self.sendMessage(message)
-		if self.checkForAcknowledgement(response) == True:
-			returnedMainVersion = response[3]
-			returnedRelease = response[4]
-			return returnedMainVersion, returnedRelease
-		else:
-			raise RuntimeError("GET_CCP_VERSION failed")
-	
-	def download(self, data: List[int]) -> Tuple[int, int]:
+		returnedMainVersion = int(response[3])
+		returnedRelease = int(response[4])
+		return returnedMainVersion, returnedRelease
+
+	def download(self, data: bytearray) -> Tuple[int, int]:
 		if self.debug == True:
 			print("DOWNLOAD")
 
 		dataLength = len(data)
 		if dataLength > 5:
 			raise ValueError("Data must be 5 bytes or less")
-		message = [0x03, self.counter, dataLength]
+		message = bytearray([0x03, self.counter, dataLength])
 		message.extend(data)
 		message = listops.padToLength(message, 8, padding=0)
 		response, msgCounter = self.sendMessage(message)
-		if self.checkForAcknowledgement(response) == True:
-			raise RuntimeError("Download failed")
-		newExtension = response[3]
-		newAddress = listops.listToInt(response[4:8])
+		newExtension = int(response[3])
+		newAddress = listops.listToInt(list(response[4:8]))
 		return newExtension, newAddress
```

### Comparing `winnie-0.0.4/src/winnie/listops.py` & `winnie-0.0.5/src/winnie/listops.py`

 * *Files identical despite different names*

### Comparing `winnie-0.0.4/src/winnie.egg-info/PKG-INFO` & `winnie-0.0.5/src/winnie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winnie
-Version: 0.0.4
+Version: 0.0.5
 Summary: CCP library
 Home-page: https://github.com/HWRacing/winnie
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/winnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

