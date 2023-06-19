# Comparing `tmp/ocean-contracts-1.1.7.tar.gz` & `tmp/ocean-contracts-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean-contracts-1.1.7.tar", last modified: Fri Sep 23 06:04:21 2022, max compression
+gzip compressed data, was "ocean-contracts-1.1.8.tar", last modified: Sat Oct 22 11:54:43 2022, max compression
```

## Comparing `ocean-contracts-1.1.7.tar` & `ocean-contracts-1.1.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 06:04:21.945456 ocean-contracts-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-09-23 06:04:21.945456 ocean-contracts-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2022-09-23 06:02:01.000000 ocean-contracts-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 06:04:21.937456 ocean-contracts-1.1.7/addresses/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 06:04:13.000000 ocean-contracts-1.1.7/addresses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12288 2022-09-23 06:02:01.000000 ocean-contracts-1.1.7/addresses/address.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 06:04:21.945456 ocean-contracts-1.1.7/artifacts/
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/Address.json
--rw-r--r--   0 runner    (1001) docker     (121)     7529 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BConst.json
--rw-r--r--   0 runner    (1001) docker     (121)    16194 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BFactory.json
--rw-r--r--   0 runner    (1001) docker     (121)    24159 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BMath.json
--rw-r--r--   0 runner    (1001) docker     (121)     7525 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BNum.json
--rw-r--r--   0 runner    (1001) docker     (121)   132390 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BPool.json
--rw-r--r--   0 runner    (1001) docker     (121)    21360 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BToken.json
--rw-r--r--   0 runner    (1001) docker     (121)     8589 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/BTokenBase.json
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/Context.json
--rw-r--r--   0 runner    (1001) docker     (121)    27770 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/DFRewards.json
--rw-r--r--   0 runner    (1001) docker     (121)     7527 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/DFStrategyV1.json
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/Deployer.json
--rw-r--r--   0 runner    (1001) docker     (121)    35597 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/Dispenser.json
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC165.json
--rw-r--r--   0 runner    (1001) docker     (121)     7746 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC20Roles.json
--rw-r--r--   0 runner    (1001) docker     (121)   135304 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC20Template.json
--rw-r--r--   0 runner    (1001) docker     (121)   140357 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC20TemplateEnterprise.json
--rw-r--r--   0 runner    (1001) docker     (121)    21917 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (121)   107431 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC721Factory.json
--rw-r--r--   0 runner    (1001) docker     (121)    27611 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC721RolesAddress.json
--rw-r--r--   0 runner    (1001) docker     (121)   124776 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC721Template.json
--rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ERC725Ocean.json
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/EnumerableMap.json
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/EnumerableSet.json
--rw-r--r--   0 runner    (1001) docker     (121)   108738 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/FactoryRouter.json
--rw-r--r--   0 runner    (1001) docker     (121)    93826 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/FixedRateExchange.json
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IDFRewards.json
--rw-r--r--   0 runner    (1001) docker     (121)     4232 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IDispenser.json
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC165.json
--rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC20.json
--rw-r--r--   0 runner    (1001) docker     (121)    17955 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC20Template.json
--rw-r--r--   0 runner    (1001) docker     (121)     4615 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC721.json
--rw-r--r--   0 runner    (1001) docker     (121)     5767 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC721Enumerable.json
--rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC721Metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC721Receiver.json
--rw-r--r--   0 runner    (1001) docker     (121)    15959 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC721Template.json
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC725X.json
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IERC725Y.json
--rw-r--r--   0 runner    (1001) docker     (121)    13108 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IFactory.json
--rw-r--r--   0 runner    (1001) docker     (121)    10207 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IFactoryRouter.json
--rw-r--r--   0 runner    (1001) docker     (121)    10066 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IFixedRateExchange.json
--rw-r--r--   0 runner    (1001) docker     (121)     7189 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IPool.json
--rw-r--r--   0 runner    (1001) docker     (121)     7179 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/ISideStaking.json
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/IveOCEAN.json
--rw-r--r--   0 runner    (1001) docker     (121)    16901 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/MockERC20.json
--rw-r--r--   0 runner    (1001) docker     (121)    17199 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/MockERC20Decimals.json
--rw-r--r--   0 runner    (1001) docker     (121)     4493 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/MockExchange.json
--rw-r--r--   0 runner    (1001) docker     (121)    16167 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/MockOcean.json
--rw-r--r--   0 runner    (1001) docker     (121)    40109 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/MockOldDT.json
--rw-r--r--   0 runner    (1001) docker     (121)    11940 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/OPFCommunityFeeCollector.json
--rw-r--r--   0 runner    (1001) docker     (121)    24521 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/OceanToken.json
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/Ownable.json
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/SafeERC20.json
--rw-r--r--   0 runner    (1001) docker     (121)    49721 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/SideStaking.json
--rw-r--r--   0 runner    (1001) docker     (121)     5041 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/SmartWalletChecker.json
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/Strings.json
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/UtilsLib.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 06:04:13.000000 ocean-contracts-1.1.7/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11817 2022-09-23 06:03:17.000000 ocean-contracts-1.1.7/artifacts/veAllocate.json
--rw-r--r--   0 runner    (1001) docker     (121)    94495 2022-09-23 06:03:57.000000 ocean-contracts-1.1.7/artifacts/veDelegation.json
--rw-r--r--   0 runner    (1001) docker     (121)     8283 2022-09-23 06:03:59.000000 ocean-contracts-1.1.7/artifacts/veDelegationProxy.json
--rw-r--r--   0 runner    (1001) docker     (121)    40977 2022-09-23 06:04:02.000000 ocean-contracts-1.1.7/artifacts/veFeeDistributor.json
--rw-r--r--   0 runner    (1001) docker     (121)    13523 2022-09-23 06:04:02.000000 ocean-contracts-1.1.7/artifacts/veFeeEstimate.json
--rw-r--r--   0 runner    (1001) docker     (121)    66452 2022-09-23 06:04:09.000000 ocean-contracts-1.1.7/artifacts/veOCEAN.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 06:04:21.945456 ocean-contracts-1.1.7/ocean_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-09-23 06:04:21.000000 ocean-contracts-1.1.7/ocean_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-09-23 06:04:21.000000 ocean-contracts-1.1.7/ocean_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 06:04:21.000000 ocean-contracts-1.1.7/ocean_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-23 06:04:21.000000 ocean-contracts-1.1.7/ocean_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-23 06:02:01.000000 ocean-contracts-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-09-23 06:04:21.945456 ocean-contracts-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 11:54:43.390120 ocean-contracts-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-10-22 11:54:43.390120 ocean-contracts-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5013 2022-10-22 11:52:57.000000 ocean-contracts-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 11:54:43.382120 ocean-contracts-1.1.8/addresses/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 11:54:36.000000 ocean-contracts-1.1.8/addresses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-10-22 11:52:57.000000 ocean-contracts-1.1.8/addresses/address.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 11:54:43.390120 ocean-contracts-1.1.8/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/Address.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7529 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BConst.json
+-rw-r--r--   0 runner    (1001) docker     (121)    16194 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BFactory.json
+-rw-r--r--   0 runner    (1001) docker     (121)    24159 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BMath.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7525 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BNum.json
+-rw-r--r--   0 runner    (1001) docker     (121)   132390 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BPool.json
+-rw-r--r--   0 runner    (1001) docker     (121)    21360 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BToken.json
+-rw-r--r--   0 runner    (1001) docker     (121)     8589 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/BTokenBase.json
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/Context.json
+-rw-r--r--   0 runner    (1001) docker     (121)    27770 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/DFRewards.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7527 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/DFStrategyV1.json
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/Deployer.json
+-rw-r--r--   0 runner    (1001) docker     (121)    35597 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/Dispenser.json
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC165.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7746 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC20Roles.json
+-rw-r--r--   0 runner    (1001) docker     (121)   135304 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC20Template.json
+-rw-r--r--   0 runner    (1001) docker     (121)   140357 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC20TemplateEnterprise.json
+-rw-r--r--   0 runner    (1001) docker     (121)    21917 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (121)   107431 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC721Factory.json
+-rw-r--r--   0 runner    (1001) docker     (121)    27611 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC721RolesAddress.json
+-rw-r--r--   0 runner    (1001) docker     (121)   124776 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC721Template.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ERC725Ocean.json
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/EnumerableMap.json
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/EnumerableSet.json
+-rw-r--r--   0 runner    (1001) docker     (121)   108738 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/FactoryRouter.json
+-rw-r--r--   0 runner    (1001) docker     (121)    93826 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/FixedRateExchange.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IDFRewards.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4232 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IDispenser.json
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC165.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC20.json
+-rw-r--r--   0 runner    (1001) docker     (121)    17955 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC20Template.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4615 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC721.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5767 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC721Enumerable.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC721Metadata.json
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC721Receiver.json
+-rw-r--r--   0 runner    (1001) docker     (121)    15959 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC721Template.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC725X.json
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IERC725Y.json
+-rw-r--r--   0 runner    (1001) docker     (121)    13108 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IFactory.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10207 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IFactoryRouter.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10066 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IFixedRateExchange.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7189 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IPool.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7179 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/ISideStaking.json
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/IveOCEAN.json
+-rw-r--r--   0 runner    (1001) docker     (121)    16901 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/MockERC20.json
+-rw-r--r--   0 runner    (1001) docker     (121)    17199 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/MockERC20Decimals.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4493 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/MockExchange.json
+-rw-r--r--   0 runner    (1001) docker     (121)    16167 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/MockOcean.json
+-rw-r--r--   0 runner    (1001) docker     (121)    40109 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/MockOldDT.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11940 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/OPFCommunityFeeCollector.json
+-rw-r--r--   0 runner    (1001) docker     (121)    24521 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/OceanToken.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/Ownable.json
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/SafeERC20.json
+-rw-r--r--   0 runner    (1001) docker     (121)    49721 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/SideStaking.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5041 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/SmartWalletChecker.json
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/Strings.json
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-10-22 11:53:54.000000 ocean-contracts-1.1.8/artifacts/UtilsLib.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 11:54:36.000000 ocean-contracts-1.1.8/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11817 2022-10-22 11:53:55.000000 ocean-contracts-1.1.8/artifacts/veAllocate.json
+-rw-r--r--   0 runner    (1001) docker     (121)    94495 2022-10-22 11:54:24.000000 ocean-contracts-1.1.8/artifacts/veDelegation.json
+-rw-r--r--   0 runner    (1001) docker     (121)     8283 2022-10-22 11:54:26.000000 ocean-contracts-1.1.8/artifacts/veDelegationProxy.json
+-rw-r--r--   0 runner    (1001) docker     (121)    40977 2022-10-22 11:54:29.000000 ocean-contracts-1.1.8/artifacts/veFeeDistributor.json
+-rw-r--r--   0 runner    (1001) docker     (121)    14728 2022-10-22 11:54:29.000000 ocean-contracts-1.1.8/artifacts/veFeeEstimate.json
+-rw-r--r--   0 runner    (1001) docker     (121)    66452 2022-10-22 11:54:34.000000 ocean-contracts-1.1.8/artifacts/veOCEAN.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 11:54:43.390120 ocean-contracts-1.1.8/ocean_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-10-22 11:54:43.000000 ocean-contracts-1.1.8/ocean_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-10-22 11:54:43.000000 ocean-contracts-1.1.8/ocean_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 11:54:43.000000 ocean-contracts-1.1.8/ocean_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-22 11:54:43.000000 ocean-contracts-1.1.8/ocean_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-22 11:52:57.000000 ocean-contracts-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-10-22 11:54:43.390120 ocean-contracts-1.1.8/setup.cfg
```

### Comparing `ocean-contracts-1.1.7/PKG-INFO` & `ocean-contracts-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-contracts
-Version: 1.1.7
+Version: 1.1.8
 Summary: 🐳 Ocean Protocol L1 - v4
 Home-page: https://github.com/oceanprotocol/contracts
 Author: leucothia
 Author-email: devops@oceanprotocol.com
 Project-URL: Bug Tracker, https://github.com/oceanprotocol/contracts/issues
 Keywords: ocean-contracts
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ocean-contracts-1.1.7/README.md` & `ocean-contracts-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/addresses/address.json` & `ocean-contracts-1.1.8/addresses/address.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8323412698412698%*

 * *Differences: {"'mainnet'": "{'veFeeEstimate': '0x4aA261bC595abC6fDEf0255C83e2a9305261753f'}",*

 * * 'delete': "['rinkeby', 'ropsten']"}*

