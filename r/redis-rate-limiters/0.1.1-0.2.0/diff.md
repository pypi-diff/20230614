# Comparing `tmp/redis_rate_limiters-0.1.1.tar.gz` & `tmp/redis_rate_limiters-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_rate_limiters-0.1.1.tar", max compression
+gzip compressed data, was "redis_rate_limiters-0.2.0.tar", max compression
```

## Comparing `redis_rate_limiters-0.1.1.tar` & `redis_rate_limiters-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1652 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/LICENSE
--rw-r--r--   0        0        0     4752 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/README.md
--rw-r--r--   0        0        0      294 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/__init__.py
--rw-r--r--   0        0        0      727 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/base.py
--rw-r--r--   0        0        0      143 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/py.typed
--rw-r--r--   0        0        0     1544 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/semaphore.lua
--rw-r--r--   0        0        0     4362 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/semaphore.py
--rw-r--r--   0        0        0     2349 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/token_bucket.lua
--rw-r--r--   0        0        0     3523 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/limiters/token_bucket.py
--rw-r--r--   0        0        0     3065 2023-05-23 14:45:46.167425 redis_rate_limiters-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6008 1970-01-01 00:00:00.000000 redis_rate_limiters-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1652 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5218 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/README.md
+-rw-r--r--   0        0        0      294 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/__init__.py
+-rw-r--r--   0        0        0     1593 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/base.py
+-rw-r--r--   0        0        0      143 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/py.typed
+-rw-r--r--   0        0        0     1544 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/semaphore.lua
+-rw-r--r--   0        0        0     4434 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/semaphore.py
+-rw-r--r--   0        0        0     2349 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/token_bucket.lua
+-rw-r--r--   0        0        0     3328 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/token_bucket.py
+-rw-r--r--   0        0        0     3155 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 redis_rate_limiters-0.2.0/PKG-INFO
```

### Comparing `redis_rate_limiters-0.1.1/LICENSE` & `redis_rate_limiters-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.1.1/README.md` & `redis_rate_limiters-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Redis rate limiters
 
