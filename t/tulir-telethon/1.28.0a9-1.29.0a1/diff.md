# Comparing `tmp/tulir-telethon-1.28.0a9.tar.gz` & `tmp/tulir-telethon-1.29.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulir-telethon-1.28.0a9.tar", last modified: Mon Mar 13 11:38:45 2023, max compression
+gzip compressed data, was "tulir-telethon-1.29.0a1.tar", last modified: Fri May 26 10:39:27 2023, max compression
```

## Comparing `tulir-telethon-1.28.0a9.tar` & `tulir-telethon-1.29.0a1.tar`

### file list

```diff
@@ -1,169 +1,171 @@
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.085007 tulir-telethon-1.28.0a9/
--rwxrwxr-x   0 tulir     (1000) tulir     (1000)     1075 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/LICENSE
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3047 2023-03-13 11:38:45.085007 tulir-telethon-1.28.0a9/PKG-INFO
--rwxrwxr-x   0 tulir     (1000) tulir     (1000)     2221 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/README.rst
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1166 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/pyproject.toml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-03-13 11:38:45.085007 tulir-telethon-1.28.0a9/setup.cfg
--rwxrwxr-x   0 tulir     (1000) tulir     (1000)     8793 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/setup.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.065009 tulir-telethon-1.28.0a9/telethon/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      407 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.065009 tulir-telethon-1.28.0a9/telethon/_updates/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      170 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/_updates/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1581 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/_updates/entitycache.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    35484 2023-03-13 11:37:07.000000 tulir-telethon-1.28.0a9/telethon/_updates/messagebox.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6168 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/_updates/session.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.069009 tulir-telethon-1.28.0a9/telethon/client/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1200 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9572 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/account.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    23787 2023-03-13 11:37:07.000000 tulir-telethon-1.28.0a9/telethon/client/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2453 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/bots.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3280 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/buttons.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    51973 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/chats.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    23008 2022-11-24 08:59:52.000000 tulir-telethon-1.28.0a9/telethon/client/dialogs.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    39687 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/client/downloads.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9387 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/messageparse.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    61834 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/client/messages.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    40109 2023-03-13 11:37:07.000000 tulir-telethon-1.28.0a9/telethon/client/telegrambaseclient.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      478 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/client/telegramclient.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    32127 2023-03-13 11:37:07.000000 tulir-telethon-1.28.0a9/telethon/client/updates.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    32607 2023-01-27 12:40:44.000000 tulir-telethon-1.28.0a9/telethon/client/uploads.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    25436 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/client/users.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.069009 tulir-telethon-1.28.0a9/telethon/crypto/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      349 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3138 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/aes.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1216 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/aesctr.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1887 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/authkey.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3844 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/cdndecrypter.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1633 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/factorization.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4528 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/libssl.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6525 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/crypto/rsa.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       25 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/custom.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5267 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/entitycache.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.069009 tulir-telethon-1.28.0a9/telethon/errors/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1659 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/errors/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6529 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/errors/common.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3470 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/errors/rpcbaseerrors.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)   191064 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/errors/rpcerrorlist.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.073008 tulir-telethon-1.28.0a9/telethon/events/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4275 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12714 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/events/album.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    13275 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/callbackquery.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17886 2023-03-10 09:46:17.000000 tulir-telethon-1.28.0a9/telethon/events/chataction.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6312 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/common.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8971 2023-01-27 12:40:44.000000 tulir-telethon-1.28.0a9/telethon/events/inlinequery.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2128 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/messagedeleted.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1886 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/messageedited.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5470 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/messageread.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9161 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/newmessage.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1651 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/events/raw.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10617 2023-01-03 19:01:09.000000 tulir-telethon-1.28.0a9/telethon/events/userupdate.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.073008 tulir-telethon-1.28.0a9/telethon/extensions/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      280 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/extensions/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5745 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/extensions/binaryreader.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8372 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/extensions/html.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6853 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/extensions/markdown.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4075 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/extensions/messagepacker.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/functions.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    14724 2023-01-27 12:40:44.000000 tulir-telethon-1.28.0a9/telethon/helpers.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1562 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/hints.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.073008 tulir-telethon-1.28.0a9/telethon/network/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      585 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7869 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/authenticator.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.077008 tulir-telethon-1.28.0a9/telethon/network/connection/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      423 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    15698 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/connection.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1220 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/http.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      961 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/tcpabridged.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1735 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/tcpfull.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1374 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/tcpintermediate.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5279 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/tcpmtproxy.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2003 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/connection/tcpobfuscated.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2019 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/mtprotoplainsender.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    38147 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/network/mtprotosender.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10902 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/mtprotostate.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      644 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/network/requeststate.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7194 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/password.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4386 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/requestiter.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.077008 tulir-telethon-1.28.0a9/telethon/sessions/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      132 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/sessions/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4425 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/sessions/abstract.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8532 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/sessions/memory.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12845 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/sessions/sqlite.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2444 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/sessions/string.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2609 2023-01-27 12:40:44.000000 tulir-telethon-1.28.0a9/telethon/sync.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.077008 tulir-telethon-1.28.0a9/telethon/tl/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       42 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    81305 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/alltlobjects.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.077008 tulir-telethon-1.28.0a9/telethon/tl/core/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1104 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/core/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1316 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/core/gzippacked.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1763 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/core/messagecontainer.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1157 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/core/rpcresult.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1070 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/core/tlmessage.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.081008 tulir-telethon-1.28.0a9/telethon/tl/custom/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      510 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    16228 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/adminlogevent.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12369 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/button.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5186 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/chatgetter.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    19403 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/conversation.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5630 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/dialog.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5748 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/draft.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4229 2023-03-13 11:34:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/file.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2123 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/forward.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17011 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/inlinebuilder.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6254 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/inlineresult.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2754 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/inlineresults.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      310 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/inputsizedfile.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    43003 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6005 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/messagebutton.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4131 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/participantpermissions.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4205 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/qrlogin.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3777 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/custom/sendergetter.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.081008 tulir-telethon-1.28.0a9/telethon/tl/functions/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17292 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    82417 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/account.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    22182 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    11323 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/bots.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    74221 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/channels.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    22581 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/contacts.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2218 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/folders.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    15604 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/help.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5106 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/langpack.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)   272021 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/messages.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12677 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/payments.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    43036 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/phone.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10086 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/photos.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7002 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/stats.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    14496 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/stickers.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4062 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/updates.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9169 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/upload.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3591 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/functions/users.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.081008 tulir-telethon-1.28.0a9/telethon/tl/patched/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      552 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/patched/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7390 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/tl/tlobject.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.085007 tulir-telethon-1.28.0a9/telethon/tl/types/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)  1607077 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    38130 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/account.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    26180 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8295 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/types/channels.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    15361 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/contacts.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    32275 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/help.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    98523 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/messages.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    18718 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/types/payments.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10850 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/types/phone.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4329 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/photos.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    14091 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/types/stats.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      923 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/types/stickers.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3544 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/storage.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17676 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/updates.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6138 2023-03-13 11:38:44.000000 tulir-telethon-1.28.0a9/telethon/tl/types/upload.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1923 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/telethon/tl/types/users.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       24 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/types.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    54792 2022-11-07 15:02:21.000000 tulir-telethon-1.28.0a9/telethon/utils.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       98 2023-03-13 11:37:07.000000 tulir-telethon-1.28.0a9/telethon/version.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-03-13 11:38:45.085007 tulir-telethon-1.28.0a9/tulir_telethon.egg-info/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3047 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/tulir_telethon.egg-info/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4458 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/tulir_telethon.egg-info/SOURCES.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/tulir_telethon.egg-info/dependency_links.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       27 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/tulir_telethon.egg-info/requires.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        9 2023-03-13 11:38:45.000000 tulir-telethon-1.28.0a9/tulir_telethon.egg-info/top_level.txt
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.582543 tulir-telethon-1.29.0a1/
+-rwxrwxr-x   0 tulir     (1000) tulir     (1000)     1075 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/LICENSE
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3365 2023-05-26 10:39:27.582543 tulir-telethon-1.29.0a1/PKG-INFO
+-rwxrwxr-x   0 tulir     (1000) tulir     (1000)     2559 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/README.rst
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1166 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/pyproject.toml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-05-26 10:39:27.582543 tulir-telethon-1.29.0a1/setup.cfg
+-rwxrwxr-x   0 tulir     (1000) tulir     (1000)     8793 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/setup.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.566542 tulir-telethon-1.29.0a1/telethon/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      407 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.566542 tulir-telethon-1.29.0a1/telethon/_updates/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      170 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/_updates/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1853 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/_updates/entitycache.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    35472 2023-05-26 10:35:16.000000 tulir-telethon-1.29.0a1/telethon/_updates/messagebox.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6168 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/_updates/session.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.566542 tulir-telethon-1.29.0a1/telethon/client/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1200 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9572 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/account.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    23996 2023-05-26 10:35:16.000000 tulir-telethon-1.29.0a1/telethon/client/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2453 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/bots.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3280 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/buttons.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    51973 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/chats.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    23008 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/dialogs.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    39687 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/client/downloads.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9387 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/messageparse.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    62616 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/client/messages.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    42194 2023-05-26 10:35:16.000000 tulir-telethon-1.29.0a1/telethon/client/telegrambaseclient.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      478 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/client/telegramclient.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34446 2023-05-26 10:35:16.000000 tulir-telethon-1.29.0a1/telethon/client/updates.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    33661 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/client/uploads.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    25874 2023-05-26 10:34:51.000000 tulir-telethon-1.29.0a1/telethon/client/users.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.570542 tulir-telethon-1.29.0a1/telethon/crypto/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      349 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3138 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/aes.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1216 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/aesctr.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1887 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/authkey.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3844 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/cdndecrypter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1633 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/factorization.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4528 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/libssl.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6525 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/crypto/rsa.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       25 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/custom.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.570542 tulir-telethon-1.29.0a1/telethon/errors/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1659 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/errors/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6485 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/errors/common.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3470 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/errors/rpcbaseerrors.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)   191064 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/errors/rpcerrorlist.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.570542 tulir-telethon-1.29.0a1/telethon/events/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4275 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/events/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12717 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/events/album.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13424 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/events/callbackquery.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    17966 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/events/chataction.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6315 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/events/common.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8974 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/events/inlinequery.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2128 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/events/messagedeleted.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1886 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/events/messageedited.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5470 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/events/messageread.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9161 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/events/newmessage.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1651 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/events/raw.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    10620 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/events/userupdate.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.570542 tulir-telethon-1.29.0a1/telethon/extensions/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      280 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/extensions/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5745 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/extensions/binaryreader.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8372 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/extensions/html.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6853 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/extensions/markdown.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4075 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/extensions/messagepacker.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/functions.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    14724 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/helpers.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1562 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/hints.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.570542 tulir-telethon-1.29.0a1/telethon/network/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      585 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7869 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/authenticator.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.570542 tulir-telethon-1.29.0a1/telethon/network/connection/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      423 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/connection/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    15860 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/network/connection/connection.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1220 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/connection/http.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      961 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/connection/tcpabridged.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2038 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/network/connection/tcpfull.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1374 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/connection/tcpintermediate.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5279 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/connection/tcpmtproxy.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2003 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/connection/tcpobfuscated.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2019 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/mtprotoplainsender.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    38147 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/network/mtprotosender.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    10968 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/network/mtprotostate.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      644 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/network/requeststate.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7194 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/password.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4386 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/requestiter.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.574543 tulir-telethon-1.29.0a1/telethon/sessions/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      132 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/sessions/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4425 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/sessions/abstract.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8532 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/sessions/memory.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12838 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/sessions/sqlite.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2444 2023-05-26 10:34:41.000000 tulir-telethon-1.29.0a1/telethon/sessions/string.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2609 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/sync.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.574543 tulir-telethon-1.29.0a1/telethon/tl/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       42 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    82769 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/alltlobjects.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.574543 tulir-telethon-1.29.0a1/telethon/tl/core/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1104 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/core/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1316 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/core/gzippacked.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1763 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/core/messagecontainer.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1157 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/core/rpcresult.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1070 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/core/tlmessage.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.574543 tulir-telethon-1.29.0a1/telethon/tl/custom/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      510 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    16228 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/adminlogevent.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12369 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/button.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5276 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/chatgetter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19403 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/conversation.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5630 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/dialog.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5845 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/draft.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4229 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/file.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2129 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/forward.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    17011 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/inlinebuilder.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6254 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/inlineresult.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2754 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/inlineresults.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      310 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/inputsizedfile.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    43090 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6005 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/messagebutton.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4131 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/participantpermissions.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4205 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/qrlogin.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3854 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/tl/custom/sendergetter.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.578543 tulir-telethon-1.29.0a1/telethon/tl/functions/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    17303 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    82711 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/account.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    23167 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    15226 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/bots.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    74221 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/channels.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13263 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/chatlists.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    22581 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/contacts.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1449 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/folders.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    15604 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/help.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5106 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/langpack.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)   274399 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/messages.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12677 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/payments.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    43036 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/phone.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    11145 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/photos.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7002 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/stats.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    14496 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/stickers.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4062 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/updates.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9169 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/upload.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3591 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/functions/users.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.578543 tulir-telethon-1.29.0a1/telethon/tl/patched/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      552 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/patched/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7390 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/tl/tlobject.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.582543 tulir-telethon-1.29.0a1/telethon/tl/types/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)  1621993 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    38130 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/account.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    26740 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1219 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/bots.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8295 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/channels.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    10454 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/chatlists.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    15361 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/contacts.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    32275 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/help.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    98523 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/messages.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    18718 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/payments.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    10850 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/phone.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4329 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/photos.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    14091 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/stats.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      923 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/stickers.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3544 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/storage.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    17676 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/updates.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6138 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/upload.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1923 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/telethon/tl/types/users.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       24 2023-05-14 10:31:03.000000 tulir-telethon-1.29.0a1/telethon/types.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    54889 2023-05-26 09:07:01.000000 tulir-telethon-1.29.0a1/telethon/utils.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       98 2023-05-26 10:35:16.000000 tulir-telethon-1.29.0a1/telethon/version.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-26 10:39:27.582543 tulir-telethon-1.29.0a1/tulir_telethon.egg-info/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3365 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/tulir_telethon.egg-info/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4526 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/tulir_telethon.egg-info/SOURCES.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/tulir_telethon.egg-info/dependency_links.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       27 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/tulir_telethon.egg-info/requires.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        9 2023-05-26 10:39:27.000000 tulir-telethon-1.29.0a1/tulir_telethon.egg-info/top_level.txt
```

### Comparing `tulir-telethon-1.28.0a9/LICENSE` & `tulir-telethon-1.29.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/PKG-INFO` & `tulir-telethon-1.29.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tulir-telethon
-Version: 1.28.0a9
+Version: 1.29.0a1
 Summary: Full-featured Telegram client library for Python 3
 Home-page: https://github.com/tulir/Telethon
 Author: Lonami Exo
 Author-email: totufals@hotmail.com
 License: MIT
 Keywords: telegram api chat client library messaging mtproto
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -31,14 +30,16 @@
 MTProto_ library to interact with Telegram_'s API
 as a user or through a bot account (bot API alternative).
 
 .. important::
 
     If you have code using Telethon before its 1.0 version, you must
     read `Compatibility and Convenience`_ to learn how to migrate.
+    As with any third-party library for Telegram, be careful not to
+    break `Telegram's ToS`_ or `Telegram can ban the account`_.
 
 What is this?
 -------------
 
 Telegram is a popular messaging application. This library is meant
 to make it easy for you to write Python programs that can interact
 with Telegram. Think of it as a wrapper that has already done the
@@ -95,14 +96,14 @@
 in-depth explanation, with examples, troubleshooting issues, and more
 useful information.
 
 .. _asyncio: https://docs.python.org/3/library/asyncio.html
 .. _MTProto: https://core.telegram.org/mtproto
 .. _Telegram: https://telegram.org
 .. _Compatibility and Convenience: https://docs.telethon.dev/en/stable/misc/compatibility-and-convenience.html
+.. _Telegram's ToS: https://core.telegram.org/api/terms
+.. _Telegram can ban the account: https://docs.telethon.dev/en/stable/quick-references/faq.html#my-account-was-deleted-limited-when-using-the-library
 .. _Read The Docs: https://docs.telethon.dev
 
 .. |logo| image:: logo.svg
     :width: 24pt
     :height: 24pt
-
-
```

### Comparing `tulir-telethon-1.28.0a9/README.rst` & `tulir-telethon-1.29.0a1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 MTProto_ library to interact with Telegram_'s API
 as a user or through a bot account (bot API alternative).
 
 .. important::
 
     If you have code using Telethon before its 1.0 version, you must
     read `Compatibility and Convenience`_ to learn how to migrate.
+    As with any third-party library for Telegram, be careful not to
+    break `Telegram's ToS`_ or `Telegram can ban the account`_.
 
 What is this?
 -------------
 
 Telegram is a popular messaging application. This library is meant
 to make it easy for you to write Python programs that can interact
 with Telegram. Think of it as a wrapper that has already done the
@@ -72,12 +74,14 @@
 in-depth explanation, with examples, troubleshooting issues, and more
 useful information.
 
 .. _asyncio: https://docs.python.org/3/library/asyncio.html
 .. _MTProto: https://core.telegram.org/mtproto
 .. _Telegram: https://telegram.org
 .. _Compatibility and Convenience: https://docs.telethon.dev/en/stable/misc/compatibility-and-convenience.html
+.. _Telegram's ToS: https://core.telegram.org/api/terms
+.. _Telegram can ban the account: https://docs.telethon.dev/en/stable/quick-references/faq.html#my-account-was-deleted-limited-when-using-the-library
 .. _Read The Docs: https://docs.telethon.dev
 
 .. |logo| image:: logo.svg
     :width: 24pt
     :height: 24pt
```

### Comparing `tulir-telethon-1.28.0a9/pyproject.toml` & `tulir-telethon-1.29.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/setup.py` & `tulir-telethon-1.29.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/_updates/entitycache.py` & `tulir-telethon-1.29.0a1/telethon/_updates/entitycache.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 
 
 class EntityCache:
     def __init__(
         self,
         hash_map: dict = _sentinel,
         self_id: int = None,
-        self_bot: bool = False
+        self_bot: bool = None
     ):
         self.hash_map = {} if hash_map is _sentinel else hash_map
         self.self_id = self_id
         self.self_bot = self_bot
 
-    def set_self_user(self, id, bot):
+    def set_self_user(self, id, bot, hash):
         self.self_id = id
         self.self_bot = bot
+        if hash:
+            self.hash_map[id] = (hash, EntityType.BOT if bot else EntityType.USER)
 
     def get(self, id):
         try:
             hash, ty = self.hash_map[id]
             return Entity(ty, id, hash)
         except KeyError:
             return None
@@ -48,7 +50,13 @@
         )
 
     def get_all_entities(self):
         return [Entity(ty, id, hash) for id, (hash, ty) in self.hash_map.items()]
 
     def put(self, entity):
         self.hash_map[entity.id] = (entity.hash, entity.ty)
+
+    def retain(self, filter):
+        self.hash_map = {k: v for k, v in self.hash_map.items() if filter(k)}
+
+    def __len__(self):
+        return len(self.hash_map)
```

### Comparing `tulir-telethon-1.28.0a9/telethon/_updates/messagebox.py` & `tulir-telethon-1.29.0a1/telethon/_updates/messagebox.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         self.map.clear()
         if session_state.pts != NO_SEQ:
             self.map[ENTRY_ACCOUNT] = State(pts=session_state.pts, deadline=deadline)
         if session_state.qts != NO_SEQ:
             self.map[ENTRY_SECRET] = State(pts=session_state.qts, deadline=deadline)
         self.map.update((s.channel_id, State(pts=s.pts, deadline=deadline)) for s in channel_states)
 
-        self.date = datetime.datetime.fromtimestamp(session_state.date).replace(tzinfo=datetime.timezone.utc)
+        self.date = datetime.datetime.fromtimestamp(session_state.date, tz=datetime.timezone.utc)
         self.seq = session_state.seq
         self.next_deadline = ENTRY_ACCOUNT
 
     def session_state(self):
         """
         Return the current state.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/_updates/session.py` & `tulir-telethon-1.29.0a1/telethon/_updates/session.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/__init__.py` & `tulir-telethon-1.29.0a1/telethon/client/__init__.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/account.py` & `tulir-telethon-1.29.0a1/telethon/client/account.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/auth.py` & `tulir-telethon-1.29.0a1/telethon/client/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,21 +237,22 @@
                               file=sys.stderr)
                 else:
                     raise errors.PasswordHashInvalidError(request=None)
             else:
                 me = await self.sign_in(phone=phone, password=password)
 
         # We won't reach here if any step failed (exit by exception)
-        signed, name = 'Signed in successfully as', utils.get_display_name(me)
+        signed, name = 'Signed in successfully as ', utils.get_display_name(me)
+        tos = '; remember to not break the ToS or you will risk an account ban!'
         try:
-            print(signed, name)
+            print(signed, name, tos, sep='')
         except UnicodeEncodeError:
             # Some terminals don't support certain characters
             print(signed, name.encode('utf-8', errors='ignore')
-                              .decode('ascii', errors='ignore'))
+                              .decode('ascii', errors='ignore'), tos, sep='')
 
         return self
 
     def _parse_phone_and_hash(self, phone, phone_hash):
         """
         Helper method to both parse and validate phone and its hash.
         """
@@ -351,15 +352,20 @@
             )
         else:
             raise ValueError(
                 'You must provide a phone and a code the first time, '
                 'and a password only if an RPCError was raised before.'
             )
 
-        result = await self(request)
+        try:
+            result = await self(request)
+        except errors.PhoneCodeExpiredError:
+            self._phone_code_hash.pop(phone, None)
+            raise
+
         if isinstance(result, types.auth.AuthorizationSignUpRequired):
             # Emulate pre-layer 104 behaviour
             self._tos = result.terms_of_service
             raise errors.PhoneNumberUnoccupiedError(request=request)
 
         return await self._on_login(result.user)
 
@@ -379,16 +385,15 @@
 
     async def _on_login(self, user):
         """
         Callback called whenever the login or sign up process completes.
 
         Returns the input user parameter.
         """
-        self._bot = bool(user.bot)
-        self._self_input_peer = utils.get_input_peer(user, allow_self=False)
+        self._mb_entity_cache.set_self_user(user.id, user.bot, user.access_hash)
         self._authorized = True
 
         state = await self(functions.updates.GetStateRequest())
         self._message_box.load(SessionState(0, 0, 0, state.pts, state.qts, int(state.date.timestamp()), state.seq, 0), [])
 
         return user
 
@@ -503,16 +508,15 @@
                 await client.log_out()
         """
         try:
             await self(functions.auth.LogOutRequest())
         except errors.RPCError:
             return False
 
-        self._bot = None
-        self._self_input_peer = None
+        self._mb_entity_cache.set_self_user(None, None, None)
         self._authorized = False
 
         await self.disconnect()
         await self.session.delete()
         self.session = None
         return True
```

### Comparing `tulir-telethon-1.28.0a9/telethon/client/bots.py` & `tulir-telethon-1.29.0a1/telethon/client/bots.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/buttons.py` & `tulir-telethon-1.29.0a1/telethon/client/buttons.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/chats.py` & `tulir-telethon-1.29.0a1/telethon/client/chats.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/dialogs.py` & `tulir-telethon-1.29.0a1/telethon/client/dialogs.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/downloads.py` & `tulir-telethon-1.29.0a1/telethon/client/downloads.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/messageparse.py` & `tulir-telethon-1.29.0a1/telethon/client/messageparse.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/client/messages.py` & `tulir-telethon-1.29.0a1/telethon/client/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -636,15 +636,16 @@
             force_document: bool = False,
             clear_draft: bool = False,
             buttons: typing.Optional['hints.MarkupLike'] = None,
             silent: bool = None,
             background: bool = None,
             supports_streaming: bool = False,
             schedule: 'hints.DateLike' = None,
-            comment_to: 'typing.Union[int, types.Message]' = None
+            comment_to: 'typing.Union[int, types.Message]' = None,
+            nosound_video: bool = None,
     ) -> 'types.Message':
         """
         Sends a message to the specified user, chat or channel.
 
         The default parse mode is the same as the official applications
         (a custom flavour of markdown). ``**bold**, `code` or __italic__``
         are available. In addition you can send ``[links](https://example.com)``
@@ -750,14 +751,23 @@
                 Similar to ``reply_to``, but replies in the linked group of a
                 broadcast channel instead (effectively leaving a "comment to"
                 the specified message).
 
                 This parameter takes precedence over ``reply_to``. If there is
                 no linked chat, `telethon.errors.sgIdInvalidError` is raised.
 
+            nosound_video (`bool`, optional):
+                Only applicable when sending a video file without an audio
+                track. If set to ``True``, the video will be displayed in
+                Telegram as a video. If set to ``False``, Telegram will attempt
+                to display the video as an animated gif. (It may still display
+                as a video due to other factors.) The value is ignored if set
+                on non-video files. This is set to ``True`` for albums, as gifs
+                cannot be sent in albums.
+
         Returns
             The sent `custom.Message <telethon.tl.custom.message.Message>`.
 
         Example
             .. code-block:: python
 
                 # Markdown is the default
@@ -817,15 +827,16 @@
             return await self.send_file(
                 entity, file, caption=message, reply_to=reply_to,
                 attributes=attributes, parse_mode=parse_mode,
                 force_document=force_document, thumb=thumb,
                 buttons=buttons, clear_draft=clear_draft, silent=silent,
                 schedule=schedule, supports_streaming=supports_streaming,
                 formatting_entities=formatting_entities,
-                comment_to=comment_to, background=background
+                comment_to=comment_to, background=background,
+                nosound_video=nosound_video,
             )
 
         entity = await self.get_input_entity(entity)
         if comment_to is not None:
             entity, reply_to = await self._get_comment_data(entity, comment_to)
 
         if isinstance(message, types.Message):
@@ -1060,15 +1071,15 @@
         Arguments
             entity (`entity` | `Message <telethon.tl.custom.message.Message>`):
                 From which chat to edit the message. This can also be
                 the message to be edited, and the entity will be inferred
                 from it, so the next parameter will be assumed to be the
                 message text.
 
-                You may also pass a :tl:`InputBotInlineMessageID`,
+                You may also pass a :tl:`InputBotInlineMessageID` or :tl:`InputBotInlineMessageID64`,
                 which is the only way to edit messages that were sent
                 after the user selects an inline query result.
 
             message (`int` | `Message <telethon.tl.custom.message.Message>` | `str`):
                 The ID of the message (or `Message
                 <telethon.tl.custom.message.Message>` itself) to be edited.
                 If the `entity` was a `Message
@@ -1132,15 +1143,15 @@
                 time.
 
                 Note that this parameter will have no effect if you are
                 trying to edit a message that was sent via inline bots.
 
         Returns
             The edited `Message <telethon.tl.custom.message.Message>`,
-            unless `entity` was a :tl:`InputBotInlineMessageID` in which
+            unless `entity` was a :tl:`InputBotInlineMessageID` or :tl:`InputBotInlineMessageID64` in which
             case this method returns a boolean.
 
         Raises
             ``MessageAuthorRequiredError`` if you're not the author of the
             message but tried editing it anyway.
 
             ``MessageNotModifiedError`` if the contents of the message were
@@ -1158,15 +1169,15 @@
 
                 await client.edit_message(chat, message, 'hello!')
                 # or
                 await client.edit_message(chat, message.id, 'hello!!')
                 # or
                 await client.edit_message(message, 'hello!!!')
         """
