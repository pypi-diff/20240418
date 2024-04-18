# Comparing `tmp/cs2_battle_bot_api_client-0.0.6.tar.gz` & `tmp/cs2_battle_bot_api_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2_battle_bot_api_client-0.0.6.tar", max compression
+gzip compressed data, was "cs2_battle_bot_api_client-0.0.7.tar", max compression
```

## Comparing `cs2_battle_bot_api_client-0.0.6.tar` & `cs2_battle_bot_api_client-0.0.7.tar`

### file list

```diff
@@ -1,126 +1,127 @@
--rw-r--r--   0        0        0     5128 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/README.md
--rw-r--r--   0        0        0      161 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/__init__.py
--rw-r--r--   0        0        0       45 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/__init__.py
--rw-r--r--   0        0        0     4607 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py
--rw-r--r--   0        0        0     2212 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py
--rw-r--r--   0        0        0     3927 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py
--rw-r--r--   0        0        0     5082 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py
--rw-r--r--   0        0        0     3359 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py
--rw-r--r--   0        0        0     4808 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py
--rw-r--r--   0        0        0     4568 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_create.py
--rw-r--r--   0        0        0     2205 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py
--rw-r--r--   0        0        0     3841 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_list.py
--rw-r--r--   0        0        0     4803 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py
--rw-r--r--   0        0        0     3273 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py
--rw-r--r--   0        0        0     4542 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_update.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/__init__.py
--rw-r--r--   0        0        0     4254 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_create.py
--rw-r--r--   0        0        0     2203 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_destroy.py
--rw-r--r--   0        0        0     3813 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_list.py
--rw-r--r--   0        0        0     4712 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_partial_update.py
--rw-r--r--   0        0        0     3246 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_retrieve.py
--rw-r--r--   0        0        0     4455 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_update.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/__init__.py
--rw-r--r--   0        0        0     4947 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_ban_create.py
--rw-r--r--   0        0        0     3293 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py
--rw-r--r--   0        0        0     3360 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py
--rw-r--r--   0        0        0     4564 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_create.py
--rw-r--r--   0        0        0     2206 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_destroy.py
--rw-r--r--   0        0        0     4905 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_join_create.py
--rw-r--r--   0        0        0     3842 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_list.py
--rw-r--r--   0        0        0     4549 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_load_create.py
--rw-r--r--   0        0        0     4804 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_partial_update.py
--rw-r--r--   0        0        0     4993 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_pick_create.py
--rw-r--r--   0        0        0     3437 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py
--rw-r--r--   0        0        0     4553 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py
--rw-r--r--   0        0        0     3274 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_retrieve.py
--rw-r--r--   0        0        0     4552 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py
--rw-r--r--   0        0        0     4543 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_update.py
--rw-r--r--   0        0        0     4345 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_create.py
--rw-r--r--   0        0        0     2206 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_destroy.py
--rw-r--r--   0        0        0     3855 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_list.py
--rw-r--r--   0        0        0     4849 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_partial_update.py
--rw-r--r--   0        0        0     3287 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_retrieve.py
--rw-r--r--   0        0        0     4586 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_update.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/schema/__init__.py
--rw-r--r--   0        0        0     4900 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/schema/schema_retrieve.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_create.py
--rw-r--r--   0        0        0     2206 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_destroy.py
--rw-r--r--   0        0        0     3292 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py
--rw-r--r--   0        0        0     4834 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_list.py
--rw-r--r--   0        0        0     4849 2024-04-18 08:43:40.713973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_partial_update.py
--rw-r--r--   0        0        0     3287 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_retrieve.py
--rw-r--r--   0        0        0     4586 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_update.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/__init__.py
--rw-r--r--   0        0        0     4519 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py
--rw-r--r--   0        0        0     2210 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py
--rw-r--r--   0        0        0     3899 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py
--rw-r--r--   0        0        0     4990 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py
--rw-r--r--   0        0        0     3331 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py
--rw-r--r--   0        0        0     4720 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/__init__.py
--rw-r--r--   0        0        0     4297 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_create.py
--rw-r--r--   0        0        0     2204 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_destroy.py
--rw-r--r--   0        0        0     3827 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_list.py
--rw-r--r--   0        0        0     4757 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_partial_update.py
--rw-r--r--   0        0        0     3259 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_retrieve.py
--rw-r--r--   0        0        0     4498 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_update.py
--rw-r--r--   0        0        0    12417 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/client.py
--rw-r--r--   0        0        0      546 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/errors.py
--rw-r--r--   0        0        0     3028 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/__init__.py
--rw-r--r--   0        0        0     4146 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_guild.py
--rw-r--r--   0        0        0     2364 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_guild_member.py
--rw-r--r--   0        0        0     7414 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_match.py
--rw-r--r--   0        0        0     1208 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_match_cvars.py
--rw-r--r--   0        0        0     3342 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/discord_user.py
--rw-r--r--   0        0        0     7098 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/guild.py
--rw-r--r--   0        0        0     3150 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/map_.py
--rw-r--r--   0        0        0     2454 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/map_ban.py
--rw-r--r--   0        0        0      237 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/map_sides_enum.py
--rw-r--r--   0        0        0    15072 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match.py
--rw-r--r--   0        0        0     2534 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_ban_map.py
--rw-r--r--   0        0        0     2287 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_ban_map_result.py
--rw-r--r--   0        0        0     4379 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config.py
--rw-r--r--   0        0        0     1208 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config_cvars.py
--rw-r--r--   0        0        0     1211 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config_team_1.py
--rw-r--r--   0        0        0     1211 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config_team_2.py
--rw-r--r--   0        0        0     2507 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_map_selected.py
--rw-r--r--   0        0        0     2539 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_pick_map.py
--rw-r--r--   0        0        0     2312 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_pick_map_result.py
--rw-r--r--   0        0        0     2160 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_player_join.py
--rw-r--r--   0        0        0      166 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_type_enum.py
--rw-r--r--   0        0        0     2284 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/nested.py
--rw-r--r--   0        0        0     3629 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_discord_user_list.py
--rw-r--r--   0        0        0     3552 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_guild_list.py
--rw-r--r--   0        0        0     3530 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_map_list.py
--rw-r--r--   0        0        0     3552 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_match_list.py
--rw-r--r--   0        0        0     3564 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_player_list.py
--rw-r--r--   0        0        0     3564 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_server_list.py
--rw-r--r--   0        0        0     3605 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_steam_user_list.py
--rw-r--r--   0        0        0     3540 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_team_list.py
--rw-r--r--   0        0        0     4717 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_discord_user.py
--rw-r--r--   0        0        0     8926 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_guild.py
--rw-r--r--   0        0        0     4506 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_map.py
--rw-r--r--   0        0        0    20077 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_match.py
--rw-r--r--   0        0        0     5742 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_player.py
--rw-r--r--   0        0        0     6039 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_server.py
--rw-r--r--   0        0        0     8050 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_steam_user.py
--rw-r--r--   0        0        0     6331 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_team.py
--rw-r--r--   0        0        0     3528 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/player.py
--rw-r--r--   0        0        0     1605 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/schema_retrieve_lang.py
--rw-r--r--   0        0        0     1256 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py
--rw-r--r--   0        0        0     5603 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/server.py
--rw-r--r--   0        0        0      207 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/status_enum.py
--rw-r--r--   0        0        0     6814 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/steam_user.py
--rw-r--r--   0        0        0     4710 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/team.py
--rw-r--r--   0        0        0      161 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/type_enum.py
--rw-r--r--   0        0        0       25 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/py.typed
--rw-r--r--   0        0        0      985 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/types.py
--rw-r--r--   0        0        0      577 2024-04-18 08:43:40.717973 cs2_battle_bot_api_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 cs2_battle_bot_api_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     5128 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/README.md
+-rw-r--r--   0        0        0      161 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/__init__.py
+-rw-r--r--   0        0        0     3645 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py
+-rw-r--r--   0        0        0     2212 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py
+-rw-r--r--   0        0        0     3927 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py
+-rw-r--r--   0        0        0     3973 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py
+-rw-r--r--   0        0        0     3359 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py
+-rw-r--r--   0        0        0     3846 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/__init__.py
+-rw-r--r--   0        0        0     3994 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py
+-rw-r--r--   0        0        0     3606 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_create.py
+-rw-r--r--   0        0        0     2265 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py
+-rw-r--r--   0        0        0     3841 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_list.py
+-rw-r--r--   0        0        0     3928 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py
+-rw-r--r--   0        0        0     3381 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py
+-rw-r--r--   0        0        0     3814 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/__init__.py
+-rw-r--r--   0        0        0     3460 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_create.py
+-rw-r--r--   0        0        0     2203 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_destroy.py
+-rw-r--r--   0        0        0     3813 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_list.py
+-rw-r--r--   0        0        0     3771 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_partial_update.py
+-rw-r--r--   0        0        0     3246 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_retrieve.py
+-rw-r--r--   0        0        0     3661 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/__init__.py
+-rw-r--r--   0        0        0     3985 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_ban_create.py
+-rw-r--r--   0        0        0     3293 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py
+-rw-r--r--   0        0        0     3360 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py
+-rw-r--r--   0        0        0     4178 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_create.py
+-rw-r--r--   0        0        0     2206 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_destroy.py
+-rw-r--r--   0        0        0     3859 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_join_create.py
+-rw-r--r--   0        0        0     3842 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_list.py
+-rw-r--r--   0        0        0     3713 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_load_create.py
+-rw-r--r--   0        0        0     3821 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_partial_update.py
+-rw-r--r--   0        0        0     4010 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_pick_create.py
+-rw-r--r--   0        0        0     3437 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py
+-rw-r--r--   0        0        0     3717 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py
+-rw-r--r--   0        0        0     3274 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_retrieve.py
+-rw-r--r--   0        0        0     3716 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py
+-rw-r--r--   0        0        0     3707 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_update.py
+-rw-r--r--   0        0        0     3509 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_create.py
+-rw-r--r--   0        0        0     2206 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_destroy.py
+-rw-r--r--   0        0        0     3855 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_list.py
+-rw-r--r--   0        0        0     3845 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_partial_update.py
+-rw-r--r--   0        0        0     3287 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_retrieve.py
+-rw-r--r--   0        0        0     3729 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/schema/__init__.py
+-rw-r--r--   0        0        0     4900 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/schema/schema_retrieve.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-18 10:17:20.581774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_create.py
+-rw-r--r--   0        0        0     2206 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_destroy.py
+-rw-r--r--   0        0        0     3292 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py
+-rw-r--r--   0        0        0     4834 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_list.py
+-rw-r--r--   0        0        0     3845 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_partial_update.py
+-rw-r--r--   0        0        0     3287 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_retrieve.py
+-rw-r--r--   0        0        0     3729 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/__init__.py
+-rw-r--r--   0        0        0     3599 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py
+-rw-r--r--   0        0        0     2210 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py
+-rw-r--r--   0        0        0     3899 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py
+-rw-r--r--   0        0        0     3923 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py
+-rw-r--r--   0        0        0     3331 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py
+-rw-r--r--   0        0        0     3800 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/__init__.py
+-rw-r--r--   0        0        0     3482 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_create.py
+-rw-r--r--   0        0        0     2204 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_destroy.py
+-rw-r--r--   0        0        0     3827 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_list.py
+-rw-r--r--   0        0        0     3795 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_partial_update.py
+-rw-r--r--   0        0        0     3259 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_retrieve.py
+-rw-r--r--   0        0        0     3683 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_update.py
+-rw-r--r--   0        0        0    12417 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/client.py
+-rw-r--r--   0        0        0      546 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/errors.py
+-rw-r--r--   0        0        0     3126 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_guild.py
+-rw-r--r--   0        0        0     1663 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_guild_member.py
+-rw-r--r--   0        0        0     4900 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_match.py
+-rw-r--r--   0        0        0     1208 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_match_cvars.py
+-rw-r--r--   0        0        0     2312 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/discord_user.py
+-rw-r--r--   0        0        0     4937 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/guild.py
+-rw-r--r--   0        0        0     2192 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/map_.py
+-rw-r--r--   0        0        0     2454 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/map_ban.py
+-rw-r--r--   0        0        0      237 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/map_sides_enum.py
+-rw-r--r--   0        0        0     9921 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match.py
+-rw-r--r--   0        0        0     1743 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_ban_map.py
+-rw-r--r--   0        0        0     2287 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_ban_map_result.py
+-rw-r--r--   0        0        0     4379 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config.py
+-rw-r--r--   0        0        0     1208 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config_cvars.py
+-rw-r--r--   0        0        0     1211 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config_team_1.py
+-rw-r--r--   0        0        0     1211 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config_team_2.py
+-rw-r--r--   0        0        0     2507 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_map_selected.py
+-rw-r--r--   0        0        0     1748 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_pick_map.py
+-rw-r--r--   0        0        0     2312 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_pick_map_result.py
+-rw-r--r--   0        0        0     1550 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_player_join.py
+-rw-r--r--   0        0        0      166 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_type_enum.py
+-rw-r--r--   0        0        0     1275 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/matches_create_response_400.py
+-rw-r--r--   0        0        0     2284 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/nested.py
+-rw-r--r--   0        0        0     3629 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_discord_user_list.py
+-rw-r--r--   0        0        0     3552 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_guild_list.py
+-rw-r--r--   0        0        0     3530 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_map_list.py
+-rw-r--r--   0        0        0     3552 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_match_list.py
+-rw-r--r--   0        0        0     3564 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_player_list.py
+-rw-r--r--   0        0        0     3564 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_server_list.py
+-rw-r--r--   0        0        0     3605 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_steam_user_list.py
+-rw-r--r--   0        0        0     3540 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_team_list.py
+-rw-r--r--   0        0        0     3336 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_discord_user.py
+-rw-r--r--   0        0        0     6184 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_guild.py
+-rw-r--r--   0        0        0     3205 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_map.py
+-rw-r--r--   0        0        0    13243 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_match.py
+-rw-r--r--   0        0        0     4147 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_player.py
+-rw-r--r--   0        0        0     4068 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_server.py
+-rw-r--r--   0        0        0     5851 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_steam_user.py
+-rw-r--r--   0        0        0     4483 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_team.py
+-rw-r--r--   0        0        0     2544 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/player.py
+-rw-r--r--   0        0        0     1605 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/schema_retrieve_lang.py
+-rw-r--r--   0        0        0     1256 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py
+-rw-r--r--   0        0        0     3745 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/server.py
+-rw-r--r--   0        0        0      207 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/status_enum.py
+-rw-r--r--   0        0        0     4952 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/steam_user.py
+-rw-r--r--   0        0        0     3374 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/team.py
+-rw-r--r--   0        0        0      161 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/type_enum.py
+-rw-r--r--   0        0        0       25 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/py.typed
+-rw-r--r--   0        0        0      985 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/types.py
+-rw-r--r--   0        0        0      577 2024-04-18 10:17:20.585774 cs2_battle_bot_api_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 cs2_battle_bot_api_client-0.0.7/PKG-INFO
```

### Comparing `cs2_battle_bot_api_client-0.0.6/README.md` & `cs2_battle_bot_api_client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,57 +2,44 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.discord_user import DiscordUser
+from ...models.patched_discord_user import PatchedDiscordUser
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: PatchedDiscordUser,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/discord-users/",
+        "method": "patch",
+        "url": f"/api/discord-users/{id}/",
     }
 