```diff
@@ -106,15 +106,15 @@
         "chainId": 1,
         "poolTemplate": "0x8daC419D5D81Af8c8E795D0D73f64d5220e28cd8",
         "startBlock": 14907021,
         "veAllocate": "0x55567E038b0a50283084ae773FA433a5029822d3",
         "veDelegation": "0xc768eDF2d21fe00ef5804A7Caa775E877e65A70E",
         "veDelegationProxy": "0x45E3BEc7D139Cd8Ed7FeB161F3B094688ddB0c20",
         "veFeeDistributor": "0x256c54219816603BB8327F9019533B020a76e936",
-        "veFeeEstimate": "0xe97a787420eD263583689Bd35B7Db1952A94710d",
+        "veFeeEstimate": "0x4aA261bC595abC6fDEf0255C83e2a9305261753f",
         "veOCEAN": "0xE86Bf3B0D3a20444DE7c78932ACe6e5EfFE92379"
     },
     "moonbase": {
         "Dispenser": "0x04706CA5d439b342449f0F483b0da0E7B70CC1ef",
         "ERC20Template": {
             "1": "0xa15024b732A8f2146423D14209eFd074e61964F3",
             "2": "0x5ee92aD0760e380501780e2c11c16451F4d3E81C"
@@ -214,55 +214,9 @@
         "FixedPrice": "0xfa48673a7C36A2A768f89AC1ee8C355D5c367B02",
         "OPFCommunityFeeCollector": "0x8daC419D5D81Af8c8E795D0D73f64d5220e28cd8",
         "Ocean": "0x8c98ea273bA22327F896Aa1a1a46E1BFf56e9b1D",
         "Router": "0x8149276f275EEFAc110D74AFE8AFECEaeC7d1593",
         "Staking": "0x7842Fa3B2d87Ff1cd52C4152382f7C4B3406E5A6",
         "chainId": 81001,
         "startBlock": 3256707
-    },
-    "rinkeby": {
-        "DFRewards": "0xD09BCDC099D635A0D8A7f003DC01F645382B6700",
-        "DFStrategyV1": "0x2Fe41338f11d7402E31A4b902F60077164C65a52",
-        "Dispenser": "0xCdbdDFeac752EC993e14bF07424D324B6B6959F2",
-        "ERC20Template": {
-            "1": "0xA0EAB6A2D6880AB37906EA5446D9085426f076E9",
-            "2": "0xF7266F51c0Cb9352aB639E9ce001a9b03316d1fE"
-        },
-        "ERC721Factory": "0x465069D3d6Ec45CDB006ec3E22cC9E8d6f9793eF",
-        "ERC721Template": {
-            "1": "0x2A1D7746BecA3910e2FaCfd26060B9960B4CD9ED"
-        },
-        "FixedPrice": "0x65Ee19cd86dE140fE08Bfd5d51e62Fe53e96358f",
-        "OPFCommunityFeeCollector": "0x39b50501c22578D084191d7E91cfDd1068A4e163",
-        "Ocean": "0x8967bcf84170c91b0d24d4302c2376283b0b3a07",
-        "Router": "0x4d3232171465C9F19b937b5ffBd25876345C8EfE",
-        "Staking": "0x651e859510A219f6CAd57E23926CdE6B9eaee822",
-        "chainId": 4,
-        "poolTemplate": "0x41016a5a0a21B24C5c8C3ae119902a5bF5999bE2",
-        "startBlock": 10693767,
-        "veAllocate": "0xbB7E22Ed79563daDb33BeDc16080DF02B62a1CE4",
-        "veDelegation": "0x15A278BaabC9EE66737562E35B3a42F77a48Fa79",
-        "veDelegationProxy": "0x7b886fa12a9b11BD0cb83e79398070CD635BcBdF",
-        "veFeeDistributor": "0xB99BAA8D5b131c9140Be2F13EA6D2494DF272919",
-        "veFeeEstimate": "0xE98Cf50B7793C120446433Ee551C39Fcc47fDe47",
-        "veOCEAN": "0x57cD87bb197B74Df44Fd69177c0550B9a0C04619"
-    },
-    "ropsten": {
-        "Dispenser": "0x660B3832e940E4bb4FfbDAA0aAB9E9B8D524C7Ef",
-        "ERC20Template": {
-            "1": "0x4F20213DB5c9dE28E51f1f557663A38fce790b3d",
-            "2": "0xe8AC04c7c6c3bD68a06D3C58F483696fE23D9dB8"
-        },
-        "ERC721Factory": "0xB0F8c68eF94ACB8E976b1dED6351Cc62e383d253",
-        "ERC721Template": {
-            "1": "0x101fd973F488c40DC57305CFED84bB2a2C8A7D6E"
-        },
-        "FixedPrice": "0x1909A3cBfE0766e7bce8cC0d4927bcFDC6591cd2",
-        "OPFCommunityFeeCollector": "0x0bA762E1b4F5772AfBb7c9A734bE0C9164ab2a30",
-        "Ocean": "0x5e8DCB2AfA23844bcc311B00Ad1A0C30025aADE9",
-        "Router": "0x41aC3dC16cb9603d5E9379dcDc5fAaa13c114ceE",
-        "Staking": "0x56b922b71D281Ef0638C6e28015f8f7A1c195B76",
-        "chainId": 3,
-        "poolTemplate": "0x6B9FeB968947C92e35BE4c16152b7694E906FB06",
-        "startBlock": 12274186
     }
 }
```

