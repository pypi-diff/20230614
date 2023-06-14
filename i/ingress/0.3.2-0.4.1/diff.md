# Comparing `tmp/ingress-0.3.2.tar.gz` & `tmp/ingress-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ingress-0.3.2.tar", last modified: Mon Nov 12 22:32:09 2018, max compression
+gzip compressed data, was "ingress-0.4.1.tar", last modified: Wed Jun 14 12:04:17 2023, max compression
```

## Comparing `ingress-0.3.2.tar` & `ingress-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 miki      (1000) miki      (1000)        0 2018-11-12 22:32:09.000000 ingress-0.3.2/
--rw-rw-r--   0 miki      (1000) miki      (1000)       32 2018-11-12 21:21:07.000000 ingress-0.3.2/MANIFEST.in
--rw-rw-r--   0 miki      (1000) miki      (1000)      784 2018-11-12 22:32:09.000000 ingress-0.3.2/PKG-INFO
--rw-rw-r--   0 miki      (1000) miki      (1000)      422 2018-11-12 22:21:21.000000 ingress-0.3.2/README.md
-drwxrwxr-x   0 miki      (1000) miki      (1000)        0 2018-11-12 22:32:09.000000 ingress-0.3.2/ingress.egg-info/
--rw-rw-r--   0 miki      (1000) miki      (1000)      784 2018-11-12 22:32:09.000000 ingress-0.3.2/ingress.egg-info/PKG-INFO
--rw-rw-r--   0 miki      (1000) miki      (1000)      221 2018-11-12 22:32:09.000000 ingress-0.3.2/ingress.egg-info/SOURCES.txt
--rw-rw-r--   0 miki      (1000) miki      (1000)        1 2018-11-12 22:32:09.000000 ingress-0.3.2/ingress.egg-info/dependency_links.txt
--rw-rw-r--   0 miki      (1000) miki      (1000)        4 2018-11-12 22:32:09.000000 ingress-0.3.2/ingress.egg-info/requires.txt
--rw-rw-r--   0 miki      (1000) miki      (1000)        8 2018-11-12 22:32:09.000000 ingress-0.3.2/ingress.egg-info/top_level.txt
--rw-rw-r--   0 miki      (1000) miki      (1000)        1 2018-11-12 21:29:48.000000 ingress-0.3.2/ingress.egg-info/zip-safe
--rwxrwxr-x   0 miki      (1000) miki      (1000)     4495 2018-11-12 22:16:08.000000 ingress-0.3.2/ingress.py
--rw-rw-r--   0 miki      (1000) miki      (1000)       38 2018-11-12 22:32:09.000000 ingress-0.3.2/setup.cfg
--rw-rw-r--   0 miki      (1000) miki      (1000)      798 2018-11-12 22:31:43.000000 ingress-0.3.2/setup.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-06-14 12:04:17.435516 ingress-0.4.1/
+-rw-r--r--   0 miki      (1000) miki      (1000)     1081 2022-11-08 07:23:11.000000 ingress-0.4.1/LICENSE.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)       32 2022-11-08 07:23:11.000000 ingress-0.4.1/MANIFEST.in
+-rw-r--r--   0 miki      (1000) miki      (1000)     1283 2023-06-14 12:04:17.435516 ingress-0.4.1/PKG-INFO
+-rw-r--r--   0 miki      (1000) miki      (1000)      534 2022-11-08 07:40:28.000000 ingress-0.4.1/README.md
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-06-14 12:04:17.435516 ingress-0.4.1/ingress.egg-info/
+-rw-r--r--   0 miki      (1000) miki      (1000)     1283 2023-06-14 12:04:17.000000 ingress-0.4.1/ingress.egg-info/PKG-INFO
+-rw-r--r--   0 miki      (1000) miki      (1000)      233 2023-06-14 12:04:17.000000 ingress-0.4.1/ingress.egg-info/SOURCES.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        1 2023-06-14 12:04:17.000000 ingress-0.4.1/ingress.egg-info/dependency_links.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        4 2023-06-14 12:04:17.000000 ingress-0.4.1/ingress.egg-info/requires.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        8 2023-06-14 12:04:17.000000 ingress-0.4.1/ingress.egg-info/top_level.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        1 2023-06-14 11:54:42.000000 ingress-0.4.1/ingress.egg-info/zip-safe
+-rw-r--r--   0 miki      (1000) miki      (1000)     3111 2023-06-14 11:52:15.000000 ingress-0.4.1/ingress.py
+-rw-r--r--   0 miki      (1000) miki      (1000)       38 2023-06-14 12:04:17.435516 ingress-0.4.1/setup.cfg
+-rw-r--r--   0 miki      (1000) miki      (1000)     1289 2023-06-14 11:54:24.000000 ingress-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ingress-0.3.2/ingress.py` & `ingress-0.4.1/ingress.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,117 @@
-#!/usr/bin/env python
-'''A 'backdoor' shell for running servers (very much like Twisted manhole).
+"""A 'backdoor' shell for running servers (very much like Twisted manhole).
 
 Once installed, you can 'telnet <host> <port>' and run Python commands on your
 server environment. This is very helpful in debugging servers.
 
 This one uses only modules found in the standard library.
-'''
+"""
 
 __author__ = 'Miki Tebeka <miki.tebeka@gmail.com>'
-__version__ = '0.3.2'
+__version__ = '0.4.1'
 
-from contextlib import contextmanager
-from six import b, exec_, string_types
-from six.moves import socketserver as socksrv
+from contextlib import redirect_stdout, redirect_stderr
+import socketserver
 from threading import Thread
 from traceback import format_exc
 import socket
-import sys
 
 EOF = chr(4)
-DEFAULT_PORT = 9998
+DEFAULT_ADDRESS = ('localhost', 9998)
 QUIT = 'quit()'
 
 
-@contextmanager
-def redirect_stdout(fo):
-    old_stdout = sys.stdout
-    sys.stdout = fo
-    yield fo
-    sys.stdout = old_stdout
-
-
-class Writer(object):
-    def __init__(self, wfile):
-        self.wfile = wfile
-
-    def write(self, obj):
-        if isinstance(obj, string_types):
-            obj = b(obj)
-        self.wfile.write(obj)
-
-
-class PyHandler(socksrv.StreamRequestHandler):
+class PyHandler(socketserver.StreamRequestHandler):
     password = None
     env = {}
-    redirect = False
     prompt = '>>> '
 
     def handle(self):
         env = self.env.copy()
         welcome = 'Welcome to ingress (type "{}" to exit)\n'.format(QUIT)
-        self.wfile.write(b(welcome))
+        self.write(welcome)
 
         if not self.login():
             return
 
         while True:
             try:
-                self.wfile.write(b(self.prompt))
-                self.wfile.flush()
+                self.write(self.prompt)
                 expr = self.rfile.readline().rstrip()
                 if expr == EOF:
                     return
 
-                if not isinstance(expr, string_types):
-                    expr = expr.decode('utf-8')
+                expr = expr.decode('utf-8')
 
                 if expr == QUIT:
                     self.request.close()
                     return
 
-                out = Writer(self.wfile) if self.redirect else sys.stdout
-                with redirect_stdout(out):
+                with redirect_stdout(self), redirect_stderr(self):
                     try:
-                        value = eval(expr, globals(), env)
+                        value = eval(expr, globals(), env)  # nosec
                         out = format(value) + '\n'
-                        self.wfile.write(b(out))
-                        self.wfile.flush()
+                        self.write(out)
                     except Exception:
-                        exec_(expr, env)
+                        exec(expr, env)  # nosec
             except (EOFError, SystemExit, socket.error):
                 return
             except Exception:
                 error = format_exc()
-                self.wfile.write(b(error))
-                self.wfile.flush()
+                import sys
+                print(error, file=sys.stderr)
+                self.write(error)
 
     def finish(self):
         try:
-            socksrv.StreamRequestHandler.finish(self)
+            super().finish()
         except socket.error:
             pass
 
     def login(self):
         if not self.password:
             return True
 
-        for i in range(3):
-            self.wfile.write('Password: ')
-            password = self.rfile.readline().strip()
+        for _ in range(3):
+            self.write('Password: ')
+            password = self.rfile.readline().strip().decode('utf-8')
             if password == self.password:
                 return True
-            self.wfile.write('Bad password\n')
+            self.write('Bad password\n')
 
         return False
 
+    def write(self, obj):
+        if isinstance(obj, str):
+            obj = obj.encode('utf-8')
+        self.wfile.write(obj)
 
-class ThreadedServer(socksrv.ThreadingMixIn, socksrv.TCPServer):
+
+class ThreadedServer(socketserver.ThreadingTCPServer):
     daemon_threads = True
     allow_reuse_address = True
 
 
-def server_thread(env, port, password=None, redirect=False, host='localhost'):
-    # Create a new handler class for this with it's own env
+def install(address=DEFAULT_ADDRESS, env=None, password=None):
+    """Install TCP handler on address
+
+    Parameters
+    ----------
+    address : tuple
+        Address to listen on (host, port)
+    env : dict
+        Environment to use when evaulation expression (default to globals)
+    password : str
+        Login password
+    """
+
     class Handler(PyHandler):
         pass
 
-    Handler.env = env
+    Handler.env = {} if env is None else env
     Handler.password = password
-    Handler.redirect = redirect
-
-    server = ThreadedServer((host, port), Handler)
-    server.serve_forever()
-
-
-def install(env=None, port=DEFAULT_PORT, password=None, redirect=False,
-            host='localhost'):
-    env = env or {}
-    t = Thread(target=server_thread,
-               args=(env, port, password, redirect, host))
-    t.daemon = True
-    t.start()
-
-    return t
-
-
-def main(argv=None):
-    from argparse import ArgumentParser
-
-    argv = argv or sys.argv
-
-    parser = ArgumentParser(description='Run demo server.')
-    parser.add_argument('-p', '--port', help='port to listen',
-                        default=DEFAULT_PORT, type=int)
-    parser.add_argument('-l', '--login', help='login password',
-                        default=None)
-    parser.add_argument('-r', '--redirect', help='redirect stdout',
-                        default=False, action='store_true')
-    parser.add_argument('-s', '--host', help='host to bind to',
-                        default='localhost')
-    args = parser.parse_args(argv[1:])
-
-    t = install(port=args.port, password=args.login, redirect=args.redirect,
-                host=args.host)
-    print('Serving on {0}:{1}'.format(args.host, args.port))
-    t.join()
 
+    server = ThreadedServer(address, Handler)
+    thr = Thread(target=server.serve_forever, daemon=True)
+    thr.start()
 
-if __name__ == '__main__':
-    main()
+    return thr
```