-    if isinstance(body, DiscordUser):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, DiscordUser):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, DiscordUser):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[DiscordUser]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = DiscordUser.from_dict(response.json())
+    if response.status_code == HTTPStatus.OK:
+        response_200 = DiscordUser.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[DiscordUser]:
@@ -61,130 +48,118 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: PatchedDiscordUser,
 ) -> Response[DiscordUser]:
     """
     Args:
-        body (DiscordUser):
-        body (DiscordUser):
-        body (DiscordUser):
+        id (str):
+        body (PatchedDiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DiscordUser]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: PatchedDiscordUser,
 ) -> Optional[DiscordUser]:
     """
     Args:
-        body (DiscordUser):
-        body (DiscordUser):
-        body (DiscordUser):
+        id (str):
+        body (PatchedDiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         DiscordUser
     """
 
     return sync_detailed(
+        id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: PatchedDiscordUser,
 ) -> Response[DiscordUser]:
     """
     Args:
-        body (DiscordUser):
-        body (DiscordUser):
-        body (DiscordUser):
+        id (str):
+        body (PatchedDiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DiscordUser]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: PatchedDiscordUser,
 ) -> Optional[DiscordUser]:
     """
     Args:
-        body (DiscordUser):
-        body (DiscordUser):
-        body (DiscordUser):
+        id (str):
+        body (PatchedDiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         DiscordUser
     """
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,49 +2,33 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.discord_user import DiscordUser
-from ...models.patched_discord_user import PatchedDiscordUser
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
     *,
-    body: Union[
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "patch",
+        "method": "put",
         "url": f"/api/discord-users/{id}/",
     }
 
-    if isinstance(body, PatchedDiscordUser):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, PatchedDiscordUser):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, PatchedDiscordUser):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[DiscordUser]:
     if response.status_code == HTTPStatus.OK:
@@ -66,26 +50,20 @@
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Response[DiscordUser]:
     """
     Args:
         id (str):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
+        body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DiscordUser]
@@ -103,26 +81,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Optional[DiscordUser]:
     """
     Args:
         id (str):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
+        body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         DiscordUser
@@ -135,26 +107,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Response[DiscordUser]:
     """
     Args:
         id (str):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
+        body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DiscordUser]
@@ -170,26 +136,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-        PatchedDiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Optional[DiscordUser]:
     """
     Args:
         id (str):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
-        body (PatchedDiscordUser):
+        body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         DiscordUser
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,54 +6,38 @@
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.discord_user import DiscordUser
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": f"/api/discord-users/{id}/",
+        "method": "post",
+        "url": "/api/discord-users/",
     }
 
-    if isinstance(body, DiscordUser):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, DiscordUser):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, DiscordUser):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[DiscordUser]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = DiscordUser.from_dict(response.json())
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = DiscordUser.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[DiscordUser]:
@@ -62,142 +46,106 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Response[DiscordUser]:
     """
     Args:
-        id (str):
-        body (DiscordUser):
-        body (DiscordUser):
         body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DiscordUser]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Optional[DiscordUser]:
     """
     Args:
-        id (str):
-        body (DiscordUser):
-        body (DiscordUser):
         body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         DiscordUser
     """
 
     return sync_detailed(
-        id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Response[DiscordUser]:
     """
     Args:
-        id (str):
-        body (DiscordUser):
-        body (DiscordUser):
         body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DiscordUser]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        DiscordUser,
-        DiscordUser,
-        DiscordUser,
-    ],
+    body: DiscordUser,
 ) -> Optional[DiscordUser]:
     """
     Args:
-        id (str):
-        body (DiscordUser):
-        body (DiscordUser):
         body (DiscordUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         DiscordUser
     """
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,44 +7,29 @@
 from ...client import AuthenticatedClient, Client
 from ...models.create_guild_member import CreateGuildMember
 from ...models.guild import Guild
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
+    guild_id: str,
     *,
-    body: Union[
-        CreateGuildMember,
-        CreateGuildMember,
-        CreateGuildMember,
-    ],
+    body: CreateGuildMember,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
-        "url": f"/api/guilds/{id}/add_member/",
+        "url": f"/api/guilds/{guild_id}/add_member/",
     }
 
-    if isinstance(body, CreateGuildMember):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, CreateGuildMember):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, CreateGuildMember):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Guild]:
     if response.status_code == HTTPStatus.OK:
@@ -63,142 +48,118 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuildMember,
-        CreateGuildMember,
-        CreateGuildMember,
-    ],
+    body: CreateGuildMember,
 ) -> Response[Guild]:
     """
     Args:
-        id (str):
-        body (CreateGuildMember):
-        body (CreateGuildMember):
+        guild_id (str):
         body (CreateGuildMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Guild]
     """
 
     kwargs = _get_kwargs(
-        id=id,
+        guild_id=guild_id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuildMember,
-        CreateGuildMember,
-        CreateGuildMember,
-    ],
+    body: CreateGuildMember,
 ) -> Optional[Guild]:
     """
     Args:
-        id (str):
-        body (CreateGuildMember):
-        body (CreateGuildMember):
+        guild_id (str):
         body (CreateGuildMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Guild
     """
 
     return sync_detailed(
-        id=id,
+        guild_id=guild_id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuildMember,
-        CreateGuildMember,
-        CreateGuildMember,
-    ],
+    body: CreateGuildMember,
 ) -> Response[Guild]:
     """
     Args:
-        id (str):
-        body (CreateGuildMember):
-        body (CreateGuildMember):
+        guild_id (str):
         body (CreateGuildMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Guild]
     """
 
     kwargs = _get_kwargs(
-        id=id,
+        guild_id=guild_id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuildMember,
-        CreateGuildMember,
-        CreateGuildMember,
-    ],
+    body: CreateGuildMember,
 ) -> Optional[Guild]:
     """
     Args:
-        id (str):
-        body (CreateGuildMember):
-        body (CreateGuildMember):
+        guild_id (str):
         body (CreateGuildMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Guild
     """
 
     return (
         await asyncio_detailed(
-            id=id,
+            guild_id=guild_id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,45 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.create_guild import CreateGuild
 from ...models.guild import Guild
+from ...models.patched_guild import PatchedGuild
 from ...types import Response
 
 
 def _get_kwargs(
+    guild_id: str,
     *,
-    body: Union[
-        CreateGuild,
-        CreateGuild,
-        CreateGuild,
-    ],
+    body: PatchedGuild,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/guilds/",
+        "method": "patch",
+        "url": f"/api/guilds/{guild_id}/",
     }
 
-    if isinstance(body, CreateGuild):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, CreateGuild):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, CreateGuild):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Guild]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = Guild.from_dict(response.json())
+    if response.status_code == HTTPStatus.OK:
+        response_200 = Guild.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Guild]:
@@ -62,130 +48,118 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuild,
-        CreateGuild,
-        CreateGuild,
-    ],
+    body: PatchedGuild,
 ) -> Response[Guild]:
     """
     Args:
-        body (CreateGuild):
-        body (CreateGuild):
-        body (CreateGuild):
+        guild_id (str):
+        body (PatchedGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Guild]
     """
 
     kwargs = _get_kwargs(
+        guild_id=guild_id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuild,
-        CreateGuild,
-        CreateGuild,
-    ],
+    body: PatchedGuild,
 ) -> Optional[Guild]:
     """
     Args:
-        body (CreateGuild):
-        body (CreateGuild):
-        body (CreateGuild):
+        guild_id (str):
+        body (PatchedGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Guild
     """
 
     return sync_detailed(
+        guild_id=guild_id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuild,
-        CreateGuild,
-        CreateGuild,
-    ],
+    body: PatchedGuild,
 ) -> Response[Guild]:
     """
     Args:
-        body (CreateGuild):
-        body (CreateGuild):
-        body (CreateGuild):
+        guild_id (str):
+        body (PatchedGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Guild]
     """
 
     kwargs = _get_kwargs(
+        guild_id=guild_id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateGuild,
-        CreateGuild,
-        CreateGuild,
-    ],
+    body: PatchedGuild,
 ) -> Optional[Guild]:
     """
     Args:
-        body (CreateGuild):
-        body (CreateGuild):
-        body (CreateGuild):
+        guild_id (str):
+        body (PatchedGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Guild
     """
 
     return (
         await asyncio_detailed(
+            guild_id=guild_id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_destroy.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_kwargs(
     id: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "delete",
-        "url": f"/api/guilds/{id}/",
+        "url": f"/api/maps/{id}/",
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_join_create.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,77 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.guild import Guild
-from ...models.patched_guild import PatchedGuild
+from ...models.match import Match
+from ...models.match_player_join import MatchPlayerJoin
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
+    id: int,
     *,
-    body: Union[
-        PatchedGuild,
-        PatchedGuild,
-        PatchedGuild,
-    ],
+    body: MatchPlayerJoin,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "patch",
-        "url": f"/api/guilds/{id}/",
+        "method": "post",
+        "url": f"/api/matches/{id}/join/",
     }
 
-    if isinstance(body, PatchedGuild):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, PatchedGuild):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, PatchedGuild):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Guild]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Guild.from_dict(response.json())
+        response_200 = Match.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Guild]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedGuild,
-        PatchedGuild,
-        PatchedGuild,
-    ],
-) -> Response[Guild]:
+    body: MatchPlayerJoin,
+) -> Response[Match]:
     """
     Args:
-        id (str):
-        body (PatchedGuild):
-        body (PatchedGuild):
-        body (PatchedGuild):
+        id (int):
+        body (MatchPlayerJoin):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Guild]
+        Response[Match]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -100,103 +79,85 @@
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedGuild,
-        PatchedGuild,
-        PatchedGuild,
-    ],
-) -> Optional[Guild]:
+    body: MatchPlayerJoin,
+) -> Optional[Match]:
     """
     Args:
-        id (str):
-        body (PatchedGuild):
-        body (PatchedGuild):
-        body (PatchedGuild):
+        id (int):
+        body (MatchPlayerJoin):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Guild
+        Match
     """
 
     return sync_detailed(
         id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedGuild,
-        PatchedGuild,
-        PatchedGuild,
-    ],
-) -> Response[Guild]:
+    body: MatchPlayerJoin,
+) -> Response[Match]:
     """
     Args:
-        id (str):
-        body (PatchedGuild):
-        body (PatchedGuild):
-        body (PatchedGuild):
+        id (int):
+        body (MatchPlayerJoin):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Guild]
+        Response[Match]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedGuild,
-        PatchedGuild,
-        PatchedGuild,
-    ],
-) -> Optional[Guild]:
+    body: MatchPlayerJoin,
+) -> Optional[Match]:
     """
     Args:
-        id (str):
-        body (PatchedGuild):
-        body (PatchedGuild):
-        body (PatchedGuild):
+        id (int):
+        body (MatchPlayerJoin):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Guild
+        Match
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
             body=body,
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_retrieve.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.guild import Guild
+from ...models.match import Match
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
+    id: int,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/guilds/{id}/",
+        "url": f"/api/matches/{id}/",
     }
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Guild]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Guild.from_dict(response.json())
+        response_200 = Match.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Guild]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-) -> Response[Guild]:
+) -> Response[Match]:
     """
     Args:
-        id (str):
+        id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Guild]
+        Response[Match]
     """
 
     kwargs = _get_kwargs(
         id=id,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-) -> Optional[Guild]:
+) -> Optional[Match]:
     """
     Args:
-        id (str):
+        id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Guild
+        Match
     """
 
     return sync_detailed(
         id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-) -> Response[Guild]:
+) -> Response[Match]:
     """
     Args:
-        id (str):
+        id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Guild]
+        Response[Match]
     """
 
     kwargs = _get_kwargs(
         id=id,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
+    id: int,
     *,
     client: AuthenticatedClient,
-) -> Optional[Guild]:
+) -> Optional[Match]:
     """
     Args:
-        id (str):
+        id (int):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Guild
+        Match
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
         )
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/guilds/guilds_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_create.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,44 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
+from ...models.create_guild import CreateGuild
 from ...models.guild import Guild
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
-    body: Union[
-        Guild,
-        Guild,
-        Guild,
-    ],
+    body: CreateGuild,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": f"/api/guilds/{id}/",
+        "method": "post",
+        "url": "/api/guilds/",
     }
 
-    if isinstance(body, Guild):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Guild):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Guild):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Guild]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Guild.from_dict(response.json())
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = Guild.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Guild]:
@@ -62,142 +47,106 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Guild,
-        Guild,
-        Guild,
-    ],
+    body: CreateGuild,
 ) -> Response[Guild]:
     """
     Args:
-        id (str):
-        body (Guild):
-        body (Guild):
-        body (Guild):
+        body (CreateGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Guild]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Guild,
-        Guild,
-        Guild,
-    ],
+    body: CreateGuild,
 ) -> Optional[Guild]:
     """
     Args:
-        id (str):
-        body (Guild):
-        body (Guild):
-        body (Guild):
+        body (CreateGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Guild
     """
 
     return sync_detailed(
-        id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Guild,
-        Guild,
-        Guild,
-    ],
+    body: CreateGuild,
 ) -> Response[Guild]:
     """
     Args:
-        id (str):
-        body (Guild):
-        body (Guild):
-        body (Guild):
+        body (CreateGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Guild]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Guild,
-        Guild,
-        Guild,
-    ],
+    body: CreateGuild,
 ) -> Optional[Guild]:
     """
     Args:
-        id (str):
-        body (Guild):
-        body (Guild):
-        body (Guild):
+        body (CreateGuild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Guild
     """
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_partial_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,190 +1,165 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.map_ import Map
+from ...models.patched_server import PatchedServer
+from ...models.server import Server
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
+    body: PatchedServer,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/maps/",
+        "method": "patch",
+        "url": f"/api/servers/{id}/",
     }
 
-    if isinstance(body, Map):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Map):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Map):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Map]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = Map.from_dict(response.json())
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Server]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = Server.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Map]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Server]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
-) -> Response[Map]:
+    body: PatchedServer,
+) -> Response[Server]:
     """
     Args:
-        body (Map):
-        body (Map):
-        body (Map):
+        id (str):
+        body (PatchedServer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Map]
+        Response[Server]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
-) -> Optional[Map]:
+    body: PatchedServer,
+) -> Optional[Server]:
     """
     Args:
-        body (Map):
-        body (Map):
-        body (Map):
+        id (str):
+        body (PatchedServer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Map
+        Server
     """
 
     return sync_detailed(
+        id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
-) -> Response[Map]:
+    body: PatchedServer,
+) -> Response[Server]:
     """
     Args:
-        body (Map):
-        body (Map):
-        body (Map):
+        id (str):
+        body (PatchedServer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Map]
+        Response[Server]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
-) -> Optional[Map]:
+    body: PatchedServer,
+) -> Optional[Server]:
     """
     Args:
-        body (Map):
-        body (Map):
-        body (Map):
+        id (str):
+        body (PatchedServer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Map
+        Server
     """
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_destroy.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_kwargs(
     id: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "delete",
-        "url": f"/api/maps/{id}/",
+        "url": f"/api/players/{id}/",
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/maps/maps_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/maps/maps_partial_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,48 +2,34 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.map_ import Map
+from ...models.patched_map import PatchedMap
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
     *,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
+    body: PatchedMap,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
+        "method": "patch",
         "url": f"/api/maps/{id}/",
     }
 
-    if isinstance(body, Map):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Map):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Map):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Map]:
     if response.status_code == HTTPStatus.OK:
@@ -65,26 +51,20 @@
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
+    body: PatchedMap,
 ) -> Response[Map]:
     """
     Args:
         id (str):
-        body (Map):
-        body (Map):
-        body (Map):
+        body (PatchedMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Map]
@@ -102,26 +82,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
+    body: PatchedMap,
 ) -> Optional[Map]:
     """
     Args:
         id (str):
-        body (Map):
-        body (Map):
-        body (Map):
+        body (PatchedMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Map
@@ -134,26 +108,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
+    body: PatchedMap,
 ) -> Response[Map]:
     """
     Args:
         id (str):
-        body (Map):
-        body (Map):
-        body (Map):
+        body (PatchedMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Map]
@@ -169,26 +137,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Map,
-        Map,
-        Map,
-    ],
+    body: PatchedMap,
 ) -> Optional[Map]:
     """
     Args:
         id (str):
-        body (Map):
-        body (Map):
-        body (Map):
+        body (PatchedMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Map
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_ban_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_ban_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,42 +9,27 @@
 from ...models.match_ban_map_result import MatchBanMapResult
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        MatchBanMap,
-        MatchBanMap,
-        MatchBanMap,
-    ],
+    body: MatchBanMap,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
         "url": f"/api/matches/{id}/ban/",
     }
 
-    if isinstance(body, MatchBanMap):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, MatchBanMap):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, MatchBanMap):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
@@ -70,26 +55,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchBanMap,
-        MatchBanMap,
-        MatchBanMap,
-    ],
+    body: MatchBanMap,
 ) -> Response[MatchBanMapResult]:
     """
     Args:
         id (int):
         body (MatchBanMap):
-        body (MatchBanMap):
-        body (MatchBanMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[MatchBanMapResult]
@@ -107,26 +86,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchBanMap,
-        MatchBanMap,
-        MatchBanMap,
-    ],
+    body: MatchBanMap,
 ) -> Optional[MatchBanMapResult]:
     """
     Args:
         id (int):
         body (MatchBanMap):
-        body (MatchBanMap):
-        body (MatchBanMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         MatchBanMapResult
@@ -139,26 +112,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchBanMap,
-        MatchBanMap,
-        MatchBanMap,
-    ],
+    body: MatchBanMap,
 ) -> Response[MatchBanMapResult]:
     """
     Args:
         id (int):
         body (MatchBanMap):
-        body (MatchBanMap):
-        body (MatchBanMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[MatchBanMapResult]
@@ -174,26 +141,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchBanMap,
-        MatchBanMap,
-        MatchBanMap,
-    ],
+    body: MatchBanMap,
 ) -> Optional[MatchBanMapResult]:
     """
     Args:
         id (int):
         body (MatchBanMap):
-        body (MatchBanMap):
-        body (MatchBanMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         MatchBanMapResult
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,93 +3,81 @@
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.create_match import CreateMatch
 from ...models.match import Match
+from ...models.matches_create_response_400 import MatchesCreateResponse400
 from ...types import Response
 
 
 def _get_kwargs(
     *,
-    body: Union[
-        CreateMatch,
-        CreateMatch,
-        CreateMatch,
-    ],
+    body: CreateMatch,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
         "url": "/api/matches/",
     }
 
-    if isinstance(body, CreateMatch):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, CreateMatch):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, CreateMatch):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
+def _parse_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Optional[Union[Match, MatchesCreateResponse400]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = Match.from_dict(response.json())
 
         return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = MatchesCreateResponse400.from_dict(response.json())
+
+        return response_400
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
+def _build_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Response[Union[Match, MatchesCreateResponse400]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateMatch,
-        CreateMatch,
-        CreateMatch,
-    ],
-) -> Response[Match]:
+    body: CreateMatch,
+) -> Response[Union[Match, MatchesCreateResponse400]]:
     """
     Args:
         body (CreateMatch):
-        body (CreateMatch):
-        body (CreateMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Match]
+        Response[Union[Match, MatchesCreateResponse400]]
     """
 
     kwargs = _get_kwargs(
         body=body,
     )
 
     response = client.get_httpx_client().request(
@@ -98,93 +86,75 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateMatch,
-        CreateMatch,
-        CreateMatch,
-    ],
-) -> Optional[Match]:
+    body: CreateMatch,
+) -> Optional[Union[Match, MatchesCreateResponse400]]:
     """
     Args:
         body (CreateMatch):
-        body (CreateMatch):
-        body (CreateMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Match
+        Union[Match, MatchesCreateResponse400]
     """
 
     return sync_detailed(
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateMatch,
-        CreateMatch,
-        CreateMatch,
-    ],
-) -> Response[Match]:
+    body: CreateMatch,
+) -> Response[Union[Match, MatchesCreateResponse400]]:
     """
     Args:
         body (CreateMatch):
-        body (CreateMatch):
-        body (CreateMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Match]
+        Response[Union[Match, MatchesCreateResponse400]]
     """
 
     kwargs = _get_kwargs(
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        CreateMatch,
-        CreateMatch,
-        CreateMatch,
-    ],
-) -> Optional[Match]:
+    body: CreateMatch,
+) -> Optional[Union[Match, MatchesCreateResponse400]]:
     """
     Args:
         body (CreateMatch):
-        body (CreateMatch):
-        body (CreateMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Match
+        Union[Match, MatchesCreateResponse400]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             body=body,
         )
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_join_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_update.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,49 +2,33 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.match import Match
-from ...models.match_player_join import MatchPlayerJoin
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-    ],
+    body: Match,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": f"/api/matches/{id}/join/",
+        "method": "put",
+        "url": f"/api/matches/{id}/",
     }
 
-    if isinstance(body, MatchPlayerJoin):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, MatchPlayerJoin):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, MatchPlayerJoin):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
@@ -66,26 +50,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -103,26 +81,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
@@ -135,26 +107,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -170,26 +136,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-        MatchPlayerJoin,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
-        body (MatchPlayerJoin):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_load_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_load_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,27 @@
 from ...models.match import Match
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
         "url": f"/api/matches/{id}/load/",
     }
 
-    if isinstance(body, Match):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Match):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Match):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
@@ -65,26 +50,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -102,26 +81,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
@@ -134,26 +107,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -169,26 +136,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_pick_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_pick_create.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,42 +9,27 @@
 from ...models.match_pick_map_result import MatchPickMapResult
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        MatchPickMap,
-        MatchPickMap,
-        MatchPickMap,
-    ],
+    body: MatchPickMap,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
         "url": f"/api/matches/{id}/pick/",
     }
 
-    if isinstance(body, MatchPickMap):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, MatchPickMap):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, MatchPickMap):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
@@ -70,26 +55,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPickMap,
-        MatchPickMap,
-        MatchPickMap,
-    ],
+    body: MatchPickMap,
 ) -> Response[MatchPickMapResult]:
     """
     Args:
         id (int):
         body (MatchPickMap):
-        body (MatchPickMap):
-        body (MatchPickMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[MatchPickMapResult]
@@ -107,26 +86,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPickMap,
-        MatchPickMap,
-        MatchPickMap,
-    ],
+    body: MatchPickMap,
 ) -> Optional[MatchPickMapResult]:
     """
     Args:
         id (int):
         body (MatchPickMap):
-        body (MatchPickMap):
-        body (MatchPickMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         MatchPickMapResult
@@ -139,26 +112,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPickMap,
-        MatchPickMap,
-        MatchPickMap,
-    ],
+    body: MatchPickMap,
 ) -> Response[MatchPickMapResult]:
     """
     Args:
         id (int):
         body (MatchPickMap):
-        body (MatchPickMap):
-        body (MatchPickMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[MatchPickMapResult]
@@ -174,26 +141,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        MatchPickMap,
-        MatchPickMap,
-        MatchPickMap,
-    ],
+    body: MatchPickMap,
 ) -> Optional[MatchPickMapResult]:
     """
     Args:
         id (int):
         body (MatchPickMap):
-        body (MatchPickMap):
-        body (MatchPickMap):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         MatchPickMapResult
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_partial_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,48 +2,34 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.match import Match
+from ...models.patched_match import PatchedMatch
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: PatchedMatch,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": f"/api/matches/{id}/recreate/",
+        "method": "patch",
+        "url": f"/api/matches/{id}/",
     }
 
-    if isinstance(body, Match):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Match):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Match):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
@@ -65,26 +51,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: PatchedMatch,
 ) -> Response[Match]:
     """
     Args:
         id (int):
-        body (Match):
-        body (Match):
-        body (Match):
+        body (PatchedMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -102,26 +82,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: PatchedMatch,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
-        body (Match):
-        body (Match):
-        body (Match):
+        body (PatchedMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
@@ -134,26 +108,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: PatchedMatch,
 ) -> Response[Match]:
     """
     Args:
         id (int):
-        body (Match):
-        body (Match):
-        body (Match):
+        body (PatchedMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -169,26 +137,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: PatchedMatch,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
-        body (Match):
-        body (Match):
-        body (Match):
+        body (PatchedMatch):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.match import Match
+from ...models.server import Server
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
+    id: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/matches/{id}/",
+        "url": f"/api/servers/{id}/",
     }
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Server]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Match.from_dict(response.json())
+        response_200 = Server.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Server]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: int,
+    id: str,
     *,
     client: AuthenticatedClient,
-) -> Response[Match]:
+) -> Response[Server]:
     """
     Args:
-        id (int):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Match]
+        Response[Server]
     """
 
     kwargs = _get_kwargs(
         id=id,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: int,
+    id: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[Match]:
+) -> Optional[Server]:
     """
     Args:
-        id (int):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Match
+        Server
     """
 
     return sync_detailed(
         id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: int,
+    id: str,
     *,
     client: AuthenticatedClient,
-) -> Response[Match]:
+) -> Response[Server]:
     """
     Args:
-        id (int):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Match]
+        Response[Server]
     """
 
     kwargs = _get_kwargs(
         id=id,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: int,
+    id: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[Match]:
+) -> Optional[Server]:
     """
     Args:
-        id (int):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Match
+        Server
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
         )
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,42 +8,27 @@
 from ...models.match import Match
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
-        "url": f"/api/matches/{id}/shuffle/",
+        "url": f"/api/matches/{id}/recreate/",
     }
 
-    if isinstance(body, Match):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Match):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Match):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
@@ -65,26 +50,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -102,26 +81,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
@@ -134,26 +107,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -169,26 +136,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,27 @@
 from ...models.match import Match
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
     *,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": f"/api/matches/{id}/",
+        "method": "post",
+        "url": f"/api/matches/{id}/shuffle/",
     }
 
-    if isinstance(body, Match):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Match):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Match):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
     if response.status_code == HTTPStatus.OK:
@@ -65,26 +50,20 @@
     )
 
 
 def sync_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -102,26 +81,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
@@ -134,26 +107,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Response[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Match]
@@ -169,26 +136,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: int,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: Match,
 ) -> Optional[Match]:
     """
     Args:
         id (int):
         body (Match):
-        body (Match):
-        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Match
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,190 +1,165 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.match import Match
+from ...models.patched_steam_user import PatchedSteamUser
+from ...models.steam_user import SteamUser
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
+    body: PatchedSteamUser,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/matches/webhook/",
+        "method": "patch",
+        "url": f"/api/steam-users/{id}/",
     }
 
-    if isinstance(body, Match):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Match):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Match):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[SteamUser]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Match.from_dict(response.json())
+        response_200 = SteamUser.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[SteamUser]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
-) -> Response[Match]:
+    body: PatchedSteamUser,
+) -> Response[SteamUser]:
     """
     Args:
-        body (Match):
-        body (Match):
-        body (Match):
+        id (str):
+        body (PatchedSteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Match]
+        Response[SteamUser]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
-) -> Optional[Match]:
+    body: PatchedSteamUser,
+) -> Optional[SteamUser]:
     """
     Args:
-        body (Match):
-        body (Match):
-        body (Match):
+        id (str):
+        body (PatchedSteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Match
+        SteamUser
     """
 
     return sync_detailed(
+        id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
-) -> Response[Match]:
+    body: PatchedSteamUser,
+) -> Response[SteamUser]:
     """
     Args:
-        body (Match):
-        body (Match):
-        body (Match):
+        id (str):
+        body (PatchedSteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Match]
+        Response[SteamUser]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Match,
-        Match,
-        Match,
-    ],
-) -> Optional[Match]:
+    body: PatchedSteamUser,
+) -> Optional[SteamUser]:
     """
     Args:
-        body (Match):
-        body (Match):
-        body (Match):
+        id (str):
+        body (PatchedSteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Match
+        SteamUser
     """
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_partial_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,45 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
+from ...models.patched_player import PatchedPlayer
 from ...models.player import Player
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: PatchedPlayer,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/players/",
+        "method": "patch",
+        "url": f"/api/players/{id}/",
     }
 
-    if isinstance(body, Player):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Player):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Player):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Player]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = Player.from_dict(response.json())
+    if response.status_code == HTTPStatus.OK:
+        response_200 = Player.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Player]:
@@ -61,130 +48,118 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: PatchedPlayer,
 ) -> Response[Player]:
     """
     Args:
-        body (Player):
-        body (Player):
-        body (Player):
+        id (str):
+        body (PatchedPlayer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Player]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: PatchedPlayer,
 ) -> Optional[Player]:
     """
     Args:
-        body (Player):
-        body (Player):
-        body (Player):
+        id (str):
+        body (PatchedPlayer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Player
     """
 
     return sync_detailed(
+        id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: PatchedPlayer,
 ) -> Response[Player]:
     """
     Args:
-        body (Player):
-        body (Player):
-        body (Player):
+        id (str):
+        body (PatchedPlayer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Player]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: PatchedPlayer,
 ) -> Optional[Player]:
     """
     Args:
-        body (Player):
-        body (Player):
-        body (Player):
+        id (str):
+        body (PatchedPlayer):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Player
     """
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_kwargs(
     id: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "delete",
-        "url": f"/api/players/{id}/",
+        "url": f"/api/servers/{id}/",
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_partial_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_list.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,204 +1,184 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.patched_player import PatchedPlayer
-from ...models.player import Player
-from ...types import Response
+from ...models.paginated_server_list import PaginatedServerList
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    id: str,
     *,
-    body: Union[
-        PatchedPlayer,
-        PatchedPlayer,
-        PatchedPlayer,
-    ],
+    guild: Union[Unset, str] = UNSET,
+    is_public: Union[Unset, bool] = UNSET,
+    page: Union[Unset, int] = UNSET,
 ) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
+    params: Dict[str, Any] = {}
 
-    _kwargs: Dict[str, Any] = {
-        "method": "patch",
-        "url": f"/api/players/{id}/",
-    }
+    params["guild"] = guild
+
+    params["is_public"] = is_public
 
-    if isinstance(body, PatchedPlayer):
-        _json_body = body.to_dict()
+    params["page"] = page
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, PatchedPlayer):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, PatchedPlayer):
-        _files_body = body.to_multipart()
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs: Dict[str, Any] = {
+        "method": "get",
+        "url": "/api/servers/",
+        "params": params,
+    }
 
-    _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Player]:
+def _parse_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Optional[PaginatedServerList]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Player.from_dict(response.json())
+        response_200 = PaginatedServerList.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Player]:
+def _build_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Response[PaginatedServerList]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedPlayer,
-        PatchedPlayer,
-        PatchedPlayer,
-    ],
-) -> Response[Player]:
+    guild: Union[Unset, str] = UNSET,
+    is_public: Union[Unset, bool] = UNSET,
+    page: Union[Unset, int] = UNSET,
+) -> Response[PaginatedServerList]:
     """
     Args:
-        id (str):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
+        guild (Union[Unset, str]):
+        is_public (Union[Unset, bool]):
+        page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Player]
+        Response[PaginatedServerList]
     """
 
     kwargs = _get_kwargs(
-        id=id,
-        body=body,
+        guild=guild,
+        is_public=is_public,
+        page=page,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedPlayer,
-        PatchedPlayer,
-        PatchedPlayer,
-    ],
-) -> Optional[Player]:
+    guild: Union[Unset, str] = UNSET,
+    is_public: Union[Unset, bool] = UNSET,
+    page: Union[Unset, int] = UNSET,
+) -> Optional[PaginatedServerList]:
     """
     Args:
-        id (str):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
+        guild (Union[Unset, str]):
+        is_public (Union[Unset, bool]):
+        page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Player
+        PaginatedServerList
     """
 
     return sync_detailed(
-        id=id,
         client=client,
-        body=body,
+        guild=guild,
+        is_public=is_public,
+        page=page,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedPlayer,
-        PatchedPlayer,
-        PatchedPlayer,
-    ],
-) -> Response[Player]:
+    guild: Union[Unset, str] = UNSET,
+    is_public: Union[Unset, bool] = UNSET,
+    page: Union[Unset, int] = UNSET,
+) -> Response[PaginatedServerList]:
     """
     Args:
-        id (str):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
+        guild (Union[Unset, str]):
+        is_public (Union[Unset, bool]):
+        page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Player]
+        Response[PaginatedServerList]
     """
 
     kwargs = _get_kwargs(
-        id=id,
-        body=body,
+        guild=guild,
+        is_public=is_public,
+        page=page,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedPlayer,
-        PatchedPlayer,
-        PatchedPlayer,
-    ],
-) -> Optional[Player]:
+    guild: Union[Unset, str] = UNSET,
+    is_public: Union[Unset, bool] = UNSET,
+    page: Union[Unset, int] = UNSET,
+) -> Optional[PaginatedServerList]:
     """
     Args:
-        id (str):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
-        body (PatchedPlayer):
+        guild (Union[Unset, str]):
+        is_public (Union[Unset, bool]):
+        page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Player
+        PaginatedServerList
     """
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
-            body=body,
+            guild=guild,
+            is_public=is_public,
+            page=page,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/players/players_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/players/players_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,42 +8,27 @@
 from ...models.player import Player
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
     *,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: Player,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "put",
         "url": f"/api/players/{id}/",
     }
 
-    if isinstance(body, Player):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Player):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Player):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Player]:
     if response.status_code == HTTPStatus.OK:
@@ -65,26 +50,20 @@
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: Player,
 ) -> Response[Player]:
     """
     Args:
         id (str):
         body (Player):
-        body (Player):
-        body (Player):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Player]
@@ -102,26 +81,20 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: Player,
 ) -> Optional[Player]:
     """
     Args:
         id (str):
         body (Player):
-        body (Player):
-        body (Player):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Player
@@ -134,26 +107,20 @@
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: Player,
 ) -> Response[Player]:
     """
     Args:
         id (str):
         body (Player):
-        body (Player):
-        body (Player):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Player]
@@ -169,26 +136,20 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Player,
-        Player,
-        Player,
-    ],
+    body: Player,
 ) -> Optional[Player]:
     """
     Args:
         id (str):
         body (Player):
-        body (Player):
-        body (Player):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Player
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/schema/schema_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/schema/schema_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,42 +7,27 @@
 from ...client import AuthenticatedClient, Client
 from ...models.server import Server
 from ...types import Response
 
 
 def _get_kwargs(
     *,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
+    body: Server,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
         "url": "/api/servers/",
     }
 
-    if isinstance(body, Server):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Server):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Server):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Server]:
     if response.status_code == HTTPStatus.CREATED:
@@ -63,25 +48,19 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
+    body: Server,
 ) -> Response[Server]:
     """
     Args:
         body (Server):
-        body (Server):
-        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Server]
@@ -97,25 +76,19 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
+    body: Server,
 ) -> Optional[Server]:
     """
     Args:
         body (Server):
-        body (Server):
-        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Server
@@ -126,25 +99,19 @@
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
+    body: Server,
 ) -> Response[Server]:
     """
     Args:
         body (Server):
-        body (Server):
-        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Server]
@@ -158,25 +125,19 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
+    body: Server,
 ) -> Optional[Server]:
     """
     Args:
         body (Server):
-        body (Server):
-        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Server
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_kwargs(
     id: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "delete",
-        "url": f"/api/servers/{id}/",
+        "url": f"/api/steam-users/{id}/",
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,184 +1,154 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.paginated_server_list import PaginatedServerList
+from ...models.paginated_team_list import PaginatedTeamList
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    guild: Union[Unset, str] = UNSET,
-    is_public: Union[Unset, bool] = UNSET,
     page: Union[Unset, int] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
-    params["guild"] = guild
-
-    params["is_public"] = is_public
-
     params["page"] = page
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/servers/",
+        "url": "/api/teams/",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[PaginatedServerList]:
+) -> Optional[PaginatedTeamList]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PaginatedServerList.from_dict(response.json())
+        response_200 = PaginatedTeamList.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[PaginatedServerList]:
+) -> Response[PaginatedTeamList]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    guild: Union[Unset, str] = UNSET,
-    is_public: Union[Unset, bool] = UNSET,
     page: Union[Unset, int] = UNSET,
-) -> Response[PaginatedServerList]:
+) -> Response[PaginatedTeamList]:
     """
     Args:
-        guild (Union[Unset, str]):
-        is_public (Union[Unset, bool]):
         page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PaginatedServerList]
+        Response[PaginatedTeamList]
     """
 
     kwargs = _get_kwargs(
-        guild=guild,
-        is_public=is_public,
         page=page,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    guild: Union[Unset, str] = UNSET,
-    is_public: Union[Unset, bool] = UNSET,
     page: Union[Unset, int] = UNSET,
-) -> Optional[PaginatedServerList]:
+) -> Optional[PaginatedTeamList]:
     """
     Args:
-        guild (Union[Unset, str]):
-        is_public (Union[Unset, bool]):
         page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PaginatedServerList
+        PaginatedTeamList
     """
 
     return sync_detailed(
         client=client,
-        guild=guild,
-        is_public=is_public,
         page=page,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    guild: Union[Unset, str] = UNSET,
-    is_public: Union[Unset, bool] = UNSET,
     page: Union[Unset, int] = UNSET,
-) -> Response[PaginatedServerList]:
+) -> Response[PaginatedTeamList]:
     """
     Args:
-        guild (Union[Unset, str]):
-        is_public (Union[Unset, bool]):
         page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PaginatedServerList]
+        Response[PaginatedTeamList]
     """
 
     kwargs = _get_kwargs(
-        guild=guild,
-        is_public=is_public,
         page=page,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    guild: Union[Unset, str] = UNSET,
-    is_public: Union[Unset, bool] = UNSET,
     page: Union[Unset, int] = UNSET,
-) -> Optional[PaginatedServerList]:
+) -> Optional[PaginatedTeamList]:
     """
     Args:
-        guild (Union[Unset, str]):
-        is_public (Union[Unset, bool]):
         page (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PaginatedServerList
+        PaginatedTeamList
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            guild=guild,
-            is_public=is_public,
             page=page,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/servers/servers_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,30 @@
 from ...client import AuthenticatedClient, Client
 from ...models.server import Server
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
+    *,
+    body: Server,
 ) -> Dict[str, Any]:
+    headers: Dict[str, Any] = {}
+
     _kwargs: Dict[str, Any] = {
-        "method": "get",
+        "method": "put",
         "url": f"/api/servers/{id}/",
     }
 
+    _body = body.to_dict()
+
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Server]:
     if response.status_code == HTTPStatus.OK:
         response_200 = Server.from_dict(response.json())
 
@@ -40,103 +50,115 @@
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
+    body: Server,
 ) -> Response[Server]:
     """
     Args:
         id (str):
+        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Server]
     """
 
     kwargs = _get_kwargs(
         id=id,
+        body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
+    body: Server,
 ) -> Optional[Server]:
     """
     Args:
         id (str):
+        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Server
     """
 
     return sync_detailed(
         id=id,
         client=client,
+        body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
+    body: Server,
 ) -> Response[Server]:
     """
     Args:
         id (str):
+        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Server]
     """
 
     kwargs = _get_kwargs(
         id=id,
+        body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
+    body: Server,
 ) -> Optional[Server]:
     """
     Args:
         id (str):
+        body (Server):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Server
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
+            body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/servers/servers_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_partial_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,77 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.server import Server
+from ...models.patched_team import PatchedTeam
+from ...models.team import Team
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
     *,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
+    body: PatchedTeam,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": f"/api/servers/{id}/",
+        "method": "patch",
+        "url": f"/api/teams/{id}/",
     }
 
-    if isinstance(body, Server):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Server):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Server):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Server]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Team]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Server.from_dict(response.json())
+        response_200 = Team.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Server]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Team]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
-) -> Response[Server]:
+    body: PatchedTeam,
+) -> Response[Team]:
     """
     Args:
         id (str):
-        body (Server):
-        body (Server):
-        body (Server):
+        body (PatchedTeam):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Server]
+        Response[Team]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -102,65 +82,53 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
-) -> Optional[Server]:
+    body: PatchedTeam,
+) -> Optional[Team]:
     """
     Args:
         id (str):
-        body (Server):
-        body (Server):
-        body (Server):
+        body (PatchedTeam):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Server
+        Team
     """
 
     return sync_detailed(
         id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
-) -> Response[Server]:
+    body: PatchedTeam,
+) -> Response[Team]:
     """
     Args:
         id (str):
-        body (Server):
-        body (Server):
-        body (Server):
+        body (PatchedTeam):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Server]
+        Response[Team]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -169,33 +137,27 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Server,
-        Server,
-        Server,
-    ],
-) -> Optional[Server]:
+    body: PatchedTeam,
+) -> Optional[Team]:
     """
     Args:
         id (str):
-        body (Server):
-        body (Server):
-        body (Server):
+        body (PatchedTeam):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Server
+        Team
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
             body=body,
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,73 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.steam_user import SteamUser
+from ...models.team import Team
 from ...types import Response
 
 
 def _get_kwargs(
     *,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
+    body: Team,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
-        "url": "/api/steam-users/",
+        "url": "/api/teams/",
     }
 
