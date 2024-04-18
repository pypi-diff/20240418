# Comparing `tmp/artesian-sdk-3.1.3.dev5.tar.gz` & `tmp/artesian_sdk-3.1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artesian-sdk-3.1.3.dev5.tar", last modified: Wed Mar 27 13:39:48 2024, max compression
+gzip compressed data, was "artesian_sdk-3.1.4.dev2.tar", last modified: Thu Apr 18 16:37:56 2024, max compression
```

## Comparing `artesian-sdk-3.1.3.dev5.tar` & `artesian_sdk-3.1.4.dev2.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.822569 artesian-sdk-3.1.3.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.802569 artesian-sdk-3.1.3.dev5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.806568 artesian-sdk-3.1.3.dev5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.github/workflows/dependency-review.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.806568 artesian-sdk-3.1.3.dev5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-03-27 13:39:48.818569 artesian-sdk-3.1.3.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21348 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.806568 artesian-sdk-3.1.3.dev5/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestActual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestAuction.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestGMEOffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestMarketDataService.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestMas.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestSearchFacet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestVersioned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryActual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryAuction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryMas.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 13:39:48.822569 artesian-sdk-3.1.3.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.802569 artesian-sdk-3.1.3.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.806568 artesian-sdk-3.1.3.dev5/src/Artesian/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/ArtesianConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/ArtesianPolicyConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.810568 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/ExtractionRangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    15422 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.810568 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/BaType.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/GenerationType.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/Market.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/Purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/Scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/Status.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/UnitType.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/Zone.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/_Enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Granularity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.810568 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/MarketDataService.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.810568 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/CurveRangeEntity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/PagedResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/UpsertData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.814569 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Enum/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Enum/AggregationRule.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Enum/ArtesianMetadataFacetType.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Enum/MarketDataType.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.814569 artesian-sdk-3.1.3.dev5/src/Artesian/Query/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/ActualQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/AuctionQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/BidAskQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/DefaultPartitionStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/MasQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/QueryService.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/RelativeInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/VersionedQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_Query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.814569 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/ExtractionRangeType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/MasQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/QueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionSelectionType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/Query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.818569 artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/Client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/RequestExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/src/Artesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-27 13:39:48.000000 artesian-sdk-3.1.3.dev5/src/Artesian/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.818569 artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-03-27 13:39:48.000000 artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-03-27 13:39:48.000000 artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:39:48.000000 artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-27 13:39:48.000000 artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 13:39:48.000000 artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:48.818569 artesian-sdk-3.1.3.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestActual.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestClientErrorHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestGMEPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestMarketDataService.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestMarketDataUpsertData.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestMas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/TestVersioned.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-27 13:39:41.000000 artesian-sdk-3.1.3.dev5/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.github/workflows/dependency-review.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21348 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.638981 artesian_sdk-3.1.4.dev2/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestAuction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestGMEOffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestMarketDataService.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestSearchFacet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryAuction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.634981 artesian_sdk-3.1.4.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.638981 artesian_sdk-3.1.4.dev2/src/Artesian/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianPolicyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.638981 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/ExtractionRangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/BaType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/GenerationType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Market.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/UnitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/Zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/_Enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Granularity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/
+-rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/MarketDataService.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/CurveRangeEntity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/PagedResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/UpsertData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.642981 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/AggregationRule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/ArtesianMetadataFacetType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/MarketDataType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.646982 artesian_sdk-3.1.4.dev2/src/Artesian/Query/
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/ActualQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/AuctionQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/BidAskQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/DefaultPartitionStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/MasQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/QueryService.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/RelativeInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/VersionedQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_Query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.646982 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ExtractionRangeType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MasQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/QueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionSelectionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/Query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.646982 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/RequestExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/src/Artesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/Artesian/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 16:37:56.000000 artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:56.650982 artesian_sdk-3.1.4.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestActual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestClientErrorHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestGMEPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestMarketDataService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestMarketDataUpsertData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestMas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/TestVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 16:37:52.000000 artesian_sdk-3.1.4.dev2/tests/helpers.py
```

### Comparing `artesian-sdk-3.1.3.dev5/.github/workflows/python-tests.yml` & `artesian_sdk-3.1.4.dev2/.github/workflows/python-tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,22 @@
         python -m pip install --upgrade pip
         pip install -e ".[dev]"
 
     - name: Run flake8
       run: |
         flake8 .
 
