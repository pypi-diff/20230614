# Comparing `tmp/pymox-1.0.1.tar.gz` & `tmp/pymox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymox-1.0.1.tar", max compression
+gzip compressed data, was "pymox-1.0.2.tar", max compression
```

## Comparing `pymox-1.0.1.tar` & `pymox-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      991 2023-06-10 12:41:09.548531 pymox-1.0.1/README.rst
--rw-r--r--   0        0        0      732 2023-06-10 12:36:46.185084 pymox-1.0.1/mox/__init__.py
--rwxr-xr-x   0        0        0    73306 2023-06-10 12:36:46.186655 pymox-1.0.1/mox/mox.py
--rw-r--r--   0        0        0     5368 2023-06-10 12:36:46.188124 pymox-1.0.1/mox/stubout.py
--rw-r--r--   0        0        0     2271 2023-06-10 12:41:16.705049 pymox-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 pymox-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11875 2023-06-14 11:36:14.149469 pymox-1.0.2/README.rst
+-rw-r--r--   0        0        0      991 2023-06-14 11:22:28.830014 pymox-1.0.2/mox/__init__.py
+-rwxr-xr-x   0        0        0    74885 2023-06-14 11:36:37.635178 pymox-1.0.2/mox/mox.py
+-rw-r--r--   0        0        0     5488 2023-06-14 11:22:28.832449 pymox-1.0.2/mox/stubout.py
+-rw-r--r--   0        0        0     2271 2023-06-14 11:37:46.154860 pymox-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13811 1970-01-01 00:00:00.000000 pymox-1.0.2/PKG-INFO
```

### Comparing `pymox-1.0.1/mox/mox.py` & `pymox-1.0.2/mox/mox.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 
     def __init__(self):
         """Initialize a new Mox."""
 
         self._mock_objects = []
         self.stubs = stubout.StubOutForTesting()
 
-    def CreateMock(self, class_to_mock, attrs=None):
+    def create_mock(self, class_to_mock, attrs=None):
         """Create a new mock object.
 
         Args:
           # class_to_mock: the class to be mocked
           class_to_mock: class
           attrs: dict of attribute names to values that will be set on the mock
             object.  Only public attributes may be set.
@@ -298,46 +298,46 @@
         """
         if attrs is None:
             attrs = {}
         new_mock = MockObject(class_to_mock, attrs=attrs)
         self._mock_objects.append(new_mock)
         return new_mock
 
-    def CreateMockAnything(self, description=None):
+    def create_mock_anything(self, description=None):
         """Create a mock that will accept any method calls.
 
         This does not enforce an interface.
 
         Args:
           description: str. Optionally, a descriptive name for the mock object
             being created, for debugging output purposes.
         """
         new_mock = MockAnything(description=description)
         self._mock_objects.append(new_mock)
         return new_mock
 
-    def ReplayAll(self):
+    def replay_all(self):
         """Set all mock objects to replay mode."""
 
         for mock_obj in self._mock_objects:
             mock_obj._Replay()
 
-    def VerifyAll(self):
+    def verify_all(self):
         """Call verify on all mock objects created."""
 
         for mock_obj in self._mock_objects:
             mock_obj._Verify()
 
-    def ResetAll(self):
+    def reset_all(self):
         """Call reset on all mock objects.  This does not unset stubs."""
 
         for mock_obj in self._mock_objects:
             mock_obj._Reset()
 
-    def StubOutWithMock(self, obj, attr_name, use_mock_anything=False):
+    def stubout(self, obj, attr_name, use_mock_anything=False):
         """Replace a method, attribute, etc. with a Mock.
 
         This will replace a class or module with a MockObject, and everything
         else (method, function, etc) with a MockAnything.  This can be
         overridden to always use a MockAnything by setting use_mock_anything to
         True.
 
@@ -348,15 +348,15 @@
             regardless of the type of attribute.
         """
 
         attr_to_replace = getattr(obj, attr_name)
         attr_type = type(attr_to_replace)
 
         if attr_type == MockAnything or attr_type == MockObject:
