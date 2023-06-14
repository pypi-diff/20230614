# Comparing `tmp/fn.py-0.5.2.tar.gz` & `tmp/fn.py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fn.py-0.5.2.tar", last modified: Tue Jul 18 01:49:18 2017, max compression
+gzip compressed data, was "fn.py-0.6.0.tar", last modified: Wed Jun 14 19:54:04 2023, max compression
```

## Comparing `fn.py-0.5.2.tar` & `fn.py-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,45 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-18 01:49:18.000000 fn.py-0.5.2/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn/immutable/
--rw-r--r--   0 travis    (1000) travis    (1000)      338 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/immutable/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7130 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/immutable/finger.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6833 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/immutable/heap.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5672 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/immutable/list.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6667 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/immutable/trie.py
--rw-r--r--   0 travis    (1000) travis    (1000)      134 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2351 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/func.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8436 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/iters.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5105 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/monad.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2685 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/op.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3711 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/recur.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2445 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/stream.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6532 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/underscore.py
--rw-r--r--   0 travis    (1000) travis    (1000)      617 2017-07-18 01:48:58.000000 fn.py-0.5.2/fn/uniform.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn.py.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)    23499 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn.py.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      423 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn.py.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn.py.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-07-18 01:49:07.000000 fn.py-0.5.2/fn.py.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)        3 2017-07-18 01:49:18.000000 fn.py-0.5.2/fn.py.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      288 2017-07-18 01:48:58.000000 fn.py-0.5.2/CHANGELOG.rst
--rw-r--r--   0 travis    (1000) travis    (1000)      583 2017-07-18 01:48:58.000000 fn.py-0.5.2/LICENSE
--rw-r--r--   0 travis    (1000) travis    (1000)       41 2017-07-18 01:48:58.000000 fn.py-0.5.2/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)    17794 2017-07-18 01:48:58.000000 fn.py-0.5.2/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     2112 2017-07-18 01:48:58.000000 fn.py-0.5.2/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)    23499 2017-07-18 01:49:18.000000 fn.py-0.5.2/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2017-07-18 01:49:18.000000 fn.py-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:04.274950 fn.py-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-14 19:53:56.000000 fn.py-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-14 19:53:56.000000 fn.py-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 19:53:56.000000 fn.py-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-06-14 19:54:04.274950 fn.py-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-06-14 19:53:56.000000 fn.py-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:04.270950 fn.py-0.6.0/fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:04.270950 fn.py-0.6.0/fn/immutable/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/immutable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/immutable/finger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/immutable/heap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/immutable/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/immutable/trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/iters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/monad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/recur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/underscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-14 19:53:56.000000 fn.py-0.6.0/fn/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:04.270950 fn.py-0.6.0/fn.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-06-14 19:54:04.000000 fn.py-0.6.0/fn.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-14 19:54:04.000000 fn.py-0.6.0/fn.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:54:04.000000 fn.py-0.6.0/fn.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:54:04.000000 fn.py-0.6.0/fn.py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 19:54:04.000000 fn.py-0.6.0/fn.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:54:04.274950 fn.py-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-14 19:53:56.000000 fn.py-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:04.274950 fn.py-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_banker_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_curry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_finger_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_linked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_stram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_underscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-14 19:53:56.000000 fn.py-0.6.0/tests/test_vector.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fn.py-0.5.2/fn/immutable/finger.py` & `fn.py-0.6.0/fn/immutable/finger.py`

 * *Files identical despite different names*

### Comparing `fn.py-0.5.2/fn/immutable/heap.py` & `fn.py-0.6.0/fn/immutable/heap.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,20 @@
 class SkewHeap(_MergeBased):
     """A skew heap (or self-adjusting heap) is a heap data structure
     implemented as a binary-tree. Amortized complexity analytics can
     be used to demonstrate that all operations one a skew heap can be
     done in O(log n).
 
     Skew heaps may be described with the following recursive definition:
-    * a heap with only one element is a skew heap
-    * the result of skew merging two skew heaps is also a skew heap
+     * a heap with only one element is a skew heap
+     * the result of skew merging two skew heaps is also a skew heap
 
-    In Haskell type definition it should looks like following:
-    data Skew a = Empty | Node a (Skew a) (Skew a)
+    In Haskell type definition it should looks like following::
+
+        data Skew a = Empty | Node a (Skew a) (Skew a)
 
     More information on Wikipedia:
     [1] http://en.wikipedia.org/wiki/Skew_heap
 
     One can also check slides from my KyivPy#11 talk "Union-based heaps":
     [2] http://goo.gl/VMgdG2
 
@@ -87,15 +88,15 @@
         return self._make_heap(el).union(self)
 
     def extract(self):
         """Returns pair of values:
         * minimum (or maximum regarding to given compare function)
         * new skew heap without extracted element
 
-        Or None and empty heap if self is an empty heap.
+        Or ``None`` and empty heap if ``self`` is an empty heap.
         """
         if not self:
             return None, self._make_heap()
         if self.left:
             tmp_heap = self.left.union(self.right)
         else:
             tmp_heap = self._make_heap()
@@ -117,16 +118,17 @@
 
 class PairingHeap(_MergeBased):
     """A pairing heap is either an empty heap, or a pair consisting of a root
     element and a possibly empty list of pairing heap. The heap ordering
     property requires that all the root elements of the subheaps in the list
     are not smaller (bigger) than the root element of the heap.
 
-    In Haskell type definition it should looks like following:
-    data Pairing a = Empty | Node a [Pairing a]
+    In Haskell type definition it should looks like following::
+
+        data Pairing a = Empty | Node a [Pairing a]
 
     Pairing heap has and excellent practical amortized performance. The
     amortized time per extract is less than O(log n), find-min/find-max, merge
     and insert are O(1).
 
     More information about performance bounds you can find here:
     "The Pairing Heap: A New Form of Self-Adjusting Heap"
@@ -172,16 +174,16 @@
 
     def insert(self, el):
         """Returns new pairing heap with additional element"""
         return self.union(self._make_heap(el))
 
     def extract(self):
         """Returns pair of values:
-        * minimum (or maximum regarding to given compare function)
-        * new pairing heap without extracted element
+         * minimum (or maximum regarding to given compare function)
+         * new pairing heap without extracted element
 
         Or None and empty heap if self is an empty heap.
         """
         if not self:
             return None, self._make_heap()
         return self.root, PairingHeap._pairing(self._make_heap, self.subs)
