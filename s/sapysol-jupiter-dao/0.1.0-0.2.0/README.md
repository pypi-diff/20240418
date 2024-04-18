# Comparing `tmp/sapysol_jupiter_dao-0.1.0.tar.gz` & `tmp/sapysol_jupiter_dao-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapysol_jupiter_dao-0.1.0.tar", max compression
+gzip compressed data, was "sapysol_jupiter_dao-0.2.0.tar", max compression
```

## Comparing `sapysol_jupiter_dao-0.1.0.tar` & `sapysol_jupiter_dao-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rwxr-xr-x   0        0        0     1071 2024-02-15 19:48:04.439476 sapysol_jupiter_dao-0.1.0/LICENSE
--rw-r--r--   0        0        0     3314 2024-04-12 10:26:20.012787 sapysol_jupiter_dao-0.1.0/README.md
--rw-r--r--   0        0        0      398 2024-04-17 18:25:37.451456 sapysol_jupiter_dao-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 17:58:24.618130 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/__init__.py
--rw-r--r--   0        0        0      279 2024-04-11 17:57:10.428691 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/__init__.py
--rw-r--r--   0        0        0      305 2024-03-30 16:46:23.873969 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/__init__.py
--rw-r--r--   0        0        0     5573 2024-03-31 16:50:03.008542 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/governor.py
--rw-r--r--   0        0        0     3851 2024-04-12 10:12:13.359136 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/option_proposal_meta.py
--rw-r--r--   0        0        0     9385 2024-04-12 10:11:34.429427 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal.py
--rw-r--r--   0        0        0     3886 2024-04-12 10:11:55.632602 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal_meta.py
--rw-r--r--   0        0        0     4654 2024-04-12 10:12:56.178816 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/vote.py
--rw-r--r--   0        0        0     1396 2024-04-12 10:13:13.068690 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/errors/__init__.py
--rw-r--r--   0        0        0    16708 2024-03-31 16:53:10.171288 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/errors/anchor.py
--rw-r--r--   0        0        0     3682 2024-03-31 16:53:27.204560 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/errors/custom.py
--rw-r--r--   0        0        0     1402 2024-04-12 10:14:06.734955 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/__init__.py
--rw-r--r--   0        0        0     1414 2024-04-12 09:48:08.196584 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/activate_proposal.py
--rw-r--r--   0        0        0     1680 2024-04-11 17:57:52.701705 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/cancel_proposal.py
--rw-r--r--   0        0        0     2243 2024-04-11 17:57:54.338359 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/claim_reward.py
--rw-r--r--   0        0        0     2409 2024-04-11 17:57:55.801681 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_governor.py
--rw-r--r--   0        0        0     2799 2024-04-11 17:57:57.954999 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_option_proposal_meta.py
--rw-r--r--   0        0        0     3028 2024-04-11 17:58:01.441639 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal.py
--rw-r--r--   0        0        0     2635 2024-04-05 19:24:46.842866 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal_meta.py
--rw-r--r--   0        0        0     2026 2024-04-11 17:58:03.021627 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/new_vote.py
--rw-r--r--   0        0        0     2284 2024-04-11 17:58:04.731614 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/queue_proposal.py
--rw-r--r--   0        0        0     1918 2024-04-11 17:58:06.468267 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_governance_params.py
--rw-r--r--   0        0        0     1771 2024-04-11 17:58:08.291587 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_locker.py
--rw-r--r--   0        0        0     1980 2024-04-11 17:58:10.168239 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_vote.py
--rw-r--r--   0        0        0     1904 2024-04-11 17:58:11.851560 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_voting_reward.py
--rw-r--r--   0        0        0      441 2024-03-31 17:23:47.111969 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/program_id.py
--rw-r--r--   0        0        0      947 2024-03-31 17:11:39.285977 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/__init__.py
--rw-r--r--   0        0        0     2611 2024-04-12 10:14:31.028107 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/governance_parameters.py
--rw-r--r--   0        0        0     2155 2024-04-12 10:14:33.224757 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_account_meta.py
--rw-r--r--   0        0        0     2676 2024-04-12 10:14:34.874745 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_instruction.py
--rw-r--r--   0        0        0     4885 2024-04-12 10:14:36.341400 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_state.py
--rw-r--r--   0        0        0     2459 2024-04-12 10:14:37.824723 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_type.py
--rw-r--r--   0        0        0     2384 2024-04-12 10:14:39.794708 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/voting_reward.py
--rw-r--r--   0        0        0        0 2024-03-30 16:34:21.429642 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/__init__.py
--rw-r--r--   0        0        0      249 2024-03-31 17:42:29.789004 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/accounts/__init__.py
--rw-r--r--   0        0        0     5780 2024-04-12 10:16:03.400748 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/accounts/escrow.py
--rw-r--r--   0        0        0     5238 2024-04-12 10:16:39.273813 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/accounts/locker.py
--rw-r--r--   0        0        0     1411 2024-04-12 10:17:49.526620 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/errors/__init__.py
--rw-r--r--   0        0        0    16723 2024-03-31 17:43:46.571906 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/errors/anchor.py
--rw-r--r--   0        0        0     3483 2024-04-12 10:17:11.953568 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/errors/custom.py
--rw-r--r--   0        0        0     1057 2024-03-31 17:45:32.460471 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/__init__.py
--rw-r--r--   0        0        0     1698 2024-04-11 17:57:29.098550 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/activate_proposal.py
--rw-r--r--   0        0        0     2292 2024-04-11 17:57:30.848537 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/cast_vote.py
--rw-r--r--   0        0        0     1908 2024-04-11 17:57:32.658523 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/extend_lock_duration.py
--rw-r--r--   0        0        0     2289 2024-04-11 17:57:34.331844 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/increase_locked_amount.py
--rw-r--r--   0        0        0     1699 2024-04-05 19:26:45.342054 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_escrow.py
--rw-r--r--   0        0        0     2303 2024-04-11 17:57:36.485161 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_locker.py
--rw-r--r--   0        0        0     1981 2024-04-11 17:57:39.285140 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_locker_params.py
--rw-r--r--   0        0        0     1858 2024-04-11 17:57:40.888461 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_vote_delegate.py
--rw-r--r--   0        0        0     1882 2024-04-11 17:57:42.665114 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/toggle_max_lock.py
--rw-r--r--   0        0        0     1966 2024-04-11 17:57:44.425101 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/withdraw.py
--rw-r--r--   0        0        0      370 2024-03-31 17:49:04.737101 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/program_id.py
--rw-r--r--   0        0        0      286 2024-03-31 20:17:33.131741 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/types/__init__.py
--rw-r--r--   0        0        0     2921 2024-04-12 10:17:40.286689 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/types/locker_params.py
--rw-r--r--   0        0        0     5359 2024-04-17 18:14:22.360494 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/batcher.py
--rw-r--r--   0        0        0     3505 2024-04-11 17:55:50.679294 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/derive.py
--rw-r--r--   0        0        0     5215 2024-04-12 10:06:06.031872 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/governor.py
--rw-r--r--   0        0        0    35952 2024-03-07 23:20:55.315692 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/idls/governor_idl.json
--rw-r--r--   0        0        0    22431 2024-03-30 16:31:34.471154 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/idls/locked_voter_idl.json
--rw-r--r--   0        0        0    29684 2024-03-30 16:32:50.590465 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/idls/smart_wallet_idl.json
--rw-r--r--   0        0        0        0 2024-03-31 17:28:08.180510 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/smart_wallet.py
--rw-r--r--   0        0        0     2778 2024-04-12 09:57:04.279183 sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/voter.py
--rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 sapysol_jupiter_dao-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-02-15 19:48:04.439476 sapysol_jupiter_dao-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3444 2024-04-18 21:20:42.720368 sapysol_jupiter_dao-0.2.0/README.md
+-rw-r--r--   0        0        0      398 2024-04-17 19:09:28.669847 sapysol_jupiter_dao-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 17:58:24.618130 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-11 17:57:10.428691 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/__init__.py
+-rw-r--r--   0        0        0      305 2024-03-30 16:46:23.873969 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/__init__.py
+-rw-r--r--   0        0        0     5573 2024-03-31 16:50:03.008542 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/governor.py
+-rw-r--r--   0        0        0     3851 2024-04-12 10:12:13.359136 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/option_proposal_meta.py
+-rw-r--r--   0        0        0     9385 2024-04-12 10:11:34.429427 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal.py
+-rw-r--r--   0        0        0     3886 2024-04-12 10:11:55.632602 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal_meta.py
+-rw-r--r--   0        0        0     4654 2024-04-12 10:12:56.178816 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/vote.py
+-rw-r--r--   0        0        0     1396 2024-04-12 10:13:13.068690 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/errors/__init__.py
+-rw-r--r--   0        0        0    16708 2024-03-31 16:53:10.171288 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/errors/anchor.py
+-rw-r--r--   0        0        0     3682 2024-03-31 16:53:27.204560 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/errors/custom.py
+-rw-r--r--   0        0        0     1402 2024-04-12 10:14:06.734955 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/__init__.py
+-rw-r--r--   0        0        0     1414 2024-04-12 09:48:08.196584 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/activate_proposal.py
+-rw-r--r--   0        0        0     1680 2024-04-11 17:57:52.701705 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/cancel_proposal.py
+-rw-r--r--   0        0        0     2243 2024-04-11 17:57:54.338359 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/claim_reward.py
+-rw-r--r--   0        0        0     2409 2024-04-11 17:57:55.801681 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_governor.py
+-rw-r--r--   0        0        0     2799 2024-04-11 17:57:57.954999 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_option_proposal_meta.py
+-rw-r--r--   0        0        0     3028 2024-04-11 17:58:01.441639 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal.py
+-rw-r--r--   0        0        0     2635 2024-04-05 19:24:46.842866 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal_meta.py
+-rw-r--r--   0        0        0     2026 2024-04-11 17:58:03.021627 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/new_vote.py
+-rw-r--r--   0        0        0     2284 2024-04-11 17:58:04.731614 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/queue_proposal.py
+-rw-r--r--   0        0        0     1918 2024-04-11 17:58:06.468267 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_governance_params.py
+-rw-r--r--   0        0        0     1771 2024-04-11 17:58:08.291587 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_locker.py
+-rw-r--r--   0        0        0     1980 2024-04-11 17:58:10.168239 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_vote.py
+-rw-r--r--   0        0        0     1904 2024-04-11 17:58:11.851560 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_voting_reward.py
+-rw-r--r--   0        0        0      441 2024-03-31 17:23:47.111969 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/program_id.py
+-rw-r--r--   0        0        0      947 2024-03-31 17:11:39.285977 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/__init__.py
+-rw-r--r--   0        0        0     2611 2024-04-12 10:14:31.028107 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/governance_parameters.py
+-rw-r--r--   0        0        0     2155 2024-04-12 10:14:33.224757 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_account_meta.py
+-rw-r--r--   0        0        0     2676 2024-04-12 10:14:34.874745 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_instruction.py
+-rw-r--r--   0        0        0     4885 2024-04-12 10:14:36.341400 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_state.py
+-rw-r--r--   0        0        0     2459 2024-04-12 10:14:37.824723 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_type.py
+-rw-r--r--   0        0        0     2384 2024-04-12 10:14:39.794708 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/voting_reward.py
+-rw-r--r--   0        0        0        0 2024-03-30 16:34:21.429642 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/__init__.py
+-rw-r--r--   0        0        0      249 2024-03-31 17:42:29.789004 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/accounts/__init__.py
+-rw-r--r--   0        0        0     5780 2024-04-12 10:16:03.400748 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/accounts/escrow.py
+-rw-r--r--   0        0        0     5238 2024-04-12 10:16:39.273813 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/accounts/locker.py
+-rw-r--r--   0        0        0     1411 2024-04-12 10:17:49.526620 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/errors/__init__.py
+-rw-r--r--   0        0        0    16723 2024-03-31 17:43:46.571906 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/errors/anchor.py
+-rw-r--r--   0        0        0     3483 2024-04-12 10:17:11.953568 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/errors/custom.py
+-rw-r--r--   0        0        0     1057 2024-03-31 17:45:32.460471 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/__init__.py
+-rw-r--r--   0        0        0     1698 2024-04-11 17:57:29.098550 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/activate_proposal.py
+-rw-r--r--   0        0        0     2292 2024-04-11 17:57:30.848537 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/cast_vote.py
+-rw-r--r--   0        0        0     1908 2024-04-11 17:57:32.658523 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/extend_lock_duration.py
+-rw-r--r--   0        0        0     2289 2024-04-11 17:57:34.331844 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/increase_locked_amount.py
+-rw-r--r--   0        0        0     1699 2024-04-05 19:26:45.342054 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_escrow.py
+-rw-r--r--   0        0        0     2303 2024-04-11 17:57:36.485161 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_locker.py
+-rw-r--r--   0        0        0     1981 2024-04-11 17:57:39.285140 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_locker_params.py
+-rw-r--r--   0        0        0     1858 2024-04-11 17:57:40.888461 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_vote_delegate.py
+-rw-r--r--   0        0        0     1882 2024-04-11 17:57:42.665114 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/toggle_max_lock.py
+-rw-r--r--   0        0        0     1966 2024-04-11 17:57:44.425101 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/withdraw.py
+-rw-r--r--   0        0        0      370 2024-03-31 17:49:04.737101 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/program_id.py
+-rw-r--r--   0        0        0      286 2024-03-31 20:17:33.131741 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/types/__init__.py
+-rw-r--r--   0        0        0     2921 2024-04-12 10:17:40.286689 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/types/locker_params.py
+-rw-r--r--   0        0        0     5913 2024-04-18 21:19:20.496586 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/batcher.py
+-rw-r--r--   0        0        0     3505 2024-04-11 17:55:50.679294 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/derive.py
+-rw-r--r--   0        0        0     5215 2024-04-12 10:06:06.031872 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/governor.py
+-rw-r--r--   0        0        0    35952 2024-03-07 23:20:55.315692 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/idls/governor_idl.json
+-rw-r--r--   0        0        0    22431 2024-03-30 16:31:34.471154 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/idls/locked_voter_idl.json
+-rw-r--r--   0        0        0    29684 2024-03-30 16:32:50.590465 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/idls/smart_wallet_idl.json
+-rw-r--r--   0        0        0        0 2024-03-31 17:28:08.180510 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/smart_wallet.py
+-rw-r--r--   0        0        0     2778 2024-04-12 09:57:04.279183 sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/voter.py
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 sapysol_jupiter_dao-0.2.0/PKG-INFO
```

### Comparing `sapysol_jupiter_dao-0.1.0/LICENSE` & `sapysol_jupiter_dao-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/README.md` & `sapysol_jupiter_dao-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 WARNING! `sapysol_jupiter_dao` is currently in `alpha` version, so, bugs, lack of tests and descriptions are expected. Some things may not work, future versions may bring breaking changes.
 
 WARNING! only casting initial vote is implemented! Changing vote, depositing JUP, withdrawing JUP is yet to be implemented!
 
 # Installation
 
 ```sh
-pip install sapysol
+pip install sapysol-jupiter-dao
 ```
 
 Note: Requires Python >= 3.10.
 
 # Usage
 
 ```py
@@ -52,14 +52,18 @@
 
 # Start voting
 batcher.Start()
 ```
 
 TODO
 
