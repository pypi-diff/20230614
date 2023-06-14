# Comparing `tmp/gitbetter-1.4.0.tar.gz` & `tmp/gitbetter-2.0.0.tar.gz`

## Comparing `gitbetter-1.4.0.tar` & `gitbetter-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 gitbetter-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/index.html
--rw-r--r--   0        0        0    63979 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/search.js
--rw-r--r--   0        0        0   238036 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   250260 2020-02-02 00:00:00.000000 gitbetter-1.4.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.4.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 gitbetter-1.4.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 gitbetter-1.4.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 gitbetter-1.4.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 gitbetter-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 gitbetter-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34198 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/index.html
+-rw-r--r--   0        0        0   178440 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/search.js
+-rw-r--r--   0        0        0   592710 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   524054 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0    58253 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter/parsers.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    17224 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/parsers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 gitbetter-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 gitbetter-2.0.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 gitbetter-2.0.0/PKG-INFO
```

### Comparing `gitbetter-1.4.0/CHANGELOG.md` & `gitbetter-2.0.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## v1.4.0 (2023-06-01)
+
+#### Refactorings
+
+* no longer necessary to specify the -f/--files flag before listing files when using the add command
 ## v1.3.0 (2023-05-30)
 
 #### New Features
 
 * add current_branch property to Git class
 #### Refactorings
```

### Comparing `gitbetter-1.4.0/docs/gitbetter.html` & `gitbetter-2.0.0/docs/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                    pattern=".+" required>
 
 
         <h2>Submodules</h2>
         <ul>
                 <li><a href="gitbetter/git.html">git</a></li>
                 <li><a href="gitbetter/gitbetter.html">gitbetter</a></li>
+                <li><a href="gitbetter/parsers.html">parsers</a></li>
         </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 
 
   ⁰
 [Unknown INPUT type]
 ***** Submodules *****
     * git
     * gitbetter
+    * parsers
 built_with_pdoc[pdoc_logo]
 
 ****** gitbetter ******
 ⁰ View Source
 1from gitbetter.git import Git
```

### Comparing `gitbetter-1.4.0/LICENSE.txt` & `gitbetter-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-1.4.0/README.md` & `gitbetter-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,48 +23,66 @@
 You can still execute a command in the shell regardless of this setting with the `sys` command.
 <pre>
 C:\gitbetter>gitbetter
 Starting gitbetter...
 Enter 'help' or '?' for command help.
 gitbetter::C:\gitbetter>help
 
-Documented commands (type help <topic>):
-========================================
-add             ignore         pull_branch
-add_url         initcommit     push
-amend           list_branches  push_new
-cd              loggy          quit
-commit          make_private   status
-commitall       make_public    switch
-commitf         merge          sys
-delete_branch   new_branch     tag
-delete_gh_repo  new_gh_remote  toggle_unrecognized_command_behavior
-git             new_repo       undo
-help            pull
+Built in Git commands (type '{command} -h' or '{command} --help'):
+==================================================================
+add            filter_branch  rebase                                version
+am             format_patch   reflog                                whatchanged
+annotate       fsck           remote                                worktree
+archive        gc             repack
+bisect         git            replace
+blame          gitk           request_pull
+branch         gitweb         rerere
+bugreport      grep           reset
+bundle         gui            restore
+cd             help           revert
+checkout       init           rm
+cherry_pick    instaweb       scalar
+citool         log            shortlog
+clean          maintenance    show
+clone          merge          show_branch
+commit         merge_tree     sparse_checkout
+config         mergetool      stash
+count_objects  mv             status
+describe       notes          submodule
+diagnose       pack_refs      switch
+diff           prune          sys
+difftool       pull           tag
+fast_export    push           toggle_unrecognized_command_behavior
+fast_import    quit           verify_commit
+fetch          range_diff     verify_tag
+
+Convenience commands (type 'help {command}'):
+=============================================
+add_url   commitall      delete_gh_repo  loggy         new_branch     push_new
+amend     commitf        ignore          make_private  new_gh_remote  undo
+branches  delete_branch  initcommit      make_public   new_repo
 
 Unrecognized command behavior: Execute in shell with os.system()
 ^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^
 
 gitbetter::C:\gitbetter>help commitf
 Stage and commit a list of files.
 Parser help for commitf:
-usage: gitbetter [-h] -m MESSAGE [-r] [files ...]
+usage: gitbetter [-h] -m MESSAGE [files ...]
 
 positional arguments:
   files                 List of files to stage and commit.
 
 options:
   -h, --help            show this help message and exit
   -m MESSAGE, --message MESSAGE
                         The commit message to use.
-  -r, --recursive       If a file name is not found in the current working directory, search for it in subfolders. This avoids having to type paths to files in subfolders,
-                        but if you have multiple files in different subfolders with the same name that have changes they will all be staged and committed.
-                        
+
 gitbetter::C:\gitbetter>help loggy
-Execute `git --oneline --name-only --abbrev-commit --graph`.
+>>> git --oneline --name-only --abbrev-commit --graph
 
 gitbetter::C:\gitbetter>loggy
 *   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
 |\
 | * b4478a3 feat: new print statement
 | | test.py
 * | eb89c2e docs: update readme
```

### Comparing `gitbetter-1.4.0/pyproject.toml` & `gitbetter-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2231 2e34 2e30 220d  rsion = "1.4.0".
+000000b0: 7273 696f 6e20 3d20 2232 2e30 2e30 220d  rsion = "2.0.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-1.4.0/PKG-INFO` & `gitbetter-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 1.4.0
+Version: 2.0.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
@@ -42,48 +42,66 @@
 You can still execute a command in the shell regardless of this setting with the `sys` command.
 <pre>
 C:\gitbetter>gitbetter
 Starting gitbetter...
 Enter 'help' or '?' for command help.
 gitbetter::C:\gitbetter>help
 
-Documented commands (type help <topic>):
-========================================
-add             ignore         pull_branch
-add_url         initcommit     push
-amend           list_branches  push_new
-cd              loggy          quit
-commit          make_private   status
-commitall       make_public    switch
-commitf         merge          sys
-delete_branch   new_branch     tag
-delete_gh_repo  new_gh_remote  toggle_unrecognized_command_behavior
-git             new_repo       undo
-help            pull
+Built in Git commands (type '{command} -h' or '{command} --help'):
+==================================================================
+add            filter_branch  rebase                                version
+am             format_patch   reflog                                whatchanged
+annotate       fsck           remote                                worktree
+archive        gc             repack
+bisect         git            replace
+blame          gitk           request_pull
+branch         gitweb         rerere
+bugreport      grep           reset
+bundle         gui            restore
+cd             help           revert
+checkout       init           rm
+cherry_pick    instaweb       scalar
+citool         log            shortlog
+clean          maintenance    show
+clone          merge          show_branch
+commit         merge_tree     sparse_checkout
+config         mergetool      stash
+count_objects  mv             status
+describe       notes          submodule
+diagnose       pack_refs      switch
+diff           prune          sys
+difftool       pull           tag
+fast_export    push           toggle_unrecognized_command_behavior
+fast_import    quit           verify_commit
+fetch          range_diff     verify_tag
+
+Convenience commands (type 'help {command}'):
+=============================================
+add_url   commitall      delete_gh_repo  loggy         new_branch     push_new
+amend     commitf        ignore          make_private  new_gh_remote  undo
+branches  delete_branch  initcommit      make_public   new_repo
 
 Unrecognized command behavior: Execute in shell with os.system()
 ^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^
 
 gitbetter::C:\gitbetter>help commitf
 Stage and commit a list of files.
 Parser help for commitf:
-usage: gitbetter [-h] -m MESSAGE [-r] [files ...]
+usage: gitbetter [-h] -m MESSAGE [files ...]
 
 positional arguments:
   files                 List of files to stage and commit.
 
 options:
   -h, --help            show this help message and exit
   -m MESSAGE, --message MESSAGE
                         The commit message to use.
-  -r, --recursive       If a file name is not found in the current working directory, search for it in subfolders. This avoids having to type paths to files in subfolders,
-                        but if you have multiple files in different subfolders with the same name that have changes they will all be staged and committed.
-                        
+
 gitbetter::C:\gitbetter>help loggy
-Execute `git --oneline --name-only --abbrev-commit --graph`.
+>>> git --oneline --name-only --abbrev-commit --graph
 
 gitbetter::C:\gitbetter>loggy
 *   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
 |\
 | * b4478a3 feat: new print statement
 | | test.py
 * | eb89c2e docs: update readme
```

