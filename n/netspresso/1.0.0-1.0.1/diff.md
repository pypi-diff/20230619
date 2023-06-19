# Comparing `tmp/netspresso-1.0.0-py3-none-any.whl.zip` & `tmp/netspresso-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 20931 bytes, number of entries: 26
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-14 07:20 netspresso/__init__.py
+Zip file size: 23609 bytes, number of entries: 27
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-19 07:37 netspresso/__init__.py
 -rw-rw-rw-  2.0 fat    23619 b- defN 23-Jun-13 07:57 netspresso/compressor/__init__.py
--rw-rw-rw-  2.0 fat     8456 b- defN 23-Jun-13 06:13 netspresso/compressor/client/__init__.py
--rw-rw-rw-  2.0 fat      535 b- defN 23-Jun-14 07:17 netspresso/compressor/client/config.py
+-rw-rw-rw-  2.0 fat     8479 b- defN 23-Jun-19 05:43 netspresso/compressor/client/__init__.py
+-rw-rw-rw-  2.0 fat      536 b- defN 23-Jun-16 05:06 netspresso/compressor/client/config.py
 -rw-rw-rw-  2.0 fat       41 b- defN 23-Jun-13 06:13 netspresso/compressor/client/configs/config-local.ini
 -rw-rw-rw-  2.0 fat       61 b- defN 23-Jun-13 06:13 netspresso/compressor/client/configs/config-prod.ini
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/__init__.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/auth.py
 -rw-rw-rw-  2.0 fat      482 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/common.py
 -rw-rw-rw-  2.0 fat     4108 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/compression.py
 -rw-rw-rw-  2.0 fat     5681 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/client/utils/__init__.py
--rw-rw-rw-  2.0 fat      533 b- defN 23-Jun-14 07:20 netspresso/compressor/client/utils/common.py
+-rw-rw-rw-  2.0 fat      597 b- defN 23-Jun-19 05:43 netspresso/compressor/client/utils/common.py
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Jun-13 06:13 netspresso/compressor/client/utils/enum.py
+-rw-rw-rw-  2.0 fat      997 b- defN 23-Jun-19 05:43 netspresso/compressor/client/utils/system.py
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-13 06:13 netspresso/compressor/client/utils/validator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/core/__init__.py
 -rw-rw-rw-  2.0 fat     1900 b- defN 23-Jun-13 06:13 netspresso/compressor/core/compression.py
 -rw-rw-rw-  2.0 fat     2966 b- defN 23-Jun-13 06:13 netspresso/compressor/core/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2035 b- defN 23-Jun-13 06:13 netspresso/compressor/utils/model.py
 -rw-rw-rw-  2.0 fat      236 b- defN 23-Jun-13 06:13 netspresso/compressor/utils/token.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-14 07:22 netspresso-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      769 b- defN 23-Jun-14 07:22 netspresso-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 07:22 netspresso-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-14 07:22 netspresso-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2452 b- defN 23-Jun-14 07:22 netspresso-1.0.0.dist-info/RECORD
-26 files, 72856 bytes uncompressed, 16833 bytes compressed:  76.9%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7286 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2553 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/RECORD
+27 files, 80559 bytes uncompressed, 19347 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -36,14 +36,17 @@
 
 Filename: netspresso/compressor/client/utils/common.py
 Comment: 
 
 Filename: netspresso/compressor/client/utils/enum.py
 Comment: 
 
+Filename: netspresso/compressor/client/utils/system.py
+Comment: 
+
 Filename: netspresso/compressor/client/utils/validator.py
 Comment: 
 
 Filename: netspresso/compressor/core/__init__.py
 Comment: 
 
 Filename: netspresso/compressor/core/compression.py
@@ -57,23 +60,23 @@
 
 Filename: netspresso/compressor/utils/model.py
 Comment: 
 
 Filename: netspresso/compressor/utils/token.py
 Comment: 
 
-Filename: netspresso-1.0.0.dist-info/LICENSE
+Filename: netspresso-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: netspresso-1.0.0.dist-info/METADATA
+Filename: netspresso-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: netspresso-1.0.0.dist-info/WHEEL
+Filename: netspresso-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: netspresso-1.0.0.dist-info/top_level.txt
+Filename: netspresso-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: netspresso-1.0.0.dist-info/RECORD
+Filename: netspresso-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netspresso/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

## netspresso/compressor/client/__init__.py

```diff
@@ -24,15 +24,15 @@
         self.ip = self.config.IP
         self.port = self.config.PORT
         self.prefix = self.config.API_PREFIX
         self.url = f"{self.ip}:{self.port}{self.prefix}"
 
     def login(self, data) -> LoginResponse:
         url = f"{self.url}/login"
-        response = requests.post(url, data=data.dict())
+        response = requests.post(url, data=data.dict(), headers=get_headers())
         response_body = json.loads(response.text)
 
         if response.status_code == 200 or response.status_code == 201:
             return LoginResponse(**response_body)
         else:
             raise Exception(response_body["detail"])
```

## netspresso/compressor/client/config.py

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 from loguru import logger
 from pydantic import BaseSettings
 
 BASE_DIR = Path(__file__).resolve().parent
 config = configparser.ConfigParser()
-DEPLOYMENT_MODE = os.getenv("DEPLOYMENT_MODE", "PROD")
+DEPLOYMENT_MODE = os.getenv("DEPLOYMENT_MODE", "LOCAL")
 logger.info(f"Read {DEPLOYMENT_MODE} config")
 config.read(f"{BASE_DIR}/configs/config-{DEPLOYMENT_MODE.lower()}.ini")
 
 
 class Config(BaseSettings):
     API_PREFIX: str = "/api/v2"
     IP: str = config["GENERAL"]["IP"]
