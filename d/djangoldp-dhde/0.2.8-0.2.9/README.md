# Comparing `tmp/djangoldp_dhde-0.2.8.tar.gz` & `tmp/djangoldp_dhde-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_dhde-0.2.8.tar", last modified: Mon Oct 31 11:22:53 2022, max compression
+gzip compressed data, was "dist/djangoldp_dhde-0.2.9.tar", last modified: Mon Oct 31 11:33:43 2022, max compression
```

## Comparing `djangoldp_dhde-0.2.8.tar` & `djangoldp_dhde-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)      105 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/
--rw-rw-rw-   0 root         (0) root         (0)      201 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      680 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)    12331 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)     2421 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)     1708 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)      952 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     2825 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      910 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)    12675 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2990 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/admin/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     2709 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)    13126 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)     2212 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-10-31 11:22:51.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/djangoldp_dhde/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-10-31 11:22:35.000000 djangoldp_dhde-0.2.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      561 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      313 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/
--rw-r--r--   0 root         (0) root         (0)      313 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      990 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-10-31 11:22:53.000000 djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      680 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)    12355 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      952 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2825 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      910 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)    12698 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/admin/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)    13195 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/password/email.html
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)       46 2022-10-31 11:33:40.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/djangoldp_dhde/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2022-10-31 11:33:24.000000 djangoldp_dhde-0.2.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      561 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      313 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 11:33:43.000000 djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      313 2022-10-31 11:33:42.000000 djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-31 11:33:42.000000 djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      990 2022-10-31 11:33:42.000000 djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-10-31 11:33:42.000000 djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-10-31 11:33:42.000000 djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/requires.txt
```

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_done.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_email.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_email.html`

 * *Files 1% similar despite different names*