-    if isinstance(body, SteamUser):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, SteamUser):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, SteamUser):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[SteamUser]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Team]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = SteamUser.from_dict(response.json())
+        response_201 = Team.from_dict(response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[SteamUser]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Team]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Response[SteamUser]:
+    body: Team,
+) -> Response[Team]:
     """
     Args:
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[SteamUser]
+        Response[Team]
     """
 
     kwargs = _get_kwargs(
         body=body,
     )
 
     response = client.get_httpx_client().request(
@@ -97,93 +76,75 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Optional[SteamUser]:
+    body: Team,
+) -> Optional[Team]:
     """
     Args:
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        SteamUser
+        Team
     """
 
     return sync_detailed(
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Response[SteamUser]:
+    body: Team,
+) -> Response[Team]:
     """
     Args:
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[SteamUser]
+        Response[Team]
     """
 
     kwargs = _get_kwargs(
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Optional[SteamUser]:
+    body: Team,
+) -> Optional[Team]:
     """
     Args:
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        SteamUser
+        Team
     """
 
     return (
         await asyncio_detailed(
             client=client,
             body=body,
         )
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
+    guild_id: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "delete",
-        "url": f"/api/steam-users/{id}/",
+        "url": f"/api/guilds/{guild_id}/",
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
@@ -34,58 +34,58 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[Any]:
     """
     Args:
-        id (str):
+        guild_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        id=id,
+        guild_id=guild_id,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[Any]:
     """
     Args:
-        id (str):
+        guild_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        id=id,
+        guild_id=guild_id,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,76 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.steam_user import SteamUser
+from ...models.team import Team
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
     *,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
+    body: Team,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "put",
-        "url": f"/api/steam-users/{id}/",
+        "url": f"/api/teams/{id}/",
     }
 
-    if isinstance(body, SteamUser):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, SteamUser):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, SteamUser):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[SteamUser]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Team]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = SteamUser.from_dict(response.json())
+        response_200 = Team.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[SteamUser]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Team]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Response[SteamUser]:
+    body: Team,
+) -> Response[Team]:
     """
     Args:
         id (str):
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[SteamUser]
+        Response[Team]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -102,65 +81,53 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Optional[SteamUser]:
+    body: Team,
+) -> Optional[Team]:
     """
     Args:
         id (str):
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        SteamUser
+        Team
     """
 
     return sync_detailed(
         id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Response[SteamUser]:
+    body: Team,
+) -> Response[Team]:
     """
     Args:
         id (str):
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[SteamUser]
+        Response[Team]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -169,33 +136,27 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        SteamUser,
-        SteamUser,
-        SteamUser,
-    ],
-) -> Optional[SteamUser]:
+    body: Team,
+) -> Optional[Team]:
     """
     Args:
         id (str):
-        body (SteamUser):
-        body (SteamUser):
-        body (SteamUser):
+        body (Team):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        SteamUser
+        Team
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
             body=body,
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_create.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,73 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.team import Team
+from ...models.match import Match
 from ...types import Response
 
 
 def _get_kwargs(
     *,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
+    body: Match,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
-        "url": "/api/teams/",
+        "url": "/api/matches/webhook/",
     }
 
-    if isinstance(body, Team):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Team):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Team):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Team]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = Team.from_dict(response.json())
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = Match.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Team]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Response[Team]:
+    body: Match,
+) -> Response[Match]:
     """
     Args:
-        body (Team):
-        body (Team):
-        body (Team):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Team]
+        Response[Match]
     """
 
     kwargs = _get_kwargs(
         body=body,
     )
 
     response = client.get_httpx_client().request(
@@ -97,93 +76,75 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Optional[Team]:
+    body: Match,
+) -> Optional[Match]:
     """
     Args:
-        body (Team):
-        body (Team):
-        body (Team):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Team
+        Match
     """
 
     return sync_detailed(
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Response[Team]:
+    body: Match,
+) -> Response[Match]:
     """
     Args:
-        body (Team):
-        body (Team):
-        body (Team):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Team]
+        Response[Match]
     """
 
     kwargs = _get_kwargs(
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Optional[Team]:
+    body: Match,
+) -> Optional[Match]:
     """
     Args:
-        body (Team):
-        body (Team):
-        body (Team):
+        body (Match):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Team
+        Match
     """
 
     return (
         await asyncio_detailed(
             client=client,
             body=body,
         )
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_destroy.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,151 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.paginated_team_list import PaginatedTeamList
-from ...types import UNSET, Response, Unset
+from ...models.steam_user import SteamUser
+from ...types import Response
 
 
 def _get_kwargs(
     *,
-    page: Union[Unset, int] = UNSET,
+    body: SteamUser,
 ) -> Dict[str, Any]:
-    params: Dict[str, Any] = {}
-
-    params["page"] = page
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+    headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "get",
-        "url": "/api/teams/",
-        "params": params,
+        "method": "post",
+        "url": "/api/steam-users/",
     }
 
+    _body = body.to_dict()
+
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[PaginatedTeamList]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = PaginatedTeamList.from_dict(response.json())
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[SteamUser]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = SteamUser.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[PaginatedTeamList]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[SteamUser]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    page: Union[Unset, int] = UNSET,
-) -> Response[PaginatedTeamList]:
+    body: SteamUser,
+) -> Response[SteamUser]:
     """
     Args:
-        page (Union[Unset, int]):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PaginatedTeamList]
+        Response[SteamUser]
     """
 
     kwargs = _get_kwargs(
-        page=page,
+        body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    page: Union[Unset, int] = UNSET,
-) -> Optional[PaginatedTeamList]:
+    body: SteamUser,
+) -> Optional[SteamUser]:
     """
     Args:
-        page (Union[Unset, int]):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PaginatedTeamList
+        SteamUser
     """
 
     return sync_detailed(
         client=client,
-        page=page,
+        body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    page: Union[Unset, int] = UNSET,
-) -> Response[PaginatedTeamList]:
+    body: SteamUser,
+) -> Response[SteamUser]:
     """
     Args:
-        page (Union[Unset, int]):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PaginatedTeamList]
+        Response[SteamUser]
     """
 
     kwargs = _get_kwargs(
-        page=page,
+        body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    page: Union[Unset, int] = UNSET,
-) -> Optional[PaginatedTeamList]:
+    body: SteamUser,
+) -> Optional[SteamUser]:
     """
     Args:
-        page (Union[Unset, int]):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PaginatedTeamList
+        SteamUser
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            page=page,
+            body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_partial_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/guilds/guilds_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,204 +1,164 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.patched_team import PatchedTeam
-from ...models.team import Team
+from ...models.guild import Guild
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
+    guild_id: str,
     *,
-    body: Union[
-        PatchedTeam,
-        PatchedTeam,
-        PatchedTeam,
-    ],
+    body: Guild,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
-        "method": "patch",
-        "url": f"/api/teams/{id}/",
+        "method": "put",
+        "url": f"/api/guilds/{guild_id}/",
     }
 
-    if isinstance(body, PatchedTeam):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, PatchedTeam):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, PatchedTeam):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Team]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Guild]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Team.from_dict(response.json())
+        response_200 = Guild.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Team]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Guild]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedTeam,
-        PatchedTeam,
-        PatchedTeam,
-    ],
-) -> Response[Team]:
+    body: Guild,
+) -> Response[Guild]:
     """
     Args:
-        id (str):
-        body (PatchedTeam):
-        body (PatchedTeam):
-        body (PatchedTeam):
+        guild_id (str):
+        body (Guild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Team]
+        Response[Guild]
     """
 
     kwargs = _get_kwargs(
-        id=id,
+        guild_id=guild_id,
         body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedTeam,
-        PatchedTeam,
-        PatchedTeam,
-    ],
-) -> Optional[Team]:
+    body: Guild,
+) -> Optional[Guild]:
     """
     Args:
-        id (str):
-        body (PatchedTeam):
-        body (PatchedTeam):
-        body (PatchedTeam):
+        guild_id (str):
+        body (Guild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Team
+        Guild
     """
 
     return sync_detailed(
-        id=id,
+        guild_id=guild_id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedTeam,
-        PatchedTeam,
-        PatchedTeam,
-    ],
-) -> Response[Team]:
+    body: Guild,
+) -> Response[Guild]:
     """
     Args:
-        id (str):
-        body (PatchedTeam):
-        body (PatchedTeam):
-        body (PatchedTeam):
+        guild_id (str):
+        body (Guild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Team]
+        Response[Guild]
     """
 
     kwargs = _get_kwargs(
-        id=id,
+        guild_id=guild_id,
         body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
+    guild_id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        PatchedTeam,
-        PatchedTeam,
-        PatchedTeam,
-    ],
-) -> Optional[Team]:
+    body: Guild,
+) -> Optional[Guild]:
     """
     Args:
-        id (str):
-        body (PatchedTeam):
-        body (PatchedTeam):
-        body (PatchedTeam):
+        guild_id (str):
+        body (Guild):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Team
+        Guild
     """
 
     return (
         await asyncio_detailed(
-            id=id,
+            guild_id=guild_id,
             client=client,
             body=body,
         )
     ).parsed
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_retrieve.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/teams/teams_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/api/teams/teams_update.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,76 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.team import Team
+from ...models.steam_user import SteamUser
 from ...types import Response
 
 
 def _get_kwargs(
     id: str,
     *,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
+    body: SteamUser,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "put",
-        "url": f"/api/teams/{id}/",
+        "url": f"/api/steam-users/{id}/",
     }
 
-    if isinstance(body, Team):
-        _json_body = body.to_dict()
+    _body = body.to_dict()
 
-        _kwargs["json"] = _json_body
-        headers["Content-Type"] = "application/json"
-    if isinstance(body, Team):
-        _data_body = body.to_dict()
-
-        _kwargs["data"] = _data_body
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
-    if isinstance(body, Team):
-        _files_body = body.to_multipart()
-
-        _kwargs["files"] = _files_body
-        headers["Content-Type"] = "multipart/form-data"
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Team]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[SteamUser]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Team.from_dict(response.json())
+        response_200 = SteamUser.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Team]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[SteamUser]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Response[Team]:
+    body: SteamUser,
+) -> Response[SteamUser]:
     """
     Args:
         id (str):
-        body (Team):
-        body (Team):
-        body (Team):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Team]
+        Response[SteamUser]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -102,65 +81,53 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Optional[Team]:
+    body: SteamUser,
+) -> Optional[SteamUser]:
     """
     Args:
         id (str):
-        body (Team):
-        body (Team):
-        body (Team):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Team
+        SteamUser
     """
 
     return sync_detailed(
         id=id,
         client=client,
         body=body,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Response[Team]:
+    body: SteamUser,
+) -> Response[SteamUser]:
     """
     Args:
         id (str):
-        body (Team):
-        body (Team):
-        body (Team):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Team]
+        Response[SteamUser]
     """
 
     kwargs = _get_kwargs(
         id=id,
         body=body,
     )
 
@@ -169,33 +136,27 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
     client: AuthenticatedClient,
-    body: Union[
-        Team,
-        Team,
-        Team,
-    ],
-) -> Optional[Team]:
+    body: SteamUser,
+) -> Optional[SteamUser]:
     """
     Args:
         id (str):
-        body (Team):
-        body (Team):
-        body (Team):
+        body (SteamUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Team
+        SteamUser
     """
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
             body=body,
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/client.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/client.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/errors.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/__init__.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .match_config_team_1 import MatchConfigTeam1
 from .match_config_team_2 import MatchConfigTeam2
 from .match_map_selected import MatchMapSelected
 from .match_pick_map import MatchPickMap
 from .match_pick_map_result import MatchPickMapResult
 from .match_player_join import MatchPlayerJoin
 from .match_type_enum import MatchTypeEnum
+from .matches_create_response_400 import MatchesCreateResponse400
 from .nested import Nested
 from .paginated_discord_user_list import PaginatedDiscordUserList
 from .paginated_guild_list import PaginatedGuildList
 from .paginated_map_list import PaginatedMapList
 from .paginated_match_list import PaginatedMatchList
 from .paginated_player_list import PaginatedPlayerList
 from .paginated_server_list import PaginatedServerList
@@ -60,14 +61,15 @@
     "Match",
     "MatchBanMap",
     "MatchBanMapResult",
     "MatchConfig",
     "MatchConfigCvars",
     "MatchConfigTeam1",
     "MatchConfigTeam2",
+    "MatchesCreateResponse400",
     "MatchMapSelected",
     "MatchPickMap",
     "MatchPickMapResult",
     "MatchPlayerJoin",
     "MatchTypeEnum",
     "Nested",
     "PaginatedDiscordUserList",
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_guild.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_guild.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import json
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import Unset
-
 if TYPE_CHECKING:
     from ..models.create_guild_member import CreateGuildMember
 
 
 T = TypeVar("T", bound="CreateGuild")
 
 
@@ -50,53 +47,14 @@
         field_dict.update(
             {
                 "name": name,
                 "guild_id": guild_id,
                 "owner_id": owner_id,
                 "owner_username": owner_username,
                 "members": members,
-            }
-        )
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        guild_id = (
-            self.guild_id if isinstance(self.guild_id, Unset) else (None, str(self.guild_id).encode(), "text/plain")
-        )
-
-        owner_id = (
-            self.owner_id if isinstance(self.owner_id, Unset) else (None, str(self.owner_id).encode(), "text/plain")
-        )
-
-        owner_username = (
-            self.owner_username
-            if isinstance(self.owner_username, Unset)
-            else (None, str(self.owner_username).encode(), "text/plain")
-        )
-
-        _temp_members = []
-        for members_item_data in self.members:
-            members_item = members_item_data.to_dict()
-            _temp_members.append(members_item)
-        members = (None, json.dumps(_temp_members).encode(), "application/json")
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "name": name,
-                "guild_id": guild_id,
-                "owner_id": owner_id,
-                "owner_username": owner_username,
-                "members": members,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_guild_member.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_guild_member.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import Unset
-
 T = TypeVar("T", bound="CreateGuildMember")
 
 
 @_attrs_define
 class CreateGuildMember:
     """
     Attributes:
@@ -30,34 +28,14 @@
         field_dict.update(
             {
                 "user_id": user_id,
                 "username": username,
             }
         )
 
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        user_id = self.user_id if isinstance(self.user_id, Unset) else (None, str(self.user_id).encode(), "text/plain")
-
-        username = (
-            self.username if isinstance(self.username, Unset) else (None, str(self.username).encode(), "text/plain")
-        )
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "user_id": user_id,
-                "username": username,
-            }
-        )
-
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         user_id = d.pop("user_id")
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/create_match_cvars.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/create_match_cvars.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/discord_user.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/player.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,89 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
-from ..types import Unset
+if TYPE_CHECKING:
+    from ..models.nested import Nested
 