```

## netspresso/compressor/client/utils/common.py

```diff
@@ -1,14 +1,16 @@
 from os.path import basename
+
 from netspresso import __version__
+from netspresso.compressor.client.utils.system import ENV_STR
 
 
 def get_headers(access_token=None, json_type=False):
     headers = {
-        "User-Agent": f"NetsPresso Model Compressor API Client v{__version__}",
+        "User-Agent": f"NetsPresso Python Package v{__version__} ({ENV_STR})",
     }
     if access_token:
         headers["Authorization"] = f"Bearer {access_token}"
     if json_type:
         headers["Content-Type"] = "application/json"
     return headers
```

## Comparing `netspresso-1.0.0.dist-info/LICENSE` & `netspresso-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netspresso-1.0.0.dist-info/RECORD` & `netspresso-1.0.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-netspresso/__init__.py,sha256=ZhzQKWZ8RFrTIkj7z87B144DI95e8LMfA5w8NDWQDtg,23
+netspresso/__init__.py,sha256=j9q3lYMZra0QrErNnn9E5GNXxWLOlDgeOkmX8oXa7ro,23
 netspresso/compressor/__init__.py,sha256=4gKZzZCd3BJUSCfLOu8crijVVY7sIVe5qQNZAvjEFpI,23619
-netspresso/compressor/client/__init__.py,sha256=pgYngRDyZBTc3vTDNeZPHpSc86KJ_122J-jdKFArpT0,8456
-netspresso/compressor/client/config.py,sha256=CjYFS5hAQ7ZjUTE0utCKNOboT7LV1FiGKk_FcsrjPXY,535
+netspresso/compressor/client/__init__.py,sha256=c2HyrKbG8gdRvaWSNAy5g_t9uh3hilG9Y2ReB7Bjyo4,8479
+netspresso/compressor/client/config.py,sha256=i3EZTWDZJEq527YY1hiyiSN-DIVQyjE7zgOI7_kLY9Y,536
 netspresso/compressor/client/configs/config-local.ini,sha256=0trP47pxMTnQCy-KAnsVpKbdcr2aJffbnAJDfTxSQu4,41
 netspresso/compressor/client/configs/config-prod.ini,sha256=en_y9NB0Rj3lfU58h4JGK6PPNAusN2hs3mXSMpEQhOQ,61
 netspresso/compressor/client/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/schemas/auth.py,sha256=NGudVfx4Q7E8XppeDgcKmQlU_3UwKDu3YjYiIwsii1g,2644
 netspresso/compressor/client/schemas/common.py,sha256=w1rR-jqIvjQ6UqMRZ5KYWW8bQrlXMSrAdWXCzA3tQuk,482
 netspresso/compressor/client/schemas/compression.py,sha256=0OwRemHeFQy4wZBWHzwcYuf0T2w8fN7Hb39fHWyPM0k,4108
 netspresso/compressor/client/schemas/model.py,sha256=hprc5AQ3gFe8hjtoHEcyKM8HoQCYn53LJwQJ_QsBUHA,5681
 netspresso/compressor/client/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-netspresso/compressor/client/utils/common.py,sha256=WrvHrtNppDvTyvp5Kn1JMOTWIhN0esAcB8jK2z07RxA,533
+netspresso/compressor/client/utils/common.py,sha256=OA7rMfupHq_wnbHjGvwLc6pk1NFNCF5_F0p87bJJPfo,597
 netspresso/compressor/client/utils/enum.py,sha256=RUtiknaDJhfML23sILSHnEvPJ2wBqsLDgId0d_IM0fI,840
+netspresso/compressor/client/utils/system.py,sha256=IQp9qQ6C9RuxBYTbdtVnQ6IacbtNPw6ldDr8_y8OG6s,997
 netspresso/compressor/client/utils/validator.py,sha256=0pONKSTlxTWcpSIiUw3P2ItPARoLXvu5YSGGxhUFPNU,3814
 netspresso/compressor/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/core/compression.py,sha256=OMrI-SsDXmwzZdz_1jRmv30KTGRRluRszJPqcXFQOwU,1900
 netspresso/compressor/core/model.py,sha256=kH0VBvcpwyxO9QsUpaQZXLB-IZXfw3T-mp613qX3_mE,2966
 netspresso/compressor/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/utils/model.py,sha256=tPojNWMvvHTNT8EgLIJfq_3EWIOIb0HuZHDbF1ANBc0,2035
 netspresso/compressor/utils/token.py,sha256=zWKx6olb8N2c3nSQhUS22IRG7ILQZYIERScETEFeUXY,236
-netspresso-1.0.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-netspresso-1.0.0.dist-info/METADATA,sha256=9-jIo1TW0XkeXvkswpaSvSNr4ZLER81sMjn64w1IFC4,769
-netspresso-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netspresso-1.0.0.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
-netspresso-1.0.0.dist-info/RECORD,,
+netspresso-1.0.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+netspresso-1.0.1.dist-info/METADATA,sha256=iLHSxl5iMgOI71UeZUcyVP4NtqEpy_-UpJOQoCvYhnk,7286
+netspresso-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+netspresso-1.0.1.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
+netspresso-1.0.1.dist-info/RECORD,,
```