+    - uses: jordemort/action-pyright@v1
+      with:
+        github_token: ${{ secrets.GITHUB_TOKEN }}
+        reporter: github-check
+        lib: 
+        level: warning
+        filter_mode: file
+
     - name: Test Pytest
       run: |
         pytest --junitxml=junit/test-results-${{ matrix.python-version }}.xml
 
     - name: Upload pytest test results
       uses: actions/upload-artifact@v3
       with:
```

### Comparing `artesian-sdk-3.1.3.dev5/.gitignore` & `artesian_sdk-3.1.4.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/.vscode/launch.json` & `artesian_sdk-3.1.4.dev2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/LICENSE` & `artesian_sdk-3.1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/PKG-INFO` & `artesian_sdk-3.1.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artesian-sdk
-Version: 3.1.3.dev5
+Version: 3.1.4.dev2
 Summary: Library provides read access to the Artesian API
 Author-email: ARK Lab <arklab@ark-energy.eu>
 Maintainer-email: ARK Lab <arklab@ark-energy.eu>
 License: MIT License
         
         Copyright (c) 2022 Ark Energy S.r.l.
```

### Comparing `artesian-sdk-3.1.3.dev5/README.md` & `artesian_sdk-3.1.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/pyproject.toml` & `artesian_sdk-3.1.4.dev2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -151,8 +151,15 @@
 local_scheme = "dirty-tag"
 
 [tool.pytest.ini_options]
 python_files = "Test*.py"
 testpaths = [
     "tests"
 ]