-        if isinstance(entity, types.InputBotInlineMessageID):
+        if isinstance(entity, (types.InputBotInlineMessageID, types.InputBotInlineMessageID64)):
             text = text or message
             message = entity
         elif isinstance(entity, types.Message):
             text = message  # Shift the parameters to the right
             message = entity
             entity = entity.peer_id
 
@@ -1174,15 +1185,15 @@
             text, formatting_entities = await self._parse_message_text(text, parse_mode)
         file_handle, media, image = await self._file_to_media(file,
                 supports_streaming=supports_streaming,
                 thumb=thumb,
                 attributes=attributes,
                 force_document=force_document)
 
-        if isinstance(entity, types.InputBotInlineMessageID):
+        if isinstance(entity, (types.InputBotInlineMessageID, types.InputBotInlineMessageID64)):
             request = functions.messages.EditInlineBotMessageRequest(
                 id=entity,
                 message=text,
                 no_webpage=not link_preview,
                 entities=formatting_entities,
                 media=media,
                 reply_markup=self.build_reply_markup(buttons)
```

### Comparing `tulir-telethon-1.28.0a9/telethon/client/telegrambaseclient.py` & `tulir-telethon-1.29.0a1/telethon/client/telegrambaseclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import platform
 import time
 import typing
 import datetime
 
 from .. import version, helpers, errors, __name__ as __base_name__
 from ..crypto import rsa
-from ..entitycache import EntityCache
 from ..extensions import markdown
 from ..network import MTProtoSender, Connection, ConnectionTcpFull, TcpMTProxy
 from ..sessions import Session, SQLiteSession, MemorySession
 from ..tl import functions, types
 from ..tl.alltlobjects import LAYER
 from .._updates import MessageBox, EntityCache as MbEntityCache, SessionState, ChannelState, Entity, EntityType, PrematureEndReason
 
@@ -205,14 +204,28 @@
             Whether the client will receive updates or not. By default, updates
             will be received from Telegram as they occur.
 
             Turning this off means that Telegram will not send updates at all
             so event handlers, conversations, and QR login will not work.
             However, certain scripts don't need updates, so this will reduce
             the amount of bandwidth used.
+
+        entity_cache_limit (`int`, optional):
+            How many users, chats and channels to keep in the in-memory cache
+            at most. This limit is checked against when processing updates.
+
+            When this limit is reached or exceeded, all entities that are not
+            required for update handling will be flushed to the session file.
+
+            Note that this implies that there is a lower bound to the amount
+            of entities that must be kept in memory.
+
+            Setting this limit too low will cause the library to attempt to
+            flush entities to the session file even if no entities can be
+            removed from the in-memory cache, which will degrade performance.
     """
 
     # Current TelegramClient version
     __version__ = version.__version__
 
     # Cached server configuration (with .dc_options), can be "global"
     _config = None
@@ -243,14 +256,15 @@
             app_version: str = None,
             lang_code: str = 'en',
             system_lang_code: str = 'en',
             loop: asyncio.AbstractEventLoop = None,
             base_logger: typing.Union[str, logging.Logger] = None,
             receive_updates: bool = True,
             catch_up: bool = False,
+            entity_cache_limit: int = 5000,
             update_error_callback: typing.Callable[[Exception], typing.Awaitable[None]] = None,
     ):
         if not api_id or not api_hash:
             raise ValueError(
                 "Your API ID or Hash cannot be empty or None. "
                 "Refer to telethon.rtfd.io for more information.")
 
@@ -297,23 +311,22 @@
                 DEFAULT_IPV6_IP if self._use_ipv6 else DEFAULT_IPV4_IP,
                 DEFAULT_PORT
             )
 
         self.flood_sleep_threshold = flood_sleep_threshold
 
         # TODO Use AsyncClassWrapper(session)
-        # ChatGetter and SenderGetter can use the in-memory _entity_cache
+        # ChatGetter and SenderGetter can use the in-memory _mb_entity_cache
         # to avoid network access and the need for await in session files.
         #
         # The session files only wants the entities to persist
         # them to disk, and to save additional useful information.
         # TODO Session should probably return all cached
         #      info of entities, not just the input versions
         self.session = session
-        self._entity_cache = EntityCache()
         self.api_id = int(api_id)
         self.api_hash = api_hash
 
         # Current proxy implementation requires `sock_connect`, and some
         # event loops lack this method. If the current loop is missing it,
         # bail out early and suggest an alternative.
         #
@@ -383,14 +396,15 @@
         # Remember flood-waited requests to avoid making them again
         self._flood_waited_requests = {}
 
         # Cache ``{dc_id: (_ExportState, MTProtoSender)}`` for all borrowed senders
         self._borrowed_senders = {}
         self._borrow_sender_lock = asyncio.Lock()
 
+        self._loop = None  # only used as a sanity check
         self._updates_error = None
         self._updates_handle = None
         self._keepalive_handle = None
         self._last_request = time.time()
         self._no_updates = not receive_updates
 
         # Used for non-sequential updates, in order to terminate all pending tasks on disconnect.
@@ -419,27 +433,23 @@
 
         # Some fields to easy signing in. Let {phone: hash} be
         # a dictionary because the user may change their mind.
         self._phone_code_hash = {}
         self._phone = None
         self._tos = None
 
-        # Sometimes we need to know who we are, cache the self peer
-        self._self_input_peer = None
-        self._bot = None
-
         # A place to store if channels are a megagroup or not (see `edit_admin`)
         self._megagroup_cache = {}
 
         # This is backported from v2 in a very ad-hoc way just to get proper update handling
         self._catch_up = catch_up
         self._updates_queue = asyncio.Queue()
         self._message_box = MessageBox(self._log['messagebox'])
-        # This entity cache is tailored for the messagebox and is not used for absolutely everything like _entity_cache
         self._mb_entity_cache = MbEntityCache()  # required for proper update handling (to know when to getDifference)
+        self._entity_cache_limit = entity_cache_limit
 
         self._sender = MTProtoSender(
             self.session.auth_key,
             loggers=self._log,
             retries=self._connection_retries,
             delay=self._retry_delay,
             auto_reconnect=self._auto_reconnect,
@@ -525,14 +535,19 @@
                     await client.connect()
                 except OSError:
                     print('Failed to connect')
         """
         if self.session is None:
             raise ValueError('TelegramClient instance cannot be reused after logging out')
 
+        if self._loop is None:
+            self._loop = helpers.get_running_loop()
+        elif self._loop != helpers.get_running_loop():
+            raise RuntimeError('The asyncio event loop must not change after connection (see the FAQ for details)')
+
         # Workaround specific to SQLiteSession, which sometimes need to persist info after init.
         # Since .save() is now async we can't do that in init. Instead we do it in the first connect.
         if isinstance(self.session, SQLiteSession) and not self.session._init_saved:
             await self.session.save()
             self.session._init_saved = True
 
         if not await self._sender.connect(self._connection(
@@ -545,14 +560,22 @@
         )):
             # We don't want to init or modify anything if we were already connected
             return
 
         self.session.auth_key = self._sender.auth_key
         await self.session.save()
 
+        try:
+            # See comment when saving entities to understand this hack
+            self_id = (await self.session.get_input_entity(0)).access_hash
+            self_user = await self.session.get_input_entity(self_id)
+            self._mb_entity_cache.set_self_user(self_id, None, self_user.access_hash)
+        except ValueError:
+            pass
+
         self._init_request.query = functions.help.GetConfigRequest()
 
         req = self._init_request
         if self._no_updates:
             req = functions.InvokeWithoutUpdatesRequest(req)
 
         await self._sender.send(functions.InvokeWithLayerRequest(
@@ -689,14 +712,32 @@
         if connection:
             if isinstance(connection, TcpMTProxy):
                 connection._ip = proxy[0]
                 connection._port = proxy[1]
             else:
                 connection._proxy = proxy
 
+    async def _save_states_and_entities(self: 'TelegramClient'):
+        entities = self._mb_entity_cache.get_all_entities()
+
+        # Piggy-back on an arbitrary TL type with users and chats so the session can understand to read the entities.
+        # It doesn't matter if we put users in the list of chats.
+        await self.session.process_entities(types.contacts.ResolvedPeer(None, [e._as_input_peer() for e in entities], []))
+
+        # As a hack to not need to change the session files, save ourselves with ``id=0`` and ``access_hash`` of our ``id``.
+        # This way it is possible to determine our own ID by querying for 0. However, whether we're a bot is not saved.
+        if self._mb_entity_cache.self_id:
+            await self.session.process_entities(types.contacts.ResolvedPeer(None, [types.InputPeerUser(0, self._mb_entity_cache.self_id)], []))
+
+        ss, cs = self._message_box.session_state()
+        await self.session.set_update_state(0, types.updates.State(**ss, unread_count=0))
+        now = datetime.datetime.now()  # any datetime works; channels don't need it
+        for channel_id, pts in cs.items():
+            await self.session.set_update_state(channel_id, types.updates.State(pts, 0, now, 0, unread_count=0))
+
     async def _disconnect_coro(self: 'TelegramClient'):
         if self.session is None:
             return  # already logged out and disconnected
 
         await self._disconnect()
 
         # Also clean-up all exported senders because we're done with them
@@ -719,19 +760,15 @@
         if self._event_handler_tasks:
             for task in self._event_handler_tasks:
                 task.cancel()
 
             await asyncio.wait(self._event_handler_tasks)
             self._event_handler_tasks.clear()
 
-        entities = self._mb_entity_cache.get_all_entities()
-
-        # Piggy-back on an arbitrary TL type with users and chats so the session can understand to read the entities.
-        # It doesn't matter if we put users in the list of chats.
-        await self.session.process_entities(types.contacts.ResolvedPeer(None, [e._as_input_peer() for e in entities], []))
+        await self._save_states_and_entities()
 
         self._log[__name__].info("Saving update states")
         await self._save_update_state()
 
         await self.session.close()
 
     async def _save_update_state(self):
```

### Comparing `tulir-telethon-1.28.0a9/telethon/client/updates.py` & `tulir-telethon-1.29.0a1/telethon/client/updates.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import itertools
 import random
 import sys
 import time
 import traceback
 import typing
 import logging
+import warnings
 from collections import deque
 
 from .. import events, utils, errors
 from ..events.common import EventBuilder, EventCommon
 from ..tl import types, functions
 from .._updates import GapError, PrematureEndReason
 from ..helpers import get_running_loop
+from ..version import __version__
 
 from .._updates.messagebox import ENTRY_ACCOUNT, ENTRY_SECRET
 
 if typing.TYPE_CHECKING:
     from .telegramclient import TelegramClient
 
 
@@ -281,14 +283,32 @@
                             # TODO if _dispatch_update fails for whatever reason, it's not logged! this should be fixed
                             task = self.loop.create_task(self._dispatch_update(updates_to_dispatch.popleft()))
                             self._event_handler_tasks.add(task)
                             task.add_done_callback(self._event_handler_tasks.discard)
 
                     continue
 
+                if len(self._mb_entity_cache) >= self._entity_cache_limit:
+                    self._log[__name__].info(
+                        'In-memory entity cache limit reached (%s/%s), flushing to session',
+                        len(self._mb_entity_cache),
+                        self._entity_cache_limit
+                    )
+                    await self._save_states_and_entities()
+                    self._mb_entity_cache.retain(lambda id: id == self._mb_entity_cache.self_id or id in self._message_box.map)
+                    if len(self._mb_entity_cache) >= self._entity_cache_limit:
+                        warnings.warn('in-memory entities exceed entity_cache_limit after flushing; consider setting a larger limit')
+
+                    self._log[__name__].info(
+                        'In-memory entity cache at %s/%s after flushing to session',
+                        len(self._mb_entity_cache),
+                        self._entity_cache_limit
+                    )
+
+
                 get_diff = self._message_box.get_difference()
                 if get_diff:
                     old_seq = self._message_box.seq
                     self._log[__name__].info(
                         'Getting difference for account updates (seq: %d, pts: %d, qts: %d, date: %s)',
                         self._message_box.seq, get_diff.pts, get_diff.qts, get_diff.date
                     )
@@ -307,14 +327,21 @@
                             self._updates_error = e
                             if self.update_error_callback:
                                 await asyncio.shield(self.update_error_callback(e))
                             else:
                                 await self.disconnect()
                             break
                         continue
+                    except errors.TypeNotFoundError as e:
+                        # User is likely doing weird things with their account or session and Telegram gets confused as to what layer they use
+                        self._log[__name__].warning('Cannot get difference since the account is likely misusing the session: %s', e)
+                        self._message_box.end_difference()
+                        self._updates_error = e
+                        await self.disconnect()
+                        break
                     except OSError as e:
                         # Network is likely down, but it's unclear for how long.
                         # If disconnect is called this task will be cancelled along with the sleep.
                         # If disconnect is not called, getting difference should be retried after a few seconds.
                         self._log[__name__].info('Cannot get difference since the network is down: %s: %s', type(e).__name__, e)
                         await asyncio.sleep(5)
                         continue
@@ -354,14 +381,27 @@
                             self._updates_error = e
                             if self.update_error_callback:
                                 await asyncio.shield(self.update_error_callback(e))
                             else:
                                 await self.disconnect()
                             break
                         continue
+                    except errors.TypeNotFoundError as e:
+                        self._log[__name__].warning(
+                            'Cannot get difference since the account is likely misusing the session: %s',
+                            get_diff.channel.channel_id, e
+                        )
+                        self._message_box.end_channel_difference(
+                            get_diff,
+                            PrematureEndReason.TEMPORARY_SERVER_ISSUES,
+                            self._mb_entity_cache
+                        )
+                        self._updates_error = e
+                        await self.disconnect()
+                        break
                     except (
                         errors.PersistentTimestampOutdatedError,
                         errors.PersistentTimestampInvalidError,
                         errors.ServerError,
                         errors.TimeoutError,
                         ValueError
                     ) as e:
@@ -452,15 +492,15 @@
                 except GapError:
                     continue  # get(_channel)_difference will start returning requests
 
                 updates_to_dispatch.extend(await self._preprocess_updates(processed, users, chats))
         except asyncio.CancelledError:
             pass
         except Exception as e:
-            self._log[__name__].exception('Fatal error handling updates (this is a bug in Telethon, please report it)')
+            self._log[__name__].exception(f'Fatal error handling updates (this is a bug in Telethon v{__version__}, please report it)')
             self._updates_error = e
             if self.update_error_callback:
                 await asyncio.shield(self.update_error_callback(e))
             else:
                 await self.disconnect()
         finally:
             self._log[__name__].info("Update loop finished")
@@ -510,28 +550,30 @@
             except (ConnectionError, asyncio.CancelledError):
                 return
 
             # Entities and cached files are not saved when they are
             # inserted because this is a rather expensive operation
             # (default's sqlite3 takes ~0.1s to commit changes). Do
             # it every minute instead. No-op if there's nothing new.
+            await self._save_states_and_entities()
+
             try:
                 await self.session.save()
             except OSError as e:
                 # No big deal if this cannot be immediately saved
                 self._log[__name__].warning('Could not perform the periodic save of session data: %s: %s', type(e), e)
 
     async def _dispatch_update(self: 'TelegramClient', update):
         # TODO only used for AlbumHack, and MessageBox is not really designed for this
         others = None
 
-        if not self._self_input_peer:
+        if not self._mb_entity_cache.self_id:
             # Some updates require our own ID, so we must make sure
             # that the event builder has offline access to it. Calling
-            # `get_me()` will cache it under `self._self_input_peer`.
+            # `get_me()` will cache it under `self._mb_entity_cache`.
             #
             # It will return `None` if we haven't logged in yet which is
             # fine, we will just retry next time anyway.
             try:
                 await self.get_me(input_peer=True)
             except OSError:
                 pass  # might not have connection
```

### Comparing `tulir-telethon-1.28.0a9/telethon/client/uploads.py` & `tulir-telethon-1.29.0a1/telethon/client/uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             # JPEG often compresses better -> smaller size -> faster upload
             # We need to mask away the alpha channel ([3]), since otherwise
             # IOError is raised when trying to save alpha channels in JPEG.
             result = PIL.Image.new('RGB', image.size, background)
             result.paste(image, mask=image.split()[alpha_index])
 
         buffer = io.BytesIO()
-        result.save(buffer, 'JPEG', **kwargs)
+        result.save(buffer, 'JPEG', progressive=True, **kwargs)
         buffer.seek(0)
         return buffer
 
     except IOError:
         return file
     finally:
         if before is not None:
@@ -113,14 +113,15 @@
             buttons: typing.Optional['hints.MarkupLike'] = None,
             silent: bool = None,
             background: bool = None,
             supports_streaming: bool = False,
             schedule: 'hints.DateLike' = None,
             comment_to: 'typing.Union[int, types.Message]' = None,
             ttl: int = None,
+            nosound_video: bool = None,
             **kwargs) -> 'types.Message':
         """
         Sends message with the given file to the specified entity.
 
         .. note::
 
             If the ``hachoir3`` package (``hachoir`` module) is installed,
@@ -282,14 +283,23 @@
 
                 The value must be at least 1 second, and at most 60 seconds,
                 otherwise Telegram will ignore this parameter.
 
                 Not all types of media can be used with this parameter, such
                 as text documents, which will fail with ``TtlMediaInvalidError``.
 
+            nosound_video (`bool`, optional):
+                Only applicable when sending a video file without an audio
+                track. If set to ``True``, the video will be displayed in
+                Telegram as a video. If set to ``False``, Telegram will attempt
+                to display the video as an animated gif. (It may still display
+                as a video due to other factors.) The value is ignored if set
+                on non-video files. This is set to ``True`` for albums, as gifs
+                cannot be sent in albums.
+
         Returns
             The `Message <telethon.tl.custom.message.Message>` (or messages)
             containing the sent file, or messages if a list of them was passed.
 
         Example
             .. code-block:: python
 
@@ -348,42 +358,36 @@
             entity, reply_to = await self._get_comment_data(entity, comment_to)
         else:
             reply_to = utils.get_message_id(reply_to)
 
         # First check if the user passed an iterable, in which case
         # we may want to send grouped.
         if utils.is_list_like(file):
+            sent_count = 0
+            used_callback = None if not progress_callback else (
+                lambda s, t: progress_callback(sent_count + s, len(file))
+            )
+
             if utils.is_list_like(caption):
                 captions = caption
             else:
                 captions = [caption]
 
             result = []
             while file:
                 result += await self._send_album(
                     entity, file[:10], caption=captions[:10],
-                    progress_callback=progress_callback, reply_to=reply_to,
+                    progress_callback=used_callback, reply_to=reply_to,
                     parse_mode=parse_mode, silent=silent, schedule=schedule,
                     supports_streaming=supports_streaming, clear_draft=clear_draft,
                     force_document=force_document, background=background,
                 )
                 file = file[10:]
                 captions = captions[10:]
-
-            for doc, cap in zip(file, captions):
-                result.append(await self.send_file(
-                    entity, doc, allow_cache=allow_cache,
-                    caption=cap, force_document=force_document,
-                    progress_callback=progress_callback, reply_to=reply_to,
-                    attributes=attributes, thumb=thumb, voice_note=voice_note,
-                    video_note=video_note, buttons=buttons, silent=silent,
-                    supports_streaming=supports_streaming, schedule=schedule,
-                    clear_draft=clear_draft, background=background,
-                    **kwargs
-                ))
+                sent_count += 10
 
             return result
 
         if formatting_entities is not None:
             msg_entities = formatting_entities
         else:
             caption, msg_entities =\
@@ -391,15 +395,16 @@
 
         file_handle, media, image = await self._file_to_media(
             file, force_document=force_document,
             file_size=file_size,
             progress_callback=progress_callback,
             attributes=attributes,  allow_cache=allow_cache, thumb=thumb,
             voice_note=voice_note, video_note=video_note,
-            supports_streaming=supports_streaming, ttl=ttl
+            supports_streaming=supports_streaming, ttl=ttl,
+            nosound_video=nosound_video,
         )
 
         # e.g. invalid cast from :tl:`MessageMediaWebPage`
         if not media:
             raise TypeError('Cannot use {!r} as file'.format(file))
 
         markup = self.build_reply_markup(buttons)
@@ -432,24 +437,30 @@
 
         captions = []
         for c in reversed(caption):  # Pop from the end (so reverse)
             captions.append(await self._parse_message_text(c or '', parse_mode))
 
         reply_to = utils.get_message_id(reply_to)
 
+        used_callback = None if not progress_callback else (
+            # use an integer when sent matches total, to easily determine a file has been fully sent
+            lambda s, t: progress_callback(sent_count + 1 if s == t else sent_count + s / t, len(files))
+        )
+
         # Need to upload the media first, but only if they're not cached yet
         media = []
-        for file in files:
+        for sent_count, file in enumerate(files):
             # Albums want :tl:`InputMedia` which, in theory, includes
-            # :tl:`InputMediaUploadedPhoto`. However using that will
+            # :tl:`InputMediaUploadedPhoto`. However, using that will
             # make it `raise MediaInvalidError`, so we need to upload
             # it as media and then convert that to :tl:`InputMediaPhoto`.
             fh, fm, _ = await self._file_to_media(
                 file, supports_streaming=supports_streaming,
-                force_document=force_document, ttl=ttl)
+                force_document=force_document, ttl=ttl,
+                progress_callback=used_callback, nosound_video=True)
             if isinstance(fm, (types.InputMediaUploadedPhoto, types.InputMediaPhotoExternal)):
                 r = await self(functions.messages.UploadMediaRequest(
                     entity, media=fm
                 ))
 
                 fm = utils.get_input_media(r.photo)
             elif isinstance(fm, types.InputMediaUploadedDocument):
@@ -542,14 +553,21 @@
             iv ('bytes', optional):
                 In case of an encrypted upload (secret chats) an iv is supplied
 
             progress_callback (`callable`, optional):
                 A callback function accepting two parameters:
                 ``(sent bytes, total)``.
 
+                When sending an album, the callback will receive a number
+                between 0 and the amount of files as the "sent" parameter,
+                and the amount of files as the "total". Note that the first
+                parameter will be a floating point number to indicate progress
+                within a file (e.g. ``2.5`` means it has sent 50% of the third
+                file, because it's between 2 and 3).
+
         Returns
             :tl:`InputFileBig` if the file size is larger than 10MB,
             `InputSizedFile <telethon.tl.custom.inputsizedfile.InputSizedFile>`
             (subclass of :tl:`InputFile`) otherwise.
 
         Example
             .. code-block:: python
@@ -664,15 +682,15 @@
     # endregion
 
     async def _file_to_media(
             self, file, force_document=False, file_size=None,
             progress_callback=None, attributes=None, thumb=None,
             allow_cache=True, voice_note=False, video_note=False,
             supports_streaming=False, mime_type=None, as_image=None,
-            ttl=None):
+            ttl=None, nosound_video=None):
         if not file:
             return None, None, None
 
         if isinstance(file, pathlib.Path):
             file = str(file.absolute())
 
         is_image = utils.is_image(file)
@@ -751,15 +769,15 @@
             else:
                 if isinstance(thumb, pathlib.Path):
                     thumb = str(thumb.absolute())
                 thumb = await self.upload_file(thumb, file_size=file_size)
 
             # setting `nosound_video` to `True` doesn't affect videos with sound
             # instead it prevents sending silent videos as GIFs
-            nosound_video = True if mime_type.split("/")[0] == 'video' else None
+            nosound_video = nosound_video if mime_type.split("/")[0] == 'video' else None
 
             media = types.InputMediaUploadedDocument(
                 file=file_handle,
                 mime_type=mime_type,
                 attributes=attributes,
                 thumb=thumb,
                 force_file=force_document and not is_image,
```

### Comparing `tulir-telethon-1.28.0a9/telethon/client/users.py` & `tulir-telethon-1.29.0a1/telethon/client/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 
 
 class UserMethods:
     async def __call__(self: 'TelegramClient', request, ordered=False, flood_sleep_threshold=None):
         return await self._call(self._sender, request, ordered=ordered)
 
     async def _call(self: 'TelegramClient', sender, request, ordered=False, flood_sleep_threshold=None):
+        if self._loop is not None and self._loop != helpers.get_running_loop():
+            raise RuntimeError('The asyncio event loop must not change after connection (see the FAQ for details)')
+        # if the loop is None it will fail with a connection error later on
+
         if flood_sleep_threshold is None:
             flood_sleep_threshold = self.flood_sleep_threshold
         requests = (request if utils.is_list_like(request) else (request,))
         for r in requests:
             if not isinstance(r, TLRequest):
                 raise _NOT_A_REQUEST()
             await r.resolve(self, utils)
@@ -72,15 +76,14 @@
                             results.append(None)
                             continue
                         try:
                             await self.session.process_entities(result)
                         except OSError as e:
                             self._log[__name__].warning(
                                 'Failed to save possibly new entities to the session: %s: %s', type(e), e)
-                        self._entity_cache.add(result)
                         exceptions.append(None)
                         results.append(result)
                         request_index += 1
                     if any(x is not None for x in exceptions):
                         raise MultiError(exceptions, results, requests)
                     else:
                         return results
@@ -90,15 +93,14 @@
                     # It only means certain entities won't be saved.
                     try:
                         await self.session.process_entities(result)
                     except OSError as e:
                         self._log[__name__].warning(
                             'Failed to save possibly new entities to the session: %s: %s', type(e), e)
 
-                    self._entity_cache.add(result)
                     return result
             except (errors.ServerError, errors.RpcCallFailError,
                     errors.RpcMcgetFailError, errors.InterdcCallErrorError,
                     errors.InterdcCallRichErrorError) as e:
                 last_error = e
                 self._log[__name__].warning(
                     'Telegram is having internal issues %s: %s',
@@ -161,57 +163,54 @@
 
         Example
             .. code-block:: python
 
                 me = await client.get_me()
                 print(me.username)
         """
-        if input_peer and self._self_input_peer:
-            return self._self_input_peer
+        if input_peer and self._mb_entity_cache.self_id:
+            return self._mb_entity_cache.get(self._mb_entity_cache.self_id)._as_input_peer()
 
         try:
             me = (await self(
                 functions.users.GetUsersRequest([types.InputUserSelf()])))[0]
 
-            self._bot = me.bot
-            if not self._self_input_peer:
-                self._self_input_peer = utils.get_input_peer(
-                    me, allow_self=False
-                )
+            if not self._mb_entity_cache.self_id:
+                self._mb_entity_cache.set_self_user(me.id, me.bot, me.access_hash)
 
-            return self._self_input_peer if input_peer else me
+            return utils.get_input_peer(me, allow_self=False) if input_peer else me
         except errors.UnauthorizedError:
             return None
 
     @property
     def _self_id(self: 'TelegramClient') -> typing.Optional[int]:
         """
         Returns the ID of the logged-in user, if known.
 
         This property is used in every update, and some like `updateLoginToken`
         occur prior to login, so it gracefully handles when no ID is known yet.
         """
-        return self._self_input_peer.user_id if self._self_input_peer else None
+        return self._mb_entity_cache.self_id
 
     async def is_bot(self: 'TelegramClient') -> bool:
         """
         Return `True` if the signed-in user is a bot, `False` otherwise.
 
         Example
             .. code-block:: python
 
                 if await client.is_bot():
                     print('Beep')
                 else:
                     print('Hello')
         """
-        if self._bot is None:
-            self._bot = (await self.get_me()).bot
+        if self._mb_entity_cache.self_bot is None:
+            await self.get_me(input_peer=True)
 
-        return self._bot
+        return self._mb_entity_cache.self_bot
 
     async def is_user_authorized(self: 'TelegramClient') -> bool:
         """
         Returns `True` if the user is authorized (logged in).
 
         Example
             .. code-block:: python
@@ -328,28 +327,30 @@
                 functions.messages.GetChatsRequest([x.chat_id for x in chats]))).chats
         if channels:
             channels = (await self(
                 functions.channels.GetChannelsRequest(channels))).chats
 
         # Merge users, chats and channels into a single dictionary
         id_entity = {
-            utils.get_peer_id(x): x
+            # `get_input_entity` might've guessed the type from a non-marked ID,
+            # so the only way to match that with the input is by not using marks here.
+            utils.get_peer_id(x, add_mark=False): x
             for x in itertools.chain(users, chats, channels)
         }
 
         # We could check saved usernames and put them into the users,
         # chats and channels list from before. While this would reduce
         # the amount of ResolveUsername calls, it would fail to catch
         # username changes.
         result = []
         for x in inputs:
             if isinstance(x, str):
                 result.append(await self._get_entity_from_string(x))
             elif not isinstance(x, types.InputPeerSelf):
-                result.append(id_entity[utils.get_peer_id(x)])
+                result.append(id_entity[utils.get_peer_id(x, add_mark=False)])
             else:
                 result.append(next(
                     u for u in id_entity.values()
                     if isinstance(u, types.User) and u.is_self
                 ))
 
         return result[0] if single else result
@@ -424,16 +425,16 @@
         except TypeError:
             pass
 
         # Next in priority is having a peer (or its ID) cached in-memory
         try:
             # 0x2d45687 == crc32(b'Peer')
             if isinstance(peer, int) or peer.SUBCLASS_OF_ID == 0x2d45687:
-                return self._entity_cache[peer]
-        except (AttributeError, KeyError):
+                return self._mb_entity_cache.get(utils.get_peer_id(peer, add_mark=False))._as_input_peer()
+        except AttributeError:
             pass
 
         # Then come known strings that take precedence
         if peer in ('me', 'self'):
             return types.InputPeerSelf()
 
         # No InputPeer, cached peer, or known string. Fetch from disk cache
```

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/aes.py` & `tulir-telethon-1.29.0a1/telethon/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/aesctr.py` & `tulir-telethon-1.29.0a1/telethon/crypto/aesctr.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/authkey.py` & `tulir-telethon-1.29.0a1/telethon/crypto/authkey.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/cdndecrypter.py` & `tulir-telethon-1.29.0a1/telethon/crypto/cdndecrypter.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/factorization.py` & `tulir-telethon-1.29.0a1/telethon/crypto/factorization.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/libssl.py` & `tulir-telethon-1.29.0a1/telethon/crypto/libssl.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/crypto/rsa.py` & `tulir-telethon-1.29.0a1/telethon/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/errors/__init__.py` & `tulir-telethon-1.29.0a1/telethon/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/errors/common.py` & `tulir-telethon-1.29.0a1/telethon/errors/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     """
     Occurs when a type is not found, for example,
     when trying to read a TLObject with an invalid constructor code.
     """
     def __init__(self, invalid_constructor_id, remaining):
         super().__init__(
             'Could not find a matching Constructor ID for the TLObject '
-            'that was supposed to be read with ID {:08x}. Most likely, '
-            'a TLObject was trying to be read when it should not be read. '
+            'that was supposed to be read with ID {:08x}. See the FAQ '
+            'for more details. '
             'Remaining bytes: {!r}'.format(invalid_constructor_id, remaining))
 
         self.invalid_constructor_id = invalid_constructor_id
         self.remaining = remaining
 
 
 class InvalidChecksumError(Exception):
```

### Comparing `tulir-telethon-1.28.0a9/telethon/errors/rpcbaseerrors.py` & `tulir-telethon-1.29.0a1/telethon/errors/rpcbaseerrors.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/errors/rpcerrorlist.py` & `tulir-telethon-1.29.0a1/telethon/errors/rpcerrorlist.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/__init__.py` & `tulir-telethon-1.29.0a1/telethon/events/__init__.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/album.py` & `tulir-telethon-1.29.0a1/telethon/events/album.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                              msg_id=message.id, broadcast=bool(message.post))
             SenderGetter.__init__(self, message.sender_id)
             self.messages = messages
 
         def _set_client(self, client):
             super()._set_client(client)
             self._sender, self._input_sender = utils._get_entity_pair(
-                self.sender_id, self._entities, client._entity_cache)
+                self.sender_id, self._entities, client._mb_entity_cache)
 
             for msg in self.messages:
                 msg._finish_init(client, self._entities, None)
 
             if len(self.messages) == 1:
                 # This will require hacks to be a proper album event
                 hack = client._albums.get(self.grouped_id)
```

### Comparing `tulir-telethon-1.28.0a9/telethon/events/callbackquery.py` & `tulir-telethon-1.29.0a1/telethon/events/callbackquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             self.pattern_match = None
             self._message = None
             self._answered = False
 
         def _set_client(self, client):
             super()._set_client(client)
             self._sender, self._input_sender = utils._get_entity_pair(
-                self.sender_id, self._entities, client._entity_cache)
+                self.sender_id, self._entities, client._mb_entity_cache)
 
         @property
         def id(self):
             """
             Returns the query ID. The user clicking the inline
             button is the one who generated this random ID.
             """
@@ -204,16 +204,17 @@
             if not self._sender:
                 return
 
             self._input_sender = utils.get_input_peer(self._chat)
             if not getattr(self._input_sender, 'access_hash', True):
                 # getattr with True to handle the InputPeerSelf() case
                 try:
-                    self._input_sender = self._client._entity_cache[self._sender_id]
-                except KeyError:
+                    self._input_sender = self._client._mb_entity_cache.get(
+                        utils.resolve_id(self._sender_id)[0])._as_input_peer()
+                except AttributeError:
                     m = await self.get_message()
                     if m:
                         self._sender = m._sender
                         self._input_sender = m._input_sender
 
         async def answer(
                 self, message=None, cache_time=0, *, url=None, alert=False):
@@ -295,28 +296,28 @@
             return await self._client.send_message(
                 await self.get_input_chat(), *args, **kwargs)
 
         async def edit(self, *args, **kwargs):
             """
             Edits the message. Shorthand for
             `telethon.client.messages.MessageMethods.edit_message` with
-            the ``entity`` set to the correct :tl:`InputBotInlineMessageID`.
+            the ``entity`` set to the correct :tl:`InputBotInlineMessageID` or :tl:`InputBotInlineMessageID64`.
 
             Returns `True` if the edit was successful.
 
             This method also creates a task to `answer` the callback.
 
             .. note::
 
                 This method won't respect the previous message unlike
                 `Message.edit <telethon.tl.custom.message.Message.edit>`,
                 since the message object is normally not present.
             """
             self._client.loop.create_task(self.answer())
-            if isinstance(self.query.msg_id, types.InputBotInlineMessageID):
+            if isinstance(self.query.msg_id, (types.InputBotInlineMessageID, types.InputBotInlineMessageID64)):
                 return await self._client.edit_message(
                     self.query.msg_id, *args, **kwargs
                 )
             else:
                 return await self._client.edit_message(
                     await self.get_input_chat(), self.query.msg_id,
                     *args, **kwargs
```

### Comparing `tulir-telethon-1.28.0a9/telethon/events/chataction.py` & `tulir-telethon-1.29.0a1/telethon/events/chataction.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,17 +421,18 @@
                         self._input_users.append(utils.get_input_peer(self._entities[user_id]))
                         continue
                     except (KeyError, TypeError):
                         pass
 
                     # If missing, try from the entity cache
                     try:
-                        self._input_users.append(self._client._entity_cache[user_id])
+                        self._input_users.append(self._client._mb_entity_cache.get(
+                            utils.resolve_id(user_id)[0])._as_input_peer())
                         continue
-                    except KeyError:
+                    except AttributeError:
                         pass
 
             return self._input_users or []
 
         async def get_input_users(self):
             """
             Returns `input_users` but will make an API call if necessary.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/events/common.py` & `tulir-telethon-1.29.0a1/telethon/events/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     def _set_client(self, client):
         """
         Setter so subclasses can act accordingly when the client is set.
         """
         self._client = client
         if self._chat_peer:
             self._chat, self._input_chat = utils._get_entity_pair(
-                self.chat_id, self._entities, client._entity_cache)
+                self.chat_id, self._entities, client._mb_entity_cache)
         else:
             self._chat = self._input_chat = None
 
     @property
     def client(self):
         """
         The `telethon.TelegramClient` that created this event.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/events/inlinequery.py` & `tulir-telethon-1.29.0a1/telethon/events/inlinequery.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             self.query = query
             self.pattern_match = None
             self._answered = False
 
         def _set_client(self, client):
             super()._set_client(client)
             self._sender, self._input_sender = utils._get_entity_pair(
-                self.sender_id, self._entities, client._entity_cache)
+                self.sender_id, self._entities, client._mb_entity_cache)
 
         @property
         def id(self):
             """
             Returns the unique identifier for the query ID.
             """
             return self.query.query_id
```

### Comparing `tulir-telethon-1.28.0a9/telethon/events/messagedeleted.py` & `tulir-telethon-1.29.0a1/telethon/events/messagedeleted.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/messageedited.py` & `tulir-telethon-1.29.0a1/telethon/events/messageedited.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/messageread.py` & `tulir-telethon-1.29.0a1/telethon/events/messageread.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/newmessage.py` & `tulir-telethon-1.29.0a1/telethon/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/raw.py` & `tulir-telethon-1.29.0a1/telethon/events/raw.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/events/userupdate.py` & `tulir-telethon-1.29.0a1/telethon/events/userupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
             self.status = status
             self.action = typing
 
         def _set_client(self, client):
             super()._set_client(client)
             self._sender, self._input_sender = utils._get_entity_pair(
-                self.sender_id, self._entities, client._entity_cache)
+                self.sender_id, self._entities, client._mb_entity_cache)
 
         @property
         def user(self):
             """Alias for `sender <telethon.tl.custom.sendergetter.SenderGetter.sender>`."""
             return self.sender
 
         async def get_user(self):
@@ -242,15 +242,15 @@
         def photo(self):
             """
             `True` if what's being uploaded is a photo.
             """
             return isinstance(self.action, types.SendMessageUploadPhotoAction)
 
         @property
-        @_requires_action
+        @_requires_status
         def last_seen(self):
             """
             Exact `datetime.datetime` when the user was last seen if known.
             """
             if isinstance(self.status, types.UserStatusOffline):
                 return self.status.was_online
```

### Comparing `tulir-telethon-1.28.0a9/telethon/extensions/binaryreader.py` & `tulir-telethon-1.29.0a1/telethon/extensions/binaryreader.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/extensions/html.py` & `tulir-telethon-1.29.0a1/telethon/extensions/html.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/extensions/markdown.py` & `tulir-telethon-1.29.0a1/telethon/extensions/markdown.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/extensions/messagepacker.py` & `tulir-telethon-1.29.0a1/telethon/extensions/messagepacker.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/helpers.py` & `tulir-telethon-1.29.0a1/telethon/helpers.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/hints.py` & `tulir-telethon-1.29.0a1/telethon/hints.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/__init__.py` & `tulir-telethon-1.29.0a1/telethon/network/__init__.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/authenticator.py` & `tulir-telethon-1.29.0a1/telethon/network/authenticator.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/connection.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,17 @@
         self._recv_task = loop.create_task(self._recv_loop())
 
     async def disconnect(self):
         """
         Disconnects from the server, and clears
         pending outgoing and incoming messages.
         """
+        if not self._connected:
+            return
+
         self._connected = False
 
         await helpers._cancel(
             self._log,
             send_task=self._send_task,
             recv_task=self._recv_task
         )
@@ -326,30 +329,32 @@
         """
         This loop is constantly putting items on the queue as they're read.
         """
         try:
             while self._connected:
                 try:
                     data = await self._recv()
+                except asyncio.CancelledError:
+                    break
                 except (IOError, asyncio.IncompleteReadError) as e:
                     self._log.warning('Server closed the connection: %s', e)
                     await self._recv_queue.put((None, e))
+                    await self.disconnect()
                 except InvalidChecksumError as e:
                     self._log.warning('Server response had invalid checksum: %s', e)
                     await self._recv_queue.put((None, e))
                 except InvalidBufferError as e:
                     self._log.warning('Server response had invalid buffer: %s', e)
                     await self._recv_queue.put((None, e))
-                except Exception:
+                except Exception as e:
                     self._log.exception('Unexpected exception in the receive loop')
                     await self._recv_queue.put((None, e))
+                    await self.disconnect()
                 else:
                     await self._recv_queue.put((data, None))
-        except asyncio.CancelledError:
-            pass
         finally:
             await self.disconnect()
 
 
     def _init_conn(self):
         """
         This method will be called after `connect` is called.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/http.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/http.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/tcpabridged.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/tcpabridged.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/tcpfull.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/tcpfull.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,14 +26,19 @@
         packet_len, seq = struct.unpack('<ii', packet_len_seq)
         if packet_len < 0 and seq < 0:
             # It has been observed that the length and seq can be -429,
             # followed by the body of 4 bytes also being -429.
             # See https://github.com/LonamiWebs/Telethon/issues/4042.
             body = await reader.readexactly(4)
             raise InvalidBufferError(body)
+        elif packet_len < 8:
+            # Currently unknown why packet_len may be less than 8 but not negative.
+            # Attempting to `readexactly` with less than 0 fails without saying what
+            # the number was which is less helpful.
+            raise InvalidBufferError(packet_len_seq)
 
         body = await reader.readexactly(packet_len - 8)
         checksum = struct.unpack('<I', body[-4:])[0]
         body = body[:-4]
 
         valid_checksum = crc32(packet_len_seq + body)
         if checksum != valid_checksum:
```

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/tcpintermediate.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/tcpintermediate.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/tcpmtproxy.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/tcpmtproxy.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/connection/tcpobfuscated.py` & `tulir-telethon-1.29.0a1/telethon/network/connection/tcpobfuscated.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/mtprotoplainsender.py` & `tulir-telethon-1.29.0a1/telethon/network/mtprotoplainsender.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/mtprotosender.py` & `tulir-telethon-1.29.0a1/telethon/network/mtprotosender.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/network/mtprotostate.py` & `tulir-telethon-1.29.0a1/telethon/network/mtprotostate.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         if msg_key != our_key.digest()[8:24]:
             raise SecurityError(
                 "Received msg_key doesn't match with expected one")
 
         reader = BinaryReader(body)
         reader.read_long()  # remote_salt
         if reader.read_long() != self.id:
-            raise SecurityError('Server replied with a wrong session ID')
+            raise SecurityError('Server replied with a wrong session ID (see FAQ for details)')
 
         remote_msg_id = reader.read_long()
 
         if remote_msg_id % 2 != 1:
             raise SecurityError('Server sent an even msg_id')
 
         # Only perform the (somewhat expensive) check of duplicate if we did receive a lower ID
@@ -204,20 +204,20 @@
         #
         # This means we skip the time check for certain types of messages.
         if obj.CONSTRUCTOR_ID not in (BadServerSalt.CONSTRUCTOR_ID, BadMsgNotification.CONSTRUCTOR_ID):
             remote_msg_time = remote_msg_id >> 32
             time_delta = now - remote_msg_time
 
             if time_delta > MSG_TOO_OLD_DELTA:
-                self._log.warning('Server sent a very old message with ID %d, ignoring', remote_msg_id)
+                self._log.warning('Server sent a very old message with ID %d, ignoring (see FAQ for details)', remote_msg_id)
                 self._count_ignored()
                 return None
 
             if -time_delta > MSG_TOO_NEW_DELTA:
-                self._log.warning('Server sent a very new message with ID %d, ignoring', remote_msg_id)
+                self._log.warning('Server sent a very new message with ID %d, ignoring (see FAQ for details)', remote_msg_id)
                 self._count_ignored()
                 return None
 
         self._recent_remote_ids.append(remote_msg_id)
         self._highest_remote_id = remote_msg_id
         self._ignore_count = 0
```

### Comparing `tulir-telethon-1.28.0a9/telethon/network/requeststate.py` & `tulir-telethon-1.29.0a1/telethon/network/requeststate.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/password.py` & `tulir-telethon-1.29.0a1/telethon/password.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/requestiter.py` & `tulir-telethon-1.29.0a1/telethon/requestiter.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/sessions/abstract.py` & `tulir-telethon-1.29.0a1/telethon/sessions/abstract.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/sessions/memory.py` & `tulir-telethon-1.29.0a1/telethon/sessions/memory.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/sessions/sqlite.py` & `tulir-telethon-1.29.0a1/telethon/sessions/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import os
 import time
 
-from telethon.tl import types
+from ..tl import types
 from .memory import MemorySession, _SentFileType
 from .. import utils
 from ..crypto import AuthKey
 from ..tl.types import (
     InputPhoto, InputDocument, PeerUser, PeerChat, PeerChannel
 )
```

### Comparing `tulir-telethon-1.28.0a9/telethon/sessions/string.py` & `tulir-telethon-1.29.0a1/telethon/sessions/string.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/sync.py` & `tulir-telethon-1.29.0a1/telethon/sync.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/alltlobjects.py` & `tulir-telethon-1.29.0a1/telethon/tl/alltlobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """File generated by TLObjects' generator. All changes will be ERASED"""
 
 from . import types, functions
 
-LAYER = 155
+LAYER = 158
 
 tlobjects = {
     0x7f3b18ea: types.InputPeerEmpty,
     0x7da07ec9: types.InputPeerSelf,
     0x35a95cb9: types.InputPeerChat,
     0xdde8a54c: types.InputPeerUser,
     0x27bcbbfc: types.InputPeerChannel,
@@ -132,19 +132,21 @@
     0x502f92f7: types.MessageActionInviteToGroupCall,
     0x3c134d7b: types.MessageActionSetMessagesTTL,
     0xb3a07661: types.MessageActionGroupCallScheduled,
     0xaa786345: types.MessageActionSetChatTheme,
     0xebbca3cb: types.MessageActionChatJoinedByRequest,
     0x47dd8079: types.MessageActionWebViewDataSentMe,
     0xb4c38cb5: types.MessageActionWebViewDataSent,
-    0xaba0f5c6: types.MessageActionGiftPremium,
+    0xc83d6aec: types.MessageActionGiftPremium,
     0x0d999256: types.MessageActionTopicCreate,
     0xc0944820: types.MessageActionTopicEdit,
     0x57de635e: types.MessageActionSuggestProfilePhoto,
     0xfe77345d: types.MessageActionRequestedPeer,
+    0xbc44a927: types.MessageActionSetChatWallPaper,
+    0xc0787d6d: types.MessageActionSetSameChatWallPaper,
     0xd58a08c6: types.Dialog,
     0x71bd134c: types.DialogFolder,
     0x2331b22d: types.PhotoEmpty,
     0xfb197a65: types.Photo,
     0x0e17e23c: types.PhotoSizeEmpty,
     0x75c78e60: types.PhotoSize,
     0x021e1ad6: types.PhotoCachedSize,
@@ -174,15 +176,15 @@
     0xadf44ee3: types.InputReportReasonChildAbuse,
     0xc1e4a2b1: types.InputReportReasonOther,
     0x9b89f93a: types.InputReportReasonCopyright,
     0xdbd4feed: types.InputReportReasonGeoIrrelevant,
     0xf5ddd6e7: types.InputReportReasonFake,
     0x0a8eb2be: types.InputReportReasonIllegalDrugs,
     0x9ec7863d: types.InputReportReasonPersonalDetails,
-    0xf8d32aed: types.UserFull,
+    0x93eadb53: types.UserFull,
     0x145ade0b: types.Contact,
     0xc13e3c50: types.ImportedContact,
     0x16d9703b: types.ContactStatus,
     0xb74ba9d2: types.contacts.ContactsNotModified,
     0xeae87e42: types.contacts.Contacts,
     0x77d01c3b: types.contacts.ImportedContacts,
     0x0ade1591: types.contacts.Blocked,
@@ -478,15 +480,15 @@
     0xc27ac8c7: types.BotCommand,
     0x8f300b57: types.BotInfo,
     0xa2fa4880: types.KeyboardButton,
     0x258aff05: types.KeyboardButtonUrl,
     0x35bbdb6b: types.KeyboardButtonCallback,
     0xb16a6c29: types.KeyboardButtonRequestPhone,
     0xfc796b3f: types.KeyboardButtonRequestGeoLocation,
-    0x0568a748: types.KeyboardButtonSwitchInline,
+    0x93b9fbb5: types.KeyboardButtonSwitchInline,
     0x50f41ccf: types.KeyboardButtonGame,
     0xafd93fbb: types.KeyboardButtonBuy,
     0x10b78d29: types.KeyboardButtonUrlAuth,
     0xd02e7fd4: types.InputKeyboardButtonUrlAuth,
     0xbbc7515d: types.KeyboardButtonRequestPoll,
     0xe988037b: types.InputKeyboardButtonUserProfile,
     0x308660c1: types.KeyboardButtonUserProfile,
@@ -577,15 +579,15 @@
     0xd61ad6ee: types.auth.CodeTypeMissedCall,
     0x06ed998c: types.auth.CodeTypeFragmentSms,
     0x3dbb5986: types.auth.SentCodeTypeApp,
     0xc000bba2: types.auth.SentCodeTypeSms,
     0x5353e5a7: types.auth.SentCodeTypeCall,
     0xab03c6d9: types.auth.SentCodeTypeFlashCall,
     0x82006484: types.auth.SentCodeTypeMissedCall,
-    0x5a159841: types.auth.SentCodeTypeEmailCode,
+    0xf450f59b: types.auth.SentCodeTypeEmailCode,
     0xa5491dea: types.auth.SentCodeTypeSetUpEmailRequired,
     0xd9565c39: types.auth.SentCodeTypeFragmentSms,
     0xe57b1432: types.auth.SentCodeTypeFirebaseSms,
     0x36585ea4: types.messages.BotCallbackAnswer,
     0x26b5dde6: types.messages.MessageEditData,
     0x890c3d89: types.InputBotInlineMessageID,
     0xb6d915d7: types.InputBotInlineMessageID64,
@@ -743,15 +745,15 @@
     0x0e6b76ae: types.ChannelAdminLogEventActionChangeLocation,
     0x53909779: types.ChannelAdminLogEventActionToggleSlowMode,
     0x23209745: types.ChannelAdminLogEventActionStartGroupCall,
     0xdb9f9140: types.ChannelAdminLogEventActionDiscardGroupCall,
     0xf92424d2: types.ChannelAdminLogEventActionParticipantMute,
     0xe64429c0: types.ChannelAdminLogEventActionParticipantUnmute,
     0x56d6a247: types.ChannelAdminLogEventActionToggleGroupCallSetting,
-    0x5cdada77: types.ChannelAdminLogEventActionParticipantJoinByInvite,
+    0xfe9fc158: types.ChannelAdminLogEventActionParticipantJoinByInvite,
     0x5a50fca4: types.ChannelAdminLogEventActionExportedInviteDelete,
     0x410a134e: types.ChannelAdminLogEventActionExportedInviteRevoke,
     0xe90ebb59: types.ChannelAdminLogEventActionExportedInviteEdit,
     0x3e7f6847: types.ChannelAdminLogEventActionParticipantVolume,
     0x6e941a38: types.ChannelAdminLogEventActionChangeHistoryTTL,
     0xafb6144a: types.ChannelAdminLogEventActionParticipantJoinByRequest,
     0xcb2ac766: types.ChannelAdminLogEventActionToggleNoForwards,
@@ -920,14 +922,15 @@
     0x3ca5b0ec: types.MessageUserVoteInputOption,
     0x8a65e557: types.MessageUserVoteMultiple,
     0x0823f649: types.messages.VotesList,
     0xf568028a: types.BankCardOpenUrl,
     0x3e24e573: types.payments.BankCardData,
     0x7438f7e8: types.DialogFilter,
     0x363293ae: types.DialogFilterDefault,
+    0xd64a04a8: types.DialogFilterChatlist,
     0x77744d4a: types.DialogFilterSuggested,
     0xb637edaf: types.StatsDateRangeDays,
     0xcb43acde: types.StatsAbsValueAndPrev,
     0xcbce2fe0: types.StatsPercentValue,
     0x4a27eb2d: types.StatsGraphAsync,
     0xbedc9822: types.StatsGraphError,
     0x8ea464b6: types.StatsGraph,
@@ -961,14 +964,15 @@
     0x9e727aad: types.phone.GroupCall,
     0xf47751b6: types.phone.GroupParticipants,
     0x3081ed9d: types.InlineQueryPeerTypeSameBotPM,
     0x833c0fac: types.InlineQueryPeerTypePM,
     0xd766c50a: types.InlineQueryPeerTypeChat,
     0x5ec4be43: types.InlineQueryPeerTypeMegagroup,
     0x6334ee9a: types.InlineQueryPeerTypeBroadcast,
+    0x0e3b2d0c: types.InlineQueryPeerTypeBotPM,
     0x1662af0b: types.messages.HistoryImport,
     0x5e0fb7b9: types.messages.HistoryImportParsed,
     0xef8d3e6c: types.messages.AffectedFoundMessages,
     0x8c5adfd9: types.ChatInviteImporter,
     0xbdc62dcc: types.messages.ExportedChatInvites,
     0x1871be50: types.messages.ExportedChatInvite,
     0x222600ef: types.messages.ExportedChatInviteReplaced,
@@ -1097,14 +1101,22 @@
     0x908c0407: types.InputBotAppShortName,
     0x5da674b7: types.BotAppNotModified,
     0x95fcd1d6: types.BotApp,
     0xeb50adf5: types.messages.BotApp,
     0x3c1b4f0d: types.AppWebViewResultUrl,
     0xb57295d5: types.InlineBotWebView,
     0x4a4ff172: types.ReadParticipantDate,
+    0xf3e0da33: types.InputChatlistDialogFilter,
+    0x0c5181ac: types.ExportedChatlistInvite,
+    0x10e6e3a6: types.chatlists.ExportedChatlistInvite,
+    0x10ab6dc7: types.chatlists.ExportedInvites,
+    0xfa87f659: types.chatlists.ChatlistInviteAlready,
+    0x1dcd839d: types.chatlists.ChatlistInvite,
+    0x93bd878d: types.chatlists.ChatlistUpdates,
+    0xe8a775b0: types.bots.BotInfo,
     0xcb9f372d: functions.InvokeAfterMsgRequest,
     0x3dc4b4f0: functions.InvokeAfterMsgsRequest,
     0xc1cd5ea9: functions.InitConnectionRequest,
     0xda9b0d0d: functions.InvokeWithLayerRequest,
     0xbf9459b7: functions.InvokeWithoutUpdatesRequest,
     0x365275f2: functions.InvokeWithMessagesRangeRequest,
     0xaca9fd2e: functions.InvokeWithTakeoutRequest,
@@ -1125,14 +1137,15 @@
     0x8e48a188: functions.auth.DropTempAuthKeysRequest,
     0xb7e085fe: functions.auth.ExportLoginTokenRequest,
     0x95ac5ce4: functions.auth.ImportLoginTokenRequest,
     0xe894ad4d: functions.auth.AcceptLoginTokenRequest,
     0x0d36bf79: functions.auth.CheckRecoveryPasswordRequest,
     0x2db873a9: functions.auth.ImportWebTokenAuthorizationRequest,
     0x89464b50: functions.auth.RequestFirebaseSmsRequest,
+    0x7e960193: functions.auth.ResetLoginEmailRequest,
     0xec86017a: functions.account.RegisterDeviceRequest,
     0x6a0d3206: functions.account.UnregisterDeviceRequest,
     0x84be5b93: functions.account.UpdateNotifySettingsRequest,
     0x12b3ad31: functions.account.GetNotifySettingsRequest,
     0xdb7e1747: functions.account.ResetNotifySettingsRequest,
     0x78515775: functions.account.UpdateProfileRequest,
     0x6628562c: functions.account.UpdateStatusRequest,
@@ -1174,15 +1187,15 @@
     0x8fdf1920: functions.account.ConfirmPasswordEmailRequest,
     0x7a7f2a15: functions.account.ResendPasswordEmailRequest,
     0xc1cbd5b6: functions.account.CancelPasswordEmailRequest,
     0x9f07c728: functions.account.GetContactSignUpNotificationRequest,
     0xcff43f61: functions.account.SetContactSignUpNotificationRequest,
     0x53577479: functions.account.GetNotifyExceptionsRequest,
     0xfc8ddbea: functions.account.GetWallPaperRequest,
-    0xdd853661: functions.account.UploadWallPaperRequest,
+    0xe39a8f03: functions.account.UploadWallPaperRequest,
     0x6c5a5b37: functions.account.SaveWallPaperRequest,
     0xfeed5769: functions.account.InstallWallPaperRequest,
     0xbb3b9804: functions.account.ResetWallPapersRequest,
     0x56da0b3f: functions.account.GetAutoDownloadSettingsRequest,
     0x76f36233: functions.account.SaveAutoDownloadSettingsRequest,
     0x1c3db333: functions.account.UploadThemeRequest,
     0x652e4400: functions.account.CreateThemeRequest,
@@ -1425,19 +1438,20 @@
     0x7488ce5b: functions.messages.GetEmojiGroupsRequest,
     0x2ecd56cd: functions.messages.GetEmojiStatusGroupsRequest,
     0x21a548f3: functions.messages.GetEmojiProfilePhotoGroupsRequest,
     0x2c11c0d7: functions.messages.SearchCustomEmojiRequest,
     0xe47cb579: functions.messages.TogglePeerTranslationsRequest,
     0x34fdc5c3: functions.messages.GetBotAppRequest,
     0x8c5a3b3c: functions.messages.RequestAppWebViewRequest,
+    0x8ffacae1: functions.messages.SetChatWallPaperRequest,
     0xedd4882a: functions.updates.GetStateRequest,
     0x25939651: functions.updates.GetDifferenceRequest,
     0x03173d78: functions.updates.GetChannelDifferenceRequest,
-    0x1c3d5956: functions.photos.UpdateProfilePhotoRequest,
-    0x093c9a51: functions.photos.UploadProfilePhotoRequest,
+    0x09e82039: functions.photos.UpdateProfilePhotoRequest,
+    0x0388a3b5: functions.photos.UploadProfilePhotoRequest,
     0x87cf7f2f: functions.photos.DeletePhotosRequest,
     0x91cd32a8: functions.photos.GetUserPhotosRequest,
     0xe14c4a71: functions.photos.UploadContactProfilePhotoRequest,
     0xb304a621: functions.upload.SaveFilePartRequest,
     0xbe5335be: functions.upload.GetFileRequest,
     0xde7b673d: functions.upload.SaveBigFilePartRequest,
     0x24e6818d: functions.upload.GetWebFileRequest,
@@ -1528,16 +1542,18 @@
     0x0517165a: functions.bots.SetBotCommandsRequest,
     0x3d8de0f9: functions.bots.ResetBotCommandsRequest,
     0xe34c0dd6: functions.bots.GetBotCommandsRequest,
     0x4504d54f: functions.bots.SetBotMenuButtonRequest,
     0x9c60eb28: functions.bots.GetBotMenuButtonRequest,
     0x788464e1: functions.bots.SetBotBroadcastDefaultAdminRightsRequest,
     0x925ec9ea: functions.bots.SetBotGroupDefaultAdminRightsRequest,
-    0xa365df7a: functions.bots.SetBotInfoRequest,
-    0x75ec12e6: functions.bots.GetBotInfoRequest,
+    0x10cf3123: functions.bots.SetBotInfoRequest,
+    0xdcd914fd: functions.bots.GetBotInfoRequest,
+    0x9709b1c2: functions.bots.ReorderUsernamesRequest,
+    0x053ca973: functions.bots.ToggleUsernameRequest,
     0x37148dbb: functions.payments.GetPaymentFormRequest,
     0x2478d1cc: functions.payments.GetPaymentReceiptRequest,
     0xb6c8f12b: functions.payments.ValidateRequestedInfoRequest,
     0x2d03522f: functions.payments.SendPaymentFormRequest,
     0x227d824b: functions.payments.GetSavedInfoRequest,
     0xd83d70c1: functions.payments.ClearSavedInfoRequest,
     0x2e79d779: functions.payments.GetBankCardDataRequest,
@@ -1588,20 +1604,30 @@
     0x41248786: functions.phone.SaveCallLogRequest,
     0xf2f2330a: functions.langpack.GetLangPackRequest,
     0xefea3803: functions.langpack.GetStringsRequest,
     0xcd984aa5: functions.langpack.GetDifferenceRequest,
     0x42c6978f: functions.langpack.GetLanguagesRequest,
     0x6a596502: functions.langpack.GetLanguageRequest,
     0x6847d0ab: functions.folders.EditPeerFoldersRequest,
-    0x1c295881: functions.folders.DeleteFolderRequest,
     0xab42441a: functions.stats.GetBroadcastStatsRequest,
     0x621d5fa0: functions.stats.LoadAsyncGraphRequest,
     0xdcdf8607: functions.stats.GetMegagroupStatsRequest,
     0x5630281b: functions.stats.GetMessagePublicForwardsRequest,
     0xb6e0a3f5: functions.stats.GetMessageStatsRequest,
+    0x8472478e: functions.chatlists.ExportChatlistInviteRequest,
+    0x719c5c5e: functions.chatlists.DeleteExportedInviteRequest,
+    0x653db63d: functions.chatlists.EditExportedInviteRequest,
+    0xce03da83: functions.chatlists.GetExportedInvitesRequest,
+    0x41c10fff: functions.chatlists.CheckChatlistInviteRequest,
+    0xa6b1e39a: functions.chatlists.JoinChatlistInviteRequest,
+    0x89419521: functions.chatlists.GetChatlistUpdatesRequest,
+    0xe089f8f5: functions.chatlists.JoinChatlistUpdatesRequest,
+    0x66e486fb: functions.chatlists.HideChatlistUpdatesRequest,
+    0xfdbcd714: functions.chatlists.GetLeaveChatlistSuggestionsRequest,
+    0x74fae13a: functions.chatlists.LeaveChatlistRequest,
     0x05162463: types.ResPQ,
     0x83c95aec: types.PQInnerData,
     0xa9f55f95: types.PQInnerDataDc,
     0x3c6a84d4: types.PQInnerDataTemp,
     0x56fddf88: types.PQInnerDataTempDc,
     0x75a3f765: types.BindAuthKeyInner,
     0x79cb045d: types.ServerDHParamsFail,
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/core/__init__.py` & `tulir-telethon-1.29.0a1/telethon/tl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/core/gzippacked.py` & `tulir-telethon-1.29.0a1/telethon/tl/core/gzippacked.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/core/messagecontainer.py` & `tulir-telethon-1.29.0a1/telethon/tl/core/messagecontainer.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/core/rpcresult.py` & `tulir-telethon-1.29.0a1/telethon/tl/core/rpcresult.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/core/tlmessage.py` & `tulir-telethon-1.29.0a1/telethon/tl/core/tlmessage.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/adminlogevent.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/adminlogevent.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/button.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/button.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/chatgetter.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/chatgetter.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,17 @@
         some cases.
 
         Note that this might not be available if the library doesn't
         have enough information available.
         """
         if self._input_chat is None and self._chat_peer and self._client:
             try:
-                self._input_chat = self._client._entity_cache[self._chat_peer]
-            except KeyError:
+                self._input_chat = self._client._mb_entity_cache.get(
+                        utils.get_peer_id(self._chat_peer, add_mark=False))._as_input_peer()
+            except AttributeError:
                 pass
 
         return self._input_chat
 
     async def get_input_chat(self):
         """
         Returns `input_chat`, but will make an API call to find the
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/conversation.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/conversation.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/dialog.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/dialog.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/draft.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/draft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 
 from .. import TLObject
 from ..functions.messages import SaveDraftRequest
 from ..types import DraftMessage
 from ...errors import RPCError
 from ...extensions import markdown
-from ...utils import get_input_peer, get_peer
+from ...utils import get_input_peer, get_peer, get_peer_id
 
 
 class Draft:
     """
     Custom class that encapsulates a draft on the Telegram servers, providing
     an abstraction to change the message conveniently. The library will return
     instances of this class when calling :meth:`get_drafts()`.
@@ -49,16 +49,17 @@
     @property
     def input_entity(self):
         """
         Input version of the entity.
         """
         if not self._input_entity:
             try:
-                self._input_entity = self._client._entity_cache[self._peer]
-            except KeyError:
+                self._input_entity = self._client._mb_entity_cache.get(
+                        get_peer_id(self._peer, add_mark=False))._as_input_peer()
+            except AttributeError:
                 pass
 
         return self._input_entity
 
     async def get_entity(self):
         """
         Returns `entity` but will make an API call if necessary.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/file.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/file.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/forward.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
         sender_id = sender = input_sender = peer = chat = input_chat = None
         if original.from_id:
             ty = helpers._entity_type(original.from_id)
             if ty == helpers._EntityType.USER:
                 sender_id = utils.get_peer_id(original.from_id)
                 sender, input_sender = utils._get_entity_pair(
-                    sender_id, entities, client._entity_cache)
+                    sender_id, entities, client._mb_entity_cache)
 
             elif ty in (helpers._EntityType.CHAT, helpers._EntityType.CHANNEL):
                 peer = original.from_id
                 chat, input_chat = utils._get_entity_pair(
-                    utils.get_peer_id(peer), entities, client._entity_cache)
+                    utils.get_peer_id(peer), entities, client._mb_entity_cache)
 
         # This call resets the client
         ChatGetter.__init__(self, peer, chat=chat, input_chat=input_chat)
         SenderGetter.__init__(self, sender_id, sender=sender, input_sender=input_sender)
         self._client = client
 
     # TODO We could reload the message
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/inlinebuilder.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/inlinebuilder.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/inlineresult.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/inlineresult.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/inlineresults.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/inlineresults.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/message.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         self._client = client
 
         # Make messages sent to ourselves outgoing unless they're forwarded.
         # This makes it consistent with official client's appearance.
         if self.peer_id == types.PeerUser(client._self_id) and not self.fwd_from:
             self.out = True
 