-A library for regulating traffic with respect to concurrency or time.
-It sync and async context managers for a [semaphore](#semaphore)- and a [token bucket](#token-bucket)
-implementation.
-
-The rate limiting implementations are distributed, using Redis,
-and leverages Lua scripts to greatly improve performance and simplify the code. Lua scripts
-run on the Redis server, and make each implementation fully atomic.
+A library which regulates traffic, with respect to concurrency or time.
+It implements sync and async context managers for a [semaphore](#semaphore)- and a [token bucket](#token-bucket)-implementation.
 
-Both implementations are compatible for use with redis-clusters.
+The rate limiters are distributed, using Redis, and leverages Lua scripts to
+improve performance and simplify the code. Lua scripts
+run on Redis, and make each implementation fully atomic, while
+also reducing the number of round-trips required.
+
+Use is supported for standalone redis instances, and clusters.
 We currently only support Python 3.11, but can add support for older versions if needed.
 
 ## Installation
 
 ```
 pip install redis-rate-limiters
 ```
@@ -29,23 +29,25 @@
 
 Here's how you might use the async version:
 
 ```python
 import asyncio
 
 from httpx import AsyncClient
+from redis.asyncio import Redis
 
 from limiters import AsyncSemaphore
 
 
 limiter = AsyncSemaphore(
     name="foo",    # name of the resource you are limiting traffic for
     capacity=5,    # allow 5 concurrent requests
     max_sleep=30,  # raise an error if it takes longer than 30 seconds to acquire the semaphore
-    expiry=30      # set expiry on the semaphore keys in Redis to prevent deadlocks
+    expiry=30,      # set expiry on the semaphore keys in Redis to prevent deadlocks
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 async def get_foo():
     async with AsyncClient() as client:
         async with limiter:
             client.get(...)
 
@@ -56,23 +58,25 @@
     )
 ```
 
 and here is how you might use the sync version:
 
 ```python
 import requests
+from redis import Redis
 
 from limiters import SyncSemaphore
 
 
 limiter = SyncSemaphore(
     name="foo",
     capacity=5,
     max_sleep=30,
-    expiry=30
+    expiry=30,
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 def main():
     with limiter:
         requests.get(...)
 ```
 
@@ -85,24 +89,26 @@
 
 Here's how you might use the async version:
 
 ```python
 import asyncio
 
 from httpx import AsyncClient
+from redis.asyncio import Redis
 
 from limiters import AsyncTokenBucket
 
 
 limiter = AsyncTokenBucket(
     name="foo",          # name of the resource you are limiting traffic for
     capacity=5,          # hold up to 5 tokens
     refill_frequency=1,  # add tokens every second
     refill_amount=1,     # add 1 token when refilling
     max_sleep=30,        # raise an error there are no free tokens for 30 seconds
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 async def get_foo():
     async with AsyncClient() as client:
         async with limiter:
             client.get(...)
 
@@ -112,24 +118,26 @@
     )
 ```
 
 and here is how you might use the sync version:
 
 ```python
 import requests
+from redis import Redis
 
 from limiters import SyncTokenBucket
 
 
 limiter = SyncTokenBucket(
     name="foo",
     capacity=5,
     refill_frequency=1,
     refill_amount=1,
     max_sleep=30,
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 def main():
     with limiter:
         requests.get(...)
 ```
 
@@ -161,15 +169,17 @@
 ## Contributing
 
 Contributions are very welcome. Here's how to get started:
 
 - Set up a Python 3.11+ venv, and `pip install poetry`
 - Install dependencies with `poetry install`
 - Run `pre-commit install` to set up pre-commit
-- Run `docker compose up` to run Redis (or run Redis for tests some other way)
+- Install [just](https://just.systems/man/en/) and run `just setup`
+  If you prefer not to install just, just take a look at the justfile and
+  run the commands yourself.
 - Make your code changes, with tests
 - Commit your changes and open a PR
 
 ## Publishing a new version
 
 To publish a new version:
```

### Comparing `redis_rate_limiters-0.1.1/limiters/semaphore.lua` & `redis_rate_limiters-0.2.0/limiters/semaphore.lua`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.1.1/limiters/semaphore.py` & `redis_rate_limiters-0.2.0/limiters/semaphore.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import logging
 from datetime import datetime
 from types import TracebackType
-from typing import TYPE_CHECKING, ClassVar
+from typing import ClassVar
 
-from pydantic import Field
-from redis import Redis as SyncRedis
-from redis.asyncio import Redis as AsyncRedis
-from redis.commands.core import AsyncScript, Script
+from pydantic import BaseModel, Field
+from redis.asyncio.client import Pipeline
+from redis.asyncio.cluster import ClusterPipeline
 
 from limiters import MaxSleepExceededError
-from limiters.base import LuaScriptBase
+from limiters.base import AsyncLuaScriptBase, SyncLuaScriptBase
 
 logger = logging.getLogger(__name__)
 
 
-class SemaphoreBase(LuaScriptBase):
+class SemaphoreBase(BaseModel):
     name: str
     capacity: int = Field(gt=0)
     max_sleep: float = Field(ge=0, default=0.0)
     expiry: int | None = None
 
-    script_name: ClassVar[str] = 'semaphore.lua'
-
     @property
     def key(self) -> str:
         """Key to use for the Semaphore list."""
         return f'{{limiter}}:semaphore:{self.name}'
 
     @property
     def exists(self) -> str:
         """Key to use when checking if the Semaphore list has been created or not."""
         return f'{{limiter}}:semaphore:{self.name}-exists'
 
     def __str__(self) -> str:
         return f'Semaphore instance for queue {self.key}'
 
 
-class SyncSemaphore(SemaphoreBase):
-    if TYPE_CHECKING:
-        connection: SyncRedis[str]
-        script: Script
+class SyncSemaphore(SemaphoreBase, SyncLuaScriptBase):
+    script_name: ClassVar[str] = 'semaphore.lua'
 
     def __enter__(self) -> None:
         """
         Call the semaphore Lua script to create a semaphore, then call BLPOP to acquire it.
         """
         # Retrieve timestamp for when to wake up from Redis
         semaphore_created: bool = self.script(
@@ -81,18 +76,16 @@
             pipeline.execute()
         else:
             self.connection.lpush(self.key, 1)
 
         logger.debug('Released semaphore')
 
 
-class AsyncSemaphore(SemaphoreBase):
-    if TYPE_CHECKING:
-        connection: AsyncRedis[str]
-        script: AsyncScript
+class AsyncSemaphore(SemaphoreBase, AsyncLuaScriptBase):
+    script_name: ClassVar[str] = 'semaphore.lua'
 
     async def __aenter__(self) -> None:
         """
         Call the semaphore Lua script to create a semaphore, then call BLPOP to acquire it.
         """
         # Retrieve timestamp for when to wake up from Redis
 
@@ -101,33 +94,33 @@
             args=[self.capacity],
         ):
             logger.info('Created new semaphore `%s` with capacity %s', self.name, self.capacity)
         else:
             logger.debug('Skipped creating semaphore, since one exists')
 
         start = datetime.now()
-        await self.connection.blpop(self.key, self.max_sleep)
+        await self.connection.blpop(self.key, self.max_sleep)  # type: ignore[union-attr]
 
         # Raise an exception if we waited too long
         if 0.0 < self.max_sleep < (datetime.now() - start).total_seconds():
             raise MaxSleepExceededError(f'Max sleep ({self.max_sleep}s) exceeded waiting for Semaphore')
 
         logger.debug('Acquired semaphore %s', self.name)
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         if self.expiry:
-            pipeline = self.connection.pipeline()
+            pipeline: Pipeline[str] | ClusterPipeline[str] = self.connection.pipeline()
             # Return capacity to the semaphore
-            pipeline.lpush(self.key, 1)
+            pipeline.lpush(self.key, 1)  # type: ignore[union-attr]
             # Set expiry to prevent deadlocks
-            pipeline.expire(self.key, self.expiry)
-            pipeline.expire(self.exists, self.expiry)
+            pipeline.expire(self.key, self.expiry)  # type: ignore[union-attr]
+            pipeline.expire(self.exists, self.expiry)  # type: ignore[union-attr]
             await pipeline.execute()
         else:
-            await self.connection.lpush(self.key, 1)
+            await self.connection.lpush(self.key, 1)  # type: ignore[union-attr]
 
         logger.debug('Released semaphore')
```

### Comparing `redis_rate_limiters-0.1.1/limiters/token_bucket.lua` & `redis_rate_limiters-0.2.0/limiters/token_bucket.lua`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.1.1/limiters/token_bucket.py` & `redis_rate_limiters-0.2.0/limiters/token_bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import asyncio
 import logging
 import time
 from datetime import datetime
 from types import TracebackType
-from typing import TYPE_CHECKING, ClassVar
+from typing import ClassVar
 
-from pydantic import Field
-from redis import Redis as SyncRedis
-from redis.asyncio import Redis as AsyncRedis
-from redis.commands.core import AsyncScript, Script
+from pydantic import BaseModel, Field
 
 from limiters import MaxSleepExceededError
-from limiters.base import LuaScriptBase
+from limiters.base import AsyncLuaScriptBase, SyncLuaScriptBase
 
 logger = logging.getLogger(__name__)
 
 
-class TokenBucketBase(LuaScriptBase):
+class TokenBucketBase(BaseModel):
     name: str
     capacity: int = Field(gt=0)
     refill_frequency: float = Field(gt=0)
     refill_amount: int = Field(gt=0)
     max_sleep: float = Field(ge=0, default=0.0)
 
-    script_name: ClassVar[str] = 'token_bucket.lua'
-
     def parse_timestamp(self, timestamp: int) -> float:
         # Parse to datetime
         wake_up_time = datetime.fromtimestamp(timestamp / 1000)
 
         # Establish the current time, with a very small buffer for processing time
         now = datetime.now()
 
@@ -53,18 +48,16 @@
     def key(self) -> str:
         return f'{{limiter}}:token-bucket:{self.name}'
 
     def __str__(self) -> str:
         return f'Token bucket instance for queue {self.key}'
 
 
-class SyncTokenBucket(TokenBucketBase):
-    if TYPE_CHECKING:
-        connection: SyncRedis[str]
-        script: Script
+class SyncTokenBucket(TokenBucketBase, SyncLuaScriptBase):
+    script_name: ClassVar[str] = 'token_bucket.lua'
 
     def __enter__(self) -> None:
         """
         Call the token bucket Lua script, receive a datetime for
         when to wake up, then sleep up until that point in time.
         """
         # Retrieve timestamp for when to wake up from Redis
@@ -84,18 +77,16 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         return
 
 
-class AsyncTokenBucket(TokenBucketBase):
-    if TYPE_CHECKING:
-        connection: AsyncRedis[str]
-        script: AsyncScript
+class AsyncTokenBucket(TokenBucketBase, AsyncLuaScriptBase):
+    script_name: ClassVar[str] = 'token_bucket.lua'
 
     async def __aenter__(self) -> None:
         """
         Call the token bucket Lua script, receive a datetime for
         when to wake up, then sleep up until that point in time.
         """
         # Retrieve timestamp for when to wake up from Redis
```

### Comparing `redis_rate_limiters-0.1.1/pyproject.toml` & `redis_rate_limiters-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-rate-limiters"
-version = "0.1.1"
+version = "0.2.0"
 description = "Distributed rate limiters"
 license = "BSD-4-Clause"
 authors = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
 readme = "README.md"
 homepage = "https://github.com/otovo/redis-rate-limiters"
 repository = "https://github.com/otovo/redis-rate-limiters"
 keywords = [
@@ -46,20 +46,23 @@
 coverage = "^7"
 pytest = "^7"
 pytest-asyncio = "*"
 pytest-mock = "*"
 pytest-randomly = "*"
 pytest-socket = "*"
 
+[tool.poetry.group.dev.dependencies]
+types-redis = "^4.5.5.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-addopts = "--allow-hosts=127.0.0.1,::1"
+addopts = "--allow-hosts=127.0.0.1,::1,10.5.0.2,10.5.0.3,10.5.0.4"
 asyncio_mode = "auto"
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 quiet = true
 preview = true
```

### Comparing `redis_rate_limiters-0.1.1/PKG-INFO` & `redis_rate_limiters-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-rate-limiters
-Version: 0.1.1
+Version: 0.2.0
 Summary: Distributed rate limiters
 Home-page: https://github.com/otovo/redis-rate-limiters
 License: BSD-4-Clause
 Keywords: async,sync,rate,limiting,limiters
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
 Requires-Python: >=3.11,<4.0
@@ -26,23 +26,23 @@
 Requires-Dist: pydantic (>1)
 Requires-Dist: redis (>4.2)
 Project-URL: Repository, https://github.com/otovo/redis-rate-limiters
 Description-Content-Type: text/markdown
 
 # Redis rate limiters
 
-A library for regulating traffic with respect to concurrency or time.
-It sync and async context managers for a [semaphore](#semaphore)- and a [token bucket](#token-bucket)
-implementation.
-
-The rate limiting implementations are distributed, using Redis,
-and leverages Lua scripts to greatly improve performance and simplify the code. Lua scripts
-run on the Redis server, and make each implementation fully atomic.
+A library which regulates traffic, with respect to concurrency or time.
+It implements sync and async context managers for a [semaphore](#semaphore)- and a [token bucket](#token-bucket)-implementation.
 
-Both implementations are compatible for use with redis-clusters.
+The rate limiters are distributed, using Redis, and leverages Lua scripts to
+improve performance and simplify the code. Lua scripts
+run on Redis, and make each implementation fully atomic, while
+also reducing the number of round-trips required.
+
+Use is supported for standalone redis instances, and clusters.
 We currently only support Python 3.11, but can add support for older versions if needed.
 
 ## Installation
 
 ```
 pip install redis-rate-limiters
 ```
@@ -59,23 +59,25 @@
 
 Here's how you might use the async version:
 
 ```python
 import asyncio
 
 from httpx import AsyncClient
+from redis.asyncio import Redis
 
 from limiters import AsyncSemaphore
 
 
 limiter = AsyncSemaphore(
     name="foo",    # name of the resource you are limiting traffic for
     capacity=5,    # allow 5 concurrent requests
     max_sleep=30,  # raise an error if it takes longer than 30 seconds to acquire the semaphore
-    expiry=30      # set expiry on the semaphore keys in Redis to prevent deadlocks
+    expiry=30,      # set expiry on the semaphore keys in Redis to prevent deadlocks
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 async def get_foo():
     async with AsyncClient() as client:
         async with limiter:
             client.get(...)
 
@@ -86,23 +88,25 @@
     )
 ```
 
 and here is how you might use the sync version:
 
 ```python
 import requests
+from redis import Redis
 
 from limiters import SyncSemaphore
 
 
 limiter = SyncSemaphore(
     name="foo",
     capacity=5,
     max_sleep=30,
-    expiry=30
+    expiry=30,
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 def main():
     with limiter:
         requests.get(...)
 ```
 
@@ -115,24 +119,26 @@
 
 Here's how you might use the async version:
 
 ```python
 import asyncio
 
 from httpx import AsyncClient
+from redis.asyncio import Redis
 
 from limiters import AsyncTokenBucket
 
 
 limiter = AsyncTokenBucket(
     name="foo",          # name of the resource you are limiting traffic for
     capacity=5,          # hold up to 5 tokens
     refill_frequency=1,  # add tokens every second
     refill_amount=1,     # add 1 token when refilling
     max_sleep=30,        # raise an error there are no free tokens for 30 seconds
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 async def get_foo():
     async with AsyncClient() as client:
         async with limiter:
             client.get(...)
 
@@ -142,24 +148,26 @@
     )
 ```
 
 and here is how you might use the sync version:
 
 ```python
 import requests
+from redis import Redis
 
 from limiters import SyncTokenBucket
 
 
 limiter = SyncTokenBucket(
     name="foo",
     capacity=5,
     refill_frequency=1,
     refill_amount=1,
     max_sleep=30,
+    connection=Redis.from_url("redis://localhost:6379"),
 )
 
 def main():
     with limiter:
         requests.get(...)
 ```
 
@@ -191,15 +199,17 @@
 ## Contributing
 
 Contributions are very welcome. Here's how to get started:
 
 - Set up a Python 3.11+ venv, and `pip install poetry`
 - Install dependencies with `poetry install`
 - Run `pre-commit install` to set up pre-commit
-- Run `docker compose up` to run Redis (or run Redis for tests some other way)
+- Install [just](https://just.systems/man/en/) and run `just setup`
+  If you prefer not to install just, just take a look at the justfile and
+  run the commands yourself.
 - Make your code changes, with tests
 - Commit your changes and open a PR
 
 ## Publishing a new version
 
 To publish a new version:
```

