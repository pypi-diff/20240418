# Comparing `tmp/web3db-1.0.1.tar.gz` & `tmp/web3db-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3db-1.0.1.tar", max compression
+gzip compressed data, was "web3db-1.0.2.tar", max compression
```

## Comparing `web3db-1.0.1.tar` & `web3db-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,16 @@
--rw-r--r--   0        0        0      482 2024-04-15 23:26:20.124780 web3db-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       51 2024-02-26 15:25:35.563030 web3db-1.0.1/web3db/__init__.py
--rw-r--r--   0        0        0    20770 2024-03-29 13:46:18.804545 web3db-1.0.1/web3db/core.py
--rw-r--r--   0        0        0      194 2024-02-26 15:25:35.549029 web3db-1.0.1/web3db/models/__init__.py
--rw-r--r--   0        0        0      528 2024-02-26 15:27:22.333753 web3db-1.0.1/web3db/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      450 2024-01-19 19:58:55.290355 web3db-1.0.1/web3db/models/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1911 2024-01-26 16:14:20.438761 web3db-1.0.1/web3db/models/__pycache__/discord.cpython-311.pyc
--rw-r--r--   0        0        0     2079 2024-02-04 19:59:52.544417 web3db-1.0.1/web3db/models/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0     1771 2024-02-04 17:51:16.577297 web3db-1.0.1/web3db/models/__pycache__/github.cpython-311.pyc
--rw-r--r--   0        0        0     5715 2024-02-26 17:15:22.282534 web3db-1.0.1/web3db/models/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0     3253 2024-03-24 21:28:25.779082 web3db-1.0.1/web3db/models/__pycache__/profile.cpython-311.pyc
--rw-r--r--   0        0        0     1751 2024-02-27 20:23:48.644261 web3db-1.0.1/web3db/models/__pycache__/proxy.cpython-311.pyc
--rw-r--r--   0        0        0     2266 2024-02-18 00:57:41.213067 web3db-1.0.1/web3db/models/__pycache__/twitter.cpython-311.pyc
--rw-r--r--   0        0        0       88 2024-01-19 19:11:12.418624 web3db-1.0.1/web3db/models/base.py
--rw-r--r--   0        0        0      867 2024-01-21 14:45:55.501349 web3db-1.0.1/web3db/models/discord.py
--rw-r--r--   0        0        0      957 2024-02-04 19:29:31.959782 web3db-1.0.1/web3db/models/email.py
--rw-r--r--   0        0        0      779 2024-02-04 17:48:00.969984 web3db-1.0.1/web3db/models/github.py
--rw-r--r--   0        0        0     2690 2024-02-26 16:52:49.709378 web3db-1.0.1/web3db/models/mixins.py
--rw-r--r--   0        0        0     1974 2024-03-24 21:27:16.492192 web3db-1.0.1/web3db/models/profile.py
--rw-r--r--   0        0        0      763 2024-02-27 20:23:16.946158 web3db-1.0.1/web3db/models/proxy.py
--rw-r--r--   0        0        0     1078 2024-02-18 00:57:20.977221 web3db-1.0.1/web3db/models/twitter.py
--rw-r--r--   0        0        0      205 2024-01-20 14:29:59.965637 web3db-1.0.1/web3db/utils/__init__.py
--rw-r--r--   0        0        0      422 2024-01-20 15:56:54.552567 web3db-1.0.1/web3db/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2246 2024-03-29 13:15:23.225725 web3db-1.0.1/web3db/utils/__pycache__/encrypt_private.cpython-311.pyc
--rw-r--r--   0        0        0     1078 2024-02-10 22:53:40.648821 web3db-1.0.1/web3db/utils/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0      922 2024-03-29 13:15:22.001268 web3db-1.0.1/web3db/utils/encrypt_private.py
--rw-r--r--   0        0        0      713 2024-02-10 15:01:20.600084 web3db-1.0.1/web3db/utils/logger.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 web3db-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      660 2024-04-18 16:39:17.914393 web3db-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-02-26 15:25:35.563030 web3db-1.0.2/web3db/__init__.py
+-rw-r--r--   0        0        0    15788 2024-04-18 17:41:03.447775 web3db-1.0.2/web3db/core.py
+-rw-r--r--   0        0        0      194 2024-02-26 15:25:35.549029 web3db-1.0.2/web3db/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-01-19 19:11:12.418624 web3db-1.0.2/web3db/models/base.py
+-rw-r--r--   0        0        0      867 2024-01-21 14:45:55.501349 web3db-1.0.2/web3db/models/discord.py
+-rw-r--r--   0        0        0     1026 2024-04-18 16:33:29.904944 web3db-1.0.2/web3db/models/email.py
+-rw-r--r--   0        0        0      779 2024-02-04 17:48:00.969984 web3db-1.0.2/web3db/models/github.py
+-rw-r--r--   0        0        0     2690 2024-02-26 16:52:49.709378 web3db-1.0.2/web3db/models/mixins.py
+-rw-r--r--   0        0        0     1974 2024-03-24 21:27:16.492192 web3db-1.0.2/web3db/models/profile.py
+-rw-r--r--   0        0        0      763 2024-02-27 20:23:16.946158 web3db-1.0.2/web3db/models/proxy.py
+-rw-r--r--   0        0        0     1078 2024-02-18 00:57:20.977221 web3db-1.0.2/web3db/models/twitter.py
+-rw-r--r--   0        0        0      205 2024-01-20 14:29:59.965637 web3db-1.0.2/web3db/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-03-29 13:15:22.001268 web3db-1.0.2/web3db/utils/encrypt_private.py
+-rw-r--r--   0        0        0      713 2024-02-10 15:01:20.600084 web3db-1.0.2/web3db/utils/logger.py
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 web3db-1.0.2/PKG-INFO
```

### Comparing `web3db-1.0.1/web3db/core.py` & `web3db-1.0.2/web3db/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import base58
 from mnemonic import Mnemonic
 from eth_account import Account as EVMAccount
 from aptos_sdk.account import Account as AptosAccount
 from solana.rpc.api import Keypair
 from bitcoinutils.hdwallet import HDWallet
 from bitcoinutils.setup import setup