-        cache = client._entity_cache
+        cache = client._mb_entity_cache
 
         self._sender, self._input_sender = utils._get_entity_pair(
             self.sender_id, entities, cache)
 
         self._chat, self._input_chat = utils._get_entity_pair(
             self.chat_id, entities, cache)
 
@@ -1134,16 +1134,17 @@
                     if button.same_peer or not self.via_bot_id:
                         bot = self.input_sender
                         if not bot:
                             raise ValueError('No input sender')
                         return bot
                     else:
                         try:
-                            return self._client._entity_cache[self.via_bot_id]
-                        except KeyError:
+                            return self._client._mb_entity_cache.get(
+                                utils.resolve_id(self.via_bot_id)[0])._as_input_peer()
+                        except AttributeError:
                             raise ValueError('No input sender') from None
 
     def _document_by_attribute(self, kind, condition=None):
         """
         Helper method to return the document only if it has an attribute
         that's an instance of the given kind, and passes the condition.
         """
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/messagebutton.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/messagebutton.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/participantpermissions.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/participantpermissions.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/qrlogin.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/qrlogin.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/custom/sendergetter.py` & `tulir-telethon-1.29.0a1/telethon/tl/custom/sendergetter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import abc
 
+from ... import utils
+
 
 class SenderGetter(abc.ABC):
     """
     Helper base class that introduces the `sender`, `input_sender`
     and `sender_id` properties and `get_sender` and `get_input_sender`
     methods.
     """