-            raise TypeError("Cannot mock a MockAnything! Did you remember to " "call UnsetStubs in your previous test?")
+            raise TypeError("Cannot mock a MockAnything! Did you remember to call unset_stubs in your previous test?")
 
         if (
             attr_type in self._USE_MOCK_OBJECT
             or
             # isinstance(attr_type, tuple(self._USE_MOCK_OBJECT)) or
             isinstance(attr_to_replace, object)
             or inspect.isclass(attr_to_replace)
@@ -364,21 +364,21 @@
             stub = self.CreateMock(attr_to_replace)
         else:
             stub = self.CreateMockAnything(description="Stub for %s" % attr_to_replace)
             stub.__name__ = attr_name
 
         self.stubs.Set(obj, attr_name, stub)
 
-    def StubOutClassWithMocks(self, obj, attr_name):
+    def stubout_class(self, obj, attr_name):
         """Replace a class with a "mock factory" that will create mock objects.
 
         This is useful if the code-under-test directly instantiates
-        dependencies.  Previously some boilder plate was necessary to
+        dependencies.  Previously some boilerplate was necessary to
         create a mock that would act as a factory.  Using
-        StubOutClassWithMocks, once you've stubbed out the class you may
+        stubout_class, once you've stubbed out the class you may
         use the stubbed class as you would any other mock created by mox:
         during the record phase, new mock instances will be created, and
         during replay, the recorded mocks will be returned.
 
         In replay mode
 
         # Example using StubOutWithMock (the old, clunky way):
@@ -406,60 +406,78 @@
         my_import.FooClass(9, 10)  # Returns mock2 again.
         mox.VerifyAll()
         """
         attr_to_replace = getattr(obj, attr_name)
         attr_type = type(attr_to_replace)
 
         if attr_type == MockAnything or attr_type == MockObject:
-            raise TypeError("Cannot mock a MockAnything! Did you remember to " "call UnsetStubs in your previous test?")
+            raise TypeError("Cannot mock a MockAnything! Did you remember to call unset_stubs in your previous test?")
 
         if not inspect.isclass(attr_to_replace):
-            raise TypeError("Given attr is not a Class.  Use StubOutWithMock.")
+            raise TypeError("Given attr is not a Class. Use stubout.")
 
         factory = _MockObjectFactory(attr_to_replace, self)
         self._mock_objects.append(factory)
         self.stubs.Set(obj, attr_name, factory)
 
-    def UnsetStubs(self):
+    def unset_stubs(self):
         """Restore stubs to their original state."""
 
-        self.stubs.UnsetAll()
+        self.stubs.unset_all()
 
+    CreateMock = create_mock
+    CreateMockAnything = create_mock_anything
+    ReplayAll = replay_all
+    VerifyAll = verify_all
+    ResetAll = reset_all
+    StubOutWithMock = stubout
+    StubOutClassWithMocks = stubout_class
+    UnsetStubs = unset_stubs
 
-def Replay(*args):
+
+def replay(*args):
     """Put mocks into Replay mode.
 
     Args:
       # args is any number of mocks to put into replay mode.
     """
 
     for mock in args:
-        mock._Replay()
+        mock._replay()
+
+
+Replay = replay
 
 
-def Verify(*args):
+def verify(*args):
     """Verify mocks.
 
     Args:
       # args is any number of mocks to be verified.
     """
 
     for mock in args:
-        mock._Verify()
+        mock._verify()
 
 
-def Reset(*args):
+Verify = verify
+
+
+def reset(*args):
     """Reset mocks.
 
     Args:
       # args is any number of mocks to be reset.
     """
 
     for mock in args:
-        mock._Reset()
+        mock._reset()
+
+
+Reset = reset
 
 
 class MockAnything:
     """A mock that can be used to mock anything.
 
     This is helpful for mocking classes that do not provide a public interface.
     """
@@ -469,15 +487,15 @@
 
         Args:
           description: str. Optionally, a descriptive name for the mock object
             being created, for debugging output purposes.
         """
         self._description = description
         self._exceptions_thrown = []
-        self._Reset()
+        self._reset()
 
     def __bases__(self):
         pass
 
     def __members__(self):
         pass
 
@@ -487,21 +505,21 @@
     def __repr__(self):
         if self._description:
             return "<MockAnything instance of %s>" % self._description
         else:
             return "<MockAnything instance>"
 
     def __str__(self):
-        return self._CreateMockMethod("__str__")()
+        return self._create_mock_method("__str__")()
 
     def __call__(self, *args, **kwargs):
-        return self._CreateMockMethod("__call__")(*args, **kwargs)
+        return self._create_mock_method("__call__")(*args, **kwargs)
 
     def __getitem__(self, i):
-        return self._CreateMockMethod("__getitem__")(i)
+        return self._create_mock_method("__getitem__")(i)
 
     def __getattr__(self, method_name):
         """Intercept method calls on this object.
 
          A new MockMethod is returned that is aware of the MockAnything's
          state (record or replay).  The call will be recorded or replayed
          by the MockMethod's __call__.
@@ -512,17 +530,17 @@
 
         Returns:
           A new MockMethod aware of MockAnything's state (record or replay).
         """
         if method_name == "__dir__":
             return self.__class__.__dir__.__get__(self, self.__class__)
 
-        return self._CreateMockMethod(method_name)
+        return self._create_mock_method(method_name)
 
-    def _CreateMockMethod(self, method_name, method_to_mock=None):
+    def _create_mock_method(self, method_name, method_to_mock=None):
         """Create a new mock method call and return it.
 
         Args:
           # method_name: the name of the method being called.
           # method_to_mock: The actual method being mocked, used for
           #   introspection.
           method_name: str
@@ -556,21 +574,21 @@
         )
 
     def __ne__(self, rhs):
         """Provide custom logic to compare objects."""
 
         return not self == rhs
 
-    def _Replay(self):
+    def _replay(self):
         """Start replaying expected method calls."""
 
         self._replay_mode = True
 
