# Comparing `tmp/tft-artemis-0.0.8.tar.gz` & `tmp/tft-artemis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tft-artemis-0.0.8.tar", last modified: Wed Dec  2 08:42:49 2020, max compression
+gzip compressed data, was "tft-artemis-0.0.9.tar", last modified: Sat Dec 19 14:26:21 2020, max compression
```

## Comparing `tft-artemis-0.0.8.tar` & `tft-artemis-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1526 2020-12-02 08:39:23.865957 tft-artemis-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    31780 2020-11-27 15:20:25.929350 tft-artemis-0.0.8/src/tft/artemis/__init__.py
--rw-r--r--   0        0        0    24971 2020-11-30 14:56:12.134440 tft-artemis-0.0.8/src/tft/artemis/api/__init__.py
--rw-r--r--   0        0        0     4176 2020-11-10 11:09:12.956542 tft-artemis-0.0.8/src/tft/artemis/api/errors.py
--rw-r--r--   0        0        0     1110 2020-09-14 12:13:33.901249 tft-artemis-0.0.8/src/tft/artemis/api/handlers.py
--rw-r--r--   0        0        0    10050 2020-11-27 13:55:47.686626 tft-artemis-0.0.8/src/tft/artemis/api/middleware.py
--rw-r--r--   0        0        0       58 2020-09-14 12:13:33.901249 tft-artemis-0.0.8/src/tft/artemis/api/settings.py
--rw-r--r--   0        0        0     3407 2020-09-14 12:13:33.901249 tft-artemis-0.0.8/src/tft/artemis/api/validators.py.bak
--rw-r--r--   0        0        0    23846 2020-11-30 12:22:09.005631 tft-artemis-0.0.8/src/tft/artemis/db.py
--rw-r--r--   0        0        0     5554 2020-11-03 08:30:00.378721 tft-artemis-0.0.8/src/tft/artemis/dispatcher.py
--rw-r--r--   0        0        0    26093 2020-12-01 14:41:40.682670 tft-artemis-0.0.8/src/tft/artemis/drivers/__init__.py
--rw-r--r--   0        0        0    21185 2020-11-27 13:55:47.690626 tft-artemis-0.0.8/src/tft/artemis/drivers/aws.py
--rw-r--r--   0        0        0    13693 2020-11-27 13:55:47.690626 tft-artemis-0.0.8/src/tft/artemis/drivers/azure.py
--rw-r--r--   0        0        0    14899 2020-11-27 13:55:47.691626 tft-artemis-0.0.8/src/tft/artemis/drivers/beaker.py
--rw-r--r--   0        0        0    23310 2020-11-27 13:55:47.692626 tft-artemis-0.0.8/src/tft/artemis/drivers/openstack.py
--rw-r--r--   0        0        0     1208 2020-11-11 15:09:02.000300 tft-artemis-0.0.8/src/tft/artemis/environment.py
--rw-r--r--   0        0        0     2463 2020-11-27 15:20:25.929350 tft-artemis-0.0.8/src/tft/artemis/guest.py
--rw-r--r--   0        0        0    13909 2020-11-11 15:09:02.001300 tft-artemis-0.0.8/src/tft/artemis/metrics.py
--rw-r--r--   0        0        0     5308 2020-12-01 14:41:40.682670 tft-artemis-0.0.8/src/tft/artemis/middleware.py
--rw-r--r--   0        0        0        0 2020-09-14 12:13:33.905249 tft-artemis-0.0.8/src/tft/artemis/py.typed
--rw-r--r--   0        0        0     2430 2020-09-14 12:13:33.906249 tft-artemis-0.0.8/src/tft/artemis/script.py
--rw-r--r--   0        0        0      279 2020-11-27 13:55:47.693626 tft-artemis-0.0.8/src/tft/artemis/snapshot.py
--rw-r--r--   0        0        0    78699 2020-12-01 14:41:40.683670 tft-artemis-0.0.8/src/tft/artemis/tasks.py
--rw-r--r--   0        0        0      379 2020-09-14 12:13:33.908249 tft-artemis-0.0.8/src/tft/artemis/vault.py
--rw-r--r--   0        0        0     1745 2020-12-02 08:42:50.760111 tft-artemis-0.0.8/setup.py
--rw-r--r--   0        0        0     1242 2020-12-02 08:42:50.760423 tft-artemis-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1754 2020-12-19 14:23:00.336519 tft-artemis-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    32922 2020-12-17 14:55:25.767658 tft-artemis-0.0.9/src/tft/artemis/__init__.py
+-rw-r--r--   0        0        0    24857 2020-12-17 14:55:25.769658 tft-artemis-0.0.9/src/tft/artemis/api/__init__.py
+-rw-r--r--   0        0        0     4176 2020-11-10 11:09:12.956542 tft-artemis-0.0.9/src/tft/artemis/api/errors.py
+-rw-r--r--   0        0        0     1110 2020-09-14 12:13:33.901249 tft-artemis-0.0.9/src/tft/artemis/api/handlers.py
+-rw-r--r--   0        0        0    10050 2020-11-27 13:55:47.686626 tft-artemis-0.0.9/src/tft/artemis/api/middleware.py
+-rw-r--r--   0        0        0       58 2020-09-14 12:13:33.901249 tft-artemis-0.0.9/src/tft/artemis/api/settings.py
+-rw-r--r--   0        0        0     3407 2020-09-14 12:13:33.901249 tft-artemis-0.0.9/src/tft/artemis/api/validators.py.bak
+-rw-r--r--   0        0        0    23846 2020-12-15 18:39:07.872543 tft-artemis-0.0.9/src/tft/artemis/db.py
+-rw-r--r--   0        0        0     5554 2020-11-03 08:30:00.378721 tft-artemis-0.0.9/src/tft/artemis/dispatcher.py
+-rw-r--r--   0        0        0    26302 2020-12-08 09:31:08.234269 tft-artemis-0.0.9/src/tft/artemis/drivers/__init__.py
+-rw-r--r--   0        0        0    21143 2020-12-17 14:55:25.770658 tft-artemis-0.0.9/src/tft/artemis/drivers/aws.py
+-rw-r--r--   0        0        0    14345 2020-12-17 14:55:25.771658 tft-artemis-0.0.9/src/tft/artemis/drivers/azure.py
+-rw-r--r--   0        0        0    15051 2020-12-17 14:55:25.772658 tft-artemis-0.0.9/src/tft/artemis/drivers/beaker.py
+-rw-r--r--   0        0        0    24158 2020-12-17 14:55:25.774658 tft-artemis-0.0.9/src/tft/artemis/drivers/openstack.py
+-rw-r--r--   0        0        0     1208 2020-12-14 21:14:47.941145 tft-artemis-0.0.9/src/tft/artemis/environment.py
+-rw-r--r--   0        0        0     2164 2020-12-17 14:55:25.774658 tft-artemis-0.0.9/src/tft/artemis/guest.py
+-rw-r--r--   0        0        0    13909 2020-11-11 15:09:02.001300 tft-artemis-0.0.9/src/tft/artemis/metrics.py
+-rw-r--r--   0        0        0     6619 2020-12-17 14:55:25.774658 tft-artemis-0.0.9/src/tft/artemis/middleware.py
+-rw-r--r--   0        0        0        0 2020-09-14 12:13:33.905249 tft-artemis-0.0.9/src/tft/artemis/py.typed
+-rw-r--r--   0        0        0     2430 2020-09-14 12:13:33.906249 tft-artemis-0.0.9/src/tft/artemis/script.py
+-rw-r--r--   0        0        0    79486 2020-12-18 11:13:00.715035 tft-artemis-0.0.9/src/tft/artemis/tasks.py
+-rw-r--r--   0        0        0      884 2020-12-17 14:55:25.778658 tft-artemis-0.0.9/src/tft/artemis/vault.py
+-rw-r--r--   0        0        0     1745 2020-12-19 14:26:22.037797 tft-artemis-0.0.9/setup.py
+-rw-r--r--   0        0        0     1242 2020-12-19 14:26:22.038220 tft-artemis-0.0.9/PKG-INFO
```

### Comparing `tft-artemis-0.0.8/pyproject.toml` & `tft-artemis-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tft-artemis"
-version = "0.0.8"
+version = "0.0.9"
 description = "Artemis is a machine provisioning service. Its goal is to provision a machine - using a set of preconfigured providers as backends - which would satisfy the given hardware and software requirements."
 authors = [
   "Milos Prchlik <mprchlik@redhat.com>",
   "Anna Khaitovich <akhaitov@redhat.com>",
   "Evgeny Fedin <efedin@redhat.com>",
   "Miroslav Vadkerti <mvadkert@redhat.com>",
   "Ondrej Ptak <optak@redhat.com>",
@@ -30,25 +30,33 @@
 python-openstackclient = "^5.0.0"
 sqlalchemy = "^1.3.12"
 stackprinter = "^0.2.4"
 typing-extensions = "^3.7.4"
 periodiq = "^0.12.1"
 
 [tool.poetry.dev-dependencies]
+# Install `toml` extra to allow parsing pyproject.toml - no need for special config file for coverage.
+coverage = { version = "*", extras = ["toml"] }
 flake8 = "*"
 pytest = "*"
 mypy = "0.720"
 mypy-extensions = "0.4.1"
 pre-commit = "^2.7.1"
 pytest-flake8 = "*"
 pytest-mock = "*"
 sqlalchemy-stubs = "*"
+sqlalchemy-utils = "*"
 
 [tool.poetry.scripts]
 artemis-api-server = "tft.artemis.api:main"
 artemis-dispatcher = "tft.artemis.dispatcher:main"
 artemis-init-sqlite-schema = "tft.artemis.db:init_sqlite"
 artemis-init-postgres-schema = "tft.artemis.db:init_postgres"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
+
+[tool.coverage.run]
+source = [
+  "src/tft/artemis"
+]
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/__init__.py` & `tft-artemis-0.0.9/src/tft/artemis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,14 +553,33 @@
 
     def to_repr(self) -> List[str]:
         return [
             'has-db=yes'
         ]
 
 
+class KnobSourceActual(KnobSource[T]):
+    """
+    Use value as-is.
+    """
+
+    def __init__(self, knob: 'Knob[T]', value: T) -> None:
+        super(KnobSourceActual, self).__init__(knob)
+
+        self.value = value
+
+    def get_value(self, *args: Any) -> Result[Optional[T], Failure]:
+        return Ok(self.value)
+
+    def to_repr(self) -> List[str]:
+        return [
+            'actual="{}"'.format(self.value)
+        ]
+
+
 class KnobError(ValueError):
     def __init__(self, knob: 'Knob[T]', message: str, failure: Optional[Failure] = None) -> None:
         super(KnobError, self).__init__('Badly configured knob: {}'.format(message))
 
         self.knobname = knob.knobname
         self.failure = failure
 
@@ -577,14 +596,15 @@
     Some of the knobs are not backed by a database, especially knobs needed by code establishing the database
     connections.
 
     The resolution order in which possible sources are checked when knob value is needed:
 
     1. the database, if the knob declaration specifies the database may be used.
     2. the environment variable.
+    3. the given "actual" value, prossibly originating from a config file.
     3. the default value.
 
     A typical knob may look like this:
 
     .. code-block:: python3
 
        # As a two-state knob, `bool` is the best choice here.
@@ -596,14 +616,20 @@
            has_db=False,
 
            # This knob gets its value from the following environment variable. It is necessary to provide
            # a callback that casts the raw string value to the proper type.
            envvar='ARTEMIS_LOG_JSON',
            envvar_cast=gluetool.utils.normalize_bool_option,
 
+           # This knob gets its value when created. Note that this is *very* similar to the default value,
+           # but the default value should stand out as the default, while this parameter represents e.g.
+           # value read from a configuration file, and as such may be left unspecified - then the default
+           # would be used.
+           actual=a_yaml_config_file['logging']['json'],
+
            # The default value - note that it is properly typed.
            default=True
        )
 
     The knob can be used in a following way:
 
     .. code-block:: python3
