# Comparing `tmp/guilded.py-1.9.0.tar.gz` & `tmp/guilded.py-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\shay\Documents\GitHub\guilded.py\dist\.tmp-cmatgno6\guilded.py-1.9.0.tar", last modified: Thu Jun  1 16:32:28 2023, max compression
+gzip compressed data, was "C:\Users\shay\Documents\GitHub\guilded.py\dist\.tmp-4c8zvw14\guilded.py-1.9.1.tar", last modified: Wed Jun 14 19:12:50 2023, max compression
```

## Comparing `guilded.py-1.9.0.tar` & `guilded.py-1.9.1.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.777519 guilded.py-1.9.0/
--rw-rw-rw-   0        0        0     2402 2021-08-25 00:53:36.000000 guilded.py-1.9.0/LICENSE
--rw-rw-rw-   0        0        0     2101 2023-06-01 16:32:28.776520 guilded.py-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2022-12-18 15:12:28.000000 guilded.py-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.723568 guilded.py-1.9.0/guilded/
--rw-rw-rw-   0        0        0      785 2023-06-01 16:31:47.000000 guilded.py-1.9.0/guilded/__init__.py
--rw-rw-rw-   0        0        0    26852 2023-05-29 23:37:49.000000 guilded.py-1.9.0/guilded/abc.py
--rw-rw-rw-   0        0        0    20033 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/asset.py
--rw-rw-rw-   0        0        0     3254 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/backoff.py
--rw-rw-rw-   0        0        0   126137 2023-05-29 23:17:33.000000 guilded.py-1.9.0/guilded/channel.py
--rw-rw-rw-   0        0        0    32508 2023-05-16 23:19:50.000000 guilded.py-1.9.0/guilded/client.py
--rw-rw-rw-   0        0        0    12981 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/colour.py
--rw-rw-rw-   0        0        0    19980 2023-04-05 23:14:18.000000 guilded.py-1.9.0/guilded/embed.py
--rw-rw-rw-   0        0        0     9002 2023-01-20 17:23:19.000000 guilded.py-1.9.0/guilded/emote.py
--rw-rw-rw-   0        0        0    13931 2023-06-01 14:41:55.000000 guilded.py-1.9.0/guilded/enums.py
--rw-rw-rw-   0        0        0     4836 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/errors.py
--rw-rw-rw-   0        0        0    95325 2023-05-30 22:32:00.000000 guilded.py-1.9.0/guilded/events.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.674569 guilded.py-1.9.0/guilded/ext/
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.751520 guilded.py-1.9.0/guilded/ext/commands/
--rw-rw-rw-   0        0        0      199 2022-10-16 15:08:32.000000 guilded.py-1.9.0/guilded/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     1938 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/_types.py
--rw-rw-rw-   0        0        0    35283 2023-05-29 23:31:15.000000 guilded.py-1.9.0/guilded/ext/commands/bot.py
--rw-rw-rw-   0        0        0    18115 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/cog.py
--rw-rw-rw-   0        0        0     6658 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/context.py
--rw-rw-rw-   0        0        0    35367 2023-05-29 21:04:13.000000 guilded.py-1.9.0/guilded/ext/commands/converters.py
--rw-rw-rw-   0        0        0    15030 2022-10-16 15:09:19.000000 guilded.py-1.9.0/guilded/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    67778 2023-06-01 16:22:16.000000 guilded.py-1.9.0/guilded/ext/commands/core.py
--rw-rw-rw-   0        0        0    30211 2022-10-16 17:27:04.000000 guilded.py-1.9.0/guilded/ext/commands/errors.py
--rw-rw-rw-   0        0        0    50177 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/help.py
--rw-rw-rw-   0        0        0     7466 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.752520 guilded.py-1.9.0/guilded/ext/tasks/
--rw-rw-rw-   0        0        0    18800 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0    13190 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/file.py
--rw-rw-rw-   0        0        0     5232 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/flowbot.py
--rw-rw-rw-   0        0        0    61856 2023-05-25 18:32:35.000000 guilded.py-1.9.0/guilded/gateway.py
--rw-rw-rw-   0        0        0     9890 2023-05-09 23:29:24.000000 guilded.py-1.9.0/guilded/group.py
--rw-rw-rw-   0        0        0    49648 2023-06-01 14:40:24.000000 guilded.py-1.9.0/guilded/http.py
--rw-rw-rw-   0        0        0     3803 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/invite.py
--rw-rw-rw-   0        0        0    39544 2023-05-30 20:25:35.000000 guilded.py-1.9.0/guilded/message.py
--rw-rw-rw-   0        0        0     2873 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/mixins.py
--rw-rw-rw-   0        0        0    62638 2023-06-01 15:35:20.000000 guilded.py-1.9.0/guilded/permissions.py
--rw-rw-rw-   0        0        0     3224 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/presence.py
--rw-rw-rw-   0        0        0    10648 2022-11-21 13:58:08.000000 guilded.py-1.9.0/guilded/reaction.py
--rw-rw-rw-   0        0        0    16453 2023-04-30 21:56:02.000000 guilded.py-1.9.0/guilded/reply.py
--rw-rw-rw-   0        0        0    12620 2023-05-25 03:57:30.000000 guilded.py-1.9.0/guilded/role.py
--rw-rw-rw-   0        0        0    50093 2023-06-01 15:09:46.000000 guilded.py-1.9.0/guilded/server.py
--rw-rw-rw-   0        0        0     3200 2023-05-19 03:57:55.000000 guilded.py-1.9.0/guilded/status.py
--rw-rw-rw-   0        0        0     3597 2023-06-01 03:01:11.000000 guilded.py-1.9.0/guilded/subscription.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.772520 guilded.py-1.9.0/guilded/types/
--rw-rw-rw-   0        0        0     1600 2023-04-17 22:54:44.000000 guilded.py-1.9.0/guilded/types/announcement.py
--rw-rw-rw-   0        0        0     3011 2023-03-25 15:03:09.000000 guilded.py-1.9.0/guilded/types/calendar_event.py
--rw-rw-rw-   0        0        0     2100 2023-05-23 16:20:34.000000 guilded.py-1.9.0/guilded/types/channel.py
--rw-rw-rw-   0        0        0      225 2023-01-23 20:13:53.000000 guilded.py-1.9.0/guilded/types/comment.py
--rw-rw-rw-   0        0        0     1639 2023-02-09 20:44:26.000000 guilded.py-1.9.0/guilded/types/doc.py
--rw-rw-rw-   0        0        0     1995 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/types/embed.py
--rw-rw-rw-   0        0        0     1324 2023-01-20 17:10:42.000000 guilded.py-1.9.0/guilded/types/emote.py
--rw-rw-rw-   0        0        0     1774 2023-02-02 18:56:59.000000 guilded.py-1.9.0/guilded/types/forum_topic.py
--rw-rw-rw-   0        0        0     6220 2023-05-30 22:32:53.000000 guilded.py-1.9.0/guilded/types/gateway.py
--rw-rw-rw-   0        0        0     1631 2023-05-09 01:29:48.000000 guilded.py-1.9.0/guilded/types/group.py
--rw-rw-rw-   0        0        0     2027 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/types/list_item.py
--rw-rw-rw-   0        0        0     1958 2023-04-30 22:01:12.000000 guilded.py-1.9.0/guilded/types/message.py
--rw-rw-rw-   0        0        0     2050 2023-04-17 22:55:33.000000 guilded.py-1.9.0/guilded/types/reaction.py
--rw-rw-rw-   0        0        0     1622 2023-05-18 21:03:59.000000 guilded.py-1.9.0/guilded/types/role.py
--rw-rw-rw-   0        0        0     1689 2022-10-27 15:22:52.000000 guilded.py-1.9.0/guilded/types/server.py
--rw-rw-rw-   0        0        0     1508 2023-02-28 00:17:19.000000 guilded.py-1.9.0/guilded/types/social_link.py
--rw-rw-rw-   0        0        0     1442 2023-06-01 03:01:41.000000 guilded.py-1.9.0/guilded/types/subscription.py
--rw-rw-rw-   0        0        0     2724 2023-05-19 03:27:49.000000 guilded.py-1.9.0/guilded/types/user.py
--rw-rw-rw-   0        0        0     3029 2023-02-02 16:43:38.000000 guilded.py-1.9.0/guilded/types/webhook.py
--rw-rw-rw-   0        0        0    24280 2023-06-01 15:32:28.000000 guilded.py-1.9.0/guilded/user.py
--rw-rw-rw-   0        0        0    13639 2022-12-16 17:30:53.000000 guilded.py-1.9.0/guilded/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.775521 guilded.py-1.9.0/guilded/webhook/
--rw-rw-rw-   0        0        0       23 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/webhook/__init__.py
--rw-rw-rw-   0        0        0    37555 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/webhook/async_.py
--rw-rw-rw-   0        0        0        0 2022-08-13 03:46:11.000000 guilded.py-1.9.0/guilded/webhook/sync.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.739567 guilded.py-1.9.0/guilded.py.egg-info/
--rw-rw-rw-   0        0        0     2101 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 16:32:28.777519 guilded.py-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1608 2022-09-23 00:42:16.000000 guilded.py-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.670994 guilded.py-1.9.1/
+-rw-rw-rw-   0        0        0     2402 2021-08-25 00:53:36.000000 guilded.py-1.9.1/LICENSE
+-rw-rw-rw-   0        0        0     2101 2023-06-14 19:12:50.669994 guilded.py-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2022-12-18 15:12:28.000000 guilded.py-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.605994 guilded.py-1.9.1/guilded/
+-rw-rw-rw-   0        0        0      785 2023-06-14 19:08:06.000000 guilded.py-1.9.1/guilded/__init__.py
+-rw-rw-rw-   0        0        0    26907 2023-06-10 18:02:55.000000 guilded.py-1.9.1/guilded/abc.py
+-rw-rw-rw-   0        0        0    20033 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/asset.py
+-rw-rw-rw-   0        0        0     3254 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/backoff.py
+-rw-rw-rw-   0        0        0   126137 2023-05-29 23:17:33.000000 guilded.py-1.9.1/guilded/channel.py
+-rw-rw-rw-   0        0        0    32508 2023-05-16 23:19:50.000000 guilded.py-1.9.1/guilded/client.py
+-rw-rw-rw-   0        0        0    12981 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/colour.py
+-rw-rw-rw-   0        0        0    19980 2023-04-05 23:14:18.000000 guilded.py-1.9.1/guilded/embed.py
+-rw-rw-rw-   0        0        0     9002 2023-01-20 17:23:19.000000 guilded.py-1.9.1/guilded/emote.py
+-rw-rw-rw-   0        0        0    13931 2023-06-01 14:41:55.000000 guilded.py-1.9.1/guilded/enums.py
+-rw-rw-rw-   0        0        0     6646 2023-06-14 19:08:18.000000 guilded.py-1.9.1/guilded/errors.py
+-rw-rw-rw-   0        0        0    95325 2023-05-30 22:32:00.000000 guilded.py-1.9.1/guilded/events.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.548053 guilded.py-1.9.1/guilded/ext/
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.636994 guilded.py-1.9.1/guilded/ext/commands/
+-rw-rw-rw-   0        0        0      199 2022-10-16 15:08:32.000000 guilded.py-1.9.1/guilded/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1938 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    35283 2023-05-29 23:31:15.000000 guilded.py-1.9.1/guilded/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    18115 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/ext/commands/cog.py
+-rw-rw-rw-   0        0        0     6658 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/ext/commands/context.py
+-rw-rw-rw-   0        0        0    35367 2023-05-29 21:04:13.000000 guilded.py-1.9.1/guilded/ext/commands/converters.py
+-rw-rw-rw-   0        0        0    15030 2022-10-16 15:09:19.000000 guilded.py-1.9.1/guilded/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    67778 2023-06-01 16:22:16.000000 guilded.py-1.9.1/guilded/ext/commands/core.py
+-rw-rw-rw-   0        0        0    30211 2022-10-16 17:27:04.000000 guilded.py-1.9.1/guilded/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    50177 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/ext/commands/help.py
+-rw-rw-rw-   0        0        0     7466 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.637994 guilded.py-1.9.1/guilded/ext/tasks/
+-rw-rw-rw-   0        0        0    18800 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0    13190 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/file.py
+-rw-rw-rw-   0        0        0     5232 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/flowbot.py
+-rw-rw-rw-   0        0        0    61818 2023-06-11 13:29:00.000000 guilded.py-1.9.1/guilded/gateway.py
+-rw-rw-rw-   0        0        0     9890 2023-05-09 23:29:24.000000 guilded.py-1.9.1/guilded/group.py
+-rw-rw-rw-   0        0        0    50403 2023-06-09 16:11:59.000000 guilded.py-1.9.1/guilded/http.py
+-rw-rw-rw-   0        0        0     3803 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/invite.py
+-rw-rw-rw-   0        0        0    39544 2023-05-30 20:25:35.000000 guilded.py-1.9.1/guilded/message.py
+-rw-rw-rw-   0        0        0     2873 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/mixins.py
+-rw-rw-rw-   0        0        0    62638 2023-06-01 15:35:20.000000 guilded.py-1.9.1/guilded/permissions.py
+-rw-rw-rw-   0        0        0     3224 2022-10-15 20:18:59.000000 guilded.py-1.9.1/guilded/presence.py
+-rw-rw-rw-   0        0        0    10648 2022-11-21 13:58:08.000000 guilded.py-1.9.1/guilded/reaction.py
+-rw-rw-rw-   0        0        0    16453 2023-04-30 21:56:02.000000 guilded.py-1.9.1/guilded/reply.py
+-rw-rw-rw-   0        0        0    13369 2023-06-01 19:48:23.000000 guilded.py-1.9.1/guilded/role.py
+-rw-rw-rw-   0        0        0    50093 2023-06-01 15:09:46.000000 guilded.py-1.9.1/guilded/server.py
+-rw-rw-rw-   0        0        0     3200 2023-05-19 03:57:55.000000 guilded.py-1.9.1/guilded/status.py
+-rw-rw-rw-   0        0        0     3597 2023-06-01 03:01:11.000000 guilded.py-1.9.1/guilded/subscription.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.664996 guilded.py-1.9.1/guilded/types/
+-rw-rw-rw-   0        0        0     1600 2023-04-17 22:54:44.000000 guilded.py-1.9.1/guilded/types/announcement.py
+-rw-rw-rw-   0        0        0     3011 2023-03-25 15:03:09.000000 guilded.py-1.9.1/guilded/types/calendar_event.py
+-rw-rw-rw-   0        0        0     2100 2023-05-23 16:20:34.000000 guilded.py-1.9.1/guilded/types/channel.py
+-rw-rw-rw-   0        0        0      225 2023-01-23 20:13:53.000000 guilded.py-1.9.1/guilded/types/comment.py
+-rw-rw-rw-   0        0        0     1639 2023-02-09 20:44:26.000000 guilded.py-1.9.1/guilded/types/doc.py
+-rw-rw-rw-   0        0        0     1995 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/types/embed.py
+-rw-rw-rw-   0        0        0     1324 2023-01-20 17:10:42.000000 guilded.py-1.9.1/guilded/types/emote.py
+-rw-rw-rw-   0        0        0     1774 2023-02-02 18:56:59.000000 guilded.py-1.9.1/guilded/types/forum_topic.py
+-rw-rw-rw-   0        0        0     6220 2023-05-30 22:32:53.000000 guilded.py-1.9.1/guilded/types/gateway.py
+-rw-rw-rw-   0        0        0     1631 2023-05-09 01:29:48.000000 guilded.py-1.9.1/guilded/types/group.py
+-rw-rw-rw-   0        0        0     1416 2023-06-09 16:24:03.000000 guilded.py-1.9.1/guilded/types/http.py
+-rw-rw-rw-   0        0        0     2027 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/types/list_item.py
+-rw-rw-rw-   0        0        0     1958 2023-04-30 22:01:12.000000 guilded.py-1.9.1/guilded/types/message.py
+-rw-rw-rw-   0        0        0     2050 2023-04-17 22:55:33.000000 guilded.py-1.9.1/guilded/types/reaction.py
+-rw-rw-rw-   0        0        0     1655 2023-06-01 19:45:15.000000 guilded.py-1.9.1/guilded/types/role.py
+-rw-rw-rw-   0        0        0     1689 2022-10-27 15:22:52.000000 guilded.py-1.9.1/guilded/types/server.py
+-rw-rw-rw-   0        0        0     1508 2023-02-28 00:17:19.000000 guilded.py-1.9.1/guilded/types/social_link.py
+-rw-rw-rw-   0        0        0     1442 2023-06-01 03:01:41.000000 guilded.py-1.9.1/guilded/types/subscription.py
+-rw-rw-rw-   0        0        0     2724 2023-05-19 03:27:49.000000 guilded.py-1.9.1/guilded/types/user.py
+-rw-rw-rw-   0        0        0     3029 2023-02-02 16:43:38.000000 guilded.py-1.9.1/guilded/types/webhook.py
+-rw-rw-rw-   0        0        0    25099 2023-06-14 19:08:15.000000 guilded.py-1.9.1/guilded/user.py
+-rw-rw-rw-   0        0        0    13639 2022-12-16 17:30:53.000000 guilded.py-1.9.1/guilded/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.668995 guilded.py-1.9.1/guilded/webhook/
+-rw-rw-rw-   0        0        0       23 2022-10-15 20:19:00.000000 guilded.py-1.9.1/guilded/webhook/__init__.py
+-rw-rw-rw-   0        0        0    37376 2023-06-10 18:00:40.000000 guilded.py-1.9.1/guilded/webhook/async_.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 03:46:11.000000 guilded.py-1.9.1/guilded/webhook/sync.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:12:50.621994 guilded.py-1.9.1/guilded.py.egg-info/
+-rw-rw-rw-   0        0        0     2101 2023-06-14 19:12:50.000000 guilded.py-1.9.1/guilded.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1694 2023-06-14 19:12:50.000000 guilded.py-1.9.1/guilded.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:12:50.000000 guilded.py-1.9.1/guilded.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-06-14 19:12:50.000000 guilded.py-1.9.1/guilded.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 19:12:50.000000 guilded.py-1.9.1/guilded.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 19:12:50.670994 guilded.py-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2022-09-23 00:42:16.000000 guilded.py-1.9.1/setup.py
```

### Comparing `guilded.py-1.9.0/LICENSE` & `guilded.py-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/PKG-INFO` & `guilded.py-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guilded.py
-Version: 1.9.0
+Version: 1.9.1
 Summary: An API wrapper in Python for Guilded's bot API
 Home-page: https://github.com/shayypy/guilded.py
 Author: shay (shayypy)
 License: MIT
 Project-URL: Documentation, https://guildedpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/shayypy/guilded.py/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `guilded.py-1.9.0/README.md` & `guilded.py-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/__init__.py` & `guilded.py-1.9.1/guilded/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 __copyright__ = 'shay 2020-present'
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 
 import logging
 
 from . import abc as abc, utils as utils
 from .utils import Object as Object
 from .asset import *
 from .channel import *
