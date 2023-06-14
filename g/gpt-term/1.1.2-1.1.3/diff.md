# Comparing `tmp/gpt-term-1.1.2.tar.gz` & `tmp/gpt-term-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.1.2.tar", last modified: Wed Jun  7 12:05:18 2023, max compression
+gzip compressed data, was "gpt-term-1.1.3.tar", last modified: Wed Jun  7 12:55:51 2023, max compression
```

## Comparing `gpt-term-1.1.2.tar` & `gpt-term-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.627585 gpt-term-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.631585 gpt-term-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 12:05:02.000000 gpt-term-1.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 12:05:02.000000 gpt-term-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 12:05:02.000000 gpt-term-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-07 12:05:18.635585 gpt-term-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.631585 gpt-term-1.1.2/README.assets/
--rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.assets/image-20230303233352970.png
--rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.assets/small.gif
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.zh-CN.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-06-07 12:05:02.000000 gpt-term-1.1.2/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/gpt_term/locale/
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.de.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.en.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.jp.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.zh_CN.yml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48430 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-07 12:05:02.000000 gpt-term-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 12:05:02.000000 gpt-term-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:05:18.635585 gpt-term-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.455803 gpt-term-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.447803 gpt-term-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.451803 gpt-term-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 12:55:39.000000 gpt-term-1.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 12:55:39.000000 gpt-term-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 12:55:39.000000 gpt-term-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-07 12:55:51.455803 gpt-term-1.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.451803 gpt-term-1.1.3/README.assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-06-07 12:55:39.000000 gpt-term-1.1.3/README.assets/image-20230303233352970.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-06-07 12:55:39.000000 gpt-term-1.1.3/README.assets/small.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-07 12:55:39.000000 gpt-term-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-07 12:55:39.000000 gpt-term-1.1.3/README.zh-CN.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-06-07 12:55:39.000000 gpt-term-1.1.3/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.455803 gpt-term-1.1.3/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.455803 gpt-term-1.1.3/gpt_term/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/locale/gpt_term.de.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/locale/gpt_term.en.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/locale/gpt_term.jp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/locale/gpt_term.zh_CN.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/locale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48384 2023-06-07 12:55:39.000000 gpt-term-1.1.3/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:51.455803 gpt-term-1.1.3/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 12:55:51.000000 gpt-term-1.1.3/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-07 12:55:39.000000 gpt-term-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 12:55:39.000000 gpt-term-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:55:51.455803 gpt-term-1.1.3/setup.cfg
```

### Comparing `gpt-term-1.1.2/.github/workflows/pypi-publish.yml` & `gpt-term-1.1.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/LICENSE` & `gpt-term-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/PKG-INFO` & `gpt-term-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.2
+Version: 1.1.3
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gpt-term-1.1.2/README.assets/image-20230303233352970.png` & `gpt-term-1.1.3/README.assets/image-20230303233352970.png`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/README.assets/small.gif` & `gpt-term-1.1.3/README.assets/small.gif`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/README.md` & `gpt-term-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/README.zh-CN.md` & `gpt-term-1.1.3/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/gpt_term/config.ini` & `gpt-term-1.1.3/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/gpt_term/locale/gpt_term.de.yml` & `gpt-term-1.1.3/gpt_term/locale/gpt_term.de.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 de:
-  welcome: "[dim]Hallo, willkommen zum Chat mit GPT. Tippen `[bright_magenta]/help[/] ein um verfügbare Befehle zu sehen."
+  welcome: "[dim]Hallo, willkommen zum Chat mit GPT. Tippen `[deep_sky_blue3]/help[/] ein um verfügbare Befehle zu sehen."
   exit: "Beenden..."
-  spent_token: "[bright_magenta]Gesamt ausgegebene Tokens: [bold]%{total_tokens_spent}"
+  spent_token: "[deep_sky_blue3]Gesamt ausgegebene Tokens: [bold]%{total_tokens_spent}"
   save_api_key: "Wirst Du API-Schlüssel in der Konfigurationsdatei speichern?"
   input_api_key: "API-Schlüssel nicht gefunden, bitte eintippen:"
-  config_key_to_shell_key: "Konfig-Element `[bright_magenta]%{key_word}[/]` ist auf [green]%{val}[/] gesetzt"
+  config_key_to_shell_key: "Konfig-Element `[deep_sky_blue3]%{key_word}[/]` ist auf [green]%{val}[/] gesetzt"
   log_level_error: "[dim]Ungültige Log-Stufe: %{e}, bitte mal config.ini Datei prüfen und die Log-stufe auf INFO setzen"
   system_prompt: "System-Prompt: "
   new_temperature: "Neue Zufälligkeit: "
   #
-  load_chat_history: "[dim]Chatverlauf erfolgreich von [bright_magenta]%{load} geladen"
+  load_chat_history: "[dim]Chatverlauf erfolgreich von [deep_sky_blue3]%{load} geladen"
   #
   code_not_found: "[dim]Code nicht gefunden"
   code_too_many_found: "[dim]Es gibt mehr als einen Code in der letzten Antwort des ChatGPTs"
   code_num: "[yellow]Code %{code_num}: "
   code_select: "Bitte wählen den Code zu kopieren aus: "
   code_index_must_int: "[red]Der Index der Codes muss eine ganze Zahl sein"
   code_index_out_range_one: "[red]Index außer Reichweite: Es gibt nur einen Code in der letzten Antwort des ChatGPTs"
   code_index_out_range_many: "[red]Index außer Reichweite: Bitte eine ganze Zahl zwischen 1 und %{len_code_list} eingeben"
   code_copy: "[dim]Der Code wurde schon in die Zwischenablage kopiert"
   code_last_copy: "[dim]Letzte Antwort wurde schon in die Zwischenablage kopiert"
-  code_copy_fail: "[dim]Keine zu tun. Verfügbarer Kopier-Befehl: `[bright_magenta]/copy code \\[index][/]` oder `[bright_magenta]/copy all[/]`"
+  code_copy_fail: "[dim]Keine zu tun. Verfügbarer Kopier-Befehl: `[deep_sky_blue3]/copy code \\[index][/]` oder `[deep_sky_blue3]/copy all[/]`"
   #
