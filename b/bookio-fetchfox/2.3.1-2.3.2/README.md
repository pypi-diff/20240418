# Comparing `tmp/bookio_fetchfox-2.3.1.tar.gz` & `tmp/bookio_fetchfox-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-2.3.1.tar", max compression
+gzip compressed data, was "bookio_fetchfox-2.3.2.tar", max compression
```

## Comparing `bookio_fetchfox-2.3.1.tar` & `bookio_fetchfox-2.3.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0     3734 2024-01-12 20:45:39.378935 bookio_fetchfox-2.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-22 18:42:59.790777 bookio_fetchfox-2.3.1/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 19:34:25.067639 bookio_fetchfox-2.3.1/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 20:35:31.808829 bookio_fetchfox-2.3.1/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2510 2024-01-12 20:36:14.497593 bookio_fetchfox-2.3.1/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      609 2024-01-12 20:20:12.987230 bookio_fetchfox-2.3.1/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1427 2024-01-12 20:11:30.370925 bookio_fetchfox-2.3.1/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     2156 2024-01-12 20:20:44.459776 bookio_fetchfox-2.3.1/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      605 2024-01-12 20:20:44.461731 bookio_fetchfox-2.3.1/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2024-02-06 20:08:14.092241 bookio_fetchfox-2.3.1/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-05-22 19:46:15.444479 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0      259 2023-11-04 23:00:04.948427 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/cexplorerio.py
--rw-r--r--   0        0        0      891 2024-01-12 20:38:44.306297 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1908 2024-01-12 20:39:14.419257 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/dexhunterio.py
--rw-r--r--   0        0        0     6920 2024-02-13 19:14:29.833982 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/gomaestroorg.py
--rw-r--r--   0        0        0     1798 2024-01-12 20:41:23.102831 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0      536 2024-01-12 20:41:35.353758 bookio_fetchfox-2.3.1/fetchfox/apis/cardano/muesliswap.py
--rwxr-xr-x   0        0        0     1572 2024-02-15 23:08:16.056979 bookio_fetchfox-2.3.1/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-05-22 20:52:16.585943 bookio_fetchfox-2.3.1/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      988 2024-01-12 20:13:29.740160 bookio_fetchfox-2.3.1/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     5658 2024-02-15 20:44:53.991570 bookio_fetchfox-2.3.1/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     3037 2024-01-12 20:40:23.660298 bookio_fetchfox-2.3.1/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      228 2024-02-15 20:43:38.059993 bookio_fetchfox-2.3.1/fetchfox/apis/pinatacloud.py
--rw-r--r--   0        0        0      228 2024-01-12 20:43:12.078434 bookio_fetchfox-2.3.1/fetchfox/apis/price.py
--rw-r--r--   0        0        0      120 2023-05-22 21:04:39.572946 bookio_fetchfox-2.3.1/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-05-22 20:40:27.617977 bookio_fetchfox-2.3.1/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0    10494 2024-01-12 20:57:40.770676 bookio_fetchfox-2.3.1/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      689 2024-01-12 20:29:40.403414 bookio_fetchfox-2.3.1/fetchfox/blockchains/algorand/exceptions.py
--rw-r--r--   0        0        0      502 2024-01-12 20:29:40.405290 bookio_fetchfox-2.3.1/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     3408 2024-01-12 20:32:27.622297 bookio_fetchfox-2.3.1/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-05-22 20:04:22.058021 bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    17237 2024-01-12 21:05:38.118871 bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0      679 2024-01-12 20:43:12.080772 bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/exceptions.py
--rw-r--r--   0        0        0     1060 2024-01-12 20:43:12.079744 bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-05-22 21:04:55.872786 bookio_fetchfox-2.3.1/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1696 2024-01-12 20:40:23.663051 bookio_fetchfox-2.3.1/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-05-22 21:02:14.850258 bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0    11892 2024-02-15 20:34:02.296705 bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      753 2024-01-12 20:52:52.997471 bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/exceptions.py
--rw-r--r--   0        0        0      617 2024-01-12 20:49:04.872672 bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0      443 2023-10-21 20:06:38.975469 bookio_fetchfox-2.3.1/fetchfox/blockchains/exceptions.py
--rw-r--r--   0        0        0       32 2023-05-22 21:05:18.318023 bookio_fetchfox-2.3.1/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1706 2024-01-12 20:40:23.664934 bookio_fetchfox-2.3.1/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2023-06-11 21:22:19.039084 bookio_fetchfox-2.3.1/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0     1135 2024-02-13 18:38:33.334392 bookio_fetchfox-2.3.1/fetchfox/book_pool.py
--rw-r--r--   0        0        0     3986 2024-02-15 22:27:18.071082 bookio_fetchfox-2.3.1/fetchfox/book_token.py
--rw-r--r--   0        0        0      322 2023-05-25 16:44:40.820770 bookio_fetchfox-2.3.1/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-03-18 01:27:25.904724 bookio_fetchfox-2.3.1/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-04-08 20:21:25.130685 bookio_fetchfox-2.3.1/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      399 2024-02-13 18:17:03.442615 bookio_fetchfox-2.3.1/fetchfox/constants/book.py
--rw-r--r--   0        0        0       82 2023-06-13 00:03:02.230103 bookio_fetchfox-2.3.1/fetchfox/constants/cardano.py
--rw-r--r--   0        0        0      136 2023-10-25 14:18:10.007236 bookio_fetchfox-2.3.1/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0       66 2023-06-13 00:12:38.375720 bookio_fetchfox-2.3.1/fetchfox/constants/evm.py
--rw-r--r--   0        0        0      341 2023-06-29 20:15:14.099766 bookio_fetchfox-2.3.1/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-04 19:58:46.799073 bookio_fetchfox-2.3.1/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       62 2023-10-17 18:57:28.495105 bookio_fetchfox-2.3.1/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      322 2023-12-18 18:25:43.796675 bookio_fetchfox-2.3.1/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     3619 2023-12-07 19:32:18.490623 bookio_fetchfox-2.3.1/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3666 2024-01-04 22:44:54.501974 bookio_fetchfox-2.3.1/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2023-06-09 12:35:49.407500 bookio_fetchfox-2.3.1/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      495 2024-01-12 21:09:28.927183 bookio_fetchfox-2.3.1/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1572 2023-10-25 14:35:03.908400 bookio_fetchfox-2.3.1/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      799 2023-11-04 22:49:54.594388 bookio_fetchfox-2.3.1/fetchfox/dtos/order.py
--rw-r--r--   0        0        0     1203 2024-01-12 20:08:01.630668 bookio_fetchfox-2.3.1/fetchfox/dtos/pair_stats.py
--rw-r--r--   0        0        0      365 2023-06-08 22:15:07.721723 bookio_fetchfox-2.3.1/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     2023 2023-10-25 14:35:03.900357 bookio_fetchfox-2.3.1/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-05-24 23:06:14.513191 bookio_fetchfox-2.3.1/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-05-24 23:06:14.513363 bookio_fetchfox-2.3.1/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     5794 2024-02-13 18:38:33.331493 bookio_fetchfox-2.3.1/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2024-02-15 23:08:27.711205 bookio_fetchfox-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 bookio_fetchfox-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3734 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      609 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1427 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     2156 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      605 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/cexplorerio.py
+-rw-r--r--   0        0        0      891 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1908 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/dexhunterio.py
+-rw-r--r--   0        0        0     6920 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/gomaestroorg.py
+-rw-r--r--   0        0        0     1798 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/jpgstore.py
+-rw-r--r--   0        0        0      536 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/cardano/muesliswap.py
+-rwxr-xr-x   0        0        0     1572 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      988 2024-04-18 08:58:01.572863 bookio_fetchfox-2.3.2/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     5658 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     3037 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      228 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/apis/pinatacloud.py
+-rw-r--r--   0        0        0      228 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/apis/price.py
+-rw-r--r--   0        0        0      120 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0    10494 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      689 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/algorand/exceptions.py
+-rw-r--r--   0        0        0      502 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     3408 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    17318 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0      679 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/exceptions.py
+-rw-r--r--   0        0        0     1060 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1696 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    11892 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      753 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/exceptions.py
+-rw-r--r--   0        0        0      617 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0      443 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/exceptions.py
+-rw-r--r--   0        0        0       32 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1706 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0     1135 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/book_pool.py
+-rw-r--r--   0        0        0     3986 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/book_token.py
+-rw-r--r--   0        0        0      322 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      399 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/book.py
+-rw-r--r--   0        0        0       82 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      136 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      341 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0   453386 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/ranks.py
+-rw-r--r--   0        0        0       95 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       62 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      322 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     3619 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3666 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      495 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1572 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      799 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/order.py
+-rw-r--r--   0        0        0     1203 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/pair_stats.py
+-rw-r--r--   0        0        0      365 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     2023 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     5794 2024-04-18 08:58:01.576863 bookio_fetchfox-2.3.2/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2024-04-18 08:58:01.588863 bookio_fetchfox-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 bookio_fetchfox-2.3.2/setup.py
+-rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 bookio_fetchfox-2.3.2/PKG-INFO
```

### Comparing `bookio_fetchfox-2.3.1/README.md` & `bookio_fetchfox-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/cardano/dexhunterio.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/cardano/dexhunterio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/cardano/gomaestroorg.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/cardano/gomaestroorg.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/cardano/muesliswap.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/cardano/muesliswap.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-2.3.2/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/algorand/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/algorand/exceptions.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/algorand/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/base.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 from datetime import datetime
 from typing import Iterable, Tuple, List
 
 import pytz
 
 from fetchfox.apis import bookio