-T = TypeVar("T", bound="DiscordUser")
+
+T = TypeVar("T", bound="Player")
 
 
 @_attrs_define
-class DiscordUser:
+class Player:
     """
     Attributes:
         id (str):
-        user_id (str):
-        username (str):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
+        discord_user (Nested):
+        steam_user (Nested):
     """
 
     id: str
-    user_id: str
-    username: str
     created_at: datetime.datetime
     updated_at: datetime.datetime
+    discord_user: "Nested"
+    steam_user: "Nested"
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        user_id = self.user_id
-
-        username = self.username
-
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "user_id": user_id,
-                "username": username,
-                "created_at": created_at,
-                "updated_at": updated_at,
-            }
-        )
-
-        return field_dict
+        discord_user = self.discord_user.to_dict()
 
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        user_id = self.user_id if isinstance(self.user_id, Unset) else (None, str(self.user_id).encode(), "text/plain")
-
-        username = (
-            self.username if isinstance(self.username, Unset) else (None, str(self.username).encode(), "text/plain")
-        )
-
-        created_at = self.created_at.isoformat().encode()
-
-        updated_at = self.updated_at.isoformat().encode()
+        steam_user = self.steam_user.to_dict()
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
+        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
-                "user_id": user_id,
-                "username": username,
                 "created_at": created_at,
                 "updated_at": updated_at,
+                "discord_user": discord_user,
+                "steam_user": steam_user,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.nested import Nested
+
         d = src_dict.copy()
         id = d.pop("id")
 
-        user_id = d.pop("user_id")
-
-        username = d.pop("username")
-
         created_at = isoparse(d.pop("created_at"))
 
         updated_at = isoparse(d.pop("updated_at"))
 
-        discord_user = cls(
+        discord_user = Nested.from_dict(d.pop("discord_user"))
+
+        steam_user = Nested.from_dict(d.pop("steam_user"))
+
+        player = cls(
             id=id,
-            user_id=user_id,
-            username=username,
             created_at=created_at,
             updated_at=updated_at,
+            discord_user=discord_user,
+            steam_user=steam_user,
         )
 
-        discord_user.additional_properties = d
-        return discord_user
+        player.additional_properties = d
+        return player
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/guild.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/guild.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import json
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
@@ -77,74 +76,14 @@
         field_dict.update(
             {
                 "id": id,
                 "name": name,
                 "guild_id": guild_id,
                 "created_at": created_at,
                 "updated_at": updated_at,
-                "owner": owner,
-                "members": members,
-            }
-        )
-        if lobby_channel is not UNSET:
-            field_dict["lobby_channel"] = lobby_channel
-        if team1_channel is not UNSET:
-            field_dict["team1_channel"] = team1_channel
-        if team2_channel is not UNSET:
-            field_dict["team2_channel"] = team2_channel
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        guild_id = (
-            self.guild_id if isinstance(self.guild_id, Unset) else (None, str(self.guild_id).encode(), "text/plain")
-        )
-
-        created_at = self.created_at.isoformat().encode()
-
-        updated_at = self.updated_at.isoformat().encode()
-
-        owner = self.owner if isinstance(self.owner, Unset) else (None, str(self.owner).encode(), "text/plain")
-
-        _temp_members = self.members
-        members = (None, json.dumps(_temp_members).encode(), "application/json")
-
-        lobby_channel: Union[None, Unset, str]
-        if isinstance(self.lobby_channel, Unset):
-            lobby_channel = UNSET
-        else:
-            lobby_channel = self.lobby_channel
-
-        team1_channel: Union[None, Unset, str]
-        if isinstance(self.team1_channel, Unset):
-            team1_channel = UNSET
-        else:
-            team1_channel = self.team1_channel
-
-        team2_channel: Union[None, Unset, str]
-        if isinstance(self.team2_channel, Unset):
-            team2_channel = UNSET
-        else:
-            team2_channel = self.team2_channel
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "id": id,
-                "name": name,
-                "guild_id": guild_id,
-                "created_at": created_at,
-                "updated_at": updated_at,
                 "owner": owner,
                 "members": members,
             }
         )
         if lobby_channel is not UNSET:
             field_dict["lobby_channel"] = lobby_channel
         if team1_channel is not UNSET:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/map_.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_map_selected.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,91 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
-from ..types import Unset
+if TYPE_CHECKING:
+    from ..models.map_ import Map
+    from ..models.team import Team
 
-T = TypeVar("T", bound="Map")
+
+T = TypeVar("T", bound="MatchMapSelected")
 
 
 @_attrs_define
-class Map:
+class MatchMapSelected:
     """
     Attributes:
-        id (str):
-        name (str):
-        tag (str):
+        id (int):
+        team (Team):
+        map_ (Map):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
     """
 
-    id: str
-    name: str
-    tag: str
+    id: int
+    team: "Team"
+    map_: "Map"
     created_at: datetime.datetime
     updated_at: datetime.datetime
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        name = self.name
+        team = self.team.to_dict()
 
-        tag = self.tag
+        map_ = self.map_.to_dict()
 
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
-                "name": name,
-                "tag": tag,
-                "created_at": created_at,
-                "updated_at": updated_at,
-            }
-        )
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        tag = self.tag if isinstance(self.tag, Unset) else (None, str(self.tag).encode(), "text/plain")
-
-        created_at = self.created_at.isoformat().encode()
-
-        updated_at = self.updated_at.isoformat().encode()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "id": id,
-                "name": name,
-                "tag": tag,
+                "team": team,
+                "map": map_,
                 "created_at": created_at,
                 "updated_at": updated_at,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.map_ import Map
+        from ..models.team import Team
+
         d = src_dict.copy()
         id = d.pop("id")
 
-        name = d.pop("name")
+        team = Team.from_dict(d.pop("team"))
 
-        tag = d.pop("tag")
+        map_ = Map.from_dict(d.pop("map"))
 
         created_at = isoparse(d.pop("created_at"))
 
         updated_at = isoparse(d.pop("updated_at"))
 
-        map_ = cls(
+        match_map_selected = cls(
             id=id,
-            name=name,
-            tag=tag,
+            team=team,
+            map_=map_,
             created_at=created_at,
             updated_at=updated_at,
         )
 
-        map_.additional_properties = d
-        return map_
+        match_map_selected.additional_properties = d
+        return match_map_selected
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/map_ban.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/map_ban.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
-import json
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..models.status_enum import StatusEnum
 from ..models.type_enum import TypeEnum
@@ -154,149 +153,14 @@
         field_dict.update(
             {
                 "id": id,
                 "team1": team1,
                 "team2": team2,
                 "winner_team": winner_team,
                 "maps": maps,
-                "map_bans": map_bans,
-                "map_picks": map_picks,
-                "connect_command": connect_command,
-                "load_match_command": load_match_command,
-                "server": server,
-                "guild": guild,
-                "created_at": created_at,
-                "updated_at": updated_at,
-            }
-        )
-        if status is not UNSET:
-            field_dict["status"] = status
-        if type is not UNSET:
-            field_dict["type"] = type
-        if num_maps is not UNSET:
-            field_dict["num_maps"] = num_maps
-        if maplist is not UNSET:
-            field_dict["maplist"] = maplist
-        if map_sides is not UNSET:
-            field_dict["map_sides"] = map_sides
-        if clinch_series is not UNSET:
-            field_dict["clinch_series"] = clinch_series
-        if cvars is not UNSET:
-            field_dict["cvars"] = cvars
-        if players_per_team is not UNSET:
-            field_dict["players_per_team"] = players_per_team
-        if message_id is not UNSET:
-            field_dict["message_id"] = message_id
-        if author is not UNSET:
-            field_dict["author"] = author
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        team1 = (None, json.dumps(self.team1.to_dict()).encode(), "application/json")
-
-        team2 = (None, json.dumps(self.team2.to_dict()).encode(), "application/json")
-
-        winner_team = (None, json.dumps(self.winner_team.to_dict()).encode(), "application/json")
-
-        _temp_maps = []
-        for maps_item_data in self.maps:
-            maps_item = maps_item_data.to_dict()
-            _temp_maps.append(maps_item)
-        maps = (None, json.dumps(_temp_maps).encode(), "application/json")
-
-        _temp_map_bans = []
-        for map_bans_item_data in self.map_bans:
-            map_bans_item = map_bans_item_data.to_dict()
-            _temp_map_bans.append(map_bans_item)
-        map_bans = (None, json.dumps(_temp_map_bans).encode(), "application/json")
-
-        _temp_map_picks = []
-        for map_picks_item_data in self.map_picks:
-            map_picks_item = map_picks_item_data.to_dict()
-            _temp_map_picks.append(map_picks_item)
-        map_picks = (None, json.dumps(_temp_map_picks).encode(), "application/json")
-
-        connect_command = (
-            self.connect_command
-            if isinstance(self.connect_command, Unset)
-            else (None, str(self.connect_command).encode(), "text/plain")
-        )
-
-        load_match_command = (
-            self.load_match_command
-            if isinstance(self.load_match_command, Unset)
-            else (None, str(self.load_match_command).encode(), "text/plain")
-        )
-
-        server = (None, json.dumps(self.server.to_dict()).encode(), "application/json")
-
-        guild = (None, json.dumps(self.guild.to_dict()).encode(), "application/json")
-
-        created_at = self.created_at.isoformat().encode()
-
-        updated_at = self.updated_at.isoformat().encode()
-
-        status: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.status, Unset):
-            status = (None, str(self.status.value).encode(), "text/plain")
-
-        type: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.type, Unset):
-            type = (None, str(self.type.value).encode(), "text/plain")
-
-        num_maps = (
-            self.num_maps if isinstance(self.num_maps, Unset) else (None, str(self.num_maps).encode(), "text/plain")
-        )
-
-        maplist = self.maplist if isinstance(self.maplist, Unset) else (None, str(self.maplist).encode(), "text/plain")
-
-        map_sides = (
-            self.map_sides if isinstance(self.map_sides, Unset) else (None, str(self.map_sides).encode(), "text/plain")
-        )
-
-        clinch_series = (
-            self.clinch_series
-            if isinstance(self.clinch_series, Unset)
-            else (None, str(self.clinch_series).encode(), "text/plain")
-        )
-
-        cvars = self.cvars if isinstance(self.cvars, Unset) else (None, str(self.cvars).encode(), "text/plain")
-
-        players_per_team = (
-            self.players_per_team
-            if isinstance(self.players_per_team, Unset)
-            else (None, str(self.players_per_team).encode(), "text/plain")
-        )
-
-        message_id: Union[None, Unset, str]
-        if isinstance(self.message_id, Unset):
-            message_id = UNSET
-        else:
-            message_id = self.message_id
-
-        author: Union[None, Unset, str]
-        if isinstance(self.author, Unset):
-            author = UNSET
-        else:
-            author = self.author
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "id": id,
-                "team1": team1,
-                "team2": team2,
-                "winner_team": winner_team,
-                "maps": maps,
                 "map_bans": map_bans,
                 "map_picks": map_picks,
                 "connect_command": connect_command,
                 "load_match_command": load_match_command,
                 "server": server,
                 "guild": guild,
                 "created_at": created_at,
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_ban_map.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_ban_map.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import Unset
-
 T = TypeVar("T", bound="MatchBanMap")
 
 
 @_attrs_define
 class MatchBanMap:
     """
     Attributes:
@@ -30,36 +28,14 @@
         field_dict.update(
             {
                 "interaction_user_id": interaction_user_id,
                 "map_tag": map_tag,
             }
         )
 
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        interaction_user_id = (
-            self.interaction_user_id
-            if isinstance(self.interaction_user_id, Unset)
-            else (None, str(self.interaction_user_id).encode(), "text/plain")
-        )
-
-        map_tag = self.map_tag if isinstance(self.map_tag, Unset) else (None, str(self.map_tag).encode(), "text/plain")
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "interaction_user_id": interaction_user_id,
-                "map_tag": map_tag,
-            }
-        )
-
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         interaction_user_id = d.pop("interaction_user_id")
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_ban_map_result.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_ban_map_result.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config_cvars.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config_cvars.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config_team_1.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config_team_1.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_config_team_2.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_config_team_2.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_map_selected.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/map_.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,83 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
-if TYPE_CHECKING:
-    from ..models.map_ import Map
-    from ..models.team import Team
-
-
-T = TypeVar("T", bound="MatchMapSelected")
+T = TypeVar("T", bound="Map")
 
 
 @_attrs_define
-class MatchMapSelected:
+class Map:
     """
     Attributes:
-        id (int):
-        team (Team):
-        map_ (Map):
+        id (str):
+        name (str):
+        tag (str):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
     """
 
-    id: int
-    team: "Team"
-    map_: "Map"
+    id: str
+    name: str
+    tag: str
     created_at: datetime.datetime
     updated_at: datetime.datetime
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        team = self.team.to_dict()
+        name = self.name
 
-        map_ = self.map_.to_dict()
+        tag = self.tag
 
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
-                "team": team,
-                "map": map_,
+                "name": name,
+                "tag": tag,
                 "created_at": created_at,
                 "updated_at": updated_at,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.map_ import Map
-        from ..models.team import Team
-
         d = src_dict.copy()
         id = d.pop("id")
 
-        team = Team.from_dict(d.pop("team"))
+        name = d.pop("name")
 
-        map_ = Map.from_dict(d.pop("map"))
+        tag = d.pop("tag")
 
         created_at = isoparse(d.pop("created_at"))
 
         updated_at = isoparse(d.pop("updated_at"))
 
-        match_map_selected = cls(
+        map_ = cls(
             id=id,
-            team=team,
-            map_=map_,
+            name=name,
+            tag=tag,
             created_at=created_at,
             updated_at=updated_at,
         )
 
-        match_map_selected.additional_properties = d
-        return match_map_selected
+        map_.additional_properties = d
+        return map_
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_pick_map_result.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_pick_map_result.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/match_player_join.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/match_player_join.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import Unset
-
 T = TypeVar("T", bound="MatchPlayerJoin")
 
 
 @_attrs_define
 class MatchPlayerJoin:
     """
     Attributes:
@@ -26,33 +24,14 @@
         field_dict.update(
             {
                 "discord_user_id": discord_user_id,
             }
         )
 
         return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        discord_user_id = (
-            self.discord_user_id
-            if isinstance(self.discord_user_id, Unset)
-            else (None, str(self.discord_user_id).encode(), "text/plain")
-        )
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "discord_user_id": discord_user_id,
-            }
-        )
-
-        return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         discord_user_id = d.pop("discord_user_id")
 
         match_player_join = cls(
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/nested.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/nested.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_discord_user_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_discord_user_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_guild_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_guild_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_map_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_map_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_match_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_match_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_player_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_player_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_server_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_server_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_steam_user_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_steam_user_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/paginated_team_list.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_discord_user.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_team.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,102 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PatchedDiscordUser")
+if TYPE_CHECKING:
+    from ..models.player import Player
+
+
+T = TypeVar("T", bound="PatchedTeam")
 
 
 @_attrs_define
-class PatchedDiscordUser:
+class PatchedTeam:
     """
     Attributes:
         id (Union[Unset, str]):
-        user_id (Union[Unset, str]):
-        username (Union[Unset, str]):
+        players (Union[Unset, List['Player']]):
+        name (Union[Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         updated_at (Union[Unset, datetime.datetime]):
+        leader (Union[None, Unset, str]):
     """
 
     id: Union[Unset, str] = UNSET
-    user_id: Union[Unset, str] = UNSET
-    username: Union[Unset, str] = UNSET
+    players: Union[Unset, List["Player"]] = UNSET
+    name: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
+    leader: Union[None, Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        user_id = self.user_id
+        players: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.players, Unset):
+            players = []
+            for players_item_data in self.players:
+                players_item = players_item_data.to_dict()
+                players.append(players_item)
 
-        username = self.username
+        name = self.name
 
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if user_id is not UNSET:
-            field_dict["user_id"] = user_id
-        if username is not UNSET:
-            field_dict["username"] = username
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        user_id = self.user_id if isinstance(self.user_id, Unset) else (None, str(self.user_id).encode(), "text/plain")
-
-        username = (
-            self.username if isinstance(self.username, Unset) else (None, str(self.username).encode(), "text/plain")
-        )
-
-        created_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat().encode()
-
-        updated_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat().encode()
+        leader: Union[None, Unset, str]
+        if isinstance(self.leader, Unset):
+            leader = UNSET
+        else:
+            leader = self.leader
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
+        field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
-        if user_id is not UNSET:
-            field_dict["user_id"] = user_id
-        if username is not UNSET:
-            field_dict["username"] = username
+        if players is not UNSET:
+            field_dict["players"] = players
+        if name is not UNSET:
+            field_dict["name"] = name
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
+        if leader is not UNSET:
+            field_dict["leader"] = leader
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.player import Player
+
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
-        user_id = d.pop("user_id", UNSET)
+        players = []
+        _players = d.pop("players", UNSET)
+        for players_item_data in _players or []:
+            players_item = Player.from_dict(players_item_data)
 
-        username = d.pop("username", UNSET)
+            players.append(players_item)
+
+        name = d.pop("name", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
@@ -113,24 +104,34 @@
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        patched_discord_user = cls(
+        def _parse_leader(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        leader = _parse_leader(d.pop("leader", UNSET))
+
+        patched_team = cls(
             id=id,
-            user_id=user_id,
-            username=username,
+            players=players,
+            name=name,
             created_at=created_at,
             updated_at=updated_at,
+            leader=leader,
         )
 
-        patched_discord_user.additional_properties = d
-        return patched_discord_user
+        patched_team.additional_properties = d
+        return patched_team
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_guild.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_guild.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
-import json
-from typing import Any, Dict, List, Tuple, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
@@ -83,84 +82,14 @@
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
         if name is not UNSET:
             field_dict["name"] = name
         if guild_id is not UNSET:
             field_dict["guild_id"] = guild_id
-        if lobby_channel is not UNSET:
-            field_dict["lobby_channel"] = lobby_channel
-        if team1_channel is not UNSET:
-            field_dict["team1_channel"] = team1_channel
-        if team2_channel is not UNSET:
-            field_dict["team2_channel"] = team2_channel
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-        if owner is not UNSET:
-            field_dict["owner"] = owner
-        if members is not UNSET:
-            field_dict["members"] = members
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        guild_id = (
-            self.guild_id if isinstance(self.guild_id, Unset) else (None, str(self.guild_id).encode(), "text/plain")
-        )
-
-        lobby_channel: Union[None, Unset, str]
-        if isinstance(self.lobby_channel, Unset):
-            lobby_channel = UNSET
-        else:
-            lobby_channel = self.lobby_channel
-
-        team1_channel: Union[None, Unset, str]
-        if isinstance(self.team1_channel, Unset):
-            team1_channel = UNSET
-        else:
-            team1_channel = self.team1_channel
-
-        team2_channel: Union[None, Unset, str]
-        if isinstance(self.team2_channel, Unset):
-            team2_channel = UNSET
-        else:
-            team2_channel = self.team2_channel
-
-        created_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat().encode()
-
-        updated_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat().encode()
-
-        owner = self.owner if isinstance(self.owner, Unset) else (None, str(self.owner).encode(), "text/plain")
-
-        members: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.members, Unset):
-            _temp_members = self.members
-            members = (None, json.dumps(_temp_members).encode(), "application/json")
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if name is not UNSET:
-            field_dict["name"] = name
-        if guild_id is not UNSET:
-            field_dict["guild_id"] = guild_id
         if lobby_channel is not UNSET:
             field_dict["lobby_channel"] = lobby_channel
         if team1_channel is not UNSET:
             field_dict["team1_channel"] = team1_channel
         if team2_channel is not UNSET:
             field_dict["team2_channel"] = team2_channel
         if created_at is not UNSET:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_map.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_player.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,134 +1,121 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PatchedMap")
+if TYPE_CHECKING:
+    from ..models.nested import Nested
+
+
+T = TypeVar("T", bound="PatchedPlayer")
 
 
 @_attrs_define
-class PatchedMap:
+class PatchedPlayer:
     """
     Attributes:
         id (Union[Unset, str]):
-        name (Union[Unset, str]):
-        tag (Union[Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         updated_at (Union[Unset, datetime.datetime]):
+        discord_user (Union[Unset, Nested]):
+        steam_user (Union[Unset, Nested]):
     """
 
     id: Union[Unset, str] = UNSET
-    name: Union[Unset, str] = UNSET
-    tag: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
+    discord_user: Union[Unset, "Nested"] = UNSET
+    steam_user: Union[Unset, "Nested"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        name = self.name
-
-        tag = self.tag
-
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if name is not UNSET:
-            field_dict["name"] = name
-        if tag is not UNSET:
-            field_dict["tag"] = tag
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        tag = self.tag if isinstance(self.tag, Unset) else (None, str(self.tag).encode(), "text/plain")
-
-        created_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat().encode()
-
-        updated_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat().encode()
+        discord_user: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.discord_user, Unset):
+            discord_user = self.discord_user.to_dict()
+
+        steam_user: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.steam_user, Unset):
+            steam_user = self.steam_user.to_dict()
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
+        field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
-        if name is not UNSET:
-            field_dict["name"] = name
-        if tag is not UNSET:
-            field_dict["tag"] = tag
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
+        if discord_user is not UNSET:
+            field_dict["discord_user"] = discord_user
+        if steam_user is not UNSET:
+            field_dict["steam_user"] = steam_user
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.nested import Nested
+
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
-        name = d.pop("name", UNSET)
-
-        tag = d.pop("tag", UNSET)
-
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        patched_map = cls(
+        _discord_user = d.pop("discord_user", UNSET)
+        discord_user: Union[Unset, Nested]
+        if isinstance(_discord_user, Unset):
+            discord_user = UNSET
+        else:
+            discord_user = Nested.from_dict(_discord_user)
+
+        _steam_user = d.pop("steam_user", UNSET)
+        steam_user: Union[Unset, Nested]
+        if isinstance(_steam_user, Unset):
+            steam_user = UNSET
+        else:
+            steam_user = Nested.from_dict(_steam_user)
+
+        patched_player = cls(
             id=id,
-            name=name,
-            tag=tag,
             created_at=created_at,
             updated_at=updated_at,
+            discord_user=discord_user,
+            steam_user=steam_user,
         )
 
-        patched_map.additional_properties = d
-        return patched_map
+        patched_player.additional_properties = d
+        return patched_player
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_match.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_match.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
-import json
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..models.status_enum import StatusEnum
 from ..models.type_enum import TypeEnum
@@ -174,179 +173,14 @@
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
         if team1 is not UNSET:
             field_dict["team1"] = team1
         if team2 is not UNSET:
             field_dict["team2"] = team2
-        if winner_team is not UNSET:
-            field_dict["winner_team"] = winner_team
-        if maps is not UNSET:
-            field_dict["maps"] = maps
-        if map_bans is not UNSET:
-            field_dict["map_bans"] = map_bans
-        if map_picks is not UNSET:
-            field_dict["map_picks"] = map_picks
-        if connect_command is not UNSET:
-            field_dict["connect_command"] = connect_command
-        if load_match_command is not UNSET:
-            field_dict["load_match_command"] = load_match_command
-        if server is not UNSET:
-            field_dict["server"] = server
-        if guild is not UNSET:
-            field_dict["guild"] = guild
-        if status is not UNSET:
-            field_dict["status"] = status
-        if type is not UNSET:
-            field_dict["type"] = type
-        if num_maps is not UNSET:
-            field_dict["num_maps"] = num_maps
-        if maplist is not UNSET:
-            field_dict["maplist"] = maplist
-        if map_sides is not UNSET:
-            field_dict["map_sides"] = map_sides
-        if clinch_series is not UNSET:
-            field_dict["clinch_series"] = clinch_series
-        if cvars is not UNSET:
-            field_dict["cvars"] = cvars
-        if players_per_team is not UNSET:
-            field_dict["players_per_team"] = players_per_team
-        if message_id is not UNSET:
-            field_dict["message_id"] = message_id
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-        if author is not UNSET:
-            field_dict["author"] = author
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        team1: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.team1, Unset):
-            team1 = (None, json.dumps(self.team1.to_dict()).encode(), "application/json")
-
-        team2: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.team2, Unset):
-            team2 = (None, json.dumps(self.team2.to_dict()).encode(), "application/json")
-
-        winner_team: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.winner_team, Unset):
-            winner_team = (None, json.dumps(self.winner_team.to_dict()).encode(), "application/json")
-
-        maps: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.maps, Unset):
-            _temp_maps = []
-            for maps_item_data in self.maps:
-                maps_item = maps_item_data.to_dict()
-                _temp_maps.append(maps_item)
-            maps = (None, json.dumps(_temp_maps).encode(), "application/json")
-
-        map_bans: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.map_bans, Unset):
-            _temp_map_bans = []
-            for map_bans_item_data in self.map_bans:
-                map_bans_item = map_bans_item_data.to_dict()
-                _temp_map_bans.append(map_bans_item)
-            map_bans = (None, json.dumps(_temp_map_bans).encode(), "application/json")
-
-        map_picks: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.map_picks, Unset):
-            _temp_map_picks = []
-            for map_picks_item_data in self.map_picks:
-                map_picks_item = map_picks_item_data.to_dict()
-                _temp_map_picks.append(map_picks_item)
-            map_picks = (None, json.dumps(_temp_map_picks).encode(), "application/json")
-
-        connect_command = (
-            self.connect_command
-            if isinstance(self.connect_command, Unset)
-            else (None, str(self.connect_command).encode(), "text/plain")
-        )
-
-        load_match_command = (
-            self.load_match_command
-            if isinstance(self.load_match_command, Unset)
-            else (None, str(self.load_match_command).encode(), "text/plain")
-        )
-
-        server: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.server, Unset):
-            server = (None, json.dumps(self.server.to_dict()).encode(), "application/json")
-
-        guild: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.guild, Unset):
-            guild = (None, json.dumps(self.guild.to_dict()).encode(), "application/json")
-
-        status: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.status, Unset):
-            status = (None, str(self.status.value).encode(), "text/plain")
-
-        type: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.type, Unset):
-            type = (None, str(self.type.value).encode(), "text/plain")
-
-        num_maps = (
-            self.num_maps if isinstance(self.num_maps, Unset) else (None, str(self.num_maps).encode(), "text/plain")
-        )
-
-        maplist = self.maplist if isinstance(self.maplist, Unset) else (None, str(self.maplist).encode(), "text/plain")
-
-        map_sides = (
-            self.map_sides if isinstance(self.map_sides, Unset) else (None, str(self.map_sides).encode(), "text/plain")
-        )
-
-        clinch_series = (
-            self.clinch_series
-            if isinstance(self.clinch_series, Unset)
-            else (None, str(self.clinch_series).encode(), "text/plain")
-        )
-
-        cvars = self.cvars if isinstance(self.cvars, Unset) else (None, str(self.cvars).encode(), "text/plain")
-
-        players_per_team = (
-            self.players_per_team
-            if isinstance(self.players_per_team, Unset)
-            else (None, str(self.players_per_team).encode(), "text/plain")
-        )
-
-        message_id: Union[None, Unset, str]
-        if isinstance(self.message_id, Unset):
-            message_id = UNSET
-        else:
-            message_id = self.message_id
-
-        created_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat().encode()
-
-        updated_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat().encode()
-
-        author: Union[None, Unset, str]
-        if isinstance(self.author, Unset):
-            author = UNSET
-        else:
-            author = self.author
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if team1 is not UNSET:
-            field_dict["team1"] = team1
-        if team2 is not UNSET:
-            field_dict["team2"] = team2
         if winner_team is not UNSET:
             field_dict["winner_team"] = winner_team
         if maps is not UNSET:
             field_dict["maps"] = maps
         if map_bans is not UNSET:
             field_dict["map_bans"] = map_bans
         if map_picks is not UNSET:
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_player.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/patched_steam_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,172 @@
 import datetime