-  raw_mode_enabled: "[dim]Rhomode [green]aktiviert[/]. Benutzen `/last` um die letzte Antwort anzuzeigen."
-  raw_mode_disabled: "[dim]Rhomode [bright_red]deaktiviert[/]. Benutzen `/last` um die letzte Antwort anzuzeigen."
+  raw_mode_enabled: "[dim]Rhomode [green]aktiviert[/]. Benutzen `[deep_sky_blue3]/last[/]` um die letzte Antwort anzuzeigen."
+  raw_mode_disabled: "[dim]Rhomode [bright_red]deaktiviert[/]. Benutzen `[deep_sky_blue3]/last[/]` um die letzte Antwort anzuzeigen."
   #
   stream_mode_enabled: "[dim]Stream-Mode [green]aktiviert[/], die Antwort wird ausgegeben, sobald der erste Teil der Antwort eintrifft."
   stream_mode_disabled: "[dim]Stream-Mode [bright_red]deaktiviert[/], die Antwort wird nach die ganze Antwort eintrifft ausgegeben."
   stream_overflow_modified: "[dim]Die Stream-Overflow Option wurde von '%{old_overflow}' auf '%{new_overflow}' geändert."
   stream_overflow_visible: "[dim]Beachten dass das Terminal bei diesem Modus das Gehalt außerhalb des Bildschirms nicht richtig bereinigt."
   stream_overflow_no_changed: "[dim]Ungültige Stream-Overflow Option, erhält die Option '%{old_overflow}' unverändert."
   #
@@ -42,15 +42,15 @@
   usage_plan: "[bright_blue]Plan: %{credit_plan}"
   #
   host_set: "[dim]API Host wurde auf '%{new_host}' gesetzt."
   #
   model_set: "[dim]Leere Eingabe, erhält das Modell '%{old_model}' unverändert."
   model_changed: "[dim]Das Modell wurde von '%{old_model}' auf '%{new_model}' geändert."
   #
-  multi_line_enable: "[dim]Multi-Linie-Mode [green]aktiviert[/], pressen [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] einzureichen."
+  multi_line_enable: "[dim]Multi-Linie-Mode [green]aktiviert[/], pressen [[deep_sky_blue3]Esc[/]] + [[deep_sky_blue3]ENTER[/]] einzureichen."
   multi_line_disabled: "[dim]Multi-Linie-Mode [bright_red]deaktiviert[/]."
   #
   ChatGPT_thinking: "[bold cyan]ChatGPT denkt nach..."
   #
   Aborted: "[bold cyan]Abbrechen."
   Error_message: "[red]Fehler: %{error_msg}"
   Error_timeout: "[red]Fehler: API hat Zeitüberschreitung (%{timeout}s) erreicht. Du kannst wiederholen oder die Zeitüberschreitung erhöhen."
@@ -69,42 +69,42 @@
   title_waiting_gen: "[bold cyan]Warten auf die letzte Titel Generierung zum Ende zu kommen..."
   title_gening: "[bold cyan]Generieren den Titel... [/](Ctrl-C zu springen)"
   title_skip_gen: "[bold cyan]Warten überspringen."
   title_gen_fail: "[red]Der Titel konnte nicht generiert werden."
   title_changed: "[red]Der Title des Kommandozeiles wurde auf '%{title}' geändert."
   title_auto_gen_fail: "[red]Fehler bei der automatischen Erzeugung des Titels im Hintergrund: %{error_msg}. Sehen Log für weitere Informationen."
   #
-  save_history_success: "[dim]Chatverlauf gespeichert in: [bright_magenta]%{filename}"
-  save_history_urgent_success: "[dim]Chatverlauf dringend gespeichert in: [bright_magenta]%{filename}"
+  save_history_success: "[dim]Chatverlauf gespeichert in: [deep_sky_blue3]%{filename}"
+  save_history_urgent_success: "[dim]Chatverlauf dringend gespeichert in: [deep_sky_blue3]%{filename}"
   #
   timeout_prompt: "OpenAI API Zeitüberschreitung: "
   timeout_changed: "[dim]API Zeitüberschreitung wurde auf [green]%{timeout}s[/] geändert."
   #
   undo_removed: "[dim]Die letzte Frage: '%{truncated_question}' und ihre Antwort wurden gelöscht."
   undo_nothing: "[dim]Keine zu tun."
   #
   temperature_must_between: "[red]Die Eingabe muss eine Zahl zwischen 0 und 2 sein"
   temperature_set: "[dim]Die Zufälligkeit wurde auf [green]%{temperature}[/] geändert."
   #
   delete_first_conversation_yes: "[dim]Die erste Frage: '%{truncated_question}' und ihre Antwort wurden gelöscht, eingespart Tokens: %{tokens_saved}"
   delete_first_conversation_no: "[red]Keine Unterhaltung jetzt."
   delete_all: "[dim]Aktuelle Unterhaltung gelöscht."
-  delete_nothing: "[dim]Keine zu tun. Verfügbarer Löschen-Befehl: `[bright_magenta]/delete first[/]` oder `[bright_magenta]/delete all[/]`"
+  delete_nothing: "[dim]Keine zu tun. Verfügbarer Löschen-Befehl: `[deep_sky_blue3]/delete first[/]` oder `[deep_sky_blue3]/delete all[/]`"
   #
   version_all: "[bold blue]Lokale Version:[/]\tv%{local_version}\n[bold green]Fernversion:[/]\tv%{remote_version}"
   version_name: "Version"
   #
-  tokens_reached: "Token-Limit erreicht, soll ich die früheste Nachricht des aktuellen Chats vergessen?"
+  tokens_reached: "Das Token-Limit wurde erreicht. Um die Konversation fortzusetzen, verwenden Sie `[deep_sky_blue3]/delete first[/]`, um die älteste Konversation zu löschen, oder verwenden Sie `[deep_sky_blue3]/model[/]`, um zu einem Modell mit einem höheren Token zu wechseln Grenze"
   tokens_approaching: "[dim]Nähert sich dem Token-Limit: %{token_left} tokens übrig"
   #
   load_file_not: "[bright_red]Datei nicht gefunden: %{file_path}"
   load_json_error: "[bright_red]Ungültiges JSON-Format in der Datei: %{file_path}"
   #
   new_lang_prompt: "Sprache: "