```

### Comparing `guilded.py-1.9.0/guilded/abc.py` & `guilded.py-1.9.1/guilded/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,27 +51,28 @@
 
 from __future__ import annotations
 
 import abc
 import datetime
 import re
 from typing import TYPE_CHECKING, List, Optional, Sequence
-from typing_extensions import Self
 
 from .asset import Asset
 from .colour import Colour
 from .enums import ChannelType, try_enum, UserType
 from .errors import InvalidArgument
 from .message import HasContentMixin, ChatMessage
 from .mixins import Hashable
 from .presence import Presence
 from .status import Status
 from .utils import ISO8601, MISSING
 
 if TYPE_CHECKING:
+    from typing_extensions import Self
+
     from .types.user import User as UserPayload
     from .types.channel import ServerChannel as ServerChannelPayload
     from .types.comment import ContentComment
 
     from .channel import Thread
     from .embed import Embed
     from .group import Group
@@ -367,16 +368,17 @@
     bot_id: Optional[:class:`str`]
         The user's corresponding bot ID, if any.
         This will likely only be available for the connected :class:`.ClientUser`.
     avatar: Optional[:class:`.Asset`]
         The user's set avatar, if any.
     banner: Optional[:class:`.Asset`]
         The user's profile banner, if any.
-    created_at: :class:`datetime.datetime`
+    created_at: Optional[:class:`datetime.datetime`]
         When the user's account was created.