-addopts = "--doctest-modules --junitxml=junit/test-results.xml --cov=src --cov-report=xml --cov-report=html"
+addopts = "--doctest-modules --junitxml=junit/test-results.xml --cov=src --cov-report=xml --cov-report=html"
+
+[tool.pyright]
+include = ["src"]
+exclude = [
+  "**/node_modules",
+  "**/__pycache__"
+]
```

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestActual.py` & `artesian_sdk-3.1.4.dev2/samples/TestActual.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestAuction.py` & `artesian_sdk-3.1.4.dev2/samples/TestAuction.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestSearchFacet.py` & `artesian_sdk-3.1.4.dev2/samples/TestSearchFacet.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestVersioned.py` & `artesian_sdk-3.1.4.dev2/samples/TestVersioned.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryActual.py` & `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryActual.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryAuction.py` & `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryAuction.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryBidAsk.py` & `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryBidAsk.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/samples/TestWriteDataAndQueryMas.py` & `artesian_sdk-3.1.4.dev2/samples/TestWriteDataAndQueryMas.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/ArtesianConfig.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/ArtesianPolicyConfig.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/ArtesianPolicyConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Exceptions.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 class ArtesianSdkOptimisticConcurrencyException(ArtesianSdkRemoteException):
     """
     Artesian optimistic concurrency exception.
     """
 
     def __init__(
-        self: ArtesianSdkValidationException,
+        self: ArtesianSdkOptimisticConcurrencyException,
         method: str,
         url: str,
         statusCode: int,
         problemDetails: Optional[dict] = None,
         errorText: Optional[str] = None,
     ) -> None:
         """
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,22 +344,27 @@
             Market.MIA3: "MIA3",
         }
         vr = switcher.get(market, "DefMarket")
         if vr == "DefMarket":
             raise Exception("Not supported Market")
         return vr
 
-    def __getPurpose(self: GMEPublicOfferQuery, purpose: Purpose) -> str:
+    def __getPurpose(self: GMEPublicOfferQuery, purpose: Purpose | None) -> str:
+        if purpose is None:
+            raise Exception("Not supported Purpose")
         switcher = {Purpose.BID: "BID", Purpose.OFF: "OFF"}
         vr = switcher.get(purpose, "Defpurp")
         if vr == "Defpurp":
             raise Exception("Not supported Purpose")
         return vr
 
-    def __getStatus(self: GMEPublicOfferQuery, status: Status) -> str:
+    def __getStatus(self: GMEPublicOfferQuery, status: Status | None) -> str:
+        if status is None:
+            raise Exception("Not supported Status")
+
         switcher = {
             Status.ACC: "ACC",
             Status.INC: "INC",
             Status.REJ: "REJ",
             Status.REP: "REP",
             Status.REV: "REV",
             Status.SUB: "SUB",
@@ -425,35 +430,27 @@
 
     def _buildExtractionRangeRoute(
         self: GMEPublicOfferQuery, queryParamaters: _GMEPublicOfferQueryParameters
     ) -> str:
         subPath = f"{self.__toUrlParam(queryParamaters.extractionRangeConfig.date)}"
         return subPath
 
-    def _buildExtractionStatus(self: GMEPublicOfferQuery, status: Status) -> str:
-        subPath = f"{parse.quote_plus(status)}"
-        return subPath
-
-    def _buildExtractionPurpose(self: GMEPublicOfferQuery, purpose: Purpose) -> str:
-        subPath = f"{parse.quote_plus(purpose)}"
-        return subPath
-
     def _exec(self: GMEPublicOfferQuery, url: str) -> Any:
         loop = get_event_loop()
         rr = loop.run_until_complete(self._execAsync(url))
         return rr
 
     async def _execAsync(self: GMEPublicOfferQuery, url: str) -> Any:
         with self.__client as c:
             res = await asyncio.gather(
                 *[self.__executor.exec(c.exec, "GET", url, None)]
             )
             return res[0]
 
-    def __toUrlParam(self: GMEPublicOfferQuery, date: str) -> str:
+    def __toUrlParam(self: GMEPublicOfferQuery, date: str | None) -> str:
         return f"{date}"
 
     def _validateQuery(self: GMEPublicOfferQuery) -> None:
         if self._queryParameters.purpose is None:
             raise Exception(
                 "Extraction Purpose must be provided. Use .forScope()"
                 + " argument takes a scope type"
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/GMEPublicOffers/__init__.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/GMEPublicOffers/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/MarketDataService.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/MarketDataService.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             )
         )
 
     async def searchFacetAsync(
         self: MarketDataService,
         page: int,
         pageSize: int,
-        searchText: str = None,
+        searchText: str | None = None,
         filters: Optional[Dict[str, List[str]]] = None,
         sorts: Optional[List[str]] = None,
         doNotLoadAdditionalInfo: bool = False,
     ) -> ArtesianSearchResults:
         """
         Search the MarketData collection with faceted results.
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianMetadataFacet.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     Attributes:
         facetName: the name of the facet
         facetType: the type of the facet
         values: list of ArtesianMetadataFacetCount
     """
 
     facetName: Optional[str] = None
-    facetType: ArtesianMetadataFacetType = None
+    facetType: Optional[ArtesianMetadataFacetType] = None
     values: Optional[List[ArtesianMetadataFacetCount]] = None
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/ArtesianSearchResults.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/CurveRangeEntity.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/CurveRangeEntity.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/PagedResult.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/PagedResult.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/UpsertData.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/UpsertData.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/_Dto/__init__.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/_Dto/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/MarketData/__init__.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/MarketData/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/ActualQuery.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/ActualQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/AuctionQuery.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/AuctionQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/BidAskQuery.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/BidAskQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/DefaultPartitionStrategy.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/DefaultPartitionStrategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 import copy
-from typing import List
+from typing import List, TypeVar
+
+from ._QueryParameters.QueryParameters import _QueryParameters
 from ._QueryParameters.ActualQueryParameters import ActualQueryParameters
 from ._QueryParameters.VersionedQueryParameters import VersionedQueryParameters
 from ._QueryParameters.AuctionQueryParameters import AuctionQueryParameters
 from ._QueryParameters.MasQueryParameters import MasQueryParameters
 from ._QueryParameters.BidAskQueryParameters import BidAskQueryParameters
 
 
+T = TypeVar("T", bound=_QueryParameters)
+
+
 class DefaultPartitionStrategy:
     """Class for the default strategy to partition Query Parameters."""
 
     maxNumberOfIds = 15
     """ Only 15 allowed."""
 
     def PartitionActual(
@@ -85,17 +90,17 @@
         Returns:
             The input list of Bid Ask Query parameters partitioned
             with the defined strategy.
         """
         return self._tsPartitionStrategy(bidAskQueryParameters)
 
     def _tsPartitionStrategy(
-        self: DefaultPartitionStrategy, Parameters: List[MasQueryParameters]
-    ) -> List[MasQueryParameters]:
-        res: List[MasQueryParameters] = []
+        self: DefaultPartitionStrategy, Parameters: List[T]
+    ) -> List[T]:
+        res: List[T] = []
         for param in Parameters:
             if param.ids is None:
                 res.append(param)
                 continue
             leng = len(param.ids)
             batches = [
                 param.ids[i : i + DefaultPartitionStrategy.maxNumberOfIds]
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/MasQuery.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/MasQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/QueryService.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/QueryService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/VersionedQuery.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/VersionedQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_Query.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_Query.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     async def _execAsync(self: _Query, urls: List[str]) -> list:
         with self._client as c:
             res = await asyncio.gather(
                 *[self._requestExecutor.exec(c.exec, "GET", i, None) for i in urls]
             )
             return list(itertools.chain(*res))
 
-    def __toUrlParam(self: _Query, start: str, end: str) -> str:
+    def __toUrlParam(self: _Query, start: str | None, end: str | None) -> str:
         return f"{start}/{end}"
 
     def _validateQuery(self: _Query) -> None:
         if self._queryParameters.extractionRangeType is None:
             raise Exception(
                 "Data extraction range must be provided. Provide a date range, period"
                 + " or period range or an interval eg .InAbsoluteDateRange()"
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/MasQueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MasQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/QueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/QueryParameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def __init__(self: _FillCustomTimeserieStrategy, val: float) -> None:
         self.val = val
 
     def getUrlParams(self: _FillCustomTimeserieStrategy) -> str:
         return f"fillerK=CustomValue&fillerDV={self.val}"
 
 
-def toQueryParams(vals: List[List[str]]) -> str:
+def toQueryParams(vals: List[List[str | float | int | None]]) -> str:
     filtered = filter(lambda x: x[1], vals)
     stringVals = map(lambda x: [x[0], str(x[1])], filtered)
     joinedEqual = map(lambda x: "=".join(x), stringVals)
     return "&".join(joinedEqual)
 
 
 class _FillCustomBidAskStrategy(_FillStrategy):
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     return result
 
 
 def __artesianDictDeserializer(
     obj: list, cls: type, *args: Any, **kwargs: Any
 ) -> object:
     key, value = get_args(cls)
-    result: Dict[key, value] = {
+    result: Dict[key, value] = {  # type: ignore
         jsons.load(item["Key"], key, *args, **kwargs): jsons.load(
             item["Value"], value, *args, **kwargs
         )
         for item in obj
     }
     return result
```

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/Client.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/Client.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/_ClientsExecutor/RequestExecutor.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/_ClientsExecutor/RequestExecutor.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/Artesian/__init__.py` & `artesian_sdk-3.1.4.dev2/src/Artesian/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/PKG-INFO` & `artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artesian-sdk
-Version: 3.1.3.dev5
+Version: 3.1.4.dev2
 Summary: Library provides read access to the Artesian API
 Author-email: ARK Lab <arklab@ark-energy.eu>
 Maintainer-email: ARK Lab <arklab@ark-energy.eu>
 License: MIT License
         
         Copyright (c) 2022 Ark Energy S.r.l.
