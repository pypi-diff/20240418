# Comparing `tmp/shippo-3.2.6.tar.gz` & `tmp/shippo-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.2.6.tar", last modified: Wed Apr 17 13:52:52 2024, max compression
+gzip compressed data, was "shippo-3.2.7.tar", last modified: Thu Apr 18 15:39:19 2024, max compression
```

## Comparing `shippo-3.2.6.tar` & `shippo-3.2.7.tar`

### file list

```diff
@@ -1,255 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.182714 shippo-3.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-17 13:52:52.182714 shippo-3.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-17 13:52:42.000000 shippo-3.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:52:52.182714 shippo-3.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-17 13:52:42.000000 shippo-3.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.150714 shippo-3.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.154714 shippo-3.2.6/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.154714 shippo-3.2.6/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28181 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.154714 shippo-3.2.6/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.174714 shippo-3.2.6/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/carriersenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationcontentstypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationeelpfcenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationincotermenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/distanceunitenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/labelfiletypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/objectstateenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/orderstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicegrouptypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/components/weightunitenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.174714 shippo-3.2.6/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.174714 shippo-3.2.6/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.182714 shippo-3.2.6/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15361 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.182714 shippo-3.2.6/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-17 13:52:42.000000 shippo-3.2.6/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:52:52.154714 shippo-3.2.6/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-17 13:52:51.000000 shippo-3.2.6/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-17 13:52:52.000000 shippo-3.2.6/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:52:51.000000 shippo-3.2.6/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 13:52:51.000000 shippo-3.2.6/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 13:52:51.000000 shippo-3.2.6/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.791010 shippo-3.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-18 15:39:19.791010 shippo-3.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-18 15:39:11.000000 shippo-3.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:39:19.791010 shippo-3.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 15:39:11.000000 shippo-3.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.755010 shippo-3.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28181 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.779010 shippo-3.2.7/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsitemcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/instanttransactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/instanttransactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/instanttransactionrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.779010 shippo-3.2.7/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.779010 shippo-3.2.7/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.787010 shippo-3.2.7/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15361 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.787010 shippo-3.2.7/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-18 15:39:11.000000 shippo-3.2.7/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:39:19.759010 shippo-3.2.7/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 15:39:19.000000 shippo-3.2.7/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.2.6/PKG-INFO` & `shippo-3.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.6
+Version: 3.2.7
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.6/README.md` & `shippo-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/setup.py` & `shippo-3.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.2.6',
+    version='3.2.7',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `shippo-3.2.6/src/shippo/_hooks/registration.py` & `shippo-3.2.7/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.7/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/_hooks/types.py` & `shippo-3.2.7/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/addresses.py` & `shippo-3.2.7/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/batches.py` & `shippo-3.2.7/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/carrier_accounts.py` & `shippo-3.2.7/src/shippo/carrier_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.7/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/customs_declarations.py` & `shippo-3.2.7/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/customs_items.py` & `shippo-3.2.7/src/shippo/customs_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,22 +79,22 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, customs_item_base: Optional[components.CustomsItemBase] = None) -> components.CustomsItem:
+    def create(self, shippo_api_version: Optional[str] = None, customs_item_create_request: Optional[components.CustomsItemCreateRequest] = None) -> components.CustomsItem:
         r"""Create a new customs item
         Creates a new customs item object.
         """
         hook_ctx = HookContext(operation_id='CreateCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateCustomsItemRequest(
             shippo_api_version=shippo_api_version,
-            customs_item_base=customs_item_base,
+            customs_item_create_request=customs_item_create_request,
         )
         
         _globals = operations.CreateCustomsItemGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
@@ -103,15 +103,15 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsItemRequest, "customs_item_base", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsItemRequest, "customs_item_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
```

### Comparing `shippo-3.2.6/src/shippo/debug.py` & `shippo-3.2.7/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/manifests.py` & `shippo-3.2.7/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/__init__.py` & `shippo-3.2.7/src/shippo/models/components/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,28 +49,30 @@
 from .customsdeclarationeelpfcenum import *
 from .customsdeclarationincotermenum import *
 from .customsdeclarationnondeliveryoptionenum import *
 from .customsdeclarationpaginatedlist import *
 from .customsexporteridentification import *
 from .customsinvoicedcharges import *
 from .customsitem import *