+        This may be ``None`` if the user object was partial.
     status: Optional[:class:`.Status`]
         The custom status set by the user.
     """
 
     __slots__ = (
         'type',
         '_user_type',
@@ -649,17 +651,16 @@
         if public is not None:
             payload['isPublic'] = public
 
         data = await self._state.update_channel(
             self.id,
             payload=payload,
         )
-        channel = self.__class__.__init__(
+        channel: Self = self._state.create_channel(
             data=data['channel'],
-            state=self._state,
             group=self.group,
         )
         return channel
 
     async def delete(self) -> None:
         """|coro|
```

### Comparing `guilded.py-1.9.0/guilded/asset.py` & `guilded.py-1.9.1/guilded/asset.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/backoff.py` & `guilded.py-1.9.1/guilded/backoff.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/channel.py` & `guilded.py-1.9.1/guilded/channel.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/client.py` & `guilded.py-1.9.1/guilded/client.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/colour.py` & `guilded.py-1.9.1/guilded/colour.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/embed.py` & `guilded.py-1.9.1/guilded/embed.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/emote.py` & `guilded.py-1.9.1/guilded/emote.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/enums.py` & `guilded.py-1.9.1/guilded/enums.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/errors.py` & `guilded.py-1.9.1/guilded/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,21 +45,31 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from aiohttp import ClientResponse
+
+    from .types.http import HTTPError as HTTPErrorPayload
+
 __all__ = (
     'GuildedException',
     'ClientException',
     'HTTPException',
     'BadRequest',
     'Forbidden',
     'NotFound',
+    'ImATeapot',
     'TooManyRequests',
     'GuildedServerError',
     'InvalidData',
     'InvalidArgument',
 )
 
 