-  lang_switch: "[dim]Wechselt zu [bright_magenta]Deutsch[/]."
+  lang_switch: "[dim]Wechselt zu [deep_sky_blue3]Deutsch[/]."
   lang_config_unsupport: "[red]Nicht unterstützte Sprache in der Konfiguration `%{config_lang}`. Die Sprache des Benutzers wird verwendet."
   lang_unsupport: "[red]Nicht unterstützte Sprache `%{new_lang}`."
   #
   upgrade_title: "Neue Version verfügbar: [red]v%{local_version}[/] -> [green]v%{remote_version}[/]"
   upgrade_use_command: "Verwenden `pip install --upgrade gpt-term` zum Upgrade."
   upgrade_see_git: "Sehen unsere [GitHub Site](https://github.com/xiaoxx970/chatgpt-in-terminal) um zu sehen, was geändert wurde!"
   #
@@ -122,17 +122,17 @@
   help_set_key: "API-Schlüssel für OpenAI einstellen"
   help_set_timeout: "Maximale Wartezeit für API-Anfragen einstellen"
   help_set_gentitle: "Festlegen, ob automatisch ein Titel für den Chat generiert werden soll"
   help_set_lang: "Sprache einstellen"
   help_set_saveperfix: "Speicherperfix für die Chatverlaufsdatei einstellen"
   help_set_loglevel: "Log-Stufe einstellen:"
   #
-  help_use_help: "Verwenden `[bright_Magenta]/help[/]`, um alle verfügbaren Slash-Befehle zu sehen"
+  help_use_help: "Verwenden `[deep_sky_blue3]/help[/]`, um alle verfügbaren Slash-Befehle zu sehen"
   help_uncommand: "Unerkannter Slash-Befehl `[bold red]%{command}[/]`"
-  help_mean_command: "Meinst Du `[bright magenta]%{most_similar_command}[/]`?"
+  help_mean_command: "Meinst Du `[deep_sky_blue3]%{most_similar_command}[/]`?"
   help_text: |
     [bold]Verfügbare Befehle:[/]
       /raw                     - Rohmode umschalten (zeigt den Rohtext der ChatGPT-Antwort an)
       /multi                   - Multi-Linie-Mode umschalten (erlaubt mehrzeilige Eingaben)
       /stream \[overflow_mode]  - Stream-Mode umschalten (fluss-drucken der Antwort)
       /tokens                  - Zeigt die insgesamt ausgegebenen Token und die Token für die aktuelle Konversation an
       /usage                   - Zeigt das gesamte Guthaben und das aktuell verbrauchte Guthaben an
```

### Comparing `gpt-term-1.1.2/gpt_term/locale/gpt_term.en.yml` & `gpt-term-1.1.3/gpt_term/locale/gpt_term.en.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 en:
-  welcome: "[dim]Hi, welcome to chat with GPT. Type `[bright_magenta]/help[/]` to display available commands."
+  welcome: "[dim]Hi, welcome to chat with GPT. Type `[deep_sky_blue3]/help[/]` to display available commands."
   exit: "Exiting..."
-  spent_token: "[bright_magenta]Total tokens spent: [bold]%{total_tokens_spent}"
+  spent_token: "[deep_sky_blue3]Total tokens spent: [bold]%{total_tokens_spent}"
   save_api_key: "Save API Key to config file?"
   input_api_key: "OpenAI API Key not found, please input: "
-  config_key_to_shell_key : "Config item `[bright_magenta]%{key_word}[/]` is set to [green]%{val}[/]"
+  config_key_to_shell_key : "Config item `[deep_sky_blue3]%{key_word}[/]` is set to [green]%{val}[/]"
   log_level_error: "[dim]Invalid log level: %{e}, check config.ini file. Set log level to INFO."
   system_prompt: "System prompt: "
   new_temperature: "New Randomness: "
   #
-  load_chat_history: "[dim]Chat history successfully loaded from: [bright_magenta]%{load}"
+  load_chat_history: "[dim]Chat history successfully loaded from: [deep_sky_blue3]%{load}"
   #
   code_not_found: "[dim]No code found"
   code_too_many_found: "[dim]There are more than one code in ChatGPT's last reply"
   code_num: "[yellow]Code %{code_num}:"
   code_select: "Please select which code to copy: "
   code_index_must_int: "[red]Code index must be an Integer"
   code_index_out_range_one: "[red]Index out of range: There is only one code in ChatGPT's last reply"
   code_index_out_range_many: "[red]Index out of range: You should input an Integer in range 1 ~%{len_code_list}"
   code_copy: "[dim]Code copied to Clipboard"
   code_last_copy: "[dim]Last reply copied to Clipboard"
-  code_copy_fail: "[dim]Nothing to do. Available copy command: `[bright_magenta]/copy code \\[index][/]` or `[bright_magenta]/copy all[/]`"
+  code_copy_fail: "[dim]Nothing to do. Available copy command: `[deep_sky_blue3]/copy code \\[index][/]` or `[deep_sky_blue3]/copy all[/]`"
   #
-  raw_mode_enabled: "[dim]Raw mode [green]enabled[/], use `[bright_magenta]/last[/]` to display the last answer."
-  raw_mode_disabled: "[dim]Raw mode [bright_red]disabled[/], use `[bright_magenta]/last[/]` to display the last answer."
+  raw_mode_enabled: "[dim]Raw mode [green]enabled[/], use `[deep_sky_blue3]/last[/]` to display the last answer."
+  raw_mode_disabled: "[dim]Raw mode [bright_red]disabled[/], use `[deep_sky_blue3]/last[/]` to display the last answer."
   #
   stream_mode_enabled: "[dim]Stream mode [green]enabled[/], the answer will start outputting as soon as the first response arrives."
   stream_mode_disabled: "[dim]Stream mode [bright_red]disabled[/], the answer is being displayed after the server finishes responding."
   stream_overflow_modified: "[dim]Stream overflow option has been modified from '%{old_overflow}' to '%{new_overflow}'."
   stream_overflow_visible: "[dim]Note that in this mode the terminal will not properly clean up off-screen content."
   stream_overflow_no_changed: "[dim]No such Stream overflow option, remain '%{old_overflow}' unchanged."
   #