@@ -622,60 +648,65 @@
        >>>
 
     :param knobname: name of the knob. It is used for presentation and as a key when the database is involved.
     :param has_db: if set, the value may also be stored in the database.
     :param envvar: if set, it is the name of the environment variable providing the value.
     :param envvar_cast: a callback used to cast the raw environment variable content to the correct type.
         Required when ``envvar`` is set.
+    :param actual: if set, it is the currently known value, e.g. provided by a config file.
     :param default: if set, it is used as a default value.
     """
 
     def __init__(
         self,
         knobname: str,
         has_db: bool = True,
         envvar: Optional[str] = None,
         envvar_cast: Optional[Callable[[str], T]] = None,
+        actual: Optional[T] = None,
         default: Optional[T] = None,
     ) -> None:
         self.knobname = knobname
         self._sources: List[KnobSource[T]] = []
 
         if has_db:
             self._sources.append(KnobSourceDB(self))
 
         if envvar is not None:
             if not envvar_cast:
                 raise Exception('Knob {} defined with envvar but no envvar_cast'.format(knobname))
 
             self._sources.append(KnobSourceEnv(self, envvar, envvar_cast))
 
+        if actual is not None:
+            self._sources.append(KnobSourceActual(self, actual))
+
         if default is not None:
             self._sources.append(KnobSourceDefault(self, default))
 
         if not self._sources:
             raise KnobError(
                 self,
-                'no source specified - no DB, envvar nor default value.'
+                'no source specified - no DB, envvar, actual nor default value.'
             )
 
         # If the knob isn't backed by a database, it should be possible to deduce its value *now*,
-        # as it depends on envvar or the default value. For such knobs, we provide a shortcut,
+        # as it depends on envvar, actual or default value. For such knobs, we provide a shortcut,
         # easy-to-use `value` attribute - no `Result`, no `unwrap()` - given the possible sources,
         # it should never fail to get a value from such sources.
         if not has_db:
             value, failure = self._get_value()
 
             # If we fail to get value from envvar/default sources, then something is wrong. Maybe there's
             # just the envvar source, no default one, and environment variable is not set? In any case,
             # this sounds like a serious bug.
             if value is None:
                 raise KnobError(
                     self,
-                    'no DB, yet other sources do not provide value! To fix, add an envvar source, or a default value.',
+                    'no DB, yet other sources do not provide value! To fix, add an envvar, actual or default value.',
                     failure=failure
                 )
 
             self.value = value
 
     def __repr__(self) -> str:
         return '<Knob: {}: {}>'.format(
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/api/__init__.py` & `tft-artemis-0.0.9/src/tft/artemis/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -322,22 +322,19 @@
 
 class GuestRequestManager:
     def __init__(self, db: artemis_db.DB) -> None:
         self.db = db
 
     def get_guest_requests(self) -> List[GuestResponse]:
         with self.db.get_session() as session:
-            guests = session.query(artemis_db.GuestRequest).all()
-
-            responses = [
-                GuestResponse.from_db(guest) for guest in guests
+            return [
+                GuestResponse.from_db(guest)
+                for guest in artemis_db.Query.from_session(session, artemis_db.GuestRequest).all()
             ]
 
-        return responses
-
     def create(self, guest_request: GuestRequest, ownername: str) -> GuestResponse:
         guestname = str(uuid.uuid4())
 
         with self.db.get_session() as session:
             session.add(
                 artemis_db.GuestRequest(
                     guestname=guestname,
@@ -374,27 +371,23 @@
                     'user_data': guest_request.user_data
                 }
             )
 
         return gr
 
     def get_by_guestname(self, guestname: str) -> Optional[GuestResponse]:
-        try:
-            with self.db.get_session() as session:
-                guest = session \
-                        .query(artemis_db.GuestRequest) \
-                        .filter(artemis_db.GuestRequest.guestname == guestname) \
-                        .one()
-
-                response = GuestResponse.from_db(guest)
+        with self.db.get_session() as session:
+            guest_request_record = artemis_db.Query.from_session(session, artemis_db.GuestRequest) \
+                .filter(artemis_db.GuestRequest.guestname == guestname) \
+                .one_or_none()
 
-        except sqlalchemy.orm.exc.NoResultFound:
-            return None
+            if guest_request_record is None:
+                return None
 
-        return response
+            return GuestResponse.from_db(guest_request_record)
 
     def delete_by_guestname(self, guestname: str, request: Request) -> None:
         with self.db.get_session() as session:
             query = sqlalchemy \
                     .update(artemis_db.GuestRequest.__table__) \
                     .where(artemis_db.GuestRequest.guestname == guestname) \
                     .values(state=GuestState.CONDEMNED.value)
@@ -491,28 +484,24 @@
 
 
 class SnapshotRequestManager:
     def __init__(self, db: artemis_db.DB) -> None:
         self.db = db
 
     def get_snapshot(self, guestname: str, snapshotname: str) -> Optional[SnapshotResponse]:
-        try:
-            with self.db.get_session() as session:
-                snapshot = session \
-                           .query(artemis_db.SnapshotRequest.__table__) \
-                           .filter(artemis_db.SnapshotRequest.snapshotname == snapshotname) \
-                           .filter(artemis_db.SnapshotRequest.guestname == guestname) \
-                           .one()
-
-                response = SnapshotResponse.from_db(snapshot)
+        with self.db.get_session() as session:
+            snapshot_request_record = artemis_db.Query.from_session(session, artemis_db.SnapshotRequest) \
+                .filter(artemis_db.SnapshotRequest.snapshotname == snapshotname) \
+                .filter(artemis_db.SnapshotRequest.guestname == guestname) \
+                .one_or_none()
 
-        except sqlalchemy.orm.exc.NoResultFound:
-            return None
+            if snapshot_request_record is None:
+                return None
 
-        return response
+            return SnapshotResponse.from_db(snapshot_request_record)
 
     def create_snapshot(self, guestname: str, snapshot_request: SnapshotRequest) -> SnapshotResponse:
         snapshotname = str(uuid.uuid4())
 
         with self.db.get_session() as session:
             session.add(
                 artemis_db.SnapshotRequest(
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/api/errors.py` & `tft-artemis-0.0.9/src/tft/artemis/api/errors.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/api/handlers.py` & `tft-artemis-0.0.9/src/tft/artemis/api/handlers.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/api/middleware.py` & `tft-artemis-0.0.9/src/tft/artemis/api/middleware.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/api/validators.py.bak` & `tft-artemis-0.0.9/src/tft/artemis/api/validators.py.bak`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/db.py` & `tft-artemis-0.0.9/src/tft/artemis/db.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/dispatcher.py` & `tft-artemis-0.0.9/src/tft/artemis/dispatcher.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/drivers/__init__.py` & `tft-artemis-0.0.9/src/tft/artemis/drivers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,19 @@
     def can_acquire(
         self,
         environment: Environment
     ) -> Result[bool, Failure]:
         """
         Find our whether this driver can provision a guest that would satisfy
         the given environment.