@@ -85,42 +95,82 @@
         The HTTP status code of the request.
     code: :class:`str`
         A PascalCase representation of the HTTP status code. Could also be
         called the error's name. Probably not useful in most cases.
     message: :class:`str`
         The message that came with the error.
     """
-    def __init__(self, response, data):
+    def __init__(self, response: ClientResponse, data: HTTPErrorPayload):
         self.response = response
         self.status = response.status
+        self.message: str = ''
+        self.code: str = ''
         if isinstance(data, dict):
-            self.message = data.get('message', data)
+            self.message = data.get('message') or ''
             self.code = data.get('code', 'UnknownCode')
-        else:
-            self.message = data
-            self.code = ''
 
         super().__init__(f'{self.status} ({self.code}): {self.message}')
 
 
 class BadRequest(HTTPException):
     """Thrown on status code 400"""
     pass
 
 
 class Forbidden(HTTPException):
-    """Thrown on status code 403"""
-    pass
+    """Thrown on status code 403
+
+    Attributes
+    -----------
+    raw_missing_permissions: Optional[List[:class:`str`]]
+        If applicable, the permissions that the client is missing for
+        the operation.
+        This is a list of :gdocs:`raw permissions values <Permissions>`\.
+
+        .. versionadded:: 1.9.1
+    """
+    def __init__(self, response: ClientResponse, data: HTTPErrorPayload):
+        super().__init__(response, data)
+
+        missing_permissions = None
+        if data.get('meta') and data['meta'].get('missingPermissions'):
+            missing_permissions = data['meta']['missingPermissions']
 
+        self.raw_missing_permissions = missing_permissions
 
 class NotFound(HTTPException):
     """Thrown on status code 404"""
     pass
 
 
+class ImATeapot(HTTPException):
+    """Thrown on status code 418
+
+    Currently, this error should only be thrown from :gdocs:`Read a server
+    member's permissions <roles/ServerMemberPermissionsRead>`, when the member
+    does not have all the permissions passed to ``ids``.
+
+    .. versionadded:: 1.9.1
+
+    Attributes
+    -----------
+    raw_missing_permissions: Optional[List[:class:`str`]]
+        If applicable, the permissions that the member is missing.
+        This is a list of :gdocs:`raw permissions values <Permissions>`\.
+    """
+    def __init__(self, response: ClientResponse, data: HTTPErrorPayload):
+        super().__init__(response, data)
+
+        missing_permissions = None
+        if data.get('meta') and data['meta'].get('missingPermissions'):
+            missing_permissions = data['meta']['missingPermissions']
+
+        self.raw_missing_permissions = missing_permissions
+
+
 class TooManyRequests(HTTPException):
     """Thrown on status code 429"""
     pass
 
 
 class GuildedServerError(HTTPException):
     """Thrown on status code 500"""
```

### Comparing `guilded.py-1.9.0/guilded/events.py` & `guilded.py-1.9.1/guilded/events.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/_types.py` & `guilded.py-1.9.1/guilded/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/bot.py` & `guilded.py-1.9.1/guilded/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/cog.py` & `guilded.py-1.9.1/guilded/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/context.py` & `guilded.py-1.9.1/guilded/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/converters.py` & `guilded.py-1.9.1/guilded/ext/commands/converters.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/cooldowns.py` & `guilded.py-1.9.1/guilded/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/core.py` & `guilded.py-1.9.1/guilded/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/errors.py` & `guilded.py-1.9.1/guilded/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/help.py` & `guilded.py-1.9.1/guilded/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/commands/view.py` & `guilded.py-1.9.1/guilded/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/ext/tasks/__init__.py` & `guilded.py-1.9.1/guilded/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/file.py` & `guilded.py-1.9.1/guilded/file.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/flowbot.py` & `guilded.py-1.9.1/guilded/flowbot.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/gateway.py` & `guilded.py-1.9.1/guilded/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -1269,28 +1269,28 @@
     async def parse_user_status_created(self, data: gw.UserStatusCreatedEvent):
         if self._exp_style:
             event = ev.UserStatusCreateEvent(self._state, data)
             self.client.dispatch(event)
 
         else:
             user = self._state._get_user(data['userId'])
-            status = Status(state=self._state, data=data['userStatus'])
+            status = Status(data=data['userStatus'])
             expires_at = ISO8601(data.get('expiresAt'))
 
             if user:
                 self.client.dispatch('user_status_create', user, status, expires_at)
 
     async def parse_user_status_deleted(self, data: gw.UserStatusDeletedEvent):
         if self._exp_style:
             event = ev.UserStatusDeleteEvent(self._state, data)
             self.client.dispatch(event)
 
         else:
             user = self._state._get_user(data['userId'])
-            status = Status(state=self._state, data=data['userStatus'])
+            status = Status(data=data['userStatus'])
 
             if user:
                 self.client.dispatch('user_status_delete', user, status)
 
     async def parse_role_created(self, data: gw.RoleEvent):
         if self._exp_style:
             event = ev.RoleCreateEvent(self._state, data)
```

### Comparing `guilded.py-1.9.0/guilded/group.py` & `guilded.py-1.9.1/guilded/group.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/http.py` & `guilded.py-1.9.1/guilded/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,15 +511,18 @@
                 self.my_id = authenticated_as
 
                 # Update the ClientUser
                 if last_user:
                     last_user.id = self.my_id
                     self._users[self.my_id] = last_user
 
-            data = await json_or_text(response)
+            if response.headers.get('Content-Type', '').startswith(('image/', 'video/')):
+                data = await response.read()
+            else:
+                data = await json_or_text(response)
 
             # The request was successful so just return the text/json
             if 300 > response.status >= 200:
                 log.debug('%s %s has received %s', method, url, data)
                 return data
 
             if response.status == 429:
@@ -1037,14 +1040,21 @@
 
     def set_member_xp(self, server_id: str, user_id: str, total: int):
         payload = {
             'total': total,
         }
         return self.request(Route('PUT', f'/servers/{server_id}/members/{user_id}/xp'), json=payload)
 
+    def get_member_permissions(self, server_id: str, user_id: str, *, ids: List[str] = None):
+        params = {}
+        if ids is not None:
+            params['ids'] = ','.join(ids)
+
+        return self.request(Route('GET', f'/servers/{server_id}/members/{user_id}/permissions'), params=params)
+
     def award_role_xp(self, server_id: str, role_id: int, amount: int):
         payload = {
             'amount': amount,
         }
         return self.request(Route('POST', f'/servers/{server_id}/roles/{role_id}/xp'), json=payload)
 
     def create_role(self, server_id: str, *, payload: Dict[str, Any]):
@@ -1055,14 +1065,20 @@
 
     def get_roles(self, server_id: str):
         return self.request(Route('GET', f'/servers/{server_id}/roles'))
 
     def update_role(self, server_id: str, role_id: int, *, payload: Dict[str, Any]):
         return self.request(Route('PATCH', f'/servers/{server_id}/roles/{role_id}'), json=payload)
 
+    def update_role_permissions(self, server_id: str, role_id: int, *, permissions: Dict[str, bool]):
+        payload = {
+            'permissions': permissions,
+        }
+        return self.request(Route('PATCH', f'/servers/{server_id}/roles/{role_id}/permissions'), json=payload)
+
     def delete_role(self, server_id: str, role_id: int):
         return self.request(Route('DELETE', f'/servers/{server_id}/roles/{role_id}'))
 
     def ban_server_member(self, server_id: str, user_id: str, *, reason: str = None):
         payload = {}
         if reason is not None:
             payload['reason'] = reason
```

### Comparing `guilded.py-1.9.0/guilded/invite.py` & `guilded.py-1.9.1/guilded/invite.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/message.py` & `guilded.py-1.9.1/guilded/message.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/mixins.py` & `guilded.py-1.9.1/guilded/mixins.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/permissions.py` & `guilded.py-1.9.1/guilded/permissions.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/presence.py` & `guilded.py-1.9.1/guilded/presence.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/reaction.py` & `guilded.py-1.9.1/guilded/reaction.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/reply.py` & `guilded.py-1.9.1/guilded/reply.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/role.py` & `guilded.py-1.9.1/guilded/role.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,26 +82,31 @@
         Whether members may add themselves to this role without requiring
         permissions to manage roles.
     displayed_separately: :class:`bool`
         Whether the role is displayed seperately (or "hoisted") in the member
         list.
     base: :class:`bool`
         Whether the role is the base ``Member`` role.
+    bot_user_id: Optional[:class:`str`]
+        The user ID of the bot that the role was created for.
+        If this is present, it means the role cannot be deleted normally or
+        assigned to other members.
     """
 
     __slots__: Tuple[str, ...] = (
         '_state',
         'server_id',
         'id',
         'name',
         '_colours',
         'created_at',
         'updated_at',
         '_icon',
         '_permissions',
+        'bot_user_id',
         'position',
         'mentionable',
         'self_assignable',
         'displayed_separately',
         'base',
     )
 