@@ -42,15 +42,15 @@
   usage_plan: "[bright_blue]Plan: %{credit_plan}"
   #
   host_set: "[dim]API Host set to '%{new_host}'."
   #
   model_set: "[dim]Empty input, the model remains '%{old_model}'."
   model_changed: "[dim]Model has been set from '%{old_model}' to '%{new_model}'."
   #
-  multi_line_enabled: "[dim]Multi-line mode [green]enabled[/], press [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] to submit."
+  multi_line_enabled: "[dim]Multi-line mode [green]enabled[/], press [[deep_sky_blue3]Esc[/]] + [[deep_sky_blue3]ENTER[/]] to submit."
   multi_line_disabled: "[dim]Multi-line mode [bright_red]disabled[/]."
   #
   ChatGPT_thinking: "[bold cyan]ChatGPT is thinking..."
   #
   Aborted: "[bold cyan]Aborted."
   Error_message: "[red]Error: %{error_msg}"
   Error_timeout: "[red]Error: API read timed out (%{timeout}s). You can retry or increase the timeout."
@@ -69,42 +69,42 @@
   title_waiting_gen: "[bold cyan]Waiting last generation to finish..."
   title_gening: "[bold cyan]Generating title... [/](Ctrl-C to skip)"
   title_skip_gen: "[bold cyan]Skip wait."
   title_gen_fail: "[red]Failed to generate title."
   title_changed: "[dim]CLI Title changed to '%{title}'"
   title_auto_gen_fail: "[red]Background Title auto-generation Error: %{error_msg}. Check log for more information"
   #
-  save_history_success: "[dim]Chat history saved to: [bright_magenta]%{filename}"
-  save_history_urgent_success: "[dim]Chat history urgently saved to: [bright_magenta]%{filename}"
+  save_history_success: "[dim]Chat history saved to: [deep_sky_blue3]%{filename}"
+  save_history_urgent_success: "[dim]Chat history urgently saved to: [deep_sky_blue3]%{filename}"
   #
   timeout_prompt: "OpenAI API timeout: "
   timeout_changed: "[dim]API timeout set to [green]%{timeout}s[/]."
   #
   undo_removed: "[dim]Last question: '%{truncated_question}' and it's answer has been removed."
   undo_nothing: "[dim]Nothing to undo."
   #
   temperature_must_between: "[red]Input must be a number between 0 and 2"
   temperature_set: "[dim]Randomness set to [green]%{temperature}[/]."
   #
   delete_first_conversation_yes: "[dim]First question: '%{truncated_question}' and it's answer has been deleted, saved tokens: %{tokens_saved}"
   delete_first_conversation_no: "[red]No conversations yet."
   delete_all: "[dim]Current chat cleared."
-  delete_nothing: "[dim]Nothing to do. Avaliable delete command: `[bright_magenta]/delete first[/]` or `[bright_magenta]/delete all[/]`"
+  delete_nothing: "[dim]Nothing to do. Avaliable delete command: `[deep_sky_blue3]/delete first[/]` or `[deep_sky_blue3]/delete all[/]`"
   #
   version_all: "[bold blue]Local Version:[/]\tv%{local_version}\n[bold green]Remote Version:[/]\tv%{remote_version}"
   version_name: "Version"
   #
-  tokens_reached: "Reached tokens limit, do you want me to forget the earliest message of current chat?"
+  tokens_reached: "The token limit has been reached. To continue the conversation, use `[deep_sky_blue3]/delete first[/]` to delete the oldest conversation, or use `[deep_sky_blue3]/model[/]` to switch to a model with a higher token limit"
   tokens_approaching : "[dim]Approaching the tokens limit: %{token_left} tokens left"
   #
   load_file_not: "[bright_red]File not found: %{file_path}"
   load_json_error: "[bright_red]Invalid JSON format in file: %{file_path}"
   #
   new_lang_prompt: "Language: "
-  lang_switch: "[dim]Language switched to [bright_magenta]English[/]."
+  lang_switch: "[dim]Language switched to [deep_sky_blue3]English[/]."
   lang_config_unsupport: "[red]Unsupported language `%{config_lang}` in config, use user local language."
   lang_unsupport: "[red]Unsupported language `%{new_lang}`."
   #
   upgrade_title: "New Version Available: [red]v%{local_version}[/] -> [green]v%{remote_version}[/]"
   upgrade_use_command: "Use `pip install --upgrade gpt-term` to upgrade."
   upgrade_see_git: "Visit our [GitHub Site](https://github.com/xiaoxx970/chatgpt-in-terminal) to see what have been changed!"
   #
@@ -122,17 +122,17 @@
   help_set_key: "Set API key for OpenAI"
   help_set_timeout: "Set maximum waiting time for API requests"
   help_set_gentitle: "Set whether to automatically generate a title for chat"
   help_set_lang: "Set language"
   help_set_saveperfix: "Set chat history file's save perfix"
   help_set_loglevel: "Set log level:"
   #
-  help_use_help: "Use `[bright magenta]/help[/]` to see all available slash commands"
+  help_use_help: "Use `[deep_sky_blue3]/help[/]` to see all available slash commands"
   help_uncommand: "Unrecognized Slash Command `[bold red]%{command}[/]`"