```

### Comparing `fn.py-0.5.2/fn/immutable/list.py` & `fn.py-0.6.0/fn/immutable/list.py`

 * *Files identical despite different names*

### Comparing `fn.py-0.5.2/fn/immutable/trie.py` & `fn.py-0.6.0/fn/immutable/trie.py`

 * *Files identical despite different names*

### Comparing `fn.py-0.5.2/fn/func.py` & `fn.py-0.6.0/fn/func.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from functools import partial, update_wrapper, wraps
-from inspect import getargspec
+from sys import version_info
+
+
+_has_type_hint_support = version_info[:2] >= (3, 5)
 
 
 def identity(arg):
     return arg
 
 
 class F(object):
@@ -65,26 +68,35 @@
     ...     return a + b + c + d + e
     ...
     >>> sum5(1)(2)(3)(4)(5)
     15
     >>> sum5(1, 2, 3)(4, 5)
     15
     """
+
+    def _args_len(func):
+        if _has_type_hint_support:
+            from inspect import signature
+            args = signature(func).parameters
+        else:
+            from inspect import getargspec
+            args = getargspec(func).args
+
+        return len(args)
+
     @wraps(func)
     def _curried(*args, **kwargs):
         f = func
         count = 0
         while isinstance(f, partial):
             if f.args:
                 count += len(f.args)
             f = f.func
 
-        spec = getargspec(f)
-
-        if count == len(spec.args) - len(args):
+        if count == _args_len(f) - len(args):
             return func(*args, **kwargs)
 
         para_func = partial(func, *args, **kwargs)
         update_wrapper(para_func, f)
         return curried(para_func)
 
     return _curried
```

### Comparing `fn.py-0.5.2/fn/iters.py` & `fn.py-0.6.0/fn/iters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from collections import Iterable, deque
+from collections import deque
 from functools import partial
 from itertools import (chain, combinations, cycle, dropwhile, islice, repeat,
                        starmap, takewhile, tee)
 from operator import add, attrgetter, itemgetter
 from sys import version_info
 
 from .func import F
 from .op import flip
-from .uniform import filterfalse, zip_longest, map, range, filter
+from .uniform import filterfalse, zip_longest, map, range, filter, Iterable
 
 
 def take(limit, base):
     return islice(base, limit)
 
 
 def drop(limit, base):
```

### Comparing `fn.py-0.5.2/fn/monad.py` & `fn.py-0.6.0/fn/monad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 ``fn.monad.Option`` represents optional values, each instance of
 ``Option`` can be either instance of ``Full`` or ``Empty``.
 It provides you with simple way to write long computation sequences
 and get rid of many ``if/else`` blocks. See usage examples below.
 
 Assume that you have ``Request`` class that gives you parameter
-value by its name. To get uppercase notation for non-empty striped value:
+value by its name. To get uppercase notation for non-empty striped value::
 
     class Request(dict):
         def parameter(self, name):
             return self.get(name, None)
 
     r = Request(testing="Fixed", empty="   ")
     param = r.parameter("testing")
@@ -19,15 +19,15 @@
         param = param.strip()
         if len(param) == 0:
             fixed = ""
         else:
             fixed = param.upper()
 
 
-Hmm, looks ugly.. Update code with ``fn.monad.Option``:
+Hmm, looks ugly.. Update code with ``fn.monad.Option``::
 
     from operator import methodcaller
     from fn.monad import optionable
 
     class Request(dict):
         @optionable
         def parameter(self, name):
@@ -39,23 +39,23 @@
              .filter(len)
              .map(methodcaller("upper"))
              .get_or("")
 
 ``fn.monad.Option.or_call`` is good method for trying several
 variant to end computation. I.e. use have ``Request`` class
 with optional attributes ``type``, ``mimetype``, ``url``.
-You need to evaluate "request type" using at least on attribute:
+You need to evaluate "request type" using at least on attribute::
 
     from fn.monad import Option
 
     request = dict(url="face.png", mimetype="PNG")
-    tp = Option(request.get("type", None)) \ # check "type" key first
-      .or_call(from_mimetype, request) \ # or.. check "mimetype" key
-      .or_call(from_extension, request) \ # or... get "url" and check extension
-      .get_or("application/undefined")
+    tp = (Option(request.get("type", None)) # check "type" key first
+      .or_call(from_mimetype, request) # or.. check "mimetype" key
+      .or_call(from_extension, request) # or... get "url" and check extension
+      .get_or("application/undefined"))
 
 """
 
 from functools import partial, wraps
 from operator import eq, is_not
```

### Comparing `fn.py-0.5.2/fn/op.py` & `fn.py-0.6.0/fn/op.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,20 @@
 
 
 def foldl(f, init=None):
     """Return function to fold iterator to scala value
     using passed function as reducer.
 
     Usage:
-    >>> print foldl(_ + _)([0,1,2,3,4])
-    10
-    >>> print foldl(_ * _, 1)([1,2,3])
-    6
+        >>> print foldl(_ + _)([0,1,2,3,4])
+        10
+        >>> print foldl(_ * _, 1)([1,2,3])
+        6
     """
+
     def fold(it):
         args = [f, it]
         if init is not None:
             args.append(init)
         return reduce(*args)
 
     return fold
@@ -68,39 +69,42 @@
 
 def foldr(f, init=None):
     """Return function to fold iterator to scala value using
     passed function as reducer in reverse order (consume values
     from iterator from right-to-left).
 
     Usage:
-    >>> print foldr(call, 10)([lambda s: s**2, lambda k: k+10])
-    400
+        >>> print foldr(call, 10)([lambda s: s**2, lambda k: k+10])
+        400
     """
+
     def fold(it):
         args = [flip(f), reversed(it)]
         if init is not None:
             args.append(init)
         return reduce(*args)
 
     return fold
 
 
 def unfold(f):
     """Return function to unfold value into stream using
     passed function as values producer. Passed function should
     accept current cursor and should return:
+
       * tuple of two elements (value, cursor), value will be added
         to output, cursor will be used for next function call
       * None in order to stop producing sequence
 
     Usage:
-    >>> doubler = unfold(lambda x: (x*2, x*2))
-    >>> list(islice(doubler(10), 0, 10))
-    [20, 40, 80, 160, 320, 640, 1280, 2560, 5120, 10240]
+        >>> doubler = unfold(lambda x: (x*2, x*2))
+        >>> list(islice(doubler(10), 0, 10))
+        [20, 40, 80, 160, 320, 640, 1280, 2560, 5120, 10240]
     """