-from sqlalchemy import Result, func, Sequence, delete, and_, not_, desc, Select, Update, Delete, case
+from sqlalchemy import Result, func, delete, and_, not_, desc, Select, Update, Delete, case
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.asyncio import create_async_engine, async_sessionmaker
 from sqlalchemy.future import select
 from sqlalchemy.orm import joinedload
 
 from web3db.models import *
 from web3db.utils import logger
@@ -75,138 +75,14 @@
         if model == Proxy:
             query = select(model).where(model.proxy_string == login).options(joinedload('*'))
         else:
             query = select(model).where(model.login == login).options(joinedload('*'))
         result = await self._exec_stmt(query)
         return result.scalars().first()
 
-    @prepare_values
-    async def add_email(self, login: str, password: str) -> None:
-        logger.info(f'Adding Email {login}:{password}')
-        await self.add_record(Email(login=login, password=password))
-
-    @prepare_values
-    async def add_twitter(
-            self,
-            auth_token: str,
-            login: str = None,
-            password: str = None,
-            email: str = None,
-            email_password: str = None
-    ) -> None:
-        (
-            auth_token, login, password,
-            email, email_password
-        ) = prepare_strings(auth_token, login, password, email, email_password)
-        logger.info(f'Adding Twitter {auth_token}')
-        if email:
-            email.strip()
-            email = (await self.get_row_by_login(email, Email)
-                     or Email(login=email, password=email_password))
-        await self.add_record(
-            Twitter(
-                login=login.strip() if login else login,
-                password=password.strip() if password else password,
-                auth_token=auth_token,
-                email=email
-            )
-        )
-
-    @prepare_values
-    async def add_discord(
-            self,
-            auth_token: str,
-            login: str = None,
-            password: str = None,
-            email_password: str = None
-    ) -> None:
-        logger.info(f'Adding Discord {auth_token}')
-        email = ((await self.get_row_by_login(login, Email))
-                 or Email(login=login, password=email_password)) if login else None
-        await self.add_record(
-            Discord(
-                login=login,
-                password=password,
-                auth_token=auth_token,
-                email=email
-            )
-        )
-
-    @prepare_values
-    async def add_proxy(self, proxy_string: str) -> None:
-        logger.info(f'Adding Proxy {proxy_string}')
-        await self.add_record(Proxy(proxy_string=proxy_string))
-
-    @prepare_values
-    async def add_github(self, login: str, password: str, email_password: str = None):
-        logger.info(f'Adding Github {login}')
-        email = (await self.get_row_by_login(login=login, model=Email)) or Email(login=login, password=email_password)
-        await self.add_record(Github(login=login, password=password, email=email))
-
-    @prepare_values
-    async def add_profile(
-            self,
-            proxy_string: str,
-            email: str,
-            discord_login: str,
-            twitter_login: str,
-            evm_private: str,
-            aptos_private: str,
-            solana_private: str,
-            btc_mnemo: str,
-            recipient: str,
-            passphrase: str
-    ) -> None:
-        logger.info(f'Adding Profile {email}:{proxy_string}')
-        mail = await self.get_row_by_login(email, Email)
-        if not mail:
-            logger.error(f'Need email {email}')
-            return
-        discord = await self.get_row_by_login(discord_login, Discord)
-        if not discord:
-            logger.error(f'Need discord {discord_login}')
-            return
-        twitter = await self.get_row_by_login(twitter_login, Twitter)
-        if not twitter:
-            logger.error(f'Need twitter {twitter_login}')
-            return
-        proxy = await self.get_row_by_login(proxy_string, Proxy)
-        if not proxy:
-            logger.error(f'Need proxy {proxy_string}')
-            return
-        evm_account = EVMAccount.from_key(evm_private)
-        aptos_account = AptosAccount.load_key(aptos_private)
-        solana_keypair = Keypair.from_base58_string(solana_private)
-        btc_hdwallet = HDWallet(mnemonic=btc_mnemo)
-        btc_hdwallet.from_path("m/84'/0'/0'/0/0")
-        btc_native_segwit_address = btc_hdwallet.get_private_key().get_public_key().get_segwit_address().to_string()
-        btc_hdwallet.from_path("m/86'/0'/0'/0/0")
-        btc_taproot_address = btc_hdwallet.get_private_key().get_public_key().get_taproot_address().to_string()
-        btc_mnemo_encoded = encrypt(btc_mnemo, recipient, passphrase)
-        evm_private_encoded = encrypt(evm_private, recipient, passphrase)
-        aptos_private_encoded = encrypt(aptos_private, recipient, passphrase)
-        solana_private_encoded = encrypt(solana_private, recipient, passphrase)
-        await self.add_record(
-            Profile(
-                proxy=proxy,
-                email=email,
-                discord=discord,
-                twitter=twitter,
-                evm_address=evm_account.address,
-                aptos_address=str(aptos_account.address()),
-                solana_address=str(solana_keypair.pubkey()),
-                btc_native_segwit_address=btc_native_segwit_address,
-                btc_taproot_address=btc_taproot_address,
-                evm_private=evm_private_encoded,
-                aptos_private=aptos_private_encoded,
-                solana_private=solana_private_encoded,
-                btc_mnemo=btc_mnemo_encoded
-            )
-        )
-
     async def edit(self, edited_model: ModelType | list) -> ModelType | None:
         if isinstance(edited_model, list):
             logger.info(f'Editing rows {[el.id for el in edited_model]} in "{edited_model[0].__tablename__}" table')
         else:
             logger.info(f'Editing row with {edited_model.id} id in "{edited_model.__tablename__}" table')
         return await self.add_record(edited_model)
 