```diff
@@ -78,24 +78,24 @@
                       <td style="font-family: sans-serif; font-size: 14px; vertical-align: top;" valign="top">
                         <img class="img-responsive" src="https://dhde.spacecoop.eu/img/DHDE_logo_transparent.png" alt="{% orbit 'client.name' %}" width="200" border="0" bgcolor="#f6f6f6">
                       </td>
                     </tr>
                     <tr>
                       <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 0;" valign="top">
                         <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px;">Dear {% firstof user.first_name user.username %},</p>
-                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px; font-style: italic;">You can set your new password clicking on the following link: <a href="{{ protocol }}://{{ domain }}{% url 'password_reset_confirm' uidb64=uid token=token %}">{{ protocol }}://{{ domain }}{% url 'password_reset_confirm' uidb64=uid token=token %}</a></p>
+                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px; font-style: italic;">You can set your new password clicking on the following link: <a  style="color: #00aca8" href="{{ protocol }}://{{ domain }}{% url 'password_reset_confirm' uidb64=uid token=token %}">{{ protocol }}://{{ domain }}{% url 'password_reset_confirm' uidb64=uid token=token %}</a></p>
                         <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px;"> or just clicking the button below: </p>
                         <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; box-sizing: border-box; width: 100%;" width="100%">
                           <tbody>
                             <tr>
                               <td align="left" style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 15px; padding-top: 15px;" valign="top">
                                 <table role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; width: auto;">
                                   <tbody>
                                     <tr>
-                                      <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; border-radius: 5px; text-align: center; background-color: #960136; color:white" valign="top" align="center" bgcolor="#960136"> <a href="{{ protocol }}://{{ domain }}{% url 'password_reset_confirm' uidb64=uid token=token %}" target="_blank" style="border: solid 1px #220039; border-radius: 5px; box-sizing: border-box; cursor: pointer; display: inline-block; font-size: 14px; font-weight: bold; margin: 0; padding: 12px 25px; text-decoration: none; text-transform: capitalize; background-color: #960136; border-color: #220039; color: #EEEEEC;">Reset Password</a></td>
+                                      <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; border-radius: 5px; text-align: center; background-color: #00aca8; color:white" valign="top" align="center" bgcolor="#00aca8"> <a href="{{ protocol }}://{{ domain }}{% url 'password_reset_confirm' uidb64=uid token=token %}" target="_blank" style="border: solid 1px #220039; border-radius: 5px; box-sizing: border-box; cursor: pointer; display: inline-block; font-size: 14px; font-weight: bold; margin: 0; padding: 12px 25px; text-decoration: none; text-transform: capitalize; background-color: #00aca8; border-color: #220039; color: #EEEEEC;">Reset Password</a></td>
                                     </tr>
                                   </tbody>
                                 </table>
                               </td>
                             </tr>
                           </tbody>
                         </table>
@@ -134,15 +134,15 @@
                           <tbody>
                             <tr>
                               <td align="center" style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-top: 15px;" valign="top">
                                 <table role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; width: auto;">
                                   <tbody>
                                     <tr>
                                       <td align="center" valign="middle" style="border-collapse:collapse;font-size:1px;line-height:1px;padding:10px; padding:0px 18px 0px;text-align:left;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:14px">
-                                        <a class="link" style="font-size: 0.8em;color:#8B5EDE;" href="https://dhde.spacecoop.eu/legal_T&amp;C.html">Terms &amp; Conditions</a>&nbsp;&nbsp;&nbsp;-&nbsp;&nbsp;&nbsp;<a class="link" style="font-size: 0.8em;color: #8B5EDE;" href="https://dhde.spacecoop.eu/legal_DPP.html">Privacy Policy</a>
+                                        <a class="link" style="font-size: 0.8em;color:#00aca8;" href="https://dhde.spacecoop.eu/legal_T&amp;C.html">Terms &amp; Conditions</a>&nbsp;&nbsp;&nbsp;-&nbsp;&nbsp;&nbsp;<a class="link" style="font-size: 0.8em;color: #00aca8;" href="https://dhde.spacecoop.eu/legal_DPP.html">Privacy Policy</a>
                                       </td>
                                     </tr>
                                   </tbody>
                                 </table>
                               </td>
                             </tr>
                           </tbody>
```

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_confirm.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_form.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_reset_complete.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/login.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/registration/password_change_done.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/email.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/email.html`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
           height: auto !important;
           max-width: 100% !important;
           width: auto !important;
         }
       }
       @media all {
         .btn-primary table td:hover {
-          background-color: #8B5EDE !important;
+          background-color: #00aca8 !important;
         }
         .btn-primary a:hover {
-          background-color: #8B5EDE !important;
-          border-color: #8B5EDE !important;
+          background-color: #00aca8 !important;
+          border-color: #00aca8 !important;
         }
       }
     </style>
   </head>
   <body style="background-color: #140651; font-family: sans-serif; -webkit-font-smoothing: antialiased; font-size: 14px; line-height: 1.4; margin: 0; padding: 0; -ms-text-size-adjust: 100%; -webkit-text-size-adjust: 100%;" bgcolor="#140651">
     <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="body" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #140651; width: 100%;" width="100%" bgcolor="#140651">
       <tr>
@@ -81,15 +81,15 @@
                       </td>
                     </tr>
                     <tr>
                       <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 0;" valign="top">
                         <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px;"><b>{{ author }}</b> {{ object }} through the <a href="https://dhde.community.spacecoop.eu/">Digital Health from Space Community Platform</a></p>
                         <p style="padding: 10px; font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 30px; margin-top: 30px;">{{ instance.summary }}</p>
                         <hr />
-                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px; font-style: italic;"> To read the whole message or answer, first connect to the community: <a href="https://dhde.community.spacecoop.eu/">https://dhde.community.spacecoop.eu/</a> and click on the notification bell at top right corner</p>
+                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px; font-style: italic;"> To read the whole message or answer, first connect to the community: <a href="https://dhde.community.spacecoop.eu/" style="color: #00aca8">https://dhde.community.spacecoop.eu/</a> and click on the notification bell at top right corner</p>
                         <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 15px; font-style: italic;"> Please, do not reply directly to this e-mail. We will ignore it.</p>
                         <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; box-sizing: border-box; width: 100%;" width="100%">
                           <tbody>
                             <tr>
                               <td align="left" style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 15px; padding-top: 15px;" valign="top">
                                 <table role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; width: auto;">
                                   <tbody>
@@ -106,27 +106,27 @@
                           <tbody>
                             <tr>
                               <td align="center" style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-top: 15px;" valign="top">
                                 <table role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; width: auto;">
                                   <tbody>
                                     <tr>
                                       <td align="left" valign="middle" style="border-collapse:collapse;font-size:1px;line-height:1px;padding:10px;">
-                                        <a class="fallback-innerfont" href="https://www.linkedin.com/company/space-cooperative-europe-sce/" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#8B5EDE;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
+                                        <a class="fallback-innerfont" href="https://www.linkedin.com/company/space-cooperative-europe-sce/" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#00aca8;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
                                           <img class="nobreak" src="https://dhde.spacecoop.eu/img/linkedin.png" alt="" width="24" height="24" style="border:none;width:24px;max-width:24px;height:24px;">
                                         </a>
-                                        <a class="fallback-innerfont" href="https://twitter.com/SCE2_SpaceHub" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#8B5EDE;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
+                                        <a class="fallback-innerfont" href="https://twitter.com/SCE2_SpaceHub" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#00aca8;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
                                           <img class="nobreak" src="https://dhde.spacecoop.eu/img/twitter.png" alt="" width="24" height="24" style="border:none;width:24px;max-width:24px;height:24px;">
                                         </a>
-                                        <a class="fallback-innerfont" href="https://www.facebook.com/SpaceCooperativeEuropeSCE/" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#8B5EDE;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
+                                        <a class="fallback-innerfont" href="https://www.facebook.com/SpaceCooperativeEuropeSCE/" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#00aca8;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
                                           <img class="nobreak" src="https://dhde.spacecoop.eu/img/facebook.png" alt="" width="24" height="24" style="border:none;width:24px;max-width:24px;height:24px;">
                                         </a>
-                                        <a class="fallback-innerfont" href="https://www.instagram.com/spacecooperativeeurope/" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#8B5EDE;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
+                                        <a class="fallback-innerfont" href="https://www.instagram.com/spacecooperativeeurope/" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#00aca8;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
                                           <img class="nobreak" src="https://dhde.spacecoop.eu/img/instagram.png" alt="" width="24" height="24" style="border:none;width:24px;max-width:24px;height:24px;">
                                         </a>
-                                        <a class="fallback-innerfont" href="mailto:dhde.community@spacecoop.eu" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#8B5EDE;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
+                                        <a class="fallback-innerfont" href="mailto:dhde.community@spacecoop.eu" target="_blank" style="display:inline-block;padding:6px!important;text-decoration:none;color:#00aca8;font-family:Arimo, Arial, Helvetica, sans-serif;font-size:16px;">
                                           <img class="nobreak" src="https://dhde.spacecoop.eu/img/mail.png" alt="" width="24" height="24" style="border:none;width:24px;max-width:24px;height:24px;">
                                         </a>
                                       </td>
                                     </tr>
                                   </tbody>
                                 </table>
                               </td>
```

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/admin/login.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/oidc_provider/authorize.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/password/email.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/password/email.html`

 * *Files 8% similar despite different names*

```diff
@@ -52,19 +52,19 @@
           height: auto !important;
           max-width: 100% !important;
           width: auto !important;
         }
       }
       @media all {
         .btn-primary table td:hover {
-          background-color: #8B5EDE !important;
+          background-color: #00aca8 !important;
         }
         .btn-primary a:hover {
-          background-color: #8B5EDE !important;
-          border-color: #8B5EDE !important;
+          background-color: #00aca8 !important;
+          border-color: #00aca8 !important;
         }
       }
     </style>
   </head>
   <body style="background-color: #140651; font-family: sans-serif; -webkit-font-smoothing: antialiased; font-size: 14px; line-height: 1.4; margin: 0; padding: 0; -ms-text-size-adjust: 100%; -webkit-text-size-adjust: 100%;" bgcolor="#140651">
     <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="body" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #140651; width: 100%;" width="100%" bgcolor="#140651">
       <tr>
