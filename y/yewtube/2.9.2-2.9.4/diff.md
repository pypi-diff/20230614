# Comparing `tmp/yewtube-2.9.2.tar.gz` & `tmp/yewtube-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yewtube-2.9.2.tar", last modified: Thu Jan 26 05:42:59 2023, max compression
+gzip compressed data, was "yewtube-2.9.4.tar", last modified: Sat Jan 28 11:15:58 2023, max compression
```

## Comparing `yewtube-2.9.2.tar` & `yewtube-2.9.4.tar`

### file list

```diff
@@ -1,120 +1,64 @@
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.525917 yewtube-2.9.2/
--rw-r--r--   0 programmer  (1000) programmer  (1000)      148 2022-03-08 09:46:08.000000 yewtube-2.9.2/.gitignore
--rw-r--r--   0 programmer  (1000) programmer  (1000)    22225 2023-01-26 05:42:54.000000 yewtube-2.9.2/CHANGELOG.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)      947 2022-03-08 09:46:08.000000 yewtube-2.9.2/CONTRIBUTING.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)      758 2022-03-08 09:46:08.000000 yewtube-2.9.2/Dockerfile
--rw-r--r--   0 programmer  (1000) programmer  (1000)      707 2022-03-08 09:46:08.000000 yewtube-2.9.2/ISSUE_TEMPLATE.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)    35127 2022-03-08 09:46:08.000000 yewtube-2.9.2/LICENSE
--rw-r--r--   0 programmer  (1000) programmer  (1000)       83 2022-03-08 09:46:08.000000 yewtube-2.9.2/MANIFEST.in
--rw-r--r--   0 programmer  (1000) programmer  (1000)     7583 2023-01-26 05:42:59.526917 yewtube-2.9.2/PKG-INFO
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5902 2022-10-20 12:27:21.000000 yewtube-2.9.2/README.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1849 2022-03-08 09:46:08.000000 yewtube-2.9.2/RELEASING.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)       26 2022-03-08 09:46:08.000000 yewtube-2.9.2/_config.yml
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.511917 yewtube-2.9.2/doc/
--rw-r--r--   0 programmer  (1000) programmer  (1000)    11602 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/conf.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      424 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/index.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)       70 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/modules.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      130 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.c.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      142 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.cache.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      190 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.album_search.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      172 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.config.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      178 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.download.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      196 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.local_playlist.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      166 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.misc.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      166 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.play.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      486 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      172 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.search.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      178 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.commands.songlist.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      145 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.config.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      148 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.content.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      130 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.g.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      151 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.helptext.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      148 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.history.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      139 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.init.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      139 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.main.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      142 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.mpris.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      142 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.paths.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      145 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.player.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      151 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.playlist.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      154 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.playlists.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      655 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      145 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.screen.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      148 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.streams.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      163 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.terminalsize.rst
--rw-r--r--   0 programmer  (1000) programmer  (1000)      139 2022-03-08 09:46:08.000000 yewtube-2.9.2/doc/mps_youtube.util.rst
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.512917 yewtube-2.9.2/docs/
--rw-r--r--   0 programmer  (1000) programmer  (1000)       22 2022-03-08 09:46:08.000000 yewtube-2.9.2/docs/changelog.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)       25 2022-03-08 09:46:08.000000 yewtube-2.9.2/docs/contributing.md
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.512917 yewtube-2.9.2/docs/css/
--rw-r--r--   0 programmer  (1000) programmer  (1000)      689 2022-03-08 09:46:08.000000 yewtube-2.9.2/docs/css/mkdocstrings.css
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1015 2022-03-08 09:46:08.000000 yewtube-2.9.2/docs/gen_ref_nav.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)       19 2022-03-08 09:46:08.000000 yewtube-2.9.2/docs/index.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)       25 2022-03-08 09:46:08.000000 yewtube-2.9.2/docs/license.md
--rw-r--r--   0 programmer  (1000) programmer  (1000)      906 2022-03-08 09:46:08.000000 yewtube-2.9.2/mkdocs.yml
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.518917 yewtube-2.9.2/mps_youtube/
--rw-r--r--   0 programmer  (1000) programmer  (1000)      275 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/__init__.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      714 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/c.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1381 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/cache.py
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.521917 yewtube-2.9.2/mps_youtube/commands/
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1259 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/commands/__init__.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     9719 2022-03-17 17:41:58.000000 yewtube-2.9.2/mps_youtube/commands/album_search.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     3110 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/commands/config.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    17514 2023-01-26 05:31:24.000000 yewtube-2.9.2/mps_youtube/commands/download.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     3968 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/commands/generate_playlist.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     2192 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/commands/lastfm.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     6435 2022-09-07 19:14:54.000000 yewtube-2.9.2/mps_youtube/commands/local_playlist.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    11994 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/commands/misc.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5519 2022-09-07 18:50:58.000000 yewtube-2.9.2/mps_youtube/commands/play.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    19769 2022-05-05 02:18:46.000000 yewtube-2.9.2/mps_youtube/commands/search.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     7877 2022-09-07 18:50:58.000000 yewtube-2.9.2/mps_youtube/commands/songlist.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     9324 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/commands/spotify_playlist.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    14401 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/config.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     9173 2022-09-07 18:50:58.000000 yewtube-2.9.2/mps_youtube/content.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1956 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/contentquery.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5017 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/description_parser.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     6892 2022-04-25 15:17:54.000000 yewtube-2.9.2/mps_youtube/g.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    19115 2022-09-07 18:50:58.000000 yewtube-2.9.2/mps_youtube/helptext.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1409 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/history.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     9175 2022-03-17 17:33:29.000000 yewtube-2.9.2/mps_youtube/init.py
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.522917 yewtube-2.9.2/mps_youtube/listview/
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5676 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/listview/__init__.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      455 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/listview/base.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      817 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/listview/livestream.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1245 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/listview/songtitle.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1030 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/listview/user.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5043 2022-09-07 18:50:58.000000 yewtube-2.9.2/mps_youtube/main.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    19026 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/mpris.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5341 2023-01-26 05:32:39.000000 yewtube-2.9.2/mps_youtube/pafy.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1563 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/paths.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    12950 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/player.py
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.523917 yewtube-2.9.2/mps_youtube/players/
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1381 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/players/GenericPlayer.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)        0 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/players/__init__.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     8608 2022-10-20 12:13:48.000000 yewtube-2.9.2/mps_youtube/players/mplayer.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    11354 2022-10-20 12:35:20.000000 yewtube-2.9.2/mps_youtube/players/mpv.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1469 2022-04-25 14:06:47.000000 yewtube-2.9.2/mps_youtube/players/vlc.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1098 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/playlist.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     5350 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/playlists.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1651 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/screen.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     7145 2022-04-25 16:47:01.000000 yewtube-2.9.2/mps_youtube/streams.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     2867 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/terminalsize.py
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.524917 yewtube-2.9.2/mps_youtube/test/
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1072 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/test/test_main.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     3511 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/test/test_mpris.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)     1255 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/test/test_players_mplayer.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      293 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/test/test_util.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      686 2023-01-26 04:54:15.000000 yewtube-2.9.2/mps_youtube/test.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)    17162 2022-03-08 09:46:08.000000 yewtube-2.9.2/mps_youtube/util.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)      134 2023-01-26 05:42:45.000000 yewtube-2.9.2/requirements.txt
--rw-r--r--   0 programmer  (1000) programmer  (1000)       98 2023-01-26 05:42:59.526917 yewtube-2.9.2/setup.cfg
--rwxr-xr-x   0 programmer  (1000) programmer  (1000)     3568 2023-01-26 05:42:54.000000 yewtube-2.9.2/setup.py
--rw-r--r--   0 programmer  (1000) programmer  (1000)       90 2022-03-08 09:46:08.000000 yewtube-2.9.2/wheel_recipe.sh
--rw-r--r--   0 programmer  (1000) programmer  (1000)      230 2022-03-08 09:46:08.000000 yewtube-2.9.2/yewtube.desktop
-drwxr-xr-x   0 programmer  (1000) programmer  (1000)        0 2023-01-26 05:42:59.525917 yewtube-2.9.2/yewtube.egg-info/
--rw-r--r--   0 programmer  (1000) programmer  (1000)     7583 2023-01-26 05:42:58.000000 yewtube-2.9.2/yewtube.egg-info/PKG-INFO
--rw-r--r--   0 programmer  (1000) programmer  (1000)     2758 2023-01-26 05:42:59.000000 yewtube-2.9.2/yewtube.egg-info/SOURCES.txt
--rw-r--r--   0 programmer  (1000) programmer  (1000)        1 2023-01-26 05:42:58.000000 yewtube-2.9.2/yewtube.egg-info/dependency_links.txt
--rw-r--r--   0 programmer  (1000) programmer  (1000)       45 2023-01-26 05:42:59.000000 yewtube-2.9.2/yewtube.egg-info/entry_points.txt
--rw-r--r--   0 programmer  (1000) programmer  (1000)      321 2023-01-26 05:42:59.000000 yewtube-2.9.2/yewtube.egg-info/requires.txt
--rw-r--r--   0 programmer  (1000) programmer  (1000)       12 2023-01-26 05:42:59.000000 yewtube-2.9.2/yewtube.egg-info/top_level.txt
--rw-r--r--   0 programmer  (1000) programmer  (1000)       70 2022-03-08 09:46:08.000000 yewtube-2.9.2/yt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:15:58.910856 yewtube-2.9.4/
+-rw-r--r--   0 root         (0) root         (0)    22730 2023-01-28 11:15:56.000000 yewtube-2.9.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35127 2023-01-28 11:15:56.000000 yewtube-2.9.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       83 2023-01-28 11:15:56.000000 yewtube-2.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-01-28 11:15:58.910856 yewtube-2.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5891 2023-01-28 11:15:56.000000 yewtube-2.9.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:15:58.906856 yewtube-2.9.4/mps_youtube/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/c.py
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:15:58.906856 yewtube-2.9.4/mps_youtube/commands/
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9719 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/album_search.py
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    17514 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/generate_playlist.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/lastfm.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/local_playlist.py
+-rw-r--r--   0 root         (0) root         (0)    11994 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/misc.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/play.py
+-rw-r--r--   0 root         (0) root         (0)    19769 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)     7877 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/songlist.py
+-rw-r--r--   0 root         (0) root         (0)     9324 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/commands/spotify_playlist.py
+-rw-r--r--   0 root         (0) root         (0)    14401 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/config.py
+-rw-r--r--   0 root         (0) root         (0)     9173 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/content.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/contentquery.py
+-rw-r--r--   0 root         (0) root         (0)     5017 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/description_parser.py
+-rw-r--r--   0 root         (0) root         (0)     6892 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/g.py
+-rw-r--r--   0 root         (0) root         (0)    19115 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/helptext.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/history.py
+-rw-r--r--   0 root         (0) root         (0)     9175 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:15:58.910856 yewtube-2.9.4/mps_youtube/listview/
+-rw-r--r--   0 root         (0) root         (0)     5676 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/listview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/listview/base.py
+-rw-r--r--   0 root         (0) root         (0)      817 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/listview/livestream.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/listview/songtitle.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/listview/user.py
+-rw-r--r--   0 root         (0) root         (0)     5043 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/main.py
+-rw-r--r--   0 root         (0) root         (0)    19026 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/mpris.py
+-rw-r--r--   0 root         (0) root         (0)     5341 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/pafy.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/paths.py
+-rw-r--r--   0 root         (0) root         (0)    12950 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/player.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:15:58.910856 yewtube-2.9.4/mps_youtube/players/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/players/GenericPlayer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/players/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8608 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/players/mplayer.py
+-rw-r--r--   0 root         (0) root         (0)    11354 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/players/mpv.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/players/vlc.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/playlist.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/playlists.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/screen.py
+-rw-r--r--   0 root         (0) root         (0)     7145 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/streams.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/terminalsize.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-01-28 11:15:56.000000 yewtube-2.9.4/mps_youtube/util.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-01-28 11:15:58.910856 yewtube-2.9.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     3568 2023-01-28 11:15:56.000000 yewtube-2.9.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-01-28 11:15:56.000000 yewtube-2.9.4/yewtube.desktop
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 11:15:58.910856 yewtube-2.9.4/yewtube.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-01-28 11:15:58.000000 yewtube-2.9.4/yewtube.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-01-28 11:15:58.000000 yewtube-2.9.4/yewtube.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-28 11:15:58.000000 yewtube-2.9.4/yewtube.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-01-28 11:15:58.000000 yewtube-2.9.4/yewtube.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-01-28 11:15:58.000000 yewtube-2.9.4/yewtube.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-01-28 11:15:58.000000 yewtube-2.9.4/yewtube.egg-info/top_level.txt
```

### Comparing `yewtube-2.9.2/CHANGELOG.md` & `yewtube-2.9.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.9.4 (2023-01-28)
+### Fix
+* Semantic release python pypi receipe ([`495629a`](https://github.com/mps-youtube/yewtube/commit/495629ab78534a1a6b36a2adae2bc6c200083706))
+
+## v2.9.3 (2023-01-28)
+### Fix
+* Updated readme metioned yewtube as fork of mpsyt ([`385d6a7`](https://github.com/mps-youtube/yewtube/commit/385d6a77708991d1d27371067023b253c2d14770))
+
+### Documentation
+* Fix broken readme links ([`6d2d723`](https://github.com/mps-youtube/yewtube/commit/6d2d723e13d18854ab0a2c8c4364ff5a1c99b5d9))
+
 ## v2.9.2 (2023-01-26)
 ### Fix
 * Remove pyreadline dependency (#105) ([#107](https://github.com/iamtalhaasghar/yewtube/issues/107)) ([`19e4148`](https://github.com/iamtalhaasghar/yewtube/commit/19e4148242380b543a4825962716550114984f11))
 
 ## v2.9.1 (2023-01-26)
 ### Fix
 * #50 - brought back download audio file ([`b46dab4`](https://github.com/iamtalhaasghar/yewtube/commit/b46dab47e61c68efa0e51836a8cc9141d15d9e87))
```

### Comparing `yewtube-2.9.2/LICENSE` & `yewtube-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/PKG-INFO` & `yewtube-2.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yewtube
-Version: 2.9.2
+Version: 2.9.4
 Summary: A Terminal based YouTube player and downloader. No Youtube API key required. Forked from mps-youtube
 Home-page: https://github.com/iamtalhaasghar/yewtube
 Download-URL: https://github.com/iamtalhaasghar/yewtube/releases
 Author: talha_programmer
 Author-email: talhaasghar.contact@simplelogin.fr
 Keywords: video,music,audio,youtube,stream,download
 Classifier: Topic :: Utilities
@@ -48,16 +48,15 @@
   \__, |\___| \_/\_/  \__|\__,_|_.__/ \___|
    __/ |                                   
   |___/
 
 
 </pre>
 
-
- Terminal based YouTube player and downloader. No Youtube API key required. Forked from mps-youtube 
+yewtube, forked from mps-youtube , is a Terminal based YouTube player and downloader. No Youtube API key required. 
 
 Installation
 -----------
 # Stable Version
 
 ### Using pip
 1. Install using `pip install yewtube`
@@ -105,59 +104,59 @@
 [mps-youtube wiki](https://github.com/mps-youtube/mps-youtube/wiki/Troubleshooting) <br>
 [yewtube wiki](https://github.com/iamtalhaasghar/yewtube/wiki/FAQ)
 
 Screenshots
 -----------
 
 Search:<br>
-![](http://mps-youtube.github.io/mps-youtube/std-search.png)
+![](http://mps-youtube.github.io/yewtube/std-search.png)
 
 A standard search is performed by entering `/` followed by search terms.
 
 You can play all of the search results by giving `1-` as input
 
 Repeating song/songs can be done with `song_number[loop]`, for example:
 `1[3]` or `4-6[2]`
 
 Local Playlists:<br>
-![](http://mps-youtube.github.io/mps-youtube/local-playlist.png)
+![](http://mps-youtube.github.io/yewtube/local-playlist.png)
 
 Search result items can easily be stored in local playlists.
 
 YouTube Playlists:<br>
-![](http://mps-youtube.github.io/mps-youtube/playlist-search.png)
+![](http://mps-youtube.github.io/yewtube/playlist-search.png)
 
 YouTube playlists can be searched and played or saved as local
 playlists.
 
 A playlist search is performed by `//` followed by search term.
 
 Download:<br>
-![](http://mps-youtube.github.io/mps-youtube/download.png)
+![](http://mps-youtube.github.io/yewtube/download.png)
 
 Content can be downloaded in various formats and resolutions.
 
 Comments:<br>
-![](http://mps-youtube.github.io/mps-youtube/comments.png)
+![](http://mps-youtube.github.io/yewtube/comments.png)
 
 A basic comments browser is available to view YouTube user comments.
 
 Music Album Matching:<br>
 
-![](http://mps-youtube.github.io/mps-youtube/album-1.png)
+![](http://mps-youtube.github.io/yewtube/album-1.png)
 
-![](http://mps-youtube.github.io/mps-youtube/album-2.png)
+![](http://mps-youtube.github.io/yewtube/album-2.png)
 
 An album title can be specified and yewtube will attempt to find
 matches for each track of the album, based on title and duration. Type
 `help search` for more info.
 
 Customisation:<br>
 
-![](http://mps-youtube.github.io/mps-youtube/customisation2.png)
+![](http://mps-youtube.github.io/yewtube/customisation2.png)
 
 Search results can be customised to display additional fields and
 ordered by various criteria.
 
 This configuration was set up using the following commands
 ```
 set order views
@@ -233,8 +232,8 @@
 ```
 
 Check also the [common-issue](https://github.com/iamtalhaasghar/yewtube/wiki/Common-issues) if you are having problem with yewtube.
 
 How to Contribute
 -----------------
 
-Contributions are welcomed! However, please check out the [contribution page](https://github.com/iamtalhaasghar/yewtube/blob/master/CONTRIBUTING.md) before making a contribution.
+Contributions are warmly welcomed! However, please check out the [contribution page](https://github.com/iamtalhaasghar/yewtube/blob/master/CONTRIBUTING.md) before making a contribution.
```

### Comparing `yewtube-2.9.2/README.md` & `yewtube-2.9.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,15 @@
   \__, |\___| \_/\_/  \__|\__,_|_.__/ \___|
    __/ |                                   
   |___/
 
 
 </pre>
 
-
- Terminal based YouTube player and downloader. No Youtube API key required. Forked from mps-youtube 
+yewtube, forked from mps-youtube , is a Terminal based YouTube player and downloader. No Youtube API key required. 
 
 Installation
 -----------
 # Stable Version
 
 ### Using pip
 1. Install using `pip install yewtube`
@@ -67,59 +66,59 @@
 [mps-youtube wiki](https://github.com/mps-youtube/mps-youtube/wiki/Troubleshooting) <br>
 [yewtube wiki](https://github.com/iamtalhaasghar/yewtube/wiki/FAQ)
 
 Screenshots
 -----------
 
 Search:<br>
-![](http://mps-youtube.github.io/mps-youtube/std-search.png)
+![](http://mps-youtube.github.io/yewtube/std-search.png)
 
 A standard search is performed by entering `/` followed by search terms.
 
 You can play all of the search results by giving `1-` as input
 
 Repeating song/songs can be done with `song_number[loop]`, for example:
 `1[3]` or `4-6[2]`
 
 Local Playlists:<br>
-![](http://mps-youtube.github.io/mps-youtube/local-playlist.png)
+![](http://mps-youtube.github.io/yewtube/local-playlist.png)
 
 Search result items can easily be stored in local playlists.
 
 YouTube Playlists:<br>
-![](http://mps-youtube.github.io/mps-youtube/playlist-search.png)
+![](http://mps-youtube.github.io/yewtube/playlist-search.png)
 
 YouTube playlists can be searched and played or saved as local
 playlists.
 
 A playlist search is performed by `//` followed by search term.
 
 Download:<br>
-![](http://mps-youtube.github.io/mps-youtube/download.png)
+![](http://mps-youtube.github.io/yewtube/download.png)
 
 Content can be downloaded in various formats and resolutions.
 
 Comments:<br>
-![](http://mps-youtube.github.io/mps-youtube/comments.png)
+![](http://mps-youtube.github.io/yewtube/comments.png)
 
 A basic comments browser is available to view YouTube user comments.
 
 Music Album Matching:<br>
 
-![](http://mps-youtube.github.io/mps-youtube/album-1.png)
+![](http://mps-youtube.github.io/yewtube/album-1.png)
 
-![](http://mps-youtube.github.io/mps-youtube/album-2.png)
+![](http://mps-youtube.github.io/yewtube/album-2.png)
 
 An album title can be specified and yewtube will attempt to find
 matches for each track of the album, based on title and duration. Type
 `help search` for more info.
 
 Customisation:<br>
 
-![](http://mps-youtube.github.io/mps-youtube/customisation2.png)
+![](http://mps-youtube.github.io/yewtube/customisation2.png)
 
 Search results can be customised to display additional fields and
 ordered by various criteria.
 
 This configuration was set up using the following commands
 ```
 set order views
@@ -195,8 +194,8 @@
 ```
 
 Check also the [common-issue](https://github.com/iamtalhaasghar/yewtube/wiki/Common-issues) if you are having problem with yewtube.
 
 How to Contribute
 -----------------
 
-Contributions are welcomed! However, please check out the [contribution page](https://github.com/iamtalhaasghar/yewtube/blob/master/CONTRIBUTING.md) before making a contribution.
+Contributions are warmly welcomed! However, please check out the [contribution page](https://github.com/iamtalhaasghar/yewtube/blob/master/CONTRIBUTING.md) before making a contribution.
```

### Comparing `yewtube-2.9.2/mps_youtube/c.py` & `yewtube-2.9.4/mps_youtube/c.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/cache.py` & `yewtube-2.9.4/mps_youtube/cache.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/__init__.py` & `yewtube-2.9.4/mps_youtube/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/album_search.py` & `yewtube-2.9.4/mps_youtube/commands/album_search.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/config.py` & `yewtube-2.9.4/mps_youtube/commands/config.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/download.py` & `yewtube-2.9.4/mps_youtube/commands/download.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/generate_playlist.py` & `yewtube-2.9.4/mps_youtube/commands/generate_playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     qs = search.generate_search_qs(query)
     wdata = pafy.call_gdata('search', qs)
     results = search.get_tracks_from_json(wdata)
     if results:
         res, score = album_search._best_song_match(
             results, query, 0.1, 1.0, 0.0)
         return res
+    return None
 
 
 def random_plname():
     """Generates a random alphanumeric string of 6 characters"""
     n_chars = 6
     return ''.join(choice(string.ascii_lowercase + string.digits)
                    for _ in range(n_chars))
```

### Comparing `yewtube-2.9.2/mps_youtube/commands/lastfm.py` & `yewtube-2.9.4/mps_youtube/commands/lastfm.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/local_playlist.py` & `yewtube-2.9.4/mps_youtube/commands/local_playlist.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/misc.py` & `yewtube-2.9.4/mps_youtube/commands/misc.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/play.py` & `yewtube-2.9.4/mps_youtube/commands/play.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/search.py` & `yewtube-2.9.4/mps_youtube/commands/search.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/songlist.py` & `yewtube-2.9.4/mps_youtube/commands/songlist.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/commands/spotify_playlist.py` & `yewtube-2.9.4/mps_youtube/commands/spotify_playlist.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/config.py` & `yewtube-2.9.4/mps_youtube/config.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/content.py` & `yewtube-2.9.4/mps_youtube/content.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/contentquery.py` & `yewtube-2.9.4/mps_youtube/contentquery.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/description_parser.py` & `yewtube-2.9.4/mps_youtube/description_parser.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/g.py` & `yewtube-2.9.4/mps_youtube/g.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/helptext.py` & `yewtube-2.9.4/mps_youtube/helptext.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/history.py` & `yewtube-2.9.4/mps_youtube/history.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/init.py` & `yewtube-2.9.4/mps_youtube/init.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/listview/__init__.py` & `yewtube-2.9.4/mps_youtube/listview/__init__.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/listview/livestream.py` & `yewtube-2.9.4/mps_youtube/listview/livestream.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/listview/songtitle.py` & `yewtube-2.9.4/mps_youtube/listview/songtitle.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/listview/user.py` & `yewtube-2.9.4/mps_youtube/listview/user.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/main.py` & `yewtube-2.9.4/mps_youtube/main.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/mpris.py` & `yewtube-2.9.4/mps_youtube/mpris.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/pafy.py` & `yewtube-2.9.4/mps_youtube/pafy.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/paths.py` & `yewtube-2.9.4/mps_youtube/paths.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/player.py` & `yewtube-2.9.4/mps_youtube/player.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/players/GenericPlayer.py` & `yewtube-2.9.4/mps_youtube/players/GenericPlayer.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/players/mplayer.py` & `yewtube-2.9.4/mps_youtube/players/mplayer.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/players/mpv.py` & `yewtube-2.9.4/mps_youtube/players/mpv.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/players/vlc.py` & `yewtube-2.9.4/mps_youtube/players/vlc.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/playlist.py` & `yewtube-2.9.4/mps_youtube/playlist.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/playlists.py` & `yewtube-2.9.4/mps_youtube/playlists.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/screen.py` & `yewtube-2.9.4/mps_youtube/screen.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/streams.py` & `yewtube-2.9.4/mps_youtube/streams.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/terminalsize.py` & `yewtube-2.9.4/mps_youtube/terminalsize.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/mps_youtube/util.py` & `yewtube-2.9.4/mps_youtube/util.py`

 * *Files identical despite different names*

### Comparing `yewtube-2.9.2/setup.py` & `yewtube-2.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
-__version__ = "2.9.2"
+__version__ = "2.9.4"
 
 options = dict(
     name="yewtube",
     version=__version__,
     description="A Terminal based YouTube player and downloader. No Youtube API key required. Forked from mps-youtube",
     keywords=["video", "music", "audio", "youtube", "stream", "download"],
     author="talha_programmer",
```

### Comparing `yewtube-2.9.2/yewtube.egg-info/PKG-INFO` & `yewtube-2.9.4/yewtube.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yewtube
-Version: 2.9.2
+Version: 2.9.4
 Summary: A Terminal based YouTube player and downloader. No Youtube API key required. Forked from mps-youtube
 Home-page: https://github.com/iamtalhaasghar/yewtube
 Download-URL: https://github.com/iamtalhaasghar/yewtube/releases
 Author: talha_programmer
 Author-email: talhaasghar.contact@simplelogin.fr
 Keywords: video,music,audio,youtube,stream,download
 Classifier: Topic :: Utilities
@@ -48,16 +48,15 @@
   \__, |\___| \_/\_/  \__|\__,_|_.__/ \___|
    __/ |                                   
   |___/
 
 
 </pre>
 
-
- Terminal based YouTube player and downloader. No Youtube API key required. Forked from mps-youtube 
+yewtube, forked from mps-youtube , is a Terminal based YouTube player and downloader. No Youtube API key required. 
 
 Installation
 -----------
 # Stable Version
 
 ### Using pip
 1. Install using `pip install yewtube`
@@ -105,59 +104,59 @@
 [mps-youtube wiki](https://github.com/mps-youtube/mps-youtube/wiki/Troubleshooting) <br>
 [yewtube wiki](https://github.com/iamtalhaasghar/yewtube/wiki/FAQ)
 
 Screenshots
 -----------
 
 Search:<br>
-![](http://mps-youtube.github.io/mps-youtube/std-search.png)
+![](http://mps-youtube.github.io/yewtube/std-search.png)
 
 A standard search is performed by entering `/` followed by search terms.
 
 You can play all of the search results by giving `1-` as input
 
 Repeating song/songs can be done with `song_number[loop]`, for example:
 `1[3]` or `4-6[2]`
 
 Local Playlists:<br>
-![](http://mps-youtube.github.io/mps-youtube/local-playlist.png)
+![](http://mps-youtube.github.io/yewtube/local-playlist.png)
 
 Search result items can easily be stored in local playlists.
 
 YouTube Playlists:<br>
-![](http://mps-youtube.github.io/mps-youtube/playlist-search.png)
+![](http://mps-youtube.github.io/yewtube/playlist-search.png)
 
 YouTube playlists can be searched and played or saved as local
 playlists.
 
 A playlist search is performed by `//` followed by search term.
 
 Download:<br>
-![](http://mps-youtube.github.io/mps-youtube/download.png)
+![](http://mps-youtube.github.io/yewtube/download.png)
 
 Content can be downloaded in various formats and resolutions.
 
 Comments:<br>
-![](http://mps-youtube.github.io/mps-youtube/comments.png)
+![](http://mps-youtube.github.io/yewtube/comments.png)
 
 A basic comments browser is available to view YouTube user comments.
 
 Music Album Matching:<br>
 
-![](http://mps-youtube.github.io/mps-youtube/album-1.png)
+![](http://mps-youtube.github.io/yewtube/album-1.png)
 
-![](http://mps-youtube.github.io/mps-youtube/album-2.png)
+![](http://mps-youtube.github.io/yewtube/album-2.png)
 
 An album title can be specified and yewtube will attempt to find
 matches for each track of the album, based on title and duration. Type
 `help search` for more info.
 
 Customisation:<br>
 
-![](http://mps-youtube.github.io/mps-youtube/customisation2.png)
+![](http://mps-youtube.github.io/yewtube/customisation2.png)
 
 Search results can be customised to display additional fields and
 ordered by various criteria.
 
 This configuration was set up using the following commands
 ```
 set order views
@@ -233,8 +232,8 @@
 ```
 
 Check also the [common-issue](https://github.com/iamtalhaasghar/yewtube/wiki/Common-issues) if you are having problem with yewtube.
 
 How to Contribute
 -----------------
 
-Contributions are welcomed! However, please check out the [contribution page](https://github.com/iamtalhaasghar/yewtube/blob/master/CONTRIBUTING.md) before making a contribution.
+Contributions are warmly welcomed! However, please check out the [contribution page](https://github.com/iamtalhaasghar/yewtube/blob/master/CONTRIBUTING.md) before making a contribution.
```