+
     def _unfolder(start):
         value, curr = None, start
         while 1:
             step = f(curr)
             if step is None:
                 break
             value, curr = step
```

### Comparing `fn.py-0.5.2/fn/recur.py` & `fn.py-0.6.0/fn/recur.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     Such function should return one of:
      * (False, result) - will exit from loop and return result to caller
      * (True, args) or (True, args, kwargs) - will repeat loop with the same
                                               function and other arguments
      * (func, args) or (func, kwargs) - will repeat loop with new callable
                                         and new arguments
 
-    Usage example:
+    Usage example::
 
-    @recur.tco
-    def accumulate(origin, f=operator.add, acc=0):
-        n = next(origin, None)
-        if n is None: return False, acc
-        return True, (origin, f, f(acc, n))
+        @recur.tco
+        def accumulate(origin, f=operator.add, acc=0):
+            n = next(origin, None)
+            if n is None: return False, acc
+            return True, (origin, f, f(acc, n))
 
     Idea was described on python mailing list:
     http://mail.python.org/pipermail/python-ideas/2009-May/004486.html
     """
 
     __slots__ = "func",
 
@@ -53,50 +53,50 @@
     decorator for generators.
 
     Invoking as f() creates the control structures. Within a
     function, only use `yield f.call()` and `yield f.tailcall()`.
 
     Usage examples:
 
-    Tail call optimised recursion with tailcall():
+    Tail call optimised recursion with tailcall()::
 
-    @recur.stackless
-    def fact(n, acc=1):
-        if n == 0:
-            yield acc
-            return
-        yield fact.tailcall(n-1, n*acc)
-
-    Non-tail recursion with call() uses heap space so won't overflow:
-
-    @recur.stackless
-    def fib(n):
-        if n == 0:
-            yield 1
-            return
-        if n == 1:
-            yield 1
-            return
-        yield (yield fib.call(n-1)) + (yield fib.call(n-2))
-
-    Mutual recursion also works:
-
-    @recur.stackless
-    def is_odd(n):
-        if n == 0:
-            yield False
-            return
-        yield is_even.tailcall(n-1)
-
-    @recur.stackless
-    def is_even(n):
-        if n == 0:
-            yield True
-            return
-        yield is_odd.tailcall(n-1)
+        @recur.stackless
+        def fact(n, acc=1):
+            if n == 0:
+                yield acc
+                return
+            yield fact.tailcall(n-1, n*acc)
+
+    Non-tail recursion with call() uses heap space so won't overflow::
+
+        @recur.stackless
+        def fib(n):
+            if n == 0:
+                yield 1
+                return
+            if n == 1:
+                yield 1
+                return
+            yield (yield fib.call(n-1)) + (yield fib.call(n-2))
+
+    Mutual recursion also works::
+
+        @recur.stackless
+        def is_odd(n):
+            if n == 0:
+                yield False
+                return
+            yield is_even.tailcall(n-1)
+
+        @recur.stackless
+        def is_even(n):
+            if n == 0:
+                yield True
+                return
+            yield is_odd.tailcall(n-1)
 
     """
 
     __slots__ = "func",
 
     Thunk = namedtuple("Thunk", ("func", "args", "kwargs", "is_tailcall"))
```

### Comparing `fn.py-0.5.2/fn/stream.py` & `fn.py-0.6.0/fn/stream.py`

 * *Files identical despite different names*

### Comparing `fn.py-0.5.2/fn/underscore.py` & `fn.py-0.6.0/fn/underscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         """Call method from _ object by given name and arguments"""
         return self.__class__(
             F(lambda f:
               apply(f, args, kwargs)) << operator.attrgetter(name) << F(self)
         )
 
     def __getattr__(self, name):
