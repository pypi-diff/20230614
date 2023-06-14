# Comparing `tmp/spotify_lyrics_scraper-1.1.3.tar.gz` & `tmp/spotify_lyrics_scraper-1.2.0.tar.gz`

## Comparing `spotify_lyrics_scraper-1.1.3.tar` & `spotify_lyrics_scraper-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/spotify_lyrics_scraper/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/LICENSE
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/README.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.2.0/example.json
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.2.0/spotify_lyrics_scraper/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.2.0/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.2.0/PKG-INFO
```

### Comparing `spotify_lyrics_scraper-1.1.3/spotify_lyrics_scraper/__init__.py` & `spotify_lyrics_scraper-1.2.0/spotify_lyrics_scraper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import requests, time
 
-def getToken(sp_dc: str) -> dict:
+class spotifyDict(dict):
+    def formatLyrics(self, mode: int = 0): return formatLyrics(self, mode)
+
+def getToken(sp_dc: str, sp_key: str = None) -> dict:
     """
     Generates a Spotify Auth Token for searching lyrics/track IDs.\n
-    To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
+    To obtain the sp_key and sp_dc, please check the README on PyPi.
 
     Returns:
         dict - {"token": "x", "expiry": 0}\n
         dict - {"status": False, "message": "error message", "data": "data"}
     """
-
+    
     headers = {
-        "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.0.0 Safari/537.36",
+        "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36",
         "App-Platform": "WebPlayer",
         "content-type": "text/html; charset=utf-8",
-        "cookie": f"sp_dc={sp_dc}"
     }
+    cookies = {"sp_dc": sp_dc}
+    if sp_key: cookies["sp_key"] = sp_key
     
-    r = requests.get("https://open.spotify.com/get_access_token?reason=transport&productType=web_player", headers=headers)
-    
+    r = requests.get("https://open.spotify.com/get_access_token?reason=transport&productType=web_player", headers=headers, cookies=cookies)
+    print(r.json())
     if r.json()["isAnonymous"] == False: return {"token": r.json()["accessToken"], "expiry": r.json()["accessTokenExpirationTimestampMs"]}
     else: return {"status": False, "message": "Error while trying to grab Spotify token.", "data": r.text}
 
 def checkExpiry(info: dict) -> dict:
     """
     Check the expiry of your token.
 
@@ -36,28 +40,45 @@
     """
     Format the lyrics to your liking with several modes.
 
     Arguments:
         lyrics {dict} - Takes the direct output from the getLyrics function. Needs the lyrics in the base spotify format.\n
         mode {int} - Choose which mode to format the lyrics in.\n
             - 0: Lyrics Only
+            - 1: Milliseconds Start and Lyrics
+            - 2: Seconds Start and Lyrics
     """
 
     if "message" not in lyrics: return {"status": False, "message": "No lyrics were provided or they were not in the correct format."}
     if "status" in lyrics:
         if not lyrics["status"]: return {"status": False, "message": "That JSON data is invalid because the status is set to false."}
 
     toReturn = []
+    if mode == 1 or mode == 2:
+        if lyrics["message"]["lyrics"]["syncType"] != "LINE_SYNCED": return {"status": False, "message": "Timestamps do not work on songs that aren't line synced."}
+    
     if mode == 0:
-        for element in lyrics["message"]["lyrics"]["lines"]: toReturn.append(str(element["words"]).replace("\\", ""))
+        for element in lyrics["message"]["lyrics"]["lines"]:
+            if str(element["words"]) == "": continue
+            toReturn.append(str(element["words"]).replace("\\", ""))
+        return {"status": True, "message": toReturn}
+    if mode == 1:
+        for element in lyrics["message"]["lyrics"]["lines"]:
+            if str(element["words"]) == "": continue
+            toReturn.append({"milliseconds": str(element["startTimeMs"]), "line": str(element["words"]).replace("\\", "")})
+        return {"status": True, "message": toReturn}
+    if mode == 2:
+        for element in lyrics["message"]["lyrics"]["lines"]:
+            if str(element["words"]) == "": continue
+            toReturn.append({"seconds": str(round(int(element["startTimeMs"])/1000, 2)), "line": str(element["words"]).replace("\\", "")})
         return {"status": True, "message": toReturn}
 
     return {"status": False, "message": "That is not a valid format type."}
 
-def getLyrics(info: dict, trackId: str = None, songName: str = None, proxies: dict = {}) -> dict:
+def getLyrics(info: dict, trackId: str = None, songName: str = None, proxies: dict = {}) -> spotifyDict:
     """
     Search up lyrics of any given song. Uses trackId first over songName.
 
     Arguments:
         info {dict} - Information (contains token and expiry)\n
         trackId {string} - The track ID for the Spotify song to search up.\n
         songName {string} - The song name to search up.\n
@@ -88,9 +109,9 @@
         except Exception as e: return {"status": False, "message": f"Error occured: {e} - song doesn't exist?"}
 
     if trackId:
 
         try: r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers, proxies=proxies)
         except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
 
-        if '"lines"' in r.text: return {"status": True, "message": r.json()}
-        else: return {"status": False, "message": f"Could not find track/{r.text}"}
+        if '"lines"' in r.text: return spotifyDict({"status": True, "message": r.json()})
+        else: return {"status": False, "message": f"Could not find track/Spotify responded with status: {r.status_code}, text: {r.text}"}
```

### Comparing `spotify_lyrics_scraper-1.1.3/LICENSE` & `spotify_lyrics_scraper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.1.3/README.md` & `spotify_lyrics_scraper-1.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,48 @@
 # Spotify Lyrics Grabber
 This Spotify Lyrics Grabber is a tool to grab Spotify Lyrics of any song, not just the one you are listening to.
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Obtaining sp_key and sp_dc](#obtaining)
 - [Examples](#examples)
 
 ### Installation
 To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify_lyrics_scraper as spotify`
 
+### Obtaining
+To obtain the sp_dc or sp_key:
+- Open a ***new Incognito Window*** in your browser. Head to https://accounts.spotify.com/en/login?continue=https:%2F%2Fopen.spotify.com%2F
+- Open Developer Tools (CTRL+SHIFT+I or F12) and head to the "Network" tab and make sure it is recording.
+- Login to Spotify.
+- Search/Filter for `?flow_id` in the "Network" tab.
+- Under cookies for the request, you will see "sp_dc" and "sp_key".
+- Close the window ***WITHOUT LOGGING OUT*** (else said cookies will be made invalid).
+
 ### Examples
-- Always using: `import spotify_lyrics_scraper as spotify`
-- To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
+Always using: `import spotify_lyrics_scraper as spotify`
 ##### Example 1
 ```
 token = spotify.getToken("SP_DC Here")
 print(spotify.getLyrics(token, songName="Song"))
 ```
 
 ##### Example 2 (Proxies)
 ```
 token = spotify.getToken("SP_DC Here")
 print(spotify.getLyrics(token, songName="Song", proxies={"https": "https://1.1.1.1:443"}))
+```
+
+##### Example 3 (Formatting)
+```
+token = spotify.getToken("SP_DC Here")
+lyrics = spotify.getLyrics(token, songName="Song")
+if type(lyrics) == spotify.spotifyDict: print(lyrics.formatLyrics()) # there are several modes, 0/none is just lyrics, 1 is starting time in ms, 2 is starting time in seconds
+else: print(f"Error: {lyrics}")
+```
+
+##### Example 4 (sp_key)
+```
+token = spotify.getToken("SP_DC Here", "SP_Key Here") #SP Key can give you up to a year worth of spotify tokens.
+print(spotify.getLyrics(token, songName="Song"))
 ```
```