+
+        :param Environment environment: environment to check
+        :rtype: result.Result[bool, Failure]
+        :returns: :py:class:`result.result` with either `bool`
+            or specification of error.
         """
 
         raise NotImplementedError()
 
     def acquire_guest(
         self,
         logger: gluetool.log.ContextAdapter,
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/drivers/aws.py` & `tft-artemis-0.0.9/src/tft/artemis/drivers/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,29 +141,37 @@
 
         return Ok(None)
 
     def can_acquire(self, environment: Environment) -> Result[bool, Failure]:
         if environment.arch != 'x86_64':
             return Ok(False)
 
+        r_image = self._env_to_image(self.logger, environment)
+        if r_image.is_error:
+            return Error(r_image.value)
+
+        r_type = self._env_to_instance_type(environment)
+        if r_type.is_error:
+            return Error(r_type.value)
+
         return Ok(True)
 
     def _env_to_instance_type(self, environment: Environment) -> Result[Any, Failure]:
         # TODO: in the future we will here translate the environment into an instance type
         return Ok(self.pool_config['default-instance-type'])
 
     def _env_to_image(
         self,
         logger: gluetool.log.ContextAdapter,
         environment: Environment
     ) -> Result[Any, Failure]:
         r_engine = hook_engine('AWS_ENVIRONMENT_TO_IMAGE')
 
         if r_engine.is_error:
-            raise Exception('Failed to load AWS_ENVIRONMENT_TO_IMAGE hook: {}'.format(r_engine.unwrap_error().message))
+            return Error(r_engine.unwrap_error())
 
         engine = r_engine.unwrap()
 
         r_image = engine.run_hook(
             'AWS_ENVIRONMENT_TO_IMAGE',
             logger=logger,
             pool=self,
@@ -529,21 +537,15 @@
         r_instance_type = self._env_to_instance_type(environment)
         if r_instance_type.is_error:
             return r_instance_type
 
         instance_type = r_instance_type.unwrap()
 
         # find out image from enviroment
-        try:
-            r_image = self._env_to_image(logger, environment)
-        except Exception as exc:
-            error_msg = str(exc)
-            if 'Failed to load AWS_ENVIRONMENT_TO_IMAGE hook' in error_msg:
-                return Error(Failure(error_msg))
-            raise exc
+        r_image = self._env_to_image(logger, environment)
 
         if r_image.is_error:
             return r_image
 
         image = r_image.unwrap()
 
         # request a spot instance and wait for it's full fillment
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/drivers/azure.py` & `tft-artemis-0.0.9/src/tft/artemis/drivers/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,21 +108,34 @@
         output = r_output.unwrap()
 
         if not output:
             return Error(Failure('Server show commmand output is empty'))
 
         status = output['provisioningState'].lower()
 
-        logger.info('instance status is {}'.format(status))
+        logger.info('current instance status {}:{}'.format(
+            AzurePoolData.unserialize(guest_request).instance_id,
+            status
+        ))
 
         if status == 'failed':
-            self.release_guest(logger, guest_request)
-            logger.warning('Instance ended up in failed state. NOT provisioning a new one')
+            logger.warning('Instance ended up in failed state')
+
+            r_acquire = self._do_acquire_guest(logger, guest_request, environment, master_key)
+
+            if r_acquire.is_ok:
+                logger.info('successfully reprovisioned, releasing the broken instance')
 
-            return self._do_acquire_guest(logger, guest_request, environment, master_key)
+                # We can schedule release only when acquire succeeded. Only successfull acquire
+                # let's us update guest request pool data with new instance ID. If acquire failed,
+                # we keep our broken instance, and enter update guest task later, trying again
+                # to either update or reschedule and drop the failed one.
+                self.release_guest(logger, guest_request)
+
+            return r_acquire
 
         r_ip_address = vm_info_to_ip(output, 'publicIps', r'((?:[0-9]{1,3}\.){3}[0-9]{1,3}).*')
 
         if r_ip_address.is_error:
             return Error(r_ip_address.unwrap_error())
 
         return Ok(ProvisioningProgress(
@@ -367,15 +380,19 @@
             return Error(r_output.unwrap_error())
 
         output = r_output.unwrap()
         if not output['id']:
             return Error(Failure('Instance id not found'))
 
         status = output['powerState'].lower()
-        logger.info('instance status is {}'.format(status))
+
+        logger.info('acquired instance status {}:{}'.format(
+            output['id'],
+            status
+        ))
 
         # There is no chance that the guest will be ready in this step
         return Ok(ProvisioningProgress(
             is_acquired=False,
             pool_data=AzurePoolData(
                 instance_id=output['id'],
                 instance_name=name,
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/drivers/beaker.py` & `tft-artemis-0.0.9/src/tft/artemis/drivers/beaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,19 @@
 
         r_parse_job_status = self._parse_job_status(job_results_xml)
         if r_parse_job_status.is_error and r_parse_job_status.error:
             return Error(r_parse_job_status.error)
 
         job_status = r_parse_job_status.unwrap()
 
+        logger.info('current job status {}:{}'.format(
+            BeakerPoolData.unserialize(guest_request).job_id,
+            job_status
+        ))
+
         if job_status == 'Pass':
             r_parse_guest_address = self._parse_guest_address(job_results_xml)
             if r_parse_guest_address.is_error and r_parse_guest_address.error:
                 return Error(r_parse_guest_address.error)
 
             return Ok(ProvisioningProgress(
                 is_acquired=True,
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/drivers/openstack.py` & `tft-artemis-0.0.9/src/tft/artemis/drivers/openstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,15 @@
         self,
         logger: gluetool.log.ContextAdapter,
         environment: Environment
     ) -> Result[Any, Failure]:
         r_engine = hook_engine('OPENSTACK_ENVIRONMENT_TO_IMAGE')
 
         if r_engine.is_error:
-            raise Exception(
-                'Failed to load OPENSTACK_ENVIRONMENT_TO_IMAGE hook: {}'.format(r_engine.unwrap_error().message)
-            )
+            return Error(r_engine.unwrap_error())
 
         engine = r_engine.unwrap()
 
         r_image = engine.run_hook(
             'OPENSTACK_ENVIRONMENT_TO_IMAGE',
             logger=logger,
             pool=self,
@@ -337,15 +335,18 @@
         output = r_output.unwrap()
         if not output['id']:
             return Error(Failure('Instance id not found'))
         instance_id = output['id']
 
         status = output['status'].lower()
 
-        logger.info('instance status is {}'.format(status))
+        logger.info('acquired instance status {}:{}'.format(
+            instance_id,
+            status
+        ))
 
         # There is no chance that the guest will be ready in this step
         return Ok(ProvisioningProgress(
             is_acquired=False,
             pool_data=OpenStackPoolData(instance_id=instance_id)
         ))
 
@@ -414,14 +415,22 @@
 
         return Ok(True)
 
     def can_acquire(self, environment: Environment) -> Result[bool, Failure]:
         if environment.arch not in self.pool_config['available-arches']:
             return Ok(False)
 
+        r_image = self._env_to_image(self.logger, environment)
+        if r_image.is_error:
+            return Error(r_image.value)
+
+        r_flavor = self._env_to_flavor(environment)
+        if r_flavor.is_error:
+            return Error(r_flavor.value)
+
         return Ok(True)
 
     def create_snapshot(
         self,
         guest_request: GuestRequest,
         snapshot_request: SnapshotRequest
     ) -> Result[ProvisioningProgress, Failure]:
@@ -548,26 +557,38 @@
         output = r_output.unwrap()
 
         if not output:
             return Error(Failure('Server show commmand output is empty'))
 
         status = output['status'].lower()
 
-        logger.info('instance status is {}'.format(status))
+        logger.info('current instance status {}:{}'.format(
+            OpenStackPoolData.unserialize(guest_request).instance_id,
+            status
+        ))
 
         def _reprovision(msg: str) -> Result[ProvisioningProgress, Failure]:
             logger.warning(msg)
 
-            self._dispatch_resource_cleanup(
-                logger,
-                instance_id=OpenStackPoolData.unserialize(guest_request).instance_id,
-                guest_request=guest_request
-            )
+            r_acquire = self._do_acquire_guest(logger, guest_request, environment, master_key)
+
+            if r_acquire.is_ok:
+                logger.info('successfully reprovisioned, releasing the broken instance')
+
+                # We can schedule release only when acquire succeeded. Only successfull acquire
+                # let's us update guest request pool data with new instance ID. If acquire failed,
+                # we keep our broken instance, and enter update guest task later, trying again
+                # to either update or reschedule and drop the failed one.
+                self._dispatch_resource_cleanup(
+                    logger,
+                    instance_id=OpenStackPoolData.unserialize(guest_request).instance_id,
+                    guest_request=guest_request
+                )
 
-            return self._do_acquire_guest(logger, guest_request, environment, master_key)
+            return r_acquire
 
         if status == 'error':
             return _reprovision('Instance ended up in error state. provisioning a new one')
 
         if status == 'build' and 'created' in output:
             try:
                 created_stamp = datetime.strptime(output['created'], '%Y-%m-%dT%H:%M:%SZ')
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/environment.py` & `tft-artemis-0.0.9/src/tft/artemis/environment.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/guest.py` & `tft-artemis-0.0.9/src/tft/artemis/guest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import dataclasses
 import enum
 
 import gluetool.log
 
-from . import db as artemis_db
-
 
 class GuestState(enum.Enum):
     ERROR = 'error'
 
     #: Initial state. Newly created guest requests are set to PENDING and wait for
     #: being picked up be the router.
     PENDING = 'pending'
@@ -54,24 +51,12 @@
 class GuestLogger(gluetool.log.ContextAdapter):
     def __init__(self, logger: gluetool.log.ContextAdapter, guestname: str) -> None:
         super(GuestLogger, self).__init__(logger, {
             'ctx_guest_name': (10, guestname)
         })
 
 
-@dataclasses.dataclass
-class SSHInfo:
-    """
-    SSH-related information used to transport all the relevant information between different subsystems.
-    We want to keep our use of SSH usernames and keys consistent.
-    """
-
-    key: artemis_db.SSHKey
-    port: int = 22
-    username: str = 'root'
-
-    def __repr__(self) -> str:
-        return '<SSHInfo: port={}, username={}, key={}>'.format(
-            self.port,
-            self.username,
-            self.key.keyname if self.key else ''
-        )
+class SnapshotLogger(gluetool.log.ContextAdapter):
+    def __init__(self, logger: gluetool.log.ContextAdapter, snapshotname: str) -> None:
+        super(SnapshotLogger, self).__init__(logger, {
+            'ctx_snapshot_name': (11, snapshotname)
+        })
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/metrics.py` & `tft-artemis-0.0.9/src/tft/artemis/metrics.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/middleware.py` & `tft-artemis-0.0.9/src/tft/artemis/middleware.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 import datetime
+import inspect
 import traceback
 
+import dramatiq.message
 import dramatiq.middleware.retries
 from dramatiq.common import compute_backoff
+import gluetool.log
 
 from .guest import GuestLogger
 
-from typing import cast, Any, Optional
+from typing import Any, Dict, Optional
 
 
 class Retries(dramatiq.middleware.retries.Retries):  # type: ignore  # Class cannot subclass 'Retries
-    def _guestname_from_message(self, message: Any) -> Optional[str]:
-        try:
-            return cast(
-                str,
-                message._message[2][0]
-            )
-
-        except IndexError:
-            return None
+    def _actor_arguments(
+        self,
+        logger: gluetool.log.ContextAdapter,
+        message: dramatiq.message.Message,
+        actor: Any  # it's actually tasks.Actor, but circular import :/
+    ) -> Optional[Dict[str, Any]]:
+        signature = inspect.signature(actor.fn)
+
+        gluetool.log.log_dict(logger.debug, 'raw message data', message._message)
+
+        if len(signature.parameters) != len(message._message[2]):
+            from . import Failure
+
+            Failure(
+                'actor signature parameters does not match message content',
+                signature=[name for name in signature.parameters.keys()],
+                arguments=message._message[2]
+            ).handle(logger)
+
+            return {}
+
+        return {
+            name: message._message[2][index]
+            for index, name in enumerate(signature.parameters.keys())
+        }
 
     def after_process_message(
         self,
         broker: Any,
-        message: Any,
+        message: dramatiq.message.Message,
         *,
         result: Optional[Any] = None,
         exception: Optional[Any] = None
     ) -> None:
         if exception is None:
             return
 
@@ -36,34 +55,29 @@
         logger = get_logger()
 
         actor = broker.get_actor(message.actor_name)
         retries = message.options.setdefault("retries", 0)
         max_retries = message.options.get("max_retries") or actor.options.get("max_retries", self.max_retries)
         retry_when = actor.options.get("retry_when", self.retry_when)
 
-        guestname = self._guestname_from_message(message)
+        actor_arguments = self._actor_arguments(logger, message, actor)
+
+        guestname = actor_arguments['guestname'] if actor_arguments and 'guestname' in actor_arguments else None
 
         if guestname:
             logger = GuestLogger(logger, guestname)
 
         logger.info(
             'retries: message={} actor={} attempts={} max_retries={}'.format(
                 message.message_id, message.actor_name, retries, max_retries
             )
         )
 
         if retry_when is not None and not retry_when(retries, exception) or \
            retry_when is None and max_retries is not None and retries >= max_retries:
-
-            # We are not interested in special handling of messages that don't relate to guests.
-            if not guestname:
-                logger.warning('retries: retries exceeded for message {}.'.format(message.message_id))
-                message.fail()
-                return
-
             # Handle the provisioning "tail": when we run out of retries on a task that works on
             # provisioning, and we need to release anything we already acquired, and start again.
             #
             # By this point, most likely, the provisioning is probably stuck with a broken pool,
             # or we already have a guest and we can't reach it, or something like that. Something
             # happened after routing and before successfully reaching READY state. We need to
             # release all the resources we have, to avoid leaks, and fall back to routing.
@@ -77,39 +91,57 @@
             # fail to schedule the routing task, we probably won't get away with a different actor.
             #
             # As of now, if we want to keep any chance of falling back to routing, rescheduling the
             # message seems to be the only way. It's quite likely it will fail again, giving us another
             # chance for release & revert. Note that this applies to situations where "release & revert"
             # attempt fails, i.e. DB or broker issues, most likely.
 
-            from .tasks import TaskLogger, handle_provisioning_chain_tail
+            from .tasks import TaskLogger, is_provisioning_tail_task, handle_provisioning_chain_tail
 
-            tail_logger = TaskLogger(logger, 'provisioning-tail')
+            if is_provisioning_tail_task(actor):
+                tail_logger = TaskLogger(logger, 'provisioning-tail')
 
-            db = get_db(tail_logger)
+                if not guestname:
+                    from . import Failure
 
-            with db.get_session() as session:
-                if handle_provisioning_chain_tail(
-                    tail_logger,
-                    db,
-                    session,
-                    guestname,
-                    actor
-                ):
-                    tail_logger.info('successfuly handled the provisioning tail')
+                    Failure(
+                        'cannot handle provisioning tail with undefined guestname',
+                    ).handle(tail_logger)
+
+                    message.fail()
                     return
 
-            tail_logger.error('failed to handle the provisioning tail')
+                db = get_db(tail_logger)
 
-            # This would cause the message to be dropped, effectively halting any work towards provisioning
-            # of the guest.
-            #
-            # In the spirit of "let's try again...", falling through to rescheduling the original task.
-            #
-            # message.fail()
+                with db.get_session() as session:
+                    if handle_provisioning_chain_tail(
+                        tail_logger,
+                        db,
+                        session,
+                        guestname,
+                        actor
+                    ):
+                        tail_logger.info('successfuly handled the provisioning tail')
+                        return
+
+                tail_logger.error('failed to handle the provisioning tail')
+
+                # This would cause the message to be dropped, effectively halting any work towards provisioning
+                # of the guest.
+                #
+                # In the spirit of "let's try again...", falling through to rescheduling the original task.
+                #
+                # message.fail()
+
+            else:
+                # Kill messages for tasks we don't handle in any better way. After all, they did run out of retires.
+                logger.warning('retries: retries exceeded for message {}.'.format(message.message_id))
+                message.fail()
+
+                return
 
         message.options["retries"] += 1
         message.options["traceback"] = traceback.format_exc(limit=30)
         min_backoff = message.options.get("min_backoff") or actor.options.get("min_backoff", self.min_backoff)
         max_backoff = message.options.get("max_backoff") or actor.options.get("max_backoff", self.max_backoff)
         max_backoff = min(max_backoff, dramatiq.middleware.retries.DEFAULT_MAX_BACKOFF)
         _, backoff = compute_backoff(retries, factor=min_backoff, max_backoff=max_backoff)
```

### Comparing `tft-artemis-0.0.8/src/tft/artemis/script.py` & `tft-artemis-0.0.9/src/tft/artemis/script.py`

 * *Files identical despite different names*

### Comparing `tft-artemis-0.0.8/src/tft/artemis/tasks.py` & `tft-artemis-0.0.9/src/tft/artemis/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 
 from . import Failure, Knob, get_db, get_logger, get_broker, safe_call, safe_db_change, log_guest_event, \
     log_error_guest_event
 from . import metrics
 from .db import DB, GuestEvent, GuestRequest, Pool, SnapshotRequest, SSHKey, Query
 from .drivers import PoolDriver, PoolLogger, PoolData
 from .environment import Environment
-from .guest import GuestLogger, GuestState
+from .guest import GuestLogger, GuestState, SnapshotLogger
 from .script import hook_engine
-from .snapshot import SnapshotLogger
 
 from .drivers import aws as aws_driver
 from .drivers import beaker as beaker_driver
 from .drivers import openstack as openstack_driver
 from .drivers import azure as azure_driver
 
-from typing import cast, Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from typing_extensions import Protocol
 
 
 # There is a very basic thing we must be aware of: a task - the Python function below - can run multiple times,
 # sequentialy or in parallel. It's like multithreading application above a database, without any locks available.
 # Tasks must be aware of this and carefully plan their workflow, to employ database queries to help with the
 # synchronization, and tasks must be always ready to rollback their changes as much as possible.
@@ -80,16 +79,16 @@
 # TODO:
 # - support queue name when sending messages - we want our tasks to use different queues.
 # - allow retries modification and tweaking
 # - "lazy actor" wrapper to avoid the necessity of initializing dramatiq at the import time
 
 
 # Initialize our top-level objects, database and logger, shared by all threads and in *this* worker.
-root_logger = get_logger()
-db = get_db(root_logger)
+_ROOT_LOGGER = get_logger()
+_ROOT_DB = get_db(_ROOT_LOGGER)
 
 # Initialize the broker instance - this call takes core of correct connection between broker and queue manager.
 BROKER = get_broker()
 
 
 KNOB_ACTOR_DEFAULT_RETRIES_COUNT: Knob[int] = Knob(
     'actor.default-retries-count',
@@ -136,23 +135,32 @@
 #
 # Note: we could use object() to create this value, but using custom class let's use limit allowed types returned
 # by doer.
 class _RescheduleType:
     pass
 
 
+# A class of unique "failed but ignore" doer return value
+class _IgnoreType:
+    pass
+
+
 # Unique object representing "reschedule task" return value of doer.
 Reschedule = _RescheduleType()
 
+# Unique object representing "failed but ignore" return value of doer.
+Ignore = _IgnoreType()
+
 # Doer return value type.
-DoerReturnType = Result[Union[None, _RescheduleType], Failure]
+DoerReturnType = Result[Union[None, _RescheduleType, _IgnoreType], Failure]
 
 # Helpers for constructing return values.
 SUCCESS: DoerReturnType = Ok(None)
 RESCHEDULE: DoerReturnType = Ok(Reschedule)
+IGNORE: DoerReturnType = Ok(Ignore)
 
 
 def FAIL(result: Result[Any, Failure]) -> DoerReturnType:
     return Error(result.unwrap_error())
 
 
 # Task doer type.
@@ -278,15 +286,18 @@
                 logger,
                 session,
                 guestname,
                 label,
                 failure
             )
 
-        return Error(failure)
+        if failure.recoverable is True:
+            return Error(failure)
+
+        return IGNORE
 
     return handle_success, handle_failure, spice_details
 
 
 def actor_control_value(actor_name: str, var_name: str, default: Any) -> Any:
     var_value = os.getenv(
         'ARTEMIS_ACTOR_{}_{}'.format(actor_name.upper(), var_name),
@@ -414,27 +425,30 @@
 
     doer_args = doer_args or tuple()
     doer_kwargs = doer_kwargs or dict()
 
     doer_result: DoerReturnType = Error(Failure('undefined doer result'))
 
     try:
-        with db.get_session() as session:
-            doer_result = run_doer(logger, db, session, cancel, doer, *doer_args, **doer_kwargs)
+        with _ROOT_DB.get_session() as session:
+            doer_result = run_doer(logger, _ROOT_DB, session, cancel, doer, *doer_args, **doer_kwargs)
 
     except Exception as exc:
         stackprinter.show_current_exception()
         failure = Failure.from_exc('unhandled doer exception', exc)
         failure.handle(logger)
 
         doer_result = Error(failure)
 
     if doer_result.is_ok:
         result = doer_result.unwrap()
 
+        if result is Ignore:
+            logger.warning('message processing encountered error and requests waiver')
+
         logger.finished()
 
         if result is Reschedule:
             raise Exception('message processing requested reschedule')
 
         return
 
@@ -512,85 +526,73 @@
 
 
 def _get_guest_request(
     logger: gluetool.log.ContextAdapter,
     session: sqlalchemy.orm.session.Session,
     guestname: str
 ) -> Result[Optional[GuestRequest], Failure]:
-    query_proxy = Query.from_session(session, GuestRequest) \
-        .filter(GuestRequest.guestname == guestname)
-
-    r_query = cast(
-        Result[GuestRequest, Failure],
-        safe_call(query_proxy.one)
-    )
-
-    if r_query.is_ok:
-        return Ok(r_query.unwrap())
-
-    failure = r_query.unwrap_error()
-
-    if isinstance(failure.exception, sqlalchemy.orm.exc.NoResultFound):
-        return Ok(None)
+    try:
+        return Ok(
+            Query.from_session(session, GuestRequest)
+            .filter(GuestRequest.guestname == guestname)
+            .one_or_none()
+        )
 
-    return Error(failure)
+    except Exception as exc:
+        return Error(Failure.from_exc(
+            'failed to fetch guest request',
+            exc,
+            guestname=guestname
+        ))
 
 
-def _get_guest_by_state(
+def _get_guest_request_by_state(
     logger: gluetool.log.ContextAdapter,
     session: sqlalchemy.orm.session.Session,
     guestname: str,
     state: GuestState
 ) -> Result[Optional[GuestRequest], Failure]:
-    query_proxy = Query.from_session(session, GuestRequest) \
-        .filter(GuestRequest.guestname == guestname) \
-        .filter(GuestRequest.state == state.value)
-
-    r_query = cast(
-        Result[GuestRequest, Failure],
-        safe_call(query_proxy.one)
-    )
-
-    if r_query.is_ok:
-        return Ok(r_query.unwrap())
-
-    failure = r_query.unwrap_error()
-
-    if isinstance(failure.exception, sqlalchemy.orm.exc.NoResultFound):
-        logger.warning('not in {} state anymore'.format(state.value))
-        return Ok(None)
+    try:
+        return Ok(
+            Query.from_session(session, GuestRequest)
+            .filter(GuestRequest.guestname == guestname)
+            .filter(GuestRequest.state == state.value)
+            .one_or_none()
+        )
 
-    return Error(failure)
+    except Exception as exc:
+        return Error(Failure.from_exc(
+            'failed to fetch guest request',
+            exc,
+            guestname=guestname,
+            state=state.name
+        ))
 
 
-def _get_snapshot_by_state(
+def _get_snapshot_request_by_state(
     logger: gluetool.log.ContextAdapter,
     session: sqlalchemy.orm.session.Session,
     snapshotname: str,
     state: GuestState
 ) -> Result[Optional[SnapshotRequest], Failure]:
-    query_proxy = Query.from_session(session, SnapshotRequest) \
-        .filter(SnapshotRequest.snapshotname == snapshotname) \
-        .filter(SnapshotRequest.state == state.value)
-
-    r_query = cast(
-        Result[SnapshotRequest, Failure],
-        safe_call(query_proxy.one)
-    )
-
-    if r_query.is_ok:
-        return Ok(r_query.unwrap())
-
-    failure = r_query.unwrap_error()
-
-    if isinstance(failure.exception, sqlalchemy.orm.exc.NoResultFound):
-        logger.warning('not in {} state anymore'.format(state.value))
-        return Ok(None)
+    try:
+        return Ok(
+            Query.from_session(session, SnapshotRequest)
+            .filter(SnapshotRequest.snapshotname == snapshotname)
+            .filter(SnapshotRequest.state == state.value)
+            .one_or_none()
+        )
 
-    return Error(failure)
+    except Exception as exc:
+        return Error(Failure.from_exc(
+            'failed to fetch snapshot request',
+            exc,
+            snapshotname=snapshotname,
+            state=state.name
+        ))
 
 
 def _update_guest_state(
     logger: gluetool.log.ContextAdapter,
     session: sqlalchemy.orm.session.Session,
     guestname: str,
     current_state: GuestState,
@@ -732,18 +734,28 @@
     logger: gluetool.log.ContextAdapter,
     session: sqlalchemy.orm.session.Session,
     poolname: str
 ) -> Result[PoolDriver, Failure]:
     try:
         pool_record = Query.from_session(session, Pool) \
             .filter(Pool.poolname == poolname) \
-            .one()
+            .one_or_none()
 
-    except sqlalchemy.orm.exc.NoResultFound:
-        raise Exception('no such pool "{}"'.format(poolname))
+    except Exception as exc:
+        return Error(Failure.from_exc(
+            'failed to fetch pool record',
+            exc,
+            poolname=poolname
+        ))
+
+    if not pool_record:
+        return Error(Failure(
+            'no such pool',
+            poolname=poolname
+        ))
 
     pool_driver_class = POOL_DRIVERS[pool_record.driver]
     driver = pool_driver_class(logger, poolname, json.loads(pool_record.parameters))
 
     r_sanity = driver.sanity()
 
     if r_sanity.is_error:
@@ -798,43 +810,43 @@
     session: sqlalchemy.orm.session.Session
 ) -> Result[SSHKey, Failure]:
     return _get_ssh_key(logger, session, 'artemis', 'master-key')
 
 
 def get_pool_logger(
     task_name: str,
-    root_logger: gluetool.log.ContextAdapter,
+    logger: gluetool.log.ContextAdapter,
     poolname: str
 ) -> TaskLogger:
     return TaskLogger(
-        PoolLogger(root_logger, poolname),
+        PoolLogger(logger, poolname),
         task_name
     )
 
 
 def get_guest_logger(
     task_name: str,
-    root_logger: gluetool.log.ContextAdapter,
+    logger: gluetool.log.ContextAdapter,
     guestname: str
 ) -> TaskLogger:
     return TaskLogger(
-        GuestLogger(root_logger, guestname),
+        GuestLogger(logger, guestname),
         task_name
     )
 
 
 def get_snapshot_logger(
     task_name: str,
-    root_logger: gluetool.log.ContextAdapter,
+    logger: gluetool.log.ContextAdapter,
     guestname: str,
     snapshotname: str
 ) -> TaskLogger:
     return TaskLogger(
         SnapshotLogger(
-            GuestLogger(root_logger, guestname),
+            GuestLogger(logger, guestname),
             snapshotname
         ),
         task_name
     )
 
 
 class Workspace:
@@ -910,15 +922,15 @@
 
         self.guestname = guestname
 
         if state is None:
             r = _get_guest_request(self.logger, self.session, guestname)
 
         else:
-            r = _get_guest_by_state(self.logger, self.session, guestname, state)
+            r = _get_guest_request_by_state(self.logger, self.session, guestname, state)
 
         if r.is_error:
             self.result = self.handle_failure(r, 'failed to load guest request')
             return
 
         gr = r.unwrap()
 
@@ -949,15 +961,15 @@
         """
 
         if self.result:
             return
 
         self.snapshotname = snapshotname
 