-import json
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.nested import Nested
-
-
-T = TypeVar("T", bound="PatchedPlayer")
+T = TypeVar("T", bound="PatchedSteamUser")
 
 
 @_attrs_define
-class PatchedPlayer:
+class PatchedSteamUser:
     """
     Attributes:
         id (Union[Unset, str]):
+        username (Union[Unset, str]):
+        steamid64 (Union[None, Unset, str]):
+        steamid32 (Union[None, Unset, str]):
+        profile_url (Union[None, Unset, str]):
+        avatar (Union[None, Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         updated_at (Union[Unset, datetime.datetime]):
-        discord_user (Union[Unset, Nested]):
-        steam_user (Union[Unset, Nested]):
     """
 
     id: Union[Unset, str] = UNSET
+    username: Union[Unset, str] = UNSET
+    steamid64: Union[None, Unset, str] = UNSET
+    steamid32: Union[None, Unset, str] = UNSET
+    profile_url: Union[None, Unset, str] = UNSET
+    avatar: Union[None, Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    discord_user: Union[Unset, "Nested"] = UNSET
-    steam_user: Union[Unset, "Nested"] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        created_at: Union[Unset, str] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat()
-
-        updated_at: Union[Unset, str] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat()
+        username = self.username
 
-        discord_user: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.discord_user, Unset):
-            discord_user = self.discord_user.to_dict()
-
-        steam_user: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.steam_user, Unset):
-            steam_user = self.steam_user.to_dict()
+        steamid64: Union[None, Unset, str]
+        if isinstance(self.steamid64, Unset):
+            steamid64 = UNSET
+        else:
+            steamid64 = self.steamid64
 
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-        if discord_user is not UNSET:
-            field_dict["discord_user"] = discord_user
-        if steam_user is not UNSET:
-            field_dict["steam_user"] = steam_user
+        steamid32: Union[None, Unset, str]
+        if isinstance(self.steamid32, Unset):
+            steamid32 = UNSET
+        else:
+            steamid32 = self.steamid32
 
-        return field_dict
+        profile_url: Union[None, Unset, str]
+        if isinstance(self.profile_url, Unset):
+            profile_url = UNSET
+        else:
+            profile_url = self.profile_url
 
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
+        avatar: Union[None, Unset, str]
+        if isinstance(self.avatar, Unset):
+            avatar = UNSET
+        else:
+            avatar = self.avatar
 
-        created_at: Union[Unset, bytes] = UNSET
+        created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat().encode()
+            created_at = self.created_at.isoformat()
 
-        updated_at: Union[Unset, bytes] = UNSET
+        updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat().encode()
-
-        discord_user: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.discord_user, Unset):
-            discord_user = (None, json.dumps(self.discord_user.to_dict()).encode(), "application/json")
-
-        steam_user: Union[Unset, Tuple[None, bytes, str]] = UNSET
-        if not isinstance(self.steam_user, Unset):
-            steam_user = (None, json.dumps(self.steam_user.to_dict()).encode(), "application/json")
+            updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
+        field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
+        if username is not UNSET:
+            field_dict["username"] = username
+        if steamid64 is not UNSET:
+            field_dict["steamid64"] = steamid64
+        if steamid32 is not UNSET:
+            field_dict["steamid32"] = steamid32
+        if profile_url is not UNSET:
+            field_dict["profile_url"] = profile_url
+        if avatar is not UNSET:
+            field_dict["avatar"] = avatar
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
-        if discord_user is not UNSET:
-            field_dict["discord_user"] = discord_user
-        if steam_user is not UNSET:
-            field_dict["steam_user"] = steam_user
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.nested import Nested
-
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
+        username = d.pop("username", UNSET)
+
+        def _parse_steamid64(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        steamid64 = _parse_steamid64(d.pop("steamid64", UNSET))
+
+        def _parse_steamid32(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        steamid32 = _parse_steamid32(d.pop("steamid32", UNSET))
+
+        def _parse_profile_url(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        profile_url = _parse_profile_url(d.pop("profile_url", UNSET))
+
+        def _parse_avatar(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        avatar = _parse_avatar(d.pop("avatar", UNSET))
+
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _discord_user = d.pop("discord_user", UNSET)
-        discord_user: Union[Unset, Nested]
-        if isinstance(_discord_user, Unset):
-            discord_user = UNSET
-        else:
-            discord_user = Nested.from_dict(_discord_user)
-
-        _steam_user = d.pop("steam_user", UNSET)
-        steam_user: Union[Unset, Nested]
-        if isinstance(_steam_user, Unset):
-            steam_user = UNSET
-        else:
-            steam_user = Nested.from_dict(_steam_user)
-
-        patched_player = cls(
+        patched_steam_user = cls(
             id=id,
+            username=username,
+            steamid64=steamid64,
+            steamid32=steamid32,
+            profile_url=profile_url,
+            avatar=avatar,
             created_at=created_at,
             updated_at=updated_at,
-            discord_user=discord_user,
-            steam_user=steam_user,
         )
 
-        patched_player.additional_properties = d
-        return patched_player
+        patched_steam_user.additional_properties = d
+        return patched_steam_user
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/patched_steam_user.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/steam_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,106 +3,49 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PatchedSteamUser")
+T = TypeVar("T", bound="SteamUser")
 
 
 @_attrs_define
-class PatchedSteamUser:
+class SteamUser:
     """
     Attributes:
-        id (Union[Unset, str]):
-        username (Union[Unset, str]):
+        id (str):
+        username (str):
+        created_at (datetime.datetime):
+        updated_at (datetime.datetime):
         steamid64 (Union[None, Unset, str]):
         steamid32 (Union[None, Unset, str]):
         profile_url (Union[None, Unset, str]):
         avatar (Union[None, Unset, str]):
-        created_at (Union[Unset, datetime.datetime]):
-        updated_at (Union[Unset, datetime.datetime]):
     """
 
-    id: Union[Unset, str] = UNSET
-    username: Union[Unset, str] = UNSET
+    id: str
+    username: str
+    created_at: datetime.datetime
+    updated_at: datetime.datetime
     steamid64: Union[None, Unset, str] = UNSET
     steamid32: Union[None, Unset, str] = UNSET
     profile_url: Union[None, Unset, str] = UNSET
     avatar: Union[None, Unset, str] = UNSET
-    created_at: Union[Unset, datetime.datetime] = UNSET
-    updated_at: Union[Unset, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         username = self.username
 
-        steamid64: Union[None, Unset, str]
-        if isinstance(self.steamid64, Unset):
-            steamid64 = UNSET
-        else:
-            steamid64 = self.steamid64
-
-        steamid32: Union[None, Unset, str]
-        if isinstance(self.steamid32, Unset):
-            steamid32 = UNSET
-        else:
-            steamid32 = self.steamid32
-
-        profile_url: Union[None, Unset, str]
-        if isinstance(self.profile_url, Unset):
-            profile_url = UNSET
-        else:
-            profile_url = self.profile_url
+        created_at = self.created_at.isoformat()
 
-        avatar: Union[None, Unset, str]
-        if isinstance(self.avatar, Unset):
-            avatar = UNSET
-        else:
-            avatar = self.avatar
-
-        created_at: Union[Unset, str] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat()
-
-        updated_at: Union[Unset, str] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if username is not UNSET:
-            field_dict["username"] = username
-        if steamid64 is not UNSET:
-            field_dict["steamid64"] = steamid64
-        if steamid32 is not UNSET:
-            field_dict["steamid32"] = steamid32
-        if profile_url is not UNSET:
-            field_dict["profile_url"] = profile_url
-        if avatar is not UNSET:
-            field_dict["avatar"] = avatar
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        username = (
-            self.username if isinstance(self.username, Unset) else (None, str(self.username).encode(), "text/plain")
-        )
+        updated_at = self.updated_at.isoformat()
 
         steamid64: Union[None, Unset, str]
         if isinstance(self.steamid64, Unset):
             steamid64 = UNSET
         else:
             steamid64 = self.steamid64
 
@@ -120,52 +63,45 @@
 
         avatar: Union[None, Unset, str]
         if isinstance(self.avatar, Unset):
             avatar = UNSET
         else:
             avatar = self.avatar
 
-        created_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.created_at, Unset):
-            created_at = self.created_at.isoformat().encode()
-
-        updated_at: Union[Unset, bytes] = UNSET
-        if not isinstance(self.updated_at, Unset):
-            updated_at = self.updated_at.isoformat().encode()
-
         field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
         field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+            {
+                "id": id,
+                "username": username,
+                "created_at": created_at,
+                "updated_at": updated_at,
+            }
         )
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if username is not UNSET:
-            field_dict["username"] = username
         if steamid64 is not UNSET:
             field_dict["steamid64"] = steamid64
         if steamid32 is not UNSET:
             field_dict["steamid32"] = steamid32
         if profile_url is not UNSET:
             field_dict["profile_url"] = profile_url
         if avatar is not UNSET:
             field_dict["avatar"] = avatar
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = d.pop("id")
+
+        username = d.pop("username")
 
-        username = d.pop("username", UNSET)
+        created_at = isoparse(d.pop("created_at"))
+
+        updated_at = isoparse(d.pop("updated_at"))
 
         def _parse_steamid64(data: object) -> Union[None, Unset, str]:
             if data is None:
                 return data
             if isinstance(data, Unset):
                 return data
             return cast(Union[None, Unset, str], data)
@@ -195,41 +131,27 @@
                 return data
             if isinstance(data, Unset):
                 return data
             return cast(Union[None, Unset, str], data)
 
         avatar = _parse_avatar(d.pop("avatar", UNSET))
 
-        _created_at = d.pop("created_at", UNSET)
-        created_at: Union[Unset, datetime.datetime]
-        if isinstance(_created_at, Unset):
-            created_at = UNSET
-        else:
-            created_at = isoparse(_created_at)
-
-        _updated_at = d.pop("updated_at", UNSET)
-        updated_at: Union[Unset, datetime.datetime]
-        if isinstance(_updated_at, Unset):
-            updated_at = UNSET
-        else:
-            updated_at = isoparse(_updated_at)
-
-        patched_steam_user = cls(
+        steam_user = cls(
             id=id,
             username=username,
+            created_at=created_at,
+            updated_at=updated_at,
             steamid64=steamid64,
             steamid32=steamid32,
             profile_url=profile_url,
             avatar=avatar,
-            created_at=created_at,
-            updated_at=updated_at,
         )
 
-        patched_steam_user.additional_properties = d
-        return patched_steam_user
+        steam_user.additional_properties = d
+        return steam_user
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/schema_retrieve_lang.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/schema_retrieve_lang.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/server.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -74,68 +74,14 @@
         if rcon_password is not UNSET:
             field_dict["rcon_password"] = rcon_password
         if guild is not UNSET:
             field_dict["guild"] = guild
 
         return field_dict
 
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        ip = self.ip if isinstance(self.ip, Unset) else (None, str(self.ip).encode(), "text/plain")
-
-        port = self.port if isinstance(self.port, Unset) else (None, str(self.port).encode(), "text/plain")
-
-        password: Union[None, Unset, str]
-        if isinstance(self.password, Unset):
-            password = UNSET
-        else:
-            password = self.password
-
-        is_public = (
-            self.is_public if isinstance(self.is_public, Unset) else (None, str(self.is_public).encode(), "text/plain")
-        )
-
-        rcon_password = (
-            self.rcon_password
-            if isinstance(self.rcon_password, Unset)
-            else (None, str(self.rcon_password).encode(), "text/plain")
-        )
-
-        guild: Union[None, Unset, str]
-        if isinstance(self.guild, Unset):
-            guild = UNSET
-        else:
-            guild = self.guild
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "id": id,
-                "name": name,
-                "ip": ip,
-                "port": port,
-            }
-        )
-        if password is not UNSET:
-            field_dict["password"] = password
-        if is_public is not UNSET:
-            field_dict["is_public"] = is_public
-        if rcon_password is not UNSET:
-            field_dict["rcon_password"] = rcon_password
-        if guild is not UNSET:
-            field_dict["guild"] = guild
-
-        return field_dict
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         name = d.pop("name")
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/models/team.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/models/team.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import json
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
@@ -60,53 +59,14 @@
         field_dict.update(
             {
                 "id": id,
                 "players": players,
                 "name": name,
                 "created_at": created_at,
                 "updated_at": updated_at,
-            }
-        )
-        if leader is not UNSET:
-            field_dict["leader"] = leader
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
-
-        _temp_players = []
-        for players_item_data in self.players:
-            players_item = players_item_data.to_dict()
-            _temp_players.append(players_item)
-        players = (None, json.dumps(_temp_players).encode(), "application/json")
-
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-
-        created_at = self.created_at.isoformat().encode()
-
-        updated_at = self.updated_at.isoformat().encode()
-
-        leader: Union[None, Unset, str]
-        if isinstance(self.leader, Unset):
-            leader = UNSET
-        else:
-            leader = self.leader
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "id": id,
-                "players": players,
-                "name": name,
-                "created_at": created_at,
-                "updated_at": updated_at,
             }
         )
         if leader is not UNSET:
             field_dict["leader"] = leader
 
         return field_dict
```

### Comparing `cs2_battle_bot_api_client-0.0.6/cs2_battle_bot_api_client/types.py` & `cs2_battle_bot_api_client-0.0.7/cs2_battle_bot_api_client/types.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.6/pyproject.toml` & `cs2_battle_bot_api_client-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cs2-battle-bot-api-client"
-version = "0.0.6"
+version = "0.0.7"
 description = "A client library for accessing cs2-battle-bot-api"
 authors = []
 readme = "README.md"
 packages = [
     {include = "cs2_battle_bot_api_client"},
 ]
 include = ["CHANGELOG.md", "cs2_battle_bot_api_client/py.typed"]
```

### Comparing `cs2_battle_bot_api_client-0.0.6/PKG-INFO` & `cs2_battle_bot_api_client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2-battle-bot-api-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A client library for accessing cs2-battle-bot-api
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

