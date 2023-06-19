# Comparing `tmp/dnsrobocert-3.9.0.tar.gz` & `tmp/dnsrobocert-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnsrobocert-3.9.0.tar", max compression
+gzip compressed data, was "dnsrobocert-3.9.1.tar", max compression
```

## Comparing `dnsrobocert-3.9.0.tar` & `dnsrobocert-3.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2021-03-21 17:29:45.134312 dnsrobocert-3.9.0/LICENSE
--rw-r--r--   0        0        0     6034 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/README.rst
--rw-r--r--   0        0        0     1870 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/pyproject.toml
--rw-r--r--   0        0        0      259 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/__init__.py
--rw-r--r--   0        0        0        0 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/__init__.py
--rw-r--r--   0        0        0     1713 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/background.py
--rw-r--r--   0        0        0     4479 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/certbot.py
--rw-r--r--   0        0        0     3474 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/challenge.py
--rw-r--r--   0        0        0     6001 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/config.py
--rw-r--r--   0        0        0     7696 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/hooks.py
--rw-r--r--   0        0        0     9780 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/legacy.py
--rw-r--r--   0        0        0     4964 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/main.py
--rw-r--r--   0        0        0     6648 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/core/utils.py
--rw-r--r--   0        0        0     3843 2021-03-21 17:29:45.138312 dnsrobocert-3.9.0/src/dnsrobocert/schema.yml
--rw-r--r--   0        0        0     7373 2021-03-21 17:29:58.237722 dnsrobocert-3.9.0/setup.py
--rw-r--r--   0        0        0     7779 2021-03-21 17:29:58.238366 dnsrobocert-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-05-02 07:09:07.783386 dnsrobocert-3.9.1/LICENSE
+-rw-r--r--   0        0        0     6034 2021-05-02 07:09:07.783386 dnsrobocert-3.9.1/README.rst
+-rw-r--r--   0        0        0     1875 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0      259 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/__init__.py
+-rw-r--r--   0        0        0     1713 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/background.py
+-rw-r--r--   0        0        0     4479 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/certbot.py
+-rw-r--r--   0        0        0     3474 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/challenge.py
+-rw-r--r--   0        0        0     6001 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/config.py
+-rw-r--r--   0        0        0     7696 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/hooks.py
+-rw-r--r--   0        0        0     9780 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/legacy.py
+-rw-r--r--   0        0        0     4964 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/main.py
+-rw-r--r--   0        0        0     6648 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/core/utils.py
+-rw-r--r--   0        0        0     3843 2021-05-02 07:09:07.787386 dnsrobocert-3.9.1/src/dnsrobocert/schema.yml
+-rw-r--r--   0        0        0     7373 2021-05-02 07:09:22.970651 dnsrobocert-3.9.1/setup.py
+-rw-r--r--   0        0        0     7779 2021-05-02 07:09:22.971345 dnsrobocert-3.9.1/PKG-INFO
```

### Comparing `dnsrobocert-3.9.0/LICENSE` & `dnsrobocert-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/README.rst` & `dnsrobocert-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/pyproject.toml` & `dnsrobocert-3.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dnsrobocert"
-version = "3.9.0"
+version = "3.9.1"
 description = "A tool to manage your DNS-challenged TLS certificates"
 license = "MIT"
 keywords = [
     "dnsrobocert"
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -51,15 +51,15 @@
 boto3 = "*"
 # --
 cryptography = ">=2,<4"
 cffi = "^1"
 lxml = "^4"
 dnspython = "^2"
 jsonschema = "^3"
-pem = "^20"
+pem = ">=20,<22"
 pyopenssl = ">=19,<21"
 pyyaml = "^5"
 schedule = "^0"
 coloredlogs = "^14"
 colorama = "^0"
 tldextract = "^3"
```

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/background.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/background.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/certbot.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/certbot.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/challenge.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/challenge.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/config.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
     with open(config_path) as file_h:
         raw_config = file_h.read()
 
     raw_config = _inject_env_variables(raw_config)
 
     try:
-        config = yaml.load(raw_config, Loader=yaml.FullLoader)
+        config = yaml.load(raw_config, Loader=yaml.SafeLoader)
     except BaseException:
         message = """
 Error while validating dnsrobocert configuration:
 Configuration file is not a valid YAML file.\
 """
         LOGGER.error(message)
         return None
 
     schema_path = pkg_resources.resource_filename("dnsrobocert", "schema.yml")
     with open(schema_path) as file_h:
-        schema = yaml.load(file_h.read(), yaml.FullLoader)
+        schema = yaml.load(file_h.read(), yaml.SafeLoader)
 
     if not config:
         message = """
 Error while validating dnsrobocert configuration:
 Configuration file is empty.\
 """
         LOGGER.error(message)
```

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/hooks.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/hooks.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/legacy.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/legacy.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/main.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/main.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/core/utils.py` & `dnsrobocert-3.9.1/src/dnsrobocert/core/utils.py`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/src/dnsrobocert/schema.yml` & `dnsrobocert-3.9.1/src/dnsrobocert/schema.yml`

 * *Files identical despite different names*

### Comparing `dnsrobocert-3.9.0/setup.py` & `dnsrobocert-3.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'coloredlogs>=14,<15',
  'cryptography>=2,<4',
  'dns-lexicon[full]==3.5.5',
  'dnspython>=2,<3',
  'jsonschema>=3,<4',
  'localzone',
  'lxml>=4,<5',
- 'pem>=20,<21',
+ 'pem>=20,<22',
  'pynamecheap',
  'pyopenssl>=19,<21',
  'pyyaml>=5,<6',
  'schedule>=0,<1',
  'softlayer',
  'tldextract>=3,<4',
  'transip',
@@ -35,15 +35,15 @@
  'zeep']
 
 entry_points = \
 {'console_scripts': ['dnsrobocert = dnsrobocert.core.main:main']}
 
 setup_kwargs = {
     'name': 'dnsrobocert',
-    'version': '3.9.0',
+    'version': '3.9.1',
     'description': 'A tool to manage your DNS-challenged TLS certificates',
     'long_description': '======\n|logo|\n======\n\n|version| |python_support| |docker| |ci| |coverage| |spectrum|\n\n.. |logo| image:: https://adferrand.github.io/dnsrobocert/images/dnsrobocert.svg\n    :alt: DNSroboCert\n.. |version| image:: https://img.shields.io/pypi/v/dnsrobocert\n    :target: https://pypi.org/project/dnsrobocert/\n.. |python_support| image:: https://img.shields.io/pypi/pyversions/dnsrobocert\n    :target: https://pypi.org/project/dnsrobocert/\n.. |docker| image:: https://img.shields.io/docker/image-size/adferrand/dnsrobocert\n    :target: https://microbadger.com/images/adferrand/dnsrobocert\n.. |ci| image:: https://img.shields.io/azure-devops/build/adferrand/338d4cba-ab35-4cf9-a9c6-1d2601554b32/21/master\n    :target: https://dev.azure.com/adferrand/dnsrobocert/_build/latest?definitionId=21&branchName=master\n.. |coverage| image:: https://img.shields.io/azure-devops/coverage/adferrand/338d4cba-ab35-4cf9-a9c6-1d2601554b32/21\n    :target: https://dev.azure.com/adferrand/dnsrobocert/_build?definitionId=21&view=ms.vss-pipelineanalytics-web.new-build-definition-pipeline-analytics-view-cardmetrics\n.. |spectrum| image:: https://withspectrum.github.io/badge/badge.svg\n    :target: https://spectrum.chat/dnsrobocert\n\n.. tag:intro-begin\n\n.. contents:: Table of Contents\n   :local:\n\nFeatures\n========\n\nDNSroboCert is designed to manage `Let\'s Encrypt`_ SSL certificates based on `DNS challenges`_.\n\n* Let\'s Encrypt wildcard and regular certificates generation by Certbot_ using DNS challenges,\n* Integrated automated renewal of almost expired certificates,\n* Standardized API through Lexicon_ library to insert the DNS challenge with various DNS providers,\n* Centralized YAML configuration file to maintain several certificates and several DNS providers\n  with configuration validity control,\n* Modification of container configuration without restart,\n* Flexible hooks upon certificate creation/renewal including containers restart, commands in containers\n  or custom hooks,\n* Support for `DNS alias mode`_ (see the ``follow_cnames`` option in the `certificate section`_),\n* Linux, Mac OS X and Windows support, with a particular care for Docker services,\n* Delivered as a standalone application and a Docker image.\n\n.. _DNS alias mode: https://github.com/acmesh-official/acme.sh/wiki/DNS-alias-mode\n.. _certificate section: https://dnsrobocert.readthedocs.io/en/latest/configuration_reference.html#certificate-properties\n\nWhy use DNSroboCert\n===================\n\nIf you are reading these lines, you certainly want to secure all your services using Let\'s Encrypt SSL\ncertificates, which are free and accepted everywhere.\n\nIf you want to secure Web services through HTTPS, there is already plenty of great tools. In the Docker\nworld, one can check Traefik_, or nginx-proxy_ + letsencrypt-nginx-proxy-companion_. Basically, theses tools\nwill allow automated and dynamic generation/renewal of SSL certificates, based on TLS or HTTP challenges,\non top of a reverse proxy to encrypt everything through HTTPS.\n\nSo far so good, but you may fall in one of the following categories:\n\n1. You are in a firewalled network, and your HTTP/80 and HTTPS/443 ports are not opened to the outside world.\n2. You want to secure non-Web services (like LDAP, IMAP, POP, etc.) were the HTTPS protocol is of no use.\n3. You want to generate a wildcard certificate, valid for any sub-domain of a given domain.\n\nFor the first case, ACME servers need to be able to access your website through HTTP (for HTTP challenges)\nor HTTPS (for TLS challenges) in order to validate the certificate. With a firewall these two challenges -\nwhich are widely used in HTTP proxy approaches - will not be usable: you need to ask a DNS challenge.\nPlease note that traefik embed DNS challenges, but only for few DNS providers.\n\nFor the second case, there is no website to use TLS or HTTP challenges, and you should ask a DNS challenge.\nOf course you could create a "fake" website to validate the domain using a HTTP challenge, and reuse the\ncertificate on the "real" service. But it is a workaround, and you have to implement a logic to propagate\nthe certificate, including during its renewal. Indeed, most of the non-Web services will need to be\nrestarted each time the certificate is renewed.\n\nFor the last case, the use of a DNS challenge is mandatory. Then the problems concerning certificates\npropagation that have been discussed in the second case will also occur.\n\nThe solution is a dedicated and specialized tool which handles the creation/renewal of Let\'s Encrypt\ncertificates, and ensure their propagation in the relevant services. It is the purpose of\nthis project.\n\n.. _Let\'s Encrypt: https://letsencrypt.org/\n.. _DNS challenges: https://tools.ietf.org/html/draft-ietf-acme-acme-01#page-44\n.. _Certbot: https://github.com/certbot/certbot\n.. _Lexicon: https://github.com/AnalogJ/lexicon\n.. _Traefik: https://hub.docker.com/_/traefik/\n.. _nginx-proxy: https://hub.docker.com/r/jwilder/nginx-proxy/\n.. _letsencrypt-nginx-proxy-companion: https://hub.docker.com/r/jrcs/letsencrypt-nginx-proxy-companion/\n\n.. tag:intro-end\n\nDocumentation\n=============\n\nOnline documentation (user guide, configuration reference) is available in the `DNSroboCert documentation`_.\n\nFor a quick start, please have a look in particular at the `User guide`_ and the `Lexicon provider configuration`_.\n\nSupport\n=======\n\nDo not hesitate to join the `DNSroboCert community on Spectrum`_ if you need help to use or develop DNSroboCert!\n\nContributing\n============\n\nIf you want to help in the DNSroboCert development, you are welcome!\nPlease have a look at the `Developer guide`_ page to know how to start.\n\n.. _DNSroboCert documentation: https://dnsrobocert.readthedocs.io\n.. _User guide: https://dnsrobocert.readthedocs.io/en/latest/user_guide.html\n.. _Lexicon provider configuration: https://dnsrobocert.readthedocs.io/en/latest/providers_options.html\n.. _Developer guide: https://dnsrobocert.readthedocs.io/en/latest/developer_guide.html\n.. _DNSroboCert community on Spectrum: https://spectrum.chat/dnsrobocert\n',
     'author': 'Adrien Ferrand',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://dnsrobocert.readthedocs.io',
```

### Comparing `dnsrobocert-3.9.0/PKG-INFO` & `dnsrobocert-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnsrobocert
-Version: 3.9.0
+Version: 3.9.1
 Summary: A tool to manage your DNS-challenged TLS certificates
 Home-page: https://dnsrobocert.readthedocs.io
 License: MIT
 Keywords: dnsrobocert
 Author: Adrien Ferrand
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -30,15 +30,15 @@
 Requires-Dist: coloredlogs (>=14,<15)
 Requires-Dist: cryptography (>=2,<4)
 Requires-Dist: dns-lexicon[full] (==3.5.5)
 Requires-Dist: dnspython (>=2,<3)
 Requires-Dist: jsonschema (>=3,<4)
 Requires-Dist: localzone
 Requires-Dist: lxml (>=4,<5)
-Requires-Dist: pem (>=20,<21)
+Requires-Dist: pem (>=20,<22)
 Requires-Dist: pynamecheap
 Requires-Dist: pyopenssl (>=19,<21)
 Requires-Dist: pyyaml (>=5,<6)
 Requires-Dist: schedule (>=0,<1)
 Requires-Dist: softlayer
 Requires-Dist: tldextract (>=3,<4)
 Requires-Dist: transip
```