-    def _Verify(self):
-        """Verify that all of the expected calls have been made.
+    def _verify(self):
+        """Verify that all the expected calls have been made.
 
         Raises:
           ExpectedMethodCallsError: if there are still more method calls in the
             expected queue.
           any exception previously raised by this object: if _Verify was called
           afterwards anyway.  (This detects tests passing erroneously.)
         """
@@ -590,23 +608,27 @@
                 and is_multiple_times_group
                 and self._expected_calls_queue[0].IsSatisfied()
             ):
                 pass
             else:
                 raise ExpectedMethodCallsError(self._expected_calls_queue)
 
-    def _Reset(self):
+    def _reset(self):
         """Reset the state of this mock to record mode with an empty queue."""
 
         # Maintain a list of method calls we are expecting
         self._expected_calls_queue = deque()
 
         # Make sure we are in setup mode, not replay mode
         self._replay_mode = False
 
+    _Replay = _replay
+    _Verify = _verify
+    _Reset = _reset
+
 
 class MockObject(MockAnything, object):
     """A mock object that simulates the public/protected interface of a class."""
 
     def __init__(self, class_to_mock, attrs=None):
         """Initialize a mock object.
 
@@ -708,15 +730,15 @@
               method.
         """
 
         if name in self._known_vars:
             return getattr(self._class_to_mock, name)
 
         if name in self._known_methods:
-            return self._CreateMockMethod(name, method_to_mock=getattr(self._class_to_mock, name))
+            return self._create_mock_method(name, method_to_mock=getattr(self._class_to_mock, name))
 
         exception = UnknownMethodCallError(name)
         self._exceptions_thrown.append(exception)
         raise exception
 
     def __eq__(self, rhs):
         """Provide custom logic to compare objects."""
@@ -758,15 +780,15 @@
                 "__setitem__",
                 self._expected_calls_queue,
                 self._exceptions_thrown,
                 self._replay_mode,
             )(key, value)
 
         # Otherwise, create a mock method __setitem__.
-        return self._CreateMockMethod("__setitem__")(key, value)
+        return self._create_mock_method("__setitem__")(key, value)
 
     def __getitem__(self, key):
         """Provide custom logic for mocking classes that are subscriptable.
 
         Args:
           key: Key to return the value for.
 
@@ -792,15 +814,15 @@
                 "__getitem__",
                 self._expected_calls_queue,
                 self._exceptions_thrown,
                 self._replay_mode,
             )(key)
 
         # Otherwise, create a mock method __getitem__.
-        return self._CreateMockMethod("__getitem__")(key)
+        return self._create_mock_method("__getitem__")(key)
 
     def __iter__(self):
         """Provide custom logic for mocking classes that are iterable.
 
         Returns:
           Expected return value in replay mode.  A MockMethod object for the
           __iter__ method that has already been called if not in replay mode.
@@ -835,15 +857,15 @@
                 "__iter__",
                 self._expected_calls_queue,
                 self._exceptions_thrown,
                 self._replay_mode,
             )()
 
         # Otherwise, create a mock method __iter__.
-        return self._CreateMockMethod("__iter__")()
+        return self._create_mock_method("__iter__")()
 
     def __contains__(self, key):
         """Provide custom logic for mocking classes that contain items.
 
         Args:
           key: Key to look in container for.
 
@@ -867,15 +889,15 @@
             return MockMethod(
                 "__contains__",
                 self._expected_calls_queue,
                 self._exceptions_thrown,
                 self._replay_mode,
             )(key)
 
-        return self._CreateMockMethod("__contains__")(key)
+        return self._create_mock_method("__contains__")(key)
 
     def __call__(self, *params, **named_params):
         """Provide custom logic for mocking classes that are callable."""
 
         # Verify the class we are mocking is callable.
         callable = hasattr(self._class_to_mock, "__call__")
         # callable = callable and str(
@@ -892,15 +914,15 @@
         # If we are mocking a Function, then use the function, and not the
         # __call__ method
         method = None
         if type(self._class_to_mock) in (types.FunctionType, types.MethodType):
             method = self._class_to_mock
         else:
             method = getattr(self._class_to_mock, "__call__")
-        mock_method = self._CreateMockMethod("__call__", method_to_mock=method)
+        mock_method = self._create_mock_method("__call__", method_to_mock=method)
 
         return mock_method(*params, **named_params)
 
     @property
     def __class__(self):
         """Return the class that is being mocked."""
 