@@ -65,17 +67,17 @@
         have things like username or similar, but still useful in some cases.
 
         Note that this might not be available if the library can't
         find the input chat, or if the message a broadcast on a channel.
         """
         if self._input_sender is None and self._sender_id and self._client:
             try:
-                self._input_sender = \
-                    self._client._entity_cache[self._sender_id]
-            except KeyError:
+                self._input_sender = self._client._mb_entity_cache.get(
+                        utils.resolve_id(self._sender_id)[0])._as_input_peer()
+            except AttributeError:
                 pass
         return self._input_sender
 
     async def get_input_sender(self):
         """
         Returns `input_sender`, but will make an API call to find the
         input sender unless it's already cached.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/__init__.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """File generated by TLObjects' generator. All changes will be ERASED"""
 from ...tl.tlobject import TLObject
 from ...tl.tlobject import TLRequest
 from typing import Optional, List, Union, TYPE_CHECKING
-from . import account, auth, bots, channels, contacts, folders, help, langpack, messages, payments, phone, photos, stats, stickers, updates, upload, users
+from . import account, auth, bots, channels, chatlists, contacts, folders, help, langpack, messages, payments, phone, photos, stats, stickers, updates, upload, users
 import os
 import struct
 from datetime import datetime
 if TYPE_CHECKING:
     from ...tl.types import TypeInputClientProxy, TypeJSONValue, TypeMessageRange, TypeType, TypeX
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/account.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -2659,47 +2659,53 @@
             _thumb = None
         _file_name = reader.tgread_string()
         _mime_type = reader.tgread_string()
         return cls(file=_file, file_name=_file_name, mime_type=_mime_type, thumb=_thumb)
 
 
 class UploadWallPaperRequest(TLRequest):
-    CONSTRUCTOR_ID = 0xdd853661
+    CONSTRUCTOR_ID = 0xe39a8f03
     SUBCLASS_OF_ID = 0x96a2c98b
 
-    def __init__(self, file: 'TypeInputFile', mime_type: str, settings: 'TypeWallPaperSettings'):
+    def __init__(self, file: 'TypeInputFile', mime_type: str, settings: 'TypeWallPaperSettings', for_chat: Optional[bool]=None):
         """
         :returns WallPaper: Instance of either WallPaper, WallPaperNoFile.
         """
         self.file = file
         self.mime_type = mime_type
         self.settings = settings
+        self.for_chat = for_chat
 
     def to_dict(self):
         return {
             '_': 'UploadWallPaperRequest',
             'file': self.file.to_dict() if isinstance(self.file, TLObject) else self.file,
             'mime_type': self.mime_type,
-            'settings': self.settings.to_dict() if isinstance(self.settings, TLObject) else self.settings
+            'settings': self.settings.to_dict() if isinstance(self.settings, TLObject) else self.settings,
+            'for_chat': self.for_chat
         }
 
     def _bytes(self):
         return b''.join((
-            b'a6\x85\xdd',
+            b'\x03\x8f\x9a\xe3',
+            struct.pack('<I', (0 if self.for_chat is None or self.for_chat is False else 1)),
             self.file._bytes(),
             self.serialize_bytes(self.mime_type),
             self.settings._bytes(),
         ))
 
     @classmethod
     def from_reader(cls, reader):
+        flags = reader.read_int()
+
+        _for_chat = bool(flags & 1)
         _file = reader.tgread_object()
         _mime_type = reader.tgread_string()
         _settings = reader.tgread_object()
-        return cls(file=_file, mime_type=_mime_type, settings=_settings)
+        return cls(file=_file, mime_type=_mime_type, settings=_settings, for_chat=_for_chat)
 
 
 class VerifyEmailRequest(TLRequest):
     CONSTRUCTOR_ID = 0x32da4cf
     SUBCLASS_OF_ID = 0x64833188
 
     def __init__(self, purpose: 'TypeEmailVerifyPurpose', verification: 'TypeEmailVerification'):
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/auth.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,14 +578,46 @@
         ))
 
     @classmethod
     def from_reader(cls, reader):
         return cls()
 
 
+class ResetLoginEmailRequest(TLRequest):
+    CONSTRUCTOR_ID = 0x7e960193
+    SUBCLASS_OF_ID = 0x6ce87081
+
+    def __init__(self, phone_number: str, phone_code_hash: str):
+        """
+        :returns auth.SentCode: Instance of either SentCode, SentCodeSuccess.
+        """
+        self.phone_number = phone_number
+        self.phone_code_hash = phone_code_hash
+
+    def to_dict(self):
+        return {
+            '_': 'ResetLoginEmailRequest',
+            'phone_number': self.phone_number,
+            'phone_code_hash': self.phone_code_hash
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'\x93\x01\x96~',
+            self.serialize_bytes(self.phone_number),
+            self.serialize_bytes(self.phone_code_hash),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        _phone_number = reader.tgread_string()
+        _phone_code_hash = reader.tgread_string()
+        return cls(phone_number=_phone_number, phone_code_hash=_phone_code_hash)
+
+
 class SendCodeRequest(TLRequest):
     CONSTRUCTOR_ID = 0xa677244f
     SUBCLASS_OF_ID = 0x6ce87081
 
     def __init__(self, phone_number: str, api_id: int, api_hash: str, settings: 'TypeCodeSettings'):
         """
         :returns auth.SentCode: Instance of either SentCode, SentCodeSuccess.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/bots.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/bots.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,39 +71,53 @@
     def from_reader(cls, reader):
         _scope = reader.tgread_object()
         _lang_code = reader.tgread_string()
         return cls(scope=_scope, lang_code=_lang_code)
 
 
 class GetBotInfoRequest(TLRequest):
-    CONSTRUCTOR_ID = 0x75ec12e6
-    SUBCLASS_OF_ID = 0x1d97512
+    CONSTRUCTOR_ID = 0xdcd914fd
+    SUBCLASS_OF_ID = 0xca7b2235
 
-    def __init__(self, lang_code: str):
+    def __init__(self, lang_code: str, bot: Optional['TypeInputUser']=None):
         """
-        :returns Vector<string>: This type has no constructors.
+        :returns bots.BotInfo: Instance of BotInfo.
         """
         self.lang_code = lang_code
+        self.bot = bot
+
+    async def resolve(self, client, utils):
+        if self.bot:
+            self.bot = utils.get_input_user(await client.get_input_entity(self.bot))
 
     def to_dict(self):
         return {
             '_': 'GetBotInfoRequest',
-            'lang_code': self.lang_code
+            'lang_code': self.lang_code,
+            'bot': self.bot.to_dict() if isinstance(self.bot, TLObject) else self.bot
         }
 
     def _bytes(self):
         return b''.join((
-            b'\xe6\x12\xecu',
+            b'\xfd\x14\xd9\xdc',
+            struct.pack('<I', (0 if self.bot is None or self.bot is False else 1)),
+            b'' if self.bot is None or self.bot is False else (self.bot._bytes()),
             self.serialize_bytes(self.lang_code),
         ))
 
     @classmethod
     def from_reader(cls, reader):
+        flags = reader.read_int()
+
+        if flags & 1:
+            _bot = reader.tgread_object()
+        else:
+            _bot = None
         _lang_code = reader.tgread_string()
-        return cls(lang_code=_lang_code)
+        return cls(lang_code=_lang_code, bot=_bot)
 
 
 class GetBotMenuButtonRequest(TLRequest):
     CONSTRUCTOR_ID = 0x9c60eb28
     SUBCLASS_OF_ID = 0x4c71bd3c
 
     def __init__(self, user_id: 'TypeInputUser'):
@@ -129,14 +143,54 @@
 
     @classmethod
     def from_reader(cls, reader):
         _user_id = reader.tgread_object()
         return cls(user_id=_user_id)
 
 