+# Changelog
+
+v.0.2.0 - Add `voteOverride` param to `SapysolJupiterDaoBatcher` which allows to change existing votes.
+
 # Contributing
 
 TODO
 
 # Tests
 
 TODO
```

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/governor.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/governor.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/option_proposal_meta.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/option_proposal_meta.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal_meta.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/proposal_meta.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/accounts/vote.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/accounts/vote.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/errors/__init__.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/errors/anchor.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/errors/anchor.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/errors/custom.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/errors/custom.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/__init__.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/activate_proposal.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/activate_proposal.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/cancel_proposal.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/cancel_proposal.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/claim_reward.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/claim_reward.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_governor.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_governor.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_option_proposal_meta.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_option_proposal_meta.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal_meta.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/create_proposal_meta.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/new_vote.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/new_vote.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/queue_proposal.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/queue_proposal.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_governance_params.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_governance_params.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_locker.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_locker.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_vote.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_vote.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_voting_reward.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/instructions/set_voting_reward.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/__init__.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/governance_parameters.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/governance_parameters.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_account_meta.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_account_meta.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_instruction.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_instruction.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_state.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_state.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_type.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/proposal_type.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_governor/types/voting_reward.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_governor/types/voting_reward.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/accounts/escrow.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/accounts/escrow.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/accounts/locker.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/accounts/locker.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/errors/__init__.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/errors/anchor.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/errors/anchor.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/errors/custom.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/errors/custom.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/__init__.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/activate_proposal.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/activate_proposal.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/cast_vote.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/cast_vote.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/extend_lock_duration.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/extend_lock_duration.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/increase_locked_amount.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/increase_locked_amount.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_escrow.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_escrow.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_locker.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/new_locker.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_locker_params.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_locker_params.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_vote_delegate.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/set_vote_delegate.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/toggle_max_lock.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/toggle_max_lock.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/instructions/withdraw.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/instructions/withdraw.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/anchorpy_voter/types/locker_params.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/anchorpy_voter/types/locker_params.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/batcher.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/batcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 # 
 class SapysolJupiterDaoBatcher:
     def __init__(self, 
                  connection:         Client,
                  proposalAddress:    SapysolPubkey,
                  votersList:         List[SapysolKeypair],
                  voteSide:           int,
+                 voteOverride:       bool = False,
                  connectionOverride: List[Union[str, Client]] = None,
                  txParams:           SapysolTxParams = SapysolTxParams(),
                  computePriceTx:     int = 1,
                  numThreads:         int = 20):
 
         self.CONNECTION:       Client                   = connection
         self.PROPOSAL_ADDRESS: Pubkey                   = MakePubkey(proposalAddress)
         self.VOTERS_LIST:      List[Keypair]            = [MakeKeypair(k) for k in votersList]
         self.VOTE_SIDE:        int                      = voteSide
+        self.VOTE_OVERRIDE:    bool                     = voteOverride
         self.TX_PARAMS:        SapysolTxParams          = txParams
         self.COMPUTE_PRICE_TX: int                      = computePriceTx
         self.CONN_OVERRIDE:    List[Union[str, Client]] = connectionOverride
         self.DISTRIBUTOR_LIST: dict                     = {}
         self.BATCHER:          SapysolBatcher = SapysolBatcher(callback    = self.VoteSingle,
                                                                entityList  = self.VOTERS_LIST,
                                                                entityKwarg = "voter",
@@ -54,46 +56,53 @@
             voteExists: bool = CheckVoteExists(connection      = self.CONNECTION,
                                                proposalAddress = self.PROPOSAL_ADDRESS,
                                                voterAddress    = _voterAddress)
             if voteExists:
                 voteSide, votePower = CheckVoteSide(connection      = self.CONNECTION,
                                                     proposalAddress = self.PROPOSAL_ADDRESS,
                                                     voterAddress    = _voterAddress)
-                print(f"Voter: {_voter.pubkey()} already voted (side: {voteSide}, power: {votePower/JUP_DELIMITER}), skipping...")
-                # TODO: check vote for who and tell
-                return
+
+                # Recast a vote only if previous one is for the other candidate
+                if self.VOTE_OVERRIDE and self.VOTE_SIDE != voteSide:
+                    print(f"Voter: {str(_voter.pubkey()):>44} already voted (side: {voteSide:>2}, power: {votePower/JUP_DELIMITER}), but voteOverride = True...")
+                else:
+                    print(f"Voter: {str(_voter.pubkey()):>44} already voted (side: {voteSide:>2}, power: {votePower/JUP_DELIMITER}), skipping...")
+                    return
 
             proposal: Proposal = Proposal.fetch(conn=self.CONNECTION, address=self.PROPOSAL_ADDRESS )
             governor: Governor = Governor.fetch(conn=self.CONNECTION, address=proposal.governor)
 
             escrowExists: bool = CheckEscrowExists(connection    = self.CONNECTION,
                                                    lockerAddress = governor.locker,
                                                    voterAddress  = _voterAddress)
             if not escrowExists:
-                print(f"Voter: {_voter.pubkey()} no escrow, can't vote, skipping...")
+                print(f"Voter: {str(_voter.pubkey()):>44} no escrow, can't vote, skipping...")
                 return
 
-            print(f"Voter: {_voter.pubkey()} - voting...")
+            print(f"Voter: {str(_voter.pubkey()):>44} - voting...")
 
             newVote: Instruction = NewVoteIx(connection      = self.CONNECTION, 
                                              proposalAddress = self.PROPOSAL_ADDRESS, 
                                              voterAddress    = _voterAddress)
 
             castVote: Instruction = CastVoteIx(connection      = self.CONNECTION,
                                                proposalAddress = self.PROPOSAL_ADDRESS,
                                                voterAddress    = _voter,
                                                voteSide        = self.VOTE_SIDE)
 
+            ixList: List[Instruction] = []
+            ixList.append(ComputeBudgetIx())
+            ixList.append(ComputePriceIx(self.COMPUTE_PRICE_TX))
+            if not voteExists:
+                ixList.append(newVote)
+            ixList.append(castVote)
+
+
             tx: SapysolTx = SapysolTx(connection=self.CONNECTION, payer=_voter)
-            tx.FromInstructionsLegacy(instructions=[
-                ComputeBudgetIx(),
-                ComputePriceIx(self.COMPUTE_PRICE_TX),
-                newVote,
-                castVote,
-            ])
+            tx.FromInstructionsLegacy(instructions=ixList)
             result: SapysolTxStatus = tx.Sign([_voter]).SendAndWait(connectionOverride=self.CONN_OVERRIDE)
             if result == SapysolTxStatus.SUCCESS:
                 break
 
     # ========================================
     #
     def Start(self, **kwargs) -> None:
```

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/derive.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/derive.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/governor.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/governor.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/idls/governor_idl.json` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/idls/governor_idl.json`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/idls/locked_voter_idl.json` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/idls/locked_voter_idl.json`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/idls/smart_wallet_idl.json` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/idls/smart_wallet_idl.json`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/sapysol_jupiter_dao/voter.py` & `sapysol_jupiter_dao-0.2.0/sapysol_jupiter_dao/voter.py`

 * *Files identical despite different names*

### Comparing `sapysol_jupiter_dao-0.1.0/PKG-INFO` & `sapysol_jupiter_dao-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapysol-jupiter-dao
-Version: 0.1.0
+Version: 0.2.0
 Summary: sapysol Jupiter LFG DAO Vote implementation
 License: MIT
 Author: Anton Platonov
 Author-email: anton@platonov.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 WARNING! `sapysol_jupiter_dao` is currently in `alpha` version, so, bugs, lack of tests and descriptions are expected. Some things may not work, future versions may bring breaking changes.
 
 WARNING! only casting initial vote is implemented! Changing vote, depositing JUP, withdrawing JUP is yet to be implemented!
 
 # Installation
 
 ```sh
-pip install sapysol
+pip install sapysol-jupiter-dao
 ```
 
 Note: Requires Python >= 3.10.
 
 # Usage
 
 ```py
@@ -70,14 +70,18 @@
 
 # Start voting
 batcher.Start()
 ```
 
 TODO
 
+# Changelog
+
+v.0.2.0 - Add `voteOverride` param to `SapysolJupiterDaoBatcher` which allows to change existing votes.
+
 # Contributing
 
 TODO
 
 # Tests
 
 TODO
```