```

### Comparing `artesian-sdk-3.1.3.dev5/src/artesian_sdk.egg-info/SOURCES.txt` & `artesian_sdk-3.1.4.dev2/src/artesian_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/dependency-review.yaml
 .github/workflows/python-tests.yml
+.vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 samples/TestActual.py
 samples/TestAuction.py
 samples/TestBidAsk.py
 samples/TestGMEOffers.py
 samples/TestMarketDataService.py
```

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestActual.py` & `artesian_sdk-3.1.4.dev2/tests/TestActual.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestBidAsk.py` & `artesian_sdk-3.1.4.dev2/tests/TestBidAsk.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestClientErrorHandling.py` & `artesian_sdk-3.1.4.dev2/tests/TestClientErrorHandling.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestGMEPO.py` & `artesian_sdk-3.1.4.dev2/tests/TestGMEPO.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestMarketDataService.py` & `artesian_sdk-3.1.4.dev2/tests/TestMarketDataService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestMarketDataUpsertData.py` & `artesian_sdk-3.1.4.dev2/tests/TestMarketDataUpsertData.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestMas.py` & `artesian_sdk-3.1.4.dev2/tests/TestMas.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/TestVersioned.py` & `artesian_sdk-3.1.4.dev2/tests/TestVersioned.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.1.3.dev5/tests/helpers.py` & `artesian_sdk-3.1.4.dev2/tests/helpers.py`

 * *Files identical despite different names*

