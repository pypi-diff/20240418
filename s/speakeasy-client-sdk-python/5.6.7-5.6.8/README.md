# Comparing `tmp/speakeasy-client-sdk-python-5.6.7.tar.gz` & `tmp/speakeasy-client-sdk-python-5.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.6.7.tar", last modified: Wed Apr 17 00:13:03 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.6.8.tar", last modified: Thu Apr 18 00:12:21 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.6.7.tar` & `speakeasy-client-sdk-python-5.6.8.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.836479 speakeasy-client-sdk-python-5.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)    22202 2024-04-17 00:13:03.836479 speakeasy-client-sdk-python-5.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:13:03.836479 speakeasy-client-sdk-python-5.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.816479 speakeasy-client-sdk-python-5.6.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.820479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.820479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.820479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.820479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.824479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.828479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getlintingreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getrevisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/uploadreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.836479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/getnamespacesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/getrevisionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/gettagsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/preflightrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/preflighttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/v2descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.836479 speakeasy-client-sdk-python-5.6.7/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-17 00:12:55.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:13:03.836479 speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22202 2024-04-17 00:13:03.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-17 00:13:03.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:13:03.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 00:13:03.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 00:13:03.000000 speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.037419 speakeasy-client-sdk-python-5.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-04-18 00:12:21.037419 speakeasy-client-sdk-python-5.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14621 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:12:21.037419 speakeasy-client-sdk-python-5.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.021419 speakeasy-client-sdk-python-5.6.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.025419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.025419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.025419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.025419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.025419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.033419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getchangesreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getlintingreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/uploadreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.037419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/getnamespacesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/getrevisionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/gettagsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/preflightrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/preflighttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/v2descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.037419 speakeasy-client-sdk-python-5.6.8/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-18 00:12:12.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:12:21.037419 speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-04-18 00:12:20.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-18 00:12:20.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:12:20.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-18 00:12:20.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 00:12:20.000000 speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.6.7/PKG-INFO` & `speakeasy-client-sdk-python-5.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.7
+Version: 5.6.8
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -106,14 +106,15 @@
         
         ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md)
         
         * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
         
         ### [reports](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md)
         
