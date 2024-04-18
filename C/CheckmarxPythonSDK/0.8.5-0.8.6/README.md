# Comparing `tmp/CheckmarxPythonSDK-0.8.5.tar.gz` & `tmp/checkmarxpythonsdk-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheckmarxPythonSDK-0.8.5.tar", last modified: Thu Feb  8 13:49:45 2024, max compression
+gzip compressed data, was "checkmarxpythonsdk-0.8.6.tar", last modified: Thu Apr 18 06:24:02 2024, max compression
```

## Comparing `CheckmarxPythonSDK-0.8.5.tar` & `checkmarxpythonsdk-0.8.6.tar`

### file list

```diff
@@ -1,458 +1,460 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.441479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.441479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/
--rw-r--r--   0 runner    (1001) docker     (127)    90214 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/AccessControl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.441479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.445479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/AuthenticationProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPGroupAndRoleMappingDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPRoleMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPServer.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPTeamMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/MyProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/OIDCClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Permission.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLIdentityProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLRoleMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLServiceProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLTeamMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SMTPSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/ServiceProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SystemLocale.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Team.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/User.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/WindowsDomain.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.445479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/HttpRequests.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/ProjectsODataAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/ResultsODataAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/ScansODataAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.449479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.449479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.449479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstIdWithName.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.453479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/AttackDetectionAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/AuthenticationManagementAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientAttributeCertificateAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientInitialAccessAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientRegistrationPolicyAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientRoleMappingsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientScopesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ComponentAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/GroupsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/IdentityProvidersAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/KeyAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ProtocolMappersAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/RealmsAdminAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/RoleMapperAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/RolesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/RolesByIDAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/RootAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ScopeMappingsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/UserStorageProviderAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/UsersAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.469479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessToken.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAuthorization.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenCertConf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AddressClaimSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionExportRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationFlowRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CertificateRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessCreatePresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessPresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientMappingsRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPoliciesRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyConditionRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyExecutorRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfileRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfilesRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeEvaluateResourceProtocolMapperEvaluationRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentExportRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ConfigPropertyRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CredentialRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/FederatedIdentityRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GlobalRequestResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GroupRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IDToken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderMapperRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/JsonNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeyStoreConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentationKeyMetadataRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ManagementPermissionReference.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MappingsRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MemoryInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MultivaluedHashMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PartialImportRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PasswordPolicyTypeRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PolicyRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProfileInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProtocolMapperRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProviderRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmEventsConfigRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    37948 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RequiredActionProviderRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceServerRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentationComposites.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RolesRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeMappingRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopePermissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ServerInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SpiInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SynchronizationResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SystemInfoRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/TestLdapConnectionRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/User.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserConsentRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationMapperRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationProviderRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/applicationsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.477479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ApiSecCounters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ApplicationInput.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ApplicationsCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/BflTree.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ComplianceSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/CreatedApplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/DefaultConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/DefaultConfigOut.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/FileInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Git.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/KicsCounters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/KicsResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/LanguageSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/MethodInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/MethodParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/PlatformSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ProjectInput.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ProjectsCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/QueriesResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/QueryDescription.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/QueryDescriptionSampleCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/QuerySummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ResultNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ResultsSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/RichProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/RuleInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SastCounters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SastResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScaContainersCounters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScaCounters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScaPackageCounters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScanConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScanInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScanParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScansCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SeveritySummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SinkFileSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SinkNodeSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SourceFileSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SourceNodeSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/StatusDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/StatusSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SubCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SubsetScan.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/TaskInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/WorkspaceQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/healthCheckServiceAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/httpRequests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/kicsResultsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/policyInformationPointAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/projectsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/repoStoreServiceAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/reportAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastBestFixLocationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastQueriesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastQueriesAuditAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastResultsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastResultsSummaryAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/scanConfigurationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/scannersResultsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/scansAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/uploadsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.481479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxAuditWebService.py
--rw-r--r--   0 runner    (1001) docker     (127)    41766 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxPortalWebService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/authHeaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/zeepClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.481479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.481479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/CreateReportDTO.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/CreateReportResponseDTO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/FilterDTO.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/ReportStatusDTO.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/httpRequests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.485479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/AccessControlAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/ConfigurationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CustomFieldsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CustomTasksAPI.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.485479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.485479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/CxXMLResults.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/PathNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Snippet.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/xml_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/DataRetentionAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/EnginesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/GeneralAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    19288 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/OsaAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    49869 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/ProjectsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/QueriesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    54861 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/ScansAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/TeamAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.485479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/httpRequests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.485479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLicense.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaMatchType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaScanDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaSeverity.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaState.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaSummaryReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityComment.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityState.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/CxSASTConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDataRetentionRequestStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDataRetentionRequestStatusStage.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionDateRangeRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionNumberOfScansRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.489479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.493479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineServer.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineServerStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxRegisterEngineRequestBody.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.493479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.493479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/CxServerLicenseData.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/CxSupportedLanguage.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.493479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.497479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCreateProjectRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCreateProjectResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCredential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCustomRemoteSourceSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxGitSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemField.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemFieldAllowedValue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemJira.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemJiraField.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemType.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxPerforceSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectExcludeSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectQueueSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSVNSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSharedRemoteSourceSettingsRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSharedRemoteSourceSettingsResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSourceSettingsLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxTFSSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxURI.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectNameTeamIdRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.497479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customFields/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customFields/CxCustomField.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customFields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.497479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/CxCustomTask.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.497479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/CxPreset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.497479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.505479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxCreateNewScanResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxDateAndTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxFinishedScanStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageState.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageStatistic.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxPolicyFindingResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxPolicyFindingsStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxRegisterScanReportResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxResultsStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanFailedGeneralQueries.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanFailedQueries.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanFileCountOfLanguage.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanParsedFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanParsedFilesMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanQueueDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportXmlContent.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVectorByBFL.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultLabelsFields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanStage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanState.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanSucceededGeneralQueries.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanType.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxSchedulingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatisticsResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatusDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.505479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsRequestBody.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxEmailNotification.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxLanguage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxScanSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.505479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/team/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.505479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/team/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/team/dto/CxTeam.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/team/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.505479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/AccessControlAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57427 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/httpRequests.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.505479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.509479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/CxCategory.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/CxSarifCategory.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifArtifactLocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifDescription.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifDriverRule.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifLocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifPhysicalLocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifPhysicalLocationPropertyBag.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifResultPropertyBag.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifResultsCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifRun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifScanResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaPropertyBag.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaRelationship.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaRelationshipTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTool.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifToolComponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/sast_xml_to_sarif.py
--rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/stig_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/CxError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/configUtility.py
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/httpRequests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-02-08 13:49:45.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24224 2024-02-08 13:49:45.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 13:49:45.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-08 13:49:45.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 13:49:45.000000 CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:49:45.513479 CheckmarxPythonSDK-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-08 13:49:32.000000 CheckmarxPythonSDK-0.8.5/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.648355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.652355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/
+-rw-r--r--   0 runner    (1001) docker     (127)    90214 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/AccessControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.652355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.656355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/AuthenticationProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPGroupAndRoleMappingDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPRoleMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPTeamMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/MyProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/OIDCClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLIdentityProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLRoleMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLServiceProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLTeamMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SMTPSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/ServiceProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SystemLocale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/WindowsDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.656355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/HttpRequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/ProjectsODataAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/ResultsODataAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/ScansODataAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.660355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.660355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.660355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstIdWithName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.664355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/AttackDetectionAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/AuthenticationManagementAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientAttributeCertificateAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientInitialAccessAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientRegistrationPolicyAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientRoleMappingsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientScopesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ComponentAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/GroupsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/IdentityProvidersAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/KeyAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ProtocolMappersAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/RealmsAdminAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/RoleMapperAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/RolesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/RolesByIDAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/RootAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ScopeMappingsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/UserStorageProviderAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/UsersAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.680355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessToken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAuthorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenCertConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AddressClaimSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionExportRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationFlowRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CertificateRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessCreatePresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessPresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientMappingsRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPoliciesRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyConditionRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyExecutorRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfileRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfilesRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeEvaluateResourceProtocolMapperEvaluationRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentExportRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ConfigPropertyRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CredentialRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/FederatedIdentityRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GlobalRequestResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GroupRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IDToken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderMapperRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/JsonNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeyStoreConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentationKeyMetadataRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ManagementPermissionReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MappingsRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MemoryInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MultivaluedHashMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PartialImportRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PasswordPolicyTypeRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PolicyRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProfileInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProtocolMapperRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProviderRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmEventsConfigRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37948 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RequiredActionProviderRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceServerRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentationComposites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RolesRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeMappingRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopePermissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ServerInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SpiInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SynchronizationResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SystemInfoRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/TestLdapConnectionRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserConsentRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationMapperRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationProviderRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/applicationsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.688355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ApiSecCounters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ApplicationInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ApplicationsCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/BflTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ComplianceSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/CreatedApplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/DefaultConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/DefaultConfigOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/FileInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/KicsCounters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/KicsResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/LanguageSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/MethodInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/MethodParameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/PlatformSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ProjectInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ProjectsCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/QueriesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/QueryDescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/QueryDescriptionSampleCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/QuerySummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ResultNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ResultsSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/RichProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/RuleInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SastCounters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SastResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScaContainersCounters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScaCounters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScaPackageCounters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScanConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScanInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScanParameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScansCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SeveritySummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SinkFileSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SinkNodeSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SourceFileSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SourceNodeSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/StatusDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/StatusSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SubCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SubsetScan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/TaskInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/WorkspaceQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/flagsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/healthCheckServiceAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/httpRequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/kicsResultsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/policyInformationPointAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/projectsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/repoStoreServiceAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/reportAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastBestFixLocationAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastQueriesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastQueriesAuditAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastResultsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastResultsSummaryAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/scanConfigurationAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/scannersResultsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/scansAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/uploadsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.692355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxAuditWebService.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41766 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxPortalWebService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/authHeaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/zeepClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.692355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.692355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/CreateReportDTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/CreateReportResponseDTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/FilterDTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/ReportStatusDTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/httpRequests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.696355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/AccessControlAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/ConfigurationAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CustomFieldsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CustomTasksAPI.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.696355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.696355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/CxXMLResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/PathNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Snippet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/xml_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/DataRetentionAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/EnginesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/GeneralAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19288 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/OsaAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49869 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/ProjectsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/QueriesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54861 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/ScansAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/TeamAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.696355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/httpRequests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.696355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLicense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaMatchType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaScanDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaSummaryReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityComment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityState.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/CxSASTConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDataRetentionRequestStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDataRetentionRequestStatusStage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionDateRangeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionNumberOfScansRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.700355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineServerStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxRegisterEngineRequestBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.704355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.704355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/CxServerLicenseData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/CxSupportedLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.704355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.708355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCreateProjectRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCreateProjectResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCredential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCustomRemoteSourceSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxGitSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemField.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemFieldAllowedValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemJira.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemJiraField.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxPerforceSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectExcludeSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectQueueSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSVNSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSharedRemoteSourceSettingsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSharedRemoteSourceSettingsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSourceSettingsLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxTFSSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxURI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectNameTeamIdRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.708355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customFields/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customFields/CxCustomField.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customFields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.708355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/CxCustomTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.708355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/CxPreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.708355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.716355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxCreateNewScanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxDateAndTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxFinishedScanStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageStatistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxPolicyFindingResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxPolicyFindingsStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxRegisterScanReportResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxResultsStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanFailedGeneralQueries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanFailedQueries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanFileCountOfLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanParsedFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanParsedFilesMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanQueueDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportXmlContent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVectorByBFL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultLabelsFields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanStage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanSucceededGeneralQueries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxSchedulingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatisticsResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatusDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.716355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsRequestBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxEmailNotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxScanSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.716355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/team/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.716355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/team/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/team/dto/CxTeam.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/team/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.716355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/AccessControlAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57436 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/httpRequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.716355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.720355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/CxCategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/CxSarifCategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifArtifactLocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifDescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifDriverRule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifLocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifPhysicalLocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifPhysicalLocationPropertyBag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifResultPropertyBag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifResultsCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifScanResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaPropertyBag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaRelationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaRelationshipTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifToolComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/sast_xml_to_sarif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/stig_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/CxError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/configUtility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/httpRequests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-18 06:24:02.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24298 2024-04-18 06:24:02.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:24:02.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 06:24:02.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 06:24:02.000000 checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:24:02.724355 checkmarxpythonsdk-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 06:23:53.000000 checkmarxpythonsdk-0.8.6/tests/test_sample.py
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/AccessControl.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/AccessControl.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/AuthenticationProvider.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/AuthenticationProvider.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Configuration.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Configuration.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPGroupAndRoleMappingDetail.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPGroupAndRoleMappingDetail.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPRoleMapping.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPRoleMapping.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPServer.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPServer.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPTeamMapping.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/LDAPTeamMapping.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/MyProfile.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/MyProfile.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/OIDCClient.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/OIDCClient.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Permission.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Permission.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Role.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Role.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLIdentityProvider.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLIdentityProvider.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLRoleMapping.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLRoleMapping.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLServiceProvider.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLServiceProvider.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLTeamMapping.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SAMLTeamMapping.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SMTPSetting.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SMTPSetting.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SystemLocale.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/SystemLocale.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Team.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/Team.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/User.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/User.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/WindowsDomain.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/WindowsDomain.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxAccessControl/accesscontrol/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/HttpRequests.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/HttpRequests.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/ProjectsODataAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/ProjectsODataAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/ResultsODataAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/ResultsODataAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/ScansODataAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/ScansODataAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/Utilities.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/Utilities.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxODataApiSDK/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxODataApiSDK/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/api.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/api.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstIdWithName.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstIdWithName.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstUser.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/AccessControlAPI/dto/AstUser.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientRoleMappingsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientRoleMappingsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/ClientsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/GroupsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/GroupsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/RoleMapperAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/RoleMapperAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/UsersAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/UsersAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessToken.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessToken.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAccess.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAccess.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAuthorization.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AccessTokenAuthorization.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AddressClaimSet.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AddressClaimSet.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionExportRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionExportRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationExecutionRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationFlowRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticationFlowRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/AuthenticatorConfigRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CertificateRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CertificateRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessCreatePresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessCreatePresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessPresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientInitialAccessPresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientMappingsRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientMappingsRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyConditionRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyConditionRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyExecutorRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyExecutorRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientPolicyRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfileRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfileRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfilesRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientProfilesRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeEvaluateResourceProtocolMapperEvaluationRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeEvaluateResourceProtocolMapperEvaluationRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ClientScopeRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentExportRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentExportRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ComponentRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ConfigPropertyRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ConfigPropertyRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CredentialRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/CredentialRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/FederatedIdentityRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/FederatedIdentityRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GlobalRequestResult.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GlobalRequestResult.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Group.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Group.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GroupRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/GroupRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IDToken.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IDToken.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderMapperRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderMapperRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/IdentityProviderRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/JsonNode.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/JsonNode.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeyStoreConfig.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeyStoreConfig.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentationKeyMetadataRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/KeysMetadataRepresentationKeyMetadataRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ManagementPermissionReference.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ManagementPermissionReference.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MappingsRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MappingsRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MemoryInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MemoryInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MultivaluedHashMap.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/MultivaluedHashMap.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PartialImportRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PartialImportRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PasswordPolicyTypeRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PasswordPolicyTypeRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Permission.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/Permission.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PolicyRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/PolicyRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProfileInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProfileInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProtocolMapperRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProtocolMapperRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProviderRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ProviderRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmEventsConfigRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmEventsConfigRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RealmRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RequiredActionProviderRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RequiredActionProviderRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceServerRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ResourceServerRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentationComposites.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RoleRepresentationComposites.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RolesRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/RolesRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeMappingRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeMappingRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopePermissions.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopePermissions.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ScopeRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ServerInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/ServerInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SpiInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SpiInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SynchronizationResult.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SynchronizationResult.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SystemInfoRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/SystemInfoRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/TestLdapConnectionRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/TestLdapConnectionRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/User.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/User.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserConsentRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserConsentRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationMapperRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationMapperRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationProviderRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserFederationProviderRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserRepresentation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/UserRepresentation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/KeycloakAPI/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     create_an_application_rule,
     get_a_list_of_rules_for_a_specific_application,
     get_an_application_rule,
     update_an_application_rule,
     delete_an_application_rule,
 )
 