@@ -79,17 +79,17 @@
                       <td style="font-family: sans-serif; font-size: 14px; vertical-align: top;" valign="top">
                         <img class="img-responsive" src="https://dhde.spacecoop.eu/img/DHDE_logo_transparent.png" alt="{% orbit 'client.name' %}" width="200" border="0" bgcolor="#f6f6f6">
                       </td>
                     </tr>
                     <tr>
                       <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 0;" valign="top">
                         <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 20px;">Dear {% firstof instance.first_name instance.username %},</p>
-                        <p style="font-family: sans-serif; font-size: 12px; font-weight: normal; margin: 0; margin-bottom: 20px; font-style: italic;">We have just created an account for you on the <a href="https://dhde.community.spacecoop.eu/">Digital Health from Space Community Platform</a>.</p>
-                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 20px;">To activate it. Please, first of all click <a href="{{ password_link }}">here</a> to define your password (<a href="{{ password_link }}">{{ password_link }}</a>) and then follow the instructions we will send to your email.</p>
-                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 20px;">Once your password is defined, your account is activated and you can log in <a href="https://dhde.community.spacecoop.eu/">here</a> (<a href="https://dhde.community.spacecoop.eu/">https://dhde.community.spacecoop.eu/</a>). Then you can define your profile filling some information about you and uploading your ID picture</p>
+                        <p style="font-family: sans-serif; font-size: 12px; font-weight: normal; margin: 0; margin-bottom: 20px; font-style: italic;">We have just created an account for you on the <a style="color: #00aca8" href="https://dhde.community.spacecoop.eu/">Digital Health from Space Community Platform</a>.</p>
+                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 20px;">To activate it. Please, first of all click <a style="color: #00aca8" href="{{ password_link }}">here</a> to define your password (<a href="{{ password_link }}">{{ password_link }}</a>) and then follow the instructions we will send to your email.</p>
+                        <p style="font-family: sans-serif; font-size: 14px; font-weight: normal; margin: 0; margin-bottom: 20px;">Once your password is defined, your account is activated and you can log in <a style="color: #00aca8" href="https://dhde.community.spacecoop.eu/">here</a> (<a href="https://dhde.community.spacecoop.eu/">https://dhde.community.spacecoop.eu/</a>). Then you can define your profile filling some information about you and uploading your ID picture</p>
                         <hr />
                         <p style="font-family: sans-serif; font-size: 12px; font-weight: normal; margin: 0; margin-bottom: 20px; font-style: italic;"> - Please, do not reply directly to this e-mail</p>
                         <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; box-sizing: border-box; width: 100%;" width="100%">
                           <tbody>
                             <tr>
                               <td align="left" style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 15px; padding-top: 15px;" valign="top">
                                 <table role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; width: auto;">
```

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde/templates/base.html` & `djangoldp_dhde-0.2.9/djangoldp_dhde/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/setup.cfg` & `djangoldp_dhde-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_dhde-0.2.8/djangoldp_dhde.egg-info/SOURCES.txt` & `djangoldp_dhde-0.2.9/djangoldp_dhde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