-  help_mean_command: "Do you mean `[bright magenta]%{most_similar_command}[/]`?"
+  help_mean_command: "Do you mean `[deep_sky_blue3]%{most_similar_command}[/]`?"
   help_text: |
     [bold]Available commands:[/]
       /raw                     - Toggle raw mode (showing raw text of ChatGPT's reply)
       /multi                   - Toggle multi-line mode (allow multi-line input)
       /stream \[overflow_mode]  - Toggle stream output mode (flow print the answer)
       /tokens                  - Show the total tokens spent and the tokens for the current conversation
       /usage                   - Show total credits and current credits used
```

### Comparing `gpt-term-1.1.2/gpt_term/locale/gpt_term.jp.yml` & `gpt-term-1.1.3/gpt_term/locale/gpt_term.jp.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 jp:
-  welcome: "[dim]こんにちは、GPTとのチャットへようこそ。使用可能なコマンドを表示するには、`[bright_magenta]/help[/]`を入力してください。"
+  welcome: "[dim]こんにちは、GPTとのチャットへようこそ。使用可能なコマンドを表示するには、`[deep_sky_blue3]/help[/]`を入力してください。"
   exit: "終了中..."
-  spent_token: "[bright_magenta]使用されたトークンの合計：[bold]%{total_tokens_spent}"
+  spent_token: "[deep_sky_blue3]使用されたトークンの合計：[bold]%{total_tokens_spent}"
   save_api_key: "APIキーを設定ファイルに保存しますか？"
   input_api_key: "OpenAI APIキーが見つかりませんでした。入力してください："
-  config_key_to_shell_key: "設定項目`[bright_magenta]%{key_word}[/]`は、[green]%{val}[/]に設定されています。"
+  config_key_to_shell_key: "設定項目`[deep_sky_blue3]%{key_word}[/]`は、[green]%{val}[/]に設定されています。"
   log_level_error: "[dim]ログレベルが無効です：%{e}、config.iniファイルを確認してください。ログレベルをINFOに設定します。"
   system_prompt: "システムプロンプト："
   new_temperature: "新しい乱数："
   #
-  load_chat_history: "[dim]チャット履歴が正常に読み込まれました：[bright_magenta]%{load}"
+  load_chat_history: "[dim]チャット履歴が正常に読み込まれました：[deep_sky_blue3]%{load}"
   #
   code_not_found: "[dim]コードが見つかりません"
   code_too_many_found: "[dim]ChatGPTの前回の返信には複数のコードがあります"
   code_num: "[yellow]コード%{code_num}:"
   code_select: "コピーするコードを選択してください："
   code_index_must_int: "[red]コードインデックスは整数である必要があります"
   code_index_out_range_one: "[red]インデックスが範囲外です：ChatGPTの前回の返信にはコードが1つしかありません"
   code_index_out_range_many: "[red]インデックスが範囲外です：1〜%{len_code_list}の範囲内の整数を入力する必要があります"
   code_copy: "[dim]コードがクリップボードにコピーされました"
   code_last_copy: "[dim]前回の返信がクリップボードにコピーされました"
-  code_copy_fail: "[dim]何もコピーできません。利用可能なコピーコマンドは、`[bright_magenta]/copy code \\[index][/]`または`[bright_magenta]/copy all[/]`です"
+  code_copy_fail: "[dim]何もコピーできません。利用可能なコピーコマンドは、`[deep_sky_blue3]/copy code \\[index][/]`または`[deep_sky_blue3]/copy all[/]`です"
   #
-  raw_mode_enabled: "[dim]ローモードは[green]有効[/]です。`[bright_magenta]/last[/]`を使用して最後の回答を表示します。"
-  raw_mode_disabled: "[dim]ローモードは[bright_red]無効[/]です。`[bright_magenta]/last[/]`を使用して最後の回答を表示します。"
+  raw_mode_enabled: "[dim]ローモードは[green]有効[/]です。`[deep_sky_blue3]/last[/]`を使用して最後の回答を表示します。"
+  raw_mode_disabled: "[dim]ローモードは[bright_red]無効[/]です。`[deep_sky_blue3]/last[/]`を使用して最後の回答を表示します。"
   #
   stream_mode_enabled: "[dim]ストリームモードは[green]有効[/]です。最初の応答が到着すると回答が出力されます。"
   stream_mode_disabled: "[dim]ストリームモードは[bright_red]無効[/]です。サーバーが応答を完了した後に回答が表示されます。"
   stream_overflow_modified: "[dim]ストリームオーバーフローオプションが'%{old_overflow}'から'%{new_overflow}'に変更されました。"
   stream_overflow_visible: "[dim]このモードでは、ターミナルは画面外のコンテンツを正しくクリーンアップしません。"
   stream_overflow_no_changed: "[dim]このようなストリームオーバーフローオプションは存在しません。'%{old_overflow}'は変更されません。"
   #
@@ -42,15 +42,15 @@
   usage_plan: "[bright_blue]プラン： %{credit_plan}"
   #
   host_set: "[dim]APIホストが '%{new_host}' に設定されました。"
   #
   model_set: "[dim]空の入力です。モデルは'%{old_model}'のままです。"
   model_changed: "[dim]モデルが'%{old_model}'から'%{new_model}'に変更されました。"
   #
-  multi_line_enabled: "[dim][green]マルチラインモードが有効になりました[/]、[[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]]を押して送信してください。"
+  multi_line_enabled: "[dim][green]マルチラインモードが有効になりました[/]、[[deep_sky_blue3]Esc[/]] + [[deep_sky_blue3]ENTER[/]]を押して送信してください。"
   multi_line_disabled: "[dim][bright_red]マルチラインモードが無効になりました[/]。"
   #
   ChatGPT_thinking: "[bold cyan]ChatGPTが考え中です...[/]"
   #
   Aborted: "[bold cyan]中止されました。"
   Error_message: "[red]エラー： %{error_msg}"
   Error_timeout: "[red]エラー：APIの読み取りがタイムアウトしました（%{timeout}s）。再試行するか、タイムアウトを増やしてください。"
@@ -69,42 +69,42 @@
   title_waiting_gen: "[bold cyan]最後の生成が完了するのを待っています..."
   title_gening: "[bold cyan]タイトルを生成中...[/]（Ctrl-Cでスキップ）"
   title_skip_gen: "[bold cyan]待たずにスキップする。"
   title_gen_fail: "[red]タイトルの生成に失敗しました。"
   title_changed: "[dim]CLIのタイトルが'%{title}'に変更されました。"
   title_auto_gen_fail: "[red]バックグラウンドのタイトル自動生成エラー：%{error_msg}。詳細についてはログを確認してください。"
   #
-  save_history_success: "[dim]チャット履歴を保存しました：[bright_magenta]%{filename}"
-  save_history_urgent_success: "[dim]緊急時のチャット履歴を保存しました：[bright_magenta]%{filename}"
+  save_history_success: "[dim]チャット履歴を保存しました：[deep_sky_blue3]%{filename}"
+  save_history_urgent_success: "[dim]緊急時のチャット履歴を保存しました：[deep_sky_blue3]%{filename}"
   #
   timeout_prompt: "OpenAI APIのタイムアウト："
   timeout_changed: "[dim]APIタイムアウトが[green]%{timeout}s[/]に設定されました。"
   #
   undo_removed: "[dim]前回の質問：'%{truncated_question}'とその回答が削除されました。"
   undo_nothing: "[dim]元に戻すものはありません。"
   #
   temperature_must_between: "[red]0から2の間の数字を入力してください"
   temperature_set: "[dim]ランダム性を[green]%{temperature}[/]に設定しました。"
   #
   delete_first_conversation_yes: "[dim]最初の質問：'%{truncated_question}'とその回答が削除されました。保存されたトークン：%{tokens_saved}"
   delete_first_conversation_no: "[red]まだ会話がありません。"
   delete_all: "[dim]現在のチャットがクリアされました。"
-  delete_nothing: "[dim]何も削除するものはありません。利用可能な削除コマンド：`[bright_magenta]/delete first[/]`または`[bright_magenta]/delete all[/]`"
+  delete_nothing: "[dim]何も削除するものはありません。利用可能な削除コマンド：`[deep_sky_blue3]/delete first[/]`または`[deep_sky_blue3]/delete all[/]`"
   #
   version_all: "[bold blue]ローカルバージョン：[/]\tv%{local_version}\n[bold green]リモートバージョン：[/]\tv%{remote_version}"
   version_name: "バージョン"
   #
-  tokens_reached: "トークン制限に達しました。現在のチャットの最初のメッセージを忘れてもよろしいですか？"
+  tokens_reached: "トークンの制限に達しました。会話を続ける必要がある場合は、`[deep_sky_blue3]/delete first[/]` を使用して最も古い会話を削除するか、`[deep_sky_blue3]/model[/]` を使用して別の会話に切り替えることができます」トークン上限が高いモデル"
   tokens_approaching : "[dim]トークン制限に近づいています：残り%{token_left}トークン"
   #
   load_file_not: "[bright_red]ファイルが見つかりません：%{file_path}"
   load_json_error: "[bright_red]ファイル内の無効なJSON形式です：%{file_path}"
   #
   new_lang_prompt: "言語："
-  lang_switch: "[dim]すでに[bright_magenta]日本語[/]に切り替わっています。"
+  lang_switch: "[dim]すでに[deep_sky_blue3]日本語[/]に切り替わっています。"
   lang_config_unsupport: "[red]設定でサポートされていない言語 `%{config_lang}` です。ユーザーのローカル言語が使用されます。"
   lang_unsupport: "[red]サポートされていない言語 `%{new_lang}` です。"
   #
   upgrade_title: "新しいバージョンが利用可能です：[red]v%{local_version}[/] -> [green]v%{remote_version}[/]"
   upgrade_use_command: "`pip install --upgrade gpt-term`\nを使用してアップグレードしてください。"
   upgrade_see_git: "変更内容を確認するには、[GitHubサイト](https://github.com/xiaoxx970/chatgpt-in-terminal)を訪問してください！"
   #
@@ -122,17 +122,17 @@
   help_set_key: "OpenAIのAPIキーを設定する"
   help_set_timeout: "APIリクエストの最大待ち時間を設定する"
   help_set_gentitle: "チャットのタイトルを自動生成するかどうかを設定する"
   help_set_lang: "言語を設定する"
   help_set_saveperfix: "チャット履歴ファイルの保存プレフィックスを設定する"
   help_set_loglevel: "ログレベルを設定する:"
   #
-  help_use_help: "`[bright magenta]/help[/]`を使用して利用可能なスラッシュコマンドをすべて表示します"
+  help_use_help: "`[deep_sky_blue3]/help[/]`を使用して利用可能なスラッシュコマンドをすべて表示します"
   help_uncommand: "未知のスラッシュコマンド `[bold red]%{command}[/]`"
-  help_mean_command: "`[bright magenta]%{most_similar_command}[/]`を意味しますか？"
+  help_mean_command: "`[deep_sky_blue3]%{most_similar_command}[/]`を意味しますか？"
   help_text: |
     [bold]利用可能なコマンド：[/]
       /raw                     - ローモードを切り替える（ChatGPTの応答の生のテキストを表示する）
       /multi                   - マルチラインモードを切り替える（複数行の入力を許可する）
       /stream \[overflow_mode]  - ストリーム出力モードを切り替える（回答を流れるように表示する）
       /tokens                  - 使用されたトークンの総数と現在の会話のトークン数を表示する
       /usage                   - 使用済みの総クレジットと現在のクレジットを表示する
```

### Comparing `gpt-term-1.1.2/gpt_term/locale/gpt_term.zh_CN.yml` & `gpt-term-1.1.3/gpt_term/locale/gpt_term.zh_CN.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 zh_CN:
-  welcome: "[dim]你好, 欢迎和 GPT 聊天. 输入`[bright_magenta]/help[/]` 显示可用命令."
+  welcome: "[dim]你好, 欢迎和 GPT 聊天. 输入`[deep_sky_blue3]/help[/]` 显示可用命令."
   exit: "退出中..."
-  spent_token: "[bright_magenta]已花费的 token 总数:[bold]%{total_tokens_spent}" 
+  spent_token: "[deep_sky_blue3]已花费的 token 总数:[bold]%{total_tokens_spent}" 
   save_api_key: "将 API Key 保存到配置文件中?" 
   input_api_key: "未找到 OpenAI API Key, 请输入:"
-  config_key_to_shell_key: "配置项 `[bright_magenta]%{key_word}[/]` 已设置为 [green]%{val}[/]"
+  config_key_to_shell_key: "配置项 `[deep_sky_blue3]%{key_word}[/]` 已设置为 [green]%{val}[/]"
   log_level_error: "[dim]无效的日志级别: %{e}，请检查 config.ini文件. 日志级别将设置为 INFO."
   system_prompt: "系统提示词: "
   new_temperature: "新随机值: "
   #
-  load_chat_history: "[dim]聊天记录已成功加载: [bright_magenta]%{load}"
+  load_chat_history: "[dim]聊天记录已成功加载: [deep_sky_blue3]%{load}"
   #
   code_not_found: "[dim]未找到代码"
   code_too_many_found: "[dim]ChatGPT 的上一条回复中有多个代码"
   code_num: "[yellow]代码 %{code_num}:"
   code_select: "请选择要复制的代码: "
   code_index_must_int: "[red]代码索引必须是整数"
   code_index_out_range_one: "[red]索引超出范围: ChatGPT 的上一条回复中只有一个代码"
   code_index_out_range_many: "[red]索引超出范围: 请输入一个在 1~%{len_code_list} 范围内的整数"
   code_copy: "[dim]代码已复制到剪贴板"
   code_last_copy: "[dim]上一条回复已复制到剪贴板"
-  code_copy_fail: "[dim]无操作可执行. 可用的复制命令为: `[bright_magenta]/copy code \\[index][/]` 或 `[bright_magenta]/copy all[/]`"
+  code_copy_fail: "[dim]无操作可执行. 可用的复制命令为: `[deep_sky_blue3]/copy code \\[index][/]` 或 `[deep_sky_blue3]/copy all[/]`"
   #
-  raw_mode_enabled: "[dim]原始模式[green]已启用[/], 使用 `[bright_magenta]/last[/]` 来显示最后一个回答."
-  raw_mode_disabled: "[dim]原始模式[bright_red]已关闭[/], 使用 `[bright_magenta]/last[/]` 来显示最后一个回答."
+  raw_mode_enabled: "[dim]原始模式[green]已启用[/], 使用 `[deep_sky_blue3]/last[/]` 来显示最后一个回答."
+  raw_mode_disabled: "[dim]原始模式[bright_red]已关闭[/], 使用 `[deep_sky_blue3]/last[/]` 来显示最后一个回答."
   #
   stream_mode_enabled: "[dim]流式传输[green]已启用[/], 回复将在第一个响应到达时开始输出."
   stream_mode_disabled: "[dim]流式传输[bright_red]已禁用[/], 回复将在服务器完成响应后显示."
   stream_overflow_modified: "[dim]输出模式已从 '%{old_overflow}' 修改为 '%{new_overflow}'."
   stream_overflow_visible: "[dim]请注意，该模式下终端不会正确清除屏幕外的内容."
   stream_overflow_no_changed: "[dim]没有此类输出模式，保持 '%{old_overflow}' 不变."
   #
@@ -42,15 +42,15 @@
   usage_plan: "[bright_blue]计划: %{credit_plan}"
   #
   host_set: "[dim]API主机地址已被设为 '%{new_host}'"
   #
   model_set: "[dim]输入为空，模型保持为 '%{old_model}'."
   model_changed: "[dim]模型已从 '%{old_model}' 修改为 '%{new_model}'."
   #
-  multi_line_enabled: "[dim]多行模式[green]已启用[/]，按 [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] 提交." 
+  multi_line_enabled: "[dim]多行模式[green]已启用[/]，按 [[deep_sky_blue3]Esc[/]] + [[deep_sky_blue3]ENTER[/]] 提交." 
   multi_line_disabled: "[dim]多行模式[bright_red]已禁用[/]."
   #
   ChatGPT_thinking: "[bold cyan]ChatGPT 正在思考..."
   #
   Aborted: "[bold cyan]中断."
   Error_message: "[red]错误: %{error_msg}"
   Error_timeout: "[red]错误: API读取超时(%{timeout}s). 您可以重试或增加超时时间."
@@ -69,42 +69,42 @@
   title_waiting_gen: "[bold cyan]等待上一次生成完成..."
   title_gening: "[bold cyan]正在生成标题... [/]（按 Ctrl-C 跳过）"
   title_skip_gen: "[bold cyan]跳过等待."
   title_gen_fail: "[red]生成标题失败."
   title_changed: "[dim]CLI标题已更改为'%{title}'"
   title_auto_gen_fail: "[red]后台标题自动生成错误: %{error_msg}.查看日志获取更多信息."
   #
-  save_history_success: "[dim]聊天记录已保存至: [bright_magenta]%{filename}"
-  save_history_urgent_success: "[dim]聊天记录已紧急保存至: [bright_magenta]%{filename}"
+  save_history_success: "[dim]聊天记录已保存至: [deep_sky_blue3]%{filename}"
+  save_history_urgent_success: "[dim]聊天记录已紧急保存至: [deep_sky_blue3]%{filename}"
   #
   timeout_prompt: "OpenAI API 超时时间: "
   timeout_changed: "[dim]API 超时时间已设置为: [green]%{timeout}s[/]."
   #
   undo_removed: "[dim]上一个问题: '%{truncated_question}' 及其回复已被删除."
   undo_nothing: "[dim]无撤消可操作."
   #
   temperature_must_between: "[red]输入必须为 0 到 2 之间的数字"
   temperature_set: "[dim]随机性已设置为[green]%{temperature}[/]."
   #
   delete_first_conversation_yes: "[dim]第一个问题: '%{truncated_question}'及其回复已被删除，已节约 toke: %{tokens_saved}"
   delete_first_conversation_no: "[red]还没有对话."
   delete_all: "[dim]当前聊天已清除."
-  delete_nothing: "[dim]无操作可执行. 可用的删除命令: [bright_magenta]/delete first[/] 或 [bright_magenta]/delete all[/]."
+  delete_nothing: "[dim]无操作可执行. 可用的删除命令: `[deep_sky_blue3]/delete first[/]` 或 `[deep_sky_blue3]/delete all[/]`."
   #
   version_all: "[bold blue]本地版本: [/]\tv%{local_version}\n[bold green]远程版本: [/]\tv%{remote_version}" 
   version_name: "版本"
   #
-  tokens_reached: "已达到 token 限制, 您是否要删除当前聊天中最早的消息?"
+  tokens_reached: "已达到 token 限制, 如需继续对话，可使用 `[deep_sky_blue3]/delete first[/]` 删除最早对话，或者使用 `[deep_sky_blue3]/model[/]` 切换 token 上限更高的模型"
   tokens_approaching: "[dim]接近 token 限制: %{token_left}个 token 剩余"
   #
   load_file_not: "[bright_red]未找到文件: %{file_path}"
   load_json_error: "[bright_red]文件格式无效: %{file_path}"
   #
   new_lang_prompt: "语言: "
-  lang_switch: "[dim]已经切换至[bright_magenta]简体中文[/]."
+  lang_switch: "[dim]已经切换至[deep_sky_blue3]简体中文[/]."
   lang_config_unsupport: "[red]配置中不支持的语言 `%{config_lang}`, 将使用用户本地语言."
   lang_unsupport: "[red]不支持的语言 `%{new_lang}`."
   #
   upgrade_title: "新版本可用: [red]v%{local_version}[/] -> [green]v%{remote_version}[/]"
   upgrade_use_command: "使用 `pip install --upgrade gpt-term` 命令来升级."
   upgrade_see_git: "访问我们的[GitHub仓库](https://github.com/xiaoxx970/chatgpt-in-terminal)以查看更新内容！"
   #
@@ -122,17 +122,17 @@
   help_set_key: "设置OpenAI的API密钥"
   help_set_timeout: "设置API请求的最大等待时间"
   help_set_gentitle: "设置是否自动生成聊天标题"
   help_set_lang: "设置语言"
   help_set_saveperfix: "设置聊天历史记录文件的保存前缀"
   help_set_loglevel: "设置日志级别: "
   #
-  help_use_help: "使用 `[bright magenta]/help[/]` 查看所有可用的斜杠命令"
-  help_uncommand: "无法识别的斜杠命令 `[bold red]%{command}[/]`"
-  help_mean_command: "您是否指的是 `[bright magenta]%{most_similar_command}[/]`?"
+  help_use_help: "使用 `[deep_sky_blue3]/help[/]` 查看所有可用命令"
+  help_uncommand: "无法识别命令 `[bold red]%{command}[/]`"
+  help_mean_command: "您是否指的是 `[deep_sky_blue3]%{most_similar_command}[/]`?"
   help_text: |
     [bold]可用命令: [/]
       /raw                     - 切换原始模式 (显示 ChatGPT 回复的原始文本)
       /multi                   - 切换多行模式 (允许多行输入)
       /stream \[overflow_mode]  - 切换流输出模式 (连续显示回复)
       /tokens                  - 显示已使用的总 token 数和当前对话的 token 数
       /usage                   - 显示总额度和已使用的当前额度
```

### Comparing `gpt-term-1.1.2/gpt_term/main.py` & `gpt-term-1.1.3/gpt_term/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,16 +252,15 @@
                 "stream": ChatMode.stream_mode,
                 "temperature": self.temperature
             }
             response = self.send_request(data)
             if response is None:
                 self.messages.pop()
                 if self.current_tokens >= self.tokens_limit:
-                    if confirm(_('gpt_term.tokens_reached')):
-                        self.delete_first_conversation()
+                    console.print(_('gpt_term.tokens_reached'))
                 return
 
             reply_message = self.process_response(response)
             if reply_message is not None:
                 log.info(f"ChatGPT: {reply_message['content']}")
                 self.messages.append(reply_message)
                 self.current_tokens = count_token(self.messages)
@@ -1101,21 +1100,23 @@
         api_key = config.get(args.key)
     else:
         api_key = config.get("OPENAI_API_KEY")
 
     if not api_key:
         log.debug("API Key not found, waiting for input")
         api_key = prompt(_("gpt_term.input_api_key"))
-        if confirm(_("gpt_term.save_api_key")):
+        if confirm(_("gpt_term.save_api_key"), suffix=" (y/N) "):
             config["OPENAI_API_KEY"] = api_key
             write_config(config_ini)
 
     api_key_log = api_key[:3] + '*' * (len(api_key) - 7) + api_key[-4:]
     log.debug(f"Loaded API Key: {api_key_log}")
 
+    console.print(_("gpt_term.welcome"))
+
     api_timeout = config.getfloat("OPENAI_API_TIMEOUT", 30)
     log.debug(f"API Timeout set to {api_timeout}")
 
     chat_save_perfix = config.get("CHAT_SAVE_PERFIX", "./chat_history_")
 
     chat_gpt = ChatGPT(api_key, api_timeout)
     
@@ -1152,17 +1153,14 @@
             for message in chat_gpt.messages:
                 print_message(message)
             chat_gpt.current_tokens = count_token(chat_gpt.messages)
             log.info(f"Chat history successfully loaded from: {args.load}")
             console.print(
                 _("gpt_term.load_chat_history",load=args.load), highlight=False)
 
-    console.print(
-        _("gpt_term.welcome"))
-
     session = PromptSession()
 
     # 绑定回车事件，达到自定义多行模式的效果
     key_bindings = create_key_bindings()
 
     while True:
         try:
```

### Comparing `gpt-term-1.1.2/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.1.3/gpt_term.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.2
+Version: 1.1.3
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gpt-term-1.1.2/gpt_term.egg-info/SOURCES.txt` & `gpt-term-1.1.3/gpt_term.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.2/pyproject.toml` & `gpt-term-1.1.3/pyproject.toml`

 * *Files identical despite different names*