-from fetchfox.apis.cardano import cnfttools, jpgstore, gomaestroorg
+from fetchfox.apis.cardano import jpgstore, gomaestroorg
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import CARDANO
 from fetchfox.constants.currencies import ADA, BOOK
 from fetchfox.constants.marketplaces import JPG_STORE
+from fetchfox.constants.ranks import CNFT_RANKS
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
     CampaignPricingDTO,
     FloorDTO,
     HoldingDTO,
     ListingDTO,
@@ -215,27 +216,28 @@
                 quantity=owner["amount"],
             )
 
     def get_asset_rank(self, collection_id: str, asset_id: str, *args, **kwargs) -> RankDTO:
         self.check_collection_id(collection_id)
         self.check_asset_id(asset_id)
 
-        asset_rank = cnfttools.get_asset_rank(asset_id)
+        _, asset_name = utils.split_asset_id(asset_id)
+        number = int("".join((c for c in asset_name if c.isdigit())))
 
-        if asset_rank is None:
+        if collection_id not in CNFT_RANKS:
             return None
 
-        _, asset_name = utils.split_asset_id(asset_id)
-        number = int("".join((c for c in asset_name if c.isdigit())))
+        if asset_name not in CNFT_RANKS[collection_id]:
+            return None
 
         return RankDTO(
             collection_id=collection_id,
-            asset_id=asset_id.lower(),
             number=number,
-            rank=int(asset_rank),
+            asset_id=asset_id,
+            rank=CNFT_RANKS[collection_id][asset_name],
         )
 
     # Collections
 
     def get_collection_assets(
         self, collection_id: str, discriminator: str = None, fetch_metadata: bool = True, *args, **kwargs
     ) -> Iterable[AssetDTO]:
@@ -336,17 +338,18 @@
                 tx_hash=listing["tx_hash"],
                 marketplace_url=f"https://jpg.store/asset/{asset_id}",
             )
 
     def get_collection_ranks(self, collection_id: str, *args, **kwargs) -> Iterable[RankDTO]:
         self.check_collection_id(collection_id)
 
-        collection_ranks = cnfttools.get_collection_ranks(collection_id) or {}
+        if collection_id not in CNFT_RANKS:
+            return
 
-        for asset_name, rank in collection_ranks.items():
+        for asset_name, rank in CNFT_RANKS[collection_id].items():
             number = int("".join((c for c in asset_name if c.isdigit())))
 
             yield RankDTO(
                 collection_id=collection_id,
                 number=number,
                 asset_id=None,
                 rank=int(rank),
```

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/exceptions.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/exceptions.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-2.3.2/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/book_pool.py` & `bookio_fetchfox-2.3.2/fetchfox/book_pool.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/book_token.py` & `bookio_fetchfox-2.3.2/fetchfox/book_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/dtos/asset.py` & `bookio_fetchfox-2.3.2/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/dtos/campaign.py` & `bookio_fetchfox-2.3.2/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/dtos/listing.py` & `bookio_fetchfox-2.3.2/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/dtos/order.py` & `bookio_fetchfox-2.3.2/fetchfox/dtos/order.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/dtos/pair_stats.py` & `bookio_fetchfox-2.3.2/fetchfox/dtos/pair_stats.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/dtos/sale.py` & `bookio_fetchfox-2.3.2/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/fetchfox/rest.py` & `bookio_fetchfox-2.3.2/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.3.1/pyproject.toml` & `bookio_fetchfox-2.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "2.3.1"
+version = "2.3.2"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-2.3.1/PKG-INFO` & `bookio_fetchfox-2.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 2.3.1
+Version: 2.3.2
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Project-URL: Documentation, https://github.com/book-io/fetchfox/blob/main/README.md
 Description-Content-Type: text/markdown
```