-from .customsitembase import *
+from .customsitemcreaterequest import *
 from .customsitempaginatedlist import *
 from .customstaxidentification import *
 from .dangerousgoodsbiologicalmaterial import *
 from .dangerousgoodslithiumbatteries import *
 from .dangerousgoodsobject import *
 from .defaultparceltemplate import *
 from .defaultparceltemplateupdaterequest import *
 from .departmentnumber import *
 from .distanceunitenum import *
 from .dryice import *
 from .errormessage import *
 from .httpmetadata import *
-from .instanttransactionrequestbody import *
+from .instanttransactioncreaterequest import *
+from .instanttransactioncreateresponse import *
+from .instanttransactionrate import *
 from .insurance import *
 from .invoicenumber import *
 from .labelfiletypeenum import *
 from .lineitem import *
 from .lineitembase import *
 from .liverate import *
 from .liveratecreaterequest import *
@@ -129,8 +131,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunitenum import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","HTTPMetadata","InstantTransactionRequestBody","Insurance","InvoiceNumber","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","HTTPMetadata","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseMessages","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
```

### Comparing `shippo-3.2.6/src/shippo/models/components/address.py` & `shippo-3.2.7/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/addressimporter.py` & `shippo-3.2.7/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.7/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.7/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/alcohol.py` & `shippo-3.2.7/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/batch.py` & `shippo-3.2.7/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/batchshipment.py` & `shippo-3.2.7/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.7/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/billing.py` & `shippo-3.2.7/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.2.7/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.7/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/carriersenum.py` & `shippo-3.2.7/src/shippo/models/components/carriersenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/cod.py` & `shippo-3.2.7/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.2.7/src/shippo/models/components/connectexistingownaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customerreference.py` & `shippo-3.2.7/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.7/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py` & `shippo-3.2.7/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 from .addressimporter import AddressImporter
 from .customsdeclarationb13afilingoptionenum import CustomsDeclarationB13AFilingOptionEnum
 from .customsdeclarationcontentstypeenum import CustomsDeclarationContentsTypeEnum
 from .customsdeclarationeelpfcenum import CustomsDeclarationEelPfcEnum
 from .customsdeclarationincotermenum import CustomsDeclarationIncotermEnum
 from .customsdeclarationnondeliveryoptionenum import CustomsDeclarationNonDeliveryOptionEnum
-from .customsitembase import CustomsItemBase
+from .customsitemcreaterequest import CustomsItemCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Any, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -23,15 +23,15 @@
     r"""Name of the person who created the customs declaration and is responsible for the validity of all
     information provided.
     """
     contents_type: CustomsDeclarationContentsTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_type') }})
     r"""Type of goods of the shipment."""
     non_delivery_option: CustomsDeclarationNonDeliveryOptionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('non_delivery_option') }})
     r"""Indicates how the carrier should proceed in case the shipment can't be delivered."""
