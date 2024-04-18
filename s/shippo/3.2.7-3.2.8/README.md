# Comparing `tmp/shippo-3.2.7.tar.gz` & `tmp/shippo-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.2.7.tar", last modified: Thu Apr 18 15:39:19 2024, max compression
+gzip compressed data, was "shippo-3.2.8.tar", last modified: Thu Apr 18 16:17:55 2024, max compression
```

## Comparing `shippo-3.2.7.tar` & `shippo-3.2.8.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.791010 shippo-3.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-18 15:39:19.791010 shippo-3.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-18 15:39:11.000000 shippo-3.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:39:19.791010 shippo-3.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 15:39:11.000000 shippo-3.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.755010 shippo-3.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28181 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.779010 shippo-3.2.7/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carriersenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationcontentstypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationeelpfcenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationincotermenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsitemcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/distanceunitenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/instanttransactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/instanttransactioncreateresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/instanttransactionrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/labelfiletypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/objectstateenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/orderstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegrouptypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/weightunitenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.779010 shippo-3.2.7/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.779010 shippo-3.2.7/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.787010 shippo-3.2.7/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15361 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.787010 shippo-3.2.7/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.149231 shippo-3.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-18 16:17:55.149231 shippo-3.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-18 16:17:46.000000 shippo-3.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:17:55.149231 shippo-3.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 16:17:46.000000 shippo-3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.113231 shippo-3.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.117231 shippo-3.2.8/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.121231 shippo-3.2.8/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28181 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.121231 shippo-3.2.8/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.137231 shippo-3.2.8/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsitemcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/instanttransactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/instanttransactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/instanttransactionrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.137231 shippo-3.2.8/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.141231 shippo-3.2.8/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.149231 shippo-3.2.8/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15361 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.149231 shippo-3.2.8/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-18 16:17:46.000000 shippo-3.2.8/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:17:55.121231 shippo-3.2.8/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-18 16:17:55.000000 shippo-3.2.8/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-18 16:17:55.000000 shippo-3.2.8/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:17:55.000000 shippo-3.2.8/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 16:17:55.000000 shippo-3.2.8/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 16:17:55.000000 shippo-3.2.8/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.2.7/PKG-INFO` & `shippo-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.7
+Version: 3.2.8
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.7/README.md` & `shippo-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/setup.py` & `shippo-3.2.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.2.7',
+    version='3.2.8',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `shippo-3.2.7/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.8/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/_hooks/types.py` & `shippo-3.2.8/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/addresses.py` & `shippo-3.2.8/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/batches.py` & `shippo-3.2.8/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/carrier_accounts.py` & `shippo-3.2.8/src/shippo/carrier_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.8/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/customs_declarations.py` & `shippo-3.2.8/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/customs_items.py` & `shippo-3.2.8/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/debug.py` & `shippo-3.2.8/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/manifests.py` & `shippo-3.2.8/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/__init__.py` & `shippo-3.2.8/src/shippo/models/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,8 +131,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunitenum import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","HTTPMetadata","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseMessages","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","HTTPMetadata","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseMessages","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
```

### Comparing `shippo-3.2.7/src/shippo/models/components/address.py` & `shippo-3.2.8/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/addressimporter.py` & `shippo-3.2.8/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.8/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.8/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/alcohol.py` & `shippo-3.2.8/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/batch.py` & `shippo-3.2.8/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/batchshipment.py` & `shippo-3.2.8/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.8/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/billing.py` & `shippo-3.2.8/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.2.8/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.8/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/carriersenum.py` & `shippo-3.2.8/src/shippo/models/components/carriersenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/cod.py` & `shippo-3.2.8/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.2.8/src/shippo/models/components/connectexistingownaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customerreference.py` & `shippo-3.2.8/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.8/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py` & `shippo-3.2.8/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsdeclarationeelpfcenum.py` & `shippo-3.2.8/src/shippo/models/components/customsdeclarationeelpfcenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsdeclarationincotermenum.py` & `shippo-3.2.8/src/shippo/models/components/customsdeclarationincotermenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.8/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.8/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsitem.py` & `shippo-3.2.8/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsitemcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/customsitemcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.8/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.8/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.8/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.8/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.8/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.8/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.8/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/dryice.py` & `shippo-3.2.8/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/errormessage.py` & `shippo-3.2.8/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/httpmetadata.py` & `shippo-3.2.8/src/shippo/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/instanttransactioncreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/instanttransactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/instanttransactioncreateresponse.py` & `shippo-3.2.8/src/shippo/models/components/instanttransactioncreateresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 from .instanttransactionrate import InstantTransactionRate
 from .labelfiletypeenum import LabelFileTypeEnum
 from .objectstateenum import ObjectStateEnum
 from .trackingstatusenum import TrackingStatusEnum
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
+from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class InstantTransactionCreateResponseMessages:
     pass
 
+class InstantTransactionCreateResponseResponseType(str, Enum):
+    INSTANT = 'instant'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InstantTransactionCreateResponse:
     commercial_invoice_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing to the commercial invoice as a 8.5x11 inch PDF file.
     A value will only be returned if the Transactions has been processed successfully and if the shipment is international.