+        * [get_changes_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_changes_report_signed_url) - Get the signed access url for the change reports for a particular document.
         * [get_linting_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_linting_report_signed_url) - Get the signed access url for the linting reports for a particular document.
         * [upload_report](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#upload_report) - Upload a report.
         
         ### [embeds](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md)
         
         * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
         * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
```

### Comparing `speakeasy-client-sdk-python-5.6.7/README.md` & `speakeasy-client-sdk-python-5.6.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
 ### [organizations](docs/sdks/organizations/README.md)
 
 * [get_organizations](docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
 
 ### [reports](docs/sdks/reports/README.md)
 
+* [get_changes_report_signed_url](docs/sdks/reports/README.md#get_changes_report_signed_url) - Get the signed access url for the change reports for a particular document.
 * [get_linting_report_signed_url](docs/sdks/reports/README.md#get_linting_report_signed_url) - Get the signed access url for the linting reports for a particular document.
 * [upload_report](docs/sdks/reports/README.md#upload_report) - Upload a report.
 
 ### [embeds](docs/sdks/embeds/README.md)
 
 * [get_embed_access_token](docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
 * [get_valid_embed_access_tokens](docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
```

### Comparing `speakeasy-client-sdk-python-5.6.7/setup.py` & `speakeasy-client-sdk-python-5.6.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.6.7',
+    version='5.6.8',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/artifacts.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/artifacts.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/auth.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/events.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .getaccesstoken import *
 from .getallapiendpoints import *
 from .getallapiversions import *
 from .getallforversionapiendpoints import *
 from .getapiendpoint import *
 from .getapis import *
 from .getblob import *
+from .getchangesreportsignedurl import *
 from .getembedaccesstoken import *
 from .getlintingreportsignedurl import *
 from .getmanifest import *
 from .getnamespaces import *
 from .getorganizations import *
 from .getrequestfromeventlog import *
 from .getrevisions import *
@@ -44,8 +45,8 @@
 from .registerschema import *
 from .revokeembedaccesstoken import *
 from .uploadreport import *
 from .upsertapi import *
 from .upsertapiendpoint import *
 from .validateapikey import *
 
-__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetBlobRequest","GetBlobResponse","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetLintingReportSignedURLRequest","GetLintingReportSignedURLResponse","GetLintingReportSignedURLSignedAccess","GetManifestRequest","GetManifestResponse","GetNamespacesResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetTagsRequest","GetTagsResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsGlobals","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaFile","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UploadReportRequestBody","UploadReportResponse","UploadReportUploadedReport","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
+__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetBlobRequest","GetBlobResponse","GetChangesReportSignedURLRequest","GetChangesReportSignedURLResponse","GetChangesReportSignedURLSignedAccess","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetLintingReportSignedURLRequest","GetLintingReportSignedURLResponse","GetLintingReportSignedURLSignedAccess","GetManifestRequest","GetManifestResponse","GetNamespacesResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetTagsRequest","GetTagsResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsGlobals","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaFile","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UploadReportRequestBody","UploadReportResponse","UploadReportUploadedReport","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
```

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getblob.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getblob.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getlintingreportsignedurl.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getlintingreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getmanifest.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getnamespaces.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getnamespaces.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getrevisions.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getrevisions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/gettags.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/preflight.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/preflight.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/uploadreport.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/uploadreport.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/annotations.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/annotations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/getrevisionsresponse.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/getrevisionsresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/manifest.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/manifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/namespace.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/namespace.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/preflighttoken.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/preflighttoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/report.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/report.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/revision.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/revision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/tag.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/tag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/v2descriptor.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/v2descriptor.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/reports.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/reports.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,68 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
+    def get_changes_report_signed_url(self, request: operations.GetChangesReportSignedURLRequest) -> operations.GetChangesReportSignedURLResponse:
+        r"""Get the signed access url for the change reports for a particular document."""
+        hook_ctx = HookContext(operation_id='getChangesReportSignedUrl', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/v1/reports/changes/{documentChecksum}', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.GetChangesReportSignedURLResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetChangesReportSignedURLSignedAccess])
+                res.signed_access = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
     def get_linting_report_signed_url(self, request: operations.GetLintingReportSignedURLRequest) -> operations.GetLintingReportSignedURLResponse:
         r"""Get the signed access url for the linting reports for a particular document."""
         hook_ctx = HookContext(operation_id='getLintingReportSignedUrl', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(base_url, '/v1/reports/linting/{documentChecksum}', request)
```

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/sdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/sdkconfiguration.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     language: str = 'python'
     openapi_doc_version: str = '0.4.0'
-    sdk_version: str = '5.6.7'
-    gen_version: str = '2.306.3'
-    user_agent: str = 'speakeasy-sdk/python 5.6.7 2.306.3 0.4.0 speakeasy-client-sdk-python'
+    sdk_version: str = '5.6.8'
+    gen_version: str = '2.308.2'
+    user_agent: str = 'speakeasy-sdk/python 5.6.8 2.308.2 0.4.0 speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.7
+Version: 5.6.8
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -106,14 +106,15 @@
         
         ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md)
         
         * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
         
         ### [reports](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md)
         
+        * [get_changes_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_changes_report_signed_url) - Get the signed access url for the change reports for a particular document.
         * [get_linting_report_signed_url](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#get_linting_report_signed_url) - Get the signed access url for the linting reports for a particular document.
         * [upload_report](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/reports/README.md#upload_report) - Upload a report.
         
         ### [embeds](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md)
         
         * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
         * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
```

### Comparing `speakeasy-client-sdk-python-5.6.7/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.6.8/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/speakeasy/models/operations/getaccesstoken.py
 src/speakeasy/models/operations/getallapiendpoints.py
 src/speakeasy/models/operations/getallapiversions.py
 src/speakeasy/models/operations/getallforversionapiendpoints.py
 src/speakeasy/models/operations/getapiendpoint.py
 src/speakeasy/models/operations/getapis.py
 src/speakeasy/models/operations/getblob.py
+src/speakeasy/models/operations/getchangesreportsignedurl.py
 src/speakeasy/models/operations/getembedaccesstoken.py
 src/speakeasy/models/operations/getlintingreportsignedurl.py
 src/speakeasy/models/operations/getmanifest.py
 src/speakeasy/models/operations/getnamespaces.py
 src/speakeasy/models/operations/getorganizations.py
 src/speakeasy/models/operations/getrequestfromeventlog.py
 src/speakeasy/models/operations/getrevisions.py
```