@@ -115,14 +120,15 @@
         self._permissions = data.get('permissions') or []
 
         self.created_at = ISO8601(data.get('createdAt'))
         self.updated_at = ISO8601(data.get('updatedAt'))
 
         self._icon = data.get('icon')
 
+        self.bot_user_id: Optional[str] = data.get('botUserId')
         self.position: int = data.get('position', 0)
         self.mentionable: bool = data.get('isMentionable', False)
         self.self_assignable: bool = data.get('isSelfAssignable', False)
         self.displayed_separately: bool = data.get('isDisplayedSeparately', False)
         self.base: bool = data.get('isBase', False)
 
     def __str__(self) -> str:
@@ -224,29 +230,39 @@
         return self.displayed_separately
 
     @property
     def permissions(self) -> Permissions:
         """:class:`.Permissions`: The permissions that the role has."""
         return Permissions(*self._permissions)
 
+    @property
+    def bot_member(self) -> Optional[Member]:
+        """Optional[:class:`.Member`]: The bot member that this managed role is assigned to."""
+        return self.server.get_member(self.bot_user_id)
+
+    def is_bot_managed(self) -> bool:
+        """:class:`bool`: Whether the role is associated with a specific bot in the server."""
+        return self.bot_user_id is not None
+
     def is_default(self) -> bool:
         """|dpyattr|
 
         This is an alias of :attr:`.base`.
         """
         return self.base
 
     def is_assignable(self) -> bool:
         """:class:`bool`: Whether the bot can give the role to users.
 
         Does not account for your permissions.
         """
         # TODO: Account for role hierarchy
         return (
-            not self.is_default()
+            not self.is_default() and
+            not self.is_bot_managed()
         )
 
     async def award_xp(self, amount: int) -> None:
         """|coro|
 
         Award XP to all members with this role. Could be a negative value to
         remove XP.
```

### Comparing `guilded.py-1.9.0/guilded/server.py` & `guilded.py-1.9.1/guilded/server.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/status.py` & `guilded.py-1.9.1/guilded/status.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/subscription.py` & `guilded.py-1.9.1/guilded/subscription.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/announcement.py` & `guilded.py-1.9.1/guilded/types/announcement.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/calendar_event.py` & `guilded.py-1.9.1/guilded/types/calendar_event.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/channel.py` & `guilded.py-1.9.1/guilded/types/channel.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/doc.py` & `guilded.py-1.9.1/guilded/types/doc.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/embed.py` & `guilded.py-1.9.1/guilded/types/embed.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/emote.py` & `guilded.py-1.9.1/guilded/types/emote.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/forum_topic.py` & `guilded.py-1.9.1/guilded/types/forum_topic.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/gateway.py` & `guilded.py-1.9.1/guilded/types/gateway.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/group.py` & `guilded.py-1.9.1/guilded/types/group.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/list_item.py` & `guilded.py-1.9.1/guilded/types/list_item.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/message.py` & `guilded.py-1.9.1/guilded/types/message.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/reaction.py` & `guilded.py-1.9.1/guilded/types/reaction.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/role.py` & `guilded.py-1.9.1/guilded/types/role.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,7 +37,8 @@
     isSelfAssignable: NotRequired[bool]
     isMentionable: NotRequired[bool]
     permissions: List[str]
     colors: NotRequired[List[int]]
     icon: NotRequired[str]
     position: int
     isBase: NotRequired[bool]
+    botUserId: NotRequired[str]
```

### Comparing `guilded.py-1.9.0/guilded/types/server.py` & `guilded.py-1.9.1/guilded/types/server.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/social_link.py` & `guilded.py-1.9.1/guilded/types/social_link.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/subscription.py` & `guilded.py-1.9.1/guilded/types/subscription.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/user.py` & `guilded.py-1.9.1/guilded/types/user.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/types/webhook.py` & `guilded.py-1.9.1/guilded/types/webhook.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/user.py` & `guilded.py-1.9.1/guilded/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,16 +214,17 @@
 
         .. describe:: str(x)
 
             Returns the member's name.
 
     Attributes
     -----------
-    joined_at: :class:`datetime.datetime`
+    joined_at: Optional[:class:`datetime.datetime`]
         When the member joined their server.
+        This may be ``None`` if the member object was partial.
     nick: Optional[:class:`str`]
         The member's nickname, if any.
     xp: Optional[:class:`int`]
         The member's XP. If this is ``None``, do not assume ``0``.
     """
 
     __slots__ = (
@@ -248,15 +249,15 @@
 
     def __init__(self, *, state, data: ServerMemberPayload, **extra):
         self._state = state
         self._user = User(state=state, data=data)
         state._users[self._user.id] = self._user
 
         self._server = extra.get('server')
-        self.server_id: str = data.get('teamId') or data.get('serverId')
+        self.server_id: str = self._server.id if self._server else data.get('serverId') or data.get('teamId')
 
         self._role_ids: Set[int] = set(data.get('roleIds') or [])
         self._owner: Optional[bool] = data.get('isOwner')
         self.nick: Optional[str] = data.get('nickname')
         self.joined_at: datetime.datetime = ISO8601(data.get('joinedAt'))
         self.xp: Optional[int] = data.get('xp')
 
@@ -629,14 +630,41 @@
             The total amount of XP this member has after the operation.
         """
 
         data = await self._state.set_member_xp(self.server.id, self.id, total)
         self.xp = data['total']
         return self.xp
 
+    async def fetch_permissions(self) -> Permissions:
+        """|coro|
+
+        Fetch this member's server permissions.
+
+        .. versionadded:: 1.9.1
+
+        Returns
+        --------
+        :class:`.Permissions`
+            The permissions that this member has.
+
+        Raises
+        -------
+        NotFound
+            The member does not exist.
+        HTTPException
+            Failed to fetch the member's permissions.
+        """
+
+        data = await self._state.get_member_permissions(
+            self.server.id,
+            self.id,
+            # ids=require.values if require is not MISSING else None,
+        )
+        return Permissions(*data['permissions'])
+
 
 class MemberBan:
     """Represents a ban created in a :class:`.Server`.
 
     .. container:: operations
 
         .. describe:: x == y
```

### Comparing `guilded.py-1.9.0/guilded/utils.py` & `guilded.py-1.9.1/guilded/utils.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.9.0/guilded/webhook/async_.py` & `guilded.py-1.9.1/guilded/webhook/async_.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,17 +568,14 @@
             The authentication token of the webhook.
         session: :class:`aiohttp.ClientSession`
             The session to use to send requests with.
             Note that the library does not manage the session and will not close it.
         auth_token: Optional[:class:`str`]
             The bot authentication token for authenticated requests
             involving the webhook.
-            For user authentication, this should be a ``guilded_mid`` cookie.
-        bot: Optional[:class:`bool`]
-            Whether ``auth_token`` represents a bot account.
 
         Returns
         --------
         :class:`Webhook`
             A partial :class:`Webhook`.
             A partial webhook is a webhook object with only an ID and a token.
         """
```

### Comparing `guilded.py-1.9.0/guilded.py.egg-info/PKG-INFO` & `guilded.py-1.9.1/guilded.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guilded.py
-Version: 1.9.0
+Version: 1.9.1
 Summary: An API wrapper in Python for Guilded's bot API
 Home-page: https://github.com/shayypy/guilded.py
 Author: shay (shayypy)
 License: MIT
 Project-URL: Documentation, https://guildedpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/shayypy/guilded.py/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `guilded.py-1.9.0/guilded.py.egg-info/SOURCES.txt` & `guilded.py-1.9.1/guilded.py.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 guilded/types/comment.py
 guilded/types/doc.py
 guilded/types/embed.py
 guilded/types/emote.py
 guilded/types/forum_topic.py
 guilded/types/gateway.py
 guilded/types/group.py
+guilded/types/http.py
 guilded/types/list_item.py
 guilded/types/message.py
 guilded/types/reaction.py
 guilded/types/role.py
 guilded/types/server.py
 guilded/types/social_link.py
 guilded/types/subscription.py
```

### Comparing `guilded.py-1.9.0/setup.py` & `guilded.py-1.9.1/setup.py`

 * *Files identical despite different names*