@@ -70,9 +74,10 @@
     tracking_status: Optional[TrackingStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
     r"""Indicates the high level status of the shipment."""
     tracking_url_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_url_provider'), 'exclude': lambda f: f is None }})
     r"""A link to track this item on the carrier-provided tracking website.
     A value will only be returned if tracking is available and the carrier provides such a service.
     """
     rate: Optional[InstantTransactionRate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
+    response_type: Optional[InstantTransactionCreateResponseResponseType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.7/src/shippo/models/components/instanttransactionrate.py` & `shippo-3.2.8/src/shippo/models/components/instanttransactionrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/insurance.py` & `shippo-3.2.8/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.8/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/labelfiletypeenum.py` & `shippo-3.2.8/src/shippo/models/components/labelfiletypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/lineitem.py` & `shippo-3.2.8/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/lineitembase.py` & `shippo-3.2.8/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/liverate.py` & `shippo-3.2.8/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/location.py` & `shippo-3.2.8/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/manifest.py` & `shippo-3.2.8/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/order.py` & `shippo-3.2.8/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/orderstatusenum.py` & `shippo-3.2.8/src/shippo/models/components/orderstatusenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parcel.py` & `shippo-3.2.8/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parcelextra.py` & `shippo-3.2.8/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.8/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.8/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.8/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/pickup.py` & `shippo-3.2.8/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/pickupbase.py` & `shippo-3.2.8/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/ponumber.py` & `shippo-3.2.8/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/rate.py` & `shippo-3.2.8/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/ratemessage.py` & `shippo-3.2.8/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/refund.py` & `shippo-3.2.8/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.8/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/rmanumber.py` & `shippo-3.2.8/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicegroup.py` & `shippo-3.2.8/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.8/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicegrouptypeenum.py` & `shippo-3.2.8/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.8/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicelevel.py` & `shippo-3.2.8/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.8/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shipment.py` & `shippo-3.2.8/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.8/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.8/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.8/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/track.py` & `shippo-3.2.8/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.8/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.8/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.2.8/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.8/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/transaction.py` & `shippo-3.2.8/src/shippo/models/components/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 import dateutil.parser
 from .labelfiletypeenum import LabelFileTypeEnum
 from .objectstateenum import ObjectStateEnum
 from .trackingstatusenum import TrackingStatusEnum
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
+from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class TransactionMessages:
     pass
 
+class ResponseType(str, Enum):
+    STANDARD = 'standard'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Transaction:
     commercial_invoice_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing to the commercial invoice as a 8.5x11 inch PDF file.
     A value will only be returned if the Transactions has been processed successfully and if the shipment is international.
@@ -72,9 +76,10 @@
     r"""A link to track this item on the carrier-provided tracking website.
     A value will only be returned if tracking is available and the carrier provides such a service.
     """
     rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
     r"""ID of the Rate object for which a Label has to be obtained.
     Please note that only rates that are not older than 7 days can be purchased in order to ensure up-to-date pricing.
     """
+    response_type: Optional[ResponseType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.7/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.8/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.8/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.8/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.8/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.2.8/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.2.8/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.8/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/__init__.py` & `shippo-3.2.8/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.8/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createaddress.py` & `shippo-3.2.8/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createbatch.py` & `shippo-3.2.8/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.8/src/shippo/models/operations/createcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.8/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.8/src/shippo/models/operations/createcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createliverate.py` & `shippo-3.2.8/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.8/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createorder.py` & `shippo-3.2.8/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createparcel.py` & `shippo-3.2.8/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createpickup.py` & `shippo-3.2.8/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createrefund.py` & `shippo-3.2.8/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.8/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createshipment.py` & `shippo-3.2.8/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.2.8/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createtrack.py` & `shippo-3.2.8/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.8/src/shippo/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.8/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getaddress.py` & `shippo-3.2.8/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getbatch.py` & `shippo-3.2.8/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.8/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.8/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.8/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.8/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.8/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getorder.py` & `shippo-3.2.8/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getparcel.py` & `shippo-3.2.8/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getrate.py` & `shippo-3.2.8/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getrefund.py` & `shippo-3.2.8/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getshipment.py` & `shippo-3.2.8/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.8/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/gettrack.py` & `shippo-3.2.8/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.8/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.2.8/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.8/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.8/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.8/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.8/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.8/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.8/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listorders.py` & `shippo-3.2.8/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listparcels.py` & `shippo-3.2.8/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listrefunds.py` & `shippo-3.2.8/src/shippo/models/operations/listrefunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listservicegroups.py` & `shippo-3.2.8/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.8/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.8/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listshipments.py` & `shippo-3.2.8/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.8/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.8/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.2.8/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/purchasebatch.py` & `shippo-3.2.8/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.8/src/shippo/models/operations/registercarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.8/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.8/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.8/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.8/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.8/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/models/operations/validateaddress.py` & `shippo-3.2.8/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/orders.py` & `shippo-3.2.8/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/parcels.py` & `shippo-3.2.8/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/pickups.py` & `shippo-3.2.8/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/rates.py` & `shippo-3.2.8/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/rates_at_checkout.py` & `shippo-3.2.8/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/refunds.py` & `shippo-3.2.8/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/sdk.py` & `shippo-3.2.8/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/sdkconfiguration.py` & `shippo-3.2.8/src/shippo/sdkconfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.2.7'
-    gen_version: str = '2.309.2'
-    user_agent: str = 'speakeasy-sdk/python 3.2.7 2.309.2 2018-02-08 shippo'
+    sdk_version: str = '3.2.8'
+    gen_version: str = '2.310.0'
+    user_agent: str = 'speakeasy-sdk/python 3.2.8 2.310.0 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.2.7/src/shippo/service_groups.py` & `shippo-3.2.8/src/shippo/service_groups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/shipments.py` & `shippo-3.2.8/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/shippo_accounts.py` & `shippo-3.2.8/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/tracking_status.py` & `shippo-3.2.8/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/transactions.py` & `shippo-3.2.8/src/shippo/transactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/user_parcel_templates.py` & `shippo-3.2.8/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/utils/retries.py` & `shippo-3.2.8/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo/utils/utils.py` & `shippo-3.2.8/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.7/src/shippo.egg-info/PKG-INFO` & `shippo-3.2.8/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.7
+Version: 3.2.8
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.7/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.8/src/shippo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