@@ -911,15 +933,15 @@
         """Return the name that is being mocked."""
         return self._description
 
 
 class _MockObjectFactory(MockObject):
     """A MockObjectFactory creates mocks and verifies __init__ params.
 
-    A MockObjectFactory removes the boiler plate code that was previously
+    A MockObjectFactory removes the boilerplate code that was previously
     necessary to stub out direction instantiation of a class.
 
     The MockObjectFactory creates new MockObjects when called and verifies the
     __init__ params are correct when in record mode.  When replaying, existing
     mocks are returned, and the __init__ params are verified.
 
     See StubOutWithMock vs StubOutClassWithMocks for more detail.
@@ -930,15 +952,15 @@
         self._mox = mox_instance
         self._instance_queue = deque()
 
     def __call__(self, *params, **named_params):
         """Instantiate and record that a new mock has been created."""
 
         method = getattr(self._class_to_mock, "__init__")
-        mock_method = self._CreateMockMethod("__init__", method_to_mock=method)
+        mock_method = self._create_mock_method("__init__", method_to_mock=method)
         # Note: calling mock_method() is deferred in order to catch the
         # empty instance_queue first.
 
         if self._replay_mode:
             if not self._instance_queue:
                 exception = UnexpectedMockCreationError(self._class_to_mock, *params, **named_params)
                 self._exceptions_thrown.append(exception)
@@ -950,19 +972,21 @@
         else:
             mock_method(*params, **named_params)
 
             instance = self._mox.CreateMock(self._class_to_mock)
             self._instance_queue.appendleft(instance)
             return instance
 
-    def _Verify(self):
+    def _verify(self):
         """Verify that all mocks have been created."""
         if self._instance_queue:
             raise ExpectedMockCreationError(self._instance_queue)
-        super(_MockObjectFactory, self)._Verify()
+        super(_MockObjectFactory, self)._verify()
+
+    _Verify = _verify
 
 
 class MethodSignatureChecker(object):
     """Ensures that methods are called correctly."""
 
     _NEEDED, _DEFAULT, _GIVEN = range(3)
 
@@ -991,15 +1015,15 @@
         if defaults is None:
             self._required_args = self._args
             self._default_args = []
         else:
             self._required_args = self._args[: -len(defaults)]
             self._default_args = self._args[-len(defaults):]
 
-    def _RecordArgumentGiven(self, arg_name, arg_status):
+    def _record_argument_given(self, arg_name, arg_status):
         """Mark an argument as being given.
 
         Args:
           # arg_name: The name of the argument to mark in arg_status.
           # arg_status: Maps argument names to one of _NEEDED, _DEFAULT,
           #  _GIVEN.
           arg_name: string
@@ -1008,15 +1032,15 @@
         Raises:
           AttributeError: arg_name is already marked as _GIVEN.
         """
         if arg_status.get(arg_name, None) == MethodSignatureChecker._GIVEN:
             raise AttributeError("%s provided more than once" % (arg_name,))
         arg_status[arg_name] = MethodSignatureChecker._GIVEN
 
-    def Check(self, params, named_params):
+    def check(self, params, named_params):
         """Ensures that the parameters used while recording a call are valid.
 
         Args:
           # params: A list of positional parameters.
           # named_params: A dict of named parameters.
           params: list
           named_params: dict
@@ -1096,27 +1120,30 @@
                 arg_name = self._args[i]
             except IndexError:
                 if not self._has_varargs:
                     raise AttributeError(
                         "%s does not take %d or more positional " "arguments" % (self._method.__name__, i)
                     )
             else:
-                self._RecordArgumentGiven(arg_name, arg_status)
+                self._record_argument_given(arg_name, arg_status)
 
         # Check each keyword argument.
         for arg_name in named_params:
             if arg_name not in arg_status and not self._has_varkw:
                 raise AttributeError("%s is not expecting keyword argument %s" % (self._method.__name__, arg_name))
-            self._RecordArgumentGiven(arg_name, arg_status)
+            self._record_argument_given(arg_name, arg_status)
 
         # Ensure all the required arguments have been given.
         still_needed = [k for k, v in arg_status.items() if v == MethodSignatureChecker._NEEDED]
         if still_needed:
             raise AttributeError("No values given for arguments: %s" % (" ".join(sorted(still_needed))))
 
+    _RecordArgumentGiven = _record_argument_given
+    Check = check
+
 
 class MockMethod(object):
     """Callable mock method.
 
     A MockMethod should act exactly like the method it mocks, accepting
     parameters and returning a value, or throwing an exception (as specified).
     When this method is called, it can optionally verify whether the called
@@ -1222,24 +1249,24 @@
 
     def __next__(self):
         """Raise a TypeError with a helpful message."""
         raise TypeError("MockMethod cannot be iterated. " "Did you remember to put your mocks in replay mode?")
 
     next = __next__
 
-    def _PopNextMethod(self):
+    def _pop_next_method(self):
         """Pop the next method from our call queue."""
         try:
             return self._call_queue.popleft()
         except IndexError:
             exception = UnexpectedMethodCallError(self, None)
             self._exception_list.append(exception)
             raise exception
 
-    def _VerifyMethodCall(self):
+    def _verify_method_call(self):
         """Verify the called method is expected.
 
         This can be an ordered method, or part of an unordered set.
 
         Returns:
           The expected mock method.
 
@@ -1297,15 +1324,15 @@
         Args:
           # rhs: the right hand side of the test
           rhs: MockMethod
         """
 
         return not self == rhs
 
-    def GetPossibleGroup(self):
+    def get_possible_group(self):
         """Returns a possible group from the end of the call queue or None if no
         other methods are on the stack.
         """
 
         # Remove this method from the tail of the queue so we can add it to a
         # group.
         this_method = self._call_queue.pop()
@@ -1318,38 +1345,38 @@
         try:
             group = self._call_queue[-1]
         except IndexError:
             pass
 
         return group
 
-    def _CheckAndCreateNewGroup(self, group_name, group_class):
+    def _check_and_create_new_group(self, group_name, group_class):
         """Checks if the last method (a possible group) is an instance of our
         group_class. Adds the current method to this group or creates a new
         one.
 
         Args:
 
           group_name: the name of the group.
           group_class: the class used to create instance of this new group
         """
-        group = self.GetPossibleGroup()
+        group = self.get_possible_group()
 
         # If this is a group, and it is the correct group, add the method.
         if isinstance(group, group_class) and group.group_name() == group_name:
             group.AddMethod(self)
             return self
 
         # Create a new group and add the method.
         new_group = group_class(group_name, self._exception_list)
         new_group.AddMethod(self)
         self._call_queue.append(new_group)
         return self
 
-    def InAnyOrder(self, group_name="default"):
+    def any_order(self, group_name="default"):
         """Move this method into a group of unordered calls.
 
         A group of unordered calls must be defined together, and must be
         executed in full before the next expected method can be called. There
         can be multiple groups that are expected serially, if they are given
         different group names.  The same group name can be reused if there is a
         standard method call, or a group with a different name, spliced between