-    items: List[CustomsItemBase] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items') }})
+    items: List[CustomsItemCreateRequest] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items') }})
     aes_itn: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aes_itn'), 'exclude': lambda f: f is None }})
     r"""**required if eel_pfc is `AES_ITN`**<br>
     AES / ITN reference of the shipment.
     """
     b13a_filing_option: Optional[CustomsDeclarationB13AFilingOptionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_filing_option'), 'exclude': lambda f: f is None }})
     r"""B13A Option details are obtained by filing a B13A Canada Export Declaration via the Canadian Export Reporting System (CERS).
     <a href=\"https://www.cbsa-asfc.gc.ca/services/export/guide-eng.html\" target=\"_blank\" rel=\"noopener noreferrer\"> More information on reporting commercial exports from Canada. </a>
```

### Comparing `shippo-3.2.6/src/shippo/models/components/customsdeclarationeelpfcenum.py` & `shippo-3.2.7/src/shippo/models/components/customsdeclarationeelpfcenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsdeclarationincotermenum.py` & `shippo-3.2.7/src/shippo/models/components/customsdeclarationincotermenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.7/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.7/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsitem.py` & `shippo-3.2.7/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customsitembase.py` & `shippo-3.2.7/src/shippo/models/components/customsitemcreaterequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CustomsItemBase:
+class CustomsItemCreateRequest:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     r"""Text description of your item."""
     mass_unit: WeightUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     net_weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('net_weight') }})
     r"""Total weight of this item, i.e. quantity * weight per item."""
     origin_country: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('origin_country') }})
```

### Comparing `shippo-3.2.6/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.7/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.7/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.7/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.7/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.7/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.7/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.7/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/dryice.py` & `shippo-3.2.7/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/errormessage.py` & `shippo-3.2.7/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/httpmetadata.py` & `shippo-3.2.7/src/shippo/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.2.7/src/shippo/models/components/transactioncreaterequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .labelfiletypeenum import LabelFileTypeEnum
-from .shipmentcreaterequest import ShipmentCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InstantTransactionRequestBody:
-    carrier_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_account') }})
-    servicelevel_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel_token') }})
-    shipment: ShipmentCreateRequest = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment') }})
+class TransactionCreateRequest:
+    rate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate') }})
+    async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
     label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.6/src/shippo/models/components/insurance.py` & `shippo-3.2.7/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.7/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/labelfiletypeenum.py` & `shippo-3.2.7/src/shippo/models/components/labelfiletypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/lineitem.py` & `shippo-3.2.7/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/lineitembase.py` & `shippo-3.2.7/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/liverate.py` & `shippo-3.2.7/src/shippo/models/components/trackingstatus.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
+from .trackingstatusenum import TrackingStatusEnum
+from .trackingstatuslocationbase import TrackingStatusLocationBase
+from .trackingstatussubstatus import TrackingStatusSubstatus
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class LiveRate:
-    amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    r"""The value of the price for the service group, in units of currency of the sender address"""
-    amount_local: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount_local'), 'exclude': lambda f: f is None }})
-    r"""The value of the price for the service group, in the currency of the destination address"""
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    r"""The ISO 4217 currency code for the price"""
-    currency_local: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency_local'), 'exclude': lambda f: f is None }})
-    r"""The ISO 4217 currency code for the currency describing amount_local"""
-    estimated_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('estimated_days'), 'exclude': lambda f: f is None }})
-    r"""The estimated days in transit of the rate that powers the shipping option, if available."""
-    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    r"""The name of the service group being returned"""
+class TrackingStatus:
+    r"""The latest tracking information of this shipment."""
+    location: TrackingStatusLocationBase = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location') }})
+    r"""An object containing zip, city, state and country information of the tracking event."""
+    object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
+    object_updated: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    status: TrackingStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""Indicates the high level status of the shipment."""
+    status_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    r"""Date and time when the carrier scanned this tracking event. This is displayed in UTC."""
+    status_details: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_details') }})
+    r"""The human-readable description of the status."""
+    substatus: Optional[TrackingStatusSubstatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substatus'), 'exclude': lambda f: f is None }})
+    r"""A finer-grained classification of the tracking event."""
```

### Comparing `shippo-3.2.6/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/location.py` & `shippo-3.2.7/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/manifest.py` & `shippo-3.2.7/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/order.py` & `shippo-3.2.7/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/orderstatusenum.py` & `shippo-3.2.7/src/shippo/models/components/orderstatusenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parcel.py` & `shippo-3.2.7/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parcelextra.py` & `shippo-3.2.7/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.7/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.7/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.7/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/pickup.py` & `shippo-3.2.7/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/pickupbase.py` & `shippo-3.2.7/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/ponumber.py` & `shippo-3.2.7/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/rate.py` & `shippo-3.2.7/src/shippo/models/components/rate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Rate:
     amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
     r"""Final Rate price, expressed in the currency used in the sender's country."""
     amount_local: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount_local') }})
     r"""Final Rate price, expressed in the currency used in the recipient's country."""
-    attributes: List[Attributes] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attributes') }})
-    r"""An array containing specific attributes of this Rate in context of the entire shipment.
-    Attributes can be assigned `CHEAPEST`, `FASTEST`, or `BESTVALUE`.
-    """
-    carrier_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_account') }})
-    r"""Object ID of the carrier account that has been used to retrieve the rate."""
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
     r"""Currency used in the sender's country, refers to `amount`.
     The <a href=\"http://www.xe.com/iso4217.php\">official ISO 4217</a> currency codes are used, e.g. `USD` or `EUR`.
     """
     currency_local: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency_local') }})
     r"""Currency used in the recipient's country, refers to `amount_local`.
     The <a href=\"http://www.xe.com/iso4217.php\">official ISO 4217</a> currency codes are used, e.g. `USD` or \"EUR\".
     """
+    attributes: List[Attributes] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attributes') }})
+    r"""An array containing specific attributes of this Rate in context of the entire shipment.
+    Attributes can be assigned `CHEAPEST`, `FASTEST`, or `BESTVALUE`.
+    """
+    carrier_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_account') }})
+    r"""Object ID of the carrier account that has been used to retrieve the rate."""
     object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     r"""Date and time of Rate creation."""
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     r"""Unique identifier of the given Rate object."""
     object_owner: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner') }})
     r"""Username of the user who created the rate object."""
     provider: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider') }})
```

### Comparing `shippo-3.2.6/src/shippo/models/components/ratemessage.py` & `shippo-3.2.7/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/refund.py` & `shippo-3.2.7/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.7/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/rmanumber.py` & `shippo-3.2.7/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicegroup.py` & `shippo-3.2.7/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.7/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicegrouptypeenum.py` & `shippo-3.2.7/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.7/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicelevel.py` & `shippo-3.2.7/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.7/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shipment.py` & `shippo-3.2.7/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.7/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.7/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.7/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/track.py` & `shippo-3.2.7/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.7/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-from .trackingstatusenum import TrackingStatusEnum
-from .trackingstatuslocationbase import TrackingStatusLocationBase
-from .trackingstatussubstatus import TrackingStatusSubstatus
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from shippo import utils
-from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TrackingStatus:
-    r"""The latest tracking information of this shipment."""
-    location: TrackingStatusLocationBase = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location') }})
-    r"""An object containing zip, city, state and country information of the tracking event."""
-    object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
-    object_updated: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    status: TrackingStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""Indicates the high level status of the shipment."""
-    status_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    r"""Date and time when the carrier scanned this tracking event. This is displayed in UTC."""
-    status_details: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_details') }})
-    r"""The human-readable description of the status."""
-    substatus: Optional[TrackingStatusSubstatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substatus'), 'exclude': lambda f: f is None }})
+class TrackingStatusSubstatus:
     r"""A finer-grained classification of the tracking event."""
+    code: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code') }})
+    r"""A code that represents the substatus of the shipment. See the <a href=\\"https://docs.goshippo.com/docs/tracking/tracking/#event-definitions\\">Event Definitions</a> for more information."""
+    text: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text') }})
+    r"""A human-readable description of the substatus. See the <a href=\\"https://docs.goshippo.com/docs/tracking/tracking/#event-definitions\\">Event Definitions</a> for more information."""
+    action_required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action_required') }})
+    r"""Indicates whether the substatus requires action from the shipper or recipient to complete delivery."""
```

### Comparing `shippo-3.2.6/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.7/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.7/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/transaction.py` & `shippo-3.2.7/src/shippo/models/components/transaction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,27 +54,27 @@
     r"""Indicates the validity of the enclosing object"""
     object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of last Transaction update."""
     qr_code_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('qr_code_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing directly to the QR code in PNG format.
     A value will only be returned if requested using qr_code_requested flag and the carrier provides such an option.
     """
-    rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
-    r"""ID of the Rate object for which a Label has to be obtained.
-    Please note that only rates that are not older than 7 days can be purchased in order to ensure up-to-date pricing.
-    """
     status: Optional[TransactionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""Indicates the status of the Transaction."""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
     tracking_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_number'), 'exclude': lambda f: f is None }})
     r"""The carrier-specific tracking number that can be used to track the Shipment.
     A value will only be returned if the Rate is for a trackable Shipment and if the Transactions has been processed successfully.
     """
     tracking_status: Optional[TrackingStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
     r"""Indicates the high level status of the shipment."""
     tracking_url_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_url_provider'), 'exclude': lambda f: f is None }})
     r"""A link to track this item on the carrier-provided tracking website.
     A value will only be returned if tracking is available and the carrier provides such a service.
     """
+    rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
+    r"""ID of the Rate object for which a Label has to be obtained.
+    Please note that only rates that are not older than 7 days can be purchased in order to ensure up-to-date pricing.
+    """
```

### Comparing `shippo-3.2.6/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .labelfiletypeenum import LabelFileTypeEnum
+from .transaction import Transaction
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TransactionCreateRequest:
-    rate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate') }})
-    async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
-    label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
-    r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
-    <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
-    """
-    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+class TransactionPaginatedList:
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+    results: Optional[List[Transaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.6/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.7/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .transaction import Transaction
-from dataclasses_json import Undefined, dataclass_json
-from shippo import utils
-from typing import List, Optional
+from typing import Optional
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TransactionPaginatedList:
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    results: Optional[List[Transaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+class ListCustomsDeclarationsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListCustomsDeclarationsRequest:
+    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""The page number you want to select"""
+    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100, default 5)"""
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.6/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.7/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.7/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.7/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.2.7/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.2.7/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.7/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/__init__.py` & `shippo-3.2.7/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.7/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createaddress.py` & `shippo-3.2.7/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createbatch.py` & `shippo-3.2.7/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.7/src/shippo/models/operations/createcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.7/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.7/src/shippo/models/operations/createcustomsitem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import customsitembase as components_customsitembase
+from ...models.components import customsitemcreaterequest as components_customsitemcreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateCustomsItemGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
@@ -14,11 +14,11 @@
 
 
 
 @dataclasses.dataclass
 class CreateCustomsItemRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    customs_item_base: Optional[components_customsitembase.CustomsItemBase] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    customs_item_create_request: Optional[components_customsitemcreaterequest.CustomsItemCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""CustomsItem details."""
```

### Comparing `shippo-3.2.6/src/shippo/models/operations/createliverate.py` & `shippo-3.2.7/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.7/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createorder.py` & `shippo-3.2.7/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createparcel.py` & `shippo-3.2.7/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createpickup.py` & `shippo-3.2.7/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createrefund.py` & `shippo-3.2.7/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.7/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createshipment.py` & `shippo-3.2.7/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.2.7/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createtrack.py` & `shippo-3.2.7/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.7/src/shippo/models/operations/createtransaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import instanttransactionrequestbody as components_instanttransactionrequestbody
+from ...models.components import instanttransactioncreaterequest as components_instanttransactioncreaterequest
 from ...models.components import transactioncreaterequest as components_transactioncreaterequest
 from typing import Optional, Union
 
 
 @dataclasses.dataclass
 class CreateTransactionGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
@@ -15,11 +15,11 @@
 
 
 
 @dataclasses.dataclass
 class CreateTransactionRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    request_body: Optional[Union[components_transactioncreaterequest.TransactionCreateRequest, components_instanttransactionrequestbody.InstantTransactionRequestBody]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    request_body: Optional[Union[components_transactioncreaterequest.TransactionCreateRequest, components_instanttransactioncreaterequest.InstantTransactionCreateRequest]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Examples."""
```

### Comparing `shippo-3.2.6/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.7/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getaddress.py` & `shippo-3.2.7/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getbatch.py` & `shippo-3.2.7/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.7/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.7/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.7/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.7/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.7/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getorder.py` & `shippo-3.2.7/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getparcel.py` & `shippo-3.2.7/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getrate.py` & `shippo-3.2.7/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getrefund.py` & `shippo-3.2.7/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getshipment.py` & `shippo-3.2.7/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.7/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/gettrack.py` & `shippo-3.2.7/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.7/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.2.7/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.7/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.7/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.7/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.7/src/shippo/models/operations/listshipments.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListCustomsDeclarationsGlobals:
+class ListShipmentsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListCustomsDeclarationsRequest:
+class ListShipmentsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100, default 5)"""
+    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.6/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.7/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.7/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listorders.py` & `shippo-3.2.7/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listparcels.py` & `shippo-3.2.7/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listrefunds.py` & `shippo-3.2.7/src/shippo/models/operations/listrefunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listservicegroups.py` & `shippo-3.2.7/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.7/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.7/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listshipments.py` & `shippo-3.2.7/src/shippo/models/operations/listshippoaccounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShipmentsGlobals:
+class ListShippoAccountsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListShipmentsRequest:
+class ListShippoAccountsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.6/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.7/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ...models.components import userparceltemplateupdaterequest as components_userparceltemplateupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShippoAccountsGlobals:
+class UpdateUserParcelTemplateGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListShippoAccountsRequest:
-    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+class UpdateUserParcelTemplateRequest:
+    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the user parcel template"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
+    user_parcel_template_update_request: Optional[components_userparceltemplateupdaterequest.UserParcelTemplateUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.6/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.7/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.2.7/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/purchasebatch.py` & `shippo-3.2.7/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.7/src/shippo/models/operations/registercarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.7/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.7/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.7/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.7/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.7/src/shippo/models/operations/validateaddress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import userparceltemplateupdaterequest as components_userparceltemplateupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class UpdateUserParcelTemplateGlobals:
+class ValidateAddressGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class UpdateUserParcelTemplateRequest:
-    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the user parcel template"""
+class ValidateAddressRequest:
+    address_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'AddressId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the address"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    user_parcel_template_update_request: Optional[components_userparceltemplateupdaterequest.UserParcelTemplateUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.6/src/shippo/orders.py` & `shippo-3.2.7/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/parcels.py` & `shippo-3.2.7/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/pickups.py` & `shippo-3.2.7/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/rates.py` & `shippo-3.2.7/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/rates_at_checkout.py` & `shippo-3.2.7/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/refunds.py` & `shippo-3.2.7/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/sdk.py` & `shippo-3.2.7/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/sdkconfiguration.py` & `shippo-3.2.7/src/shippo/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.2.6'
-    gen_version: str = '2.306.3'
-    user_agent: str = 'speakeasy-sdk/python 3.2.6 2.306.3 2018-02-08 shippo'
+    sdk_version: str = '3.2.7'
+    gen_version: str = '2.309.2'
+    user_agent: str = 'speakeasy-sdk/python 3.2.7 2.309.2 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.2.6/src/shippo/service_groups.py` & `shippo-3.2.7/src/shippo/service_groups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/shipments.py` & `shippo-3.2.7/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/shippo_accounts.py` & `shippo-3.2.7/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/tracking_status.py` & `shippo-3.2.7/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/transactions.py` & `shippo-3.2.7/src/shippo/transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, request_body: Optional[Union[components.TransactionCreateRequest, components.InstantTransactionRequestBody]] = None) -> components.Transaction:
+    def create(self, shippo_api_version: Optional[str] = None, request_body: Optional[Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest]] = None) -> Union[components.Transaction, components.InstantTransactionCreateResponse]:
         r"""Create a shipping label
         Creates a new transaction object and purchases the shipping label using a rate object that has previously been created. <br> OR <br> Creates a new transaction object and purchases the shipping label instantly using shipment details, an existing carrier account, and an existing service level token.
         """
         hook_ctx = HookContext(operation_id='CreateTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateTransactionRequest(
             shippo_api_version=shippo_api_version,
             request_body=request_body,
@@ -128,15 +128,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Transaction])
+                out = utils.unmarshal_json(http_res.text, Optional[Union[components.Transaction, components.InstantTransactionCreateResponse]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.2.6/src/shippo/user_parcel_templates.py` & `shippo-3.2.7/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/utils/retries.py` & `shippo-3.2.7/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo/utils/utils.py` & `shippo-3.2.7/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.6/src/shippo.egg-info/PKG-INFO` & `shippo-3.2.7/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.6
+Version: 3.2.7
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.6/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.7/src/shippo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,28 +83,30 @@
 src/shippo/models/components/customsdeclarationeelpfcenum.py
 src/shippo/models/components/customsdeclarationincotermenum.py
 src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
 src/shippo/models/components/customsdeclarationpaginatedlist.py
 src/shippo/models/components/customsexporteridentification.py
 src/shippo/models/components/customsinvoicedcharges.py
 src/shippo/models/components/customsitem.py
-src/shippo/models/components/customsitembase.py
+src/shippo/models/components/customsitemcreaterequest.py
 src/shippo/models/components/customsitempaginatedlist.py
 src/shippo/models/components/customstaxidentification.py
 src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
 src/shippo/models/components/dangerousgoodslithiumbatteries.py
 src/shippo/models/components/dangerousgoodsobject.py
 src/shippo/models/components/defaultparceltemplate.py
 src/shippo/models/components/defaultparceltemplateupdaterequest.py
 src/shippo/models/components/departmentnumber.py
 src/shippo/models/components/distanceunitenum.py
 src/shippo/models/components/dryice.py
 src/shippo/models/components/errormessage.py
 src/shippo/models/components/httpmetadata.py
-src/shippo/models/components/instanttransactionrequestbody.py
+src/shippo/models/components/instanttransactioncreaterequest.py
+src/shippo/models/components/instanttransactioncreateresponse.py
+src/shippo/models/components/instanttransactionrate.py
 src/shippo/models/components/insurance.py
 src/shippo/models/components/invoicenumber.py
 src/shippo/models/components/labelfiletypeenum.py
 src/shippo/models/components/lineitem.py
 src/shippo/models/components/lineitembase.py
 src/shippo/models/components/liverate.py
 src/shippo/models/components/liveratecreaterequest.py
```