-        r = _get_snapshot_by_state(self.logger, self.session, snapshotname, state)
+        r = _get_snapshot_request_by_state(self.logger, self.session, snapshotname, state)
 
         if r.is_error:
             self.result = self.handle_failure(r, 'failed to load snapshot request')
             return
 
         sr = r.unwrap()
 
@@ -1368,19 +1380,21 @@
 
     handle_success('enter-task')
 
     try:
         resource_ids = json.loads(serialized_resource_ids)
 
     except Exception as exc:
-        return Error(Failure.from_exc(
+        failure = Failure.from_exc(
             'failed to unserialize resource IDs',
             exc,
-            resource_ids=resource_ids
-        ))
+            serialized_resource_ids=serialized_resource_ids
+        )
+
+        return handle_failure(Error(failure), 'failed to unserialize resource IDs')
 
     r_pool = _get_pool(logger, session, poolname)
 
     if r_pool.is_error:
         return handle_failure(r_pool, 'pool sanity failed')
 
     pool = r_pool.unwrap()
@@ -1392,26 +1406,39 @@
 
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('RELEASE_POOL_RESOURCES'))  # type: ignore  # Untyped decorator
 def release_pool_resources(poolname: str, resource_ids: str, guestname: Optional[str]) -> None:
     if guestname:
-        logger = get_guest_logger('release-pool-resources', root_logger, guestname)
+        logger = get_guest_logger('release-pool-resources', _ROOT_LOGGER, guestname)
 
     else:
-        logger = TaskLogger(root_logger, 'release-pool-resources')
+        logger = TaskLogger(_ROOT_LOGGER, 'release-pool-resources')
 
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_release_pool_resources,
         logger=logger,
         doer_args=(poolname, resource_ids, guestname)
     )
 
 
+def is_provisioning_tail_task(actor: Actor) -> bool:
+    """
+    Returns ``True`` if the given task is considered to be part of the provisioning "tail",
+    i.e. tasks that take care of provisioning and follow up tasks.
+    """
+
+    return actor.actor_name in (
+        acquire_guest_request.actor_name,
+        update_guest_request.actor_name,
+        route_guest_request.actor_name
+    )
+
+
 def do_handle_provisioning_chain_tail(
     logger: gluetool.log.ContextAdapter,
     db: DB,
     session: sqlalchemy.orm.session.Session,
     cancel: threading.Event,
     guestname: str,
     current_state: GuestState,
@@ -1612,15 +1639,15 @@
     return handle_failure(r_delete, 'failed to release guest')
 
 
 @dramatiq.actor(**actor_kwargs('RELEASE_GUEST_REQUEST'))  # type: ignore  # Untyped decorator
 def release_guest_request(guestname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_release_guest_request,
-        logger=get_guest_logger('release-guest-request', root_logger, guestname),
+        logger=get_guest_logger('release-guest-request', _ROOT_LOGGER, guestname),
         doer_args=(guestname,)
     )
 
 
 def do_update_guest_request(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -1726,15 +1753,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('UPDATE_GUEST_REQUEST'))  # type: ignore  # Untyped decorator
 def update_guest_request(guestname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_update_guest_request,
-        logger=get_guest_logger('update-guest-request', root_logger, guestname),
+        logger=get_guest_logger('update-guest-request', _ROOT_LOGGER, guestname),
         doer_args=(guestname,)
     )
 
 
 def do_acquire_guest_request(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -1841,15 +1868,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('ACQUIRE_GUEST_REQUEST'))  # type: ignore  # Untyped decorator
 def acquire_guest_request(guestname: str, poolname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_acquire_guest_request,
-        logger=get_guest_logger('acquire-guest-request', root_logger, guestname),
+        logger=get_guest_logger('acquire-guest-request', _ROOT_LOGGER, guestname),
         doer_args=(guestname, poolname)
     )
 
 
 def do_route_guest_request(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -1942,15 +1969,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('ROUTE_GUEST_REQUEST'))  # type: ignore  # Untyped decorator
 def route_guest_request(guestname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_route_guest_request,
-        logger=get_guest_logger('route-guest-request', root_logger, guestname),
+        logger=get_guest_logger('route-guest-request', _ROOT_LOGGER, guestname),
         doer_args=(guestname,)
     )
 
 
 def do_release_snapshot_request(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2016,15 +2043,15 @@
     return handle_failure(r_delete, 'failed to release snapshot')
 
 
 @dramatiq.actor(**actor_kwargs('RELEASE_SNAPSHOT_REQUEST'))  # type: ignore  # Untyped decorator
 def release_snapshot_request(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_release_snapshot_request,
-        logger=get_snapshot_logger('release-snapshot', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('release-snapshot', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_create_snapshot_start_guest(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2090,15 +2117,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('CREATE_SNAPSHOT_START_GUEST_REQUEST'))  # type: ignore  # Untyped decorator
 def create_snapshot_start_guest(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_create_snapshot_start_guest,
-        logger=get_snapshot_logger('create-snapshot-start-guest', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('create-snapshot-start-guest', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_update_snapshot(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2205,15 +2232,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('UPDATE_SNAPSHOT_REQUEST'))  # type: ignore  # Untyped decorator
 def update_snapshot(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_update_snapshot,
-        logger=get_snapshot_logger('update-snapshot', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('update-snapshot', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_create_snapshot_create(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2324,15 +2351,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('CREATE_SNAPSHOT_CREATE_REQUEST'))  # type: ignore  # Untyped decorator
 def create_snapshot_create(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_create_snapshot_create,
-        logger=get_snapshot_logger('create-snapshot-create', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('create-snapshot-create', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_create_snapshot_stop_guest(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2405,15 +2432,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('CREATE_SNAPSHOT_STOP_GUEST_REQUEST'))  # type: ignore  # Untyped decorator
 def create_snapshot_stop_guest(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_create_snapshot_stop_guest,
-        logger=get_snapshot_logger('create-snapshot-stop-guest', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('create-snapshot-stop-guest', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_create_snapshot(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2494,15 +2521,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('CREATE_SNAPSHOT_REQUEST'))  # type: ignore  # Untyped decorator
 def create_snapshot(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore  # Argument 1 has incompatible type
         do_create_snapshot,
-        logger=get_snapshot_logger('create-snapshot', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('create-snapshot', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_route_snapshot_request(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2553,15 +2580,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('ROUTE_SNAPSHOT_REQUEST'))  # type: ignore  # Untyped decorator
 def route_snapshot_request(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore # Argument 1 has incompatible type
         do_route_snapshot_request,
-        logger=get_snapshot_logger('route-snapshot', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('route-snapshot', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_restore_snapshot_request(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2622,15 +2649,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('RESTORE_SNAPSHOT_REQUEST'))  # type: ignore  # Untyped decorator
 def restore_snapshot_request(guestname: str, snapshotname: str) -> None:
     task_core(  # type: ignore # Argument 1 has incompatible type
         do_restore_snapshot_request,
-        logger=get_snapshot_logger('restore-snapshot', root_logger, guestname, snapshotname),
+        logger=get_snapshot_logger('restore-snapshot', _ROOT_LOGGER, guestname, snapshotname),
         doer_args=(guestname, snapshotname)
     )
 
 
 def do_refresh_pool_resources_metrics(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2670,15 +2697,15 @@
     return SUCCESS
 
 
 @dramatiq.actor(**actor_kwargs('REFRESH_POOL_RESOURCES_METRICS'))  # type: ignore  # Untyped decorator
 def refresh_pool_resources_metrics(poolname: str) -> None:
     task_core(  # type: ignore # Argument 1 has incompatible type
         do_refresh_pool_resources_metrics,
-        logger=get_pool_logger('refresh-pool-resources-metrics', root_logger, poolname),
+        logger=get_pool_logger('refresh-pool-resources-metrics', _ROOT_LOGGER, poolname),
         doer_args=(poolname,)
     )
 
 
 def do_refresh_pool_resources_metrics_dispatcher(
     logger: gluetool.log.ContextAdapter,
     db: DB,
@@ -2691,17 +2718,17 @@
         task='refresh-pool-metrics-dispatcher'
     )
 
     handle_success('enter-task')
 
     logger.info('scheduling pool metrics refresh')
 
-    for pool in get_pools(root_logger, session):
+    for pool in get_pools(_ROOT_LOGGER, session):
         dispatch_task(
-            get_pool_logger('refresh-pool-resources-metrics-dispatcher', root_logger, pool.poolname),
+            get_pool_logger('refresh-pool-resources-metrics-dispatcher', _ROOT_LOGGER, pool.poolname),
             refresh_pool_resources_metrics,
             pool.poolname
         )
 
     return SUCCESS
 
 
@@ -2721,9 +2748,9 @@
 
     We don't care about rescheduling or retries - this task would be executed again very soon, exponential
     retries would make the metrics more outdated.
     """
 
     task_core(  # type: ignore # Argument 1 has incompatible type
         do_refresh_pool_resources_metrics_dispatcher,
-        logger=TaskLogger(root_logger, 'refresh-pool-resources-dispatcher')
+        logger=TaskLogger(_ROOT_LOGGER, 'refresh-pool-resources-dispatcher')
     )
```

### Comparing `tft-artemis-0.0.8/setup.py` & `tft-artemis-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 install_requires = \
 ['alembic>=1.4.2,<2.0.0',
  'ansible-vault>=1.2.0,<2.0.0',
  'awscli>=1.16.298,<2.0.0',
  'beaker-client>=27.0,<28.0',
  'beautifulsoup4>=4.6.3,<5.0.0',
- 'dramatiq[rabbitmq,watch]>=1.7.0,<2.0.0',
+ 'dramatiq[watch,rabbitmq]>=1.7.0,<2.0.0',
  'gluetool>=1.24,<2.0',
  'gunicorn==19.9.0',
  'jinja2-ansible-filters>=1.3.0,<2.0.0',
  'molten>=1.0.1,<2.0.0',
  'periodiq>=0.12.1,<0.13.0',
  'psycopg2==2.8.4',
  'python-openstackclient>=5.0.0,<6.0.0',
@@ -33,15 +33,15 @@
                      'artemis-dispatcher = tft.artemis.dispatcher:main',
                      'artemis-init-postgres-schema = '
                      'tft.artemis.db:init_postgres',
                      'artemis-init-sqlite-schema = tft.artemis.db:init_sqlite']}
 
 setup_kwargs = {
     'name': 'tft-artemis',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Artemis is a machine provisioning service. Its goal is to provision a machine - using a set of preconfigured providers as backends - which would satisfy the given hardware and software requirements.',
     'long_description': None,
     'author': 'Milos Prchlik',
     'author_email': 'mprchlik@redhat.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tft-artemis-0.0.8/PKG-INFO` & `tft-artemis-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tft-artemis
-Version: 0.0.8
+Version: 0.0.9
 Summary: Artemis is a machine provisioning service. Its goal is to provision a machine - using a set of preconfigured providers as backends - which would satisfy the given hardware and software requirements.
 License: Apache-2.0
 Author: Milos Prchlik
 Author-email: mprchlik@redhat.com
 Requires-Python: >=3.7,<3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: alembic (>=1.4.2,<2.0.0)
 Requires-Dist: ansible-vault (>=1.2.0,<2.0.0)
 Requires-Dist: awscli (>=1.16.298,<2.0.0)
 Requires-Dist: beaker-client (>=27.0,<28.0)
 Requires-Dist: beautifulsoup4 (>=4.6.3,<5.0.0)
-Requires-Dist: dramatiq[rabbitmq,watch] (>=1.7.0,<2.0.0)
+Requires-Dist: dramatiq[watch,rabbitmq] (>=1.7.0,<2.0.0)
 Requires-Dist: gluetool (>=1.24,<2.0)
 Requires-Dist: gunicorn (==19.9.0)
 Requires-Dist: jinja2-ansible-filters (>=1.3.0,<2.0.0)
 Requires-Dist: molten (>=1.0.1,<2.0.0)
 Requires-Dist: periodiq (>=0.12.1,<0.13.0)
 Requires-Dist: psycopg2 (==2.8.4)
 Requires-Dist: python-openstackclient (>=5.0.0,<6.0.0)
```