@@ -1357,64 +1384,74 @@
 
         Args:
           group_name: the name of the unordered group.
 
         Returns:
           self
         """
-        return self._CheckAndCreateNewGroup(group_name, UnorderedGroup)
+        return self._check_and_create_new_group(group_name, UnorderedGroup)
 
-    def MultipleTimes(self, group_name="default"):
+    def multiple_times(self, group_name="default"):
         """Move this method into group of calls which may be called multiple
         times.
 
         A group of repeating calls must be defined together, and must be
         executed in full before the next expected method can be called.
 
         Args:
           group_name: the name of the unordered group.
 
         Returns:
           self
         """
-        return self._CheckAndCreateNewGroup(group_name, MultipleTimesGroup)
+        return self._check_and_create_new_group(group_name, MultipleTimesGroup)
 
-    def AndReturn(self, return_value):
+    def returns(self, return_value):
         """Set the value to return when this method is called.
 
         Args:
           # return_value can be anything.
         """
 
         self._return_value = return_value
         return return_value
 
-    def AndRaise(self, exception):
+    def raises(self, exception):
         """Set the exception to raise when this method is called.
 
         Args:
           # exception: the exception to raise when this method is called.
           exception: Exception
         """
 
         self._exception = exception
 
-    def WithSideEffects(self, side_effects):
+    def with_side_effects(self, side_effects):
         """Set the side effects that are simulated when this method is called.
 
         Args:
           side_effects: A callable which modifies the parameters or other
             relevant state which a given test case depends on.
 
         Returns:
           Self for chaining with AndReturn and AndRaise.
         """
         self._side_effects = side_effects
         return self
 
+    _PopNextMethod = _pop_next_method
+    _VerifyMethodCall = _verify_method_call
+    GetPossibleGroup = get_possible_group
+    _CheckAndCreateNewGroup = _check_and_create_new_group
+    InAnyOrder = any_order
+    MultipleTimes = multiple_times
+    AndReturn = returns
+    AndRaise = raises
+    WithSideEffects = with_side_effects
+
 
 class Comparator:
     """Base class for all Mox comparators.
 
     A Comparator can be used as a parameter to a mocked method when the exact
     value is not known.  For example, the code you are testing might build up a
     long SQL string that is passed to your mock DAO. You're only interested
@@ -1460,14 +1497,17 @@
     def equals(self, rhs):
         return rhs is self._obj
 
     def __repr__(self):
         return "<is %r (%s)>" % (self._obj, id(self._obj))
 
 
+is_ = Is
+
+
 class IsA(Comparator):
     """This class wraps a basic Python type or class.  It is used to verify
     that a parameter is of the given type or class.
 
     Example:
     mock_dao.Connect(IsA(DbConnectInfo))
     """
@@ -1495,15 +1535,15 @@
         try:
             return isinstance(rhs, self._class_name)
         except TypeError:
             # Check raw types if there was a type error.  This is helpful for
             # things like cStringIO.StringIO.
             return isinstance(rhs, type(self._class_name))
 
-    def _IsSubClass(self, clazz):
+    def _is_subclass(self, clazz):
         """Check to see if the IsA comparators class is a subclass of clazz.
 
         Args:
           # clazz: a class object
 
         Returns:
           bool
@@ -1515,14 +1555,19 @@
             # Check raw types if there was a type error.  This is helpful for
             # things like cStringIO.StringIO.
             return isinstance(clazz, type(self._class_name))
 
     def __repr__(self):
         return "mox.IsA(%s) " % str(self._class_name)
 
+    _IsSubClass = _is_subclass
+
+
+is_a = IsA
+
 
 class IsAlmost(Comparator):
     """Comparison class used to check whether a parameter is nearly equal
     to a given value.  Generally useful for floating point numbers.
 
     Example mock_dao.SetTimeout((IsAlmost(3.9)))
     """
@@ -1555,14 +1600,17 @@
             # number.
             return False
 
     def __repr__(self):
         return str(self._float_value)
 
 
+is_almost = IsAlmost
+
+
 class StrContains(Comparator):
     """Comparison class used to check whether a substring exists in a
     string parameter.  This can be useful in mocking a database with SQL
     passed in as a string parameter, for example.
 
     Example:
     mock_dao.RunQuery(StrContains('IN (1, 2, 4, 5)')).AndReturn(mock_result)
@@ -1594,14 +1642,17 @@
         except Exception:
             return False
 
     def __repr__(self):
         return "<str containing '%s'>" % self._search_string
 
 
+str_contains = StrContains
+
+
 class Regex(Comparator):
     """Checks if a string matches a regular expression.
 
     This uses a given regular expression to determine equality.
     """
 
     def __init__(self, pattern, flags=0):