### Comparing `ocean-contracts-1.1.7/artifacts/Address.json` & `ocean-contracts-1.1.8/artifacts/Address.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BConst.json` & `ocean-contracts-1.1.8/artifacts/BConst.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BFactory.json` & `ocean-contracts-1.1.8/artifacts/BFactory.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BMath.json` & `ocean-contracts-1.1.8/artifacts/BMath.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BNum.json` & `ocean-contracts-1.1.8/artifacts/BNum.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BPool.json` & `ocean-contracts-1.1.8/artifacts/BPool.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BToken.json` & `ocean-contracts-1.1.8/artifacts/BToken.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/BTokenBase.json` & `ocean-contracts-1.1.8/artifacts/BTokenBase.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/DFRewards.json` & `ocean-contracts-1.1.8/artifacts/DFRewards.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/DFStrategyV1.json` & `ocean-contracts-1.1.8/artifacts/DFStrategyV1.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/Deployer.json` & `ocean-contracts-1.1.8/artifacts/Deployer.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/Dispenser.json` & `ocean-contracts-1.1.8/artifacts/Dispenser.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC165.json` & `ocean-contracts-1.1.8/artifacts/ERC165.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC20Roles.json` & `ocean-contracts-1.1.8/artifacts/ERC20Roles.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC20Template.json` & `ocean-contracts-1.1.8/artifacts/ERC20Template.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC20TemplateEnterprise.json` & `ocean-contracts-1.1.8/artifacts/ERC20TemplateEnterprise.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC721.json` & `ocean-contracts-1.1.8/artifacts/ERC721.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC721Factory.json` & `ocean-contracts-1.1.8/artifacts/ERC721Factory.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC721RolesAddress.json` & `ocean-contracts-1.1.8/artifacts/ERC721RolesAddress.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC721Template.json` & `ocean-contracts-1.1.8/artifacts/ERC721Template.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ERC725Ocean.json` & `ocean-contracts-1.1.8/artifacts/ERC725Ocean.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/EnumerableMap.json` & `ocean-contracts-1.1.8/artifacts/EnumerableMap.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/EnumerableSet.json` & `ocean-contracts-1.1.8/artifacts/EnumerableSet.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/FactoryRouter.json` & `ocean-contracts-1.1.8/artifacts/FactoryRouter.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/FixedRateExchange.json` & `ocean-contracts-1.1.8/artifacts/FixedRateExchange.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IDFRewards.json` & `ocean-contracts-1.1.8/artifacts/IDFRewards.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IDispenser.json` & `ocean-contracts-1.1.8/artifacts/IDispenser.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC165.json` & `ocean-contracts-1.1.8/artifacts/IERC165.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC20.json` & `ocean-contracts-1.1.8/artifacts/IERC20.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC20Template.json` & `ocean-contracts-1.1.8/artifacts/IERC20Template.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC721.json` & `ocean-contracts-1.1.8/artifacts/IERC721.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC721Enumerable.json` & `ocean-contracts-1.1.8/artifacts/IERC721Enumerable.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC721Metadata.json` & `ocean-contracts-1.1.8/artifacts/IERC721Metadata.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC721Receiver.json` & `ocean-contracts-1.1.8/artifacts/IERC721Receiver.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC721Template.json` & `ocean-contracts-1.1.8/artifacts/IERC721Template.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC725X.json` & `ocean-contracts-1.1.8/artifacts/IERC725X.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IERC725Y.json` & `ocean-contracts-1.1.8/artifacts/IERC725Y.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IFactory.json` & `ocean-contracts-1.1.8/artifacts/IFactory.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IFactoryRouter.json` & `ocean-contracts-1.1.8/artifacts/IFactoryRouter.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IFixedRateExchange.json` & `ocean-contracts-1.1.8/artifacts/IFixedRateExchange.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IPool.json` & `ocean-contracts-1.1.8/artifacts/IPool.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/ISideStaking.json` & `ocean-contracts-1.1.8/artifacts/ISideStaking.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/IveOCEAN.json` & `ocean-contracts-1.1.8/artifacts/IveOCEAN.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/MockERC20.json` & `ocean-contracts-1.1.8/artifacts/MockERC20.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/MockERC20Decimals.json` & `ocean-contracts-1.1.8/artifacts/MockERC20Decimals.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/MockExchange.json` & `ocean-contracts-1.1.8/artifacts/MockExchange.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/MockOcean.json` & `ocean-contracts-1.1.8/artifacts/MockOcean.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/MockOldDT.json` & `ocean-contracts-1.1.8/artifacts/MockOldDT.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/OPFCommunityFeeCollector.json` & `ocean-contracts-1.1.8/artifacts/OPFCommunityFeeCollector.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/OceanToken.json` & `ocean-contracts-1.1.8/artifacts/OceanToken.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/Ownable.json` & `ocean-contracts-1.1.8/artifacts/Ownable.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/SafeERC20.json` & `ocean-contracts-1.1.8/artifacts/SafeERC20.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/SideStaking.json` & `ocean-contracts-1.1.8/artifacts/SideStaking.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/SmartWalletChecker.json` & `ocean-contracts-1.1.8/artifacts/SmartWalletChecker.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/Strings.json` & `ocean-contracts-1.1.8/artifacts/Strings.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/UtilsLib.json` & `ocean-contracts-1.1.8/artifacts/UtilsLib.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/veAllocate.json` & `ocean-contracts-1.1.8/artifacts/veAllocate.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/veDelegation.json` & `ocean-contracts-1.1.8/artifacts/veDelegation.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/veDelegationProxy.json` & `ocean-contracts-1.1.8/artifacts/veDelegationProxy.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/veFeeDistributor.json` & `ocean-contracts-1.1.8/artifacts/veFeeDistributor.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/artifacts/veFeeEstimate.json` & `ocean-contracts-1.1.8/artifacts/veFeeEstimate.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.859375%*

 * *Differences: {"'abi'": "{2: {'gas': 693987}, 3: {'gas': 1211}, 4: {'gas': 1241}, insert: [(1, "*

 * *          "OrderedDict([('name', 'estimateClaimAcc'), ('outputs', [OrderedDict([('type', "*

 * *          "'uint256'), ('name', '')])]), ('inputs', [OrderedDict([('type', 'address'), ('name', "*

 * *          "'addr')])]), ('stateMutability', 'view'), ('type', 'function'), ('gas', 696611)]))]}",*

 * * "'bytecode'": "'0x6f7fffffffffffffffffffffffffffffff6040526040610cfe610140396020610cfe60c03960c05160a01c1561003457600080fd5b60206020610cfe016 […]*

```diff
@@ -13,15 +13,33 @@
                 }
             ],
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "constructor"
         },
         {
-            "gas": 442703,
+            "gas": 696611,
+            "inputs": [
+                {
+                    "name": "addr",
+                    "type": "address"
+                }
+            ],
+            "name": "estimateClaimAcc",
+            "outputs": [
+                {
+                    "name": "",
+                    "type": "uint256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "gas": 693987,
             "inputs": [
                 {
                     "name": "addr",
                     "type": "address"
                 }
             ],
             "name": "estimateClaim",
@@ -31,40 +49,40 @@
                     "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "gas": 1151,
+            "gas": 1211,
             "inputs": [],
             "name": "voting_escrow",
             "outputs": [
                 {
                     "name": "",
                     "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "gas": 1181,
+            "gas": 1241,
             "inputs": [],
             "name": "fee_distributor",
             "outputs": [
                 {
                     "name": "",
                     "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         }
     ],
-    "bytecode": "0x6f7fffffffffffffffffffffffffffffff6040526040610c22610140396020610c2260c03960c05160a01c1561003457600080fd5b60206020610c220160c03960c05160a01c1561004f57600080fd5b6101405160005561016051600155610c0a56341561000a57600080fd5b600436101561001857610ba2565b600035601c526f7fffffffffffffffffffffffffffffff6040526000156101ed575b61018052610140526101605260006101a0526020610240600463900cf0cf6101e0526101fc610140515afa61006e57600080fd5b601f3d1161007b57600080fd5b600050610240516101c0526101e060006080818352015b6101c0516101a0511015156100a6576101d9565b6101a0516101c0518181830110156100bd57600080fd5b8082019050905060028181830110156100d557600080fd5b80820190509050600280820490509050610200526102206080610320602463d1febfb96102a052610200516102c0526102bc610140515afa61011657600080fd5b607f3d1161012357600080fd5b61032080808080516103a0525050602081019050808080516103c0525050602081019050808080516103e05250506020810190508080805161040052505050506000506103a080518252806020015182602001528060400151826040015280606001518260600152505061016051610260511115156101a957610200516101a0526101c8565b610200516001808210156101bc57600080fd5b808203905090506101c0525b5b8151600101808352811415610092575b50506101a051600052600051610180515650005b600015610386575b6101c0526101405261016052610180526101a05260006101e0526101a0516102005261022060006080818352015b610200516101e05110151561023757610372565b6101e0516102005181818301101561024e57600080fd5b80820190509050600281818301101561026657600080fd5b8082019050905060028082049050905061024052610260608061038060446328d09d476102e052610160516103005261024051610320526102fc610140515afa6102af57600080fd5b607f3d116102bc57600080fd5b61038080808080516104005250506020810190508080805161042052505060208101905080808051610440525050602081019050808080516104605250505050600050610400805182528060200151826020015280604001518260400152806060015182606001525050610180516102a05111151561034257610240516101e052610361565b6102405160018082101561035557600080fd5b80820390509050610200525b5b8151600101808352811415610223575b50506101e0516000526000516101c0515650005b634e5e01346000511415610b695760043560a01c156103a457600080fd5b6040366101403760206102006004637f58e8f86101a0526101bc6001545afa6103cc57600080fd5b601f3d116103d957600080fd5b60005061020051610180526020610240602463010ae7576101c0526004356101e0526101dc6000545afa61040c57600080fd5b601f3d1161041957600080fd5b600050610240516101a0526020610240600463834ee4176101e0526101fc6001545afa61044557600080fd5b601f3d1161045257600080fd5b600050610240516101c0526020610240600463127dcbd36101e0526101fc6001545afa61047e57600080fd5b601f3d1161048b57600080fd5b60005061024051421015156104df576308c379a06102605260206102805260186102a0527f43616c6c20636865636b706f696e742066756e6374696f6e00000000000000006102c0526102a050606461027cfd5b61018051620151808181830110156104f657600080fd5b80820190509050421115610549576308c379a06101e0526020610200526018610220527f43616c6c20636865636b706f696e742066756e6374696f6e0000000000000000610240526102205060646101fcfd5b6101805162093a808082049050905062093a80808202821582848304141761057057600080fd5b80905090509050610180526101a051151561059157600060005260206000f3505b60206102806024632a2a314b610200526004356102205261021c6001545afa6105b957600080fd5b601f3d116105c657600080fd5b600050610280516101e0526101e0511515610653576101405161016051610180516101a0516101c0516101e05160005461020052600435610220526101c051610240526101a0516102605261026051610240516102205161020051600658016101f5565b6102c0526101e0526101c0526101a0526101805261016052610140526102c05161014052610694565b6020610280602463d5d46e88610200526004356102205261021c6001545afa61067b57600080fd5b601f3d1161068857600080fd5b60005061028051610140525b6101405115156106a5576001610140525b610200608061032060446328d09d47610280526004356102a052610140516102c05261029c6000545afa6106d857600080fd5b607f3d116106e557600080fd5b61032080808080516103a0525050602081019050808080516103c0525050602081019050808080516103e05250506020810190508080805161040052505050506000506103a08051825280602001518260200152806040015182604001528060600151826060015250506101e05115156107bc576102405162093a8081818301101561077057600080fd5b8082019050905060018082101561078657600080fd5b8082039050905062093a808082049050905062093a8080820282158284830414176107b057600080fd5b809050905090506101e0525b610180516101e0511015156107d757600060005260206000f3505b6101c0516101e05110156107ee576101c0516101e0525b6080366102803761030060006032818352015b610180516101e05110151561081557610b58565b610240516101e051101515610833576101a051610140511115610836565b60005b1561094f576101408051600181818301101561085157600080fd5b808201905090508152506102806102008051825280602001518260200152806040015182604001528060600151826060015250506101a05161014051111561089f576080366102003761094a565b61020060806103c060446328d09d476103205260043561034052610140516103605261033c6000545afa6108d257600080fd5b607f3d116108df57600080fd5b6103c080808080516104405250506020810190508080805161046052505060208101905080808051610480525050602081019050808080516104a052505050506000506104408051825280602001518260200152806040015182604001528060600151826060015250505b610b47565b6101e0516102c0518082101561096457600080fd5b8082039050905060405181111561097a57600080fd5b6103205261028051610320516102a0518082028080600081121561099a57195b607f1c156109a757600080fd5b905090509050808203808060008112156109bd57195b607f1c156109ca57600080fd5b9050905090506000808212156109e057806109e2565b815b9050905060008112156109f457600080fd5b61034052610340511515610a10576101a0516101405111610a13565b60005b15610a1d57610b58565b6000610340511115610b24576020610400602463edf59997610380526101e0516103a05261039c6001545afa610a5257600080fd5b601f3d11610a5f57600080fd5b60005061040051610360526020610420602463d4dafba86103a0526101e0516103c0526103bc6001545afa610a9357600080fd5b601f3d11610aa057600080fd5b60005061042051610380526000610380511815610ac4576000610360511415610ac7565b60005b15610b2357610160805161034051610360518082028215828483041417610aed57600080fd5b80905090509050610380518080610b0357600080fd5b820490509050818183011015610b1857600080fd5b808201905090508152505b5b6101e0805162093a80818183011015610b3c57600080fd5b808201905090508152505b5b8151600101808352811415610801575b50506101605160005260206000f350005b63dfe050316000511415610b855760005460005260206000f350005b63895b5d386000511415610ba15760015460005260206000f350005b5b60006000fd5b610062610c0a03610062600039610062610c0a036000f3",
+    "bytecode": "0x6f7fffffffffffffffffffffffffffffff6040526040610cfe610140396020610cfe60c03960c05160a01c1561003457600080fd5b60206020610cfe0160c03960c05160a01c1561004f57600080fd5b6101405160005561016051600155610ce656341561000a57600080fd5b600436101561001857610c7e565b600035601c526f7fffffffffffffffffffffffffffffff6040526000156101ed575b61018052610140526101605260006101a0526020610240600463900cf0cf6101e0526101fc610140515afa61006e57600080fd5b601f3d1161007b57600080fd5b600050610240516101c0526101e060006080818352015b6101c0516101a0511015156100a6576101d9565b6101a0516101c0518181830110156100bd57600080fd5b8082019050905060028181830110156100d557600080fd5b80820190509050600280820490509050610200526102206080610320602463d1febfb96102a052610200516102c0526102bc610140515afa61011657600080fd5b607f3d1161012357600080fd5b61032080808080516103a0525050602081019050808080516103c0525050602081019050808080516103e05250506020810190508080805161040052505050506000506103a080518252806020015182602001528060400151826040015280606001518260600152505061016051610260511115156101a957610200516101a0526101c8565b610200516001808210156101bc57600080fd5b808203905090506101c0525b5b8151600101808352811415610092575b50506101a051600052600051610180515650005b600015610386575b6101c0526101405261016052610180526101a05260006101e0526101a0516102005261022060006080818352015b610200516101e05110151561023757610372565b6101e0516102005181818301101561024e57600080fd5b80820190509050600281818301101561026657600080fd5b8082019050905060028082049050905061024052610260608061038060446328d09d476102e052610160516103005261024051610320526102fc610140515afa6102af57600080fd5b607f3d116102bc57600080fd5b61038080808080516104005250506020810190508080805161042052505060208101905080808051610440525050602081019050808080516104605250505050600050610400805182528060200151826020015280604001518260400152806060015182606001525050610180516102a05111151561034257610240516101e052610361565b6102405160018082101561035557600080fd5b80820390509050610200525b5b8151600101808352811415610223575b50506101e0516000526000516101c0515650005b600015610a8e575b61016052610140526040366101803760206102406004637f58e8f86101e0526101fc6001545afa6103be57600080fd5b601f3d116103cb57600080fd5b600050610240516101c0526020610280602463010ae75761020052610140516102205261021c6000545afa6103ff57600080fd5b601f3d1161040c57600080fd5b600050610280516101e0526020610280600463834ee4176102205261023c6001545afa61043857600080fd5b601f3d1161044557600080fd5b60005061028051610200526101c05162093a808082049050905062093a80808202821582848304141761047757600080fd5b809050905090506101c0526101e051151561049b5760006000526000516101605156505b60206102c06024632a2a314b61024052610140516102605261025c6001545afa6104c457600080fd5b601f3d116104d157600080fd5b6000506102c0516102205261022051151561056f576101405161016051610180516101a0516101c0516101e051610200516102205160005461024052610140516102605261020051610280526101e0516102a0526102a051610280516102605161024051600658016101f5565b6103005261022052610200526101e0526101c0526101a05261018052610160526101405261030051610180526105b1565b60206102c0602463d5d46e8861024052610140516102605261025c6001545afa61059857600080fd5b601f3d116105a557600080fd5b6000506102c051610180525b6101805115156105c2576001610180525b610240608061036060446328d09d476102c052610140516102e05261018051610300526102dc6000545afa6105f657600080fd5b607f3d1161060357600080fd5b61036080808080516103e052505060208101905080808051610400525050602081019050808080516104205250506020810190508080805161044052505050506000506103e08051825280602001518260200152806040015182604001528060600151826060015250506102205115156106da576102805162093a8081818301101561068e57600080fd5b808201905090506001808210156106a457600080fd5b8082039050905062093a808082049050905062093a8080820282158284830414176106ce57600080fd5b80905090509050610220525b6101c051610220511015156106f85760006000526000516101605156505b6102005161022051101561070f5761020051610220525b6080366102c03761034060006032818352015b6101c0516102205110151561073657610a7a565b6102805161022051101515610754576101e051610180511115610757565b60005b15610871576101808051600181818301101561077257600080fd5b808201905090508152506102c06102408051825280602001518260200152806040015182604001528060600151826060015250506101e0516101805111156107c0576080366102403761086c565b610240608061040060446328d09d47610360526101405161038052610180516103a05261037c6000545afa6107f457600080fd5b607f3d1161080157600080fd5b6104008080808051610480525050602081019050808080516104a0525050602081019050808080516104c0525050602081019050808080516104e052505050506000506104808051825280602001518260200152806040015182604001528060600151826060015250505b610a69565b61022051610300518082101561088657600080fd5b8082039050905060405181111561089c57600080fd5b610360526102c051610360516102e051808202808060008112156108bc57195b607f1c156108c957600080fd5b905090509050808203808060008112156108df57195b607f1c156108ec57600080fd5b9050905090506000808212156109025780610904565b815b90509050600081121561091657600080fd5b61038052610380511515610932576101e0516101805111610935565b60005b1561093f57610a7a565b6000610380511115610a46576020610440602463edf599976103c052610220516103e0526103dc6001545afa61097457600080fd5b601f3d1161098157600080fd5b600050610440516103a0526020610460602463d4dafba86103e05261022051610400526103fc6001545afa6109b557600080fd5b601f3d116109c257600080fd5b600050610460516103c05260006103c05118156109e65760006103a05114156109e9565b60005b15610a45576101a08051610380516103a0518082028215828483041417610a0f57600080fd5b809050905090506103c0518080610a2557600080fd5b820490509050818183011015610a3a57600080fd5b808201905090508152505b5b610220805162093a80818183011015610a5e57600080fd5b808201905090508152505b5b8151600101808352811415610722575b50506101a051600052600051610160515650005b633513b8fc6000511415610c005760043560a01c15610aac57600080fd5b60206101c06004637f58e8f86101605261017c6001545afa610acd57600080fd5b601f3d11610ada57600080fd5b6000506101c0516101405260206101c0600463127dcbd36101605261017c6001545afa610b0657600080fd5b601f3d11610b1357600080fd5b6000506101c05142101515610b67576308c379a06101e0526020610200526018610220527f43616c6c20636865636b706f696e742066756e6374696f6e0000000000000000610240526102205060646101fcfd5b6101405162015180818183011015610b7e57600080fd5b80820190509050421115610bd1576308c379a06101605260206101805260186101a0527f43616c6c20636865636b706f696e742066756e6374696f6e00000000000000006101c0526101a050606461017cfd5b6101405160043561016052610160516006580161038e565b6101c052610140526101c05160005260206000f350005b634e5e01346000511415610c455760043560a01c15610c1e57600080fd5b60043561014052610140516006580161038e565b6101a0526101a05160005260206000f350005b63dfe050316000511415610c615760005460005260206000f350005b63895b5d386000511415610c7d5760015460005260206000f350005b5b60006000fd5b610062610ce603610062600039610062610ce6036000f3",
     "contractName": "veFeeEstimate",
-    "deployedBytecode": "0x341561000a57600080fd5b600436101561001857610ba2565b600035601c526f7fffffffffffffffffffffffffffffff6040526000156101ed575b61018052610140526101605260006101a0526020610240600463900cf0cf6101e0526101fc610140515afa61006e57600080fd5b601f3d1161007b57600080fd5b600050610240516101c0526101e060006080818352015b6101c0516101a0511015156100a6576101d9565b6101a0516101c0518181830110156100bd57600080fd5b8082019050905060028181830110156100d557600080fd5b80820190509050600280820490509050610200526102206080610320602463d1febfb96102a052610200516102c0526102bc610140515afa61011657600080fd5b607f3d1161012357600080fd5b61032080808080516103a0525050602081019050808080516103c0525050602081019050808080516103e05250506020810190508080805161040052505050506000506103a080518252806020015182602001528060400151826040015280606001518260600152505061016051610260511115156101a957610200516101a0526101c8565b610200516001808210156101bc57600080fd5b808203905090506101c0525b5b8151600101808352811415610092575b50506101a051600052600051610180515650005b600015610386575b6101c0526101405261016052610180526101a05260006101e0526101a0516102005261022060006080818352015b610200516101e05110151561023757610372565b6101e0516102005181818301101561024e57600080fd5b80820190509050600281818301101561026657600080fd5b8082019050905060028082049050905061024052610260608061038060446328d09d476102e052610160516103005261024051610320526102fc610140515afa6102af57600080fd5b607f3d116102bc57600080fd5b61038080808080516104005250506020810190508080805161042052505060208101905080808051610440525050602081019050808080516104605250505050600050610400805182528060200151826020015280604001518260400152806060015182606001525050610180516102a05111151561034257610240516101e052610361565b6102405160018082101561035557600080fd5b80820390509050610200525b5b8151600101808352811415610223575b50506101e0516000526000516101c0515650005b634e5e01346000511415610b695760043560a01c156103a457600080fd5b6040366101403760206102006004637f58e8f86101a0526101bc6001545afa6103cc57600080fd5b601f3d116103d957600080fd5b60005061020051610180526020610240602463010ae7576101c0526004356101e0526101dc6000545afa61040c57600080fd5b601f3d1161041957600080fd5b600050610240516101a0526020610240600463834ee4176101e0526101fc6001545afa61044557600080fd5b601f3d1161045257600080fd5b600050610240516101c0526020610240600463127dcbd36101e0526101fc6001545afa61047e57600080fd5b601f3d1161048b57600080fd5b60005061024051421015156104df576308c379a06102605260206102805260186102a0527f43616c6c20636865636b706f696e742066756e6374696f6e00000000000000006102c0526102a050606461027cfd5b61018051620151808181830110156104f657600080fd5b80820190509050421115610549576308c379a06101e0526020610200526018610220527f43616c6c20636865636b706f696e742066756e6374696f6e0000000000000000610240526102205060646101fcfd5b6101805162093a808082049050905062093a80808202821582848304141761057057600080fd5b80905090509050610180526101a051151561059157600060005260206000f3505b60206102806024632a2a314b610200526004356102205261021c6001545afa6105b957600080fd5b601f3d116105c657600080fd5b600050610280516101e0526101e0511515610653576101405161016051610180516101a0516101c0516101e05160005461020052600435610220526101c051610240526101a0516102605261026051610240516102205161020051600658016101f5565b6102c0526101e0526101c0526101a0526101805261016052610140526102c05161014052610694565b6020610280602463d5d46e88610200526004356102205261021c6001545afa61067b57600080fd5b601f3d1161068857600080fd5b60005061028051610140525b6101405115156106a5576001610140525b610200608061032060446328d09d47610280526004356102a052610140516102c05261029c6000545afa6106d857600080fd5b607f3d116106e557600080fd5b61032080808080516103a0525050602081019050808080516103c0525050602081019050808080516103e05250506020810190508080805161040052505050506000506103a08051825280602001518260200152806040015182604001528060600151826060015250506101e05115156107bc576102405162093a8081818301101561077057600080fd5b8082019050905060018082101561078657600080fd5b8082039050905062093a808082049050905062093a8080820282158284830414176107b057600080fd5b809050905090506101e0525b610180516101e0511015156107d757600060005260206000f3505b6101c0516101e05110156107ee576101c0516101e0525b6080366102803761030060006032818352015b610180516101e05110151561081557610b58565b610240516101e051101515610833576101a051610140511115610836565b60005b1561094f576101408051600181818301101561085157600080fd5b808201905090508152506102806102008051825280602001518260200152806040015182604001528060600151826060015250506101a05161014051111561089f576080366102003761094a565b61020060806103c060446328d09d476103205260043561034052610140516103605261033c6000545afa6108d257600080fd5b607f3d116108df57600080fd5b6103c080808080516104405250506020810190508080805161046052505060208101905080808051610480525050602081019050808080516104a052505050506000506104408051825280602001518260200152806040015182604001528060600151826060015250505b610b47565b6101e0516102c0518082101561096457600080fd5b8082039050905060405181111561097a57600080fd5b6103205261028051610320516102a0518082028080600081121561099a57195b607f1c156109a757600080fd5b905090509050808203808060008112156109bd57195b607f1c156109ca57600080fd5b9050905090506000808212156109e057806109e2565b815b9050905060008112156109f457600080fd5b61034052610340511515610a10576101a0516101405111610a13565b60005b15610a1d57610b58565b6000610340511115610b24576020610400602463edf59997610380526101e0516103a05261039c6001545afa610a5257600080fd5b601f3d11610a5f57600080fd5b60005061040051610360526020610420602463d4dafba86103a0526101e0516103c0526103bc6001545afa610a9357600080fd5b601f3d11610aa057600080fd5b60005061042051610380526000610380511815610ac4576000610360511415610ac7565b60005b15610b2357610160805161034051610360518082028215828483041417610aed57600080fd5b80905090509050610380518080610b0357600080fd5b820490509050818183011015610b1857600080fd5b808201905090508152505b5b6101e0805162093a80818183011015610b3c57600080fd5b808201905090508152505b5b8151600101808352811415610801575b50506101605160005260206000f350005b63dfe050316000511415610b855760005460005260206000f350005b63895b5d386000511415610ba15760015460005260206000f350005b5b60006000fd",
+    "deployedBytecode": "0x341561000a57600080fd5b600436101561001857610c7e565b600035601c526f7fffffffffffffffffffffffffffffff6040526000156101ed575b61018052610140526101605260006101a0526020610240600463900cf0cf6101e0526101fc610140515afa61006e57600080fd5b601f3d1161007b57600080fd5b600050610240516101c0526101e060006080818352015b6101c0516101a0511015156100a6576101d9565b6101a0516101c0518181830110156100bd57600080fd5b8082019050905060028181830110156100d557600080fd5b80820190509050600280820490509050610200526102206080610320602463d1febfb96102a052610200516102c0526102bc610140515afa61011657600080fd5b607f3d1161012357600080fd5b61032080808080516103a0525050602081019050808080516103c0525050602081019050808080516103e05250506020810190508080805161040052505050506000506103a080518252806020015182602001528060400151826040015280606001518260600152505061016051610260511115156101a957610200516101a0526101c8565b610200516001808210156101bc57600080fd5b808203905090506101c0525b5b8151600101808352811415610092575b50506101a051600052600051610180515650005b600015610386575b6101c0526101405261016052610180526101a05260006101e0526101a0516102005261022060006080818352015b610200516101e05110151561023757610372565b6101e0516102005181818301101561024e57600080fd5b80820190509050600281818301101561026657600080fd5b8082019050905060028082049050905061024052610260608061038060446328d09d476102e052610160516103005261024051610320526102fc610140515afa6102af57600080fd5b607f3d116102bc57600080fd5b61038080808080516104005250506020810190508080805161042052505060208101905080808051610440525050602081019050808080516104605250505050600050610400805182528060200151826020015280604001518260400152806060015182606001525050610180516102a05111151561034257610240516101e052610361565b6102405160018082101561035557600080fd5b80820390509050610200525b5b8151600101808352811415610223575b50506101e0516000526000516101c0515650005b600015610a8e575b61016052610140526040366101803760206102406004637f58e8f86101e0526101fc6001545afa6103be57600080fd5b601f3d116103cb57600080fd5b600050610240516101c0526020610280602463010ae75761020052610140516102205261021c6000545afa6103ff57600080fd5b601f3d1161040c57600080fd5b600050610280516101e0526020610280600463834ee4176102205261023c6001545afa61043857600080fd5b601f3d1161044557600080fd5b60005061028051610200526101c05162093a808082049050905062093a80808202821582848304141761047757600080fd5b809050905090506101c0526101e051151561049b5760006000526000516101605156505b60206102c06024632a2a314b61024052610140516102605261025c6001545afa6104c457600080fd5b601f3d116104d157600080fd5b6000506102c0516102205261022051151561056f576101405161016051610180516101a0516101c0516101e051610200516102205160005461024052610140516102605261020051610280526101e0516102a0526102a051610280516102605161024051600658016101f5565b6103005261022052610200526101e0526101c0526101a05261018052610160526101405261030051610180526105b1565b60206102c0602463d5d46e8861024052610140516102605261025c6001545afa61059857600080fd5b601f3d116105a557600080fd5b6000506102c051610180525b6101805115156105c2576001610180525b610240608061036060446328d09d476102c052610140516102e05261018051610300526102dc6000545afa6105f657600080fd5b607f3d1161060357600080fd5b61036080808080516103e052505060208101905080808051610400525050602081019050808080516104205250506020810190508080805161044052505050506000506103e08051825280602001518260200152806040015182604001528060600151826060015250506102205115156106da576102805162093a8081818301101561068e57600080fd5b808201905090506001808210156106a457600080fd5b8082039050905062093a808082049050905062093a8080820282158284830414176106ce57600080fd5b80905090509050610220525b6101c051610220511015156106f85760006000526000516101605156505b6102005161022051101561070f5761020051610220525b6080366102c03761034060006032818352015b6101c0516102205110151561073657610a7a565b6102805161022051101515610754576101e051610180511115610757565b60005b15610871576101808051600181818301101561077257600080fd5b808201905090508152506102c06102408051825280602001518260200152806040015182604001528060600151826060015250506101e0516101805111156107c0576080366102403761086c565b610240608061040060446328d09d47610360526101405161038052610180516103a05261037c6000545afa6107f457600080fd5b607f3d1161080157600080fd5b6104008080808051610480525050602081019050808080516104a0525050602081019050808080516104c0525050602081019050808080516104e052505050506000506104808051825280602001518260200152806040015182604001528060600151826060015250505b610a69565b61022051610300518082101561088657600080fd5b8082039050905060405181111561089c57600080fd5b610360526102c051610360516102e051808202808060008112156108bc57195b607f1c156108c957600080fd5b905090509050808203808060008112156108df57195b607f1c156108ec57600080fd5b9050905090506000808212156109025780610904565b815b90509050600081121561091657600080fd5b61038052610380511515610932576101e0516101805111610935565b60005b1561093f57610a7a565b6000610380511115610a46576020610440602463edf599976103c052610220516103e0526103dc6001545afa61097457600080fd5b601f3d1161098157600080fd5b600050610440516103a0526020610460602463d4dafba86103e05261022051610400526103fc6001545afa6109b557600080fd5b601f3d116109c257600080fd5b600050610460516103c05260006103c05118156109e65760006103a05114156109e9565b60005b15610a45576101a08051610380516103a0518082028215828483041417610a0f57600080fd5b809050905090506103c0518080610a2557600080fd5b820490509050818183011015610a3a57600080fd5b808201905090508152505b5b610220805162093a80818183011015610a5e57600080fd5b808201905090508152505b5b8151600101808352811415610722575b50506101a051600052600051610160515650005b633513b8fc6000511415610c005760043560a01c15610aac57600080fd5b60206101c06004637f58e8f86101605261017c6001545afa610acd57600080fd5b601f3d11610ada57600080fd5b6000506101c0516101405260206101c0600463127dcbd36101605261017c6001545afa610b0657600080fd5b601f3d11610b1357600080fd5b6000506101c05142101515610b67576308c379a06101e0526020610200526018610220527f43616c6c20636865636b706f696e742066756e6374696f6e0000000000000000610240526102205060646101fcfd5b6101405162015180818183011015610b7e57600080fd5b80820190509050421115610bd1576308c379a06101605260206101805260186101a0527f43616c6c20636865636b706f696e742066756e6374696f6e00000000000000006101c0526101a050606461017cfd5b6101405160043561016052610160516006580161038e565b6101c052610140526101c05160005260206000f350005b634e5e01346000511415610c455760043560a01c15610c1e57600080fd5b60043561014052610140516006580161038e565b6101a0526101a05160005260206000f350005b63dfe050316000511415610c615760005460005260206000f350005b63895b5d386000511415610c7d5760015460005260206000f350005b5b60006000fd",
     "deployedLinkReferences": {},
     "linkReferences": {},
     "sourceName": "contracts/ve/veFeeEstimate.vy"
 }
```

### Comparing `ocean-contracts-1.1.7/artifacts/veOCEAN.json` & `ocean-contracts-1.1.8/artifacts/veOCEAN.json`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/ocean_contracts.egg-info/PKG-INFO` & `ocean-contracts-1.1.8/ocean_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-contracts
-Version: 1.1.7
+Version: 1.1.8
 Summary: 🐳 Ocean Protocol L1 - v4
 Home-page: https://github.com/oceanprotocol/contracts
 Author: leucothia
 Author-email: devops@oceanprotocol.com
 Project-URL: Bug Tracker, https://github.com/oceanprotocol/contracts/issues
 Keywords: ocean-contracts
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ocean-contracts-1.1.7/ocean_contracts.egg-info/SOURCES.txt` & `ocean-contracts-1.1.8/ocean_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocean-contracts-1.1.7/setup.cfg` & `ocean-contracts-1.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocean-contracts
-version = v1.1.7
+version = v1.1.8
 author = leucothia
 author_email = devops@oceanprotocol.com
 description = 🐳 Ocean Protocol L1 - v4
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/oceanprotocol/contracts
 project_urls =
```