+class ReorderUsernamesRequest(TLRequest):
+    CONSTRUCTOR_ID = 0x9709b1c2
+    SUBCLASS_OF_ID = 0xf5b399ac
+
+    def __init__(self, bot: 'TypeInputUser', order: List[str]):
+        """
+        :returns Bool: This type has no constructors.
+        """
+        self.bot = bot
+        self.order = order
+
+    async def resolve(self, client, utils):
+        self.bot = utils.get_input_user(await client.get_input_entity(self.bot))
+
+    def to_dict(self):
+        return {
+            '_': 'ReorderUsernamesRequest',
+            'bot': self.bot.to_dict() if isinstance(self.bot, TLObject) else self.bot,
+            'order': [] if self.order is None else self.order[:]
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'\xc2\xb1\t\x97',
+            self.bot._bytes(),
+            b'\x15\xc4\xb5\x1c',struct.pack('<i', len(self.order)),b''.join(self.serialize_bytes(x) for x in self.order),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        _bot = reader.tgread_object()
+        reader.read_int()
+        _order = []
+        for _ in range(reader.read_int()):
+            _x = reader.tgread_string()
+            _order.append(_x)
+
+        return cls(bot=_bot, order=_order)
+
+
 class ResetBotCommandsRequest(TLRequest):
     CONSTRUCTOR_ID = 0x3d8de0f9
     SUBCLASS_OF_ID = 0xf5b399ac
 
     def __init__(self, scope: 'TypeBotCommandScope', lang_code: str):
         """
         :returns Bool: This type has no constructors.
@@ -291,56 +345,74 @@
     @classmethod
     def from_reader(cls, reader):
         _admin_rights = reader.tgread_object()
         return cls(admin_rights=_admin_rights)
 
 
 class SetBotInfoRequest(TLRequest):
-    CONSTRUCTOR_ID = 0xa365df7a
+    CONSTRUCTOR_ID = 0x10cf3123
     SUBCLASS_OF_ID = 0xf5b399ac
 
-    def __init__(self, lang_code: str, about: Optional[str]=None, description: Optional[str]=None):
+    def __init__(self, lang_code: str, bot: Optional['TypeInputUser']=None, name: Optional[str]=None, about: Optional[str]=None, description: Optional[str]=None):
         """
         :returns Bool: This type has no constructors.
         """
         self.lang_code = lang_code
+        self.bot = bot
+        self.name = name
         self.about = about
         self.description = description
 
+    async def resolve(self, client, utils):
+        if self.bot:
+            self.bot = utils.get_input_user(await client.get_input_entity(self.bot))
+
     def to_dict(self):
         return {
             '_': 'SetBotInfoRequest',
             'lang_code': self.lang_code,
+            'bot': self.bot.to_dict() if isinstance(self.bot, TLObject) else self.bot,
+            'name': self.name,
             'about': self.about,
             'description': self.description
         }
 
     def _bytes(self):
         return b''.join((
-            b'z\xdfe\xa3',
-            struct.pack('<I', (0 if self.about is None or self.about is False else 1) | (0 if self.description is None or self.description is False else 2)),
+            b'#1\xcf\x10',
+            struct.pack('<I', (0 if self.bot is None or self.bot is False else 4) | (0 if self.name is None or self.name is False else 8) | (0 if self.about is None or self.about is False else 1) | (0 if self.description is None or self.description is False else 2)),
+            b'' if self.bot is None or self.bot is False else (self.bot._bytes()),
             self.serialize_bytes(self.lang_code),
+            b'' if self.name is None or self.name is False else (self.serialize_bytes(self.name)),
             b'' if self.about is None or self.about is False else (self.serialize_bytes(self.about)),
             b'' if self.description is None or self.description is False else (self.serialize_bytes(self.description)),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
+        if flags & 4:
+            _bot = reader.tgread_object()
+        else:
+            _bot = None
         _lang_code = reader.tgread_string()
+        if flags & 8:
+            _name = reader.tgread_string()
+        else:
+            _name = None
         if flags & 1:
             _about = reader.tgread_string()
         else:
             _about = None
         if flags & 2:
             _description = reader.tgread_string()
         else:
             _description = None
-        return cls(lang_code=_lang_code, about=_about, description=_description)
+        return cls(lang_code=_lang_code, bot=_bot, name=_name, about=_about, description=_description)
 
 
 class SetBotMenuButtonRequest(TLRequest):
     CONSTRUCTOR_ID = 0x4504d54f
     SUBCLASS_OF_ID = 0xf5b399ac
 
     def __init__(self, user_id: 'TypeInputUser', button: 'TypeBotMenuButton'):
@@ -369,7 +441,46 @@
 
     @classmethod
     def from_reader(cls, reader):
         _user_id = reader.tgread_object()
         _button = reader.tgread_object()
         return cls(user_id=_user_id, button=_button)
 
+
+class ToggleUsernameRequest(TLRequest):
+    CONSTRUCTOR_ID = 0x53ca973
+    SUBCLASS_OF_ID = 0xf5b399ac
+
+    def __init__(self, bot: 'TypeInputUser', username: str, active: bool):
+        """
+        :returns Bool: This type has no constructors.
+        """
+        self.bot = bot
+        self.username = username
+        self.active = active
+
+    async def resolve(self, client, utils):
+        self.bot = utils.get_input_user(await client.get_input_entity(self.bot))
+
+    def to_dict(self):
+        return {
+            '_': 'ToggleUsernameRequest',
+            'bot': self.bot.to_dict() if isinstance(self.bot, TLObject) else self.bot,
+            'username': self.username,
+            'active': self.active
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b's\xa9<\x05',
+            self.bot._bytes(),
+            self.serialize_bytes(self.username),
+            b'\xb5ur\x99' if self.active else b'7\x97y\xbc',
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        _bot = reader.tgread_object()
+        _username = reader.tgread_string()
+        _active = reader.tgread_bool()
+        return cls(bot=_bot, username=_username, active=_active)
+
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/channels.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/channels.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/contacts.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/contacts.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/folders.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/folders.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,42 +6,14 @@
 import struct
 from datetime import datetime
 if TYPE_CHECKING:
     from ...tl.types import TypeInputFolderPeer
 
 
 
-class DeleteFolderRequest(TLRequest):
-    CONSTRUCTOR_ID = 0x1c295881
-    SUBCLASS_OF_ID = 0x8af52aac
-
-    def __init__(self, folder_id: int):
-        """
-        :returns Updates: Instance of either UpdatesTooLong, UpdateShortMessage, UpdateShortChatMessage, UpdateShort, UpdatesCombined, Updates, UpdateShortSentMessage.
-        """
-        self.folder_id = folder_id
-
-    def to_dict(self):
-        return {
-            '_': 'DeleteFolderRequest',
-            'folder_id': self.folder_id
-        }
-
-    def _bytes(self):
-        return b''.join((
-            b'\x81X)\x1c',
-            struct.pack('<i', self.folder_id),
-        ))
-
-    @classmethod
-    def from_reader(cls, reader):
-        _folder_id = reader.read_int()
-        return cls(folder_id=_folder_id)
-
-
 class EditPeerFoldersRequest(TLRequest):
     CONSTRUCTOR_ID = 0x6847d0ab
     SUBCLASS_OF_ID = 0x8af52aac
 
     def __init__(self, folder_peers: List['TypeInputFolderPeer']):
         """
         :returns Updates: Instance of either UpdatesTooLong, UpdateShortMessage, UpdateShortChatMessage, UpdateShort, UpdatesCombined, Updates, UpdateShortSentMessage.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/help.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/help.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/langpack.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/langpack.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/messages.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ...tl.tlobject import TLObject
 from ...tl.tlobject import TLRequest
 from typing import Optional, List, Union, TYPE_CHECKING
 import os
 import struct
 from datetime import datetime
 if TYPE_CHECKING:
-    from ...tl.types import TypeChatBannedRights, TypeChatReactions, TypeDataJSON, TypeDialogFilter, TypeInlineBotSwitchPM, TypeInlineBotWebView, TypeInputBotApp, TypeInputBotInlineMessageID, TypeInputBotInlineResult, TypeInputChatPhoto, TypeInputCheckPasswordSRP, TypeInputDialogPeer, TypeInputDocument, TypeInputEncryptedChat, TypeInputEncryptedFile, TypeInputFile, TypeInputGeoPoint, TypeInputMedia, TypeInputMessage, TypeInputPeer, TypeInputSingleMedia, TypeInputStickerSet, TypeInputStickeredMedia, TypeInputUser, TypeMessageEntity, TypeMessagesFilter, TypeReaction, TypeReplyMarkup, TypeReportReason, TypeSendMessageAction, TypeShippingOption, TypeTextWithEntities
+    from ...tl.types import TypeChatBannedRights, TypeChatReactions, TypeDataJSON, TypeDialogFilter, TypeInlineBotSwitchPM, TypeInlineBotWebView, TypeInputBotApp, TypeInputBotInlineMessageID, TypeInputBotInlineResult, TypeInputChatPhoto, TypeInputCheckPasswordSRP, TypeInputDialogPeer, TypeInputDocument, TypeInputEncryptedChat, TypeInputEncryptedFile, TypeInputFile, TypeInputGeoPoint, TypeInputMedia, TypeInputMessage, TypeInputPeer, TypeInputSingleMedia, TypeInputStickerSet, TypeInputStickeredMedia, TypeInputUser, TypeInputWallPaper, TypeMessageEntity, TypeMessagesFilter, TypeReaction, TypeReplyMarkup, TypeReportReason, TypeSendMessageAction, TypeShippingOption, TypeTextWithEntities, TypeWallPaperSettings
 
 
 
 class AcceptEncryptionRequest(TLRequest):
     CONSTRUCTOR_ID = 0x3dbc0415
     SUBCLASS_OF_ID = 0x6d28a37a
 
@@ -6756,14 +6756,70 @@
     @classmethod
     def from_reader(cls, reader):
         _peer = reader.tgread_object()
         _emoticon = reader.tgread_string()
         return cls(peer=_peer, emoticon=_emoticon)
 
 
+class SetChatWallPaperRequest(TLRequest):
+    CONSTRUCTOR_ID = 0x8ffacae1
+    SUBCLASS_OF_ID = 0x8af52aac
+
+    # noinspection PyShadowingBuiltins
+    def __init__(self, peer: 'TypeInputPeer', wallpaper: Optional['TypeInputWallPaper']=None, settings: Optional['TypeWallPaperSettings']=None, id: Optional[int]=None):
+        """
+        :returns Updates: Instance of either UpdatesTooLong, UpdateShortMessage, UpdateShortChatMessage, UpdateShort, UpdatesCombined, Updates, UpdateShortSentMessage.
+        """
+        self.peer = peer
+        self.wallpaper = wallpaper
+        self.settings = settings
+        self.id = id
+
+    async def resolve(self, client, utils):
+        self.peer = utils.get_input_peer(await client.get_input_entity(self.peer))
+
+    def to_dict(self):
+        return {
+            '_': 'SetChatWallPaperRequest',
+            'peer': self.peer.to_dict() if isinstance(self.peer, TLObject) else self.peer,
+            'wallpaper': self.wallpaper.to_dict() if isinstance(self.wallpaper, TLObject) else self.wallpaper,
+            'settings': self.settings.to_dict() if isinstance(self.settings, TLObject) else self.settings,
+            'id': self.id
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'\xe1\xca\xfa\x8f',
+            struct.pack('<I', (0 if self.wallpaper is None or self.wallpaper is False else 1) | (0 if self.settings is None or self.settings is False else 4) | (0 if self.id is None or self.id is False else 2)),
+            self.peer._bytes(),
+            b'' if self.wallpaper is None or self.wallpaper is False else (self.wallpaper._bytes()),
+            b'' if self.settings is None or self.settings is False else (self.settings._bytes()),
+            b'' if self.id is None or self.id is False else (struct.pack('<i', self.id)),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        flags = reader.read_int()
+
+        _peer = reader.tgread_object()
+        if flags & 1:
+            _wallpaper = reader.tgread_object()
+        else:
+            _wallpaper = None
+        if flags & 4:
+            _settings = reader.tgread_object()
+        else:
+            _settings = None
+        if flags & 2:
+            _id = reader.read_int()
+        else:
+            _id = None
+        return cls(peer=_peer, wallpaper=_wallpaper, settings=_settings, id=_id)
+
+
 class SetDefaultHistoryTTLRequest(TLRequest):
     CONSTRUCTOR_ID = 0x9eb51445
     SUBCLASS_OF_ID = 0xf5b399ac
 
     def __init__(self, period: int):
         """
         :returns Bool: This type has no constructors.
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/payments.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/payments.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/phone.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/phone.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/photos.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/photos.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,49 +96,58 @@
         _offset = reader.read_int()
         _max_id = reader.read_long()
         _limit = reader.read_int()
         return cls(user_id=_user_id, offset=_offset, max_id=_max_id, limit=_limit)
 
 
 class UpdateProfilePhotoRequest(TLRequest):
-    CONSTRUCTOR_ID = 0x1c3d5956
+    CONSTRUCTOR_ID = 0x9e82039
     SUBCLASS_OF_ID = 0xc292bd24
 
     # noinspection PyShadowingBuiltins
-    def __init__(self, id: 'TypeInputPhoto', fallback: Optional[bool]=None):
+    def __init__(self, id: 'TypeInputPhoto', fallback: Optional[bool]=None, bot: Optional['TypeInputUser']=None):
         """
         :returns photos.Photo: Instance of Photo.
         """
         self.id = id
         self.fallback = fallback
+        self.bot = bot
 
     async def resolve(self, client, utils):
         self.id = utils.get_input_photo(self.id)
+        if self.bot:
+            self.bot = utils.get_input_user(await client.get_input_entity(self.bot))
 
     def to_dict(self):
         return {
             '_': 'UpdateProfilePhotoRequest',
             'id': self.id.to_dict() if isinstance(self.id, TLObject) else self.id,
-            'fallback': self.fallback
+            'fallback': self.fallback,
+            'bot': self.bot.to_dict() if isinstance(self.bot, TLObject) else self.bot
         }
 
     def _bytes(self):
         return b''.join((
-            b'VY=\x1c',
-            struct.pack('<I', (0 if self.fallback is None or self.fallback is False else 1)),
+            b'9 \xe8\t',
+            struct.pack('<I', (0 if self.fallback is None or self.fallback is False else 1) | (0 if self.bot is None or self.bot is False else 2)),
+            b'' if self.bot is None or self.bot is False else (self.bot._bytes()),
             self.id._bytes(),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
         _fallback = bool(flags & 1)
+        if flags & 2:
+            _bot = reader.tgread_object()
+        else:
+            _bot = None
         _id = reader.tgread_object()
-        return cls(id=_id, fallback=_fallback)
+        return cls(id=_id, fallback=_fallback, bot=_bot)
 
 
 class UploadContactProfilePhotoRequest(TLRequest):
     CONSTRUCTOR_ID = 0xe14c4a71
     SUBCLASS_OF_ID = 0xc292bd24
 
     def __init__(self, user_id: 'TypeInputUser', suggest: Optional[bool]=None, save: Optional[bool]=None, file: Optional['TypeInputFile']=None, video: Optional['TypeInputFile']=None, video_start_ts: Optional[float]=None, video_emoji_markup: Optional['TypeVideoSize']=None):
@@ -202,52 +211,63 @@
             _video_emoji_markup = reader.tgread_object()
         else:
             _video_emoji_markup = None
         return cls(user_id=_user_id, suggest=_suggest, save=_save, file=_file, video=_video, video_start_ts=_video_start_ts, video_emoji_markup=_video_emoji_markup)
 
 
 class UploadProfilePhotoRequest(TLRequest):
-    CONSTRUCTOR_ID = 0x93c9a51
+    CONSTRUCTOR_ID = 0x388a3b5
     SUBCLASS_OF_ID = 0xc292bd24
 
-    def __init__(self, fallback: Optional[bool]=None, file: Optional['TypeInputFile']=None, video: Optional['TypeInputFile']=None, video_start_ts: Optional[float]=None, video_emoji_markup: Optional['TypeVideoSize']=None):
+    def __init__(self, fallback: Optional[bool]=None, bot: Optional['TypeInputUser']=None, file: Optional['TypeInputFile']=None, video: Optional['TypeInputFile']=None, video_start_ts: Optional[float]=None, video_emoji_markup: Optional['TypeVideoSize']=None):
         """
         :returns photos.Photo: Instance of Photo.
         """
         self.fallback = fallback
+        self.bot = bot
         self.file = file
         self.video = video
         self.video_start_ts = video_start_ts
         self.video_emoji_markup = video_emoji_markup
 
+    async def resolve(self, client, utils):
+        if self.bot:
+            self.bot = utils.get_input_user(await client.get_input_entity(self.bot))
+
     def to_dict(self):
         return {
             '_': 'UploadProfilePhotoRequest',
             'fallback': self.fallback,
+            'bot': self.bot.to_dict() if isinstance(self.bot, TLObject) else self.bot,
             'file': self.file.to_dict() if isinstance(self.file, TLObject) else self.file,
             'video': self.video.to_dict() if isinstance(self.video, TLObject) else self.video,
             'video_start_ts': self.video_start_ts,
             'video_emoji_markup': self.video_emoji_markup.to_dict() if isinstance(self.video_emoji_markup, TLObject) else self.video_emoji_markup
         }
 
     def _bytes(self):
         return b''.join((
-            b'Q\x9a<\t',
-            struct.pack('<I', (0 if self.fallback is None or self.fallback is False else 8) | (0 if self.file is None or self.file is False else 1) | (0 if self.video is None or self.video is False else 2) | (0 if self.video_start_ts is None or self.video_start_ts is False else 4) | (0 if self.video_emoji_markup is None or self.video_emoji_markup is False else 16)),
+            b'\xb5\xa3\x88\x03',
+            struct.pack('<I', (0 if self.fallback is None or self.fallback is False else 8) | (0 if self.bot is None or self.bot is False else 32) | (0 if self.file is None or self.file is False else 1) | (0 if self.video is None or self.video is False else 2) | (0 if self.video_start_ts is None or self.video_start_ts is False else 4) | (0 if self.video_emoji_markup is None or self.video_emoji_markup is False else 16)),
+            b'' if self.bot is None or self.bot is False else (self.bot._bytes()),
             b'' if self.file is None or self.file is False else (self.file._bytes()),
             b'' if self.video is None or self.video is False else (self.video._bytes()),
             b'' if self.video_start_ts is None or self.video_start_ts is False else (struct.pack('<d', self.video_start_ts)),
             b'' if self.video_emoji_markup is None or self.video_emoji_markup is False else (self.video_emoji_markup._bytes()),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
         _fallback = bool(flags & 8)
+        if flags & 32:
+            _bot = reader.tgread_object()
+        else:
+            _bot = None
         if flags & 1:
             _file = reader.tgread_object()
         else:
             _file = None
         if flags & 2:
             _video = reader.tgread_object()
         else:
@@ -256,9 +276,9 @@
             _video_start_ts = reader.read_double()
         else:
             _video_start_ts = None
         if flags & 16:
             _video_emoji_markup = reader.tgread_object()
         else:
             _video_emoji_markup = None
-        return cls(fallback=_fallback, file=_file, video=_video, video_start_ts=_video_start_ts, video_emoji_markup=_video_emoji_markup)
+        return cls(fallback=_fallback, bot=_bot, file=_file, video=_video, video_start_ts=_video_start_ts, video_emoji_markup=_video_emoji_markup)
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/stats.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/stats.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/stickers.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/stickers.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/updates.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/updates.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/upload.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/upload.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/functions/users.py` & `tulir-telethon-1.29.0a1/telethon/tl/functions/users.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/patched/__init__.py` & `tulir-telethon-1.29.0a1/telethon/tl/patched/__init__.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/tlobject.py` & `tulir-telethon-1.29.0a1/telethon/tl/tlobject.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/__init__.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """File generated by TLObjects' generator. All changes will be ERASED"""
 from ...tl.tlobject import TLObject
 from typing import Optional, List, Union, TYPE_CHECKING
-from . import account, auth, channels, contacts, help, messages, payments, phone, photos, stats, stickers, storage, updates, upload, users
+from . import account, auth, bots, channels, chatlists, contacts, help, messages, payments, phone, photos, stats, stickers, storage, updates, upload, users
 import os
 import struct
 from datetime import datetime
 if TYPE_CHECKING:
     from ...tl.types import Typefuture_salt
 
 
@@ -2834,39 +2834,45 @@
 
     @classmethod
     def from_reader(cls, reader):
         return cls()
 
 
 class ChannelAdminLogEventActionParticipantJoinByInvite(TLObject):
-    CONSTRUCTOR_ID = 0x5cdada77
+    CONSTRUCTOR_ID = 0xfe9fc158
     SUBCLASS_OF_ID = 0xb2b987f3
 
-    def __init__(self, invite: 'TypeExportedChatInvite'):
+    def __init__(self, invite: 'TypeExportedChatInvite', via_chatlist: Optional[bool]=None):
         """
         Constructor for ChannelAdminLogEventAction: Instance of either ChannelAdminLogEventActionChangeTitle, ChannelAdminLogEventActionChangeAbout, ChannelAdminLogEventActionChangeUsername, ChannelAdminLogEventActionChangePhoto, ChannelAdminLogEventActionToggleInvites, ChannelAdminLogEventActionToggleSignatures, ChannelAdminLogEventActionUpdatePinned, ChannelAdminLogEventActionEditMessage, ChannelAdminLogEventActionDeleteMessage, ChannelAdminLogEventActionParticipantJoin, ChannelAdminLogEventActionParticipantLeave, ChannelAdminLogEventActionParticipantInvite, ChannelAdminLogEventActionParticipantToggleBan, ChannelAdminLogEventActionParticipantToggleAdmin, ChannelAdminLogEventActionChangeStickerSet, ChannelAdminLogEventActionTogglePreHistoryHidden, ChannelAdminLogEventActionDefaultBannedRights, ChannelAdminLogEventActionStopPoll, ChannelAdminLogEventActionChangeLinkedChat, ChannelAdminLogEventActionChangeLocation, ChannelAdminLogEventActionToggleSlowMode, ChannelAdminLogEventActionStartGroupCall, ChannelAdminLogEventActionDiscardGroupCall, ChannelAdminLogEventActionParticipantMute, ChannelAdminLogEventActionParticipantUnmute, ChannelAdminLogEventActionToggleGroupCallSetting, ChannelAdminLogEventActionParticipantJoinByInvite, ChannelAdminLogEventActionExportedInviteDelete, ChannelAdminLogEventActionExportedInviteRevoke, ChannelAdminLogEventActionExportedInviteEdit, ChannelAdminLogEventActionParticipantVolume, ChannelAdminLogEventActionChangeHistoryTTL, ChannelAdminLogEventActionParticipantJoinByRequest, ChannelAdminLogEventActionToggleNoForwards, ChannelAdminLogEventActionSendMessage, ChannelAdminLogEventActionChangeAvailableReactions, ChannelAdminLogEventActionChangeUsernames, ChannelAdminLogEventActionToggleForum, ChannelAdminLogEventActionCreateTopic, ChannelAdminLogEventActionEditTopic, ChannelAdminLogEventActionDeleteTopic, ChannelAdminLogEventActionPinTopic, ChannelAdminLogEventActionToggleAntiSpam.
         """
         self.invite = invite
+        self.via_chatlist = via_chatlist
 
     def to_dict(self):
         return {
             '_': 'ChannelAdminLogEventActionParticipantJoinByInvite',
-            'invite': self.invite.to_dict() if isinstance(self.invite, TLObject) else self.invite
+            'invite': self.invite.to_dict() if isinstance(self.invite, TLObject) else self.invite,
+            'via_chatlist': self.via_chatlist
         }
 
     def _bytes(self):
         return b''.join((
-            b'w\xda\xda\\',
+            b'X\xc1\x9f\xfe',
+            struct.pack('<I', (0 if self.via_chatlist is None or self.via_chatlist is False else 1)),
             self.invite._bytes(),
         ))
 
     @classmethod
     def from_reader(cls, reader):
+        flags = reader.read_int()
+
+        _via_chatlist = bool(flags & 1)
         _invite = reader.tgread_object()
-        return cls(invite=_invite)
+        return cls(invite=_invite, via_chatlist=_via_chatlist)
 
 
 class ChannelAdminLogEventActionParticipantJoinByRequest(TLObject):
     CONSTRUCTOR_ID = 0xafb6144a
     SUBCLASS_OF_ID = 0xb2b987f3
 
     def __init__(self, invite: 'TypeExportedChatInvite', approved_by: int):
@@ -5137,60 +5143,63 @@
         return cls(link=_link, admin_id=_admin_id, date=_date, revoked=_revoked, permanent=_permanent, request_needed=_request_needed, start_date=_start_date, expire_date=_expire_date, usage_limit=_usage_limit, usage=_usage, requested=_requested, title=_title)
 
 
 class ChatInviteImporter(TLObject):
     CONSTRUCTOR_ID = 0x8c5adfd9
     SUBCLASS_OF_ID = 0x5312542e
 
-    def __init__(self, user_id: int, date: Optional[datetime], requested: Optional[bool]=None, about: Optional[str]=None, approved_by: Optional[int]=None):
+    def __init__(self, user_id: int, date: Optional[datetime], requested: Optional[bool]=None, via_chatlist: Optional[bool]=None, about: Optional[str]=None, approved_by: Optional[int]=None):
         """
         Constructor for ChatInviteImporter: Instance of ChatInviteImporter.
         """
         self.user_id = user_id
         self.date = date
         self.requested = requested
+        self.via_chatlist = via_chatlist
         self.about = about
         self.approved_by = approved_by
 
     def to_dict(self):
         return {
             '_': 'ChatInviteImporter',
             'user_id': self.user_id,
             'date': self.date,
             'requested': self.requested,
+            'via_chatlist': self.via_chatlist,
             'about': self.about,
             'approved_by': self.approved_by
         }
 
     def _bytes(self):
         return b''.join((
             b'\xd9\xdfZ\x8c',
-            struct.pack('<I', (0 if self.requested is None or self.requested is False else 1) | (0 if self.about is None or self.about is False else 4) | (0 if self.approved_by is None or self.approved_by is False else 2)),
+            struct.pack('<I', (0 if self.requested is None or self.requested is False else 1) | (0 if self.via_chatlist is None or self.via_chatlist is False else 8) | (0 if self.about is None or self.about is False else 4) | (0 if self.approved_by is None or self.approved_by is False else 2)),
             struct.pack('<q', self.user_id),
             self.serialize_datetime(self.date),
             b'' if self.about is None or self.about is False else (self.serialize_bytes(self.about)),
             b'' if self.approved_by is None or self.approved_by is False else (struct.pack('<q', self.approved_by)),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
         _requested = bool(flags & 1)
+        _via_chatlist = bool(flags & 8)
         _user_id = reader.read_long()
         _date = reader.tgread_date()
         if flags & 4:
             _about = reader.tgread_string()
         else:
             _about = None
         if flags & 2:
             _approved_by = reader.read_long()
         else:
             _approved_by = None
-        return cls(user_id=_user_id, date=_date, requested=_requested, about=_about, approved_by=_approved_by)
+        return cls(user_id=_user_id, date=_date, requested=_requested, via_chatlist=_via_chatlist, about=_about, approved_by=_approved_by)
 
 
 class ChatInvitePeek(TLObject):
     CONSTRUCTOR_ID = 0x61695cb0
     SUBCLASS_OF_ID = 0x4561736
 
     def __init__(self, chat: 'TypeChat', expires: Optional[datetime]):
@@ -6453,15 +6462,15 @@
 class DialogFilter(TLObject):
     CONSTRUCTOR_ID = 0x7438f7e8
     SUBCLASS_OF_ID = 0x692bc457
 
     # noinspection PyShadowingBuiltins
     def __init__(self, id: int, title: str, pinned_peers: List['TypeInputPeer'], include_peers: List['TypeInputPeer'], exclude_peers: List['TypeInputPeer'], contacts: Optional[bool]=None, non_contacts: Optional[bool]=None, groups: Optional[bool]=None, broadcasts: Optional[bool]=None, bots: Optional[bool]=None, exclude_muted: Optional[bool]=None, exclude_read: Optional[bool]=None, exclude_archived: Optional[bool]=None, emoticon: Optional[str]=None):
         """
-        Constructor for DialogFilter: Instance of either DialogFilter, DialogFilterDefault.
+        Constructor for DialogFilter: Instance of either DialogFilter, DialogFilterDefault, DialogFilterChatlist.
         """
         self.id = id
         self.title = title
         self.pinned_peers = pinned_peers
         self.include_peers = include_peers
         self.exclude_peers = exclude_peers
         self.contacts = contacts
@@ -6540,14 +6549,78 @@
         for _ in range(reader.read_int()):
             _x = reader.tgread_object()
             _exclude_peers.append(_x)
 
         return cls(id=_id, title=_title, pinned_peers=_pinned_peers, include_peers=_include_peers, exclude_peers=_exclude_peers, contacts=_contacts, non_contacts=_non_contacts, groups=_groups, broadcasts=_broadcasts, bots=_bots, exclude_muted=_exclude_muted, exclude_read=_exclude_read, exclude_archived=_exclude_archived, emoticon=_emoticon)
 
 
+class DialogFilterChatlist(TLObject):
+    CONSTRUCTOR_ID = 0xd64a04a8
+    SUBCLASS_OF_ID = 0x692bc457
+
+    # noinspection PyShadowingBuiltins
+    def __init__(self, id: int, title: str, pinned_peers: List['TypeInputPeer'], include_peers: List['TypeInputPeer'], has_my_invites: Optional[bool]=None, emoticon: Optional[str]=None):
+        """
+        Constructor for DialogFilter: Instance of either DialogFilter, DialogFilterDefault, DialogFilterChatlist.
+        """
+        self.id = id
+        self.title = title
+        self.pinned_peers = pinned_peers
+        self.include_peers = include_peers
+        self.has_my_invites = has_my_invites
+        self.emoticon = emoticon
+
+    def to_dict(self):
+        return {
+            '_': 'DialogFilterChatlist',
+            'id': self.id,
+            'title': self.title,
+            'pinned_peers': [] if self.pinned_peers is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.pinned_peers],
+            'include_peers': [] if self.include_peers is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.include_peers],
+            'has_my_invites': self.has_my_invites,
+            'emoticon': self.emoticon
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'\xa8\x04J\xd6',
+            struct.pack('<I', (0 if self.has_my_invites is None or self.has_my_invites is False else 67108864) | (0 if self.emoticon is None or self.emoticon is False else 33554432)),
+            struct.pack('<i', self.id),
+            self.serialize_bytes(self.title),
+            b'' if self.emoticon is None or self.emoticon is False else (self.serialize_bytes(self.emoticon)),
+            b'\x15\xc4\xb5\x1c',struct.pack('<i', len(self.pinned_peers)),b''.join(x._bytes() for x in self.pinned_peers),
+            b'\x15\xc4\xb5\x1c',struct.pack('<i', len(self.include_peers)),b''.join(x._bytes() for x in self.include_peers),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        flags = reader.read_int()
+
+        _has_my_invites = bool(flags & 67108864)
+        _id = reader.read_int()
+        _title = reader.tgread_string()
+        if flags & 33554432:
+            _emoticon = reader.tgread_string()
+        else:
+            _emoticon = None
+        reader.read_int()
+        _pinned_peers = []
+        for _ in range(reader.read_int()):
+            _x = reader.tgread_object()
+            _pinned_peers.append(_x)
+
+        reader.read_int()
+        _include_peers = []
+        for _ in range(reader.read_int()):
+            _x = reader.tgread_object()
+            _include_peers.append(_x)
+
+        return cls(id=_id, title=_title, pinned_peers=_pinned_peers, include_peers=_include_peers, has_my_invites=_has_my_invites, emoticon=_emoticon)
+
+
 class DialogFilterDefault(TLObject):
     CONSTRUCTOR_ID = 0x363293ae
     SUBCLASS_OF_ID = 0x692bc457
 
     def to_dict(self):
         return {
             '_': 'DialogFilterDefault'
@@ -8076,14 +8149,58 @@
         _random_id = reader.read_long()
         _chat_id = reader.read_int()
         _date = reader.tgread_date()
         _bytes = reader.tgread_bytes()
         return cls(chat_id=_chat_id, date=_date, bytes=_bytes, random_id=_random_id)
 
 
+class ExportedChatlistInvite(TLObject):
+    CONSTRUCTOR_ID = 0xc5181ac
+    SUBCLASS_OF_ID = 0x7711f8ff
+
+    def __init__(self, title: str, url: str, peers: List['TypePeer']):
+        """
+        Constructor for ExportedChatlistInvite: Instance of ExportedChatlistInvite.
+        """
+        self.title = title
+        self.url = url
+        self.peers = peers
+
+    def to_dict(self):
+        return {
+            '_': 'ExportedChatlistInvite',
+            'title': self.title,
+            'url': self.url,
+            'peers': [] if self.peers is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.peers]
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'\xac\x81Q\x0c',
+            b'\0\0\0\0',
+            self.serialize_bytes(self.title),
+            self.serialize_bytes(self.url),
+            b'\x15\xc4\xb5\x1c',struct.pack('<i', len(self.peers)),b''.join(x._bytes() for x in self.peers),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        flags = reader.read_int()
+
+        _title = reader.tgread_string()
+        _url = reader.tgread_string()
+        reader.read_int()
+        _peers = []
+        for _ in range(reader.read_int()):
+            _x = reader.tgread_object()
+            _peers.append(_x)
+
+        return cls(title=_title, url=_url, peers=_peers)
+
+
 class ExportedContactToken(TLObject):
     CONSTRUCTOR_ID = 0x41bf109b
     SUBCLASS_OF_ID = 0x86ddbed1
 
     def __init__(self, url: str, expires: Optional[datetime]):
         """
         Constructor for ExportedContactToken: Instance of ExportedContactToken.
@@ -9177,14 +9294,33 @@
     @classmethod
     def from_reader(cls, reader):
         _text = reader.tgread_string()
         _url = reader.tgread_string()
         return cls(text=_text, url=_url)
 
 
+class InlineQueryPeerTypeBotPM(TLObject):
+    CONSTRUCTOR_ID = 0xe3b2d0c
+    SUBCLASS_OF_ID = 0xafb0fa1f
+
+    def to_dict(self):
+        return {
+            '_': 'InlineQueryPeerTypeBotPM'
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'\x0c-;\x0e',
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        return cls()
+
+
 class InlineQueryPeerTypeBroadcast(TLObject):
     CONSTRUCTOR_ID = 0x6334ee9a
     SUBCLASS_OF_ID = 0xafb0fa1f
 
     def to_dict(self):
         return {
             '_': 'InlineQueryPeerTypeBroadcast'
@@ -10226,14 +10362,42 @@
         if flags & 8:
             _video_emoji_markup = reader.tgread_object()
         else:
             _video_emoji_markup = None
         return cls(file=_file, video=_video, video_start_ts=_video_start_ts, video_emoji_markup=_video_emoji_markup)
 
 
+class InputChatlistDialogFilter(TLObject):
+    CONSTRUCTOR_ID = 0xf3e0da33
+    SUBCLASS_OF_ID = 0x23f9659
+
+    def __init__(self, filter_id: int):
+        """
+        Constructor for InputChatlist: Instance of InputChatlistDialogFilter.
+        """
+        self.filter_id = filter_id
+
+    def to_dict(self):
+        return {
+            '_': 'InputChatlistDialogFilter',
+            'filter_id': self.filter_id
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'3\xda\xe0\xf3',
+            struct.pack('<i', self.filter_id),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        _filter_id = reader.read_int()
+        return cls(filter_id=_filter_id)
+
+
 class InputCheckPasswordEmpty(TLObject):
     CONSTRUCTOR_ID = 0x9880f658
     SUBCLASS_OF_ID = 0xd41af560
 
     def to_dict(self):
         return {
             '_': 'InputCheckPasswordEmpty'
@@ -15545,49 +15709,61 @@
     def from_reader(cls, reader):
         _text = reader.tgread_string()
         _url = reader.tgread_string()
         return cls(text=_text, url=_url)
 
 
 class KeyboardButtonSwitchInline(TLObject):
-    CONSTRUCTOR_ID = 0x568a748
+    CONSTRUCTOR_ID = 0x93b9fbb5
     SUBCLASS_OF_ID = 0xbad74a3
 
-    def __init__(self, text: str, query: str, same_peer: Optional[bool]=None):
+    def __init__(self, text: str, query: str, same_peer: Optional[bool]=None, peer_types: Optional[List['TypeInlineQueryPeerType']]=None):
         """
         Constructor for KeyboardButton: Instance of either KeyboardButton, KeyboardButtonUrl, KeyboardButtonCallback, KeyboardButtonRequestPhone, KeyboardButtonRequestGeoLocation, KeyboardButtonSwitchInline, KeyboardButtonGame, KeyboardButtonBuy, KeyboardButtonUrlAuth, InputKeyboardButtonUrlAuth, KeyboardButtonRequestPoll, InputKeyboardButtonUserProfile, KeyboardButtonUserProfile, KeyboardButtonWebView, KeyboardButtonSimpleWebView, KeyboardButtonRequestPeer.
         """
         self.text = text
         self.query = query
         self.same_peer = same_peer
+        self.peer_types = peer_types
 
     def to_dict(self):
         return {
             '_': 'KeyboardButtonSwitchInline',
             'text': self.text,
             'query': self.query,
-            'same_peer': self.same_peer
+            'same_peer': self.same_peer,
+            'peer_types': [] if self.peer_types is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.peer_types]
         }
 
     def _bytes(self):
         return b''.join((
-            b'H\xa7h\x05',
-            struct.pack('<I', (0 if self.same_peer is None or self.same_peer is False else 1)),
+            b'\xb5\xfb\xb9\x93',
+            struct.pack('<I', (0 if self.same_peer is None or self.same_peer is False else 1) | (0 if self.peer_types is None or self.peer_types is False else 2)),
             self.serialize_bytes(self.text),
             self.serialize_bytes(self.query),
+            b'' if self.peer_types is None or self.peer_types is False else b''.join((b'\x15\xc4\xb5\x1c',struct.pack('<i', len(self.peer_types)),b''.join(x._bytes() for x in self.peer_types))),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
         _same_peer = bool(flags & 1)
         _text = reader.tgread_string()
         _query = reader.tgread_string()
-        return cls(text=_text, query=_query, same_peer=_same_peer)
+        if flags & 2:
+            reader.read_int()
+            _peer_types = []
+            for _ in range(reader.read_int()):
+                _x = reader.tgread_object()
+                _peer_types.append(_x)
+
+        else:
+            _peer_types = None
+        return cls(text=_text, query=_query, same_peer=_same_peer, peer_types=_peer_types)
 
 
 class KeyboardButtonUrl(TLObject):
     CONSTRUCTOR_ID = 0x258aff05
     SUBCLASS_OF_ID = 0xbad74a3
 
     def __init__(self, text: str, url: str):
@@ -16245,15 +16421,15 @@
 
 class MessageActionBotAllowed(TLObject):
     CONSTRUCTOR_ID = 0xc516d679
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, attach_menu: Optional[bool]=None, domain: Optional[str]=None, app: Optional['TypeBotApp']=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.attach_menu = attach_menu
         self.domain = domain
         self.app = app
 
     def to_dict(self):
         return {
@@ -16289,15 +16465,15 @@
 
 class MessageActionChannelCreate(TLObject):
     CONSTRUCTOR_ID = 0x95d2ac92
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, title: str):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.title = title
 
     def to_dict(self):
         return {
             '_': 'MessageActionChannelCreate',
             'title': self.title
@@ -16317,15 +16493,15 @@
 
 class MessageActionChannelMigrateFrom(TLObject):
     CONSTRUCTOR_ID = 0xea3948e9
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, title: str, chat_id: int):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.title = title
         self.chat_id = chat_id
 
     def to_dict(self):
         return {
             '_': 'MessageActionChannelMigrateFrom',
@@ -16349,15 +16525,15 @@
 
 class MessageActionChatAddUser(TLObject):
     CONSTRUCTOR_ID = 0x15cefd00
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, users: List[int]):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.users = users
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatAddUser',
             'users': [] if self.users is None else self.users[:]
@@ -16382,15 +16558,15 @@
 
 class MessageActionChatCreate(TLObject):
     CONSTRUCTOR_ID = 0xbd47cbad
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, title: str, users: List[int]):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.title = title
         self.users = users
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatCreate',
@@ -16438,15 +16614,15 @@
 
 class MessageActionChatDeleteUser(TLObject):
     CONSTRUCTOR_ID = 0xa43f30cc
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, user_id: int):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.user_id = user_id
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatDeleteUser',
             'user_id': self.user_id
@@ -16466,15 +16642,15 @@
 
 class MessageActionChatEditPhoto(TLObject):
     CONSTRUCTOR_ID = 0x7fcb13a8
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, photo: 'TypePhoto'):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.photo = photo
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatEditPhoto',
             'photo': self.photo.to_dict() if isinstance(self.photo, TLObject) else self.photo
@@ -16494,15 +16670,15 @@
 
 class MessageActionChatEditTitle(TLObject):
     CONSTRUCTOR_ID = 0xb5a1ce5a
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, title: str):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.title = title
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatEditTitle',
             'title': self.title
@@ -16522,15 +16698,15 @@
 
 class MessageActionChatJoinedByLink(TLObject):
     CONSTRUCTOR_ID = 0x31224c3
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, inviter_id: int):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.inviter_id = inviter_id
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatJoinedByLink',
             'inviter_id': self.inviter_id
@@ -16569,15 +16745,15 @@
 
 class MessageActionChatMigrateTo(TLObject):
     CONSTRUCTOR_ID = 0xe1037f92
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, channel_id: int):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.channel_id = channel_id
 
     def to_dict(self):
         return {
             '_': 'MessageActionChatMigrateTo',
             'channel_id': self.channel_id
@@ -16616,15 +16792,15 @@
 
 class MessageActionCustomAction(TLObject):
     CONSTRUCTOR_ID = 0xfae69f56
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, message: str):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.message = message
 
     def to_dict(self):
         return {
             '_': 'MessageActionCustomAction',
             'message': self.message
@@ -16663,15 +16839,15 @@
 
 class MessageActionGameScore(TLObject):
     CONSTRUCTOR_ID = 0x92a72876
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, game_id: int, score: int):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.game_id = game_id
         self.score = score
 
     def to_dict(self):
         return {
             '_': 'MessageActionGameScore',
@@ -16695,15 +16871,15 @@
 
 class MessageActionGeoProximityReached(TLObject):
     CONSTRUCTOR_ID = 0x98e0d697
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, from_id: 'TypePeer', to_id: 'TypePeer', distance: int):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.from_id = from_id
         self.to_id = to_id
         self.distance = distance
 
     def to_dict(self):
         return {
@@ -16726,56 +16902,74 @@
         _from_id = reader.tgread_object()
         _to_id = reader.tgread_object()
         _distance = reader.read_int()
         return cls(from_id=_from_id, to_id=_to_id, distance=_distance)
 
 
 class MessageActionGiftPremium(TLObject):
-    CONSTRUCTOR_ID = 0xaba0f5c6
+    CONSTRUCTOR_ID = 0xc83d6aec
     SUBCLASS_OF_ID = 0x8680d126
 
-    def __init__(self, currency: str, amount: int, months: int):
+    def __init__(self, currency: str, amount: int, months: int, crypto_currency: Optional[str]=None, crypto_amount: Optional[int]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.currency = currency
         self.amount = amount
         self.months = months
+        self.crypto_currency = crypto_currency
+        self.crypto_amount = crypto_amount
 
     def to_dict(self):
         return {
             '_': 'MessageActionGiftPremium',
             'currency': self.currency,
             'amount': self.amount,
-            'months': self.months
+            'months': self.months,
+            'crypto_currency': self.crypto_currency,
+            'crypto_amount': self.crypto_amount
         }
 
     def _bytes(self):
+        assert ((self.crypto_currency or self.crypto_currency is not None) and (self.crypto_amount or self.crypto_amount is not None)) or ((self.crypto_currency is None or self.crypto_currency is False) and (self.crypto_amount is None or self.crypto_amount is False)), 'crypto_currency, crypto_amount parameters must all be False-y (like None) or all me True-y'
         return b''.join((
-            b'\xc6\xf5\xa0\xab',
+            b'\xecj=\xc8',
+            struct.pack('<I', (0 if self.crypto_currency is None or self.crypto_currency is False else 1) | (0 if self.crypto_amount is None or self.crypto_amount is False else 1)),
             self.serialize_bytes(self.currency),
             struct.pack('<q', self.amount),
             struct.pack('<i', self.months),
+            b'' if self.crypto_currency is None or self.crypto_currency is False else (self.serialize_bytes(self.crypto_currency)),
+            b'' if self.crypto_amount is None or self.crypto_amount is False else (struct.pack('<q', self.crypto_amount)),
         ))
 
     @classmethod
     def from_reader(cls, reader):
+        flags = reader.read_int()
+
         _currency = reader.tgread_string()
         _amount = reader.read_long()
         _months = reader.read_int()
-        return cls(currency=_currency, amount=_amount, months=_months)
+        if flags & 1:
+            _crypto_currency = reader.tgread_string()
+        else:
+            _crypto_currency = None
+        if flags & 1:
+            _crypto_amount = reader.read_long()
+        else:
+            _crypto_amount = None
+        return cls(currency=_currency, amount=_amount, months=_months, crypto_currency=_crypto_currency, crypto_amount=_crypto_amount)
 
 
 class MessageActionGroupCall(TLObject):
     CONSTRUCTOR_ID = 0x7a0d7f42
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, call: 'TypeInputGroupCall', duration: Optional[int]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.call = call
         self.duration = duration
 
     def to_dict(self):
         return {
             '_': 'MessageActionGroupCall',
@@ -16805,15 +16999,15 @@
 
 class MessageActionGroupCallScheduled(TLObject):
     CONSTRUCTOR_ID = 0xb3a07661
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, call: 'TypeInputGroupCall', schedule_date: Optional[datetime]):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.call = call
         self.schedule_date = schedule_date
 
     def to_dict(self):
         return {
             '_': 'MessageActionGroupCallScheduled',
@@ -16856,15 +17050,15 @@
 
 class MessageActionInviteToGroupCall(TLObject):
     CONSTRUCTOR_ID = 0x502f92f7
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, call: 'TypeInputGroupCall', users: List[int]):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.call = call
         self.users = users
 
     def to_dict(self):
         return {
             '_': 'MessageActionInviteToGroupCall',
@@ -16893,15 +17087,15 @@
 
 class MessageActionPaymentSent(TLObject):
     CONSTRUCTOR_ID = 0x96163f56
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, currency: str, total_amount: int, recurring_init: Optional[bool]=None, recurring_used: Optional[bool]=None, invoice_slug: Optional[str]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.currency = currency
         self.total_amount = total_amount
         self.recurring_init = recurring_init
         self.recurring_used = recurring_used
         self.invoice_slug = invoice_slug
 
@@ -16941,15 +17135,15 @@
 
 class MessageActionPaymentSentMe(TLObject):
     CONSTRUCTOR_ID = 0x8f31b327
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, currency: str, total_amount: int, payload: bytes, charge: 'TypePaymentCharge', recurring_init: Optional[bool]=None, recurring_used: Optional[bool]=None, info: Optional['TypePaymentRequestedInfo']=None, shipping_option_id: Optional[str]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.currency = currency
         self.total_amount = total_amount
         self.payload = payload
         self.charge = charge
         self.recurring_init = recurring_init
         self.recurring_used = recurring_used
@@ -17004,15 +17198,15 @@
 
 class MessageActionPhoneCall(TLObject):
     CONSTRUCTOR_ID = 0x80e11a7f
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, call_id: int, video: Optional[bool]=None, reason: Optional['TypePhoneCallDiscardReason']=None, duration: Optional[int]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.call_id = call_id
         self.video = video
         self.reason = reason
         self.duration = duration
 
     def to_dict(self):
@@ -17071,15 +17265,15 @@
 
 class MessageActionRequestedPeer(TLObject):
     CONSTRUCTOR_ID = 0xfe77345d
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, button_id: int, peer: 'TypePeer'):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.button_id = button_id
         self.peer = peer
 
     def to_dict(self):
         return {
             '_': 'MessageActionRequestedPeer',
@@ -17122,15 +17316,15 @@
 
 class MessageActionSecureValuesSent(TLObject):
     CONSTRUCTOR_ID = 0xd95c6154
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, types: List['TypeSecureValueType']):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.types = types
 
     def to_dict(self):
         return {
             '_': 'MessageActionSecureValuesSent',
             'types': [] if self.types is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.types]
@@ -17155,15 +17349,15 @@
 
 class MessageActionSecureValuesSentMe(TLObject):
     CONSTRUCTOR_ID = 0x1b287353
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, values: List['TypeSecureValue'], credentials: 'TypeSecureCredentialsEncrypted'):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.values = values
         self.credentials = credentials
 
     def to_dict(self):
         return {
             '_': 'MessageActionSecureValuesSentMe',
@@ -17192,15 +17386,15 @@
 
 class MessageActionSetChatTheme(TLObject):
     CONSTRUCTOR_ID = 0xaa786345
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, emoticon: str):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.emoticon = emoticon
 
     def to_dict(self):
         return {
             '_': 'MessageActionSetChatTheme',
             'emoticon': self.emoticon
@@ -17214,21 +17408,49 @@
 
     @classmethod
     def from_reader(cls, reader):
         _emoticon = reader.tgread_string()
         return cls(emoticon=_emoticon)
 
 
+class MessageActionSetChatWallPaper(TLObject):
+    CONSTRUCTOR_ID = 0xbc44a927
+    SUBCLASS_OF_ID = 0x8680d126
+
+    def __init__(self, wallpaper: 'TypeWallPaper'):
+        """
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
+        """
+        self.wallpaper = wallpaper
+
+    def to_dict(self):
+        return {
+            '_': 'MessageActionSetChatWallPaper',
+            'wallpaper': self.wallpaper.to_dict() if isinstance(self.wallpaper, TLObject) else self.wallpaper
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b"'\xa9D\xbc",
+            self.wallpaper._bytes(),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        _wallpaper = reader.tgread_object()
+        return cls(wallpaper=_wallpaper)
+
+
 class MessageActionSetMessagesTTL(TLObject):
     CONSTRUCTOR_ID = 0x3c134d7b
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, period: int, auto_setting_from: Optional[int]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.period = period
         self.auto_setting_from = auto_setting_from
 
     def to_dict(self):
         return {
             '_': 'MessageActionSetMessagesTTL',
@@ -17252,21 +17474,49 @@
         if flags & 1:
             _auto_setting_from = reader.read_long()
         else:
             _auto_setting_from = None
         return cls(period=_period, auto_setting_from=_auto_setting_from)
 
 
+class MessageActionSetSameChatWallPaper(TLObject):
+    CONSTRUCTOR_ID = 0xc0787d6d
+    SUBCLASS_OF_ID = 0x8680d126
+
+    def __init__(self, wallpaper: 'TypeWallPaper'):
+        """
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
+        """
+        self.wallpaper = wallpaper
+
+    def to_dict(self):
+        return {
+            '_': 'MessageActionSetSameChatWallPaper',
+            'wallpaper': self.wallpaper.to_dict() if isinstance(self.wallpaper, TLObject) else self.wallpaper
+        }
+
+    def _bytes(self):
+        return b''.join((
+            b'm}x\xc0',
+            self.wallpaper._bytes(),
+        ))
+
+    @classmethod
+    def from_reader(cls, reader):
+        _wallpaper = reader.tgread_object()
+        return cls(wallpaper=_wallpaper)
+
+
 class MessageActionSuggestProfilePhoto(TLObject):
     CONSTRUCTOR_ID = 0x57de635e
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, photo: 'TypePhoto'):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.photo = photo
 
     def to_dict(self):
         return {
             '_': 'MessageActionSuggestProfilePhoto',
             'photo': self.photo.to_dict() if isinstance(self.photo, TLObject) else self.photo
@@ -17286,15 +17536,15 @@
 
 class MessageActionTopicCreate(TLObject):
     CONSTRUCTOR_ID = 0xd999256
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, title: str, icon_color: int, icon_emoji_id: Optional[int]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.title = title
         self.icon_color = icon_color
         self.icon_emoji_id = icon_emoji_id
 
     def to_dict(self):
         return {
@@ -17328,15 +17578,15 @@
 
 class MessageActionTopicEdit(TLObject):
     CONSTRUCTOR_ID = 0xc0944820
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, title: Optional[str]=None, icon_emoji_id: Optional[int]=None, closed: Optional[bool]=None, hidden: Optional[bool]=None):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.title = title
         self.icon_emoji_id = icon_emoji_id
         self.closed = closed
         self.hidden = hidden
 
     def to_dict(self):
@@ -17383,15 +17633,15 @@
 
 class MessageActionWebViewDataSent(TLObject):
     CONSTRUCTOR_ID = 0xb4c38cb5
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, text: str):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.text = text
 
     def to_dict(self):
         return {
             '_': 'MessageActionWebViewDataSent',
             'text': self.text
@@ -17411,15 +17661,15 @@
 
 class MessageActionWebViewDataSentMe(TLObject):
     CONSTRUCTOR_ID = 0x47dd8079
     SUBCLASS_OF_ID = 0x8680d126
 
     def __init__(self, text: str, data: str):
         """
-        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer.
+        Constructor for MessageAction: Instance of either MessageActionEmpty, MessageActionChatCreate, MessageActionChatEditTitle, MessageActionChatEditPhoto, MessageActionChatDeletePhoto, MessageActionChatAddUser, MessageActionChatDeleteUser, MessageActionChatJoinedByLink, MessageActionChannelCreate, MessageActionChatMigrateTo, MessageActionChannelMigrateFrom, MessageActionPinMessage, MessageActionHistoryClear, MessageActionGameScore, MessageActionPaymentSentMe, MessageActionPaymentSent, MessageActionPhoneCall, MessageActionScreenshotTaken, MessageActionCustomAction, MessageActionBotAllowed, MessageActionSecureValuesSentMe, MessageActionSecureValuesSent, MessageActionContactSignUp, MessageActionGeoProximityReached, MessageActionGroupCall, MessageActionInviteToGroupCall, MessageActionSetMessagesTTL, MessageActionGroupCallScheduled, MessageActionSetChatTheme, MessageActionChatJoinedByRequest, MessageActionWebViewDataSentMe, MessageActionWebViewDataSent, MessageActionGiftPremium, MessageActionTopicCreate, MessageActionTopicEdit, MessageActionSuggestProfilePhoto, MessageActionRequestedPeer, MessageActionSetChatWallPaper, MessageActionSetSameChatWallPaper.
         """
         self.text = text
         self.data = data
 
     def to_dict(self):
         return {
             '_': 'MessageActionWebViewDataSentMe',
@@ -28997,58 +29247,61 @@
         return cls(channel_id=_channel_id, id=_id, views=_views)
 
 
 class UpdateChannelParticipant(TLObject):
     CONSTRUCTOR_ID = 0x985d3abb
     SUBCLASS_OF_ID = 0x9f89304e
 
-    def __init__(self, channel_id: int, date: Optional[datetime], actor_id: int, user_id: int, qts: int, prev_participant: Optional['TypeChannelParticipant']=None, new_participant: Optional['TypeChannelParticipant']=None, invite: Optional['TypeExportedChatInvite']=None):
+    def __init__(self, channel_id: int, date: Optional[datetime], actor_id: int, user_id: int, qts: int, via_chatlist: Optional[bool]=None, prev_participant: Optional['TypeChannelParticipant']=None, new_participant: Optional['TypeChannelParticipant']=None, invite: Optional['TypeExportedChatInvite']=None):
         """
         Constructor for Update: Instance of either UpdateNewMessage, UpdateMessageID, UpdateDeleteMessages, UpdateUserTyping, UpdateChatUserTyping, UpdateChatParticipants, UpdateUserStatus, UpdateUserName, UpdateNewEncryptedMessage, UpdateEncryptedChatTyping, UpdateEncryption, UpdateEncryptedMessagesRead, UpdateChatParticipantAdd, UpdateChatParticipantDelete, UpdateDcOptions, UpdateNotifySettings, UpdateServiceNotification, UpdatePrivacy, UpdateUserPhone, UpdateReadHistoryInbox, UpdateReadHistoryOutbox, UpdateWebPage, UpdateReadMessagesContents, UpdateChannelTooLong, UpdateChannel, UpdateNewChannelMessage, UpdateReadChannelInbox, UpdateDeleteChannelMessages, UpdateChannelMessageViews, UpdateChatParticipantAdmin, UpdateNewStickerSet, UpdateStickerSetsOrder, UpdateStickerSets, UpdateSavedGifs, UpdateBotInlineQuery, UpdateBotInlineSend, UpdateEditChannelMessage, UpdateBotCallbackQuery, UpdateEditMessage, UpdateInlineBotCallbackQuery, UpdateReadChannelOutbox, UpdateDraftMessage, UpdateReadFeaturedStickers, UpdateRecentStickers, UpdateConfig, UpdatePtsChanged, UpdateChannelWebPage, UpdateDialogPinned, UpdatePinnedDialogs, UpdateBotWebhookJSON, UpdateBotWebhookJSONQuery, UpdateBotShippingQuery, UpdateBotPrecheckoutQuery, UpdatePhoneCall, UpdateLangPackTooLong, UpdateLangPack, UpdateFavedStickers, UpdateChannelReadMessagesContents, UpdateContactsReset, UpdateChannelAvailableMessages, UpdateDialogUnreadMark, UpdateMessagePoll, UpdateChatDefaultBannedRights, UpdateFolderPeers, UpdatePeerSettings, UpdatePeerLocated, UpdateNewScheduledMessage, UpdateDeleteScheduledMessages, UpdateTheme, UpdateGeoLiveViewed, UpdateLoginToken, UpdateMessagePollVote, UpdateDialogFilter, UpdateDialogFilterOrder, UpdateDialogFilters, UpdatePhoneCallSignalingData, UpdateChannelMessageForwards, UpdateReadChannelDiscussionInbox, UpdateReadChannelDiscussionOutbox, UpdatePeerBlocked, UpdateChannelUserTyping, UpdatePinnedMessages, UpdatePinnedChannelMessages, UpdateChat, UpdateGroupCallParticipants, UpdateGroupCall, UpdatePeerHistoryTTL, UpdateChatParticipant, UpdateChannelParticipant, UpdateBotStopped, UpdateGroupCallConnection, UpdateBotCommands, UpdatePendingJoinRequests, UpdateBotChatInviteRequester, UpdateMessageReactions, UpdateAttachMenuBots, UpdateWebViewResultSent, UpdateBotMenuButton, UpdateSavedRingtones, UpdateTranscribedAudio, UpdateReadFeaturedEmojiStickers, UpdateUserEmojiStatus, UpdateRecentEmojiStatuses, UpdateRecentReactions, UpdateMoveStickerSetToTop, UpdateMessageExtendedMedia, UpdateChannelPinnedTopic, UpdateChannelPinnedTopics, UpdateUser, UpdateAutoSaveSettings, UpdateGroupInvitePrivacyForbidden.
         """
         self.channel_id = channel_id
         self.date = date
         self.actor_id = actor_id
         self.user_id = user_id
         self.qts = qts
+        self.via_chatlist = via_chatlist
         self.prev_participant = prev_participant
         self.new_participant = new_participant
         self.invite = invite
 
     def to_dict(self):
         return {
             '_': 'UpdateChannelParticipant',
             'channel_id': self.channel_id,
             'date': self.date,
             'actor_id': self.actor_id,
             'user_id': self.user_id,
             'qts': self.qts,
+            'via_chatlist': self.via_chatlist,
             'prev_participant': self.prev_participant.to_dict() if isinstance(self.prev_participant, TLObject) else self.prev_participant,
             'new_participant': self.new_participant.to_dict() if isinstance(self.new_participant, TLObject) else self.new_participant,
             'invite': self.invite.to_dict() if isinstance(self.invite, TLObject) else self.invite
         }
 
     def _bytes(self):
         return b''.join((
             b'\xbb:]\x98',
-            struct.pack('<I', (0 if self.prev_participant is None or self.prev_participant is False else 1) | (0 if self.new_participant is None or self.new_participant is False else 2) | (0 if self.invite is None or self.invite is False else 4)),
+            struct.pack('<I', (0 if self.via_chatlist is None or self.via_chatlist is False else 8) | (0 if self.prev_participant is None or self.prev_participant is False else 1) | (0 if self.new_participant is None or self.new_participant is False else 2) | (0 if self.invite is None or self.invite is False else 4)),
             struct.pack('<q', self.channel_id),
             self.serialize_datetime(self.date),
             struct.pack('<q', self.actor_id),
             struct.pack('<q', self.user_id),
             b'' if self.prev_participant is None or self.prev_participant is False else (self.prev_participant._bytes()),
             b'' if self.new_participant is None or self.new_participant is False else (self.new_participant._bytes()),
             b'' if self.invite is None or self.invite is False else (self.invite._bytes()),
             struct.pack('<i', self.qts),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
+        _via_chatlist = bool(flags & 8)
         _channel_id = reader.read_long()
         _date = reader.tgread_date()
         _actor_id = reader.read_long()
         _user_id = reader.read_long()
         if flags & 1:
             _prev_participant = reader.tgread_object()
         else:
@@ -29058,15 +29311,15 @@
         else:
             _new_participant = None
         if flags & 4:
             _invite = reader.tgread_object()
         else:
             _invite = None
         _qts = reader.read_int()
-        return cls(channel_id=_channel_id, date=_date, actor_id=_actor_id, user_id=_user_id, qts=_qts, prev_participant=_prev_participant, new_participant=_new_participant, invite=_invite)
+        return cls(channel_id=_channel_id, date=_date, actor_id=_actor_id, user_id=_user_id, qts=_qts, via_chatlist=_via_chatlist, prev_participant=_prev_participant, new_participant=_new_participant, invite=_invite)
 
 
 class UpdateChannelPinnedTopic(TLObject):
     CONSTRUCTOR_ID = 0x192efbe3
     SUBCLASS_OF_ID = 0x9f89304e
 
     def __init__(self, channel_id: int, topic_id: int, pinned: Optional[bool]=None):
@@ -32890,15 +33143,15 @@
 
 
 class User(TLObject):
     CONSTRUCTOR_ID = 0x8f97c628
     SUBCLASS_OF_ID = 0x2da17977
 
     # noinspection PyShadowingBuiltins
-    def __init__(self, id: int, is_self: Optional[bool]=None, contact: Optional[bool]=None, mutual_contact: Optional[bool]=None, deleted: Optional[bool]=None, bot: Optional[bool]=None, bot_chat_history: Optional[bool]=None, bot_nochats: Optional[bool]=None, verified: Optional[bool]=None, restricted: Optional[bool]=None, min: Optional[bool]=None, bot_inline_geo: Optional[bool]=None, support: Optional[bool]=None, scam: Optional[bool]=None, apply_min_photo: Optional[bool]=None, fake: Optional[bool]=None, bot_attach_menu: Optional[bool]=None, premium: Optional[bool]=None, attach_menu_enabled: Optional[bool]=None, access_hash: Optional[int]=None, first_name: Optional[str]=None, last_name: Optional[str]=None, username: Optional[str]=None, phone: Optional[str]=None, photo: Optional['TypeUserProfilePhoto']=None, status: Optional['TypeUserStatus']=None, bot_info_version: Optional[int]=None, restriction_reason: Optional[List['TypeRestrictionReason']]=None, bot_inline_placeholder: Optional[str]=None, lang_code: Optional[str]=None, emoji_status: Optional['TypeEmojiStatus']=None, usernames: Optional[List['TypeUsername']]=None):
+    def __init__(self, id: int, is_self: Optional[bool]=None, contact: Optional[bool]=None, mutual_contact: Optional[bool]=None, deleted: Optional[bool]=None, bot: Optional[bool]=None, bot_chat_history: Optional[bool]=None, bot_nochats: Optional[bool]=None, verified: Optional[bool]=None, restricted: Optional[bool]=None, min: Optional[bool]=None, bot_inline_geo: Optional[bool]=None, support: Optional[bool]=None, scam: Optional[bool]=None, apply_min_photo: Optional[bool]=None, fake: Optional[bool]=None, bot_attach_menu: Optional[bool]=None, premium: Optional[bool]=None, attach_menu_enabled: Optional[bool]=None, bot_can_edit: Optional[bool]=None, access_hash: Optional[int]=None, first_name: Optional[str]=None, last_name: Optional[str]=None, username: Optional[str]=None, phone: Optional[str]=None, photo: Optional['TypeUserProfilePhoto']=None, status: Optional['TypeUserStatus']=None, bot_info_version: Optional[int]=None, restriction_reason: Optional[List['TypeRestrictionReason']]=None, bot_inline_placeholder: Optional[str]=None, lang_code: Optional[str]=None, emoji_status: Optional['TypeEmojiStatus']=None, usernames: Optional[List['TypeUsername']]=None):
         """
         Constructor for User: Instance of either UserEmpty, User.
         """
         self.id = id
         self.is_self = is_self
         self.contact = contact
         self.mutual_contact = mutual_contact
@@ -32913,14 +33166,15 @@
         self.support = support
         self.scam = scam
         self.apply_min_photo = apply_min_photo
         self.fake = fake
         self.bot_attach_menu = bot_attach_menu
         self.premium = premium
         self.attach_menu_enabled = attach_menu_enabled
+        self.bot_can_edit = bot_can_edit
         self.access_hash = access_hash
         self.first_name = first_name
         self.last_name = last_name
         self.username = username
         self.phone = phone
         self.photo = photo
         self.status = status
@@ -32949,14 +33203,15 @@
             'support': self.support,
             'scam': self.scam,
             'apply_min_photo': self.apply_min_photo,
             'fake': self.fake,
             'bot_attach_menu': self.bot_attach_menu,
             'premium': self.premium,
             'attach_menu_enabled': self.attach_menu_enabled,
+            'bot_can_edit': self.bot_can_edit,
             'access_hash': self.access_hash,
             'first_name': self.first_name,
             'last_name': self.last_name,
             'username': self.username,
             'phone': self.phone,
             'photo': self.photo.to_dict() if isinstance(self.photo, TLObject) else self.photo,
             'status': self.status.to_dict() if isinstance(self.status, TLObject) else self.status,
@@ -32970,15 +33225,15 @@
 
     def _bytes(self):
         assert ((self.bot or self.bot is not None) and (self.bot_info_version or self.bot_info_version is not None)) or ((self.bot is None or self.bot is False) and (self.bot_info_version is None or self.bot_info_version is False)), 'bot, bot_info_version parameters must all be False-y (like None) or all me True-y'
         assert ((self.restricted or self.restricted is not None) and (self.restriction_reason or self.restriction_reason is not None)) or ((self.restricted is None or self.restricted is False) and (self.restriction_reason is None or self.restriction_reason is False)), 'restricted, restriction_reason parameters must all be False-y (like None) or all me True-y'
         return b''.join((
             b'(\xc6\x97\x8f',
             struct.pack('<I', (0 if self.is_self is None or self.is_self is False else 1024) | (0 if self.contact is None or self.contact is False else 2048) | (0 if self.mutual_contact is None or self.mutual_contact is False else 4096) | (0 if self.deleted is None or self.deleted is False else 8192) | (0 if self.bot is None or self.bot is False else 16384) | (0 if self.bot_chat_history is None or self.bot_chat_history is False else 32768) | (0 if self.bot_nochats is None or self.bot_nochats is False else 65536) | (0 if self.verified is None or self.verified is False else 131072) | (0 if self.restricted is None or self.restricted is False else 262144) | (0 if self.min is None or self.min is False else 1048576) | (0 if self.bot_inline_geo is None or self.bot_inline_geo is False else 2097152) | (0 if self.support is None or self.support is False else 8388608) | (0 if self.scam is None or self.scam is False else 16777216) | (0 if self.apply_min_photo is None or self.apply_min_photo is False else 33554432) | (0 if self.fake is None or self.fake is False else 67108864) | (0 if self.bot_attach_menu is None or self.bot_attach_menu is False else 134217728) | (0 if self.premium is None or self.premium is False else 268435456) | (0 if self.attach_menu_enabled is None or self.attach_menu_enabled is False else 536870912) | (0 if self.access_hash is None or self.access_hash is False else 1) | (0 if self.first_name is None or self.first_name is False else 2) | (0 if self.last_name is None or self.last_name is False else 4) | (0 if self.username is None or self.username is False else 8) | (0 if self.phone is None or self.phone is False else 16) | (0 if self.photo is None or self.photo is False else 32) | (0 if self.status is None or self.status is False else 64) | (0 if self.bot_info_version is None or self.bot_info_version is False else 16384) | (0 if self.restriction_reason is None or self.restriction_reason is False else 262144) | (0 if self.bot_inline_placeholder is None or self.bot_inline_placeholder is False else 524288) | (0 if self.lang_code is None or self.lang_code is False else 4194304) | (0 if self.emoji_status is None or self.emoji_status is False else 1073741824)),
-            struct.pack('<I', (0 if self.usernames is None or self.usernames is False else 1)),
+            struct.pack('<I', (0 if self.bot_can_edit is None or self.bot_can_edit is False else 2) | (0 if self.usernames is None or self.usernames is False else 1)),
             struct.pack('<q', self.id),
             b'' if self.access_hash is None or self.access_hash is False else (struct.pack('<q', self.access_hash)),
             b'' if self.first_name is None or self.first_name is False else (self.serialize_bytes(self.first_name)),
             b'' if self.last_name is None or self.last_name is False else (self.serialize_bytes(self.last_name)),
             b'' if self.username is None or self.username is False else (self.serialize_bytes(self.username)),
             b'' if self.phone is None or self.phone is False else (self.serialize_bytes(self.phone)),
             b'' if self.photo is None or self.photo is False else (self.photo._bytes()),
@@ -33011,14 +33266,15 @@
         _apply_min_photo = bool(flags & 33554432)
         _fake = bool(flags & 67108864)
         _bot_attach_menu = bool(flags & 134217728)
         _premium = bool(flags & 268435456)
         _attach_menu_enabled = bool(flags & 536870912)
         flags2 = reader.read_int()
 
+        _bot_can_edit = bool(flags2 & 2)
         _id = reader.read_long()
         if flags & 1:
             _access_hash = reader.read_long()
         else:
             _access_hash = None
         if flags & 2:
             _first_name = reader.tgread_string()
@@ -33074,15 +33330,15 @@
             _usernames = []
             for _ in range(reader.read_int()):
                 _x = reader.tgread_object()
                 _usernames.append(_x)
 
         else:
             _usernames = None
-        return cls(id=_id, is_self=_is_self, contact=_contact, mutual_contact=_mutual_contact, deleted=_deleted, bot=_bot, bot_chat_history=_bot_chat_history, bot_nochats=_bot_nochats, verified=_verified, restricted=_restricted, min=_min, bot_inline_geo=_bot_inline_geo, support=_support, scam=_scam, apply_min_photo=_apply_min_photo, fake=_fake, bot_attach_menu=_bot_attach_menu, premium=_premium, attach_menu_enabled=_attach_menu_enabled, access_hash=_access_hash, first_name=_first_name, last_name=_last_name, username=_username, phone=_phone, photo=_photo, status=_status, bot_info_version=_bot_info_version, restriction_reason=_restriction_reason, bot_inline_placeholder=_bot_inline_placeholder, lang_code=_lang_code, emoji_status=_emoji_status, usernames=_usernames)
+        return cls(id=_id, is_self=_is_self, contact=_contact, mutual_contact=_mutual_contact, deleted=_deleted, bot=_bot, bot_chat_history=_bot_chat_history, bot_nochats=_bot_nochats, verified=_verified, restricted=_restricted, min=_min, bot_inline_geo=_bot_inline_geo, support=_support, scam=_scam, apply_min_photo=_apply_min_photo, fake=_fake, bot_attach_menu=_bot_attach_menu, premium=_premium, attach_menu_enabled=_attach_menu_enabled, bot_can_edit=_bot_can_edit, access_hash=_access_hash, first_name=_first_name, last_name=_last_name, username=_username, phone=_phone, photo=_photo, status=_status, bot_info_version=_bot_info_version, restriction_reason=_restriction_reason, bot_inline_placeholder=_bot_inline_placeholder, lang_code=_lang_code, emoji_status=_emoji_status, usernames=_usernames)
 
 
 class UserEmpty(TLObject):
     CONSTRUCTOR_ID = 0xd3bc4b7a
     SUBCLASS_OF_ID = 0x2da17977
 
     # noinspection PyShadowingBuiltins
@@ -33107,19 +33363,19 @@
     @classmethod
     def from_reader(cls, reader):
         _id = reader.read_long()
         return cls(id=_id)
 
 
 class UserFull(TLObject):
-    CONSTRUCTOR_ID = 0xf8d32aed
+    CONSTRUCTOR_ID = 0x93eadb53
     SUBCLASS_OF_ID = 0x1f4661b9
 
     # noinspection PyShadowingBuiltins
-    def __init__(self, id: int, settings: 'TypePeerSettings', notify_settings: 'TypePeerNotifySettings', common_chats_count: int, blocked: Optional[bool]=None, phone_calls_available: Optional[bool]=None, phone_calls_private: Optional[bool]=None, can_pin_message: Optional[bool]=None, has_scheduled: Optional[bool]=None, video_calls_available: Optional[bool]=None, voice_messages_forbidden: Optional[bool]=None, translations_disabled: Optional[bool]=None, about: Optional[str]=None, personal_photo: Optional['TypePhoto']=None, profile_photo: Optional['TypePhoto']=None, fallback_photo: Optional['TypePhoto']=None, bot_info: Optional['TypeBotInfo']=None, pinned_msg_id: Optional[int]=None, folder_id: Optional[int]=None, ttl_period: Optional[int]=None, theme_emoticon: Optional[str]=None, private_forward_name: Optional[str]=None, bot_group_admin_rights: Optional['TypeChatAdminRights']=None, bot_broadcast_admin_rights: Optional['TypeChatAdminRights']=None, premium_gifts: Optional[List['TypePremiumGiftOption']]=None):
+    def __init__(self, id: int, settings: 'TypePeerSettings', notify_settings: 'TypePeerNotifySettings', common_chats_count: int, blocked: Optional[bool]=None, phone_calls_available: Optional[bool]=None, phone_calls_private: Optional[bool]=None, can_pin_message: Optional[bool]=None, has_scheduled: Optional[bool]=None, video_calls_available: Optional[bool]=None, voice_messages_forbidden: Optional[bool]=None, translations_disabled: Optional[bool]=None, about: Optional[str]=None, personal_photo: Optional['TypePhoto']=None, profile_photo: Optional['TypePhoto']=None, fallback_photo: Optional['TypePhoto']=None, bot_info: Optional['TypeBotInfo']=None, pinned_msg_id: Optional[int]=None, folder_id: Optional[int]=None, ttl_period: Optional[int]=None, theme_emoticon: Optional[str]=None, private_forward_name: Optional[str]=None, bot_group_admin_rights: Optional['TypeChatAdminRights']=None, bot_broadcast_admin_rights: Optional['TypeChatAdminRights']=None, premium_gifts: Optional[List['TypePremiumGiftOption']]=None, wallpaper: Optional['TypeWallPaper']=None):
         """
         Constructor for UserFull: Instance of UserFull.
         """
         self.id = id
         self.settings = settings
         self.notify_settings = notify_settings
         self.common_chats_count = common_chats_count
@@ -33140,14 +33396,15 @@
         self.folder_id = folder_id
         self.ttl_period = ttl_period
         self.theme_emoticon = theme_emoticon
         self.private_forward_name = private_forward_name
         self.bot_group_admin_rights = bot_group_admin_rights
         self.bot_broadcast_admin_rights = bot_broadcast_admin_rights
         self.premium_gifts = premium_gifts
+        self.wallpaper = wallpaper
 
     def to_dict(self):
         return {
             '_': 'UserFull',
             'id': self.id,
             'settings': self.settings.to_dict() if isinstance(self.settings, TLObject) else self.settings,
             'notify_settings': self.notify_settings.to_dict() if isinstance(self.notify_settings, TLObject) else self.notify_settings,
@@ -33168,21 +33425,22 @@
             'pinned_msg_id': self.pinned_msg_id,
             'folder_id': self.folder_id,
             'ttl_period': self.ttl_period,
             'theme_emoticon': self.theme_emoticon,
             'private_forward_name': self.private_forward_name,
             'bot_group_admin_rights': self.bot_group_admin_rights.to_dict() if isinstance(self.bot_group_admin_rights, TLObject) else self.bot_group_admin_rights,
             'bot_broadcast_admin_rights': self.bot_broadcast_admin_rights.to_dict() if isinstance(self.bot_broadcast_admin_rights, TLObject) else self.bot_broadcast_admin_rights,
-            'premium_gifts': [] if self.premium_gifts is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.premium_gifts]
+            'premium_gifts': [] if self.premium_gifts is None else [x.to_dict() if isinstance(x, TLObject) else x for x in self.premium_gifts],
+            'wallpaper': self.wallpaper.to_dict() if isinstance(self.wallpaper, TLObject) else self.wallpaper
         }
 
     def _bytes(self):
         return b''.join((
-            b'\xed*\xd3\xf8',
-            struct.pack('<I', (0 if self.blocked is None or self.blocked is False else 1) | (0 if self.phone_calls_available is None or self.phone_calls_available is False else 16) | (0 if self.phone_calls_private is None or self.phone_calls_private is False else 32) | (0 if self.can_pin_message is None or self.can_pin_message is False else 128) | (0 if self.has_scheduled is None or self.has_scheduled is False else 4096) | (0 if self.video_calls_available is None or self.video_calls_available is False else 8192) | (0 if self.voice_messages_forbidden is None or self.voice_messages_forbidden is False else 1048576) | (0 if self.translations_disabled is None or self.translations_disabled is False else 8388608) | (0 if self.about is None or self.about is False else 2) | (0 if self.personal_photo is None or self.personal_photo is False else 2097152) | (0 if self.profile_photo is None or self.profile_photo is False else 4) | (0 if self.fallback_photo is None or self.fallback_photo is False else 4194304) | (0 if self.bot_info is None or self.bot_info is False else 8) | (0 if self.pinned_msg_id is None or self.pinned_msg_id is False else 64) | (0 if self.folder_id is None or self.folder_id is False else 2048) | (0 if self.ttl_period is None or self.ttl_period is False else 16384) | (0 if self.theme_emoticon is None or self.theme_emoticon is False else 32768) | (0 if self.private_forward_name is None or self.private_forward_name is False else 65536) | (0 if self.bot_group_admin_rights is None or self.bot_group_admin_rights is False else 131072) | (0 if self.bot_broadcast_admin_rights is None or self.bot_broadcast_admin_rights is False else 262144) | (0 if self.premium_gifts is None or self.premium_gifts is False else 524288)),
+            b'S\xdb\xea\x93',
+            struct.pack('<I', (0 if self.blocked is None or self.blocked is False else 1) | (0 if self.phone_calls_available is None or self.phone_calls_available is False else 16) | (0 if self.phone_calls_private is None or self.phone_calls_private is False else 32) | (0 if self.can_pin_message is None or self.can_pin_message is False else 128) | (0 if self.has_scheduled is None or self.has_scheduled is False else 4096) | (0 if self.video_calls_available is None or self.video_calls_available is False else 8192) | (0 if self.voice_messages_forbidden is None or self.voice_messages_forbidden is False else 1048576) | (0 if self.translations_disabled is None or self.translations_disabled is False else 8388608) | (0 if self.about is None or self.about is False else 2) | (0 if self.personal_photo is None or self.personal_photo is False else 2097152) | (0 if self.profile_photo is None or self.profile_photo is False else 4) | (0 if self.fallback_photo is None or self.fallback_photo is False else 4194304) | (0 if self.bot_info is None or self.bot_info is False else 8) | (0 if self.pinned_msg_id is None or self.pinned_msg_id is False else 64) | (0 if self.folder_id is None or self.folder_id is False else 2048) | (0 if self.ttl_period is None or self.ttl_period is False else 16384) | (0 if self.theme_emoticon is None or self.theme_emoticon is False else 32768) | (0 if self.private_forward_name is None or self.private_forward_name is False else 65536) | (0 if self.bot_group_admin_rights is None or self.bot_group_admin_rights is False else 131072) | (0 if self.bot_broadcast_admin_rights is None or self.bot_broadcast_admin_rights is False else 262144) | (0 if self.premium_gifts is None or self.premium_gifts is False else 524288) | (0 if self.wallpaper is None or self.wallpaper is False else 16777216)),
             struct.pack('<q', self.id),
             b'' if self.about is None or self.about is False else (self.serialize_bytes(self.about)),
             self.settings._bytes(),
             b'' if self.personal_photo is None or self.personal_photo is False else (self.personal_photo._bytes()),
             b'' if self.profile_photo is None or self.profile_photo is False else (self.profile_photo._bytes()),
             b'' if self.fallback_photo is None or self.fallback_photo is False else (self.fallback_photo._bytes()),
             self.notify_settings._bytes(),
@@ -33192,14 +33450,15 @@
             b'' if self.folder_id is None or self.folder_id is False else (struct.pack('<i', self.folder_id)),
             b'' if self.ttl_period is None or self.ttl_period is False else (struct.pack('<i', self.ttl_period)),
             b'' if self.theme_emoticon is None or self.theme_emoticon is False else (self.serialize_bytes(self.theme_emoticon)),
             b'' if self.private_forward_name is None or self.private_forward_name is False else (self.serialize_bytes(self.private_forward_name)),
             b'' if self.bot_group_admin_rights is None or self.bot_group_admin_rights is False else (self.bot_group_admin_rights._bytes()),
             b'' if self.bot_broadcast_admin_rights is None or self.bot_broadcast_admin_rights is False else (self.bot_broadcast_admin_rights._bytes()),
             b'' if self.premium_gifts is None or self.premium_gifts is False else b''.join((b'\x15\xc4\xb5\x1c',struct.pack('<i', len(self.premium_gifts)),b''.join(x._bytes() for x in self.premium_gifts))),
+            b'' if self.wallpaper is None or self.wallpaper is False else (self.wallpaper._bytes()),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
         _blocked = bool(flags & 1)
@@ -33267,15 +33526,19 @@
             _premium_gifts = []
             for _ in range(reader.read_int()):
                 _x = reader.tgread_object()
                 _premium_gifts.append(_x)
 
         else:
             _premium_gifts = None
-        return cls(id=_id, settings=_settings, notify_settings=_notify_settings, common_chats_count=_common_chats_count, blocked=_blocked, phone_calls_available=_phone_calls_available, phone_calls_private=_phone_calls_private, can_pin_message=_can_pin_message, has_scheduled=_has_scheduled, video_calls_available=_video_calls_available, voice_messages_forbidden=_voice_messages_forbidden, translations_disabled=_translations_disabled, about=_about, personal_photo=_personal_photo, profile_photo=_profile_photo, fallback_photo=_fallback_photo, bot_info=_bot_info, pinned_msg_id=_pinned_msg_id, folder_id=_folder_id, ttl_period=_ttl_period, theme_emoticon=_theme_emoticon, private_forward_name=_private_forward_name, bot_group_admin_rights=_bot_group_admin_rights, bot_broadcast_admin_rights=_bot_broadcast_admin_rights, premium_gifts=_premium_gifts)
+        if flags & 16777216:
+            _wallpaper = reader.tgread_object()
+        else:
+            _wallpaper = None
+        return cls(id=_id, settings=_settings, notify_settings=_notify_settings, common_chats_count=_common_chats_count, blocked=_blocked, phone_calls_available=_phone_calls_available, phone_calls_private=_phone_calls_private, can_pin_message=_can_pin_message, has_scheduled=_has_scheduled, video_calls_available=_video_calls_available, voice_messages_forbidden=_voice_messages_forbidden, translations_disabled=_translations_disabled, about=_about, personal_photo=_personal_photo, profile_photo=_profile_photo, fallback_photo=_fallback_photo, bot_info=_bot_info, pinned_msg_id=_pinned_msg_id, folder_id=_folder_id, ttl_period=_ttl_period, theme_emoticon=_theme_emoticon, private_forward_name=_private_forward_name, bot_group_admin_rights=_bot_group_admin_rights, bot_broadcast_admin_rights=_bot_broadcast_admin_rights, premium_gifts=_premium_gifts, wallpaper=_wallpaper)
 
 
 class UserProfilePhoto(TLObject):
     CONSTRUCTOR_ID = 0x82d1f706
     SUBCLASS_OF_ID = 0xc6338f7d
 
     def __init__(self, photo_id: int, dc_id: int, has_video: Optional[bool]=None, personal: Optional[bool]=None, stripped_thumb: Optional[bytes]=None):
@@ -34389,15 +34652,15 @@
 TypeDataJSON = DataJSON
 TypeDcOption = DcOption
 TypeDefaultHistoryTTL = DefaultHistoryTTL
 TypeDestroyAuthKeyRes = Union[DestroyAuthKeyOk,DestroyAuthKeyNone,DestroyAuthKeyFail]
 TypeDestroySessionRes = Union[DestroySessionOk,DestroySessionNone]
 TypeSet_client_DH_params_answer = Union[DhGenOk,DhGenRetry,DhGenFail]
 TypeDialog = Union[Dialog,DialogFolder]
-TypeDialogFilter = Union[DialogFilter,DialogFilterDefault]
+TypeDialogFilter = Union[DialogFilter,DialogFilterDefault,DialogFilterChatlist]
 TypeDialogFilterSuggested = DialogFilterSuggested
 TypeDialogPeer = Union[DialogPeer,DialogPeerFolder]
 TypeDocument = Union[DocumentEmpty,Document]
 TypeDocumentAttribute = Union[DocumentAttributeImageSize,DocumentAttributeAnimated,DocumentAttributeSticker,DocumentAttributeVideo,DocumentAttributeAudio,DocumentAttributeFilename,DocumentAttributeHasStickers,DocumentAttributeCustomEmoji]
 TypeDraftMessage = Union[DraftMessageEmpty,DraftMessage]
 TypeEmailVerification = Union[EmailVerificationCode,EmailVerificationGoogle,EmailVerificationApple]
 TypeEmailVerifyPurpose = Union[EmailVerifyPurposeLoginSetup,EmailVerifyPurposeLoginChange,EmailVerifyPurposePassport]
@@ -34407,14 +34670,15 @@
 TypeEmojiLanguage = EmojiLanguage
 TypeEmojiList = Union[EmojiListNotModified,EmojiList]
 TypeEmojiStatus = Union[EmojiStatusEmpty,EmojiStatus,EmojiStatusUntil]
 TypeEmojiURL = EmojiURL
 TypeEncryptedChat = Union[EncryptedChatEmpty,EncryptedChatWaiting,EncryptedChatRequested,EncryptedChat,EncryptedChatDiscarded]
 TypeEncryptedFile = Union[EncryptedFileEmpty,EncryptedFile]
 TypeEncryptedMessage = Union[EncryptedMessage,EncryptedMessageService]
+TypeExportedChatlistInvite = ExportedChatlistInvite
 TypeExportedContactToken = ExportedContactToken
 TypeExportedMessageLink = ExportedMessageLink
 TypeFileHash = FileHash
 TypeFolder = Folder
 TypeFolderPeer = FolderPeer
 TypeForumTopic = Union[ForumTopicDeleted,ForumTopic]
 TypeFutureSalt = FutureSalt
@@ -34428,22 +34692,23 @@
 TypeGroupCallParticipantVideoSourceGroup = GroupCallParticipantVideoSourceGroup
 TypeGroupCallStreamChannel = GroupCallStreamChannel
 TypeHighScore = HighScore
 TypeHttpWait = HttpWait
 TypeImportedContact = ImportedContact
 TypeInlineBotSwitchPM = InlineBotSwitchPM
 TypeInlineBotWebView = InlineBotWebView
-TypeInlineQueryPeerType = Union[InlineQueryPeerTypeSameBotPM,InlineQueryPeerTypePM,InlineQueryPeerTypeChat,InlineQueryPeerTypeMegagroup,InlineQueryPeerTypeBroadcast]
+TypeInlineQueryPeerType = Union[InlineQueryPeerTypeSameBotPM,InlineQueryPeerTypePM,InlineQueryPeerTypeChat,InlineQueryPeerTypeMegagroup,InlineQueryPeerTypeBroadcast,InlineQueryPeerTypeBotPM]
 TypeInputAppEvent = InputAppEvent
 TypeInputBotApp = Union[InputBotAppID,InputBotAppShortName]
 TypeInputBotInlineMessage = Union[InputBotInlineMessageMediaAuto,InputBotInlineMessageText,InputBotInlineMessageMediaGeo,InputBotInlineMessageMediaVenue,InputBotInlineMessageMediaContact,InputBotInlineMessageGame,InputBotInlineMessageMediaInvoice]
 TypeInputBotInlineMessageID = Union[InputBotInlineMessageID,InputBotInlineMessageID64]
 TypeInputBotInlineResult = Union[InputBotInlineResult,InputBotInlineResultPhoto,InputBotInlineResultDocument,InputBotInlineResultGame]
 TypeInputChannel = Union[InputChannelEmpty,InputChannel,InputChannelFromMessage]
 TypeInputChatPhoto = Union[InputChatPhotoEmpty,InputChatUploadedPhoto,InputChatPhoto]
+TypeInputChatlist = InputChatlistDialogFilter
 TypeInputCheckPasswordSRP = Union[InputCheckPasswordEmpty,InputCheckPasswordSRP]
 TypeInputClientProxy = InputClientProxy
 TypeInputDialogPeer = Union[InputDialogPeer,InputDialogPeerFolder]
 TypeInputDocument = Union[InputDocumentEmpty,InputDocument]
 TypeInputFileLocation = Union[InputFileLocation,InputEncryptedFileLocation,InputDocumentFileLocation,InputSecureFileLocation,InputTakeoutFileLocation,InputPhotoFileLocation,InputPhotoLegacyFileLocation,InputPeerPhotoFileLocation,InputStickerSetThumb,InputGroupCallStream]
 TypeInputEncryptedChat = InputEncryptedChat
 TypeInputEncryptedFile = Union[InputEncryptedFileEmpty,InputEncryptedFileUploaded,InputEncryptedFile,InputEncryptedFileBigUploaded]
@@ -34488,15 +34753,15 @@
 TypeKeyboardButtonRow = KeyboardButtonRow
 TypeLabeledPrice = LabeledPrice
 TypeLangPackDifference = LangPackDifference
 TypeLangPackLanguage = LangPackLanguage
 TypeLangPackString = Union[LangPackString,LangPackStringPluralized,LangPackStringDeleted]
 TypeMaskCoords = MaskCoords
 TypeMessage = Union[MessageEmpty,Message,MessageService]
-TypeMessageAction = Union[MessageActionEmpty,MessageActionChatCreate,MessageActionChatEditTitle,MessageActionChatEditPhoto,MessageActionChatDeletePhoto,MessageActionChatAddUser,MessageActionChatDeleteUser,MessageActionChatJoinedByLink,MessageActionChannelCreate,MessageActionChatMigrateTo,MessageActionChannelMigrateFrom,MessageActionPinMessage,MessageActionHistoryClear,MessageActionGameScore,MessageActionPaymentSentMe,MessageActionPaymentSent,MessageActionPhoneCall,MessageActionScreenshotTaken,MessageActionCustomAction,MessageActionBotAllowed,MessageActionSecureValuesSentMe,MessageActionSecureValuesSent,MessageActionContactSignUp,MessageActionGeoProximityReached,MessageActionGroupCall,MessageActionInviteToGroupCall,MessageActionSetMessagesTTL,MessageActionGroupCallScheduled,MessageActionSetChatTheme,MessageActionChatJoinedByRequest,MessageActionWebViewDataSentMe,MessageActionWebViewDataSent,MessageActionGiftPremium,MessageActionTopicCreate,MessageActionTopicEdit,MessageActionSuggestProfilePhoto,MessageActionRequestedPeer]
+TypeMessageAction = Union[MessageActionEmpty,MessageActionChatCreate,MessageActionChatEditTitle,MessageActionChatEditPhoto,MessageActionChatDeletePhoto,MessageActionChatAddUser,MessageActionChatDeleteUser,MessageActionChatJoinedByLink,MessageActionChannelCreate,MessageActionChatMigrateTo,MessageActionChannelMigrateFrom,MessageActionPinMessage,MessageActionHistoryClear,MessageActionGameScore,MessageActionPaymentSentMe,MessageActionPaymentSent,MessageActionPhoneCall,MessageActionScreenshotTaken,MessageActionCustomAction,MessageActionBotAllowed,MessageActionSecureValuesSentMe,MessageActionSecureValuesSent,MessageActionContactSignUp,MessageActionGeoProximityReached,MessageActionGroupCall,MessageActionInviteToGroupCall,MessageActionSetMessagesTTL,MessageActionGroupCallScheduled,MessageActionSetChatTheme,MessageActionChatJoinedByRequest,MessageActionWebViewDataSentMe,MessageActionWebViewDataSent,MessageActionGiftPremium,MessageActionTopicCreate,MessageActionTopicEdit,MessageActionSuggestProfilePhoto,MessageActionRequestedPeer,MessageActionSetChatWallPaper,MessageActionSetSameChatWallPaper]
 TypeMessageExtendedMedia = Union[MessageExtendedMediaPreview,MessageExtendedMedia]
 TypeMessageFwdHeader = MessageFwdHeader
 TypeMessageInteractionCounters = MessageInteractionCounters
 TypeMessageMedia = Union[MessageMediaEmpty,MessageMediaPhoto,MessageMediaGeo,MessageMediaContact,MessageMediaUnsupported,MessageMediaDocument,MessageMediaWebPage,MessageMediaVenue,MessageMediaGame,MessageMediaInvoice,MessageMediaGeoLive,MessageMediaPoll,MessageMediaDice]
 TypeMessagePeerReaction = MessagePeerReaction
 TypeMessageRange = MessageRange
 TypeMessageReactions = MessageReactions
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/account.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/account.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/auth.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -514,59 +514,66 @@
     @classmethod
     def from_reader(cls, reader):
         _length = reader.read_int()
         return cls(length=_length)
 
 
 class SentCodeTypeEmailCode(TLObject):
-    CONSTRUCTOR_ID = 0x5a159841
+    CONSTRUCTOR_ID = 0xf450f59b
     SUBCLASS_OF_ID = 0xff5b158e
 
-    def __init__(self, email_pattern: str, length: int, apple_signin_allowed: Optional[bool]=None, google_signin_allowed: Optional[bool]=None, next_phone_login_date: Optional[datetime]=None):
+    def __init__(self, email_pattern: str, length: int, apple_signin_allowed: Optional[bool]=None, google_signin_allowed: Optional[bool]=None, reset_available_period: Optional[int]=None, reset_pending_date: Optional[datetime]=None):
         """
         Constructor for auth.SentCodeType: Instance of either SentCodeTypeApp, SentCodeTypeSms, SentCodeTypeCall, SentCodeTypeFlashCall, SentCodeTypeMissedCall, SentCodeTypeEmailCode, SentCodeTypeSetUpEmailRequired, SentCodeTypeFragmentSms, SentCodeTypeFirebaseSms.
         """
         self.email_pattern = email_pattern
         self.length = length
         self.apple_signin_allowed = apple_signin_allowed
         self.google_signin_allowed = google_signin_allowed
-        self.next_phone_login_date = next_phone_login_date
+        self.reset_available_period = reset_available_period
+        self.reset_pending_date = reset_pending_date
 
     def to_dict(self):
         return {
             '_': 'SentCodeTypeEmailCode',
             'email_pattern': self.email_pattern,
             'length': self.length,
             'apple_signin_allowed': self.apple_signin_allowed,
             'google_signin_allowed': self.google_signin_allowed,
-            'next_phone_login_date': self.next_phone_login_date
+            'reset_available_period': self.reset_available_period,
+            'reset_pending_date': self.reset_pending_date
         }
 
     def _bytes(self):
         return b''.join((
-            b'A\x98\x15Z',
-            struct.pack('<I', (0 if self.apple_signin_allowed is None or self.apple_signin_allowed is False else 1) | (0 if self.google_signin_allowed is None or self.google_signin_allowed is False else 2) | (0 if self.next_phone_login_date is None or self.next_phone_login_date is False else 4)),
+            b'\x9b\xf5P\xf4',
+            struct.pack('<I', (0 if self.apple_signin_allowed is None or self.apple_signin_allowed is False else 1) | (0 if self.google_signin_allowed is None or self.google_signin_allowed is False else 2) | (0 if self.reset_available_period is None or self.reset_available_period is False else 8) | (0 if self.reset_pending_date is None or self.reset_pending_date is False else 16)),
             self.serialize_bytes(self.email_pattern),
             struct.pack('<i', self.length),
-            b'' if self.next_phone_login_date is None or self.next_phone_login_date is False else (self.serialize_datetime(self.next_phone_login_date)),
+            b'' if self.reset_available_period is None or self.reset_available_period is False else (struct.pack('<i', self.reset_available_period)),
+            b'' if self.reset_pending_date is None or self.reset_pending_date is False else (self.serialize_datetime(self.reset_pending_date)),
         ))
 
     @classmethod
     def from_reader(cls, reader):
         flags = reader.read_int()
 
         _apple_signin_allowed = bool(flags & 1)
         _google_signin_allowed = bool(flags & 2)
         _email_pattern = reader.tgread_string()
         _length = reader.read_int()
-        if flags & 4:
-            _next_phone_login_date = reader.tgread_date()
+        if flags & 8:
+            _reset_available_period = reader.read_int()
         else:
-            _next_phone_login_date = None
-        return cls(email_pattern=_email_pattern, length=_length, apple_signin_allowed=_apple_signin_allowed, google_signin_allowed=_google_signin_allowed, next_phone_login_date=_next_phone_login_date)
+            _reset_available_period = None
+        if flags & 16:
+            _reset_pending_date = reader.tgread_date()
+        else:
+            _reset_pending_date = None
+        return cls(email_pattern=_email_pattern, length=_length, apple_signin_allowed=_apple_signin_allowed, google_signin_allowed=_google_signin_allowed, reset_available_period=_reset_available_period, reset_pending_date=_reset_pending_date)
 
 
 class SentCodeTypeFirebaseSms(TLObject):
     CONSTRUCTOR_ID = 0xe57b1432
     SUBCLASS_OF_ID = 0xff5b158e
 
     def __init__(self, length: int, nonce: Optional[bytes]=None, receipt: Optional[str]=None, push_timeout: Optional[int]=None):
```

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/channels.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/channels.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/contacts.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/contacts.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/help.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/help.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/messages.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/messages.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/payments.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/payments.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/phone.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/phone.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/photos.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/photos.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/stats.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/stats.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/stickers.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/stickers.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/storage.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/storage.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/updates.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/updates.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/upload.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/upload.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/tl/types/users.py` & `tulir-telethon-1.29.0a1/telethon/tl/types/users.py`

 * *Files identical despite different names*

### Comparing `tulir-telethon-1.28.0a9/telethon/utils.py` & `tulir-telethon-1.29.0a1/telethon/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,19 +579,22 @@
 
 
 def _get_entity_pair(entity_id, entities, cache,
                      get_input_peer=get_input_peer):
     """
     Returns ``(entity, input_entity)`` for the given entity ID.
     """
+    if not entity_id:
+        return None, None
+
     entity = entities.get(entity_id)
     try:
-        input_entity = cache[entity_id]
-    except KeyError:
-        # KeyError is unlikely, so another TypeError won't hurt
+        input_entity = cache.get(resolve_id(entity_id)[0])._as_input_peer()
+    except AttributeError:
+        # AttributeError is unlikely, so another TypeError won't hurt
         try:
             input_entity = get_input_peer(entity)
         except TypeError:
             input_entity = None
 
     return entity, input_entity
```

### Comparing `tulir-telethon-1.28.0a9/tulir_telethon.egg-info/PKG-INFO` & `tulir-telethon-1.29.0a1/tulir_telethon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tulir-telethon
-Version: 1.28.0a9
+Version: 1.29.0a1
 Summary: Full-featured Telegram client library for Python 3
 Home-page: https://github.com/tulir/Telethon
 Author: Lonami Exo
 Author-email: totufals@hotmail.com
 License: MIT
 Keywords: telegram api chat client library messaging mtproto
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -31,14 +30,16 @@
 MTProto_ library to interact with Telegram_'s API
 as a user or through a bot account (bot API alternative).
 
 .. important::
 
     If you have code using Telethon before its 1.0 version, you must
     read `Compatibility and Convenience`_ to learn how to migrate.
+    As with any third-party library for Telegram, be careful not to
+    break `Telegram's ToS`_ or `Telegram can ban the account`_.
 
 What is this?
 -------------
 
 Telegram is a popular messaging application. This library is meant
 to make it easy for you to write Python programs that can interact
 with Telegram. Think of it as a wrapper that has already done the
@@ -95,14 +96,14 @@
 in-depth explanation, with examples, troubleshooting issues, and more
 useful information.
 
 .. _asyncio: https://docs.python.org/3/library/asyncio.html
 .. _MTProto: https://core.telegram.org/mtproto
 .. _Telegram: https://telegram.org
 .. _Compatibility and Convenience: https://docs.telethon.dev/en/stable/misc/compatibility-and-convenience.html
+.. _Telegram's ToS: https://core.telegram.org/api/terms
+.. _Telegram can ban the account: https://docs.telethon.dev/en/stable/quick-references/faq.html#my-account-was-deleted-limited-when-using-the-library
 .. _Read The Docs: https://docs.telethon.dev
 
 .. |logo| image:: logo.svg
     :width: 24pt
     :height: 24pt
-
-
```

### Comparing `tulir-telethon-1.28.0a9/tulir_telethon.egg-info/SOURCES.txt` & `tulir-telethon-1.29.0a1/tulir_telethon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.py
 telethon/__init__.py
 telethon/custom.py
-telethon/entitycache.py
 telethon/functions.py
 telethon/helpers.py
 telethon/hints.py
 telethon/password.py
 telethon/requestiter.py
 telethon/sync.py
 telethon/types.py
@@ -108,14 +107,15 @@
 telethon/tl/custom/qrlogin.py
 telethon/tl/custom/sendergetter.py
 telethon/tl/functions/__init__.py
 telethon/tl/functions/account.py
 telethon/tl/functions/auth.py
 telethon/tl/functions/bots.py
 telethon/tl/functions/channels.py
+telethon/tl/functions/chatlists.py
 telethon/tl/functions/contacts.py
 telethon/tl/functions/folders.py
 telethon/tl/functions/help.py
 telethon/tl/functions/langpack.py
 telethon/tl/functions/messages.py
 telethon/tl/functions/payments.py
 telethon/tl/functions/phone.py
@@ -125,15 +125,17 @@
 telethon/tl/functions/updates.py
 telethon/tl/functions/upload.py
 telethon/tl/functions/users.py
 telethon/tl/patched/__init__.py
 telethon/tl/types/__init__.py
 telethon/tl/types/account.py
 telethon/tl/types/auth.py
+telethon/tl/types/bots.py
 telethon/tl/types/channels.py
+telethon/tl/types/chatlists.py
 telethon/tl/types/contacts.py
 telethon/tl/types/help.py
 telethon/tl/types/messages.py
 telethon/tl/types/payments.py
 telethon/tl/types/phone.py
 telethon/tl/types/photos.py
 telethon/tl/types/stats.py
```