@@ -1635,26 +1686,29 @@
         s = "<regular expression '{}'".format(pattern)
         if self.regex.flags:
             s += ", flags=%d" % self.regex.flags
         s += ">"
         return s
 
 
+regex = Regex
+
+
 class In(Comparator):
     """Checks whether an item (or key) is in a list (or dict) parameter.
 
     Example:
     mock_dao.GetUsersInfo(In('expectedUserName')).AndReturn(mock_result)
     """
 
     def __init__(self, key):
         """Initialize.
 
         Args:
-          # key is any thing that could be in a list or a key in a dict
+          # key is anything that could be in a list or a key in a dict
         """
 
         self._key = key
 
     def equals(self, rhs):
         """Check to see whether key is in rhs.
 
@@ -1670,14 +1724,17 @@
         except Exception:
             return False
 
     def __repr__(self):
         return "<sequence or map containing '%s'>" % str(self._key)
 
 
+in_ = In
+
+
 class Not(Comparator):
     """Checks whether a predicates is False.
 
     Example:
       mock_dao.UpdateUsers(Not(ContainsKeyValue('stevepm', stevepm_user_info)))
     """
 
@@ -1707,14 +1764,17 @@
         except Exception:
             return False
 
     def __repr__(self):
         return "<not '%s'>" % self._predicate
 
 
+not_ = Not
+
+
 class ContainsKeyValue(Comparator):
     """Checks whether a key/value pair is in a dict parameter.
 
     Example:
     mock_dao.UpdateUsers(ContainsKeyValue('stevepm', stevepm_user_info))
     """
 
@@ -1744,14 +1804,17 @@
     def __repr__(self):
         return "<map containing the entry '%s: %s'>" % (
             str(self._key),
             str(self._value),
         )
 
 
+contains_key_value = ContainsKeyValue
+
+
 class ContainsAttributeValue(Comparator):
     """Checks whether a passed parameter contains attributes with a given
     value.
 
     Example:
     mock_dao.UpdateSomething(ContainsAttribute('stevepm', stevepm_user_info))
     """
@@ -1777,14 +1840,17 @@
 
         try:
             return getattr(rhs, self._key) == self._value
         except Exception:
             return False
 
 
+contains_attribute_value = ContainsAttributeValue
+
+
 class SameElementsAs(Comparator):
     """Checks whether sequences contain the same elements (ignoring order).
 
     Example:
     mock_dao.ProcessUsers(SameElementsAs('stevepm', 'salomaki'))
     """
 
@@ -1835,14 +1901,17 @@
         else:
             return set(actual_list) == set(self._expected_list)
 
     def __repr__(self):
         return "<sequence with same elements as '%s'>" % self._expected_list
 
 
+same_elements_as = SameElementsAs
+
+
 class And(Comparator):
     """Evaluates one or more Comparators on RHS and returns an AND of the
     results.
     """
 
     def __init__(self, *args):
         """Initialize.
@@ -1869,14 +1938,17 @@
 
         return True
 
     def __repr__(self):
         return "<AND %s>" % str(self._comparators)
 
 
+and_ = And
+
+
 class Or(Comparator):
     """Evaluates one or more Comparators on RHS and returns an OR of the
     results.
     """
 
     def __init__(self, *args):
         """Initialize.
@@ -1903,14 +1975,17 @@
 
         return False
 
     def __repr__(self):
         return "<OR %s>" % str(self._comparators)
 
 
+or_ = Or
+
+
 class Func(Comparator):
     """Call a function that should verify the parameter passed in is correct.
 
     You may need the ability to perform more advanced operations on the
     parameter in order to validate it.  You can use this to have a callable
     validate any parameter. The callable should return either True or False.
 
@@ -1947,14 +2022,17 @@
 
         return self._func(rhs)
 
     def __repr__(self):
         return str(self._func)
 
 
+func = Func
+
+
 class IgnoreArg(Comparator):
     """Ignore an argument.
 
     This can be used when we don't care about an argument of a method call.
 
     Example:
     # Check if CastMagic is called with 3 as first arg and 'disappear' as
@@ -1973,14 +2051,17 @@
 
         return True
 
     def __repr__(self):
         return "<IgnoreArg>"
 
 
+ignore_arg = IgnoreArg
+
+
 class Value(Comparator):
     """Compares argument against a remembered value.
 
     To be used in conjunction with Remember comparator.  See Remember()
     for example.
     """
 
@@ -2001,14 +2082,17 @@
     def __repr__(self):
         if self._has_value:
             return "<Value %r>" % self._value
         else:
             return "<Value>"
 
 
+value = Value
+
+
 class Remember(Comparator):
     """Remembers the argument to a value store.
 
     To be used in conjunction with Value comparator.
 
     Example:
     # Remember the argument for one method call.
@@ -2028,14 +2112,17 @@
         self._value_store.store_value(rhs)
         return True
 
     def __repr__(self):
         return "<Remember %d>" % id(self._value_store)
 
 