@@ -226,15 +102,15 @@
 
     async def get_row_by_id(self, id_: int, model: ModelType) -> ModelType:
         logger.info(f'Getting row with {id_} id from "{model.__tablename__}" table')
         query = select(model).where(model.id == id_).options(joinedload('*'))
         result = await self._exec_stmt(query)
         return result.scalars().first()
 
-    async def get_rows_by_id(self, ids: list[int], model: ModelType) -> Sequence[ModelType]:
+    async def get_rows_by_id(self, ids: list[int], model: ModelType) -> list[ModelType]:
         logger.info(f'Getting rows with {", ".join(map(str, ids))} ids from "{model.__tablename__}" table')
         query = select(model).filter(model.id.in_(ids)).order_by(model.id).options(joinedload('*'))
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
     async def get_profiles_light_by_model(
             self,
@@ -260,15 +136,15 @@
 
     async def get_random_profile(self) -> Profile:
         logger.info(f'Getting random profile')
         query = select(Profile).order_by(func.random()).options(joinedload('*'))
         result = await self._exec_stmt(query)
         return result.scalars().first()
 
-    async def get_random_profiles_by_proxy(self, limit: int = None) -> Sequence[Profile]:
+    async def get_random_profiles_by_proxy(self, limit: int = None) -> list[Profile]:
         logger.info(f'Getting random profiles by proxy')
         subquery = (
             select(
                 func.row_number().over(
                     partition_by=Profile.proxy_id,
                     order_by=func.random()
                 ).label('rn'),
@@ -282,15 +158,15 @@
             .where(subquery.c.rn == 1)
             .options(joinedload('*'))
             .limit(limit)
         )
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
-    async def get_random_profiles_ids_by_proxy(self, limit: int = None) -> Sequence[int]:
+    async def get_random_profiles_ids_by_proxy(self, limit: int = None) -> list[int]:
         logger.info(f'Getting random profiles by proxy (light with social)')
         subquery = (
             select(
                 func.row_number().over(
                     partition_by=Profile.proxy_id,
                     order_by=func.random()
                 ).label('rn'),
@@ -304,62 +180,62 @@
             .join(subquery, subquery.c.id == Profile.id)
             .where(subquery.c.rn == 1)
             .limit(limit)
         )
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
-    async def get_ready_profiles_by_model(self, model: ModelType, limit: int = None) -> Sequence[Profile]:
+    async def get_ready_profiles_by_model(self, model: ModelType, limit: int = None) -> list[Profile]:
         logger.info(f'Getting ready {model.__name__.lower()} profiles')
         query = (
             select(Profile).join(model).where(model.ready).options(joinedload('*')).limit(limit).order_by(Profile.id)
         )
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
-    async def get_ready_profiles_ids_by_model(self, model: ModelType, limit: int = None) -> Sequence[int]:
+    async def get_ready_profiles_ids_by_model(self, model: ModelType, limit: int = None) -> list[int]:
         logger.info(f'Getting ready {model.__name__.lower()} profiles (light with social)')
         query = select(Profile.id).join(model).where(model.ready).limit(limit)
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
-    async def get_profiles_with_totp_by_model(self, model: ModelType, limit: int = None) -> Sequence[Profile]:
+    async def get_profiles_with_totp_by_model(self, model: ModelType, limit: int = None) -> list[Profile]:
         logger.info(f'Getting {model.__name__.lower()} profiles with totp (light with social)')
         query = (
             select(Profile)
             .join(model)
             .where(model.totp_secret != None)
             .options(joinedload(getattr(Profile, model.__name__.lower())))
             .limit(limit)
             .order_by(Profile.id)
         )
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
     async def get_potential_profiles(self, limit: int = None) -> list[Profile]:
-        free_proxies: list[Proxy] = await self.get_free_proxies(limit=limit)
-        free_proxies_count = sum([el[-1] for el in free_proxies])
-        free_emails: list[Email] = await self.get_free_emails(limit=limit or free_proxies_count)
-        free_discords: list[Discord] = await self.get_free_model(Discord, limit=limit or free_proxies_count)
-        free_twitters: list[Twitter] = await self.get_free_model(Twitter, limit=limit or free_proxies_count)
-        free_proxies_all = []
-        for free_proxy, n in free_proxies:
-            free_proxies_all += [free_proxy] * n
-        random.shuffle(free_proxies_all)
+        unused_proxies: list[tuple[Proxy, int]] = await self.get_unused_proxies(limit=limit)
+        unused_proxies_count = sum([el[-1] for el in unused_proxies])
+        unused_emails: list[Email] = await self.get_unused_emails(limit=limit or unused_proxies_count)
+        unused_discords: list[Discord] = await self.get_unused_model(Discord, limit=limit or unused_proxies_count)
+        unused_twitters: list[Twitter] = await self.get_unused_model(Twitter, limit=limit or unused_proxies_count)
+        unused_proxies_all = []
+        for unused_proxy, n in unused_proxies:
+            unused_proxies_all += [unused_proxy] * n
+        random.shuffle(unused_proxies_all)
         potential_profiles = []
-        for i, free_proxy in enumerate(free_proxies_all):
+        for i, unused_proxy in enumerate(unused_proxies_all):
             potential_profiles.append(Profile(
-                email=free_emails[i] if i < len(free_emails) else None,
-                discord=free_discords[i] if i < len(free_discords) else None,
-                twitter=free_twitters[i] if i < len(free_twitters) else None,
-                proxy=free_proxy
+                email=unused_emails[i] if i < len(unused_emails) else None,
+                discord=unused_discords[i] if i < len(unused_discords) else None,
+                twitter=unused_twitters[i] if i < len(unused_twitters) else None,
+                proxy=unused_proxy
             ))
         return potential_profiles
 
-    async def create_profiles_from_free(
+    async def create_profiles(
             self,
             recipient: str,
             passphrase: str,
             limit: int = None
     ) -> list[Profile]:
         potential_profiles = await self.get_potential_profiles(limit)
         for i, profile in enumerate(potential_profiles):
@@ -385,50 +261,50 @@
             btc_hdwallet.from_path("m/86'/0'/0'/0/0")
             profile.btc_taproot_address = (
                 btc_hdwallet.get_private_key().get_public_key().get_taproot_address().to_string()
             )
         result = await self.add_record(potential_profiles)
         return result
 
-    async def get_free_emails(self, limit: int = None) -> Sequence[Email]:
-        logger.info(f'Getting free mails')
+    async def get_unused_emails(self, limit: int = None) -> list[Email]:
+        logger.info(f'Getting unused mails')
         subquery = (
             select(Twitter.email_id)
             .where(Twitter.email_id.isnot(None))
             .union(select(Profile.email_id).where(Profile.email_id.isnot(None)))
         )
         query = (
             select(Email)
             .where(and_(~Email.id.in_(subquery), not_(Email.login.ilike('%.ru'))))
             .order_by(Email.id)
             .limit(limit)
         )
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
-    async def get_free_model(
+    async def get_unused_model(
             self,
             model: type(Twitter) | type(Discord) | type(Github),
             limit: int = None
-    ) -> Sequence[Twitter | Discord | Github]:
-        logger.info(f'Getting free {model.__tablename__}')
+    ) -> list[Twitter | Discord | Github]:
+        logger.info(f'Getting unused {model.__tablename__}')
         query = (
             select(model)
             .where(~model.id.in_(
                 select(getattr(Profile, model.__name__.lower() + '_id'))
                 .where(getattr(Profile, model.__name__.lower() + '_id').isnot(None))))
             .order_by(model.id)
             .options(joinedload(model.email))
             .limit(limit)
         )
         result = await self._exec_stmt(query)
         return result.scalars().all()
 
-    async def get_free_proxies(self, limit: int = None) -> Sequence[Proxy]:
-        logger.info(f'Getting free proxies')
+    async def get_unused_proxies(self, limit: int = None) -> list[tuple[Proxy, int]]:
+        logger.info(f'Getting unused proxies')
         query = (
             select(Proxy, case(
                 (Proxy.proxy_type == 'individual', INDIVIDUAL_PROXY_LIMIT - func.count(Profile.proxy_id)),
                 (Proxy.proxy_type == 'shared', SHARED_PROXY_LIMIT - func.count(Profile.proxy_id))
             ).label('count_1')).outerjoin(Profile).group_by(Proxy).having(
                 (Proxy.proxy_type == 'individual' and func.count(Profile.proxy_id) < 3) or
                 (Proxy.proxy_type == 'shared' and func.count(Profile.proxy_id) < 2)
@@ -445,21 +321,22 @@
             delete_models_email: bool = False
     ) -> ModelType | None:
         if isinstance(profile_ids, int):
             profile_ids = [profile_ids]
         logger.info(f'Changing {model.__name__.lower()} for {profile_ids} profiles')
         profiles: list[Profile] = await self.get_rows_by_id(profile_ids, Profile)
         models_to_delete: list[model] = [getattr(profile, model.__name__.lower()) for profile in profiles]
+        unused_models_rows = []
         if model in (Twitter, Discord, Github):
-            free_models_rows = await self.get_free_model(model, limit=len(profile_ids))
+            unused_models_rows = await self.get_unused_model(model, limit=len(profile_ids))
         elif model == Proxy:
-            free_models_rows = await self.get_free_proxies(limit=len(profile_ids))
+            unused_models_rows = await self.get_unused_proxies(limit=len(profile_ids))
         elif model == Email:
-            free_models_rows = await self.get_free_emails(limit=len(profile_ids))
-        for profile, model in zip(profiles, free_models_rows):
+            unused_models_rows = await self.get_unused_emails(limit=len(profile_ids))
+        for profile, model in zip(profiles, unused_models_rows):
             logger.info(
                 f'{profile.id} | Old {type(model).__name__.lower()} {getattr(profile, type(model).__name__.lower())}')
             setattr(profile, type(model).__name__.lower(), model)
             logger.info(
                 f'{profile.id} | New {type(model).__name__.lower()} {getattr(profile, type(model).__name__.lower())}')
         edited_profile = await self.edit(profiles)
         if delete_model:
```

### Comparing `web3db-1.0.1/web3db/models/discord.py` & `web3db-1.0.2/web3db/models/discord.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/models/email.py` & `web3db-1.0.2/web3db/models/email.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class Email(Base):
     __tablename__ = 'emails'
 
     id: Mapped[int] = mapped_column(primary_key=True)
     login: Mapped[str] = mapped_column(String, unique=True)
     password: Mapped[str] = mapped_column(String)
+    totp_secret: Mapped[str] = mapped_column(String, nullable=True)
 
     discord: Mapped['Discord'] = relationship(back_populates='email')
     twitter: Mapped['Twitter'] = relationship(back_populates='email')
     profile: Mapped['Profile'] = relationship(back_populates='email')
     github: Mapped['Github'] = relationship(back_populates='email')
 
     def __repr__(self):
```

### Comparing `web3db-1.0.1/web3db/models/github.py` & `web3db-1.0.2/web3db/models/github.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/models/mixins.py` & `web3db-1.0.2/web3db/models/mixins.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/models/profile.py` & `web3db-1.0.2/web3db/models/profile.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/models/proxy.py` & `web3db-1.0.2/web3db/models/proxy.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/models/twitter.py` & `web3db-1.0.2/web3db/models/twitter.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/utils/encrypt_private.py` & `web3db-1.0.2/web3db/utils/encrypt_private.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/web3db/utils/logger.py` & `web3db-1.0.2/web3db/utils/logger.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.1/PKG-INFO` & `web3db-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: web3db
-Version: 1.0.1
+Version: 1.0.2
 Summary: Database for web3
+Home-page: https://github.com/timertimertimer/web3db
 Author: timertimertimer
 Author-email: timerkhan2002@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=2.0.29,<3.0.0)
 Requires-Dist: aptos-sdk (==0.7.1)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: bitcoin-utils (>=0.6.6,<0.7.0)
 Requires-Dist: eth-account (>=0.12.2,<0.13.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-gnupg (>=0.5.2,<0.6.0)
 Requires-Dist: solana (>=0.33.0,<0.34.0)
+Project-URL: Repository, https://github.com/timertimertimer/web3db
```