+from .flagsAPI import (
+    get_all_feature_flags,
+    get_feature_flag,
+)
+
 from .healthCheckServiceAPI import (
     get_health_of_the_database,
     get_health_of_the_in_memory_db,
     get_health_of_the_message_queue,
     get_health_of_the_object_stroe_including_all_buckets,
     get_health_of_the_logging,
     get_health_of_the_scan_flow,
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/applicationsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/applicationsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/config.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/config.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ApiSecCounters.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ApiSecCounters.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Application.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Application.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ApplicationInput.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ApplicationInput.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ApplicationsCollection.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ApplicationsCollection.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/BflTree.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/BflTree.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/CreatedApplication.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/CreatedApplication.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Credentials.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Credentials.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/DefaultConfig.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/DefaultConfig.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/DefaultConfigOut.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/DefaultConfigOut.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Error.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Error.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/FileInfo.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/FileInfo.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Git.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Git.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/KicsCounters.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/KicsCounters.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/KicsResult.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/KicsResult.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/MethodInfo.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/MethodInfo.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Project.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Project.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ProjectInput.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ProjectInput.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ProjectsCollection.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ProjectsCollection.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Queries.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Queries.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Query.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Query.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/QueryDescription.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/QueryDescription.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/QuerySummary.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/QuerySummary.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Result.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Result.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ResultNode.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ResultNode.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ResultsSummary.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ResultsSummary.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/RichProject.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/RichProject.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Rule.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Rule.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/RuleInput.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/RuleInput.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SastCounters.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SastCounters.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SastResult.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SastResult.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScaContainersCounters.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScaContainersCounters.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScaCounters.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScaCounters.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScaPackageCounters.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScaPackageCounters.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Scan.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Scan.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScanConfig.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScanConfig.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScanInput.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScanInput.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScanParameter.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScanParameter.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/ScansCollection.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/ScansCollection.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/StatusDetails.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/StatusDetails.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/SubsetScan.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/SubsetScan.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/TaskInfo.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/TaskInfo.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Tree.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Tree.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/Upload.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/Upload.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/WorkspaceQuery.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/WorkspaceQuery.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/dto/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/dto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .BflTree import BflTree
 from .CreatedApplication import CreatedApplication
 from .Credentials import Credentials
 from .DefaultConfig import DefaultConfig
 from .DefaultConfigOut import DefaultConfigOut
 from .Error import Error
 from .FileInfo import FileInfo
+from .Flag import Flag
 from .Git import Git
 from .Group import Group
 from .KicsResult import KicsResult
 from .MethodInfo import MethodInfo
 from .MethodParameter import MethodParameter
 from .Preset import Preset
 from .Project import Project
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/healthCheckServiceAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/healthCheckServiceAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/httpRequests.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/httpRequests.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/kicsResultsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/kicsResultsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/policyInformationPointAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/policyInformationPointAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/projectsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/projectsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/repoStoreServiceAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/repoStoreServiceAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/reportAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/reportAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastBestFixLocationAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastBestFixLocationAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastQueriesAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastQueriesAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastQueriesAuditAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastQueriesAuditAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastResultsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastResultsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/sastResultsSummaryAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/sastResultsSummaryAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/scanConfigurationAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/scanConfigurationAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/scannersResultsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/scannersResultsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/scansAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/scansAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/uploadsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/uploadsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxOne/utilities.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxOne/utilities.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxAuditWebService.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxAuditWebService.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxPortalWebService.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/CxPortalWebService.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/authHeaders.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/authHeaders.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxPortalSoapApiSDK/zeepClient.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxPortalSoapApiSDK/zeepClient.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/api.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from .httpRequests import (get_request, post_request)
 from CheckmarxPythonSDK.utilities.compat import (OK, CREATED)
 
 from .dto import (
     CreateReportDTO,
 )
 
+headers = {"Content-Type": "application/json; v=1.0"}
+
 
 def retrieve_the_file_of_a_specific_report(report_id):
     """
 
     Args:
         report_id (int):
 
     Returns:
         file content (binary string)
     """
     report_content = None
     relative_url = "/api/reports/{id}".format(id=report_id)
-    response = get_request(relative_url=relative_url)
+    response = get_request(relative_url=relative_url, headers=headers)
     if response.status_code == OK:
         report_content = response.content
     return report_content
 
 
 def create_a_new_report_request(report_request):
     """
@@ -36,15 +38,15 @@
     report_id = None
 
     if not isinstance(report_request, CreateReportDTO):
         return report_id
 
     relative_url = "/api/reports"
     data = report_request.get_post_data()
-    response = post_request(relative_url=relative_url, data=data)
+    response = post_request(relative_url=relative_url, data=data, headers=headers)
     if response.status_code == CREATED:
         item = response.json()
         report_id = item.get("reportId")
     return report_id
 
 
 def retrieve_the_status_of_a_specific_report(report_id):
@@ -57,15 +59,15 @@
         report_status (str)
             NEW
             PROCESSING
             FINISHED
     """
     report_status = None
     relative_url = "/api/reports/{id}/status".format(id=report_id)
-    response = get_request(relative_url=relative_url)
+    response = get_request(relative_url=relative_url, headers=headers)
     if response.status_code == OK:
         item = response.json()
         report_status = item.get("reportStatus")
     return report_status
 
 
 def get_report(report_request):
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/config.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/config.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/CreateReportDTO.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/CreateReportDTO.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/FilterDTO.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/FilterDTO.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/dto/ReportStatusDTO.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/dto/ReportStatusDTO.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxReporting/httpRequests.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxReporting/httpRequests.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/AccessControlAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/AccessControlAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/ConfigurationAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/ConfigurationAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CustomFieldsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CustomFieldsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CustomTasksAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CustomTasksAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/CxXMLResults.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/CxXMLResults.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Path.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Path.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/PathNode.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/PathNode.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Query.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Query.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Result.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/dto/Result.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/xml_results.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/CxSastXML/xml_results.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/DataRetentionAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/DataRetentionAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/EnginesAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/EnginesAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/GeneralAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/GeneralAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/OsaAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/OsaAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/ProjectsAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/ProjectsAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/QueriesAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/QueriesAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/ScansAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/ScansAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/TeamAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/TeamAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/config.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/config.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/httpRequests.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/httpRequests.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLibrary.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLibrary.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLicense.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaLicense.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaMatchType.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaMatchType.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaScanDetail.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaScanDetail.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaSummaryReport.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaSummaryReport.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerability.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerability.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityComment.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityComment.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityState.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/osa/dto/CxOsaVulnerabilityState.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/CxSASTConfig.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/configuration/dto/CxSASTConfig.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDataRetentionRequestStatus.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDataRetentionRequestStatus.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionDateRangeRequest.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionDateRangeRequest.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionNumberOfScansRequest.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/dataRetention/dto/CxDefineDataRetentionNumberOfScansRequest.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineConfiguration.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineConfiguration.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineServer.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxEngineServer.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxRegisterEngineRequestBody.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/engines/dto/CxRegisterEngineRequestBody.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/CxServerLicenseData.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/general/dto/CxServerLicenseData.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCreateProjectRequest.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCreateProjectRequest.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCustomRemoteSourceSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxCustomRemoteSourceSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxGitSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxGitSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystem.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystem.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemDetail.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemDetail.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemField.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemField.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemJira.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemJira.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemType.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxIssueTrackingSystemType.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxPerforceSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxPerforceSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProject.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProject.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectExcludeSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectExcludeSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectQueueSetting.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxProjectQueueSetting.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSVNSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSVNSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSharedRemoteSourceSettingsRequest.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSharedRemoteSourceSettingsRequest.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSourceSettingsLink.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxSourceSettingsLink.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxTFSSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxTFSSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectNameTeamIdRequest.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectNameTeamIdRequest.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectRequest.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/CxUpdateProjectRequest.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/CxCustomTask.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/customTasks/CxCustomTask.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/CxPreset.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/projects/dto/presets/CxPreset.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxDateAndTime.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxDateAndTime.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageState.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageState.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageStatistic.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxLanguageStatistic.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxPolicyFindingsStatus.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxPolicyFindingsStatus.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxRegisterScanReportResponse.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxRegisterScanReportResponse.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanDetail.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanDetail.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanParsedFilesMetric.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanParsedFilesMetric.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanQueueDetail.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanQueueDetail.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportStatus.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportStatus.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportXmlContent.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanReportXmlContent.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVector.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVector.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVectorByBFL.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultAttackVectorByBFL.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultNode.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanResultNode.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanState.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanState.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanStatistics.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanStatistics.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanSucceededGeneralQueries.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxScanSucceededGeneralQueries.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxSchedulingSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxSchedulingSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatisticsResult.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/CxStatisticsResult.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsRequestBody.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsRequestBody.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsResponse.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxCreateScanSettingsResponse.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxEmailNotification.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxEmailNotification.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxScanSettings.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/sast/scans/dto/scanSettings/CxScanSettings.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxRestAPISDK/team/dto/CxTeam.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxRestAPISDK/team/dto/CxTeam.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/AccessControlAPI.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/AccessControlAPI.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/api.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1138,15 +1138,15 @@
         package_type (str): e.g.  Python
         package_name:
         version:
 
     Returns:
 
     """
-    url = "/public/packages/{}/{}/{}".format(package_type, package_name, version)
+    url = "/public/packages/{}/{}/versions/{}".format(package_type, package_name, version)
     response = get_request(relative_url=url)
     return response.json()
 
 
 def get_suggest_private_package(package_type, package_name, version):
     """
         This is a public API
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/CxScaApiSDK/httpRequests.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/CxScaApiSDK/httpRequests.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/CxCategory.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/CxCategory.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifDriver.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifDriver.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifDriverRule.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifDriverRule.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifPhysicalLocation.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifPhysicalLocation.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifRegion.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifRegion.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifResultPropertyBag.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifResultPropertyBag.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifResultsCollection.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifResultsCollection.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifRun.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifRun.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifScanResult.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifScanResult.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxa.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxa.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaPropertyBag.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaPropertyBag.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaRelationshipTarget.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxaRelationshipTarget.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/SarifTaxonomy.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/SarifTaxonomy.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/dto/__init__.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/sast_xml_to_sarif.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/sast_xml_to_sarif.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/external/sarif/stig_mapping.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/external/sarif/stig_mapping.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/CxError.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/CxError.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/compat.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/compat.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/configUtility.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/configUtility.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK/utilities/httpRequests.py` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK/utilities/httpRequests.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,16 @@
         verify_ssl_cert=verify_ssl_cert,
         cert=cert
     )
     auth_header.update({"Authorization": new_token})
 
 
 auth_header = {
-    "Authorization": None
+    "Authorization": None,
+    "Content-Type": "application/json"
 }
 
 
 def retry_when_unauthorized(function_to_send_request, data, get_data_from_config, relative_url, files=None, auth=None,
                             headers=(), is_iam=False):
     server_url, token_url, timeout, verify, cert, token_req_data = get_data_from_config()
     url = server_url + relative_url
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/PKG-INFO` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheckmarxPythonSDK
-Version: 0.8.5
+Version: 0.8.6
 Summary: Checkmarx Python SDK
 Home-page: https://github.com/checkmarx-ts/checkmarx-python-sdk
 Author: Happy Yang
 Author-email: happy.yang@checkmarx.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `CheckmarxPythonSDK-0.8.5/CheckmarxPythonSDK.egg-info/SOURCES.txt` & `checkmarxpythonsdk-0.8.6/CheckmarxPythonSDK.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 CheckmarxPythonSDK/CxODataApiSDK/ResultsODataAPI.py
 CheckmarxPythonSDK/CxODataApiSDK/ScansODataAPI.py
 CheckmarxPythonSDK/CxODataApiSDK/Utilities.py
 CheckmarxPythonSDK/CxODataApiSDK/__init__.py
 CheckmarxPythonSDK/CxOne/__init__.py
 CheckmarxPythonSDK/CxOne/applicationsAPI.py
 CheckmarxPythonSDK/CxOne/config.py
+CheckmarxPythonSDK/CxOne/flagsAPI.py
 CheckmarxPythonSDK/CxOne/healthCheckServiceAPI.py
 CheckmarxPythonSDK/CxOne/httpRequests.py
 CheckmarxPythonSDK/CxOne/kicsResultsAPI.py
 CheckmarxPythonSDK/CxOne/policyInformationPointAPI.py
 CheckmarxPythonSDK/CxOne/projectsAPI.py
 CheckmarxPythonSDK/CxOne/repoStoreServiceAPI.py
 CheckmarxPythonSDK/CxOne/reportAPI.py
@@ -168,14 +169,15 @@
 CheckmarxPythonSDK/CxOne/dto/ComplianceSummary.py
 CheckmarxPythonSDK/CxOne/dto/CreatedApplication.py
 CheckmarxPythonSDK/CxOne/dto/Credentials.py
 CheckmarxPythonSDK/CxOne/dto/DefaultConfig.py
 CheckmarxPythonSDK/CxOne/dto/DefaultConfigOut.py
 CheckmarxPythonSDK/CxOne/dto/Error.py
 CheckmarxPythonSDK/CxOne/dto/FileInfo.py
+CheckmarxPythonSDK/CxOne/dto/Flag.py
 CheckmarxPythonSDK/CxOne/dto/Git.py
 CheckmarxPythonSDK/CxOne/dto/Group.py
 CheckmarxPythonSDK/CxOne/dto/KicsCounters.py
 CheckmarxPythonSDK/CxOne/dto/KicsResult.py
 CheckmarxPythonSDK/CxOne/dto/LanguageSummary.py
 CheckmarxPythonSDK/CxOne/dto/MethodInfo.py
 CheckmarxPythonSDK/CxOne/dto/MethodParameter.py
```

### Comparing `CheckmarxPythonSDK-0.8.5/LICENSE` & `checkmarxpythonsdk-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/PKG-INFO` & `checkmarxpythonsdk-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheckmarxPythonSDK
-Version: 0.8.5
+Version: 0.8.6
 Summary: Checkmarx Python SDK
 Home-page: https://github.com/checkmarx-ts/checkmarx-python-sdk
 Author: Happy Yang
 Author-email: happy.yang@checkmarx.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `CheckmarxPythonSDK-0.8.5/README.md` & `checkmarxpythonsdk-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/setup.py` & `checkmarxpythonsdk-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `CheckmarxPythonSDK-0.8.5/tests/test_sample.py` & `checkmarxpythonsdk-0.8.6/tests/test_sample.py`

 * *Files identical despite different names*