+remember = Remember
+
+
 class MethodGroup(object):
     """Base class containing common behaviour for MethodGroups."""
 
     def __init__(self, group_name, exception_list):
         """Construct a new method group.
 
         Args:
@@ -2050,23 +2137,27 @@
 
     def group_name(self):
         return self._group_name
 
     def __str__(self):
         return '<%s "%s">' % (self.__class__.__name__, self._group_name)
 
-    def AddMethod(self, mock_method):
+    def add_method(self, mock_method):
         raise NotImplementedError
 
-    def MethodCalled(self, mock_method):
+    def method_called(self, mock_method):
         raise NotImplementedError
 
-    def IsSatisfied(self):
+    def is_satisfied(self):
         raise NotImplementedError
 
+    AddMethod = add_method
+    MethodCalled = method_called
+    IsSatisfied = is_satisfied
+
 
 class UnorderedGroup(MethodGroup):
     """UnorderedGroup holds a set of method calls that may occur in any order.
 
     This construct is helpful for non-deterministic events, such as iterating
     over the keys of a dict.
     """
@@ -2078,24 +2169,24 @@
     def __str__(self):
         return '%s "%s" pending calls:\n%s' % (
             self.__class__.__name__,
             self._group_name,
             "\n".join(str(method) for method in self._methods),
         )
 
-    def AddMethod(self, mock_method):
+    def add_method(self, mock_method):
         """Add a method to this group.
 
         Args:
           mock_method: A mock method to be added to this group.
         """
 
         self._methods.append(mock_method)
 
-    def MethodCalled(self, mock_method):
+    def method_called(self, mock_method):
         """Remove a method call from the group.
 
         If the method is not in the set, an UnexpectedMethodCallError will be
         raised.
 
         Args:
           mock_method: a mock method that should be equal to a method in the
@@ -2126,19 +2217,23 @@
 
                 return self, method
 
         exception = UnexpectedMethodCallError(mock_method, self)
         self._exception_list.append(exception)
         raise exception
 
-    def IsSatisfied(self):
+    def is_satisfied(self):
         """Return True if there are not any methods in this group."""
 
         return len(self._methods) == 0
 
+    AddMethod = add_method
+    MethodCalled = method_called
+    IsSatisfied = is_satisfied
+
 
 class MultipleTimesGroup(MethodGroup):
     """MultipleTimesGroup holds methods that may be called any number of times.
 
     Note: Each method must be called at least once.
 
     This is helpful, if you don't know or care how many times a method is
@@ -2146,25 +2241,25 @@
     """
 
     def __init__(self, group_name, exception_list):
         super(MultipleTimesGroup, self).__init__(group_name, exception_list)
         self._methods = set()
         self._methods_left = set()
 
-    def AddMethod(self, mock_method):
+    def add_method(self, mock_method):
         """Add a method to this group.
 
         Args:
           mock_method: A mock method to be added to this group.
         """
 
         self._methods.add(mock_method)
         self._methods_left.add(mock_method)
 
-    def MethodCalled(self, mock_method):
+    def method_called(self, mock_method):
         """Remove a method call from the group.
 
         If the method is not in the set, an UnexpectedMethodCallError will be
         raised.
 
         Args:
           mock_method: a mock method that should be equal to a method in the
@@ -2191,18 +2286,22 @@
             next_method = mock_method._PopNextMethod()
             return next_method, None
         else:
             exception = UnexpectedMethodCallError(mock_method, self)
             self._exception_list.append(exception)
             raise exception
 
-    def IsSatisfied(self):
+    def is_satisfied(self):
         """Return True if all methods in this group are called at least once."""
         return len(self._methods_left) == 0
 
+    AddMethod = add_method
+    MethodCalled = method_called
+    IsSatisfied = is_satisfied
+
 
 class MoxMetaTestBase(type):
     """Metaclass to add mox cleanup and verification to every test.
     As the mox unit testing class is being constructed (MoxTestBase or a
     subclass), this metaclass will modify all test functions to call the
     CleanUpMox method of the test class after they finish. This means that
     unstubbing and verifying will happen for every test with no additional
@@ -2221,18 +2320,18 @@
                     try:  # pragma: nocover
                         d[attr_name] = getattr(base, attr_name)
                     except AttributeError:
                         continue
 
         for func_name, func in d.items():
             if func_name.startswith("test") and callable(func):
-                setattr(cls, func_name, MoxMetaTestBase.CleanUpTest(cls, func))
+                setattr(cls, func_name, MoxMetaTestBase.clean_up_test(cls, func))
 
     @staticmethod
-    def CleanUpTest(cls, func):
+    def clean_up_test(cls, func):
         """Adds Mox cleanup code to any MoxTestBase method.
         Always unsets stubs after a test. Will verify all mocks for tests that
         otherwise pass.
         Args:
           cls: MoxTestBase or subclass; the class whose test method we are
             altering.
           func: method; the method of the MoxTestBase test class we wish to
@@ -2262,19 +2361,22 @@
                 mox_obj.VerifyAll()
 
         new_method.__name__ = func.__name__
         new_method.__doc__ = func.__doc__
         new_method.__module__ = func.__module__
         return new_method
 
+    CleanUpTest = clean_up_test
+
 
 _MoxTestBase = MoxMetaTestBase("_MoxTestBase", (unittest.TestCase,), {})
 
 
 class MoxTestBase(_MoxTestBase):
+    # class MoxTestBase(unittest.TestCase, metaclass=MoxMetaTestBase):
     """Convenience test class to make stubbing easier.
     Sets up a "mox" attribute which is an instance of Mox (any mox tests will
     want this), and a "stubs" attribute that is an instance of
     StubOutForTesting (needed at times). Also automatically unsets any stubs
     and verifies that all mock methods have been called at the end of each
     test, eliminating boilerplate code.
     """
```

### Comparing `pymox-1.0.1/mox/stubout.py` & `pymox-1.0.2/mox/stubout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python2.4
+#!/usr/bin/env python
 #
 # Copyright 2008 Google Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -18,33 +18,33 @@
 
 
 class StubOutForTesting:
     """Sample Usage:
     You want os.path.exists() to always return true during testing.
 
     stubs = StubOutForTesting()