+        if name == '__wrapped__':  # Guard for recursive call by doctest
+            raise AttributeError
         attr_name = _random_name()
         return self.__class__(
             F(operator.attrgetter(name)) << F(self),
             "getattr(%s, %%(%s)r)" % (self._format, attr_name),
             dict(
                 list(self._format_args.items()) + [(attr_name, name)]
             ),
```

### Comparing `fn.py-0.5.2/LICENSE` & `fn.py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fn.py-0.5.2/README.rst` & `fn.py-0.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,269 +1,323 @@
+Metadata-Version: 2.1
+Name: fn.py
+Version: 0.6.0
+Summary: Implementation of missing features to enjoy functional programming in Python
+Home-page: https://github.com/fnpy/fn.py
+Author: fnpy team
+Author-email: vash0the0stampede@gmail.com
+License: Copyright 2013 Alexey Kachayev
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Keywords: functional,fp,utility
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
+
 Fn.py: enjoy FP in Python
 =========================
 
 .. image:: https://badges.gitter.im/fnpy/fn.py.svg
    :alt: Join the chat at https://gitter.im/fnpy/fn.py
    :target: https://gitter.im/fnpy/fn.py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-   
+
 .. image:: https://travis-ci.org/fnpy/fn.py.svg?branch=master
     :target: https://travis-ci.org/fnpy/fn.py
 
-Despite the fact that Python is not pure-functional programming
-language, it's multi-paradigm PL and it gives you enough freedom to take
-credits from functional programming approach. There are theoretical and
-practical advantages to the functional style:
+.. image:: https://img.shields.io/pypi/v/fn.py
+    :alt: PyPI
+    :target: https://pypi.org/project/fn.py
+
+.. image:: https://img.shields.io/pypi/dm/fn.py
+    :alt: PyPI - Downloads
+    :target: https://pypi.org/project/fn.py
+
+Despite the fact that Python is not a pure-functional programming language, it
+is multi-paradigm and gives you enough freedom to take advantage of a functional
+approach.  There are theoretical and practical advantages to the functional
+style:
 
 -  Formal provability
 -  Modularity
 -  Composability
 -  Ease of debugging and testing
 
-``Fn.py`` library provides you with missing "batteries" to get maximum
-from functional approach even in mostly-imperative program.
+``Fn.py`` library provides you with the missing "batteries" to get the maximum
+from a functional approach, even in mostly-imperative softwares.
 
-More about functional approach from my Pycon UA 2012 talks: `Functional
-Programming with
-Python <http://kachayev.github.com/talks/uapycon2012/index.html>`_.
+You can find more about the functional approach from my Pycon UA 2012 talks:
+`Functional Programming with Python
+<https://kachayev.github.com/talks/uapycon2012/index.html>`_.
 
 Scala-style lambdas definition
 ------------------------------
 
-.. code-block:: python
-
-    from fn import _
-    from fn.op import zipwith
-    from itertools import repeat
-
-    assert list(map(_ * 2, range(5))) == [0,2,4,6,8]
-    assert list(filter(_ < 10, [9,10,11])) == [9]
-    assert list(zipwith(_ + _)([0,1,2], repeat(10))) == [10,11,12]
-
-More examples of using ``_`` you can find in `test
-cases <https://github.com/kachayev/fn.py/blob/master/tests.py>`_
-declaration (attributes resolving, method calling, slicing).
-
-**Attention!** If you work in interactive python shell, your should remember that ``_`` means "latest output" and you'll get unpredictable results. In this case, you can do something like ``from fn import _ as X`` (and then write functions like ``X * 2``).
+::
 
-If you are not sure, what your function is going to do, you can print it:
-
-.. code-block:: python
-
-    from fn import _
-
-    print (_ + 2) # "(x1) => (x1 + 2)"
-    print (_ + _ * _) # "(x1, x2, x3) => (x1 + (x2 * x3))"
+    >>> from fn import _
+    >>> from fn.op import zipwith
+    >>> from itertools import repeat
 
-``_`` will fail with ``ArityError`` (``TypeError`` subclass) on inaccurate number of passed arguments. This is one more restrictions to ensure that you did everything right:
+    >>> list(map(_ * 2, range(5)))
+    [0, 2, 4, 6, 8]
+    >>> list(filter(_ < 10, [9,10,11]))
+    [9]
+    >>> list(zipwith(_ + _)([0,1,2], repeat(10)))
+    [10, 11, 12]
+
+You can find more examples of ``_`` in `test cases <tests/test_underscore.py>`_
+(attributes resolving, method calling, slicing).
+
+**Attention!** If you work in an interactive python shell, ``_`` can be assigned
+to the latest output and you'll get unpredictable results.  In this case, you
+can use ``X`` instead with ``from fn import _ as X``.
+
+If you are not sure what your function is going to do, print it::
+
+    >>> print(_ + 2)
+    (x1) => (x1 + 2)
+    >>> print(_ + _ * _)
+    (x1, x2, x3) => (x1 + (x2 * x3))
 
-.. code-block:: python
+Note that ``_`` will fail with ``ArityError`` (``TypeError`` subclass) when
+called with the wrong number of arguments, so as to avoid errors::
 
-    >>> from fn import _
     >>> (_ + _)(1)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
       File "fn/underscore.py", line 82, in __call__
         raise ArityError(self, self._arity, len(args))
     fn.underscore.ArityError: (_ + _) expected 2 arguments, got 1
 
 
 Persistent data structures
 --------------------------
 
 **Attention:** Persistent data structures are under active development.
 
-Persistent data structure is a data structure that always preserves the previous version of itself when it is modified (more formal information on `Wikipedia <http://goo.gl/8VveOH>`_). Each operation with such data structure yields a new updated structure instead of in-place modification (all previous versions are potentially available or GC-ed when possible).
+A persistent data structure always preserves its previous version when it is
+modified (more on `Wikipedia <https://goo.gl/8VveOH>`_).  Each operation thus
+yields a new updated structure instead of performing in-place modifications (all
+previous versions are potentially available or GC-ed when possible).
 
-Lets take a quick look:
-
-.. code-block:: python
+::
 
     >>> from fn.immutable import SkewHeap
     >>> s1 = SkewHeap(10)
     >>> s2 = s1.insert(20)
     >>> s2
-    <fn.immutable.heap.SkewHeap object at 0x10b14c050>
+    <fn.immutable.heap.SkewHeap object at 0x...>
     >>> s3 = s2.insert(30)
     >>> s3
-    <fn.immutable.heap.SkewHeap object at 0x10b14c158> # <-- other object
+    <fn.immutable.heap.SkewHeap object at 0x...>
+    >>> id(s3) != id(s2)
+    True
     >>> s3.extract()
-    (10, <fn.immutable.heap.SkewHeap object at 0x10b14c050>)
+    (10, <fn.immutable.heap.SkewHeap object at 0x...>)
     >>> s3.extract() # <-- s3 isn't changed
-    (10, <fn.immutable.heap.SkewHeap object at 0x10b11c052>)
-
-If you think I'm totally crazy and it will work despairingly slow, just give it 5 minutes. Relax, take a deep breath and read about few techniques that make persistent data structures fast and efficient: `structural sharing <http://en.wikipedia.org/wiki/Persistent_data_structure#Examples_of_persistent_data_structures>`_ and `path copying <http://en.wikipedia.org/wiki/Persistent_data_structure#Path_Copying>`_.
+    (10, <fn.immutable.heap.SkewHeap object at 0x...>)
 
-To see how it works in "pictures", you can check great slides from Zach Allaun's talk (StrangeLoop 2013): `"Functional Vectors, Maps And Sets In Julia" <http://goo.gl/Cp1Qsq>`_.
+If you think I'm totally crazy and it will work despairingly slow, just give it
+5 minutes.  Relax, take a deep breath and read about a few techniques that make
+persistent data structures fast and efficient: `structural sharing
+<https://en.wikipedia.org/wiki/Persistent_data_structure#Examples_of_persistent_data_structures>`_
+and `path copying
+<https://en.wikipedia.org/wiki/Persistent_data_structure#Path_Copying>`_.  To
+see how it works in "pictures", you can check the great slides from Zach
+Allaun's talk (StrangeLoop 2013): `"Functional Vectors, Maps And Sets In Julia"
+<https://goo.gl/Cp1Qsq>`_.  And, if you are brave enough, go and read:
 
-And, if you are brave enough, go and read:
+- `Chris Okasaki, "Purely Functional Data Structures" <https://goo.gl/c7ptkk>`_
+- `Fethi Rabhi and Guy Lapalme, "Algorithms: A Functional Programming Approach" <https://goo.gl/00BxTO>`_
 
-- Chris Okasaki, "Purely Functional Data Structures" (`Amazon <http://goo.gl/c7ptkk>`_)
-- Fethi Rabhi and Guy Lapalme, "Algorithms: A Functional Programming Approach" (`Amazon <http://goo.gl/00BxTO>`_)
+Immutable data structures available in ``fn.immutable``:
 
-Available immutable data structures in ``fn.immutable`` module:
-
-- ``LinkedList``: most "obvious" persistent data structure, used as building block for other list-based structures (stack, queue)
+- ``LinkedList``: the most "obvious" persistent data structure, used as building
+  block for other list-based structures (stack, queue)
 - ``Stack``: wraps linked list implementation with well-known pop/push API
-- ``Queue``: uses two linked lists and lazy copy to provide O(1) enqueue and dequeue operations
+- ``Queue``: uses two linked lists and lazy copy to provide O(1) enqueue and
+  dequeue operations
 - ``Deque`` (in progress): `"Confluently Persistent Deques via Data
-  Structural Bootstrapping" <http://goo.gl/vVTzx3>`_
+  Structural Bootstrapping" <https://goo.gl/vVTzx3>`_
 - ``Deque`` based on ``FingerTree`` data structure (see more information below)
-- ``Vector``: O(log32(n)) access to elements by index (which is near-O(1) for reasonable vector size), implementation is based on ``BitmappedTrie``, almost drop-in replacement for built-in Python ``list``
-- ``SkewHeap``: self-adjusting heap implemented as a binary tree with specific branching model, uses heap merge as basic operation, more information - `"Self-adjusting heaps" <http://goo.gl/R1PZME>`_
-- ``PairingHeap``: `"The Pairing-Heap: A New Form of Self-Adjusting Heap" <http://goo.gl/aiVtPH>`_
-- ``Dict`` (in progress): persistent hash map implementation based on ``BitmappedTrie``
-- ``FingerTree`` (in progress): `"Finger Trees: A Simple General-purpose Data Structure" <http://goo.gl/Bzo0df>`_
-
-Use appropriate doc strings to get more information about each data structure as well as sample code.
-
-To get more clear vision of how persistent heaps work (``SkewHeap`` and ``PairingHeap``), you can look at slides from my talk `"Union-based heaps" <http://goo.gl/VMgdG2>`_ (with analyzed data structures definitions in Python and Haskell).
+- ``Vector``: O(log32(n)) access to elements by index (which is near-O(1) for
+  reasonable vector size), implementation is based on ``BitmappedTrie``, almost
+  drop-in replacement for built-in Python ``list``
+- ``SkewHeap``: self-adjusting heap implemented as a binary tree with specific
+  branching model, uses heap merge as basic operation, more information -
+  `"Self-adjusting heaps" <https://goo.gl/R1PZME>`_
+- ``PairingHeap``: `"The Pairing-Heap: A New Form of Self-Adjusting Heap"
+  <https://goo.gl/aiVtPH>`_
+- ``Dict`` (in progress): persistent hash map implementation based on
+  ``BitmappedTrie``
+- ``FingerTree`` (in progress): `"Finger Trees: A Simple General-purpose Data
+  Structure" <https://goo.gl/Bzo0df>`_
+
+To get a clearer vision of how persistent heaps work (``SkewHeap`` and
+``PairingHeap``), you can look at slides from my talk `"Union-based heaps"
+<https://goo.gl/VMgdG2>`_ (with analyzed data structures definitions in Python
+and Haskell).
+
+**Note.** Most functional languages use persistent data structures as basic
+building blocks, well-known examples are Clojure, Haskell and Scala.  Clojure
+community puts much effort to popularize programming based on the idea of data
+immutability.  There are few amazing talk given by Rich Hickey (creator of
+Clojure), you can check them to find answers on both questions "How?" and
+"Why?":
 
-**Note.** Most functional languages use persistent data structures as basic building blocks, well-known examples are Clojure, Haskell and Scala. Clojure community puts much effort to popularize programming based on the idea of data immutability. There are few amazing talk given by Rich Hickey (creator of Clojure), you can check them to find answers on both questions "How?" and "Why?":
-
-- `"The Value of Values" <http://goo.gl/137UG5>`_
-- `"Persistent Data Structures and Managed References" <http://goo.gl/M3vZ7E>`_
+- `"The Value of Values" <https://goo.gl/137UG5>`_
+- `"Persistent Data Structures and Managed References" <https://goo.gl/M3vZ7E>`_
 
 Streams and infinite sequences declaration
 ------------------------------------------
 
-Lazy-evaluated Scala-style streams. Basic idea: evaluate each new
-element "on demand" and share calculated elements between all created
-iterators. ``Stream`` object supports ``<<`` operator that means pushing
-new elements when it's necessary.
-
-Simplest cases:
-
-.. code-block:: python
-
-    from fn import Stream
-
-    s = Stream() << [1,2,3,4,5]
-    assert list(s) == [1,2,3,4,5]
-    assert s[1] == 2
-    assert list(s[0:2]) == [1,2]
-
-    s = Stream() << range(6) << [6,7]
-    assert list(s) == [0,1,2,3,4,5,6,7]
-
-    def gen():
-        yield 1
-        yield 2
-        yield 3
-
-    s = Stream() << gen << (4,5)
-    assert list(s) == [1,2,3,4,5]
-
-Lazy-evaluated stream is useful for infinite sequences, i.e. fibonacci
-sequence can be calculated as:
-
-.. code-block:: python
-
-    from fn import Stream
-    from fn.iters import take, drop, map
-    from operator import add
-
-    f = Stream()
-    fib = f << [0, 1] << map(add, f, drop(1, f))
-
-    assert list(take(10, fib)) == [0,1,1,2,3,5,8,13,21,34]
-    assert fib[20] == 6765
-    assert list(fib[30:35]) == [832040,1346269,2178309,3524578,5702887]
+Lazy-evaluated Scala-style streams.  Basic idea: evaluate each new element "on
+demand" and share consumed elements between all created iterators.  A ``Stream``
+instance supports ``<<`` to push new elements.
+
+::
+
+    >>> from fn import Stream
+
+    >>> s = Stream() << [1,2,3,4,5]
+    >>> list(s)
+    [1, 2, 3, 4, 5]
+    >>> s[1]
+    2
+    >>> list(s[0:2])
+    [1, 2]
+
+    >>> s = Stream() << range(6) << [6,7]
+    >>> list(s)
+    [0, 1, 2, 3, 4, 5, 6, 7]
+
+    >>> def gen():
+    ...     yield 1
+    ...     yield 2
+    ...     yield 3
+
+    >>> s = Stream() << gen << (4,5)
+    >>> list(s)
+    [1, 2, 3, 4, 5]
+
+Lazy-evaluated streams are useful for infinite sequences, e.g. the fibonacci
+sequence can be computed as::
+
+    >>> from fn.iters import take, drop, map
+    >>> from operator import add
+
+    >>> f = Stream()
+    >>> fib = f << [0, 1] << map(add, f, drop(1, f))
+
+    >>> list(take(10, fib))
+    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
+    >>> fib[20]
+    6765
+    >>> list(fib[30:35])
+    [832040, 1346269, 2178309, 3524578, 5702887]
 
 Trampolines decorator
 ---------------------
 
-``fn.recur.tco`` is a workaround for dealing with TCO without heavy stack utilization. Let's start from simple example of recursive factorial calculation:
-
-.. code-block:: python
-
-    def fact(n):
-        if n == 0: return 1
-        return n * fact(n-1)
-
-This variant works, but it's really ugly. Why? It will utilize memory too heavy cause of recursive storing all previous values to calculate final result. If you will execute this function with big ``n`` (more than ``sys.getrecursionlimit()``) CPython will fail with
+``fn.recur.tco`` simulates TCO (tail call optimization).  Let's start with a
+simple example of recursive factorial computation::
 
-.. code-block:: python
+    >>> def fact(n):
+    ...    if n == 0: return 1
+    ...    return n * fact(n-1)
+
+This variant works, but it's really inefficient.  Why?  It will consume too much
+memory, linear in the depth of the recursion: if you execute this function
+with a big ``n`` (more than ``sys.getrecursionlimit()``) CPython will fail::
 
     >>> import sys
     >>> fact(sys.getrecursionlimit() * 2)
-    ... many many lines of stacktrace ...
-    RuntimeError: maximum recursion depth exceeded
-
-Which is good, cause it prevents you from terrible mistakes in your code.
+    Traceback (most recent call last):
+        ...
+    RecursionError: maximum recursion depth exceeded ...
 
-How can we optimize this solution? Answer is simple, lets transform function to use tail call:
+Which is good, as it prevents you from terrible mistakes in your code.
 
-.. code-block:: python
+How can we optimize this function?  Easy, let's transform it to use a tail
+call::
 
     def fact(n, acc=1):
         if n == 0: return acc
         return fact(n-1, acc*n)
 
-Why this variant is better? Cause you don't need to remember previous values to calculate final result. More about `tail call optimization <http://en.wikipedia.org/wiki/Tail_call>`_ on Wikipedia. But... Python interpreter will execute this function the same way as previous one, so you won't win anything.
-
-``fn.recur.tco`` gives you mechanism to write "optimized a bit" tail call recursion (using "trampoline" approach):
+Is this variant better?  Yes, because you don't need to remember previous values
+(local variables) to get the final result.  More about `tail call optimization
+<https://en.wikipedia.org/wiki/Tail_call>`_ on Wikipedia.  But... the Python
+interpreter will execute this function the same way as the previous one, so you
+won't win anything here.
 
-.. code-block:: python
+``fn.recur.tco`` allows you to optimize a bit this tail call recursion (using a
+"trampoline" approach)::
 
-    from fn import recur
-
-    @recur.tco
-    def fact(n, acc=1):
-        if n == 0: return False, acc
-        return True, (n-1, acc*n)
+    >>> from fn import recur
 
-``@recur.tco`` is a decorator that execute your function in ``while`` loop and check output:
+    >>> @recur.tco
+    ... def fact(n, acc=1):
+    ...    if n == 0: return False, acc
+    ...    return True, (n-1, acc*n)
 
-- ``(False, result)`` means that we finished
-- ``(True, args, kwargs)`` means that we need to call function again with other arguments
-- ``(func, args, kwargs)`` to switch function to be executed inside while loop
+``@recur.tco`` executes your function in a ``while`` loop and checks the output:
 
-The last variant is really useful, when you need to switch callable inside evaluation loop. Good example for such situation is recursive detection if given number is odd or even:
+- ``(False, result)`` means that we finished,
+- ``(True, args, kwargs)`` means that we need to recurse,
+- ``(func, args, kwargs)`` switches the function executed inside the while loop.
 
-.. code-block:: python
+Example for the third case, to recursively check the parity of a number::
 
-    >>> from fn import recur
     >>> @recur.tco
     ... def even(x):
     ...     if x == 0: return False, True
     ...     return odd, (x-1,)
     ...
     >>> @recur.tco
     ... def odd(x):
     ...     if x == 0: return False, False
     ...     return even, (x-1,)
     ...
-    >>> print even(100000)
+    >>> even(100000)
     True
 
 **Attention:** be careful with mutable/immutable data structures processing.
 
 Itertools recipes
 -----------------
 
-``fn.uniform`` provides you with "unification"
-of lazy functionality for few functions to work the same way in Python
-2+/3+:
-
--  ``map`` (returns ``itertools.imap`` in Python 2+)
--  ``filter`` (returns ``itertools.ifilter`` in Python 2+)
--  ``reduce`` (returns ``functools.reduce`` in Python 3+)
--  ``zip`` (returns ``itertools.izip`` in Python 2+)
--  ``range`` (returns ``xrange`` in Python 2+)
--  ``filterfalse`` (returns ``itertools.ifilterfalse`` in Python 2+)
--  ``zip_longest`` (returns ``itertools.izip_longest`` in Python 2+)
--  ``accumulate`` (backported to Python < 3.3)
-
-``fn.iters`` is high-level recipes to work with iterators. Most
-of them taken from `Python
-docs <http://docs.python.org/2.7/library/itertools.html#itertools.product>`_
-and adopted to work both with Python 2+/3+. Such recipes as ``drop``,
-``takelast``, ``droplast``, ``splitat``, ``splitby`` I have already
-submitted as `docs patch <http://bugs.python.org/issue16774>`_ which is
-review status just now.
+``fn.uniform`` unifies generator functions between Python versions (use
+generator versions of ``map, filter, reduce, zip, range, filterfalse,
+zip_longest``, backported ``accumulate``).
+
+``fn.iters`` offers high-level recipes for working with iterators, most of them
+are from the `itertools docs
+<https://docs.python.org/3/library/itertools.html#itertools-recipes>`_ and
+adapted for Python 2+/3+.
 
 -  ``take``, ``drop``
 -  ``takelast``, ``droplast``
 -  ``head`` (alias: ``first``), ``tail`` (alias: ``rest``)
 -  ``second``, ``ffirst``
 -  ``compact``, ``reject``
 -  ``every``, ``some``
@@ -275,180 +329,171 @@
 -  ``grouper``, ``powerset``, ``pairwise``
 -  ``roundrobin``
 -  ``partition``, ``splitat``, ``splitby``
 -  ``flatten``
 -  ``iter_except``
 -  ``first_true``
 
-More information about use cases you can find in docstrings for each
-function in `source
-code <https://github.com/kachayev/fn.py/blob/master/fn/iters.py>`__ and
-in `test
-cases <https://github.com/kachayev/fn.py/blob/master/tests.py>`_.
+See the `docstrings <fn/iters.py>`_ and `tests <tests/test_iterators.py>`_ for
+more information.
 
 High-level operations with functions
 ------------------------------------
 
-``fn.F`` is a useful function wrapper to provide easy-to-use partial
-application and functions composition.
-
-.. code-block:: python
+``fn.F`` wraps functions for easy-to-use partial application and composition::
 
-    from fn import F, _
-    from operator import add, mul
+    >>> from fn import F
+    >>> from operator import add, mul
 
     # F(f, *args) means partial application
     # same as functools.partial but returns fn.F instance
-    assert F(add, 1)(10) == 11
+    >>> F(add, 1)(10)
+    11
 
     # F << F means functions composition,
     # so (F(f) << g)(x) == f(g(x))
-    f = F(add, 1) << F(mul, 100)
-    assert list(map(f, [0, 1, 2])) == [1, 101, 201]
-    assert list(map(F() << str << (_ ** 2) << (_ + 1), range(3))) == ["1", "4", "9"]
-
-It also give you move readable in many cases "pipe" notation to deal with functions composition:
-
-.. code-block:: python
+    >>> f = F(add, 1) << F(mul, 100)
+    >>> list(map(f, [0, 1, 2]))
+    [1, 101, 201]
+    >>> list(map(F() << str << (_ ** 2) << (_ + 1), range(3)))
+    ['1', '4', '9']
 
-    from fn import F, _
-    from fn.iters import filter, range
+You can also pipe functions with ``>>``::
 
-    func = F() >> (filter, _ < 6) >> sum
-    assert func(range(10)) == 15
+    >>> from fn.iters import filter, range
 
-You can find more examples for compositions usage in ``fn._``
-implementation `source
-code <https://github.com/kachayev/fn.py/blob/master/fn/underscore.py>`__.
-
-``fn.op.apply`` executes given function with given positional arguments
-in list (or any other iterable). ``fn.op.flip`` returns you function
-that will reverse arguments order before apply.
-
-.. code-block:: python
-
-    from fn.op import apply, flip
-    from operator import add, sub
-
-    assert apply(add, [1, 2]) == 3
-    assert flip(sub)(20,10) == -10
-    assert list(map(apply, [add, mul], [(1,2), (10,20)])) == [3, 200]
-
-``fn.op.foldl`` and ``fn.op.foldr`` are folding operators. Each accepts function with arity 2 and returns function that can be used to reduce iterable to scalar: from left-to-right and from right-to-left in case of ``foldl`` and ``foldr`` respectively.
-
-.. code-block:: python
-
-    from fn import op, _
-
-    folder = op.foldr(_ * _, 1)
-    assert 6 == op.foldl(_ + _)([1,2,3])
-    assert 6 == folder([1,2,3])
+    >>> func = F() >> (filter, _ < 6) >> sum
+    >>> func(range(10))
+    15
 
-Use case specific for right-side folding is:
+You can find more examples in the ``fn._`` `implementation <fn/underscore.py>`_.
 
-.. code-block:: python
+``fn.op.apply`` executes a function with given args and kwargs.  ``fn.op.flip``
+wraps a function, flipping the order of its arguments.
 
-    from fn.op import foldr, call
+::
 
-    assert 100 == foldr(call, 0 )([lambda s: s**2, lambda k: k+10])
-    assert 400 == foldr(call, 10)([lambda s: s**2, lambda k: k+10])
+    >>> from fn.op import apply, flip
+    >>> from operator import add, sub
+
+    >>> apply(add, [1, 2])
+    3
+    >>> flip(sub)(20, 10)
+    -10
+    >>> list(map(apply, [add, mul], [(1 ,2), (10, 20)]))
+    [3, 200]
+
+``fn.op.foldl`` and ``fn.op.foldr`` create a reducer from a function of two
+arguments (think of it as curried ``reduce``).
+
+::
+
+    >>> from fn import op
+    >>> op.foldl(_ + _)([1,2,3])
+    6
+    >>> mult = op.foldr(_ * _, 1)
+    >>> mult([1,2,3])
+    6
+    >>> op.foldr(op.call, 0 )([_ ** 2, _ + 10])
+    100
+    >>> op.foldr(op.call, 10)([_ ** 2, _ + 10])
+    400
 
 
 Function currying
 -----------------
 
-``fn.func.curried`` is a decorator for building curried functions, for example:
-
-.. code-block:: python
+::
 
     >>> from fn.func import curried
     >>> @curried
     ... def sum5(a, b, c, d, e):
     ...     return a + b + c + d + e
     ...
     >>> sum5(1)(2)(3)(4)(5)
     15
     >>> sum5(1, 2, 3)(4, 5)
     15
 
 
-Functional style for error-handling
+Functional style error-handling
 -----------------------------------
 
-``fn.monad.Option`` represents optional values, each instance of ``Option`` can be either instance of ``Full`` or ``Empty``. It provides you with simple way to write long computation sequences and get rid of many ``if/else`` blocks. See usage examples below.
-
-Assume that you have ``Request`` class that gives you parameter value by its name. To get uppercase notation for non-empty striped value:
+``fn.monad.Option`` represents optional values, each instance of ``Option`` can
+be either ``Full`` or ``Empty``.  It provides you with a simple way to write
+long computation sequences and get rid of many ``if/else`` blocks.  See usage
+examples below.
+
+Assume that you have a ``Request`` class that gives you a parameter value by its
+name, and you have to convert it to uppercase and strip it::
+
+    >>> class Request(dict):
+    ...     def parameter(self, name):
+    ...         return self.get(name, None)
+
+    >>> r = Request(testing="Fixed", empty="   ")
+    >>> param = r.parameter("testing")
+    >>> if param is None:
+    ...     fixed = ""
+    ... else:
+    ...     param = param.strip()
+    ...     if len(param) == 0:
+    ...         fixed = ""
+    ...     else:
+    ...         fixed = param.upper()
+    >>> fixed
+    'FIXED'
+
+
+Hmm, looks ugly..  But now with ``fn.monad.Option``::
+
+    >>> from operator import methodcaller
+    >>> from fn.monad import optionable
+
+    >>> class Request(dict):
+    ...     @optionable
+    ...     def parameter(self, name):
+    ...         return self.get(name, None)
+
+    >>> r = Request(testing="Fixed", empty="   ")
+    >>> (r
+    ...     .parameter("testing")
+    ...     .map(methodcaller("strip"))
+    ...     .filter(len)
+    ...     .map(methodcaller("upper"))
+    ...     .get_or("")
+    ... )
+    'FIXED'
 
-.. code-block:: python
-
-    class Request(dict):
-        def parameter(self, name):
-            return self.get(name, None)
-
-    r = Request(testing="Fixed", empty="   ")
-    param = r.parameter("testing")
-    if param is None:
-        fixed = ""
-    else:
-        param = param.strip()
-        if len(param) == 0:
-            fixed = ""
-        else:
-            fixed = param.upper()
-
-
-Hmm, looks ugly.. Update code with ``fn.monad.Option``:
-
-.. code-block:: python
-
-    from operator import methodcaller
-    from fn.monad import optionable
-
-    class Request(dict):
-        @optionable
-        def parameter(self, name):
-            return self.get(name, None)
-
-    r = Request(testing="Fixed", empty="   ")
-    fixed = r.parameter("testing")
-             .map(methodcaller("strip"))
-             .filter(len)
-             .map(methodcaller("upper"))
-             .get_or("")
-
-``fn.monad.Option.or_call`` is good method for trying several variant to end computation. I.e. use have ``Request`` class with optional attributes ``type``, ``mimetype``, ``url``. You need to evaluate "request type" using at least one attribute:
-
-.. code-block:: python
+Use ``or_call`` for more complex alternatives, for example::
 
     from fn.monad import Option
 
     request = dict(url="face.png", mimetype="PNG")
-    tp = Option \
-            .from_value(request.get("type", None)) \ # check "type" key first
-            .or_call(from_mimetype, request) \ # or.. check "mimetype" key
-            .or_call(from_extension, request) \ # or... get "url" and check extension
-            .get_or("application/undefined")
+    tp = (Option 
+        .from_value(request.get("type", None))  # check "type" key first
+        .or_call(from_mimetype, request)  # or.. check "mimetype" key
+        .or_call(from_extension, request)  # or... get "url" and check extension
+        .get_or("application/undefined")
+    )
 
 
 Installation
 ------------
 
-To install ``fn.py``, simply:
-
-.. code-block:: console
+To install ``fn.py``, simply::
 
     $ pip install fn.py
 
 You can also build library from source
 
-.. code-block:: console
+::
 
     $ git clone https://github.com/fnpy/fn.py.git
-    $ cd fn.py
-    $ python setup.py install
+    $ pip install -e fn.py
 
 Work in progress
 ----------------
 
 "Roadmap":
 
 - ``fn.monad.Either`` to deal with error logging
@@ -457,15 +502,15 @@
 Ideas to think about:
 
 -  Scala-style for-yield loop to simplify long map/filter blocks
 
 Contribute
 ----------
 
-If you found a bug:
+If you find a bug:
 
 1. Check for open issues or open a fresh issue to start a discussion
    around a feature idea or a bug.
 2. Fork the repository on Github to start making your changes to the
    master branch (or branch off of it).
 3. Write a test which shows that the bug was fixed or that the feature
    works as expected.
@@ -476,12 +521,55 @@
    it or collaborate with those who have claimed it.
 2. Fork the repository on Github to start making your changes to the
    master branch (or branch off of it).
 3. Write a test which shows that the bug was fixed or that the feature
    works as expected.
 
 How to contact the maintainers
---------------
+------------------------------
 
 - Gitter: https://gitter.im/fnpy/fn.py
 - Jacob's (Organization Owner) Email: him <at> jacobandkate143.com
 - Alex's (Original Project Owner) Email: kachayev <at> gmail.com
+
+
+Changelog
+=========
+
+(v0.6.0) June 14, 2023
+----------------------
+
+Commit `ef005bd <https://github.com/fnpy/fn.py/commit/ef005bdc89aae0494b18792834a1dd47a027036c>`_ by `jacobbridges <https://github.com/jacobbridges>`_ on Jun 14, 2023
+
+- `Pull Request #46 <https://github.com/fnpy/fn.py/pull/46>`_
+- Switch from TravisCI to Github Actions
+
+
+Commit `d8c21ab <https://github.com/fnpy/fn.py/commit/d8c21abef1db3bf558b4d90469483461d4149210>`_ by `artemisart <https://github.com/artemisart>`_ on Apr 25, 2020
+
+- `Pull Request #40 <https://github.com/fnpy/fn.py/pull/40>`_
+- Documentation + some fixes
+
+
+Commit `9958f1f <https://github.com/fnpy/fn.py/commit/9958f1f8678f27239760e17a8866288875519a7e>`_ by `soasme <https://github.com/soasme>`_ on Sep 5, 2019
+
+- `Pull Request #39 <https://github.com/fnpy/fn.py/pull/39>`_
+- Import Iterable from collections.abc for >=3.8
+
+
+Commit `486119e <https://github.com/fnpy/fn.py/commit/486119e4d25892c8a8052826fd392601ad6e4d4e>`_ by `fwfurtado <https://github.com/fwfurtado>`_ on Sep 5, 2019
+
+- `Pull Request #37 <https://github.com/fnpy/fn.py/pull/37>`_
+- Added supporting to type hint in curried decorator
+
+
+Commit `c01c2b7 <https://github.com/fnpy/fn.py/commit/c01c2b7235e0ef8b65a53b91df560c7e01c50027>`_ by `katoken-0215 <https://github.com/katoken-0215>`_ on Mar 24, 2018
+
+- `Pull Request #33 <https://github.com/fnpy/fn.py/pull/33>`_
+- Introduce guard for recursive call by doctest.
+
+(v0.5.0) July 17, 2017
+----------------------
+
+Commit: `10efa8b <https://github.com/fnpy/fn.py/commit/10efa8b35c327ae77dfb01878451694bd5a47ea9>`_.
+
+- Added ``recur.stackless()`` Provides a "stackless" (constant Python stack space) recursion decorator for generators.
```

### Comparing `fn.py-0.5.2/setup.py` & `fn.py-0.6.0/setup.py`

 * *Files identical despite different names*