-    stubs.Set(os.path, 'exists', lambda x: 1)
+    stubs.set(os.path, 'exists', lambda x: 1)
       ...
-    stubs.UnsetAll()
+    stubs.unset_all()
 
-    The above changes os.path.exists into a lambda that returns 1.  Once
-    the ... part of the code finishes, the UnsetAll() looks up the old value
+    The above changes os.path.exists into a lambda that returns 1. Once
+    the ... part of the code finishes, the unset_all() looks up the old value
     of os.path.exists and restores it.
 
     """
 
     def __init__(self):
         self.cache = []
         self.stubs = []
 
     def __del__(self):
-        self.SmartUnsetAll()
-        self.UnsetAll()
+        self.smart_unset_all()
+        self.unset_all()
 
-    def SmartSet(self, obj, attr_name, new_attr):
+    def smart_set(self, obj, attr_name, new_attr):
         """Replace obj.attr_name with new_attr. This method is smart and works
          at the module, class, and instance level while preserving proper
          inheritance. It will not stub out C types however unless that has
          been explicitly allowed by the type.
 
          This method supports the case where attr_name is a staticmethod or a
          classmethod of obj.
@@ -56,17 +56,15 @@
         - The stubbing is using the builtin getattr and setattr. So, the
           __get__ and __set__ will be called when stubbing (TODO: A better
           idea would probably be to manipulate obj.__dict__ instead of
           getattr() and setattr()).
 
          Raises AttributeError if the attribute cannot be found.
         """
-        if inspect.ismodule(obj) or (
-            not inspect.isclass(obj) and attr_name in obj.__dict__
-        ):
+        if inspect.ismodule(obj) or (not inspect.isclass(obj) and attr_name in obj.__dict__):
             orig_obj = obj
             orig_attr = getattr(obj, attr_name)
 
         else:
             if not inspect.isclass(obj):
                 mro = list(inspect.getmro(obj.__class__))
             else:
@@ -91,28 +89,28 @@
         old_attribute = obj.__dict__.get(attr_name)
         if old_attribute is not None and isinstance(old_attribute, staticmethod):
             orig_attr = staticmethod(orig_attr)
 
         self.stubs.append((orig_obj, attr_name, orig_attr))
         setattr(orig_obj, attr_name, new_attr)
 
-    def SmartUnsetAll(self):
+    def smart_unset_all(self):
         """Reverses all the SmartSet() calls, restoring things to their
         original definition.  Its okay to call SmartUnsetAll() repeatedly, as
         later calls have no effect if no SmartSet() calls have been made.
 
         """
         self.stubs.reverse()
 
         for args in self.stubs:
             setattr(*args)
 
         self.stubs = []
 
-    def Set(self, parent, child_name, new_child):
+    def set(self, parent, child_name, new_child):
         """Replace child_name's old definition with new_child, in the context
         of the given parent.  The parent could be a module when the child is a
         function at module scope.  Or the parent could be a class when a class'
         method is being replaced.  The named child is set to new_child, while
         the prior definition is saved away for later, when UnsetAll() is
         called.
 
@@ -127,21 +125,29 @@
                 old_child = staticmethod(old_child)
             elif isinstance(old_attribute, classmethod):
                 old_child = classmethod(old_child.__func__)
 
         self.cache.append((parent, old_child, child_name))
         setattr(parent, child_name, new_child)
 
-    def UnsetAll(self):
+    def unset_all(self):
         """Reverses all the Set() calls, restoring things to their original
         definition.  Its okay to call UnsetAll() repeatedly, as later calls
         have no effect if no Set() calls have been made.
 
         """
         # Undo calls to Set() in reverse order, in case Set() was called on the
         # same arguments repeatedly (want the original call to be last one
         # undone)
         self.cache.reverse()
 
         for parent, old_child, child_name in self.cache:
             setattr(parent, child_name, old_child)
         self.cache = []
+
+    SmartSet = smart_set
+    SmartUnsetAll = smart_unset_all
+    Set = set
+    UnsetAll = unset_all
+
+
+stubout = StubOutForTesting()
```

### Comparing `pymox-1.0.1/pyproject.toml` & `pymox-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "pymox"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "pymox"
 description = "Mock object framework"
 packages = [{include = "mox"}]
-version = "1.0.1"
+version = "1.0.2"
 authors = ["Ivan Neto <ivan.cr.neto@gmail.com>"]
 license = "Apache License, Version 2.0"
 homepage = "http://pymox.rtfd.io"
 repository = "https://github.com/ivancrneto/pymox"
 classifiers = [
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
```

